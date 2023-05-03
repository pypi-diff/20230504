# Comparing `tmp/sqlfluff-2.0.6.tar.gz` & `tmp/sqlfluff-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-qhi7531s/sqlfluff-2.0.6.tar", last modified: Thu Apr 20 09:29:28 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-npizmwgn/sqlfluff-2.0.7.tar", last modified: Thu Apr 20 21:05:59 2023, max compression
```

## Comparing `sqlfluff-2.0.6.tar` & `sqlfluff-2.0.7.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)   380758 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129858 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68071 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80702 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   165688 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69018 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   200280 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   102212 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172023 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    91962 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:29:28.000000 sqlfluff-2.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-20 09:29:01.000000 sqlfluff-2.0.6/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)   381650 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129858 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68071 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17642 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80702 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165688 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69018 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200280 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102212 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172023 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:05:59.000000 sqlfluff-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-20 21:05:42.000000 sqlfluff-2.0.7/test/test_testing.py
```

### Comparing `sqlfluff-2.0.6/CHANGELOG.md` & `sqlfluff-2.0.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,32 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.0.7] - 2023-04-20
+
+## Highlights
+
+This is a bugfix release to resolve two regressions included in 2.0.6
+related to implicit indents. This also includes a bugfix for config
+file on osx, contributed by first time contributor [@jpuris](https://github.com/jpuris) 🎉.
+
+## What’s Changed
+
+* Fix regression in implicit indents [#4798](https://github.com/sqlfluff/sqlfluff/pull/4798) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix bug with brackets and implicit indents [#4797](https://github.com/sqlfluff/sqlfluff/pull/4797) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* fix: correct macos/osx config file location [#4795](https://github.com/sqlfluff/sqlfluff/pull/4795) [@jpuris](https://github.com/jpuris)
+
+## New Contributors
+
+* [@jpuris](https://github.com/jpuris) made their first contribution in [#4795](https://github.com/sqlfluff/sqlfluff/pull/4795)
+
 ## [2.0.6] - 2023-04-19
 
 ## Highlights
 
 * Introduction of a `--quiet` option for the CLI for situations
   where less output is useful.
 * When using the `--force` option is used for `sqlfluff fix` each
```

### Comparing `sqlfluff-2.0.6/LICENSE.md` & `sqlfluff-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/PKG-INFO` & `sqlfluff-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.6
+Version: 2.0.7
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.6/README.md` & `sqlfluff-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/setup.cfg` & `sqlfluff-2.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.0.6
+version = 2.0.7
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.0.6
+stable_version = 2.0.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.0.6/src/sqlfluff/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/api/simple.py` & `sqlfluff-2.0.7/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/commands.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/commands.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.0.7/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/config.py` & `sqlfluff-2.0.7/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.0.7/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.0.7/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.0.7/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/enums.py` & `sqlfluff-2.0.7/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/errors.py` & `sqlfluff-2.0.7/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.0.7/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.0.7/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.0.7/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.0.7/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.0.7/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.0.7/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.0.7/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/core/timing.py` & `sqlfluff-2.0.7/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.0.7/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.0.7/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.0.7/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/reindent.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,32 +673,56 @@
     cached_point: Optional[_IndentPoint] = None
     for idx, elem in enumerate(elements):
         if isinstance(elem, ReflowPoint):
             # NOTE: The following line should never lead to an index error
             # because files should always have a trailing IndentBlock containing
             # an "end_of_file" marker, and so the final IndentPoint should always
             # have _something_ after it.
-            following_class_types = elements[idx + 1].class_types
             indent_stats = IndentStats.from_combination(
                 cached_indent_stats,
                 elem.get_indent_impulse(),
             )
-
             # If don't allow implicit indents we should remove them here.
             # Also, if we do - we should check for brackets.
-            # NOTE: The reason we check `following_class_types` is because
+            # NOTE: The reason we check following class_types is because
             # bracketed expressions behave a little differently and are an
             # exception to the normal implicit indent rules. For implicit
             # indents which precede bracketed expressions, the implicit indent
-            # is treated as a normal indent.
-            if not allow_implicit_indents or "start_bracket" in following_class_types:
-                # Blank indent stats if not using them
-                indent_stats = IndentStats(
-                    indent_stats.impulse, indent_stats.trough, ()
-                )
+            # is treated as a normal indent. In this case the start_bracket
+            # must be the start of the bracketed section which isn't closed
+            # on the same line - if it _is_ closed then we keep the implicit
+            # indents.
+            if indent_stats.implicit_indents:
+                unclosed_bracket = False
+                if (
+                    allow_implicit_indents
+                    and "start_bracket" in elements[idx + 1].class_types
+                ):
+                    # Is it closed in the line? Iterate forward to find out.
+                    # get the stack depth
+                    next_elem = cast(ReflowBlock, elements[idx + 1])
+                    depth = next_elem.depth_info.stack_depth
+                    for elem_j in elements[idx + 1 :]:
+                        if isinstance(elem_j, ReflowPoint):
+                            if elem_j.num_newlines() > 0:
+                                unclosed_bracket = True
+                                break
+                        elif (
+                            "end_bracket" in elem_j.class_types
+                            and elem_j.depth_info.stack_depth == depth
+                        ):
+                            break
+                    else:  # pragma: no cover
+                        unclosed_bracket = True
+
+                if unclosed_bracket or not allow_implicit_indents:
+                    # Blank indent stats if not using them
+                    indent_stats = IndentStats(
+                        indent_stats.impulse, indent_stats.trough, ()
+                    )
 
             # Was there a cache?
             if cached_indent_stats:
                 # If there was we can safely assume there is a cached point.
                 assert cached_point
                 # If there was, this is a signal that we need to yield two points.
                 # The content of those points depends on the newlines that surround the
@@ -838,15 +862,21 @@
         # we first build up a buffer.
         point_buffer.append(indent_point)
         _previous_points[indent_point.idx] = indent_point
 
         if not indent_point.is_line_break:
             # If it's not a line break, we should still check whether it's
             # a positive untaken to keep track of them.
-            if indent_point.indent_impulse > indent_point.indent_trough:
+            # ...unless it's implicit.
+            indent_stats = cast(
+                ReflowPoint, elements[indent_point.idx]
+            ).get_indent_impulse()
+            if indent_point.indent_impulse > indent_point.indent_trough and not (
+                allow_implicit_indents and indent_stats.implicit_indents
+            ):
                 untaken_indent_locs[
                     indent_point.initial_indent_balance + indent_point.indent_impulse
                 ] = indent_point.idx
             continue
 
         # If it *is* a line break, then store it.
         lines.append(_IndentLine.from_points(point_buffer))
```

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.0.7/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.0.7/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.6
+Version: 2.0.7
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.6/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.0.7/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.0.7/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.6/test/test_testing.py` & `sqlfluff-2.0.7/test/test_testing.py`

 * *Files identical despite different names*

