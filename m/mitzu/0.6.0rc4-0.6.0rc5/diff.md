# Comparing `tmp/mitzu-0.6.0rc4.tar.gz` & `tmp/mitzu-0.6.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc4.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc5.tar", max compression
```

## Comparing `mitzu-0.6.0rc4.tar` & `mitzu-0.6.0rc5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-04-29 20:11:16.877457 mitzu-0.6.0rc4/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-04-29 20:11:16.877457 mitzu-0.6.0rc4/README.md
--rw-r--r--   0        0        0     6148 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-04-29 20:12:16.723844 mitzu-0.6.0rc4/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39656 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1394 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/helper.py
--rw-r--r--   0        0        0    53851 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2086 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11910 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     6951 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13345 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7392 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2511 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     2750 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5802 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15464 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4281 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21140 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9846 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    14708 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16412 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10152 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3956 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5027 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10128 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11849 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10013 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    36159 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5034 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3185 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2172 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0     2105 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4758 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    20518 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25939 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0      666 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     4141 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2943 2023-04-29 20:12:16.719844 mitzu-0.6.0rc4/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-04 19:30:11.338744 mitzu-0.6.0rc5/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-04 19:30:11.338744 mitzu-0.6.0rc5/README.md
+-rw-r--r--   0        0        0     6148 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-05-04 19:31:10.975585 mitzu-0.6.0rc5/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39764 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-04 19:30:11.734749 mitzu-0.6.0rc5/mitzu/helper.py
+-rw-r--r--   0        0        0    53852 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11926 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7022 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13737 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-04 19:30:11.738749 mitzu-0.6.0rc5/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1403 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3056 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5802 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15464 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4527 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21140 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9846 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14654 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21781 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0     9604 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1347 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4107 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5027 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10191 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11849 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9629 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    36159 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5155 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3185 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     5198 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    20635 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25830 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     3949 2023-05-04 19:30:11.742749 mitzu-0.6.0rc5/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2943 2023-05-04 19:31:10.975585 mitzu-0.6.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc5/PKG-INFO
```

### Comparing `mitzu-0.6.0rc4/LICENSE.txt` & `mitzu-0.6.0rc5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/README.md` & `mitzu-0.6.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/.DS_Store` & `mitzu-0.6.0rc5/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/__init__.py` & `mitzu-0.6.0rc5/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.4"
+__version__ = "0.6.0-rc.5"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc5/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/helper.py` & `mitzu-0.6.0rc5/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,19 @@
             for f in fields:
                 field_values = values[f._get_name()]
                 if (
                     (field_values is None)
                     or (len(field_values) == 1 and field_values[0])
                     or (len(field_values) > 1)
                 ):
-                    vals = [v for v in field_values if v] if field_values else None
+                    vals = (
+                        [v for v in field_values if v is not None]
+                        if field_values
+                        else None
+                    )
                     field_defs[f] = M.EventFieldDef(
                         _event_name=evt,
                         _field=f,
                         _event_data_table=event_data_table,
                         _enums=vals,
                     )
```

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc5/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/helper.py` & `mitzu-0.6.0rc5/mitzu/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,9 +40,21 @@
             raise ValueError(f"Segment's left value is of invalid type: {type(left)}")
     elif isinstance(segment, M.ComplexSegment):
         return get_segment_project(segment._left)
     else:
         raise ValueError(f"Segment is of invalid type: {type(segment)}")
 
 
+def get_metric_group_by(metric: M.Metric) -> Optional[M.EventFieldDef]:
+    if isinstance(metric, M.SegmentationMetric):
+        return metric._segment._group_by
+    elif (
+        isinstance(metric, M.ConversionMetric) and len(metric._conversion._segments) > 0
+    ):
+        return metric._conversion._segments[0]._group_by
+    elif isinstance(metric, M.RetentionMetric):
+        return metric._initial_segment._group_by
+    return None
+
+
 def create_unique_id():
     return str(uuid4())[-12:]
```

### Comparing `mitzu-0.6.0rc4/mitzu/model.py` & `mitzu-0.6.0rc5/mitzu/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         if self.period == TimeGroup.WEEK:
             return relativedelta(weeks=self.value)
         if self.period == TimeGroup.MONTH:
             return relativedelta(months=self.value)
         if self.period == TimeGroup.QUARTER:
             return relativedelta(months=self.value * 4)
         if self.period == TimeGroup.YEAR:
-            return relativedelta(year=self.value)
+            return relativedelta(years=self.value)
         raise Exception(f"Unsupported relative delta value: {self.period}")
 
 
 class Identifiable(Protocol):
     def get_id(self) -> str:
         pass
```

### Comparing `mitzu-0.6.0rc4/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc5/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/project_discovery.py` & `mitzu-0.6.0rc5/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/project_serialization.py` & `mitzu-0.6.0rc5/mitzu/project_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         PROJECT: dp.project,
         CONNECTION: dp.project.connection,
     }
 
     project_binary = pickle.dumps(serializable)
     data = {
         "version": DISCOVERED_PROJECT_FILE_VERSION,
-        "project": base64.b64encode(project_binary).decode("UTF-8"),
+        "project": base64.urlsafe_b64encode(project_binary).decode("UTF-8"),
     }
     return json.dumps(data)
 
 
 def deserialize_discovered_project(raw_data: bytes) -> M.DiscoveredProject:
     try:
         data = json.loads(raw_data)
@@ -49,15 +49,15 @@
             )
     except Exception as e:
         raise DiscoveredProjectSerializationError(
             "Something went wrong, cannot deserialize discovered project file.\n"
             "Try discovering the project again."
         ) from e
 
-    res: Dict[str, Any] = pickle.loads(base64.b64decode(data["project"]))
+    res: Dict[str, Any] = pickle.loads(base64.urlsafe_b64decode(data["project"]))
 
     project: M.Project = res[PROJECT]
 
     for edt in project.event_data_tables:
         edt.set_project(project)
     project.set_connection(res[CONNECTION])
```

### Comparing `mitzu-0.6.0rc4/mitzu/samples/__init__.py` & `mitzu-0.6.0rc5/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc5/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc5/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/serialization.py` & `mitzu-0.6.0rc5/mitzu/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,19 +302,19 @@
 def from_dict(value: Dict, project: M.Project) -> M.Metric:
     return _from_dict(value, project, None, "")
 
 
 def dict_to_compressed_string(metric_dict: Dict) -> str:
     metric_json = json.dumps(metric_dict)
     zipped = zlib.compress(metric_json.encode("utf-8"), 9)
-    return base64.b64encode(zipped).decode("utf-8")
+    return base64.urlsafe_b64encode(zipped).decode("utf-8")
 
 
 def to_compressed_string(metric: M.Metric) -> str:
     return dict_to_compressed_string(to_dict(metric))
 
 
 def from_compressed_string(compressed_str: str, project: M.Project) -> M.Metric:
-    zipped = base64.b64decode(compressed_str)
+    zipped = base64.urlsafe_b64decode(compressed_str)
     unzipped = zlib.decompress(zipped)
     val = json.loads(unzipped)
     return from_dict(val, project)
```

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/charts.py` & `mitzu-0.6.0rc5/mitzu/visualization/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 
 def filter_top_groups(
     pdf: pd.DataFrame,
     metric: M.Metric,
     order_by_col: str,
 ) -> pd.DataFrame:
     max = metric._max_group_count
-    g_users = (
-        pdf[[GA.GROUP_COL, order_by_col]].groupby(GA.GROUP_COL).sum().reset_index()
-    )
+    pdf_simple = pdf[[GA.GROUP_COL, order_by_col]]
+    groupped = pdf_simple.groupby(GA.GROUP_COL)[order_by_col]
+    summed = groupped.sum()
+    g_users = summed.reset_index()
+
     if g_users.shape[0] > 0:
         g_users = g_users.sort_values(order_by_col, ascending=False)
     g_users = g_users.head(max)
     top_groups = list(g_users[GA.GROUP_COL].values)
     return pdf[pdf[GA.GROUP_COL].isin(top_groups)]
```

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/common.py` & `mitzu-0.6.0rc5/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/labels.py` & `mitzu-0.6.0rc5/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/plot.py` & `mitzu-0.6.0rc5/mitzu/visualization/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 import plotly.express as px
 import plotly.figure_factory as ff
 
 import pandas as pd
 import mitzu.model as M
+import mitzu.helper as H
 import mitzu.visualization.common as C
 from typing import Dict, List, Tuple
 from base64 import b64encode
 import plotly.io as pio
 import traceback
 
 PRISM2 = [
@@ -38,16 +39,18 @@
             line=dict(width=1.5),
             mode="lines+markers",
             textposition="top center",
             textfont_size=9,
         )
     elif metric._chart_type == M.SimpleChartType.STACKED_AREA:
         fig.update_traces(textposition="top center", textfont_size=9)
+    elif metric._chart_type in (M.SimpleChartType.STACKED_BAR, M.SimpleChartType.BAR):
+        fig.update_traces(textposition="auto", textfont_size=9)
     else:
