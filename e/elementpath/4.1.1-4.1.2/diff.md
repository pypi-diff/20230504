# Comparing `tmp/elementpath-4.1.1.tar.gz` & `tmp/elementpath-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementpath-4.1.1.tar", last modified: Tue Apr 11 07:40:51 2023, max compression
+gzip compressed data, was "elementpath-4.1.2.tar", last modified: Thu May  4 09:50:32 2023, max compression
```

## Comparing `elementpath-4.1.1.tar` & `elementpath-4.1.2.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.358302 elementpath-4.1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.1/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15546 2023-04-11 07:36:42.000000 elementpath-4.1.1/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.1/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.1/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6235 2023-04-11 07:40:51.357302 elementpath-4.1.1/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:37:27.000000 elementpath-4.1.1/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.325302 elementpath-4.1.1/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.1/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.1/doc/advanced.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-04-11 07:36:42.000000 elementpath-4.1.1/doc/conf.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.1/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.1/doc/introduction.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.1/doc/make.bat
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.1/doc/pratt_api.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.1/doc/xpath_api.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.331302 elementpath-4.1.1/elementpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.1/elementpath/collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.1/elementpath/compare.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.337302 elementpath-4.1.1/elementpath/datatypes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/datatypes/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.1/elementpath/datatypes/atomic_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/binary.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/datatypes/datetime.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/numeric.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/proxies.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/qname.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/string.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/datatypes/untyped.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.1/elementpath/datatypes/uri.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.1/elementpath/protocols.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.1/elementpath/py.typed
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.339302 elementpath-4.1.1/elementpath/regex/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.1/elementpath/regex/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.1/elementpath/regex/character_classes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.1/elementpath/regex/codepoints.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/regex/generate_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/regex/patterns.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.1/elementpath/regex/unicode_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/regex/unicode_subsets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17093 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35171 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/tdop.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    12844 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/tree_builders.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.339302 elementpath-4.1.1/elementpath/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/validators/analyze-string.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/validators/schema-for-json.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.340302 elementpath-4.1.1/elementpath/xpath1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.1/elementpath/xpath1/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_axes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28755 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath1/_xpath1_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/xpath1/xpath1_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.342302 elementpath-4.1.1/elementpath/xpath2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.1/elementpath/xpath2/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/_xpath2_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath2/xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.343302 elementpath-4.1.1/elementpath/xpath30/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.1/elementpath/xpath30/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.1/elementpath/xpath30/_translation_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67763 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/_xpath30_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/_xpath30_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.1/elementpath/xpath30/xpath30_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath30/xpath30_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.344302 elementpath-4.1.1/elementpath/xpath31/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.1/elementpath/xpath31/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath31/_xpath31_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath31/_xpath31_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.1/elementpath/xpath31/xpath31_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    29844 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.1/elementpath/xpath_tokens.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.333302 elementpath-4.1.1/elementpath.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6235 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3450 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/SOURCES.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/dependency_links.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/requires.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-04-11 07:40:51.000000 elementpath-4.1.1/elementpath.egg-info/top_level.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.1/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-02-01 12:54:01.000000 elementpath-4.1.1/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-04-11 07:40:51.358302 elementpath-4.1.1/setup.cfg
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2296 2023-04-11 07:36:42.000000 elementpath-4.1.1/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.354302 elementpath-4.1.1/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.1/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/execute_w3c_tests.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/memory_profiling.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.355302 elementpath-4.1.1/tests/mypy_tests/
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2021-11-06 19:48:44.000000 elementpath-4.1.1/tests/mypy_tests/selectors.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-04-11 07:40:51.356302 elementpath-4.1.1/tests/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.1/tests/resources/analyze-string.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.1/tests/resources/sample.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/resources/schema-for-json.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unused_external_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/unused_unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_compare.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_datatypes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.1/tests/test_elementpath.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.1/tests/test_namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_regex.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_schema_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3790 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15390 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14616 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_tdop_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7098 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_tree_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1887 2023-03-01 06:49:20.000000 elementpath-4.1.1/tests/test_typing.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_validators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    83882 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_xpath1_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.1/tests/test_xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    57332 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath30.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath31.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.1/tests/test_xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16701 2023-02-01 12:54:01.000000 elementpath-4.1.1/tests/test_xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/test_xpath_tokens.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11906 2023-03-21 14:20:19.000000 elementpath-4.1.1/tests/xpath_test_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1429 2023-04-11 07:36:42.000000 elementpath-4.1.1/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.998775 elementpath-4.1.2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.2/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15773 2023-04-28 14:38:26.000000 elementpath-4.1.2/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.2/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.2/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-05-04 09:50:31.998775 elementpath-4.1.2/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:55:05.000000 elementpath-4.1.2/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.987775 elementpath-4.1.2/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.2/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.2/doc/advanced.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-04-28 14:38:26.000000 elementpath-4.1.2/doc/conf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.2/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.2/doc/introduction.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.2/doc/make.bat
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.2/doc/pratt_api.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.2/doc/xpath_api.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.989775 elementpath-4.1.2/elementpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.2/elementpath/collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.2/elementpath/compare.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.991775 elementpath-4.1.2/elementpath/datatypes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/datatypes/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.2/elementpath/datatypes/atomic_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/binary.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/datatypes/datetime.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/numeric.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/proxies.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/qname.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/string.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/untyped.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.2/elementpath/datatypes/uri.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.2/elementpath/protocols.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.2/elementpath/py.typed
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.991775 elementpath-4.1.2/elementpath/regex/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.2/elementpath/regex/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.2/elementpath/regex/character_classes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.2/elementpath/regex/codepoints.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/regex/generate_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/regex/patterns.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.2/elementpath/regex/unicode_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/regex/unicode_subsets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17185 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35099 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/tdop.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12572 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/tree_builders.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.992775 elementpath-4.1.2/elementpath/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/validators/analyze-string.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/validators/schema-for-json.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.992775 elementpath-4.1.2/elementpath/xpath1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.2/elementpath/xpath1/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_axes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28752 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/xpath1/xpath1_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.993775 elementpath-4.1.2/elementpath/xpath2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.2/elementpath/xpath2/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.993775 elementpath-4.1.2/elementpath/xpath30/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.2/elementpath/xpath30/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.2/elementpath/xpath30/_translation_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67763 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/_xpath30_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/_xpath30_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/xpath30/xpath30_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/xpath30_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.994775 elementpath-4.1.2/elementpath/xpath31/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.2/elementpath/xpath31/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath31/_xpath31_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath31/_xpath31_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/xpath31/xpath31_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30076 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_tokens.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.990775 elementpath-4.1.2/elementpath.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3478 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/SOURCES.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/dependency_links.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/requires.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/top_level.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.2/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-04-28 13:30:35.000000 elementpath-4.1.2/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-05-04 09:50:31.999775 elementpath-4.1.2/setup.cfg
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2346 2023-04-28 14:38:26.000000 elementpath-4.1.2/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.997775 elementpath-4.1.2/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.2/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/execute_w3c_tests.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/memory_profiling.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.997775 elementpath-4.1.2/tests/mypy_tests/
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2023-04-28 12:53:02.000000 elementpath-4.1.2/tests/mypy_tests/selectors.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.998775 elementpath-4.1.2/tests/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.2/tests/resources/analyze-string.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.2/tests/resources/sample.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/resources/schema-for-json.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unused_external_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unused_unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_compare.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_datatypes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.2/tests/test_elementpath.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.2/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_regex.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_schema_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3793 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15434 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17460 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16558 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_tdop_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7919 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_tree_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1887 2023-04-28 13:22:02.000000 elementpath-4.1.2/tests/test_typing.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_validators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    84012 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_xpath1_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.2/tests/test_xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    57332 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath30.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath31.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/test_xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17766 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-04-26 14:25:47.000000 elementpath-4.1.2/tests/test_xpath_tokens.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11906 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/xpath_test_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1574 2023-04-28 15:16:01.000000 elementpath-4.1.2/tox.ini
```

### Comparing `elementpath-4.1.1/CHANGELOG.rst` & `elementpath-4.1.2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v4.1.2`_ (2023-04-28)
+======================
+* Add support for Python 3.12
+* Fix self shortcut operator (adding is_schema_node() to node classes)
+
 `v4.1.1`_ (2023-04-11)
 ======================
 * Simplify type annotations for XSD datatypes
 * Full test coverage of sequence type functions with bugfixes
 
 `v4.1.0`_ (2023-03-21)
 ======================
@@ -408,7 +413,8 @@
 .. _v3.0.0: https://github.com/sissaschool/elementpath/compare/v2.5.3...v3.0.0
 .. _v3.0.1: https://github.com/sissaschool/elementpath/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/sissaschool/elementpath/compare/v3.0.1...v3.0.2
 .. _v4.0.0: https://github.com/sissaschool/elementpath/compare/v3.0.2...v4.0.0
 .. _v4.0.1: https://github.com/sissaschool/elementpath/compare/v4.0.0...v4.0.1
 .. _v4.1.0: https://github.com/sissaschool/elementpath/compare/v4.0.1...v4.1.0
 .. _v4.1.1: https://github.com/sissaschool/elementpath/compare/v4.1.0...v4.1.1
+.. _v4.1.2: https://github.com/sissaschool/elementpath/compare/v4.1.1...v4.1.2
```

