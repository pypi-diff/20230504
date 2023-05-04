# Comparing `tmp/dbt-athena-community-1.4.4.tar.gz` & `tmp/dbt-athena-community-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.4.4.tar", last modified: Wed May  3 08:00:02 2023, max compression
+gzip compressed data, was "dbt-athena-community-1.4.5.tar", last modified: Thu May  4 10:11:45 2023, max compression
```

## Comparing `dbt-athena-community-1.4.4.tar` & `dbt-athena-community-1.4.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31197 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/ddl_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22332 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32056 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.844940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.848940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/ddl_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 10:11:45.000000 dbt-athena-community-1.4.5/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:11:45.852940 dbt-athena-community-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-04 10:11:30.000000 dbt-athena-community-1.4.5/setup.py
```

### Comparing `dbt-athena-community-1.4.4/LICENSE.txt` & `dbt-athena-community-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/PKG-INFO` & `dbt-athena-community-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.4.4
+Version: 1.4.5
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
+License: Apache License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.4.*`
-* Supports [Seeds][seeds]
+* Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
-  * [Iceberg tables][athena-iceberg] is supported **only with Athena Engine v3** and **a unique table location**
+  * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
-  * Hive tables is supported by both Athena engines.
+  * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
-  * On iceberg tables :
-    * Support the use of `unique_key` only with the `merge` strategy
-    * Support the `append` strategy
+  * On Iceberg tables :
+    * Supports the use of `unique_key` only with the `merge` strategy
+    * Supports the `append` strategy
   * On Hive tables :
-    * Support two incremental update strategies: `insert_overwrite` and `append`
+    * Supports two incremental update strategies: `insert_overwrite` and `append`
     * Does **not** support the use of `unique_key`
 * Supports [snapshots][snapshots]
 * Does not support [Python models][python-models]
 * Does not support [persist docs][persist-docs] for views
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 [incremental]: https://docs.getdbt.com/docs/build/incremental-models
@@ -67,15 +79,15 @@
 
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
 You can either:
 - configure `aws_access_key_id` and `aws_secret_access_key`
 - configure `aws_profile_name` to match a profile defined in your AWS credentials file
-Checkout DBT profile configuration below for details.
+Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                    | Required? | Example                                    |
 |-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
@@ -145,33 +157,35 @@
 * `lf_tags` (`default=none`)
   * lf tags to associate with the table
   * format: `{"tag1": "value1", "tag2": "value2"}`
 * `lf_tags_columns` (`default=none`)
   * lf tags to associate with the table columns
   * format: `{"tag1": {"value1": ["column1": "column2"]}}`
 
+[create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+
 ### Table location
 
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
-3. If `s3_data_dir` is not defined data is stored under `s3_staging_dir/tables/`
+3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 * `uuid`: `{s3_data_dir}/{uuid4()}/`
-* `table_table`: `{s3_data_dir}/{table}/`
+* `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
 