-        fig.update_traces(textposition="outside", textfont_size=9)
+        fig.update_traces(textposition="top center", textfont_size=9)
 
     fig.update_yaxes(
         rangemode="tozero",
         showline=True,
         linecolor="rgba(127,127,127,0.1)",
         gridcolor="rgba(127,127,127,0.1)",
         fixedrange=True,
@@ -75,15 +78,17 @@
         uniformtext_minsize=7,
         height=600,
         hoverlabel={"font": {"size": 12}},
         paper_bgcolor="rgba(0,0,0,0)",
         plot_bgcolor="rgba(0,0,0,0)",
         hovermode=simple_chart.hover_mode,
         legend=dict(orientation="h", yanchor="bottom", y=-0.2, xanchor="left"),
-        showlegend=len(fig.data) > 1,
+        showlegend=(
+            H.get_metric_group_by(metric=metric) is not None or len(fig.data) > 1
+        ),
     )
     return fig
 
 
 def set_heatmap_figure_style(fig, simple_chart: C.SimpleChart):
     fig.update_traces(xgap=1, ygap=1, hovertemplate="%{hovertext} <extra></extra>")
     fig.update_xaxes(
```

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/titles.py` & `mitzu-0.6.0rc5/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc5/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc5/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc5/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc5/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc5/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc5/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc5/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc5/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc5/mitzu/webapp/auth/authorizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from __future__ import annotations
 
-import dash
-import os
 import time
 import traceback
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 import flask
 import werkzeug
 import jwt
 import requests
 import base64
-from typing import Any, Dict, Optional, List
+from typing import Any, Dict, List, Optional
 from urllib import parse
 from mitzu.helper import LOGGER
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.configs as configs
 import mitzu.webapp.service.user_service as U
 import mitzu.webapp.model as WM
 
-HOME_URL = os.getenv("HOME_URL", "http://localhost:8082")
-MITZU_WEBAPP_URL = os.getenv("MITZU_WEBAPP_URL", HOME_URL)
 JWT_ALGORITHM = "HS256"
 JWT_CLAIM_ROLE = "rol"
 
 
 @dataclass(frozen=True)
 class OAuthConfig:
     """
@@ -79,66 +75,75 @@
         )
 
 
 @dataclass(frozen=True)
 class AuthConfig:
     user_service: U.UserService
 
-    token_cookie_name: str = field(default_factory=lambda: "auth-token")
-    redirect_cookie_name: str = field(default_factory=lambda: "redirect-to")
+    token_cookie_name: str = "auth-token"
+    redirect_cookie_name: str = "redirect-to"
 
-    session_timeout: int = field(default_factory=lambda: 7 * 24 * 60 * 60)
-    token_signing_key: str = field(default_factory=lambda: configs.AUTH_JWT_SECRET)
+    session_timeout: int = 7 * 24 * 60 * 60
+    token_signing_key: str = configs.AUTH_JWT_SECRET
 
     oauth: Optional[OAuthConfig] = None
     token_validator: Optional[TokenValidator] = None
 
 
 @dataclass(frozen=True)
 class OAuthAuthorizer:
     _config: AuthConfig
 
     _authorized_url_prefixes: List[str] = field(
         default_factory=lambda: [
             P.UNAUTHORIZED_URL,
-            configs.HEALTH_CHECK_PATH,
+            P.HEALTHCHECK_PATH,
             "/assets/",
             "/_dash-update-component",
             "/_dash-component-suites/",
             "/_dash-layout",
             "/_dash-dependencies",
         ]
     )
     _ignore_token_refresh_prefixes: List[str] = field(
         default_factory=lambda: [
             P.UNAUTHORIZED_URL,
             P.SIGN_OUT_URL,
-            configs.HEALTH_CHECK_PATH,
+            P.HEALTHCHECK_PATH,
             "/assets/",
         ]
     )
 
+    def get_home_url(self):
+        url = flask.request.host_url
+        return url[:-1] if url.endswith("/") else url
+
     @classmethod
     def create(cls, config: AuthConfig) -> OAuthAuthorizer:
         return OAuthAuthorizer(
             _config=config,
         )
 
     def _get_unauthenticated_response(
-        self, redirect: Optional[str] = None
+        self, redirect_url: Optional[str] = None
     ) -> werkzeug.wrappers.response.Response:
         resp = self._redirect(P.UNAUTHORIZED_URL)
-        resp.set_cookie(self._config.token_cookie_name, "", expires=0)
-        if (
-            redirect
-            and not redirect.startswith("/assets/")
-            and not redirect.startswith("/_dash")
-            and not redirect.startswith(configs.HEALTH_CHECK_PATH)
-        ):
-            resp.set_cookie(self._config.redirect_cookie_name, redirect)
+        self.clear_cookie(resp, self._config.token_cookie_name)
+        if redirect_url:
+            url = parse.urlparse(redirect_url)
+
+            if (
+                url.path
+                and not url.path.startswith("/assets/")
+                and not url.path.startswith("/_dash")
+                and not url.path.startswith("/_reload-hash")
+                and not url.path.startswith("/auth")
+                and not url.path.startswith(P.HEALTHCHECK_PATH)
+            ):
+                self.set_cookie(resp, self._config.redirect_cookie_name, redirect_url)
         return resp
 
     def _redirect(self, location: str) -> werkzeug.wrappers.response.Response:
         resp = flask.redirect(code=307, location=location)
         resp.headers["Cache-Control"] = "no-cache, no-store, must-revalidate"
         resp.headers["Pragma"] = "no-cache"
         resp.headers["Expires"] = "0"
@@ -164,15 +169,15 @@
             "utf-8",
         )
         secret_hash = base64.b64encode(message).decode()
         payload = {
             "grant_type": "authorization_code",
             "client_id": self._config.oauth.client_id,
             "code": auth_code,
-            "redirect_uri": f"{HOME_URL}{P.OAUTH_CODE_URL}",
+            "redirect_uri": f"{self.get_home_url()}{P.OAUTH_CODE_URL}",
         }
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": f"Basic {secret_hash}",
         }
 
         resp = requests.post(
@@ -206,18 +211,15 @@
             claims = jwt.decode(
                 token, self._config.token_signing_key, algorithms=[JWT_ALGORITHM]
             )
 
             token_subject = claims["sub"]
             user = self._config.user_service.get_user_by_id(token_subject)
             if user is None:
-                # SSO tokens contains the email not the use id
-                user = self._config.user_service.get_user_by_email(token_subject)
-                if user is None:
-                    raise Exception("User not found")
+                raise Exception("User not found")
             claims[JWT_CLAIM_ROLE] = user.role
             return claims
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def _validate_foreign_token(self, token) -> Optional[str]:
@@ -248,15 +250,15 @@
         if self._config.oauth and request.path == P.OAUTH_CODE_URL:
             code = self._get_oauth_code()
             if code is not None:
                 LOGGER.debug(f"Redirected with code={code}")
                 try:
                     id_token = self._get_identity_token(code)
                     redirect_url = flask.request.cookies.get(
-                        self._config.redirect_cookie_name, MITZU_WEBAPP_URL
+                        self._config.redirect_cookie_name, request.host_url
                     )
 
                     user_email = self._validate_foreign_token(id_token)
                     if not user_email:
                         raise Exception("Unauthorized (Invalid jwt token)")
 
                     user = self._config.user_service.get_user_by_email(user_email)
@@ -268,46 +270,43 @@
                     token_identity = user.id
 
                     token = self._generate_new_token_for_identity(
                         token_identity, role=user_role
                     )
 
                     resp = self._redirect(redirect_url)
-                    resp.set_cookie(self._config.token_cookie_name, token)
-                    resp.set_cookie(self._config.redirect_cookie_name, "", expires=0)
+                    self.set_cookie(resp, self._config.token_cookie_name, token)
+                    self.clear_cookie(resp, self._config.redirect_cookie_name)
                     return resp
                 except Exception as exc:
                     traceback.print_exception(type(exc), exc, exc.__traceback__)
                     LOGGER.warning(f"Failed to authenticate: {str(exc)}")
                     if self._config.oauth and self._config.oauth.sign_out_url:
                         resp = self._redirect(self._config.oauth.sign_out_url)
-                        resp.set_cookie(self._config.token_cookie_name, "", expires=0)
+                        self.clear_cookie(resp, self._config.token_cookie_name)
                         return resp
                     return self._get_unauthenticated_response()
 
         auth_token = flask.request.cookies.get(self._config.token_cookie_name)
 
         if request.path == P.SIGN_OUT_URL:
             if self._config.oauth and self._config.oauth.sign_out_url:
                 resp = self._redirect(self._config.oauth.sign_out_url)
-                resp.set_cookie(self._config.token_cookie_name, "", expires=0)
+                self.clear_cookie(resp, self._config.token_cookie_name)
                 return resp
             return self._get_unauthenticated_response()
 
         for prefix in self._authorized_url_prefixes:
             if request.path.startswith(prefix):
                 return None
 
         if auth_token and self._validate_token(auth_token) is not None:
             return None
 
-        redirect_url = request.path
-        if len(request.query_string) > 0:
-            redirect_url += "?" + request.query_string.decode("utf-8")
-        return self._get_unauthenticated_response(redirect_url)
+        return self._get_unauthenticated_response(request.url)
 
     def refresh_auth_token(
         self, request: flask.Request, resp: flask.Response
     ) -> werkzeug.wrappers.response.Response:
         for prefix in self._ignore_token_refresh_prefixes:
             if request.path.startswith(prefix):
                 return resp
@@ -315,15 +314,15 @@
         auth_token = flask.request.cookies.get(self._config.token_cookie_name)
         if auth_token is not None:
             identity = self._validate_token(auth_token)
             if identity is not None:
                 new_token = self._generate_new_token_for_identity(
                     identity["sub"], role=identity[JWT_CLAIM_ROLE]
                 )
-                resp.set_cookie(self._config.token_cookie_name, new_token)
+                self.set_cookie(resp, self._config.token_cookie_name, new_token)
         return resp
 
     def is_request_authorized(self, request: flask.Request) -> bool:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         return auth_token is not None and self._validate_token(auth_token) is not None
 
     def get_current_user_role(self, request: flask.Request) -> Optional[WM.Role]:
@@ -334,27 +333,49 @@
 
         claims = self._validate_token(auth_token)
         if claims is None or JWT_CLAIM_ROLE not in claims.keys():
             return None
 
         return WM.Role(claims[JWT_CLAIM_ROLE])
 
-    def login_local_user(self, email: str, password: str) -> bool:
+    def login_local_user(
+        self, email: str, password: str, response: Optional[flask.Response] = None
+    ) -> Optional[str]:
         if self._config.oauth:
             raise ValueError("Password login is not enabled, need to use SSO")
 
         user = self._config.user_service.get_user_by_email_and_password(email, password)
         if user is None:
-            return False
+            return None
 
         token = self._generate_new_token_for_identity(user.id, role=user.role)
-        dash.callback_context.response.set_cookie(self._config.token_cookie_name, token)
-        return True
+
+        if response:
+            self.set_cookie(response, self._config.token_cookie_name, token)
+            self.clear_cookie(response, self._config.redirect_cookie_name)
+
+        return flask.request.cookies.get(
+            self._config.redirect_cookie_name, self.get_home_url()
+        )
 
     def get_current_user_id(self) -> Optional[str]:
         auth_token = flask.request.cookies.get(self._config.token_cookie_name)
         if auth_token is None:
             return None
         token_claims = self._validate_token(auth_token)
         if token_claims is None:
             return None
         return token_claims.get("sub")
+
+    def set_cookie(
+        self,
+        response: werkzeug.wrappers.response.Response,
+        cookie_name: str,
+        value: str,
+        **params,
+    ):
+        response.set_cookie(cookie_name, value, path="/", httponly=True, **params)
+
+    def clear_cookie(
+        self, response: werkzeug.wrappers.response.Response, cookie_name: str
+    ):
+        self.set_cookie(response, cookie_name, "", expires=0)
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc5/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc5/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc5/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/cache.py` & `mitzu-0.6.0rc5/mitzu/webapp/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,30 @@
             self.clear(key)
 
     def list_keys(
         self, prefix: Optional[str] = None, strip_prefix: bool = True
     ) -> List[str]:
         raise NotImplementedError()
 
+    def health_check(self):
+        raise NotImplementedError()
+
 
 @dataclass(frozen=True, init=False)
 class DiskMitzuCache(MitzuCache):
 
     _disk_cache: diskcache.Cache
     _global_prefix: Optional[str] = None
 
     def __init__(self, name: str, global_prefix: Optional[str] = None) -> None:
         super().__init__()
         object.__setattr__(
             self,
             "_disk_cache",
-            diskcache.Cache(timeout=10, directory=f"{configs.DISK_CACHE_PATH}/{name}"),
+            diskcache.Cache(timeout=10, directory=f"./storage/{name}"),
         )
         object.__setattr__(
             self,
             "_global_prefix",
             global_prefix,
         )
 
@@ -105,14 +108,17 @@
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"LIST {prefix}: {res}")
         return res
 
     def get_disk_cache(self) -> diskcache.Cache:
         return self._disk_cache
 
+    def health_check(self):
+        self.get_disk_cache().get("health_check", "ok")
+
 
 @dataclass(frozen=True)
 class RequestCache(MitzuCache):
     """This cache is in-memory however it is ephemeral, it only stores values until the end of the request
     This is because it is not picklable.
     """
 
@@ -142,14 +148,17 @@
         self.delegate.clear(key)
 
     def list_keys(
         self, prefix: Optional[str] = None, strip_prefix: bool = True
     ) -> List[str]:
         return self.delegate.list_keys(prefix, strip_prefix)
 
+    def health_check(self):
+        return self.delegate.health_check()
+
 
 class RedisException(Exception):
     pass
 
 
 @dataclass(init=False, frozen=True)
 class RedisMitzuCache(MitzuCache):
@@ -164,26 +173,20 @@
     ) -> None:
         super().__init__()
 
         if redis_cache is not None:
             object.__setattr__(self, "_redis", redis_cache)
             object.__setattr__(self, "_global_prefix", global_prefix)
         else:
-            if configs.STORAGE_REDIS_HOST is None:
+            if configs.CACHE_REDIS_URL is None:
                 raise ValueError(
-                    "STORAGE_REDIS_HOST env variable is not set, can't create redis cache."
+                    "CACHE_REDIS_URL env variable is not set, can't create redis cache."
                 )
             object.__setattr__(
-                self,
-                "_redis",
-                redis.Redis(
-                    host=configs.STORAGE_REDIS_HOST,
-                    port=configs.STORAGE_REDIS_PORT,
-                    password=configs.STORAGE_REDIS_PASSWORD,
-                ),
+                self, "_redis", redis.Redis.from_url(url=configs.CACHE_REDIS_URL)
             )
             object.__setattr__(self, "_global_prefix", global_prefix)
 
     def _get_key(self, key: str) -> str:
         if self._global_prefix:
             return f"{self._global_prefix}.{key}"
         return key
@@ -225,7 +228,10 @@
             prefix = ""
         keys = self._redis.keys(f"{prefix}*")
         start_pos = len(prefix) if strip_prefix else 0
         res = [k.decode()[start_pos:] for k in keys]
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"LIST prefix={prefix}: {res}")
         return res
+
+    def health_check(self):
+        self._redis.get("health_check")
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc5/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc5/mitzu/webapp/dependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-
+from typing import Optional
 
 import mitzu.webapp.auth.authorizer as A
 import mitzu.webapp.cache as C
 import mitzu.webapp.configs as configs
 import mitzu.webapp.storage as S
 import mitzu.webapp.service.user_service as U
 import mitzu.webapp.service.navbar_service as NB
 import mitzu.webapp.service.events_service as E
 import mitzu.webapp.service.secret_service as SS
+import mitzu.webapp.service.notification_service as NS
 
 CONFIG_KEY = "dependencies"
 
 
 @dataclass(frozen=True)
 class Dependencies:
 
@@ -22,19 +23,25 @@
     storage: S.MitzuStorage
     queue: C.MitzuCache
     cache: C.MitzuCache
     events_service: E.EventsService
     navbar_service: NB.NavbarService
     secret_service: SS.SecretService
     user_service: U.UserService
+    notification_service: NS.NotificationService
 
     @classmethod
-    def from_configs(cls) -> Dependencies:
+    def from_configs(
+        cls, notification_service: Optional[NS.NotificationService] = None
+    ) -> Dependencies:
+        if notification_service is None:
+            notification_service = NS.DummyNotificationService()
+
         delegate_cache: C.MitzuCache
-        if configs.STORAGE_REDIS_HOST is not None:
+        if configs.CACHE_REDIS_URL is not None:
             delegate_cache = C.RedisMitzuCache(global_prefix=configs.CACHE_PREFIX)
         else:
             delegate_cache = C.DiskMitzuCache(
                 "cache", global_prefix=configs.CACHE_PREFIX
             )
         cache = C.RequestCache(delegate_cache)
         storage = S.MitzuStorage(connection_string=configs.STORAGE_CONNECTION_STRING)
@@ -45,41 +52,41 @@
 
             oauth_config = Cognito.get_config()
         elif configs.AUTH_BACKEND == "google":
             from mitzu.webapp.auth.google import GoogleOAuth
 
             oauth_config = GoogleOAuth.get_config()
 
-        user_service = U.UserService(storage, root_password=configs.AUTH_ROOT_PASSWORD)
+        user_service = U.UserService(
+            storage,
+            notification_service=notification_service,
+        )
 
         auth_config = A.AuthConfig(
             oauth=oauth_config,
-            token_validator=A.JWTTokenValidator.create_from_oauth_config(oauth_config)
-            if oauth_config is not None
-            else None,
+            token_validator=(
+                A.JWTTokenValidator.create_from_oauth_config(oauth_config)
+                if oauth_config is not None
+                else None
+            ),
             token_signing_key=configs.AUTH_JWT_SECRET,
             session_timeout=configs.AUTH_SESSION_TIMEOUT,
             user_service=user_service,
         )
         authorizer = A.OAuthAuthorizer.create(auth_config)
-
-        queue: C.MitzuCache
-        if configs.QUEUE_REDIS_HOST is not None:
-            queue = C.RedisMitzuCache()
-        else:
-            queue = C.DiskMitzuCache("queue")
+        queue = C.DiskMitzuCache("queue")
 
         # Adding cache layer over storage
         events_service = E.EventsService(storage)
-
         secret_service = SS.SecretService()
 
         return Dependencies(
             authorizer=authorizer,
             cache=cache,
             storage=storage,
             queue=queue,
             user_service=user_service,
             navbar_service=NB.NavbarService(),
             events_service=events_service,
             secret_service=secret_service,
+            notification_service=notification_service,
         )
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/helper.py` & `mitzu-0.6.0rc5/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/model.py` & `mitzu-0.6.0rc5/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc5/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/connections_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,33 +30,38 @@
         connections.append(con)
 
     return html.Div(
         [
             NB.create_mitzu_navbar("explore-navbar"),
             dbc.Container(
                 children=[
-                    html.H4("Choose from connections:", className="card-title"),
-                    html.Hr(),
-                    create_connections_container(connections),
-                    html.Hr(),
                     dbc.Row(
-                        dbc.Col(
-                            dbc.Button(
-                                [
-                                    html.B(className="bi bi-plus-circle"),
-                                    " New Warehouse Connection",
-                                ],
-                                size="sm",
-                                color="primary",
-                                href=P.CONNECTIONS_CREATE_PATH,
+                        [
+                            dbc.Col(
+                                html.H4("Manage connections", className="card-title"),
+                                width="auto",
                             ),
-                            lg=3,
-                            sm=12,
-                        )
+                            dbc.Col(
+                                dbc.Button(
+                                    [
+                                        html.B(className="bi bi-plus-circle me-1"),
+                                        "New Connection",
+                                    ],
+                                    size="sm",
+                                    color="primary",
+                                    href=P.CONNECTIONS_CREATE_PATH,
+                                ),
+                                width="auto",
+                                class_name="ms-auto",
+                            ),
+                        ],
                     ),
+                    html.Hr(),
+                    create_connections_container(connections),
+                    html.Hr(),
                 ]
             ),
         ]
     )
 
 
 def create_connections_container(connections: List[M.Connection]):
@@ -86,43 +91,44 @@
     if connection.catalog is not None:
         details.append(f"Catalog: {connection.catalog}")
     if connection.schema is not None:
         details.append(f"Schema: {connection.schema}")
 
     project_jumbotron = dbc.Col(
         dbc.Card(
-            dbc.CardBody(
-                [
-                    html.H4(
-                        H.value_to_label(connection.connection_name),
-                        className="card-title",
-                        id=CONNECTION_TITLE,
-                    ),
-                    html.Hr(),
-                    html.Img(
-                        src=f"/assets/warehouse/{str(connection.connection_type.name).lower()}.png",
-                        height=40,
-                    ),
-                    *[html.Div(d) for d in details],
-                    html.Hr(),
+            [
+                dbc.CardHeader(
+                    H.value_to_label(connection.connection_name),
+                    class_name="lead",
+                    id=CONNECTION_TITLE,
+                ),
+                dbc.CardBody(
                     html.Div(
-                        [
-                            dbc.Button(
-                                "Manage",
-                                size="sm",
-                                color="primary",
-                                href=P.create_path(
-                                    P.CONNECTIONS_MANAGE_PATH,
-                                    connection_id=connection.id,
-                                ),
+                        children=[
+                            html.Img(
+                                src=f"/assets/warehouse/{str(connection.connection_type.name).lower()}.png",
+                                height=40,
                             ),
+                            *[html.Div(d) for d in details],
                         ],
+                        style={"min-height": "100px"},
+                    )
+                ),
+                dbc.CardFooter(
+                    dbc.Button(
+                        "Manage",
+                        size="sm",
+                        color="primary",
+                        href=P.create_path(
+                            P.CONNECTIONS_MANAGE_PATH,
+                            connection_id=connection.id,
+                        ),
                     ),
-                ]
-            ),
+                ),
+            ],
             class_name="mb-3",
         ),
         lg=3,
         sm=12,
     )
     return project_jumbotron
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/edit_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dash import (
     Input,
     Output,
     State,
     callback,
     html,
     register_page,
+    ALL,
 )
 import dash_bootstrap_components as dbc
 import dash.development.base_component as bc
 import dash_mantine_components as dmc
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
@@ -273,30 +274,30 @@
     },
     inputs={
         "n_clicks": Input(USER_CREATE_BUTTON, "n_clicks"),
     },
     state={
         "email": State({"type": INDEX_TYPE, "index": PROP_EMAIL}, "value"),
         "role": State({"type": INDEX_TYPE, "index": PROP_ROLE}, "value"),
-        "password": State({"type": INDEX_TYPE, "index": PROP_PASSWORD}, "value"),
-        "confirm_password": State(
-            {"type": INDEX_TYPE, "index": PROP_CONFIRM_PASSWORD}, "value"
-        ),
+        "all_inputs": State({"type": INDEX_TYPE, "index": ALL}, "value"),
     },
     prevent_initial_call=True,
 )
 @restricted_for_admin
-def create_new_user(n_clicks: int, email="", role="", password="", confirm_password=""):
+def create_new_user(n_clicks: int, email="", role="", all_inputs=[]):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
     if deps.authorizer._config.oauth:
         # SSO users don't have passwords
         password = None
         confirm_password = None
+    else:
+        password = all_inputs[2]
+        confirm_password = all_inputs[3]
 
     try:
         user_service.new_user(email, password, confirm_password, role=WM.Role(role))
         return {
             SAVE_RESPONSE_CONTAINER: "User created!",
         }
     except Exception as e:
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/explore_page.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,33 +23,39 @@
 import mitzu.webapp.navbar as NB
 import mitzu.visualization.charts as CHRT
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 from mitzu.webapp.helper import MITZU_LOCATION, find_event_field_def, CHILDREN
 import mitzu.webapp.pages.paths as P
 import flask
-import dash_mantine_components as dmc
 import traceback
 from dash import ctx, html, callback, no_update, dcc
 from dash.dependencies import ALL, Input, Output, State
-from dash_iconify import DashIconify
 from mitzu.webapp.auth.decorator import restricted
 
 
 from mitzu.webapp.helper import (
     get_final_all_inputs,
 )
 
 NAVBAR_ID = "explore_navbar"
 SHARE_BUTTON = "share_button"
 CLIPBOARD = "share_clipboard"
-METRIC_NAME_INPUT = "metric_name_input"
+
 METRIC_ID_VALUE = "metric_id_value"
-METRIC_NAME_PROGRESS = "metric_name_progress"
+METRIC_NAME_INPUT = "metric_name_input"
+METRIC_SAVE_DIALOG = "metric_save_dialog"
+METRIC_SAVE_NAVBAR_BUTTON = "metric_save_navbar_button"
+METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON = "metric_save_dialog_save_new_button"
+METRIC_SAVE_DIALOG_CLOSE_BUTTON = "metric_save_dialog_close_button"
+METRIC_SAVE_DIALOG_REPLACE_BUTTON = "metric_save_dialog_replace_button"
+METRIC_SAVE_DIALOG_INFO = "metric_save_dialog_info"
+
 EXPLORE_PAGE = "explore_page"
+
 ALL_INPUT_COMPS = {
     "all_inputs": {
         ES.EVENT_NAME_DROPDOWN: Input(
             {"type": ES.EVENT_NAME_DROPDOWN, "index": ALL}, "value"
         ),
         SS.PROPERTY_OPERATOR_DROPDOWN: Input(
             {"type": SS.PROPERTY_OPERATOR_DROPDOWN, "index": ALL}, "value"
@@ -83,37 +89,26 @@
     id: str, show_metric_type: bool = False, metric: Optional[M.Metric] = None, **kwargs
 ) -> Optional[bc.Component]:
     if not show_metric_type:
         return None
     return MTH.from_metric_type(MTH.MetricType.from_metric(metric))
 
 
-def metric_name_navbar_provider(
+def save_metric_navbar_provider(
     id: str,
     show_metric_name: bool = False,
-    saved_metric: Optional[WM.SavedMetric] = None,
     **kwargs,
 ) -> Optional[bc.Component]:
     if not show_metric_name:
         return None
-
-    return dmc.TextInput(
-        id=METRIC_NAME_INPUT,
-        debounce=700,
-        placeholder="Name your metric",
-        value=saved_metric.name if saved_metric is not None else None,
-        size="xs",
-        icon=DashIconify(icon="material-symbols:star", color="dark"),
-        rightSection=dmc.Loader(
-            size="xs",
-            color="dark",
-            className="d-none",
-            id=METRIC_NAME_PROGRESS,
-        ),
-        style={"width": "200px"},
+    return dbc.Button(
+        children=[html.I(className="bi bi-save me-1"), "save"],
+        size="sm",
+        color="success",
+        id=METRIC_SAVE_NAVBAR_BUTTON,
     )
 
 
 def share_button_navbar_provider(
     id: str, notebook_mode: bool = True, **kwargs
 ) -> Optional[bc.Component]:
     return (
@@ -132,34 +127,103 @@
             color="light",
             size="sm",
             style={"display": "none" if notebook_mode else "inline-block"},
         ),
     )
 
 
+def create_saved_metric_dialog(saved_metric: Optional[WM.SavedMetric]) -> dbc.Modal:
+    return dbc.Modal(
+        [
+            dbc.ModalHeader(
+                (
+                    "Save new metric"
+                    if saved_metric is None
+                    else "Save new or update metric"
+                ),
+                className="lead",
+            ),
+            dbc.ModalBody(
+                [
+                    dbc.Input(
+                        value=saved_metric.name if saved_metric else "",
+                        type="text",
+                        minLength=4,
+                        maxlength=30,
+                        id=METRIC_NAME_INPUT,
+                        placeholder="Metric name",
+                    ),
+                    html.Div(id=METRIC_SAVE_DIALOG_INFO, className="text-danger mt-1"),
+                ],
+            ),
+            dbc.ModalFooter(
+                [
+                    dbc.Button(
+                        [html.I(className=("bi bi-x me-1")), "Close"],
+                        id=METRIC_SAVE_DIALOG_CLOSE_BUTTON,
+                        size="sm",
+                        color="secondary",
+                        class_name="me-1",
+                    ),
+                    dbc.Button(
+                        [
+                            html.I(className=("bi bi-check me-1")),
+                            ("Save" if saved_metric is None else "Save as new"),
+                        ],
+                        id=METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON,
+                        size="sm",
+                        color="success",
+                    ),
+                    dbc.Button(
+                        [
+                            html.I(className=("bi bi-arrow-counterclockwise me-1")),
+                            "Update",
+                        ],
+                        id=METRIC_SAVE_DIALOG_REPLACE_BUTTON,
+                        size="sm",
+                        color="primary",
+                        disabled=saved_metric is None,
+                        class_name="d-none"
+                        if saved_metric is None
+                        else "d-inline-block",
+                    ),
+                ]
+            ),
+        ],
+        id=METRIC_SAVE_DIALOG,
+        is_open=False,
+    )
+
+
 def create_explore_page(
     query_params: Dict[str, str],
     discovered_project: M.DiscoveredProject,
     storage: S.MitzuStorage,
     notebook_mode: bool = False,
 ) -> bc.Component:
     metric: Optional[M.Metric] = None
     saved_metric: Optional[WM.SavedMetric] = None
     if P.PROJECTS_EXPLORE_METRIC_QUERY in query_params:
-        metric = SE.from_compressed_string(
-            query_params[P.PROJECTS_EXPLORE_METRIC_QUERY], discovered_project.project
-        )
+        try:
+            metric = SE.from_compressed_string(
+                query_params[P.PROJECTS_EXPLORE_METRIC_QUERY],
+                discovered_project.project,
+            )
+        except Exception:
+            traceback.print_exc()
+            metric = None
     elif P.PROJECTS_EXPLORE_SAVED_METRIC_QUERY in query_params:
         saved_metric = storage.get_saved_metric(
             query_params[P.PROJECTS_EXPLORE_SAVED_METRIC_QUERY]
         )
         metric = saved_metric.metric
 
     metric_segments_div = MS.from_metric(metric, discovered_project)
     graph_container = create_graph_container(metric, discovered_project.project)
+    save_metric_dialog = create_saved_metric_dialog(saved_metric)
     navbar = NB.create_mitzu_navbar(
         id=NAVBAR_ID,
         show_metric_type=True,
         show_metric_name=True,
         metric=metric,
         saved_metric=saved_metric,
         notebook_mode=notebook_mode,
@@ -180,14 +244,15 @@
                         justify="start",
                         align="top",
                         className="g-1",
                     ),
                 ],
                 fluid=True,
             ),
+            save_metric_dialog,
         ],
         className=EXPLORE_PAGE,
         id=EXPLORE_PAGE,
     )
     return res
 
 
@@ -407,54 +472,139 @@
             return handle_input_changes(all_inputs, discovered_project)
         except Exception:
             traceback.print_exc()
             return no_update_response
 
 
 @callback(
-    Output(METRIC_NAME_PROGRESS, "className"),
-    Input(METRIC_NAME_INPUT, "value"),
+    Input(METRIC_SAVE_NAVBAR_BUTTON, "n_clicks"),
+    Input(METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON, "n_clicks"),
+    Input(METRIC_SAVE_DIALOG_REPLACE_BUTTON, "n_clicks"),
+    Input(METRIC_SAVE_DIALOG_CLOSE_BUTTON, "n_clicks"),
     State(METRIC_ID_VALUE, "children"),
+    State(METRIC_NAME_INPUT, "value"),
     State(MITZU_LOCATION, "href"),
-    background=True,
-    running=[
-        (Output(METRIC_NAME_PROGRESS, "className"), "d-inline-block", "d-none"),
-    ],
+    output={
+        METRIC_SAVE_DIALOG: Output(METRIC_SAVE_DIALOG, "is_open"),
+        METRIC_NAME_INPUT: Output(METRIC_NAME_INPUT, "value"),
+        METRIC_SAVE_DIALOG_INFO: Output(METRIC_SAVE_DIALOG_INFO, "children"),
+    },
     prevent_initial_call=True,
 )
 @restricted
-def handle_metric_name_changed(
-    metric_name: str,
+def handle_save_metric_dialog(
+    navbar_btn_nclicks: int,
+    save_new_nclicks: int,
+    replace_nclicks: int,
+    close_nclicks: int,
     metric_id: str,
+    metric_name: str,
     href: str,
-) -> str:
+) -> Dict[str, Any]:
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     storage = deps.storage
     mitzu_cache = deps.cache
-    parse_result = urlparse(href)
-    sm = storage.get_saved_metric(metric_id)
-    if sm is not None and sm.project is not None:
-        storage.clear_saved_metric(metric_id)
-        if metric_name:
-            storage.set_saved_metric(metric_id, sm.rename(metric_name))
-    else:
+    if ctx.triggered_id == METRIC_SAVE_NAVBAR_BUTTON:
+        original_name = None
+        if metric_id is not None:
+            try:
+                sm = storage.get_saved_metric(metric_id)
+                if sm is not None:
+                    original_name = sm.name
+            except ValueError:
+                original_name = None
+
+        return {
+            METRIC_SAVE_DIALOG: True,
+            METRIC_NAME_INPUT: original_name,
+            METRIC_SAVE_DIALOG_INFO: "",
+        }
+
+    if ctx.triggered_id == METRIC_SAVE_DIALOG_CLOSE_BUTTON:
+        return {
+            METRIC_SAVE_DIALOG: False,
+            METRIC_NAME_INPUT: None,
+            METRIC_SAVE_DIALOG_INFO: "",
+        }
+
+    if not metric_name:
+        return {
+            METRIC_SAVE_DIALOG: no_update,
+            METRIC_NAME_INPUT: no_update,
+            METRIC_SAVE_DIALOG_INFO: "Please name your metric.",
+        }
+    if len(metric_name) < 4:
+        return {
+            METRIC_SAVE_DIALOG: no_update,
+            METRIC_NAME_INPUT: no_update,
+            METRIC_SAVE_DIALOG_INFO: "Metric name must be at least 4 characters.",
+        }
+    if len(metric_name) > 30:
+        return {
+            METRIC_SAVE_DIALOG: no_update,
+            METRIC_NAME_INPUT: no_update,
+            METRIC_SAVE_DIALOG_INFO: "Metric name must be at most 30 characters.",
+        }
+
+    try:
+        parse_result = urlparse(href)
 
         project_id = P.get_path_value(
             P.PROJECTS_EXPLORE_PATH, parse_result.path, P.PROJECT_ID_PATH_PART
         )
         project = storage.get_project(project_id)
         metric_v64 = parse_qs(parse_result.query).get(P.PROJECTS_EXPLORE_METRIC_QUERY)
         if metric_v64 is not None:
             metric = SE.from_compressed_string(metric_v64[0], project)
-            hash_key = GH.create_metric_hash_key(metric)
-            result_df = GH.get_metric_result_df(hash_key, metric, mitzu_cache)
-            simple_chart = CHRT.get_simple_chart(metric, result_df)
-            GH.store_rendered_saved_metric(
-                metric_name=metric_name,
-                metric=metric,
-                simple_chart=simple_chart,
-                project=project,
-                storage=storage,
-                metric_id=metric_id,
-            )
 
-    return "d-none"
+        elif metric_id is not None:
+            sm = storage.get_saved_metric(metric_id)
+            if sm is None or sm.metric is None:
+                return {
+                    METRIC_SAVE_DIALOG: True,
+                    METRIC_NAME_INPUT: no_update,
+                    METRIC_SAVE_DIALOG_INFO: "Couldn't save metric. Invalid state.",
+                }
+
+            if (
+                sm.name.strip() == metric_name.strip()
+                and ctx.triggered_id == METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON
+            ):
+                return {
+                    METRIC_SAVE_DIALOG: True,
+                    METRIC_NAME_INPUT: no_update,
+                    METRIC_SAVE_DIALOG_INFO: "Make sure you give a different name to your metric.",
+                }
+            metric = sm.metric
+        else:
+            return {
+                METRIC_SAVE_DIALOG: True,
+                METRIC_NAME_INPUT: no_update,
+                METRIC_SAVE_DIALOG_INFO: "Couldn't save metric. Invalid state.",
+            }
+        hash_key = GH.create_metric_hash_key(metric)
+        result_df = GH.get_metric_result_df(hash_key, metric, mitzu_cache)
+        simple_chart = CHRT.get_simple_chart(metric, result_df)
+
+        if ctx.triggered_id == METRIC_SAVE_DIALOG_SAVE_NEW_BUTTON:
+            metric_id = H.create_unique_id()
+
+        GH.store_rendered_saved_metric(
+            metric_name=metric_name,
+            metric=metric,
+            simple_chart=simple_chart,
+            project=project,
+            storage=storage,
+            metric_id=metric_id,
+        )
+        return {
+            METRIC_SAVE_DIALOG: False,
+            METRIC_NAME_INPUT: no_update,
+            METRIC_SAVE_DIALOG_INFO: "",
+        }
+    except Exception:
+        traceback.print_exc()
+        return {
+            METRIC_SAVE_DIALOG: True,
+            METRIC_NAME_INPUT: no_update,
+            METRIC_SAVE_DIALOG_INFO: "Couldn't save metric. Something went wrong.",
+        }
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,41 +48,33 @@
 GRAPH_CONTAINER = (
     "graph_container d-flex justify-content-stretch align-items-center pt-3"
 )
 GRAPH_REFRESHER_INTERVAL = "graph_refresher_interval"
 
 
 def create_graph_container() -> bc.Component:
-    if configs.BACKGROUND_CALLBACK:
-        return html.Div(
-            id=GRAPH_CONTAINER,
-            children=[],
-            className=GRAPH_CONTAINER,
-        )
-    else:
-        return html.Div(
-            dcc.Loading(
-                id=GRAPH_CONTAINER,
-                children=[],
-                color="#287bb5",
-                type="dot",
-                className=GRAPH_CONTAINER,
-            ),
-        )
+    return html.Div(
+        id=GRAPH_CONTAINER,
+        children=[],
+        className=GRAPH_CONTAINER,
+    )
 
 
 def create_metric_hash_key(metric: M.Metric) -> str:
     metric_dict = SE.to_dict(metric)
 
     #  We need to remove these keys from the metric dict as changes in these shouldn't trigger reexecution
     metric_dict["co"]["mn"] = None
     metric_dict["co"]["mgc"] = None
     metric_dict["co"]["ct"] = None
     metric_dict["co"]["cat"] = None
     metric_dict["id"] = None
+    # The project_id is not part of the query param, but the path.
+    # However we need to use the ID as well for caching, some project may contain the same events.
+    metric_dict["prj"] = metric.get_project().get_id()
 
     return hashlib.md5(json.dumps(metric_dict).encode("ascii")).hexdigest()
 
 
 def get_metric_result_df(
     hash_key: str, metric: M.Metric, mitzu_cache: C.MitzuCache
 ) -> pd.DataFrame:
@@ -192,15 +184,15 @@
         state=dict(
             graph_content_type=State(TH.GRAPH_CONTENT_TYPE, "value"),
             href=State(MITZU_LOCATION, "href"),
             metric_name=State(EXP.METRIC_NAME_INPUT, "value"),
             metric_id=State(EXP.METRIC_ID_VALUE, "children"),
         ),
         interval=configs.GRAPH_POLL_INTERVAL_MS,
-        background=configs.BACKGROUND_CALLBACK,
+        background=True,
         running=[
             (
                 Output(TH.GRAPH_REFRESH_BUTTON, "disabled"),
                 True,
                 False,
             ),
             (
@@ -237,15 +229,16 @@
             all_inputs[EXP.METRIC_ID_VALUE] = metric_id
             all_inputs[EXP.METRIC_NAME_INPUT] = metric_name
             all_inputs[EXP.MITZU_LOCATION] = parse_result.query
             dp = project._discovered_project.get_value()
             if dp is None:
                 return html.Div(
                     [
-                        "Your project haven't been discovered yet",
+                        "Your project haven't been discovered yet. ",
+                        html.Br(),
                         dcc.Link(
                             f"Discover {project.project_name}",
                             href=P.create_path(
                                 P.EVENTS_AND_PROPERTIES_PROJECT_PATH,
                                 project_id=project.id,
                             ),
                         ),
@@ -255,15 +248,14 @@
                 )
 
             metric, _, _ = EXP.create_metric_from_all_inputs(all_inputs, dp)
 
             if metric is None:
                 return html.Div("Select an event", id=GRAPH, className=MESSAGE)
 
-            should_save_metrics = all_inputs[EXP.METRIC_NAME_INPUT] is not None
             simple_chart: CO.SimpleChart
 
             hash_key = create_metric_hash_key(metric)
             if ctx.triggered_id in (TH.GRAPH_REFRESH_BUTTON, TH.GRAPH_RUN_QUERY_BUTTON):
                 mitzu_cache.clear(hash_key)
 
             if (
@@ -271,35 +263,25 @@
                 and ctx.triggered_id != TH.GRAPH_RUN_QUERY_BUTTON
                 and mitzu_cache.get(hash_key) is None
             ):
                 return html.Div(
                     "Click run to execute the query", id=GRAPH, className=MESSAGE
                 )
 
-            if graph_content_type == TH.CHART_VAL or should_save_metrics:
+            if graph_content_type == TH.CHART_VAL:
                 result_df = get_metric_result_df(hash_key, metric, mitzu_cache)
                 simple_chart = CHRT.get_simple_chart(metric, result_df)
 
             if graph_content_type == TH.CHART_VAL:
                 res = create_graph(metric, simple_chart)  # noqa
             if graph_content_type == TH.TABLE_VAL:
                 res = create_table(metric, hash_key, mitzu_cache)
             elif graph_content_type == TH.SQL_VAL:
                 res = create_sql_area(metric)
 
-            if should_save_metrics and metric_name is not None:
-                store_rendered_saved_metric(
-                    metric_name=metric_name,
-                    metric=metric,
-                    simple_chart=simple_chart,
-                    project=project,
-                    storage=storage,
-                    metric_id=metric_id,
-                )
-
             return res
         except Exception as exc:
             traceback.print_exc()
             return html.Div(
                 [
                     html.B("Something has gone wrong. Details:"),
                     html.Pre(children=str(exc)),
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/explore_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dash import html, register_page
 
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.explore.explore_page as EXP
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted_layout
 import traceback
+import mitzu.model as M
 
 register_page(
     __name__,
     path_template=P.PROJECTS_EXPLORE_PATH,
     title="Mitzu - Explore",
 )
 
@@ -26,18 +27,15 @@
         project = depenednecies.storage.get_project(project_id)
 
         if project is None:
             return html.Div("Project not found", className="d-flex text-center lead")
 
         discovered_project = project._discovered_project.get_value()
         if discovered_project is None:
-            return html.Div(
-                "Project have not been discovered yet",
-                className="d-flex text-center lead",
-            )
+            discovered_project = M.DiscoveredProject({}, project=project)
 
         return EXP.create_explore_page(
             query_params=query_params,
             discovered_project=discovered_project,
             storage=depenednecies.storage,
         )
     except Exception as exc:
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     callback,
     Input,
     Output,
     State,
     html,
     no_update,
     ALL,
+    callback_context,
 )
 import dash_bootstrap_components as dbc
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.helper import create_form_property_input
 
@@ -128,26 +129,32 @@
             ],
             justify="center",
         ),
     ]
 
 
 @callback(
-    [Output(LOCATION, "pathname"), Output(LOGIN_ERROR, "children")],
+    [
+        Output(LOCATION, "href"),
+        Output(LOGIN_ERROR, "children"),
+    ],
     Input(BUTTON_LOGIN, "n_clicks"),
     State({"type": INDEX_TYPE, "index": ALL}, "value"),
     prevent_initial_call=True,
 )
 def login(n_click: int, inputs: List[str]):
     authorizer = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     ).authorizer
 
-    if authorizer.login_local_user(inputs[0], inputs[1]):
-        return (P.HOME_PATH, "")
+    redirect_when_authorized = authorizer.login_local_user(
+        inputs[0], inputs[1], callback_context.response
+    )
+    if redirect_when_authorized:
+        return (redirect_when_authorized, "")
     return (
         no_update,
         html.P(
             "Bad credentials",
             className="text-danger lead text-center",
         ),
     )
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_event_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
         ]
     )
 
 
 def create_event_table_component(project: Optional[M.Project]) -> bc.Component:
     rows = []
     if project is not None:
-        dp = project._discovered_project.get_value_if_exsits()
+        dp = project._discovered_project.get_value()
+        if dp is None:
+            dp = M.DiscoveredProject({}, project)
         events_service = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         ).events_service
         events_service.populate_discovered_project(dp)
 
         if dp is not None:
             for edt, df in dp.definitions.items():
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,29 +262,14 @@
     return (False, "", "")
 
 
 @callback(
     Output(SAVED_METRICS_CONTAINER, "children"),
     Input(CONFIRM_DIALOG_ACCEPT, "n_clicks"),
     State(CONFIRM_METRIC_ID, "children"),
-    background=True,
-    running=[
-        (
-            Output(SAVED_METRICS_INFO, "children"),
-            [
-                dbc.Spinner(
-                    spinner_style={"width": "1rem", "height": "1rem"},
-                    spinner_class_name="me-1",
-                ),
-                "Loading saved metrics",
-            ],
-            "",
-        )
-    ],
-    interval=200,
     prevent_initial_call=True,
 )
 @restricted
 def confirm_button_clicked(close_button: int, metric_id: str) -> List:
     storage = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     ).storage
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 PROJECT_ID_PATH_PART = "project_id"
 CONNECTION_ID_PATH_PART = "connection_id"
 USER_PATH_PART = "user_id"
 DASHBOARD_ID = "dashboard_id"
 
-ADMIN_PAGE = "/admin"
-
 EVENTS_AND_PROPERTIES_PATH = "/events"
 EVENTS_AND_PROPERTIES_PROJECT_PATH = f"/events/<{PROJECT_ID_PATH_PART}>"
 
 PROJECTS_PATH = "/projects"
 PROJECTS_CREATE_PATH = "/projects/create/"
 PROJECTS_EXPLORE_PATH = f"/projects/<{PROJECT_ID_PATH_PART}>/explore"
 PROJECTS_MANAGE_PATH = f"/projects/<{PROJECT_ID_PATH_PART}>/manage"
@@ -32,14 +30,16 @@
 SAVED_METRICS = "/saved_metrics"
 
 SIGN_OUT_URL = "/auth/logout"
 UNAUTHORIZED_URL = "/auth/unauthorized"
 REDIRECT_TO_LOGIN_URL = "/auth/redirect-to-login"
 OAUTH_CODE_URL = "/auth/oauth"
 
+HEALTHCHECK_PATH = "/ping"
+
 
 class PathException(Exception):
     pass
 
 
 def create_path(template: str, **kwargs) -> str:
     for k, v in kwargs.items():
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/projects_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,50 +98,54 @@
     project = deps.storage.get_project(project_id)
     discovered_project = project._discovered_project.get_value()
 
     tables = len(project.event_data_tables)
     events = len(discovered_project.get_all_event_names()) if discovered_project else 0
     project_jumbotron = dbc.Col(
         dbc.Card(
-            dbc.CardBody(
-                [
-                    html.H4(
-                        project.project_name,
-                        className="card-title",
-                        id=PROJECT_CARD_TITLE,
-                    ),
-                    html.Hr(),
-                    html.Img(
-                        src=f"/assets/warehouse/{str(project.connection.connection_type.name).lower()}.png",
-                        height=40,
-                    ),
-                    html.P(f"This project has {events} events in {tables} datasets."),
-                    html.P(project.description),
+            [
+                dbc.CardHeader(
+                    project.project_name, class_name="lead", id=PROJECT_CARD_TITLE
+                ),
+                dbc.CardBody(
                     html.Div(
-                        [
-                            dbc.Button(
-                                "Explore",
-                                color="primary",
-                                class_name="me-3",
-                                size="sm",
-                                href=P.create_path(
-                                    P.PROJECTS_EXPLORE_PATH, project_id=project_id
-                                ),
+                        children=[
+                            html.Img(
+                                src=f"/assets/warehouse/{str(project.connection.connection_type.name).lower()}.png",
+                                height=40,
                             ),
-                            dbc.Button(
-                                "Manage",
-                                size="sm",
-                                color="secondary",
-                                href=P.create_path(
-                                    P.PROJECTS_MANAGE_PATH, project_id=project_id
-                                ),
+                            html.P(
+                                f"This project has {events} events in {tables} datasets."
                             ),
+                            html.P(project.description),
                         ],
-                    ),
-                ]
-            ),
+                        style={"min-height": "100px"},
+                    )
+                ),
+                dbc.CardFooter(
+                    children=[
+                        dbc.Button(
+                            "Explore",
+                            color="primary",
+                            class_name="me-3",
+                            size="sm",
+                            href=P.create_path(
+                                P.PROJECTS_EXPLORE_PATH, project_id=project_id
+                            ),
+                        ),
+                        dbc.Button(
+                            "Manage",
+                            size="sm",
+                            color="secondary",
+                            href=P.create_path(
+                                P.PROJECTS_MANAGE_PATH, project_id=project_id
+                            ),
+                        ),
+                    ],
+                ),
+            ],
             class_name="mb-3",
         ),
         lg=3,
         sm=12,
     )
     return project_jumbotron
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc5/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc5/mitzu/webapp/service/events_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     def populate_discovered_project(self, discovered_project: M.DiscoveredProject):
         self.storage.populate_discovered_project(discovered_project)
 
     def get_project_definition(
         self, project_id: str
     ) -> Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]]:
         project = self.storage.get_project(project_id)
-        dp = project._discovered_project.get_value_if_exsits()
+        dp = project._discovered_project.get_value()
+        if dp is None:
+            return {}
         self.storage.populate_discovered_project(dp)
         return dp.definitions
 
     def discover_project(
         self,
         project_id: str,
         callback: Callable[
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc5/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc5/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc5/mitzu/webapp/service/user_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Optional, Tuple
 import random
 import string
 import hashlib
 import mitzu.webapp.storage as S
 import mitzu.webapp.configs as configs
 import mitzu.webapp.model as WM
+import mitzu.webapp.service.notification_service as NS
+import mitzu.helper as H
 
 
 class UserNotFoundException(Exception):
     """
     Raised when the user is not found in the local user store
     """
 
@@ -46,30 +48,36 @@
 
 
 class UserService:
     """
     UserService provides the a single API to manage users in the local user storage
     """
 
-    def __init__(self, storage: S.MitzuStorage, root_password: Optional[str] = None):
+    def __init__(
+        self,
+        storage: S.MitzuStorage,
+        notification_service: Optional[NS.NotificationService] = None,
+    ):
         self._storage = storage
 
-        has_admin = False
-        for user in self.list_users():
-            if user.role == WM.Role.ADMIN:
-                has_admin = True
-                break
-
-        if root_password and not has_admin:
-            self.new_user(
-                configs.AUTH_ROOT_USER_EMAIL,
-                root_password,
-                root_password,
-                role=WM.Role.ADMIN,
-            )
+        if notification_service:
+            self._notification_service = notification_service
+        else:
+            self._notification_service = NS.DummyNotificationService()
+
+        try:
+            if configs.AUTH_ROOT_USER_EMAIL:
+                self.new_user(
+                    configs.AUTH_ROOT_USER_EMAIL,
+                    configs.AUTH_ROOT_PASSWORD,
+                    configs.AUTH_ROOT_PASSWORD,
+                    role=WM.Role.ADMIN,
+                )
+        except UserAlreadyExists:
+            H.LOGGER.info(f"Root user {configs.AUTH_ROOT_USER_EMAIL} already exists.")
 
     def list_users(self) -> List[WM.User]:
         return self._storage.list_users()
 
     def get_user_by_id(self, user_id: str) -> Optional[WM.User]:
         return self._storage.get_user_by_id(user_id)
 
@@ -115,32 +123,33 @@
         password: Optional[str] = None,
         password_confirmation: Optional[str] = None,
         role: WM.Role = WM.Role.MEMBER,
     ) -> str:
         if self.get_user_by_email(email) is not None:
             raise UserAlreadyExists()
 
+        hash = None
+        salt = None
         if password is not None:
             if password != password_confirmation:
                 raise UserPasswordAndConfirmationDoNotMatch()
 
             if len(password) < 8:
                 raise UserPasswordRequirementsNotMet()
 
             hash, salt = self._get_password_hash_with_salt(password)
-        else:
-            raise UserPasswordRequirementsNotMet()
 
         user = WM.User(
             email=email,
             password_hash=hash,
             password_salt=salt,
             role=role,
         )
         self._storage.set_user(user)
+        self._notification_service.user_created(user.id, user.email)
         return user.id
 
     def get_user_by_email_and_password(
         self, email: str, password: str
     ) -> Optional[WM.User]:
         user = self.get_user_by_email(email)
         if user is None:
@@ -154,7 +163,8 @@
 
     def delete_user(self, user_id: str):
         user = self.get_user_by_id(user_id)
         if user is None:
             raise UserNotFoundException()
 
         self._storage.clear_user(user_id)
+        self._notification_service.user_deleted(user.id)
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/storage.py` & `mitzu-0.6.0rc5/mitzu/webapp/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 class MitzuStorage:
     def __init__(
         self,
         connection_string: str = "sqlite://?check_same_thread=False",
     ) -> None:
-        self._engine = SA.create_engine(connection_string)
+        self._engine = SA.create_engine(connection_string, pool_pre_ping=True)
         self._is_sqlite = connection_string.startswith("sqlite")
         self.__init_schema()
 
     @property
     def _session(self) -> Session:
         if flask.has_app_context():
             if "request_session_cache" not in flask.g:
@@ -590,7 +590,11 @@
             session.query(SM.UserStorageRecord)
             .filter(SM.UserStorageRecord.user_id == user_id)
             .first()
         )
         if record is not None:
             session.delete(record)
             session.commit()
+
+    def health_check(self):
+        session = self._session
+        session.execute("select 1")
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc5/mitzu/webapp/storage_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,24 @@
     return json.dumps(
         {
             "_name": field._name,
             "_type": field._type.value,
             "_sub_fields": [serialize_field(f) for f in field._sub_fields]
             if field._sub_fields
             else None,
-            "_parent": serialize_field(field._parent) if field._parent else None,
         }
     )
 
 
 def deserialize_field(serialized: str) -> M.Field:
     data = json.loads(serialized)
     return M.Field(
         _name=data["_name"],
         _type=M.DataType(data["_type"]),
         _sub_fields=data["_sub_fields"],
-        _parent=data["_parent"],
     )
 
 
 class UserStorageRecord(Base):
     __tablename__ = "users"
 
     user_id = SA.Column(SA.String, primary_key=True)
@@ -490,18 +488,18 @@
         )
 
     @classmethod
     def from_model_instance(
         self, event_data_table_id: str, event_def: M.EventDef
     ) -> EventDefStorageRecord:
         fields = []
-        for field_name, field_def in event_def._fields.items():
+        for field, field_def in event_def._fields.items():
             fields.append(
                 {
-                    "_key": serialize_field(field_name),
+                    "_key": serialize_field(field),
                     "_event_name": field_def._event_name,
                     "_field": serialize_field(field_def._field),
                     "_event_data_table_id": field_def._event_data_table.id,
                     "_description": field_def._description,
                     "_enums": field_def._enums,
                 }
             )
@@ -569,15 +567,15 @@
             title=data["title"],
             x_axis_label=data["x_axis_label"],
             y_axis_label=data["y_axis_label"],
             color_label=data["color_label"],
             yaxis_ticksuffix=data["yaxis_ticksuffix"],
             hover_mode=data["hover_mode"],
             chart_type=M.SimpleChartType(data["chart_type"]),
-            dataframe=pickle.loads(base64.b64decode(data["dataframe"])),
+            dataframe=pickle.loads(base64.urlsafe_b64decode(data["dataframe"])),
         )
 
     @classmethod
     def __simple_chart_to_dict(self, chart: VC.SimpleChart) -> Dict[str, Any]:
         f = io.BytesIO()
         pickle.dump(chart.dataframe, f)
         f.seek(0)
@@ -586,15 +584,15 @@
             "title": chart.title,
             "x_axis_label": chart.x_axis_label,
             "y_axis_label": chart.y_axis_label,
             "color_label": chart.color_label,
             "yaxis_ticksuffix": chart.yaxis_ticksuffix,
             "hover_mode": chart.hover_mode,
             "chart_type": chart.chart_type.value,
-            "dataframe": base64.b64encode(f.read()).decode(),
+            "dataframe": base64.urlsafe_b64encode(f.read()).decode(),
             # FIXME: label funcs are not serialized
         }
 
     @classmethod
     def from_model_instance(
         self, saved_metric: WM.SavedMetric
     ) -> SavedMetricStorageRecord:
```

### Comparing `mitzu-0.6.0rc4/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc5/mitzu/webapp/webapp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 from typing import Optional, cast
 
 import dash.development.base_component as bc
 import dash_bootstrap_components as dbc
 import flask
-from dash import CeleryManager, Dash, DiskcacheManager, dcc, html, page_container
+from dash import Dash, DiskcacheManager, dcc, html, page_container
 from dash.long_callback.managers import BaseLongCallbackManager
+import mitzu.webapp.cache as C
 
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 import mitzu.webapp.offcanvas as OC
 import mitzu.webapp.pages.explore.explore_page as EXP
+import mitzu.webapp.pages.paths as P
 from mitzu.helper import LOGGER
-
+import json
+import traceback
 from mitzu.webapp.helper import MITZU_LOCATION
 
 MAIN = "main"
 
 MDB_CSS = "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.0.1/mdb.min.css"
 DCC_DBC_CSS = (
     "https://cdn.jsdelivr.net/gh/AnnMarieW/dash-bootstrap-templates/dbc.min.css"
@@ -33,33 +36,15 @@
         children=[location, offcanvas, page_container],
         className=MAIN,
         id=MAIN,
     )
 
 
 def get_callback_manager(dependencies: DEPS.Dependencies) -> BaseLongCallbackManager:
-    if configs.QUEUE_REDIS_HOST is not None:
-        from celery import Celery
-
-        celery_app = Celery(
-            __name__, broker=configs.QUEUE_REDIS_HOST, backend=configs.QUEUE_REDIS_HOST
-        )
-        return CeleryManager(
-            celery_app,
-            cache_by=[lambda: configs.LAUNCH_UID],
-            expire=configs.CACHE_EXPIRATION,
-        )
-    else:
-        import mitzu.webapp.cache as C
-
-        return DiskcacheManager(
-            cast(C.DiskMitzuCache, dependencies.queue).get_disk_cache(),
-            cache_by=[lambda: configs.LAUNCH_UID],
-            expire=configs.CACHE_EXPIRATION,
-        )
+    return DiskcacheManager(cast(C.DiskMitzuCache, dependencies.queue).get_disk_cache())
 
 
 def create_dash_app(dependencies: Optional[DEPS.Dependencies] = None) -> Dash:
     server = flask.Flask(__name__)
     if dependencies is None:
         dependencies = DEPS.Dependencies.from_configs()
 
@@ -83,50 +68,57 @@
     dependencies.navbar_service.register_navbar_item_provider(
         "left",
         EXP.metric_type_navbar_provider,
         priority=20,
     )
     dependencies.navbar_service.register_navbar_item_provider(
         "left",
-        EXP.metric_name_navbar_provider,
-        priority=30,
+        EXP.save_metric_navbar_provider,
+        priority=40,
     )
     dependencies.navbar_service.register_navbar_item_provider(
         "left",
         EXP.share_button_navbar_provider,
-        priority=40,
+        priority=30,
     )
 
     app = Dash(
         __name__,
-        compress=configs.DASH_COMPRESS_RESPONSES,
+        compress=True,
         server=server,
         external_stylesheets=[
             MDB_CSS,
             dbc.icons.BOOTSTRAP,
             "/assets/explore_page.css",
         ],
-        assets_folder=configs.DASH_ASSETS_FOLDER,
-        assets_url_path=configs.DASH_ASSETS_URL_PATH,
-        serve_locally=configs.DASH_SERVE_LOCALLY,
         title=configs.DASH_TITLE,
         update_title=None,
         suppress_callback_exceptions=True,
         use_pages=True,
         background_callback_manager=get_callback_manager(dependencies),
-        external_scripts=[
-            "https://cdnjs.cloudflare.com/ajax/libs/dragula/3.7.2/dragula.min.js"
-        ],
     )
     app._favicon = configs.DASH_FAVICON_PATH
     app.layout = create_webapp_layout(dependencies)
 
-    @server.route(configs.HEALTH_CHECK_PATH)
+    @server.route(P.HEALTHCHECK_PATH)
     def healthcheck():
-        return flask.Response("ok", status=200)
+        dependencies: DEPS.Dependencies = cast(
+            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
+        )
+        try:
+            # These will fail with exception if there is an underlying issue
+            dependencies.queue.health_check()
+            dependencies.cache.health_check()
+            dependencies.storage.health_check()
+        except Exception as exc:
+            traceback.print_exc()
+            return flask.Response(
+                json.dumps({"status": "fail", "message": str(exc)}), status=500
+            )
+        return flask.Response('{"status": "ok"}', status=200)
 
     return app
 
 
 if __name__ == "__main__":
     app = create_dash_app()
```

### Comparing `mitzu-0.6.0rc4/pyproject.toml` & `mitzu-0.6.0rc5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.4"
+version = "0.6.0-rc.5"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc4/PKG-INFO` & `mitzu-0.6.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc4
+Version: 0.6.0rc5
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