### Comparing `elementpath-4.1.1/LICENSE` & `elementpath-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/PKG-INFO` & `elementpath-4.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.1
+Version: 4.1.2
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `elementpath-4.1.1/README.rst` & `elementpath-4.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/doc/Makefile` & `elementpath-4.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/doc/advanced.rst` & `elementpath-4.1.2/doc/advanced.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/doc/conf.py` & `elementpath-4.1.2/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = 'elementpath'
 copyright = '2018-2023, SISSA (International School for Advanced Studies)'
 author = 'Davide Brunato'
 
 # The short X.Y version
 version = '4.1'
 # The full version, including alpha/beta/rc tags
-release = '4.1.1'
+release = '4.1.2'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `elementpath-4.1.1/doc/make.bat` & `elementpath-4.1.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/doc/pratt_api.rst` & `elementpath-4.1.2/doc/pratt_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/doc/xpath_api.rst` & `elementpath-4.1.2/doc/xpath_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/__init__.py` & `elementpath-4.1.2/elementpath/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-__version__ = '4.1.1'
+__version__ = '4.1.2'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2018-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 # Imports here are considered as stable API, other internal calls may change.
```

### Comparing `elementpath-4.1.1/elementpath/collations.py` & `elementpath-4.1.2/elementpath/collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/compare.py` & `elementpath-4.1.2/elementpath/compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/__init__.py` & `elementpath-4.1.2/elementpath/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/atomic_types.py` & `elementpath-4.1.2/elementpath/datatypes/atomic_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/binary.py` & `elementpath-4.1.2/elementpath/datatypes/binary.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/datetime.py` & `elementpath-4.1.2/elementpath/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/numeric.py` & `elementpath-4.1.2/elementpath/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/proxies.py` & `elementpath-4.1.2/elementpath/datatypes/proxies.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/qname.py` & `elementpath-4.1.2/elementpath/datatypes/qname.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/string.py` & `elementpath-4.1.2/elementpath/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/untyped.py` & `elementpath-4.1.2/elementpath/datatypes/untyped.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/datatypes/uri.py` & `elementpath-4.1.2/elementpath/datatypes/uri.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/etree.py` & `elementpath-4.1.2/elementpath/etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/exceptions.py` & `elementpath-4.1.2/elementpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/helpers.py` & `elementpath-4.1.2/elementpath/helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/namespaces.py` & `elementpath-4.1.2/elementpath/namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/protocols.py` & `elementpath-4.1.2/elementpath/protocols.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/__init__.py` & `elementpath-4.1.2/elementpath/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/character_classes.py` & `elementpath-4.1.2/elementpath/regex/character_classes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/codepoints.py` & `elementpath-4.1.2/elementpath/regex/codepoints.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/generate_categories.py` & `elementpath-4.1.2/elementpath/regex/generate_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/patterns.py` & `elementpath-4.1.2/elementpath/regex/patterns.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/unicode_categories.py` & `elementpath-4.1.2/elementpath/regex/unicode_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/regex/unicode_subsets.py` & `elementpath-4.1.2/elementpath/regex/unicode_subsets.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/schema_proxy.py` & `elementpath-4.1.2/elementpath/schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/sequence_types.py` & `elementpath-4.1.2/elementpath/sequence_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/serialization.py` & `elementpath-4.1.2/elementpath/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def get_serialization_params(params: Union[None, ElementNode, XPathMap] = None,
                              token: Optional[XPathToken] = None) -> Dict['str', Any]:
 
     kwargs: Dict[str, Any] = {}
     if isinstance(params, XPathMap):
-        if len(params[:]) > len(params.keys()):
+        if len(params[:]) > len(params.keys()):  # pragma: no cover
             raise xpath_error('SEPM0019', token=token)
 
         for key, value in params.items():
             if not isinstance(key, str) or value is None:
                 continue
             elif isinstance(value, UntypedAtomic):
                 value = str(value)
@@ -59,24 +59,25 @@
 
             elif key == 'cdata-section-elements':
                 # TODO: doesn't work within element nodes
                 if isinstance(value, XPathArray):
                     value = value.items()
                 if not isinstance(value, list) or not all(isinstance(x, QName) for x in value):
                     raise xpath_error('XPTY0004', token=token)
-                kwargs['cdata-section-elements'] = value
+                kwargs['cdata_section'] = value
 
             elif key == 'method':
                 if value not in ('html', 'xml', 'xhtml', 'text', 'adaptive', 'json'):
                     raise xpath_error('SEPM0017', token=token)