-> Note: when using a work group with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the work group is used.
+> Note: when using a workgroup with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the workgroup is used.
 
 ### Incremental models
 
 Support for [incremental models](https://docs.getdbt.com/docs/build/incremental-models).
 
 These strategies are supported:
 
@@ -188,83 +202,83 @@
 `on_schema_change` is an option to reflect changes of schema in incremental models.
 The following options are supported:
 * `ignore` (default)
 * `fail`
 * `append_new_columns`
 * `sync_all_columns`
 
-In detail, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
+For details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
 
 ### Iceberg
 
 The adapter supports table materialization for Iceberg.
 
 To get started just add this as your model:
-```
+```sql
 {{ config(
     materialized='table',
     table_type='iceberg',
     format='parquet',
     partitioned_by=['bucket(user_id, 5)'],
     table_properties={
     	'optimize_rewrite_delete_file_threshold': '2'
     	}
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
-It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
+It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
    It performs an upsert, new record are added, and record already existing are updated. If
    `delete_condition` is provided in the model config, it can also delete records based on the
    provided condition (SQL condition). You can use any column of the incremental table (`src`) or
    the final table (`target`). You must prefix the column by the name of the table to prevent
    `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
-    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
-    format='parquet',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
+    format='parquet'
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
-### High available table materialization
+### High availability table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
-the target table to the location of the tmp table.
-This materialization is only available for `table_type=hive` and requires using unique locations.
+**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
+the target table to the location of the temp table.
+This materialization is only available for `table_type='hive'` and requires using unique locations.
 
-```
+```sql
 {{ config(
     materialized='table_hive_ha',
     format='parquet',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
@@ -275,27 +289,27 @@
 union all
 select
   'b' as user_id,
   'sh' as user_name,
   'disabled' as status
 ```
 
-By default, the materialization keeps the last 4 table versions, you can change it that setting `versions_to_keep`.
+By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
 #### Known issues
 * When swapping from a table with partitions to a table without (and the other way around), there could be a little downtime.
   In case high performances are needed consider bucketing instead of partitions
-* By default, Glue "duplicate" the versions internally, so the last 2 versions of a table point to the same location
-* It's recommended to have versions_to_keep>= 4, as this will avoid to have the older location removed
-* The macro athena__end_of_time needs to be overwritten by the user if using Athena v3 since it requires a precision parameter for timestamps
+* By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
+* It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+* The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a precision parameter for timestamps
 
 
 ## Snapshots
 
-The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If directory does not exist create one.
+The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
 To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended)
 
 ### Check strategy
 
@@ -328,77 +342,78 @@
 MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468,
 MEIM.S1WA,2000.09,72462,
 MEIM.S1WA,2000.1,74897,
 ```
 
 model.sql
-```
+```sql
 {{ config(
     materialized='table'
 ) }}
 
-SELECT
-    ROW_NUMBER() OVER () AS id
+select
+    row_number() over() as id
     , *
-    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS refresh_timestamp
-FROM {{ ref('employment_indicators_november_2022_csv_tables') }}
+    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
 ```
 
 timestamp strategy - model_snapshot_1
 
-```
+```sql
 {% snapshot model_snapshot_1 %}
 
 {{
     config(
       strategy='timestamp',
       updated_at='refresh_timestamp',
       unique_key='id'
     )
 }}
 
-SELECT *
-
+select *
 from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 invalidate hard deletes - model_snapshot_2
-```
+```sql
 {% snapshot model_snapshot_2 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='timestamp',
         updated_at='refresh_timestamp',
         invalidate_hard_deletes=True,
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 check strategy - model_snapshot_3
-```
+```sql
 {% snapshot model_snapshot_3 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='check',
         check_cols=['series_reference','data_value']
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 ### Known issues
 
 * Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
@@ -437,14 +452,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,26 +1,33 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.4 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.5 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena Description-Content-Type: text/markdown License-File:
-LICENSE.txt
+dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [Seeds][seeds] *
+## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
-[table] * [Iceberg tables][athena-iceberg] is supported **only with Athena
+[table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
-* Hive tables is supported by both Athena engines. * Supports [incremental
-models][incremental] * On iceberg tables : * Support the use of `unique_key`
-only with the `merge` strategy * Support the `append` strategy * On Hive tables
-: * Support two incremental update strategies: `insert_overwrite` and `append`
-* Does **not** support the use of `unique_key` * Supports [snapshots]
+* Hive tables are supported by both Athena engines. * Supports [incremental
+models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
+only with the `merge` strategy * Supports the `append` strategy * On Hive
+tables : * Supports two incremental update strategies: `insert_overwrite` and
+`append` * Does **not** support the use of `unique_key` * Supports [snapshots]
 [snapshots] * Does not support [Python models][python-models] * Does not
 support [persist docs][persist-docs] for views [seeds]: https://
 docs.getdbt.com/docs/building-a-dbt-project/seeds [incremental]: https://
 docs.getdbt.com/docs/build/incremental-models [table]: https://docs.getdbt.com/
 docs/build/materializations#table [python-models]: https://docs.getdbt.com/
 docs/build/python-models#configuring-python-models [athena-iceberg]: https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html [snapshots]: https:/
@@ -35,15 +42,15 @@
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
 Athena databases. ### Credentials Credentials can be passed directly to the
 adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
 v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
 conventions. You can either: - configure `aws_access_key_id` and
 `aws_secret_access_key` - configure `aws_profile_name` to match a profile
-defined in your AWS credentials file Checkout DBT profile configuration below
+defined in your AWS credentials file Checkout dbt profile configuration below
 for details. ### Configuring your profile A dbt profile can be configured to
 run against AWS Athena using the following configuration: | Option |
 Description | Required? | Example | |-----------------------|------------------
 --------------------------------------------------------------|-----------|----
 ----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
@@ -83,135 +90,136 @@
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` ### Table location The location
-in which a table is saved is determined by: 1. If `external_location` is
-defined, that value is used. 2. If `s3_data_dir` is defined, the path is
-determined by that and `s3_data_naming` 3. If `s3_data_dir` is not defined data
-is stored under `s3_staging_dir/tables/` Here all the options available for
-`s3_data_naming`: * `uuid`: `{s3_data_dir}/{uuid4()}/` * `table_table`: `
-{s3_data_dir}/{table}/` * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` *
-`schema_table`: `{s3_data_dir}/{schema}/{table}/` *
-`s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4
-()}/` It's possible to set the `s3_data_naming` globally in the target profile,
-or overwrite the value in the table config, or setting up the value for groups
-of model in dbt_project.yml. > Note: when using a work group with a default
-output location configured, `s3_data_naming` and any configured buckets are
-ignored and the location configured in the work group is used. ### Incremental
-models Support for [incremental models](https://docs.getdbt.com/docs/build/
-incremental-models). These strategies are supported: * `insert_overwrite`
-(default): The insert overwrite strategy deletes the overlapping partitions
-from the destination table, and then inserts the new records from the source.
-This strategy depends on the `partitioned_by` keyword! If no partitions are
-defined, dbt will fall back to the `append` strategy. * `append`: Insert new
-records without updating, deleting or overwriting any existing data. There
-might be duplicate data (e.g. great for log or historical data). * `merge`:
-Conditionally updates, deletes, or inserts rows into an Iceberg table. Used in
-combination with `unique_key`. Only available when using Iceberg. ### On schema
-change `on_schema_change` is an option to reflect changes of schema in
-incremental models. The following options are supported: * `ignore` (default) *
-`fail` * `append_new_columns` * `sync_all_columns` In detail, please refer to
-[dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-
-columns-of-my-incremental-model-change). ### Iceberg The adapter supports table
-materialization for Iceberg. To get started just add this as your model: ``` {
-{ config( materialized='table', table_type='iceberg', format='parquet',
-partitioned_by=['bucket(user_id, 5)'], table_properties=
-{ 'optimize_rewrite_delete_file_threshold': '2' } ) }} SELECT 'A' AS user_id,
-'pi' AS name, 'active' AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS
-quantity_big, current_date AS my_date ``` Iceberg supports bucketing as hidden
-partitions, therefore use the `partitioned_by` config to add specific bucketing
-conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
-and `ORC`. It is possible to use iceberg in an incremental fashion,
-specifically 2 strategies are supported: * `append`: new records are appended
-to the table, this can lead to duplicates * `merge`: must be used in
-combination with `unique_key` and it's only available with Engine version 3. It
-performs an upsert, new record are added, and record already existing are
-updated. If `delete_condition` is provided in the model config, it can also
-delete records based on the provided condition (SQL condition). You can use any
-column of the incremental table (`src`) or the final table (`target`). You must
-prefix the column by the name of the table to prevent `Column is ambiguous`
-error. ```sql {{ config( materialized='incremental', table_type='iceberg',
-incremental_strategy='merge', unique_key='user_id',
+{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+### Table location The location in which a table is saved is determined by: 1.
+If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
+defined, the path is determined by that and `s3_data_naming` 3. If
+`s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
+` Here all the options available for `s3_data_naming`: * `uuid`: `
+{s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
+`{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
+{table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
+{table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
+target profile, or overwrite the value in the table config, or setting up the
+value for groups of model in dbt_project.yml. > Note: when using a workgroup
+with a default output location configured, `s3_data_naming` and any configured
+buckets are ignored and the location configured in the workgroup is used. ###
+Incremental models Support for [incremental models](https://docs.getdbt.com/
+docs/build/incremental-models). These strategies are supported: *
+`insert_overwrite` (default): The insert overwrite strategy deletes the
+overlapping partitions from the destination table, and then inserts the new
+records from the source. This strategy depends on the `partitioned_by` keyword!
+If no partitions are defined, dbt will fall back to the `append` strategy. *
+`append`: Insert new records without updating, deleting or overwriting any
+existing data. There might be duplicate data (e.g. great for log or historical
+data). * `merge`: Conditionally updates, deletes, or inserts rows into an
+Iceberg table. Used in combination with `unique_key`. Only available when using
+Iceberg. ### On schema change `on_schema_change` is an option to reflect
+changes of schema in incremental models. The following options are supported: *
+`ignore` (default) * `fail` * `append_new_columns` * `sync_all_columns` For
+details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/
+incremental-models#what-if-the-columns-of-my-incremental-model-change). ###
+Iceberg The adapter supports table materialization for Iceberg. To get started
+just add this as your model: ```sql {{ config( materialized='table',
+table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
+table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
+'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
+100000000 as quantity_big, current_date as my_date ``` Iceberg supports
+bucketing as hidden partitions, therefore use the `partitioned_by` config to
+add specific bucketing conditions. Iceberg supports several table formats for
+data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
+incremental fashion, specifically two strategies are supported: * `append`: new
+records are appended to the table, this can lead to duplicates * `merge`: must
+be used in combination with `unique_key` and it's only available with Engine
+version 3. It performs an upsert, new record are added, and record already
+existing are updated. If `delete_condition` is provided in the model config, it
+can also delete records based on the provided condition (SQL condition). You
+can use any column of the incremental table (`src`) or the final table
+(`target`). You must prefix the column by the name of the table to prevent
+`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
+table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
-'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
-AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
-current_date AS my_date ``` ### High available table materialization The
+'2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
+as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
+current_date as my_date ``` ### High availability table materialization The
 current implementation of the table materialization can lead to downtime, as
 target table is dropped and re-created. To have the less destructive behavior
 it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverage the table versions feature of glue catalog, creating a tmp table and
-swapping the target table to the location of the tmp table. This
-materialization is only available for `table_type=hive` and requires using
-unique locations. ``` {{ config( materialized='table_hive_ha',
+leverages the table versions feature of Glue catalog, creating a temp table and
+swapping the target table to the location of the temp table. This
+materialization is only available for `table_type='hive'` and requires using
+unique locations. ```sql {{ config( materialized='table_hive_ha',
 format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
 select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it that setting
+materialization keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
-instead of partitions * By default, Glue "duplicate" the versions internally,
-so the last 2 versions of a table point to the same location * It's recommended
-to have versions_to_keep>= 4, as this will avoid to have the older location
-removed * The macro athena__end_of_time needs to be overwritten by the user if
-using Athena v3 since it requires a precision parameter for timestamps ##
-Snapshots The adapter supports snapshot materialization. It supports both
-timestamp and check strategy. To create a snapshot create a snapshot file in
-the snapshots directory. If directory does not exist create one. ### Timestamp
-strategy To use the timestamp strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
-strategy To use the check strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
-materialization also supports invalidating hard deletes. Check the [docs]
-(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+instead of partitions * By default, Glue "duplicates" the versions internally,
+so the last two versions of a table point to the same location * It's
+recommended to have `versions_to_keep` >= 4, as this will avoid having the
+older location removed * The macro `athena__end_of_time` needs to be
+overwritten by the user if using Athena engine v3 since it requires a precision
+parameter for timestamps ## Snapshots The adapter supports snapshot
+materialization. It supports both timestamp and check strategy. To create a
+snapshot create a snapshot file in the snapshots directory. If the directory
+does not exist create one. ### Timestamp strategy To use the timestamp strategy
+refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
+strategy-recommended) ### Check strategy To use the check strategy refer to the
+[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
+Hard-deletes The materialization also supports invalidating hard deletes. Check
+the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
-model.sql ``` {{ config( materialized='table' ) }} SELECT ROW_NUMBER() OVER ()
-AS id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS
-refresh_timestamp FROM {{ ref('employment_indicators_november_2022_csv_tables')
-}} ``` timestamp strategy - model_snapshot_1 ``` {% snapshot model_snapshot_1
-%} {{ config( strategy='timestamp', updated_at='refresh_timestamp',
-unique_key='id' ) }} SELECT * from {{ ref('model') }} {% endsnapshot %} ```
-invalidate hard deletes - model_snapshot_2 ``` {% snapshot model_snapshot_2 %}
-{{ config ( unique_key='id', strategy='timestamp',
-updated_at='refresh_timestamp', invalidate_hard_deletes=True, ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` check strategy - model_snapshot_3
-``` {% snapshot model_snapshot_3 %} {{ config ( unique_key='id',
-strategy='check', check_cols=['series_reference','data_value'] ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` ### Known issues * Incremental
-Iceberg models - Sync all columns on schema change can't remove columns used as
-partitioning. The only way, from a dbt perspective, is to do a full-refresh of
-the incremental model. * Tables, schemas and database should only be lowercase
-* In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
-(https://github.com/Tomme/dbt-athena) is not installed in the target
-environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
-details. * Snapshot does not support dropping columns from the source table. If
-you drop a column make sure to drop the column from the snapshot as well.
-Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)):
-        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
-         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
-      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
-                               ð ð§                                                           Lee
-                                                                                                           ð
-      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
-       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
-             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+model.sql ```sql {{ config( materialized='table' ) }} select row_number() over
+() as id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as
+refresh_timestamp from {{ ref('employment_indicators_november_2022_csv_tables')
+}} ``` timestamp strategy - model_snapshot_1 ```sql {% snapshot
+model_snapshot_1 %} {{ config( strategy='timestamp',
+updated_at='refresh_timestamp', unique_key='id' ) }} select * from {{ ref
+('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
+```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
+strategy='timestamp', updated_at='refresh_timestamp',
+invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
+model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
+['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` ### Known issues * Incremental Iceberg models - Sync all
+columns on schema change can't remove columns used as partitioning. The only
+way, from a dbt perspective, is to do a full-refresh of the incremental model.
+* Tables, schemas and database should only be lowercase * In order to avoid
+potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
+dbt-athena) is not installed in the target environment. See https://github.com/
+dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
+dropping columns from the source table. If you drop a column make sure to drop
+the column from the snapshot as well. Another workaround is to NULL the column
+in the snapshot definition to preserve history ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
+                               ð ð§                                                                    Lee
+                                                                                                                    ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko      ð» ð
                                              Reinaldo                             ð» ð
                                                ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.4/README.md` & `dbt-athena-community-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.4.*`
-* Supports [Seeds][seeds]
+* Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
-  * [Iceberg tables][athena-iceberg] is supported **only with Athena Engine v3** and **a unique table location**
+  * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
-  * Hive tables is supported by both Athena engines.
+  * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
-  * On iceberg tables :
-    * Support the use of `unique_key` only with the `merge` strategy
-    * Support the `append` strategy
+  * On Iceberg tables :
+    * Supports the use of `unique_key` only with the `merge` strategy
+    * Supports the `append` strategy
   * On Hive tables :
-    * Support two incremental update strategies: `insert_overwrite` and `append`
+    * Supports two incremental update strategies: `insert_overwrite` and `append`
     * Does **not** support the use of `unique_key`
 * Supports [snapshots][snapshots]
 * Does not support [Python models][python-models]
 * Does not support [persist docs][persist-docs] for views
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 [incremental]: https://docs.getdbt.com/docs/build/incremental-models
@@ -59,15 +59,15 @@
 
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
 You can either:
 - configure `aws_access_key_id` and `aws_secret_access_key`
 - configure `aws_profile_name` to match a profile defined in your AWS credentials file
-Checkout DBT profile configuration below for details.
+Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                    | Required? | Example                                    |
 |-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
@@ -137,33 +137,35 @@
 * `lf_tags` (`default=none`)
   * lf tags to associate with the table
   * format: `{"tag1": "value1", "tag2": "value2"}`
 * `lf_tags_columns` (`default=none`)
   * lf tags to associate with the table columns
   * format: `{"tag1": {"value1": ["column1": "column2"]}}`
 
+[create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+
 ### Table location
 
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
-3. If `s3_data_dir` is not defined data is stored under `s3_staging_dir/tables/`
+3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 * `uuid`: `{s3_data_dir}/{uuid4()}/`
-* `table_table`: `{s3_data_dir}/{table}/`
+* `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
 
-> Note: when using a work group with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the work group is used.
+> Note: when using a workgroup with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the workgroup is used.
 
 ### Incremental models
 
 Support for [incremental models](https://docs.getdbt.com/docs/build/incremental-models).
 
 These strategies are supported:
 
@@ -180,83 +182,83 @@
 `on_schema_change` is an option to reflect changes of schema in incremental models.
 The following options are supported:
 * `ignore` (default)
 * `fail`
 * `append_new_columns`
 * `sync_all_columns`
 
-In detail, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
+For details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
 
 ### Iceberg
 
 The adapter supports table materialization for Iceberg.
 
 To get started just add this as your model:
-```
+```sql
 {{ config(
     materialized='table',
     table_type='iceberg',
     format='parquet',
     partitioned_by=['bucket(user_id, 5)'],
     table_properties={
     	'optimize_rewrite_delete_file_threshold': '2'
     	}
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
-It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
+It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
    It performs an upsert, new record are added, and record already existing are updated. If
    `delete_condition` is provided in the model config, it can also delete records based on the
    provided condition (SQL condition). You can use any column of the incremental table (`src`) or
    the final table (`target`). You must prefix the column by the name of the table to prevent
    `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
-    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
-    format='parquet',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
+    format='parquet'
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
-### High available table materialization
+### High availability table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
-the target table to the location of the tmp table.
-This materialization is only available for `table_type=hive` and requires using unique locations.
+**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
+the target table to the location of the temp table.
+This materialization is only available for `table_type='hive'` and requires using unique locations.
 
-```
+```sql
 {{ config(
     materialized='table_hive_ha',
     format='parquet',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
@@ -267,27 +269,27 @@
 union all
 select
   'b' as user_id,
   'sh' as user_name,
   'disabled' as status
 ```
 
-By default, the materialization keeps the last 4 table versions, you can change it that setting `versions_to_keep`.
+By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
 #### Known issues
 * When swapping from a table with partitions to a table without (and the other way around), there could be a little downtime.
   In case high performances are needed consider bucketing instead of partitions
-* By default, Glue "duplicate" the versions internally, so the last 2 versions of a table point to the same location
-* It's recommended to have versions_to_keep>= 4, as this will avoid to have the older location removed
-* The macro athena__end_of_time needs to be overwritten by the user if using Athena v3 since it requires a precision parameter for timestamps
+* By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
+* It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+* The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a precision parameter for timestamps
 
 
 ## Snapshots
 
-The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If directory does not exist create one.
+The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
 To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended)
 
 ### Check strategy
 
@@ -320,77 +322,78 @@
 MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468,
 MEIM.S1WA,2000.09,72462,
 MEIM.S1WA,2000.1,74897,
 ```
 
 model.sql
-```
+```sql
 {{ config(
     materialized='table'
 ) }}
 
-SELECT
-    ROW_NUMBER() OVER () AS id
+select
+    row_number() over() as id
     , *
-    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS refresh_timestamp
-FROM {{ ref('employment_indicators_november_2022_csv_tables') }}
+    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
 ```
 
 timestamp strategy - model_snapshot_1
 
-```
+```sql
 {% snapshot model_snapshot_1 %}
 
 {{
     config(
       strategy='timestamp',
       updated_at='refresh_timestamp',
       unique_key='id'
     )
 }}
 
-SELECT *
-
+select *
 from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 invalidate hard deletes - model_snapshot_2
-```
+```sql
 {% snapshot model_snapshot_2 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='timestamp',
         updated_at='refresh_timestamp',
         invalidate_hard_deletes=True,
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 check strategy - model_snapshot_3
-```
+```sql
 {% snapshot model_snapshot_3 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='check',
         check_cols=['series_reference','data_value']
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 ### Known issues
 
 * Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
@@ -429,14 +432,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [Seeds][seeds] *
+## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
-[table] * [Iceberg tables][athena-iceberg] is supported **only with Athena
+[table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
-* Hive tables is supported by both Athena engines. * Supports [incremental
-models][incremental] * On iceberg tables : * Support the use of `unique_key`
-only with the `merge` strategy * Support the `append` strategy * On Hive tables
-: * Support two incremental update strategies: `insert_overwrite` and `append`
-* Does **not** support the use of `unique_key` * Supports [snapshots]
+* Hive tables are supported by both Athena engines. * Supports [incremental
+models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
+only with the `merge` strategy * Supports the `append` strategy * On Hive
+tables : * Supports two incremental update strategies: `insert_overwrite` and
+`append` * Does **not** support the use of `unique_key` * Supports [snapshots]
 [snapshots] * Does not support [Python models][python-models] * Does not
 support [persist docs][persist-docs] for views [seeds]: https://
 docs.getdbt.com/docs/building-a-dbt-project/seeds [incremental]: https://
 docs.getdbt.com/docs/build/incremental-models [table]: https://docs.getdbt.com/
 docs/build/materializations#table [python-models]: https://docs.getdbt.com/
 docs/build/python-models#configuring-python-models [athena-iceberg]: https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html [snapshots]: https:/
@@ -31,15 +31,15 @@
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
 Athena databases. ### Credentials Credentials can be passed directly to the
 adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
 v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
 conventions. You can either: - configure `aws_access_key_id` and
 `aws_secret_access_key` - configure `aws_profile_name` to match a profile
-defined in your AWS credentials file Checkout DBT profile configuration below
+defined in your AWS credentials file Checkout dbt profile configuration below
 for details. ### Configuring your profile A dbt profile can be configured to
 run against AWS Athena using the following configuration: | Option |
 Description | Required? | Example | |-----------------------|------------------
 --------------------------------------------------------------|-----------|----
 ----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
@@ -79,135 +79,136 @@
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` ### Table location The location
-in which a table is saved is determined by: 1. If `external_location` is
-defined, that value is used. 2. If `s3_data_dir` is defined, the path is
-determined by that and `s3_data_naming` 3. If `s3_data_dir` is not defined data
-is stored under `s3_staging_dir/tables/` Here all the options available for
-`s3_data_naming`: * `uuid`: `{s3_data_dir}/{uuid4()}/` * `table_table`: `
-{s3_data_dir}/{table}/` * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` *
-`schema_table`: `{s3_data_dir}/{schema}/{table}/` *
-`s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4
-()}/` It's possible to set the `s3_data_naming` globally in the target profile,
-or overwrite the value in the table config, or setting up the value for groups
-of model in dbt_project.yml. > Note: when using a work group with a default
-output location configured, `s3_data_naming` and any configured buckets are
-ignored and the location configured in the work group is used. ### Incremental
-models Support for [incremental models](https://docs.getdbt.com/docs/build/
-incremental-models). These strategies are supported: * `insert_overwrite`
-(default): The insert overwrite strategy deletes the overlapping partitions
-from the destination table, and then inserts the new records from the source.
-This strategy depends on the `partitioned_by` keyword! If no partitions are
-defined, dbt will fall back to the `append` strategy. * `append`: Insert new
-records without updating, deleting or overwriting any existing data. There
-might be duplicate data (e.g. great for log or historical data). * `merge`:
-Conditionally updates, deletes, or inserts rows into an Iceberg table. Used in
-combination with `unique_key`. Only available when using Iceberg. ### On schema
-change `on_schema_change` is an option to reflect changes of schema in
-incremental models. The following options are supported: * `ignore` (default) *
-`fail` * `append_new_columns` * `sync_all_columns` In detail, please refer to
-[dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-
-columns-of-my-incremental-model-change). ### Iceberg The adapter supports table
-materialization for Iceberg. To get started just add this as your model: ``` {
-{ config( materialized='table', table_type='iceberg', format='parquet',
-partitioned_by=['bucket(user_id, 5)'], table_properties=
-{ 'optimize_rewrite_delete_file_threshold': '2' } ) }} SELECT 'A' AS user_id,
-'pi' AS name, 'active' AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS
-quantity_big, current_date AS my_date ``` Iceberg supports bucketing as hidden
-partitions, therefore use the `partitioned_by` config to add specific bucketing
-conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
-and `ORC`. It is possible to use iceberg in an incremental fashion,
-specifically 2 strategies are supported: * `append`: new records are appended
-to the table, this can lead to duplicates * `merge`: must be used in
-combination with `unique_key` and it's only available with Engine version 3. It
-performs an upsert, new record are added, and record already existing are
-updated. If `delete_condition` is provided in the model config, it can also
-delete records based on the provided condition (SQL condition). You can use any
-column of the incremental table (`src`) or the final table (`target`). You must
-prefix the column by the name of the table to prevent `Column is ambiguous`
-error. ```sql {{ config( materialized='incremental', table_type='iceberg',
-incremental_strategy='merge', unique_key='user_id',
+{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+### Table location The location in which a table is saved is determined by: 1.
+If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
+defined, the path is determined by that and `s3_data_naming` 3. If
+`s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
+` Here all the options available for `s3_data_naming`: * `uuid`: `
+{s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
+`{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
+{table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
+{table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
+target profile, or overwrite the value in the table config, or setting up the
+value for groups of model in dbt_project.yml. > Note: when using a workgroup
+with a default output location configured, `s3_data_naming` and any configured
+buckets are ignored and the location configured in the workgroup is used. ###
+Incremental models Support for [incremental models](https://docs.getdbt.com/
+docs/build/incremental-models). These strategies are supported: *
+`insert_overwrite` (default): The insert overwrite strategy deletes the
+overlapping partitions from the destination table, and then inserts the new
+records from the source. This strategy depends on the `partitioned_by` keyword!
+If no partitions are defined, dbt will fall back to the `append` strategy. *
+`append`: Insert new records without updating, deleting or overwriting any
+existing data. There might be duplicate data (e.g. great for log or historical
+data). * `merge`: Conditionally updates, deletes, or inserts rows into an
+Iceberg table. Used in combination with `unique_key`. Only available when using
+Iceberg. ### On schema change `on_schema_change` is an option to reflect
+changes of schema in incremental models. The following options are supported: *
+`ignore` (default) * `fail` * `append_new_columns` * `sync_all_columns` For
+details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/
+incremental-models#what-if-the-columns-of-my-incremental-model-change). ###
+Iceberg The adapter supports table materialization for Iceberg. To get started
+just add this as your model: ```sql {{ config( materialized='table',
+table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
+table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
+'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
+100000000 as quantity_big, current_date as my_date ``` Iceberg supports
+bucketing as hidden partitions, therefore use the `partitioned_by` config to
+add specific bucketing conditions. Iceberg supports several table formats for
+data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
+incremental fashion, specifically two strategies are supported: * `append`: new
+records are appended to the table, this can lead to duplicates * `merge`: must
+be used in combination with `unique_key` and it's only available with Engine
+version 3. It performs an upsert, new record are added, and record already
+existing are updated. If `delete_condition` is provided in the model config, it
+can also delete records based on the provided condition (SQL condition). You
+can use any column of the incremental table (`src`) or the final table
+(`target`). You must prefix the column by the name of the table to prevent
+`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
+table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
-'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
-AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
-current_date AS my_date ``` ### High available table materialization The
+'2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
+as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
+current_date as my_date ``` ### High availability table materialization The
 current implementation of the table materialization can lead to downtime, as
 target table is dropped and re-created. To have the less destructive behavior
 it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverage the table versions feature of glue catalog, creating a tmp table and
-swapping the target table to the location of the tmp table. This
-materialization is only available for `table_type=hive` and requires using
-unique locations. ``` {{ config( materialized='table_hive_ha',
+leverages the table versions feature of Glue catalog, creating a temp table and
+swapping the target table to the location of the temp table. This
+materialization is only available for `table_type='hive'` and requires using
+unique locations. ```sql {{ config( materialized='table_hive_ha',
 format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
 select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it that setting
+materialization keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
-instead of partitions * By default, Glue "duplicate" the versions internally,
-so the last 2 versions of a table point to the same location * It's recommended
-to have versions_to_keep>= 4, as this will avoid to have the older location
-removed * The macro athena__end_of_time needs to be overwritten by the user if
-using Athena v3 since it requires a precision parameter for timestamps ##
-Snapshots The adapter supports snapshot materialization. It supports both
-timestamp and check strategy. To create a snapshot create a snapshot file in
-the snapshots directory. If directory does not exist create one. ### Timestamp
-strategy To use the timestamp strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
-strategy To use the check strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
-materialization also supports invalidating hard deletes. Check the [docs]
-(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+instead of partitions * By default, Glue "duplicates" the versions internally,
+so the last two versions of a table point to the same location * It's
+recommended to have `versions_to_keep` >= 4, as this will avoid having the
+older location removed * The macro `athena__end_of_time` needs to be
+overwritten by the user if using Athena engine v3 since it requires a precision
+parameter for timestamps ## Snapshots The adapter supports snapshot
+materialization. It supports both timestamp and check strategy. To create a
+snapshot create a snapshot file in the snapshots directory. If the directory
+does not exist create one. ### Timestamp strategy To use the timestamp strategy
+refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
+strategy-recommended) ### Check strategy To use the check strategy refer to the
+[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
+Hard-deletes The materialization also supports invalidating hard deletes. Check
+the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
-model.sql ``` {{ config( materialized='table' ) }} SELECT ROW_NUMBER() OVER ()
-AS id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS
-refresh_timestamp FROM {{ ref('employment_indicators_november_2022_csv_tables')
-}} ``` timestamp strategy - model_snapshot_1 ``` {% snapshot model_snapshot_1
-%} {{ config( strategy='timestamp', updated_at='refresh_timestamp',
-unique_key='id' ) }} SELECT * from {{ ref('model') }} {% endsnapshot %} ```
-invalidate hard deletes - model_snapshot_2 ``` {% snapshot model_snapshot_2 %}
-{{ config ( unique_key='id', strategy='timestamp',
-updated_at='refresh_timestamp', invalidate_hard_deletes=True, ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` check strategy - model_snapshot_3
-``` {% snapshot model_snapshot_3 %} {{ config ( unique_key='id',
-strategy='check', check_cols=['series_reference','data_value'] ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` ### Known issues * Incremental
-Iceberg models - Sync all columns on schema change can't remove columns used as
-partitioning. The only way, from a dbt perspective, is to do a full-refresh of
-the incremental model. * Tables, schemas and database should only be lowercase
-* In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
-(https://github.com/Tomme/dbt-athena) is not installed in the target
-environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
-details. * Snapshot does not support dropping columns from the source table. If
-you drop a column make sure to drop the column from the snapshot as well.
-Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)):
-        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
-         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
-      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
-                               ð ð§                                                           Lee
-                                                                                                           ð
-      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
-       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
-             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+model.sql ```sql {{ config( materialized='table' ) }} select row_number() over
+() as id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as
+refresh_timestamp from {{ ref('employment_indicators_november_2022_csv_tables')
+}} ``` timestamp strategy - model_snapshot_1 ```sql {% snapshot
+model_snapshot_1 %} {{ config( strategy='timestamp',
+updated_at='refresh_timestamp', unique_key='id' ) }} select * from {{ ref
+('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
+```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
+strategy='timestamp', updated_at='refresh_timestamp',
+invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
+model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
+['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` ### Known issues * Incremental Iceberg models - Sync all
+columns on schema change can't remove columns used as partitioning. The only
+way, from a dbt perspective, is to do a full-refresh of the incremental model.
+* Tables, schemas and database should only be lowercase * In order to avoid
+potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
+dbt-athena) is not installed in the target environment. See https://github.com/
+dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
+dropping columns from the source table. If you drop a column make sure to drop
+the column from the snapshot as well. Another workaround is to NULL the column
+in the snapshot definition to preserve history ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
+                               ð ð§                                                                    Lee
+                                                                                                                    ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko      ð» ð
                                              Reinaldo                             ð» ð
                                                ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/__init__.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/column.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/connections.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/impl.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -727,7 +727,28 @@
         partition_keys = table.get("PartitionKeys", [])
 
         logger.debug(f"Columns in relation {relation.identifier}: {columns + partition_keys}")
 
         return [
             AthenaColumn(column=c["Name"], dtype=c["Type"], table_type=table_type) for c in columns + partition_keys
         ]
+
+    @available
+    def delete_from_glue_catalog(self, relation: AthenaRelation):
+        schema_name = relation.schema
+        table_name = relation.identifier
+
+        conn = self.connections.get_thread_connection()
+        client = conn.handle
+
+        with boto3_client_lock:
+            glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
+
+        try:
+            glue_client.delete_table(DatabaseName=schema_name, Name=table_name)
+            logger.debug(f"Deleted table from glue catalog: {relation.render()}")
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "EntityNotFoundException":
+                logger.debug(f"Table {relation.render()} does not exist and will not be deleted, ignoring")
+            else:
+                logger.error(e)
+                raise e
```

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/query_headers.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/adapters/athena/relation.py` & `dbt-athena-community-1.4.5/dbt/adapters/athena/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/relation.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 {% macro athena__drop_relation(relation) -%}
-  {% set rel_type = adapter.get_table_type(relation.schema, relation.table) %}
-  {%- if rel_type is not none %}
-    {%- if rel_type == 'table' %}
-      {%- do adapter.clean_up_table(relation.schema, relation.table) -%}
+  {% set rel_type_object = adapter.get_table_type(relation.schema, relation.identifier) %}
+  {%- if rel_type_object is not none %}
+    {% set rel_type = rel_type_object.value %}
+    {%- if rel_type == 'table' or rel_type == 'iceberg_table' %}
+      {%- do adapter.clean_up_table(relation.schema, relation.identifier) -%}
     {%- endif %}
-    {% call statement('drop_relation', auto_begin=False) -%}
-      {%- if relation.type == 'view' -%}
-        drop {{ relation.type }} if exists {{ relation.render() }}
-      {%- else -%}
-        drop {{ relation.type }} if exists {{ relation.render_hive() }}
-      {% endif %}
-    {%- endcall %}
+    {%- do adapter.delete_from_glue_catalog(relation) -%}
   {%- endif %}
 {% endmacro %}
 
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
     alter table {{ relation.render_hive() }} set tblproperties ('classification' = '{{ format }}')
```

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       bucketed_by or bucket_count cannot be used with Iceberg tables. You have to use the bucket function
       when partitioning. Will be ignored
       {%- endset -%}
       {%- set bucketed_by = none -%}
       {%- set bucket_count = none -%}
       {% do log(ignored_bucket_iceberg) %}
     {%- endif -%}
-    {%- if s3_data_naming in ['table', 'table_schema'] or external_location is not none -%}
+    {%- if s3_data_naming in ['table', 'schema_table'] or external_location is not none -%}
       {%- set error_unique_location_iceberg -%}
         You need to have an unique table location when creating Iceberg table. Right now we are building tables in
         a destructive way but in the near future we will be using the RENAME feature to provide near-zero downtime.
       {%- endset -%}
       {% do exceptions.raise_compiler_error(error_unique_location_iceberg) %}
     {%- endif -%}
   {%- endif %}
```

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   {%- set full_refresh_config = config.get('full_refresh', default=False) -%}
   {%- set full_refresh_mode = (flags.FULL_REFRESH == True or full_refresh_config == True) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type='table') -%}
 
-  {%- if s3_data_naming in ['table', 'table_schema'] or external_location is not none -%}
+  {%- if s3_data_naming in ['table', 'schema_table'] or external_location is not none -%}
     {%- set error_unique_location_hive_ha -%}
         You need to have an unique table location when using table_hive_ha materialization.
         Use s3_data_naming table_unique or schema_table_unique, and avoid to set an explicit external_location.
     {%- endset -%}
     {% do exceptions.raise_compiler_error(error_unique_location_hive_ha) %}
   {%- endif -%}
 
@@ -34,33 +34,29 @@
     {% call statement('main') -%}
       {{ create_table_as(False, target_relation, sql) }}
     {%- endcall %}
   {%- else -%}
     {% set tmp_relation = make_temp_relation(target_relation, '__ha') %}
 
     -- drop the tmp_relation
-    {% call statement('drop_tmp_relation', auto_begin=False) -%}
-      drop table if exists {{ tmp_relation.render_hive() }}
-    {%- endcall %}
+    {{ adapter.delete_from_glue_catalog(tmp_relation) }}
 
     -- create tmp table
     {% call statement('main') -%}
       {{ create_table_as(False, tmp_relation, sql) }}
     {%- endcall %}
 
     -- save the original target table location before swapping
     {% set original_table_location = adapter.get_table_location(target_relation.schema, target_relation.table) %}
 
     -- swap table
     {% set swap_table = adapter.swap_table(tmp_relation.schema, tmp_relation.name, target_relation.schema, target_relation.table) %}
 
     -- delete glue tmp table, do not use drop_relation, as it will remove data of the target table
-    {% call statement('drop_tmp_relation', auto_begin=False) -%}
-      drop table if exists {{ tmp_relation.render_hive() }}
-    {%- endcall %}
+    {{ adapter.delete_from_glue_catalog(tmp_relation) }}
 
     {% set result_table_version_expiration = adapter.expire_glue_table_versions(target_relation.schema, target_relation.table, versions_to_keep, True) %}
 
   {% endif %}
 
   {{ set_table_classification(target_relation) }}
```

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datediff.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/ddl_data_type.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/ddl_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/timestamps.sql` & `dbt-athena-community-1.4.5/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt/include/athena/profile_template.yml` & `dbt-athena-community-1.4.5/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/dbt_athena_community.egg-info/PKG-INFO` & `dbt-athena-community-1.4.5/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.4.4
+Version: 1.4.5
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
+License: Apache License 2.0
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
 
 ## Features
 
 * Supports dbt version `1.4.*`
-* Supports [Seeds][seeds]
+* Supports [seeds][seeds]
 * Correctly detects views and their columns
 * Supports [table materialization][table]
-  * [Iceberg tables][athena-iceberg] is supported **only with Athena Engine v3** and **a unique table location**
+  * [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
   (see table location section below)
-  * Hive tables is supported by both Athena engines.
+  * Hive tables are supported by both Athena engines.
 * Supports [incremental models][incremental]
-  * On iceberg tables :
-    * Support the use of `unique_key` only with the `merge` strategy
-    * Support the `append` strategy
+  * On Iceberg tables :
+    * Supports the use of `unique_key` only with the `merge` strategy
+    * Supports the `append` strategy
   * On Hive tables :
-    * Support two incremental update strategies: `insert_overwrite` and `append`
+    * Supports two incremental update strategies: `insert_overwrite` and `append`
     * Does **not** support the use of `unique_key`
 * Supports [snapshots][snapshots]
 * Does not support [Python models][python-models]
 * Does not support [persist docs][persist-docs] for views
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 [incremental]: https://docs.getdbt.com/docs/build/incremental-models
@@ -67,15 +79,15 @@
 
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
 You can either:
 - configure `aws_access_key_id` and `aws_secret_access_key`
 - configure `aws_profile_name` to match a profile defined in your AWS credentials file
-Checkout DBT profile configuration below for details.
+Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                    | Required? | Example                                    |
 |-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
@@ -145,33 +157,35 @@
 * `lf_tags` (`default=none`)
   * lf tags to associate with the table
   * format: `{"tag1": "value1", "tag2": "value2"}`
 * `lf_tags_columns` (`default=none`)
   * lf tags to associate with the table columns
   * format: `{"tag1": {"value1": ["column1": "column2"]}}`
 
+[create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+
 ### Table location
 
 The location in which a table is saved is determined by:
 
 1. If `external_location` is defined, that value is used.
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
-3. If `s3_data_dir` is not defined data is stored under `s3_staging_dir/tables/`
+3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 * `uuid`: `{s3_data_dir}/{uuid4()}/`
-* `table_table`: `{s3_data_dir}/{table}/`
+* `table`: `{s3_data_dir}/{table}/`
 * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/`
 * `schema_table`: `{s3_data_dir}/{schema}/{table}/`
 * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4()}/`
 
 It's possible to set the `s3_data_naming` globally in the target profile, or overwrite the value in the table config,
 or setting up the value for groups of model in dbt_project.yml.
 
-> Note: when using a work group with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the work group is used.
+> Note: when using a workgroup with a default output location configured, `s3_data_naming` and any configured buckets are ignored and the location configured in the workgroup is used.
 
 ### Incremental models
 
 Support for [incremental models](https://docs.getdbt.com/docs/build/incremental-models).
 
 These strategies are supported:
 
@@ -188,83 +202,83 @@
 `on_schema_change` is an option to reflect changes of schema in incremental models.
 The following options are supported:
 * `ignore` (default)
 * `fail`
 * `append_new_columns`
 * `sync_all_columns`
 
-In detail, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
+For details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change).
 
 ### Iceberg
 
 The adapter supports table materialization for Iceberg.
 
 To get started just add this as your model:
-```
+```sql
 {{ config(
     materialized='table',
     table_type='iceberg',
     format='parquet',
     partitioned_by=['bucket(user_id, 5)'],
     table_properties={
     	'optimize_rewrite_delete_file_threshold': '2'
     	}
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
-It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
+It is possible to use Iceberg in an incremental fashion, specifically two strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
    It performs an upsert, new record are added, and record already existing are updated. If
    `delete_condition` is provided in the model config, it can also delete records based on the
    provided condition (SQL condition). You can use any column of the incremental table (`src`) or
    the final table (`target`). You must prefix the column by the name of the table to prevent
    `Column is ambiguous` error.
 
 ```sql
 {{ config(
     materialized='incremental',
     table_type='iceberg',
     incremental_strategy='merge',
     unique_key='user_id',
-    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
-    format='parquet',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year",
+    format='parquet'
 ) }}
 
-SELECT
-	'A' AS user_id,
-	'pi' AS name,
-	'active' AS status,
-	17.89 AS cost,
-	1 AS quantity,
-	100000000 AS quantity_big,
-	current_date AS my_date
+select
+	'A' as user_id,
+	'pi' as name,
+	'active' as status,
+	17.89 as cost,
+	1 as quantity,
+	100000000 as quantity_big,
+	current_date as my_date
 ```
 
-### High available table materialization
+### High availability table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
-**table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
-the target table to the location of the tmp table.
-This materialization is only available for `table_type=hive` and requires using unique locations.
+**table_hive_ha** leverages the table versions feature of Glue catalog, creating a temp table and swapping
+the target table to the location of the temp table.
+This materialization is only available for `table_type='hive'` and requires using unique locations.
 
-```
+```sql
 {{ config(
     materialized='table_hive_ha',
     format='parquet',
     partition_by=['status'],
     s3_data_naming='table_unique'
 ) }}
 
@@ -275,27 +289,27 @@
 union all
 select
   'b' as user_id,
   'sh' as user_name,
   'disabled' as status
 ```
 
-By default, the materialization keeps the last 4 table versions, you can change it that setting `versions_to_keep`.
+By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
 #### Known issues
 * When swapping from a table with partitions to a table without (and the other way around), there could be a little downtime.
   In case high performances are needed consider bucketing instead of partitions
-* By default, Glue "duplicate" the versions internally, so the last 2 versions of a table point to the same location
-* It's recommended to have versions_to_keep>= 4, as this will avoid to have the older location removed
-* The macro athena__end_of_time needs to be overwritten by the user if using Athena v3 since it requires a precision parameter for timestamps
+* By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
+* It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+* The macro `athena__end_of_time` needs to be overwritten by the user if using Athena engine v3 since it requires a precision parameter for timestamps
 
 
 ## Snapshots
 
-The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If directory does not exist create one.
+The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
 To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended)
 
 ### Check strategy
 
@@ -328,77 +342,78 @@
 MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468,
 MEIM.S1WA,2000.09,72462,
 MEIM.S1WA,2000.1,74897,
 ```
 
 model.sql
-```
+```sql
 {{ config(
     materialized='table'
 ) }}
 
-SELECT
-    ROW_NUMBER() OVER () AS id
+select
+    row_number() over() as id
     , *
-    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS refresh_timestamp
-FROM {{ ref('employment_indicators_november_2022_csv_tables') }}
+    , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
 ```
 
 timestamp strategy - model_snapshot_1
 
-```
+```sql
 {% snapshot model_snapshot_1 %}
 
 {{
     config(
       strategy='timestamp',
       updated_at='refresh_timestamp',
       unique_key='id'
     )
 }}
 
-SELECT *
-
+select *
 from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 invalidate hard deletes - model_snapshot_2
-```
+```sql
 {% snapshot model_snapshot_2 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='timestamp',
         updated_at='refresh_timestamp',
         invalidate_hard_deletes=True,
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 check strategy - model_snapshot_3
-```
+```sql
 {% snapshot model_snapshot_3 %}
 
 {{
     config
     (
         unique_key='id',
         strategy='check',
         check_cols=['series_reference','data_value']
     )
 }}
-SELECT * from {{ ref('model') }}
+select *
+from {{ ref('model') }}
 
 {% endsnapshot %}
 ```
 
 ### Known issues
 
 * Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
@@ -437,14 +452,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrischin478"><img src="https://avatars.githubusercontent.com/u/47199426?v=4?s=100" width="100px;" alt="chrischin478"/><br /><sub><b>chrischin478</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=chrischin478" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Achrischin478" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,26 +1,33 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.4 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.5 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena Description-Content-Type: text/markdown License-File:
-LICENSE.txt
+dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
-## Features * Supports dbt version `1.4.*` * Supports [Seeds][seeds] *
+## Features * Supports dbt version `1.4.*` * Supports [seeds][seeds] *
 Correctly detects views and their columns * Supports [table materialization]
-[table] * [Iceberg tables][athena-iceberg] is supported **only with Athena
+[table] * [Iceberg tables][athena-iceberg] are supported **only with Athena
 Engine v3** and **a unique table location** (see table location section below)
-* Hive tables is supported by both Athena engines. * Supports [incremental
-models][incremental] * On iceberg tables : * Support the use of `unique_key`
-only with the `merge` strategy * Support the `append` strategy * On Hive tables
-: * Support two incremental update strategies: `insert_overwrite` and `append`
-* Does **not** support the use of `unique_key` * Supports [snapshots]
+* Hive tables are supported by both Athena engines. * Supports [incremental
+models][incremental] * On Iceberg tables : * Supports the use of `unique_key`
+only with the `merge` strategy * Supports the `append` strategy * On Hive
+tables : * Supports two incremental update strategies: `insert_overwrite` and
+`append` * Does **not** support the use of `unique_key` * Supports [snapshots]
 [snapshots] * Does not support [Python models][python-models] * Does not
 support [persist docs][persist-docs] for views [seeds]: https://
 docs.getdbt.com/docs/building-a-dbt-project/seeds [incremental]: https://
 docs.getdbt.com/docs/build/incremental-models [table]: https://docs.getdbt.com/
 docs/build/materializations#table [python-models]: https://docs.getdbt.com/
 docs/build/python-models#configuring-python-models [athena-iceberg]: https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html [snapshots]: https:/
@@ -35,15 +42,15 @@
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
 Athena databases. ### Credentials Credentials can be passed directly to the
 adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
 v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
 conventions. You can either: - configure `aws_access_key_id` and
 `aws_secret_access_key` - configure `aws_profile_name` to match a profile
-defined in your AWS credentials file Checkout DBT profile configuration below
+defined in your AWS credentials file Checkout dbt profile configuration below
 for details. ### Configuring your profile A dbt profile can be configured to
 run against AWS Athena using the following configuration: | Option |
 Description | Required? | Example | |-----------------------|------------------
 --------------------------------------------------------------|-----------|----
 ----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
@@ -83,135 +90,136 @@
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
 (`default=none`) * lf tags to associate with the table columns * format: `
-{"tag1": {"value1": ["column1": "column2"]}}` ### Table location The location
-in which a table is saved is determined by: 1. If `external_location` is
-defined, that value is used. 2. If `s3_data_dir` is defined, the path is
-determined by that and `s3_data_naming` 3. If `s3_data_dir` is not defined data
-is stored under `s3_staging_dir/tables/` Here all the options available for
-`s3_data_naming`: * `uuid`: `{s3_data_dir}/{uuid4()}/` * `table_table`: `
-{s3_data_dir}/{table}/` * `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` *
-`schema_table`: `{s3_data_dir}/{schema}/{table}/` *
-`s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/{table}/{uuid4
-()}/` It's possible to set the `s3_data_naming` globally in the target profile,
-or overwrite the value in the table config, or setting up the value for groups
-of model in dbt_project.yml. > Note: when using a work group with a default
-output location configured, `s3_data_naming` and any configured buckets are
-ignored and the location configured in the work group is used. ### Incremental
-models Support for [incremental models](https://docs.getdbt.com/docs/build/
-incremental-models). These strategies are supported: * `insert_overwrite`
-(default): The insert overwrite strategy deletes the overlapping partitions
-from the destination table, and then inserts the new records from the source.
-This strategy depends on the `partitioned_by` keyword! If no partitions are
-defined, dbt will fall back to the `append` strategy. * `append`: Insert new
-records without updating, deleting or overwriting any existing data. There
-might be duplicate data (e.g. great for log or historical data). * `merge`:
-Conditionally updates, deletes, or inserts rows into an Iceberg table. Used in
-combination with `unique_key`. Only available when using Iceberg. ### On schema
-change `on_schema_change` is an option to reflect changes of schema in
-incremental models. The following options are supported: * `ignore` (default) *
-`fail` * `append_new_columns` * `sync_all_columns` In detail, please refer to
-[dbt docs](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-
-columns-of-my-incremental-model-change). ### Iceberg The adapter supports table
-materialization for Iceberg. To get started just add this as your model: ``` {
-{ config( materialized='table', table_type='iceberg', format='parquet',
-partitioned_by=['bucket(user_id, 5)'], table_properties=
-{ 'optimize_rewrite_delete_file_threshold': '2' } ) }} SELECT 'A' AS user_id,
-'pi' AS name, 'active' AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS
-quantity_big, current_date AS my_date ``` Iceberg supports bucketing as hidden
-partitions, therefore use the `partitioned_by` config to add specific bucketing
-conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
-and `ORC`. It is possible to use iceberg in an incremental fashion,
-specifically 2 strategies are supported: * `append`: new records are appended
-to the table, this can lead to duplicates * `merge`: must be used in
-combination with `unique_key` and it's only available with Engine version 3. It
-performs an upsert, new record are added, and record already existing are
-updated. If `delete_condition` is provided in the model config, it can also
-delete records based on the provided condition (SQL condition). You can use any
-column of the incremental table (`src`) or the final table (`target`). You must
-prefix the column by the name of the table to prevent `Column is ambiguous`
-error. ```sql {{ config( materialized='incremental', table_type='iceberg',
-incremental_strategy='merge', unique_key='user_id',
+{"tag1": {"value1": ["column1": "column2"]}}` [create-table-as]: https://
+docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
+### Table location The location in which a table is saved is determined by: 1.
+If `external_location` is defined, that value is used. 2. If `s3_data_dir` is
+defined, the path is determined by that and `s3_data_naming` 3. If
+`s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/
+` Here all the options available for `s3_data_naming`: * `uuid`: `
+{s3_data_dir}/{uuid4()}/` * `table`: `{s3_data_dir}/{table}/` * `table_unique`:
+`{s3_data_dir}/{table}/{uuid4()}/` * `schema_table`: `{s3_data_dir}/{schema}/
+{table}/` * `s3_data_naming=schema_table_unique`: `{s3_data_dir}/{schema}/
+{table}/{uuid4()}/` It's possible to set the `s3_data_naming` globally in the
+target profile, or overwrite the value in the table config, or setting up the
+value for groups of model in dbt_project.yml. > Note: when using a workgroup
+with a default output location configured, `s3_data_naming` and any configured
+buckets are ignored and the location configured in the workgroup is used. ###
+Incremental models Support for [incremental models](https://docs.getdbt.com/
+docs/build/incremental-models). These strategies are supported: *
+`insert_overwrite` (default): The insert overwrite strategy deletes the
+overlapping partitions from the destination table, and then inserts the new
+records from the source. This strategy depends on the `partitioned_by` keyword!
+If no partitions are defined, dbt will fall back to the `append` strategy. *
+`append`: Insert new records without updating, deleting or overwriting any
+existing data. There might be duplicate data (e.g. great for log or historical
+data). * `merge`: Conditionally updates, deletes, or inserts rows into an
+Iceberg table. Used in combination with `unique_key`. Only available when using
+Iceberg. ### On schema change `on_schema_change` is an option to reflect
+changes of schema in incremental models. The following options are supported: *
+`ignore` (default) * `fail` * `append_new_columns` * `sync_all_columns` For
+details, please refer to [dbt docs](https://docs.getdbt.com/docs/build/
+incremental-models#what-if-the-columns-of-my-incremental-model-change). ###
+Iceberg The adapter supports table materialization for Iceberg. To get started
+just add this as your model: ```sql {{ config( materialized='table',
+table_type='iceberg', format='parquet', partitioned_by=['bucket(user_id, 5)'],
+table_properties={ 'optimize_rewrite_delete_file_threshold': '2' } ) }} select
+'A' as user_id, 'pi' as name, 'active' as status, 17.89 as cost, 1 as quantity,
+100000000 as quantity_big, current_date as my_date ``` Iceberg supports
+bucketing as hidden partitions, therefore use the `partitioned_by` config to
+add specific bucketing conditions. Iceberg supports several table formats for
+data : `PARQUET`, `AVRO` and `ORC`. It is possible to use Iceberg in an
+incremental fashion, specifically two strategies are supported: * `append`: new
+records are appended to the table, this can lead to duplicates * `merge`: must
+be used in combination with `unique_key` and it's only available with Engine
+version 3. It performs an upsert, new record are added, and record already
+existing are updated. If `delete_condition` is provided in the model config, it
+can also delete records based on the provided condition (SQL condition). You
+can use any column of the incremental table (`src`) or the final table
+(`target`). You must prefix the column by the name of the table to prevent
+`Column is ambiguous` error. ```sql {{ config( materialized='incremental',
+table_type='iceberg', incremental_strategy='merge', unique_key='user_id',
 delete_condition="src.status != 'active' and target.my_date < now() - interval
-'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
-AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
-current_date AS my_date ``` ### High available table materialization The
+'2' year", format='parquet' ) }} select 'A' as user_id, 'pi' as name, 'active'
+as status, 17.89 as cost, 1 as quantity, 100000000 as quantity_big,
+current_date as my_date ``` ### High availability table materialization The
 current implementation of the table materialization can lead to downtime, as
 target table is dropped and re-created. To have the less destructive behavior
 it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
-leverage the table versions feature of glue catalog, creating a tmp table and
-swapping the target table to the location of the tmp table. This
-materialization is only available for `table_type=hive` and requires using
-unique locations. ``` {{ config( materialized='table_hive_ha',
+leverages the table versions feature of Glue catalog, creating a temp table and
+swapping the target table to the location of the temp table. This
+materialization is only available for `table_type='hive'` and requires using
+unique locations. ```sql {{ config( materialized='table_hive_ha',
 format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
 select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
-materialization keeps the last 4 table versions, you can change it that setting
+materialization keeps the last 4 table versions, you can change it by setting
 `versions_to_keep`. #### Known issues * When swapping from a table with
 partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
-instead of partitions * By default, Glue "duplicate" the versions internally,
-so the last 2 versions of a table point to the same location * It's recommended
-to have versions_to_keep>= 4, as this will avoid to have the older location
-removed * The macro athena__end_of_time needs to be overwritten by the user if
-using Athena v3 since it requires a precision parameter for timestamps ##
-Snapshots The adapter supports snapshot materialization. It supports both
-timestamp and check strategy. To create a snapshot create a snapshot file in
-the snapshots directory. If directory does not exist create one. ### Timestamp
-strategy To use the timestamp strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
-strategy To use the check strategy refer to the [dbt docs](https://
-docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
-materialization also supports invalidating hard deletes. Check the [docs]
-(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+instead of partitions * By default, Glue "duplicates" the versions internally,
+so the last two versions of a table point to the same location * It's
+recommended to have `versions_to_keep` >= 4, as this will avoid having the
+older location removed * The macro `athena__end_of_time` needs to be
+overwritten by the user if using Athena engine v3 since it requires a precision
+parameter for timestamps ## Snapshots The adapter supports snapshot
+materialization. It supports both timestamp and check strategy. To create a
+snapshot create a snapshot file in the snapshots directory. If the directory
+does not exist create one. ### Timestamp strategy To use the timestamp strategy
+refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
+strategy-recommended) ### Check strategy To use the check strategy refer to the
+[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
+Hard-deletes The materialization also supports invalidating hard deletes. Check
+the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
-model.sql ``` {{ config( materialized='table' ) }} SELECT ROW_NUMBER() OVER ()
-AS id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) AS
-refresh_timestamp FROM {{ ref('employment_indicators_november_2022_csv_tables')
-}} ``` timestamp strategy - model_snapshot_1 ``` {% snapshot model_snapshot_1
-%} {{ config( strategy='timestamp', updated_at='refresh_timestamp',
-unique_key='id' ) }} SELECT * from {{ ref('model') }} {% endsnapshot %} ```
-invalidate hard deletes - model_snapshot_2 ``` {% snapshot model_snapshot_2 %}
-{{ config ( unique_key='id', strategy='timestamp',
-updated_at='refresh_timestamp', invalidate_hard_deletes=True, ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` check strategy - model_snapshot_3
-``` {% snapshot model_snapshot_3 %} {{ config ( unique_key='id',
-strategy='check', check_cols=['series_reference','data_value'] ) }} SELECT *
-from {{ ref('model') }} {% endsnapshot %} ``` ### Known issues * Incremental
-Iceberg models - Sync all columns on schema change can't remove columns used as
-partitioning. The only way, from a dbt perspective, is to do a full-refresh of
-the incremental model. * Tables, schemas and database should only be lowercase
-* In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
-(https://github.com/Tomme/dbt-athena) is not installed in the target
-environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
-details. * Snapshot does not support dropping columns from the source table. If
-you drop a column make sure to drop the column from the snapshot as well.
-Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)):
-        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
-         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
-      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
-                               ð ð§                                                           Lee
-                                                                                                           ð
-      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
-       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
-             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+model.sql ```sql {{ config( materialized='table' ) }} select row_number() over
+() as id , * , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as
+refresh_timestamp from {{ ref('employment_indicators_november_2022_csv_tables')
+}} ``` timestamp strategy - model_snapshot_1 ```sql {% snapshot
+model_snapshot_1 %} {{ config( strategy='timestamp',
+updated_at='refresh_timestamp', unique_key='id' ) }} select * from {{ ref
+('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
+```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
+strategy='timestamp', updated_at='refresh_timestamp',
+invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
+model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
+['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
+endsnapshot %} ``` ### Known issues * Incremental Iceberg models - Sync all
+columns on schema change can't remove columns used as partitioning. The only
+way, from a dbt perspective, is to do a full-refresh of the incremental model.
+* Tables, schemas and database should only be lowercase * In order to avoid
+potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/
+dbt-athena) is not installed in the target environment. See https://github.com/
+dbt-athena/dbt-athena/issues/103 for more details. * Snapshot does not support
+dropping columns from the source table. If you drop a column make sure to drop
+the column from the snapshot as well. Another workaround is to NULL the column
+in the snapshot definition to preserve history ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]            [Mattia]     [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom              Mattia        Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð      ð§    Gatsby
+                               ð ð§                                                                    Lee
+                                                                                                                    ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii       [chrischin478]
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]       chrischin478
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko      ð» ð
                                              Reinaldo                             ð» ð
                                                ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.4/dbt_athena_community.egg-info/SOURCES.txt` & `dbt-athena-community-1.4.5/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/pyproject.toml` & `dbt-athena-community-1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.4/setup.py` & `dbt-athena-community-1.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,19 +40,34 @@
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
+    platforms="any",
+    license="Apache License 2.0",
+    license_files=("LICENSE.txt",),
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         # In order to control dbt-core version and package version
         "boto3~=1.26",
         "boto3-stubs[athena,glue,lakeformation,sts]~=1.26",
         "dbt-core~=1.4.6",
         "pyathena~=2.25",
         "tenacity~=8.2",
     ],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

