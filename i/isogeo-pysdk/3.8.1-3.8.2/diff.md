# Comparing `tmp/isogeo-pysdk-3.8.1.tar.gz` & `tmp/isogeo-pysdk-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isogeo-pysdk-3.8.1.tar", last modified: Fri Apr 14 15:35:04 2023, max compression
+gzip compressed data, was "isogeo-pysdk-3.8.2.tar", last modified: Thu May  4 17:57:43 2023, max compression
```

## Comparing `isogeo-pysdk-3.8.1.tar` & `isogeo-pysdk-3.8.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/
--rw-rw-rw-   0        0        0     7817 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/LICENSE
--rw-rw-rw-   0        0        0     4149 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2878 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.062095 isogeo-pysdk-3.8.1/isogeo_pysdk/
--rw-rw-rw-   0        0        0      714 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/__about__.py
--rw-rw-rw-   0        0        0      738 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.077716 isogeo-pysdk-3.8.1/isogeo_pysdk/api/
--rw-rw-rw-   0        0        0     1508 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/__init__.py
--rw-rw-rw-   0        0        0     5991 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_about.py
--rw-rw-rw-   0        0        0     5945 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_account.py
--rw-rw-rw-   0        0        0    19343 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_application.py
--rw-rw-rw-   0        0        0    22863 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_catalog.py
--rw-rw-rw-   0        0        0     8245 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_condition.py
--rw-rw-rw-   0        0        0     7558 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_conformity.py
--rw-rw-rw-   0        0        0    16653 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_contact.py
--rw-rw-rw-   0        0        0    14009 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_coordinate_systems.py
--rw-rw-rw-   0        0        0    13598 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_datasource.py
--rw-rw-rw-   0        0        0     2819 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_directives.py
--rw-rw-rw-   0        0        0    10559 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_event.py
--rw-rw-rw-   0        0        0    19108 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_feature_attributes.py
--rw-rw-rw-   0        0        0    12852 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_format.py
--rw-rw-rw-   0        0        0    10496 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_invitation.py
--rw-rw-rw-   0        0        0    38458 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_keyword.py
--rw-rw-rw-   0        0        0    15256 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_license.py
--rw-rw-rw-   0        0        0    11164 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_limitation.py
--rw-rw-rw-   0        0        0    25144 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_link.py
--rw-rw-rw-   0        0        0    15535 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata.py
--rw-rw-rw-   0        0        0     6058 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata_bulk.py
--rw-rw-rw-   0        0        0    17200 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_search.py
--rw-rw-rw-   0        0        0    16317 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service.py
--rw-rw-rw-   0        0        0    17176 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_layers.py
--rw-rw-rw-   0        0        0    18310 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_operations.py
--rw-rw-rw-   0        0        0    23781 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_share.py
--rw-rw-rw-   0        0        0    14650 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_specification.py
--rw-rw-rw-   0        0        0     4307 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_thesaurus.py
--rw-rw-rw-   0        0        0    12937 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_user.py
--rw-rw-rw-   0        0        0    18202 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_workgroup.py
--rw-rw-rw-   0        0        0     1605 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api_hooks.py
--rw-rw-rw-   0        0        0    18711 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/checker.py
--rw-rw-rw-   0        0        0     2255 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/decorators.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.093344 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/
--rw-rw-rw-   0        0        0     1424 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/application_types.py
--rw-rw-rw-   0        0        0     2130 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_actions.py
--rw-rw-rw-   0        0        0     2315 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_ignore_reasons.py
--rw-rw-rw-   0        0        0     2422 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_targets.py
--rw-rw-rw-   0        0        0     2861 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/catalog_statistics_tags.py
--rw-rw-rw-   0        0        0     2349 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_roles.py
--rw-rw-rw-   0        0        0     2082 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_types.py
--rw-rw-rw-   0        0        0     2066 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/edition_profiles.py
--rw-rw-rw-   0        0        0     2144 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/event_kinds.py
--rw-rw-rw-   0        0        0     2204 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/keyword_casing.py
--rw-rw-rw-   0        0        0     2591 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_restrictions.py
--rw-rw-rw-   0        0        0     2067 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_types.py
--rw-rw-rw-   0        0        0     2058 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_actions.py
--rw-rw-rw-   0        0        0     2470 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_kinds.py
--rw-rw-rw-   0        0        0     2026 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_types.py
--rw-rw-rw-   0        0        0     2819 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_subresources.py
--rw-rw-rw-   0        0        0     2518 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_types.py
--rw-rw-rw-   0        0        0     2466 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/search_filters_georelations.py
--rw-rw-rw-   0        0        0     2128 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/service_layer_types.py
--rw-rw-rw-   0        0        0     2215 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/session_status.py
--rw-rw-rw-   0        0        0     2125 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/share_types.py
--rw-rw-rw-   0        0        0     1998 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/user_roles.py
--rw-rw-rw-   0        0        0     3054 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/workgroup_statistics_tags.py
--rw-rw-rw-   0        0        0     1001 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/exceptions.py
--rw-rw-rw-   0        0        0    19870 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/isogeo.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.108965 isogeo-pysdk-3.8.1/isogeo_pysdk/models/
--rw-rw-rw-   0        0        0     1748 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/__init__.py
--rw-rw-rw-   0        0        0    16184 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/application.py
--rw-rw-rw-   0        0        0     4260 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_report.py
--rw-rw-rw-   0        0        0     6262 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_request.py
--rw-rw-rw-   0        0        0    10991 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/catalog.py
--rw-rw-rw-   0        0        0     7922 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/condition.py
--rw-rw-rw-   0        0        0     7812 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/conformity.py
--rw-rw-rw-   0        0        0    15867 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/contact.py
--rw-rw-rw-   0        0        0     6213 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/coordinates_system.py
--rw-rw-rw-   0        0        0    10550 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/datasource.py
--rw-rw-rw-   0        0        0     4238 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/directive.py
--rw-rw-rw-   0        0        0     7486 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/event.py
--rw-rw-rw-   0        0        0    17324 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/feature_attributes.py
--rw-rw-rw-   0        0        0     8175 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/format.py
--rw-rw-rw-   0        0        0     9348 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/invitation.py
--rw-rw-rw-   0        0        0     9533 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword.py
--rw-rw-rw-   0        0        0     5635 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword_search.py
--rw-rw-rw-   0        0        0     9004 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/license.py
--rw-rw-rw-   0        0        0     9250 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/limitation.py
--rw-rw-rw-   0        0        0    10510 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/link.py
--rw-rw-rw-   0        0        0    43405 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata.py
--rw-rw-rw-   0        0        0     7856 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata_search.py
--rw-rw-rw-   0        0        0    12874 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_layer.py
--rw-rw-rw-   0        0        0     8952 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_operation.py
--rw-rw-rw-   0        0        0    15186 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/share.py
--rw-rw-rw-   0        0        0    10004 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/specification.py
--rw-rw-rw-   0        0        0     6780 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/thesaurus.py
--rw-rw-rw-   0        0        0    11239 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/user.py
--rw-rw-rw-   0        0        0    18470 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/workgroup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.124592 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/
--rw-rw-rw-   0        0        0        0 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/__init__.py
--rw-rw-rw-   0        0        0     4258 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/attributes_frequency.py
--rw-rw-rw-   0        0        0     2563 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/download_batch_hosted_data.py
--rw-rw-rw-   0        0        0     2623 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/export_batch_xml19139_sync.py
--rw-rw-rw-   0        0        0     2830 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/get_OpenCatalog.py
--rw-rw-rw-   0        0        0     2293 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/latest_md_modified.py
--rw-rw-rw-   0        0        0     6737 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/related_links.py
--rw-rw-rw-   0        0        0     5378 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/results_parser.py
--rw-rw-rw-   0        0        0     2741 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/search.py
--rw-rw-rw-   0        0        0     3554 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/spatial_search.py
--rw-rw-rw-   0        0        0     6106 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_read.py
--rw-rw-rw-   0        0        0     7670 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_rw.py
--rw-rw-rw-   0        0        0     7790 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/translator.py
--rw-rw-rw-   0        0        0      838 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/type_hints_custom.py
--rw-rw-rw-   0        0        0    40710 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.062095 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/
--rw-rw-rw-   0        0        0     4149 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4886 2023-04-14 15:35:04.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      965 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2378 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/tests/
--rw-rw-rw-   0        0        0     3224 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_about.py
--rw-rw-rw-   0        0        0     4808 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_account.py
--rw-rw-rw-   0        0        0    14716 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_applications.py
--rw-rw-rw-   0        0        0     6528 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7000 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_bulks.py
--rw-rw-rw-   0        0        0    13494 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_catalogs.py
--rw-rw-rw-   0        0        0    17511 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_checker.py
--rw-rw-rw-   0        0        0     8878 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_conditions.py
--rw-rw-rw-   0        0        0     6847 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_conformity.py
--rw-rw-rw-   0        0        0    12329 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_contacts.py
--rw-rw-rw-   0        0        0     9587 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_coordinate_systems.py
--rw-rw-rw-   0        0        0    11990 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_datasources.py
--rw-rw-rw-   0        0        0     5479 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_directives.py
--rw-rw-rw-   0        0        0    10121 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_enums.py
--rw-rw-rw-   0        0        0    10212 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_events.py
--rw-rw-rw-   0        0        0    16151 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_feature_attributes.py
--rw-rw-rw-   0        0        0     7002 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_formats.py
--rw-rw-rw-   0        0        0    33394 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_keywords.py
--rw-rw-rw-   0        0        0    13605 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_licenses.py
--rw-rw-rw-   0        0        0    10637 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_limitations.py
--rw-rw-rw-   0        0        0    10744 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_links.py
--rw-rw-rw-   0        0        0    10964 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_metadatas_noGeo.py
--rw-rw-rw-   0        0        0    10929 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_metadatas_vector.py
--rw-rw-rw-   0        0        0    13188 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_search.py
--rw-rw-rw-   0        0        0    16057 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_service_layers.py
--rw-rw-rw-   0        0        0    11398 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_service_operations.py
--rw-rw-rw-   0        0        0    14385 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_shares.py
--rw-rw-rw-   0        0        0    14313 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_specifications.py
--rw-rw-rw-   0        0        0     5781 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_thesauri.py
--rw-rw-rw-   0        0        0     3867 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_token.py
--rw-rw-rw-   0        0        0     5457 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_translator.py
--rw-rw-rw-   0        0        0     4972 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_users.py
--rw-rw-rw-   0        0        0    17075 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils.py
--rw-rw-rw-   0        0        0     9312 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils_credentials.py
--rw-rw-rw-   0        0        0     5532 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils_uuid.py
--rw-rw-rw-   0        0        0    12714 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_workgroups.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.541145 isogeo-pysdk-3.8.2/
+-rw-rw-rw-   0        0        0     7817 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/LICENSE
+-rw-rw-rw-   0        0        0     4149 2023-05-04 17:57:43.541145 isogeo-pysdk-3.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2878 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.413874 isogeo-pysdk-3.8.2/isogeo_pysdk/
+-rw-rw-rw-   0        0        0      714 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/__about__.py
+-rw-rw-rw-   0        0        0      738 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.442568 isogeo-pysdk-3.8.2/isogeo_pysdk/api/
+-rw-rw-rw-   0        0        0     1508 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/__init__.py
+-rw-rw-rw-   0        0        0     5991 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_about.py
+-rw-rw-rw-   0        0        0     5945 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_account.py
+-rw-rw-rw-   0        0        0    19343 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_application.py
+-rw-rw-rw-   0        0        0    22863 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_catalog.py
+-rw-rw-rw-   0        0        0     8245 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_condition.py
+-rw-rw-rw-   0        0        0     7558 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_conformity.py
+-rw-rw-rw-   0        0        0    16653 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_contact.py
+-rw-rw-rw-   0        0        0    14009 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_coordinate_systems.py
+-rw-rw-rw-   0        0        0    13598 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_datasource.py
+-rw-rw-rw-   0        0        0     2819 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_directives.py
+-rw-rw-rw-   0        0        0    10559 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_event.py
+-rw-rw-rw-   0        0        0    19108 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_feature_attributes.py
+-rw-rw-rw-   0        0        0    12852 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_format.py
+-rw-rw-rw-   0        0        0    10496 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_invitation.py
+-rw-rw-rw-   0        0        0    38458 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_keyword.py
+-rw-rw-rw-   0        0        0    15256 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_license.py
+-rw-rw-rw-   0        0        0    11164 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_limitation.py
+-rw-rw-rw-   0        0        0    25144 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_link.py
+-rw-rw-rw-   0        0        0    15535 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_metadata.py
+-rw-rw-rw-   0        0        0     6058 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_metadata_bulk.py
+-rw-rw-rw-   0        0        0    17200 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_search.py
+-rw-rw-rw-   0        0        0    16317 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service.py
+-rw-rw-rw-   0        0        0    17176 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service_layers.py
+-rw-rw-rw-   0        0        0    18310 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service_operations.py
+-rw-rw-rw-   0        0        0    23781 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_share.py
+-rw-rw-rw-   0        0        0    14650 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_specification.py
+-rw-rw-rw-   0        0        0     4307 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_thesaurus.py
+-rw-rw-rw-   0        0        0    12937 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_user.py
+-rw-rw-rw-   0        0        0    18202 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_workgroup.py
+-rw-rw-rw-   0        0        0     1605 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/api_hooks.py
+-rw-rw-rw-   0        0        0    18711 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/checker.py
+-rw-rw-rw-   0        0        0     2255 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/decorators.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.473956 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/
+-rw-rw-rw-   0        0        0     1424 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/application_types.py
+-rw-rw-rw-   0        0        0     2130 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_actions.py
+-rw-rw-rw-   0        0        0     2315 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_ignore_reasons.py
+-rw-rw-rw-   0        0        0     2422 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_targets.py
+-rw-rw-rw-   0        0        0     2861 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/catalog_statistics_tags.py
+-rw-rw-rw-   0        0        0     2349 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/contact_roles.py
+-rw-rw-rw-   0        0        0     2082 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/contact_types.py
+-rw-rw-rw-   0        0        0     2066 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/edition_profiles.py
+-rw-rw-rw-   0        0        0     2144 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/event_kinds.py
+-rw-rw-rw-   0        0        0     2204 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/keyword_casing.py
+-rw-rw-rw-   0        0        0     2591 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/limitation_restrictions.py
+-rw-rw-rw-   0        0        0     2067 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/limitation_types.py
+-rw-rw-rw-   0        0        0     2058 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_actions.py
+-rw-rw-rw-   0        0        0     2470 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_kinds.py
+-rw-rw-rw-   0        0        0     2026 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_types.py
+-rw-rw-rw-   0        0        0     2819 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/metadata_subresources.py
+-rw-rw-rw-   0        0        0     2518 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/metadata_types.py
+-rw-rw-rw-   0        0        0     2466 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/search_filters_georelations.py
+-rw-rw-rw-   0        0        0     2128 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/service_layer_types.py
+-rw-rw-rw-   0        0        0     2215 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/session_status.py
+-rw-rw-rw-   0        0        0     2125 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/share_types.py
+-rw-rw-rw-   0        0        0     1998 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/user_roles.py
+-rw-rw-rw-   0        0        0     3054 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/enums/workgroup_statistics_tags.py
+-rw-rw-rw-   0        0        0     1001 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    19870 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/isogeo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.505064 isogeo-pysdk-3.8.2/isogeo_pysdk/models/
+-rw-rw-rw-   0        0        0     1748 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/__init__.py
+-rw-rw-rw-   0        0        0    16184 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/application.py
+-rw-rw-rw-   0        0        0     4260 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/bulk_report.py
+-rw-rw-rw-   0        0        0     6262 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/bulk_request.py
+-rw-rw-rw-   0        0        0    10991 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/catalog.py
+-rw-rw-rw-   0        0        0     7922 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/condition.py
+-rw-rw-rw-   0        0        0     7812 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/conformity.py
+-rw-rw-rw-   0        0        0    15867 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/contact.py
+-rw-rw-rw-   0        0        0     6213 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/coordinates_system.py
+-rw-rw-rw-   0        0        0    10550 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/datasource.py
+-rw-rw-rw-   0        0        0     4238 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/directive.py
+-rw-rw-rw-   0        0        0     7486 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/event.py
+-rw-rw-rw-   0        0        0    17324 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/feature_attributes.py
+-rw-rw-rw-   0        0        0     8175 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/format.py
+-rw-rw-rw-   0        0        0     9348 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/invitation.py
+-rw-rw-rw-   0        0        0     9533 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/keyword.py
+-rw-rw-rw-   0        0        0     5635 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/keyword_search.py
+-rw-rw-rw-   0        0        0     9004 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/license.py
+-rw-rw-rw-   0        0        0     9250 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/limitation.py
+-rw-rw-rw-   0        0        0    10510 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/link.py
+-rw-rw-rw-   0        0        0    43405 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/metadata.py
+-rw-rw-rw-   0        0        0     7856 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/metadata_search.py
+-rw-rw-rw-   0        0        0    12874 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/service_layer.py
+-rw-rw-rw-   0        0        0     8952 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/service_operation.py
+-rw-rw-rw-   0        0        0    15186 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/share.py
+-rw-rw-rw-   0        0        0    10004 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/specification.py
+-rw-rw-rw-   0        0        0     6780 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/thesaurus.py
+-rw-rw-rw-   0        0        0    11239 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/user.py
+-rw-rw-rw-   0        0        0    19996 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/models/workgroup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.505064 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/__init__.py
+-rw-rw-rw-   0        0        0     4258 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/attributes_frequency.py
+-rw-rw-rw-   0        0        0     2563 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/download_batch_hosted_data.py
+-rw-rw-rw-   0        0        0     2623 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/export_batch_xml19139_sync.py
+-rw-rw-rw-   0        0        0     2830 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/get_OpenCatalog.py
+-rw-rw-rw-   0        0        0     2293 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/latest_md_modified.py
+-rw-rw-rw-   0        0        0     6737 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/related_links.py
+-rw-rw-rw-   0        0        0     5378 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/results_parser.py
+-rw-rw-rw-   0        0        0     2741 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/search.py
+-rw-rw-rw-   0        0        0     3554 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/spatial_search.py
+-rw-rw-rw-   0        0        0     6106 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/store_api_responses_read.py
+-rw-rw-rw-   0        0        0     7670 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/samples/store_api_responses_rw.py
+-rw-rw-rw-   0        0        0     7790 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/translator.py
+-rw-rw-rw-   0        0        0      838 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/type_hints_custom.py
+-rw-rw-rw-   0        0        0    40710 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/isogeo_pysdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.426935 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/
+-rw-rw-rw-   0        0        0     4149 2023-05-04 17:57:43.000000 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4886 2023-05-04 17:57:43.000000 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:57:43.000000 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-04 17:57:43.000000 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 17:57:43.000000 isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      965 2023-05-04 17:57:43.541145 isogeo-pysdk-3.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     2378 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:57:43.541145 isogeo-pysdk-3.8.2/tests/
+-rw-rw-rw-   0        0        0     3224 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_about.py
+-rw-rw-rw-   0        0        0     4808 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_account.py
+-rw-rw-rw-   0        0        0    14716 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_applications.py
+-rw-rw-rw-   0        0        0     6528 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7000 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_bulks.py
+-rw-rw-rw-   0        0        0    13494 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_catalogs.py
+-rw-rw-rw-   0        0        0    17511 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_checker.py
+-rw-rw-rw-   0        0        0     8878 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_conditions.py
+-rw-rw-rw-   0        0        0     6847 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_conformity.py
+-rw-rw-rw-   0        0        0    12329 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     9587 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_coordinate_systems.py
+-rw-rw-rw-   0        0        0    11990 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_datasources.py
+-rw-rw-rw-   0        0        0     5479 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_directives.py
+-rw-rw-rw-   0        0        0    10121 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_enums.py
+-rw-rw-rw-   0        0        0    10212 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_events.py
+-rw-rw-rw-   0        0        0    16151 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_feature_attributes.py
+-rw-rw-rw-   0        0        0     7002 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_formats.py
+-rw-rw-rw-   0        0        0    33394 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_keywords.py
+-rw-rw-rw-   0        0        0    13605 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_licenses.py
+-rw-rw-rw-   0        0        0    10637 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_limitations.py
+-rw-rw-rw-   0        0        0    10744 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_links.py
+-rw-rw-rw-   0        0        0    10964 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_metadatas_noGeo.py
+-rw-rw-rw-   0        0        0    10929 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_metadatas_vector.py
+-rw-rw-rw-   0        0        0    13188 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_search.py
+-rw-rw-rw-   0        0        0    16057 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_service_layers.py
+-rw-rw-rw-   0        0        0    11398 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_service_operations.py
+-rw-rw-rw-   0        0        0    14385 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_shares.py
+-rw-rw-rw-   0        0        0    14313 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_specifications.py
+-rw-rw-rw-   0        0        0     5781 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_thesauri.py
+-rw-rw-rw-   0        0        0     3867 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_token.py
+-rw-rw-rw-   0        0        0     5457 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_translator.py
+-rw-rw-rw-   0        0        0     4972 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_users.py
+-rw-rw-rw-   0        0        0    17075 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_utils.py
+-rw-rw-rw-   0        0        0     9312 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_utils_credentials.py
+-rw-rw-rw-   0        0        0     5532 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_utils_uuid.py
+-rw-rw-rw-   0        0        0    12714 2023-05-04 17:56:10.000000 isogeo-pysdk-3.8.2/tests/test_workgroups.py
```

### Comparing `isogeo-pysdk-3.8.1/LICENSE` & `isogeo-pysdk-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/PKG-INFO` & `isogeo-pysdk-3.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogeo-pysdk
-Version: 3.8.1
+Version: 3.8.2
 Summary: API wrapper for the Isogeo REST API
 Home-page: https://github.com/isogeo/isogeo-api-py-minsdk/
 Author: Isogeo
 Author-email: contact@isogeo.com
 License: LGPL3
 Project-URL: Docs, https://isogeo-api-pysdk.readthedocs.io/
 Project-URL: Bug Reports, https://github.com/isogeo/isogeo-api-py-minsdk/issues/