-                kwargs['method'] = value if value != 'xhtml' else 'html'
+                kwargs[key] = value if value != 'xhtml' else 'html'
 
             elif key == 'indent':
                 if not isinstance(value, bool):
                     raise xpath_error('XPTY0004', token=token)
+                kwargs[key] = value
 
             elif key == 'item-separator':
                 if not isinstance(value, str):
                     raise xpath_error('XPTY0004', token=token)
                 kwargs['item_separator'] = value
 
             elif key == 'use-character-maps':
@@ -86,22 +87,23 @@
                 kwargs['character_map'] = character_map = {}
                 for k, v in value.items():
                     if not isinstance(k, str) or not isinstance(v, str):
                         raise xpath_error('XPTY0004', token=token)
                     elif len(k) != 1:
                         msg = f'invalid character {k!r} in character map'
                         raise xpath_error('SEPM0016', msg, token)
-                    elif k in character_map:
-                        msg = f'duplicate character {k!r} in character map'
-                        raise xpath_error('SEPM0018', msg, token)
                     else:
                         character_map[k] = v
 
-            elif key == 'suppress-indentation':
-                pass  # TODO param
+            elif key == 'suppress-indentation':  # pragma: no cover
+                if isinstance(value, QName) or isinstance(value, list) \
+                        and all(isinstance(x, QName) for x in value):
+                    kwargs[key] = value
+                else:
+                    raise xpath_error('XPTY0004', token=token)
             elif key == 'standalone':
                 if not value and isinstance(value, list):
                     pass
                 elif isinstance(value, bool):
                     kwargs['standalone'] = value
                 else:
                     if value not in ('yes', 'no', 'omit'):
@@ -113,28 +115,28 @@
                 if not isinstance(value, (str, QName)):
                     raise xpath_error('XPTY0004', token=token)
                 kwargs[key] = value
 
             elif key == 'allow-duplicate-names':
                 if value is not None and not isinstance(value, bool):
                     raise xpath_error('XPTY0004', token=token)
-                kwargs[key] = value
+                kwargs['allow_duplicate_names'] = value
 
             elif key == 'encoding':
                 if not isinstance(value, str):
                     raise xpath_error('XPTY0004', token=token)
                 kwargs[key] = value
 
             elif key == 'html-version':
                 if not isinstance(value, (int, Decimal)):
                     raise xpath_error('XPTY0004', token=token)
                 kwargs[key] = value
 
     elif isinstance(params, ElementNode):
-        root = params.value
+        root = params.elem
         if root.tag != SERIALIZATION_PARAMS:
             msg = 'output:serialization-parameters tag expected'
             raise xpath_error('XPTY0004', msg, token)
 
         if len(root) > len({e.tag for e in root}):
             raise xpath_error('SEPM0019', token=token)
 
@@ -254,37 +256,37 @@
     if etree_module is None:
         from xml.etree import ElementTree
         etree_module = ElementTree
 
     item_separator = params.get('item_separator')
     character_map = params.get('character_map')
 
-    cdata_sections: Union[Set[str], Tuple[()]]
+    cdata_section: Union[Set[str], Tuple[()]]
     kwargs = {}
     if 'xml_declaration' in params:
         kwargs['xml_declaration'] = params['xml_declaration']
     if 'standalone' in params:
         kwargs['standalone'] = params['standalone']
-    if 'cdata-section-elements' in params:
-        cdata_sections = {x.expanded_name for x in params['cdata-section-elements']}
+    if 'cdata_section' in params:
+        cdata_section = {x.expanded_name for x in params['cdata_section']}
     else:
-        cdata_sections = ()
+        cdata_section = ()
 
     method = kwargs.get('method', 'xml')
     if method == 'xhtml':
         method = 'html'
 
     chunks = []
     for item in iter_normalized(elements, item_separator):
         if isinstance(item, ElementNode):
             item = item.elem
         elif isinstance(item, (AttributeNode, NamespaceNode)):
             raise xpath_error('SENR0001', token=token)
         elif isinstance(item, TextNode):
-            if item.parent is not None and item.parent.name in cdata_sections:
+            if item.parent is not None and item.parent.name in cdata_section:
                 chunks.append(f'<![CDATA[{item.value}]]>')
             else:
                 chunks.append(item.value)
             continue
         elif not isinstance(item, str):
             raise xpath_error('SENR0001', token=token)
         else:
@@ -351,41 +353,39 @@
                 elif isinstance(obj, (AttributeNode, NamespaceNode)):
                     return f'{obj.name}="{obj.string_value}"'
                 elif isinstance(obj, TextNode):
                     return obj.value
                 elif isinstance(obj, CommentNode):
                     return f'<!--{obj.string_value}-->'
                 else:
-                    return f'<?{obj.string_value}?>'
+                    return f'<?{obj.name} {obj.string_value}?>'
             elif isinstance(obj, XPathMap):
                 if any(isinstance(v, list) and len(v) > 1 for v in obj.values()):
                     raise xpath_error('SERE0023', token=token)
 
                 map_keys = set()
                 map_items = []
                 k: Any
                 for k, v in obj.items():
                     if isinstance(k, QName):
                         k = str(k)
                     map_items.append((k, v))
 
                     if k not in map_keys:
                         map_keys.add(k)
-                    elif not params.get('allow-duplicate-names'):
+                    elif not params.get('allow_duplicate_names'):
                         raise xpath_error('SERE0022', token=token)
                 return MapEncodingDict(map_items)
 
             elif isinstance(obj, XPathArray):
                 return [v if v or not isinstance(v, list) else None for v in obj.items()]
             elif isinstance(obj, (AbstractBinary, AbstractDateTime, AnyURI, UntypedAtomic)):
                 return str(obj)
             elif isinstance(obj, Decimal):
                 return float(Decimal(obj).quantize(Decimal("0.01"), ROUND_UP))
-            elif not obj and isinstance(obj, list):
-                return super().default(None)
             else:
                 return super().default(obj)
 
     kwargs: Dict[str, Any] = {
         'cls': XPathEncoder,
         'ensure_ascii': True,
         'separators': (',', ':'),
@@ -393,14 +393,16 @@
     }
     try:
         parts = [json.dumps(x, **kwargs) for x in elements]
     except ElementPathError:
         raise
     except ValueError:
         raise xpath_error('SERE0020', token=token)
+    except TypeError:
+        raise xpath_error('SERE0021', token=token)
 
     if not parts:
         return 'null'
     elif len(parts) > 1:
         raise xpath_error('SERE0023', token=token)
 
     result = parts[0].replace('/', '\\/')
```

### Comparing `elementpath-4.1.1/elementpath/tdop.py` & `elementpath-4.1.2/elementpath/tdop.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,18 @@
                  value: Optional[Any] = None) -> None:
         self._items = []
         self.parser = parser
         self.value = value if value is not None else self.symbol
         self.span = (0, 0) if parser.next_match is None else parser.next_match.span()
 
     @overload
-    def __getitem__(self, i: int) -> TK: ...
+    def __getitem__(self, i: int) -> TK: ...  # pragma: no cover
 
     @overload
-    def __getitem__(self, s: slice) -> MutableSequence[TK]: ...
+    def __getitem__(self, s: slice) -> MutableSequence[TK]: ...  # pragma: no cover
 
     def __getitem__(self, i: Union[int, slice]) \
             -> Union[TK, MutableSequence[TK]]:
         return self._items[i]
 
     def __setitem__(self, i: Union[int, slice], o: Any) -> None:
         self._items[i] = o
@@ -219,23 +219,21 @@
     def tree(self) -> str:
         """Returns a tree representation string."""
         if self.symbol == '(name)':
             return '(%s)' % self.value
         elif self.symbol in SPECIAL_SYMBOLS:
             return '(%r)' % self.value
         elif self.symbol == '(':
-            if not self:
-                return '()'
-            elif len(self) == 1:
+            if len(self) == 1:
                 return self[0].tree
-            return '(%s)' % ' '.join(item.tree for item in self)
+            return f"({' '.join(item.tree for item in self)})"
         elif not self:
             return '(%s)' % self.symbol
         else:
-            return '(%s %s)' % (self.symbol, ' '.join(item.tree for item in self))
+            return f"({self.symbol} {' '.join(item.tree for item in self)})"
 
     @property
     def source(self) -> str:
         """Returns the source representation string."""
         symbol = self.symbol
         if symbol == '(name)':
             return cast(str, self.value)
@@ -326,30 +324,15 @@
         """Returns a generator for iterating the token's tree."""
         status: List[Tuple[Optional['Token[TK]'], Iterator['Token[TK]']]] = []
         parent: Optional['Token[TK]'] = self
         children: Iterator['Token[TK]'] = iter(self)
         tk: 'Token[TK]'
 
         while True:
-            try:
-                tk = next(children)
-            except StopIteration:
-                try:
-                    parent, children = status.pop()
-                except IndexError:
-                    if parent is not None:
-                        if not symbols or parent.symbol in symbols:
-                            yield parent
-                    return
-                else:
-                    if parent is not None:
-                        if not symbols or parent.symbol in symbols:
-                            yield parent
-                        parent = None
-            else:
+            for tk in children:
                 if parent is not None and len(parent._items) == 1:
                     if not symbols or parent.symbol in symbols:
                         yield parent
                     parent = None
 
                 if not tk._items:
                     if not symbols or tk.symbol in symbols:
@@ -357,14 +340,28 @@
                     if parent is not None:
                         if not symbols or parent.symbol in symbols:
                             yield parent
                         parent = None
                     continue
                 status.append((parent, children))
                 parent, children = tk, iter(tk)
+                break
+            else:
+                try:
+                    parent, children = status.pop()
+                except IndexError:
+                    if parent is not None:
+                        if not symbols or parent.symbol in symbols:
+                            yield parent
+                    return
+                else:
+                    if parent is not None:
+                        if not symbols or parent.symbol in symbols:
+                            yield parent
+                        parent = None
 
     def expected(self, *symbols: str, message: Optional[str] = None) -> None:
         if symbols and self.symbol not in symbols:
             raise self.wrong_syntax(message)
 
     def unexpected(self, *symbols: str, message: Optional[str] = None) -> None:
         if not symbols or self.symbol in symbols:
@@ -800,15 +797,15 @@
         """
         token_class = cls.register(symbol, label='operator', lbp=bp, rbp=bp)
 
         @no_type_check_decorator
         def bind(func: Callable[..., Any]) -> Callable[..., Any]:
             method_name = func.__name__.partition('_')[0]
             if not callable(getattr(token_class, method_name)):
-                raise TypeError(f"The attribute {method_name!r} is not a callable of {token_class}")
+                raise TypeError(f"{method_name!r} is not a method of {token_class}")
             setattr(token_class, method_name, func)
             return func
         return bind
 
     @classmethod
     def build(cls) -> None:
         """
```

### Comparing `elementpath-4.1.1/elementpath/tree_builders.py` & `elementpath-4.1.2/elementpath/tree_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,18 +257,14 @@
                 iterators.append(children)
                 children = iter(elem)
                 break
         else:
             try:
                 children, parent = iterators.pop(), ancestors.pop()
             except IndexError:
-                if isinstance(root_node, ElementNode) and root_node.elem is not root:
-                    for _node in root_node.iter_descendants():
-                        if isinstance(_node, ElementNode) and _node.elem is root:
-                            return _node
                 return root_node
 
 
 def build_schema_node_tree(root: SchemaElemType,
                            elements: Optional[ElementMapType] = None,
                            global_elements: Optional[List[ChildNodeType]] = None) \
         -> SchemaElementNode:
```

### Comparing `elementpath-4.1.1/elementpath/validators/__init__.py` & `elementpath-4.1.2/elementpath/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/validators/analyze-string.xsd` & `elementpath-4.1.2/elementpath/validators/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/validators/schema-for-json.xsd` & `elementpath-4.1.2/elementpath/validators/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath1/_xpath1_axes.py` & `elementpath-4.1.2/elementpath/xpath1/_xpath1_axes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath1/_xpath1_functions.py` & `elementpath-4.1.2/elementpath/xpath1/_xpath1_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath1/_xpath1_operators.py` & `elementpath-4.1.2/elementpath/xpath1/_xpath1_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 def select_self_shortcut(self, context=None):
     if context is None:
         raise self.missing_context()
 
     elif isinstance(context, XPathSchemaContext):
         for item in context.iter_self():
             if isinstance(item, (AttributeNode, ElementNode)):
-                if item.is_schema_element():
+                if item.is_schema_node():
                     self.add_xsd_type(item)
                 elif item is context.root:
                     # item is the schema
                     for xsd_element in item:
                         self.add_xsd_type(xsd_element)
             yield item