```

### Comparing `isogeo-pysdk-3.8.1/README.md` & `isogeo-pysdk-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/__about__.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 ]
 
 
 __title__ = "Isogeo Python SDK"
 __summary__ = "API wrapper for the Isogeo REST API"
 __uri__ = "https://github.com/isogeo/isogeo-api-py-minsdk/"
 
-__version__ = "3.8.1"
+__version__ = "3.8.2"
 
 __author__ = "Isogeo"
 __email__ = "contact@isogeo.com"
 
 __license__ = "GNU Lesser General Public License v3.0"
 __copyright__ = "2016 - {0}, {1}".format(date.today().year, __author__)
```

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/__init__.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/__init__.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_about.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_about.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_account.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_account.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_application.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_application.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_catalog.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_catalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_condition.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_condition.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_conformity.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_conformity.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_contact.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_contact.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_coordinate_systems.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_datasource.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_datasource.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_directives.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_directives.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_event.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_event.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_feature_attributes.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_feature_attributes.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_format.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_format.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_invitation.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_invitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_keyword.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_keyword.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_license.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_license.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_limitation.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_limitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_link.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_link.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_metadata.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata_bulk.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_metadata_bulk.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_search.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_layers.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service_layers.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_operations.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_service_operations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_share.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_share.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_specification.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_specification.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_thesaurus.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_thesaurus.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_user.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_user.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_workgroup.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api/routes_workgroup.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/api_hooks.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/api_hooks.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/checker.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/checker.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/decorators.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/decorators.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/__init__.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/application_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/application_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_actions.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_actions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_ignore_reasons.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_ignore_reasons.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_targets.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/bulk_targets.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/catalog_statistics_tags.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/catalog_statistics_tags.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_roles.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/contact_roles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/contact_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/edition_profiles.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/edition_profiles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/event_kinds.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/event_kinds.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/keyword_casing.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/keyword_casing.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_restrictions.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/limitation_restrictions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/limitation_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_actions.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_actions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_kinds.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_kinds.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/link_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_subresources.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/metadata_subresources.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/metadata_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/search_filters_georelations.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/search_filters_georelations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/service_layer_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/service_layer_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/session_status.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/session_status.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/share_types.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/share_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/user_roles.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/user_roles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/workgroup_statistics_tags.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/enums/workgroup_statistics_tags.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/exceptions.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/isogeo.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/isogeo.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/__init__.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/application.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/application.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_report.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/bulk_report.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_request.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/bulk_request.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/catalog.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/condition.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/condition.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/conformity.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/conformity.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/contact.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/contact.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/coordinates_system.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/coordinates_system.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/datasource.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/directive.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/directive.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/event.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/event.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/feature_attributes.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/feature_attributes.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/format.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/format.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/invitation.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/invitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/keyword.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword_search.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/keyword_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/license.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/license.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/limitation.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/limitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/link.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/link.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/metadata.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata_search.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/metadata_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_layer.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/service_layer.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_operation.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/service_operation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/share.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/share.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/specification.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/specification.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/thesaurus.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/thesaurus.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/user.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/user.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/models/workgroup.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/models/workgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
                 'name': 'Isogeo Test',
                 'phone': '33 (0)9 67 46 50 06',
                 'type': 'group',
                 'zipCode': '75012'
             },
             'hasCswClient': True,
             'hasScanFme': True,
+            'hasFlashScan': True,
+            'hasAGSScan': True,
             'keywordsCasing': 'lowercase',
             'limits': {
                 'canDiffuse': False,
                 'canShare': True,
                 'Workgroups': {
                     'current': 1,
                     'max': -1
@@ -100,14 +102,16 @@
         "areKeywordsRestricted": bool,
         "canCreateLegacyServiceLinks": bool,
         "canCreateMetadata": bool,
         "code": str,
         "contact": Contact,
         "hasCswClient": bool,
         "hasScanFme": bool,
+        "hasFlashScan": bool,
+        "hasAGSScan": bool,
         "limits": dict,
         "keywordsCasing": str,
         "metadataLanguage": str,
         "themeColor": str,
     }
 
     ATTR_CREA = {
@@ -142,14 +146,16 @@
         areKeywordsRestricted: bool = None,
         canCreateLegacyServiceLinks: bool = None,
         canCreateMetadata: bool = None,
         code: str = None,
         contact: Contact = None,
         hasCswClient: bool = None,
         hasScanFme: bool = None,
+        hasFlashScan: bool = None,
+        hasAGSScan: bool = None,
         keywordsCasing: str = None,
         limits: dict = None,
         metadataLanguage: str = None,
         themeColor: str = None,
     ):
         """Workgroup model."""
 
@@ -162,14 +168,16 @@
         self._areKeywordsRestricted = None
         self._canCreateLegacyServiceLinks = None
         self._canCreateMetadata = None
         self._code = code
         self._contact = Contact
         self._hasCswClient = None
         self._hasScanFme = None
+        self._hasFlashScan = None
+        self._hasAGSScan = None
         self._keywordsCasing = None
         self._limits = None
         self._metadataLanguage = None
         self._themeColor = None
 
         # if values have been passed, so use them as objects attributes.
         # attributes are prefixed by an underscore '_'
@@ -191,14 +199,18 @@
             self._canCreateMetadata = canCreateMetadata
         if code is not None:
             self._code = code
         if hasCswClient is not None:
             self._hasCswClient = hasCswClient
         if hasScanFme is not None:
             self._hasScanFme = hasScanFme
+        if hasFlashScan is not None:
+            self._hasFlashScan = hasFlashScan
+        if hasAGSScan is not None:
+            self._hasAGSScan = hasAGSScan
         if keywordsCasing is not None:
             self._keywordsCasing = keywordsCasing
         if limits is not None:
             self._limits = limits
         if metadataLanguage is not None:
             self._metadataLanguage = metadataLanguage
         if themeColor is not None:
@@ -381,14 +393,52 @@
         """Sets the access of the group to the Scan.
 
         :param bool hasScanFme: The hasScanFme of this Workgroup. Must be one of GROUP_KIND_VALUES
         """
 
         self._hasScanFme = hasScanFme
 
+    # hasFlashScan
+    @property
+    def hasFlashScan(self) -> bool:
+        """Find out if the group has access to the Scan.
+
+        :return: The hasFlashScan value of this Workgroup.
+        :rtype: bool
+        """
+        return self._hasFlashScan
+
+    @hasFlashScan.setter
+    def hasFlashScan(self, hasFlashScan: bool):
+        """Sets the access of the group to the Scan.
+
+        :param bool hasFlashScan: The hasFlashScan of this Workgroup. Must be one of GROUP_KIND_VALUES
+        """
+
+        self._hasFlashScan = hasFlashScan
+
+    # hasAGSScan
+    @property
+    def hasAGSScan(self) -> bool:
+        """Find out if the group has access to the Scan.
+
+        :return: The hasAGSScan value of this Workgroup.
+        :rtype: bool
+        """
+        return self._hasAGSScan
+
+    @hasAGSScan.setter
+    def hasAGSScan(self, hasAGSScan: bool):
+        """Sets the access of the group to the Scan.
+
+        :param bool hasAGSScan: The hasAGSScan of this Workgroup. Must be one of GROUP_KIND_VALUES
+        """
+
+        self._hasAGSScan = hasAGSScan
+
     # keywordsCasing
     @property
     def keywordsCasing(self) -> str:
         """Gets the keywordsCasing of this Workgroup.
 
         :return: The keywordsCasing of this Workgroup.
         :rtype: str
```

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/attributes_frequency.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/attributes_frequency.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/download_batch_hosted_data.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/download_batch_hosted_data.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/export_batch_xml19139_sync.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/export_batch_xml19139_sync.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/get_OpenCatalog.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/get_OpenCatalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/latest_md_modified.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/latest_md_modified.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/related_links.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/related_links.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/results_parser.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/results_parser.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/search.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/spatial_search.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/spatial_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_read.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/store_api_responses_read.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_rw.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/samples/store_api_responses_rw.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/translator.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/translator.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/type_hints_custom.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/type_hints_custom.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk/utils.py` & `isogeo-pysdk-3.8.2/isogeo_pysdk/utils.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/PKG-INFO` & `isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogeo-pysdk
-Version: 3.8.1
+Version: 3.8.2
 Summary: API wrapper for the Isogeo REST API
 Home-page: https://github.com/isogeo/isogeo-api-py-minsdk/
 Author: Isogeo
 Author-email: contact@isogeo.com
 License: LGPL3
 Project-URL: Docs, https://isogeo-api-pysdk.readthedocs.io/
 Project-URL: Bug Reports, https://github.com/isogeo/isogeo-api-py-minsdk/issues/