```

### Comparing `elementpath-4.1.1/elementpath/xpath1/xpath1_parser.py` & `elementpath-4.1.2/elementpath/xpath1/xpath1_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath2/__init__.py` & `elementpath-4.1.2/elementpath/xpath2/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath2/_xpath2_constructors.py` & `elementpath-4.1.2/elementpath/xpath2/_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath2/_xpath2_functions.py` & `elementpath-4.1.2/elementpath/xpath2/_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath2/_xpath2_operators.py` & `elementpath-4.1.2/elementpath/xpath2/_xpath2_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath2/xpath2_parser.py` & `elementpath-4.1.2/elementpath/xpath2/xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/__init__.py` & `elementpath-4.1.2/elementpath/xpath30/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/_translation_maps.py` & `elementpath-4.1.2/elementpath/xpath30/_translation_maps.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/_xpath30_functions.py` & `elementpath-4.1.2/elementpath/xpath30/_xpath30_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/_xpath30_operators.py` & `elementpath-4.1.2/elementpath/xpath30/_xpath30_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/xpath30_helpers.py` & `elementpath-4.1.2/elementpath/xpath30/xpath30_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath30/xpath30_parser.py` & `elementpath-4.1.2/elementpath/xpath30/xpath30_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath31/__init__.py` & `elementpath-4.1.2/elementpath/xpath31/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath31/_xpath31_functions.py` & `elementpath-4.1.2/elementpath/xpath31/_xpath31_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath31/_xpath31_operators.py` & `elementpath-4.1.2/elementpath/xpath31/_xpath31_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath31/xpath31_parser.py` & `elementpath-4.1.2/elementpath/xpath31/xpath31_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath_context.py` & `elementpath-4.1.2/elementpath/xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath_nodes.py` & `elementpath-4.1.2/elementpath/xpath_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,21 @@
     def string_value(self) -> str:
         raise NotImplementedError()
 
     @property
     def typed_value(self) -> Optional[AtomicValueType]:
         raise NotImplementedError()
 
-    # Other common attributes and methods
+    # Other common attributes, properties and methods
     value: Any
     position: int  # for document total order
 
+    def is_schema_node(self) -> Optional[bool]:
+        return None
+
     def match_name(self, name: str, default_namespace: Optional[str] = None) -> bool:
         """
         Returns `True` if the argument is matching the name of the node, `False` otherwise.
         Raises a ValueError if the argument is used, but it's in a wrong format.
 
         :param name: a fully qualified name, a local name or a wildcard. The accepted \
         wildcard formats are '*', '*:*', '*:local-name' and '{namespace}*'.
@@ -186,14 +189,17 @@
 
     @property
     def path(self) -> str:
         if self.parent is None:
             return f'@{self._name}'
         return f'{self.parent.path}/@{self._name}'
 
+    def is_schema_node(self) -> bool:
+        return hasattr(self.value, 'name') and hasattr(self.value, 'type')
+
     def match_name(self, name: str, default_namespace: Optional[str] = None) -> bool:
         if '*' in name:
             return match_wildcard(self._name, name)
         else:
             return self._name == name
 
 
@@ -559,30 +565,32 @@
             position = self.position + len(self.nsmap) + int('xml' not in self.nsmap)
             self._attributes = [
                 AttributeNode(name, value, self, pos)
                 for pos, (name, value) in enumerate(self.elem.attrib.items(), position)
             ]
         return self._attributes
 
-    def is_schema_element(self) -> bool:
-        return hasattr(self.elem, 'name') and hasattr(self.elem, 'type')
-
     @property
     def path(self) -> str:
         """Returns an absolute path for the node."""
         path = []
         item: Any = self
         while True:
             if isinstance(item, ElementNode):
                 path.append(item.elem.tag)
 
             item = item.parent
             if item is None:
                 return '/{}'.format('/'.join(reversed(path)))
 
+    def is_schema_node(self) -> bool:
+        return hasattr(self.elem, 'name') and hasattr(self.elem, 'type')
+
+    is_schema_element = is_schema_node
+
     def match_name(self, name: str, default_namespace: Optional[str] = None) -> bool:
         if '*' in name:
             return match_wildcard(self.elem.tag, name)
         elif not name:
             return not self.elem.tag
         elif hasattr(self.elem, 'type'):
             return cast(XsdElementProtocol, self.elem).is_matching(name, default_namespace)
```

### Comparing `elementpath-4.1.1/elementpath/xpath_selectors.py` & `elementpath-4.1.2/elementpath/xpath_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath/xpath_tokens.py` & `elementpath-4.1.2/elementpath/xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/elementpath.egg-info/PKG-INFO` & `elementpath-4.1.2/elementpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.1
+Version: 4.1.2
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `elementpath-4.1.1/elementpath.egg-info/SOURCES.txt` & `elementpath-4.1.2/elementpath.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 tests/test_namespaces.py
 tests/test_package.py
 tests/test_regex.py
 tests/test_schema_context.py
 tests/test_schema_proxy.py
 tests/test_selectors.py
 tests/test_sequence_types.py
+tests/test_serialization.py
 tests/test_tdop_parser.py
 tests/test_tree_builders.py
 tests/test_typing.py
 tests/test_validators.py
 tests/test_xpath1_parser.py
 tests/test_xpath2_constructors.py
 tests/test_xpath2_functions.py
```

### Comparing `elementpath-4.1.1/setup.py` & `elementpath-4.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='elementpath',
-    version='4.1.1',
+    version='4.1.2',
     packages=find_packages(include=['elementpath', 'elementpath.*']),
     package_data={
         'elementpath': ['py.typed'],
         'elementpath.validators': ['analyze-string.xsd', 'schema-for-json.xsd'],
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
@@ -45,13 +45,14 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Libraries',
         'Topic :: Text Processing :: Markup :: XML',
     ]
 )
```

### Comparing `elementpath-4.1.1/tests/execute_w3c_tests.py` & `elementpath-4.1.2/tests/execute_w3c_tests.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/memory_profiling.py` & `elementpath-4.1.2/tests/memory_profiling.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/resources/analyze-string.xsd` & `elementpath-4.1.2/tests/resources/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/resources/schema-for-json.xsd` & `elementpath-4.1.2/tests/resources/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_collations.py` & `elementpath-4.1.2/tests/test_collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_compare.py` & `elementpath-4.1.2/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_datatypes.py` & `elementpath-4.1.2/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_elementpath.py` & `elementpath-4.1.2/tests/test_elementpath.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_etree.py` & `elementpath-4.1.2/tests/test_etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_exceptions.py` & `elementpath-4.1.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_helpers.py` & `elementpath-4.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_namespaces.py` & `elementpath-4.1.2/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_package.py` & `elementpath-4.1.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_regex.py` & `elementpath-4.1.2/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_schema_context.py` & `elementpath-4.1.2/tests/test_schema_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_schema_proxy.py` & `elementpath-4.1.2/tests/test_schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_selectors.py` & `elementpath-4.1.2/tests/test_selectors.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 try:
     import lxml.etree as lxml_etree
 except ImportError:
     lxml_etree = None
 
 
 class XPathSelectorsTest(unittest.TestCase):
-    root = ElementTree.XML('<author>Dickens</author>')
     etree = ElementTree
 
+    @classmethod
+    def setUpClass(cls) -> None:
+        cls.root = cls.etree.XML('<author>Dickens</author>')
+
     def test_select_function(self):
         self.assertListEqual(select(self.root, 'text()'), ['Dickens'])
         self.assertEqual(select(self.root, '$a', variables={'a': 1}), 1)
 
         self.assertEqual(
             select(self.root, '$a', variables={'a': 1}, variable_types={'a': 'xs:decimal'}), 1
         )
@@ -64,15 +67,14 @@
         selector2 = Selector('sup[1]/following-sibling::text()')
         root = self.etree.XML('<root><sup>1</sup>b<sup>2</sup>c<sup>3</sup>d</root>')
         self.assertListEqual(selector1.select(root), selector2.select(root))
 
 
 @unittest.skipIf(lxml_etree is None, "The lxml library is not installed")
 class LxmlXPathSelectorsTest(XPathSelectorsTest):
-    root = lxml_etree.XML('<author>Dickens</author>')
     etree = lxml_etree
 
     def test_issue_058(self):
         tei = """<?xml version='1.0' encoding='UTF8'?>
         <?xml-model type="application/xml"?>
         <TEI xmlns="http://www.tei-c.org/ns/1.0">
           <text>
```

### Comparing `elementpath-4.1.1/tests/test_sequence_types.py` & `elementpath-4.1.2/tests/test_sequence_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 # @author Davide Brunato <brunato@sissa.it>
 #
 import unittest
 import io
 from textwrap import dedent
 from xml.etree import ElementTree
 
-import xmlschema.xpath
+try:
+    import xmlschema
+except ImportError:
+    xmlschema = None
 
 from elementpath.sequence_types import normalize_sequence_type, is_instance, \
     is_sequence_type, match_sequence_type, is_sequence_type_restriction
 from elementpath import XPath2Parser, XPathContext
 from elementpath.xpath3 import XPath30Parser, XPath31Parser
 from elementpath.namespaces import XSD_NAMESPACE, XSD_UNTYPED_ATOMIC, \
     XSD_ANY_ATOMIC_TYPE, XSD_ANY_SIMPLE_TYPE, XSI_NIL, XSD_STRING
```

### Comparing `elementpath-4.1.1/tests/test_tdop_parser.py` & `elementpath-4.1.2/tests/test_tdop_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,23 @@
 
 
 class TdopParserTest(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         class ExpressionParser(Parser):
-            SYMBOLS = {'(integer)', '+', '-', '(name)', '(end)', '(invalid)', '(unknown)'}
-
             @classmethod
             def create_tokenizer(cls, symbol_table):
                 return re.compile(
                     r'INCOMPATIBLE | (\d+) | (UNKNOWN|[+\-]) | (\w+) | (\S)| \s+',
                     flags=re.VERBOSE
                 )
 
         ExpressionParser.literal('(integer)')
-        ExpressionParser.register('(name)', bp=100, lbp=100)
-        ExpressionParser.register('(end)')
-        ExpressionParser.register('(invalid)')
-        ExpressionParser.register('(unknown)')
+        ExpressionParser.register('(name)')
 
         @ExpressionParser.method(ExpressionParser.infix('+', bp=40))
         def evaluate_plus(self, context=None):
             return self[0].evaluate(context) + self[1].evaluate(context)
 
         @ExpressionParser.method(ExpressionParser.infix('-', bp=40))
         def evaluate_minus(self, context=None):
@@ -131,18 +126,44 @@
                              [('5', '', '', ''), ('', '', 'x', '')])
 
     def test_incompatible_tokenizer(self):
         with self.assertRaises(RuntimeError) as ec:
             self.parser.parse('INCOMPATIBLE')
         self.assertIn("incompatible tokenizer", str(ec.exception))
 
+    def test_string_repr(self):
+        self.assertEqual(repr(self.parser), 'ExpressionParser()')
+        self.assertEqual(str(self.parser), repr(self.parser))
+
     def test_expression(self):
         token = self.parser.parse('10 + 6')
         self.assertEqual(token.evaluate(), 16)
 
+    def test_iter_method(self):
+        token = self.parser.parse('9 + 7 - 5')
+
+        self.assertListEqual(list(tk.source for tk in token.iter()),
+                             ['9', '9 + 7', '7', '9 + 7 - 5', '5'])
+        self.assertListEqual(list(tk.source for tk in token.iter('(integer)')),
+                             ['9', '7', '5'])
+        self.assertListEqual(list(tk.source for tk in token.iter('(name)')), [])
+
+        class SampleParser(Parser):
+            pass
+
+        @SampleParser.method(SampleParser.nullary('.'))
+        def evaluate_self(_self, _context=None):
+            return _self
+
+        parser = SampleParser()
+        token = parser.parse('.')
+        self.assertListEqual(list(tk.source for tk in token.iter()), ['.'])
+        self.assertListEqual(list(tk.source for tk in token.iter('.')), ['.'])
+        self.assertListEqual(list(tk.source for tk in token.iter('..')), [])
+
     def test_syntax_errors(self):
         with self.assertRaises(ParseError) as ec:
             self.parser.parse('x')   # with nud()
         self.assertEqual(str(ec.exception), "unexpected name 'x'")
 
         with self.assertRaises(ParseError) as ec:
             self.parser.parse('5y')  # with led()
@@ -300,27 +321,37 @@
         self.assertIs(AnotherParser.token_base_class, Token)
         self.assertEqual(AnotherParser.literals_pattern.pattern,
                          r"""'[^']*'|"[^"]*"|(?:\d+|\.\d+)(?:\.\d*)?(?:[Ee][+-]?\d+)?""")
 
     def test_invalid_registrations(self):
 
         class AnotherParser(Parser):
-            SYMBOLS = {'(integer)', r'function\(', '(name)', '(end)'}
+            SYMBOLS = {'(integer)', '(name)'}
 
         with self.assertRaises(ValueError) as ec:
             AnotherParser.register(r'function \(')
         self.assertIn("a symbol can't contain whitespaces", str(ec.exception))
 
+        with self.assertRaises(TypeError) as ec:
+            AnotherParser.register(9)
+        self.assertIn("A string or a", str(ec.exception))
+
+        with self.assertRaises(ValueError) as ec:
+            AnotherParser.register(self.parser.symbol_table['+'])
+        self.assertIn("Token class ", str(ec.exception))
+        self.assertIn("is not registered", str(ec.exception))
+
     def test_other_operators(self):
 
         class ExpressionParser(Parser):
-            SYMBOLS = {'(integer)', '+', '++', '-', '*', '(end)'}
+            SYMBOLS = {'(integer)', '+', '++', '-', '*', '(name)'}
 
         ExpressionParser.prefix('++')
         ExpressionParser.postfix('+')
+        ExpressionParser.nullary('(name)')
 
         @ExpressionParser.method(ExpressionParser.prefix('++', bp=90))
         def evaluate_increment(self_, context=None):
             return self_[0].evaluate(context) + 1
 
         @ExpressionParser.method(ExpressionParser.postfix('+', bp=90))
         def evaluate_plus(self_, context=None):
@@ -340,20 +371,39 @@
         def evaluate_mul(self_, context=None):
             return self_[0].evaluate(context) * \
                 self_[1].evaluate(context) * self_[2].evaluate(context)
 
         ExpressionParser.literal('(integer)')
         ExpressionParser.register('(end)')
 