```

### Comparing `isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/SOURCES.txt` & `isogeo-pysdk-3.8.2/isogeo_pysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/setup.cfg` & `isogeo-pysdk-3.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/setup.py` & `isogeo-pysdk-3.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_about.py` & `isogeo-pysdk-3.8.2/tests/test_about.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_account.py` & `isogeo-pysdk-3.8.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_applications.py` & `isogeo-pysdk-3.8.2/tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_authentication.py` & `isogeo-pysdk-3.8.2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_bulks.py` & `isogeo-pysdk-3.8.2/tests/test_bulks.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_catalogs.py` & `isogeo-pysdk-3.8.2/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_checker.py` & `isogeo-pysdk-3.8.2/tests/test_checker.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_conditions.py` & `isogeo-pysdk-3.8.2/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_conformity.py` & `isogeo-pysdk-3.8.2/tests/test_conformity.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_contacts.py` & `isogeo-pysdk-3.8.2/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_coordinate_systems.py` & `isogeo-pysdk-3.8.2/tests/test_coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_datasources.py` & `isogeo-pysdk-3.8.2/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_directives.py` & `isogeo-pysdk-3.8.2/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_enums.py` & `isogeo-pysdk-3.8.2/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_events.py` & `isogeo-pysdk-3.8.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_feature_attributes.py` & `isogeo-pysdk-3.8.2/tests/test_feature_attributes.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_formats.py` & `isogeo-pysdk-3.8.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_keywords.py` & `isogeo-pysdk-3.8.2/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_licenses.py` & `isogeo-pysdk-3.8.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_limitations.py` & `isogeo-pysdk-3.8.2/tests/test_limitations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_links.py` & `isogeo-pysdk-3.8.2/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_metadatas_noGeo.py` & `isogeo-pysdk-3.8.2/tests/test_metadatas_noGeo.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_metadatas_vector.py` & `isogeo-pysdk-3.8.2/tests/test_metadatas_vector.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_search.py` & `isogeo-pysdk-3.8.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_service_layers.py` & `isogeo-pysdk-3.8.2/tests/test_service_layers.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_service_operations.py` & `isogeo-pysdk-3.8.2/tests/test_service_operations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_shares.py` & `isogeo-pysdk-3.8.2/tests/test_shares.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_specifications.py` & `isogeo-pysdk-3.8.2/tests/test_specifications.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_thesauri.py` & `isogeo-pysdk-3.8.2/tests/test_thesauri.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_token.py` & `isogeo-pysdk-3.8.2/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_translator.py` & `isogeo-pysdk-3.8.2/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_users.py` & `isogeo-pysdk-3.8.2/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_utils.py` & `isogeo-pysdk-3.8.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_utils_credentials.py` & `isogeo-pysdk-3.8.2/tests/test_utils_credentials.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_utils_uuid.py` & `isogeo-pysdk-3.8.2/tests/test_utils_uuid.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.1/tests/test_workgroups.py` & `isogeo-pysdk-3.8.2/tests/test_workgroups.py`

 * *Files identical despite different names*