+        with self.assertRaises(AttributeError) as ec:
+            @ExpressionParser.method('*', bp=70)
+            def foo_mul(self_):
+                return None
+        self.assertIn("has no attribute 'foo'", str(ec.exception))
+
+        with self.assertRaises(TypeError) as ec:
+            @ExpressionParser.method('*', bp=70)
+            def label_mul(self_):
+                return None
+        self.assertIn("'label' is not a method of ", str(ec.exception))
+
         parser = ExpressionParser()
 
+        token = parser.parse('foo')
+        self.assertEqual(token.evaluate(), 'foo')
+
         token = parser.parse('++5')
         self.assertEqual(token.source, '++ 5')
         self.assertEqual(token.evaluate(), 6)
 
+        with self.assertRaises(ParseError) as ec:
+            parser.parse('1 ++ 5')
+        self.assertEqual(str(ec.exception), "unexpected '++' prefix operator")
+
         token = parser.parse('8 +')
         self.assertEqual(token.source, '8 +')
         self.assertEqual(token.evaluate(), 9)
 
         token = parser.parse(' 8 -  5')
         self.assertEqual(token.source, '8 - 5')
         self.assertEqual(token.evaluate(), 3)
```

### Comparing `elementpath-4.1.1/tests/test_tree_builders.py` & `elementpath-4.1.2/tests/test_tree_builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,18 @@
         <!-- Child 1 comment -->
         <elem1 a1="value1"/>
         <elem2 a2="value2"/>
         child1 text2
     </child1>
     <child2/>
     <tns:other/>
+    <?PI-target PI content?>
 </root>
+<?xml-model type="application/xml"?>
+<!-- Document comment 2 -->
 """
 
 
 class TreeBuildersTest(unittest.TestCase):
     namespaces = {'tns': "http://elementpath.test/ns"}
 
     def test_build_node_tree_with_element(self):
@@ -77,51 +80,55 @@
         self.assertIsInstance(node[0].children[3], ElementNode)
         self.assertIsInstance(node[0].children[4], TextNode)
         self.assertIsInstance(node[0].children[5], ElementNode)
         self.assertIsInstance(node[0].children[6], TextNode)
 
     @unittest.skipIf(sys.version_info <= (3, 8),
                      "Comments not available in ElementTree")
-    def test_build_node_tree_with_comments(self):
+    def test_build_node_tree_with_comments_and_pis(self):
         parser = ElementTree.XMLParser(
             target=ElementTree.TreeBuilder(
                 insert_comments=True, insert_pis=True
             )
         )
         root = ElementTree.XML(XML_DATA, parser=parser)
         node = build_node_tree(root, self.namespaces)
         self.assertIsInstance(node, ElementNode)
 
-        self.assertEqual(len(node.children), 9)
+        self.assertEqual(len(node.children), 11)
         self.assertIsInstance(node.children[0], TextNode)
         self.assertIsInstance(node.children[1], CommentNode)
         self.assertIsInstance(node.children[2], TextNode)
         self.assertIsInstance(node.children[3], ElementNode)
         self.assertIsInstance(node.children[4], TextNode)
         self.assertIsInstance(node.children[5], ElementNode)
         self.assertIsInstance(node.children[6], TextNode)
-        self.assertIsInstance(node.children[5], ElementNode)
-        self.assertIsInstance(node.children[6], TextNode)
+        self.assertIsInstance(node.children[7], ElementNode)
+        self.assertIsInstance(node.children[8], TextNode)
+        self.assertIsInstance(node.children[9], ProcessingInstructionNode)
+        self.assertIsInstance(node.children[10], TextNode)
 
     @unittest.skipIf(lxml_etree is None, "lxml library is not installed")
     def test_build_lxml_node_tree_with_element(self):
         root = lxml_etree.XML(XML_DATA.encode('utf-8'))
         node = build_lxml_node_tree(root)
 
         self.assertIsInstance(node, DocumentNode)
         self.assertEqual(node.position, 0)
         self.assertIsNotNone(node.document)
-        self.assertEqual(len(node.children), 3)
+        self.assertEqual(len(node.children), 5)
         self.assertIsInstance(node.children[0], ProcessingInstructionNode)
         self.assertIsInstance(node.children[1], CommentNode)
         self.assertIsInstance(node.children[2], ElementNode)
+        self.assertIsInstance(node.children[3], ProcessingInstructionNode)
+        self.assertIsInstance(node.children[4], CommentNode)
 
         self.assertIsInstance(node[2], ElementNode)
         self.assertEqual(node[2].position, 3)
-        self.assertEqual(len(node[2].children), 9)
+        self.assertEqual(len(node[2].children), 11)
         self.assertIsInstance(node[2].children[0], TextNode)
         self.assertIsInstance(node[2].children[1], CommentNode)
         self.assertIsInstance(node[2].children[2], TextNode)
         self.assertIsInstance(node[2].children[3], ElementNode)
         self.assertIsInstance(node[2].children[4], TextNode)
         self.assertIsInstance(node[2].children[5], ElementNode)
         self.assertIsInstance(node[2].children[6], TextNode)
@@ -143,28 +150,39 @@
     def test_build_lxml_node_tree_with_element_tree(self):
         root = lxml_etree.parse(io.BytesIO(XML_DATA.encode('utf-8')))
         node = build_lxml_node_tree(root)
 
         self.assertIsInstance(node, DocumentNode)
         self.assertEqual(node.position, 1)
         self.assertIs(node.document, root)
-        self.assertEqual(len(node.children), 3)
+        self.assertEqual(len(node.children), 5)
         self.assertIsInstance(node.children[0], ProcessingInstructionNode)
         self.assertIsInstance(node.children[1], CommentNode)
         self.assertIsInstance(node.children[2], ElementNode)
+        self.assertIsInstance(node.children[3], ProcessingInstructionNode)
+        self.assertIsInstance(node.children[4], CommentNode)
 
         self.assertIsInstance(node[2], ElementNode)
         self.assertEqual(node[2].position, 4)
-        self.assertEqual(len(node[2].children), 9)
+        self.assertEqual(len(node[2].children), 11)
         self.assertIsInstance(node[2].children[0], TextNode)
         self.assertIsInstance(node[2].children[1], CommentNode)
         self.assertIsInstance(node[2].children[2], TextNode)
         self.assertIsInstance(node[2].children[3], ElementNode)
         self.assertIsInstance(node[2].children[4], TextNode)
         self.assertIsInstance(node[2].children[5], ElementNode)
         self.assertIsInstance(node[2].children[6], TextNode)
         self.assertIsInstance(node[2].children[5], ElementNode)
         self.assertIsInstance(node[2].children[6], TextNode)
 
+        root = lxml_etree.ElementTree()
+        self.assertIsNone(root.getroot())
+        node = build_lxml_node_tree(root)
+
+        self.assertIsInstance(node, DocumentNode)
+        self.assertEqual(node.position, 1)
+        self.assertIs(node.document, root)
+        self.assertEqual(len(node.children), 0)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `elementpath-4.1.1/tests/test_typing.py` & `elementpath-4.1.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_validators.py` & `elementpath-4.1.2/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath1_parser.py` & `elementpath-4.1.2/tests/test_xpath1_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #       References:
 #           http://www.w3.org/TR/1999/REC-xpath-19991116/
 #           http://www.w3.org/TR/2010/REC-xpath20-20101214/
 #           http://www.w3.org/TR/2010/REC-xpath-functions-20101214/
 #           https://www.w3.org/Consortium/Legal/2015/doc-license
 #           https://www.w3.org/TR/charmod-norm/
 #
+import sys
 import unittest
 import io
 import math
 import pickle
 from decimal import Decimal
 from textwrap import dedent
 from typing import Optional, List, Tuple
@@ -1125,15 +1126,18 @@
         self.check_selector("count(@min | @max) = 1", root, False)
         self.check_selector("count(@min | @max) = 2", root, True)
 
     def test_sum_function(self):
         root = self.etree.XML(XML_DATA_TEST)
         context = XPathContext(root, variables=self.variables)
         self.check_value("sum($values)", 35, context)
-        self.check_selector("sum(/values/a)", root, 13.299999999999999)
+        if sys.version_info < (3, 12):
+            self.check_selector("sum(/values/a)", root, 13.299999999999999)
+        else:
+            self.check_selector("sum(/values/a)", root, 13.3)
 
         if self.parser.version == '1.0':
             self.check_selector("sum(/values/*)", root, math.isnan)
             self.wrong_syntax("sum(())")
         else:
             self.check_selector("sum(/values/*)", root, TypeError)
             self.check_value("sum(())", 0)
```

### Comparing `elementpath-4.1.1/tests/test_xpath2_constructors.py` & `elementpath-4.1.2/tests/test_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath2_functions.py` & `elementpath-4.1.2/tests/test_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath2_parser.py` & `elementpath-4.1.2/tests/test_xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath30.py` & `elementpath-4.1.2/tests/test_xpath30.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath31.py` & `elementpath-4.1.2/tests/test_xpath31.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath_context.py` & `elementpath-4.1.2/tests/test_xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/test_xpath_nodes.py` & `elementpath-4.1.2/tests/test_xpath_nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,30 @@
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import unittest
 from unittest.mock import patch
+from textwrap import dedent
 import io
 import xml.etree.ElementTree as ElementTree
 
+try:
+    import xmlschema
+except ImportError:
+    xmlschema = None
+else:
+    xmlschema.XMLSchema.meta_schema.build()
+
 from elementpath.etree import is_etree_element, etree_iter_strings, \
     etree_deep_equal, etree_iter_paths
 from elementpath.xpath_nodes import DocumentNode, ElementNode, AttributeNode, TextNode, \
     NamespaceNode, CommentNode, ProcessingInstructionNode
-from elementpath.xpath_context import XPathContext
+from elementpath.xpath_context import XPathContext, XPathSchemaContext
 
 
 class DummyXsdType:
     name = local_name = None
 
     def is_matching(self, name, default_namespace): pass
     def is_empty(self): pass
@@ -345,14 +353,34 @@
         context = XPathContext(doc)
 
         self.assertListEqual(
             list(e.elem for e in context.root.iter() if isinstance(e, ElementNode)),
             list(doc.iter())
         )
 
+    def test_is_schema_node(self):
+        root = ElementTree.XML('<root a="10">text</root>')
+        context = XPathContext(root)
+
+        self.assertFalse(context.root.is_schema_node())
+        self.assertFalse(context.root.attributes[0].is_schema_node())
+        self.assertIsNone(context.root.children[0].is_schema_node())
+
+        if xmlschema is not None:
+            schema = xmlschema.XMLSchema(dedent("""
+                <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+                  <xs:element name="elem"/>
+                  <xs:attribute name="attr" type="xs:string"/>
+                </xs:schema>"""))
+
+            context = XPathSchemaContext(schema)
+            self.assertFalse(context.root.is_schema_node())  # Is the schema
+            self.assertTrue(context.root.attributes[0].is_schema_node())
+            self.assertTrue(context.root.children[0].is_schema_node())
+
     def test_etree_iter_paths(self):
         root = ElementTree.XML('<a><b1><c1/><c2/></b1><b2/><b3><c3/></b3></a>')
         root[2].append(ElementTree.Comment('a comment'))
         root[2].append(ElementTree.Element('c3'))  # duplicated tag
 
         items = list(etree_iter_paths(root))
         self.assertListEqual(items, [
```

### Comparing `elementpath-4.1.1/tests/test_xpath_tokens.py` & `elementpath-4.1.2/tests/test_xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tests/xpath_test_class.py` & `elementpath-4.1.2/tests/xpath_test_class.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.1/tox.ini` & `elementpath-4.1.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 # Tox (http://tox.testrun.org/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
 envlist =
-    py{37,38,39,310,311}, pypy3, xmlschema{20},
-    docs, flake8, mypy-py{38,39,310,311,py3}, pytest, coverage
+    py{37,38,39,310,311,312}, pypy3, xmlschema{20},
+    docs, flake8, mypy-py{38,39,310,311,312,py3}, pytest, coverage
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/elementpath
 
 [testenv]
 deps =
     lxml
+    lxml-stubs
     xmlschema>=2.0.0
     docs: Sphinx
     coverage: coverage
     xmlschema20: xmlschema~=2.0.0
 commands = python -m unittest
-allowlist_externals = make
+
+[testenv:py312]
+deps =
+    lxml-stubs
+    xmlschema>=2.2.3
+    # skip tests that require lxml for now
 
 [testenv:docs]
 commands =
     make -C doc html SPHINXOPTS="-W -n"
     make -C doc latexpdf SPHINXOPTS="-W -n"
     make -C doc doctest SPHINXOPTS="-W -n"
     sphinx-build -W -n -T -b man doc build/sphinx/man
+allowlist_externals = make
 
 [flake8]
 max-line-length = 100
 
 [testenv:flake8]
 deps =
     flake8
 commands =
     flake8 elementpath
     flake8 tests
 
-[testenv:mypy-py{38,39,310,311,py3}]
+[testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
     mypy==1.2.0
     xmlschema
     lxml-stubs
 commands =
     mypy --strict elementpath
     python tests/test_typing.py
@@ -53,14 +60,15 @@
     coverage report -m
 
 [testenv:pytest]
 deps =
     pytest
     pytest-randomly
     lxml
+    lxml-stubs
     xmlschema>=2.0.0
 commands =
     pytest tests -ra
 
 [testenv:build]
 deps =
     setuptools
```

