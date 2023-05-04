# Comparing `tmp/fastavro-1.7.3.tar.gz` & `tmp/fastavro-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastavro-1.7.3.tar", last modified: Wed Mar  8 23:06:12 2023, max compression
+gzip compressed data, was "fastavro-1.7.4.tar", last modified: Thu May  4 15:54:08 2023, max compression
```

## Comparing `fastavro-1.7.3.tar` & `fastavro-1.7.4.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.670410 fastavro-1.7.3/
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.7.3/.azure_upload.sh
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.7.3/.flake8.cython
--rw-r--r--   0 sbelden    (501) staff       (20)    26083 2023-03-08 20:56:35.000000 fastavro-1.7.3/ChangeLog
--rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.7.3/Dockerfile
--rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.7.3/LICENSE
--rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.7.3/MANIFEST.in
--rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.7.3/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.7.3/NOTICE.txt
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-03-08 23:06:12.670529 fastavro-1.7.3/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     3870 2022-10-26 14:14:35.000000 fastavro-1.7.3/README.md
--rw-r--r--   0 sbelden    (501) staff       (20)      528 2022-08-11 13:05:27.000000 fastavro-1.7.3/developer_requirements.txt
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.577328 fastavro-1.7.3/docs/
--rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.7.3/docs/command_line_script.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/conf.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/index.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.578468 fastavro-1.7.3/docs/io/
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/io/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/io/json_decoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/io/json_encoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.7.3/docs/json_reader.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.7.3/docs/json_writer.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/logical_types.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.7.3/docs/reader.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.579310 fastavro-1.7.3/docs/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/repository/base.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/repository/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.7.3/docs/schema.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.7.3/docs/utils.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.7.3/docs/validation.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.7.3/docs/writer.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.611955 fastavro-1.7.3/fastavro/
--rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-03-08 20:56:39.000000 fastavro-1.7.3/fastavro/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.7.3/fastavro/__main__.py
--rw-r--r--   0 sbelden    (501) staff       (20)   262056 2023-03-08 23:06:08.000000 fastavro-1.7.3/fastavro/_logical_readers.c
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_logical_readers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_logical_readers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_logical_readers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_logical_readers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)   430913 2023-03-08 23:06:09.000000 fastavro-1.7.3/fastavro/_logical_writers.c
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.3/fastavro/_logical_writers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.7.3/fastavro/_logical_writers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.7.3/fastavro/_logical_writers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.3/fastavro/_logical_writers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)  1109567 2023-03-08 23:06:09.000000 fastavro-1.7.3/fastavro/_read.c
--rw-r--r--   0 sbelden    (501) staff       (20)     1827 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_read.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    35286 2023-02-22 18:29:22.000000 fastavro-1.7.3/fastavro/_read.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      703 2021-05-14 16:27:52.000000 fastavro-1.7.3/fastavro/_read_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    35776 2023-02-22 18:29:22.000000 fastavro-1.7.3/fastavro/_read_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   703036 2023-03-08 23:06:09.000000 fastavro-1.7.3/fastavro/_schema.c
--rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.7.3/fastavro/_schema.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    24094 2023-02-22 18:29:22.000000 fastavro-1.7.3/fastavro/_schema.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.7.3/fastavro/_schema_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33002 2023-02-22 18:29:22.000000 fastavro-1.7.3/fastavro/_schema_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.7.3/fastavro/_six.c
--rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/_validate_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)   390961 2023-03-08 23:06:10.000000 fastavro-1.7.3/fastavro/_validation.c
--rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.7.3/fastavro/_validation.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.7.3/fastavro/_validation.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.7.3/fastavro/_validation_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)  1717084 2023-03-08 23:06:11.000000 fastavro-1.7.3/fastavro/_write.c
--rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.7.3/fastavro/_write.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-02-14 22:23:08.000000 fastavro-1.7.3/fastavro/_write.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      619 2020-08-23 17:48:32.000000 fastavro-1.7.3/fastavro/_write_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-02-14 22:23:08.000000 fastavro-1.7.3/fastavro/_write_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/const.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.617459 fastavro-1.7.3/fastavro/io/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.7.3/fastavro/io/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4319 2022-10-06 12:45:36.000000 fastavro-1.7.3/fastavro/io/binary_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/io/binary_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     6904 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/io/json_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/io/json_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.7.3/fastavro/io/parser.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.7.3/fastavro/io/symbols.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1109 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/json_read.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.7.3/fastavro/json_write.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/logical_readers.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.7.3/fastavro/logical_writers.py
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.7.3/fastavro/py.typed
--rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/read.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.619554 fastavro-1.7.3/fastavro/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/repository/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/repository/base.py
--rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/repository/flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.7.3/fastavro/types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.7.3/fastavro/utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.7.3/fastavro/validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.7.3/fastavro/write.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.614530 fastavro-1.7.3/fastavro.egg-info/
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/SOURCES.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/dependency_links.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/entry_points.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/not-zip-safe
--rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/requires.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-03-08 23:06:12.000000 fastavro-1.7.3/fastavro.egg-info/top_level.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.3/mypy.ini
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1930 2023-03-08 23:04:55.000000 fastavro-1.7.3/publish.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      204 2023-03-08 20:55:48.000000 fastavro-1.7.3/pyproject.toml
--rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.7.3/pytest.ini
--rw-r--r--   0 sbelden    (501) staff       (20)      710 2022-09-20 17:48:57.000000 fastavro-1.7.3/run-tests.cmd
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1050 2023-02-22 18:29:28.000000 fastavro-1.7.3/run-tests.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-03-08 23:06:12.671054 fastavro-1.7.3/setup.cfg
--rw-r--r--   0 sbelden    (501) staff       (20)     2796 2022-10-26 14:14:35.000000 fastavro-1.7.3/setup.py
--rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.7.3/tag.sh
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.634721 fastavro-1.7.3/tests/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/__init__.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.652431 fastavro-1.7.3/tests/avro-files/
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/Child.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/Child1.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/Parent.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/ParentMissingChild.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/a_triple_pair.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/bool.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/double_float.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/error-type.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/java-generated-uuid.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/lines.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/m.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/no-fields.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/part-00000.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/recursive.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/request.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/response.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-0.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-1-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-1.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-3-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-6-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-deflate-9.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-null-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test-snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/test.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/testDataFileMeta.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/avro-files/weather-legacy-generated.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/avro-files/weather-legacy-with-names.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/weather-snappy.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/weather-sorted.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.7.3/tests/avro-files/weather.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.7.3/tests/conftest.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.653846 fastavro-1.7.3/tests/load_schema_test/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.655430 fastavro-1.7.3/tests/load_schema_test_10/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_10/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_10/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_10/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_10/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.657199 fastavro-1.7.3/tests/load_schema_test_11/
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_11/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_11/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_11/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_11/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_11/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.657464 fastavro-1.7.3/tests/load_schema_test_12/
--rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_12/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.657999 fastavro-1.7.3/tests/load_schema_test_12/com/
--rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_12/com/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_12/com/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.658647 fastavro-1.7.3/tests/load_schema_test_12/com/namespace/
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_12/com/namespace/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_12/com/namespace/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.659469 fastavro-1.7.3/tests/load_schema_test_13/
--rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_13/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_13/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.659925 fastavro-1.7.3/tests/load_schema_test_14/
--rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_14/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.660768 fastavro-1.7.3/tests/load_schema_test_15/
--rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_15/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_15/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.3/tests/load_schema_test_15/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.661428 fastavro-1.7.3/tests/load_schema_test_16/
--rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/load_schema_test_16/namespace.match.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/load_schema_test_16/namespace.team.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.662392 fastavro-1.7.3/tests/load_schema_test_2/
--rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test_2/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test_2/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.3/tests/load_schema_test_2/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.663638 fastavro-1.7.3/tests/load_schema_test_3/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_3/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_3/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_3/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.664819 fastavro-1.7.3/tests/load_schema_test_4/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_4/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_4/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_4/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.665712 fastavro-1.7.3/tests/load_schema_test_5/
--rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_5/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_5/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.666550 fastavro-1.7.3/tests/load_schema_test_6/
--rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_6/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/load_schema_test_6/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.667273 fastavro-1.7.3/tests/load_schema_test_7/
--rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_7/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_7/namespace.B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.668280 fastavro-1.7.3/tests/load_schema_test_8/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_8/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_8/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_8/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.669189 fastavro-1.7.3/tests/load_schema_test_9/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_9/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_9/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.3/tests/load_schema_test_9/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.669484 fastavro-1.7.3/tests/repository/
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-03-08 23:06:12.670163 fastavro-1.7.3/tests/repository/flat_dict_test/
--rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/repository/flat_dict_test/InvalidJson.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/repository/flat_dict_test/Valid.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/repository/test_flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.7.3/tests/test_aliases.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/test_appendable.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.7.3/tests/test_block_reader.py
--rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.7.3/tests/test_canonical_form.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_complex.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.7.3/tests/test_compression.py
--rw-r--r--   0 sbelden    (501) staff       (20)    98991 2023-02-22 18:29:22.000000 fastavro-1.7.3/tests/test_fastavro.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.7.3/tests/test_fingerprint.py
--rw-r--r--   0 sbelden    (501) staff       (20)    26782 2022-09-09 20:03:51.000000 fastavro-1.7.3/tests/test_json.py
--rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.7.3/tests/test_logical_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_main_cli.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_promotion.py
--rw-r--r--   0 sbelden    (501) staff       (20)    39721 2022-12-29 14:56:38.000000 fastavro-1.7.3/tests/test_schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.7.3/tests/test_schema_evolution.py
--rw-r--r--   0 sbelden    (501) staff       (20)     8069 2022-09-09 20:03:51.000000 fastavro-1.7.3/tests/test_schemaless.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.7.3/tests/test_str_py3.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_timezone.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.7.3/tests/test_utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.7.3/tests/test_validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.7.3/tests/test_write_block.py
--rw-r--r--   0 sbelden    (501) staff       (20)      253 2022-10-26 15:21:05.000000 fastavro-1.7.3/tox.ini
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.976793 fastavro-1.7.4/
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.7.4/.azure_upload.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.7.4/.flake8.cython
+-rw-r--r--   0 sbelden    (501) staff       (20)    26245 2023-05-04 14:38:48.000000 fastavro-1.7.4/ChangeLog
+-rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.7.4/Dockerfile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.7.4/LICENSE
+-rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.7.4/MANIFEST.in
+-rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.7.4/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.7.4/NOTICE.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-05-04 15:54:08.976914 fastavro-1.7.4/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     3870 2022-10-26 14:14:35.000000 fastavro-1.7.4/README.md
+-rw-r--r--   0 sbelden    (501) staff       (20)      520 2023-05-04 13:14:43.000000 fastavro-1.7.4/developer_requirements.txt
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.867907 fastavro-1.7.4/docs/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.7.4/docs/command_line_script.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/conf.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/index.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.868853 fastavro-1.7.4/docs/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/json_decoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/io/json_encoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.7.4/docs/json_reader.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.7.4/docs/json_writer.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/logical_types.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.7.4/docs/reader.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.869470 fastavro-1.7.4/docs/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/repository/base.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/repository/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.7.4/docs/schema.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.7.4/docs/utils.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.7.4/docs/validation.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.7.4/docs/writer.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.907334 fastavro-1.7.4/fastavro/
+-rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-05-04 14:38:56.000000 fastavro-1.7.4/fastavro/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/__main__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   262056 2023-05-04 15:54:04.000000 fastavro-1.7.4/fastavro/_logical_readers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_logical_readers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)   430913 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_logical_writers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/_logical_writers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.7.4/fastavro/_logical_writers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.7.4/fastavro/_logical_writers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/_logical_writers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)  1109567 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_read.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     1827 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_read.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    35286 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      703 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    35776 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_read_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   704359 2023-05-04 15:54:05.000000 fastavro-1.7.4/fastavro/_schema.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.7.4/fastavro/_schema.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    24103 2023-05-04 14:35:44.000000 fastavro-1.7.4/fastavro/_schema.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.7.4/fastavro/_schema_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33011 2023-05-04 14:35:44.000000 fastavro-1.7.4/fastavro/_schema_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.7.4/fastavro/_six.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/_validate_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   390961 2023-05-04 15:54:06.000000 fastavro-1.7.4/fastavro/_validation.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.7.4/fastavro/_validation.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_validation.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_validation_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)  1717084 2023-05-04 15:54:07.000000 fastavro-1.7.4/fastavro/_write.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/_write.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_write.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      619 2023-05-03 19:57:13.000000 fastavro-1.7.4/fastavro/_write_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-04-17 20:07:08.000000 fastavro-1.7.4/fastavro/_write_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/const.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.913799 fastavro-1.7.4/fastavro/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.7.4/fastavro/io/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4319 2022-10-06 12:45:36.000000 fastavro-1.7.4/fastavro/io/binary_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/binary_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     6904 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/json_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/io/json_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.7.4/fastavro/io/parser.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.7.4/fastavro/io/symbols.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1603 2023-03-16 19:48:58.000000 fastavro-1.7.4/fastavro/json_read.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.7.4/fastavro/json_write.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/logical_readers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/logical_writers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.7.4/fastavro/py.typed
+-rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/read.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.915607 fastavro-1.7.4/fastavro/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/base.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/repository/flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.7.4/fastavro/types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.7.4/fastavro/utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.7.4/fastavro/validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.7.4/fastavro/write.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.910355 fastavro-1.7.4/fastavro.egg-info/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/SOURCES.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/dependency_links.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/entry_points.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-03-16 16:53:53.000000 fastavro-1.7.4/fastavro.egg-info/not-zip-safe
+-rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/requires.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-05-04 15:54:08.000000 fastavro-1.7.4/fastavro.egg-info/top_level.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2023-04-17 20:07:08.000000 fastavro-1.7.4/mypy.ini
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1930 2023-03-16 18:04:24.000000 fastavro-1.7.4/publish.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      204 2023-03-08 20:55:48.000000 fastavro-1.7.4/pyproject.toml
+-rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.7.4/pytest.ini
+-rw-r--r--   0 sbelden    (501) staff       (20)      710 2022-09-20 17:48:57.000000 fastavro-1.7.4/run-tests.cmd
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1050 2023-05-04 13:44:25.000000 fastavro-1.7.4/run-tests.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-05-04 15:54:08.977634 fastavro-1.7.4/setup.cfg
+-rw-r--r--   0 sbelden    (501) staff       (20)     2796 2022-10-26 14:14:35.000000 fastavro-1.7.4/setup.py
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.7.4/tag.sh
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.934647 fastavro-1.7.4/tests/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/__init__.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.956336 fastavro-1.7.4/tests/avro-files/
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Child.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Child1.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/Parent.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/ParentMissingChild.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/a_triple_pair.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/bool.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/double_float.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/error-type.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/java-generated-uuid.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/lines.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/m.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/no-fields.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/part-00000.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/recursive.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/request.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/response.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-0.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-1-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-1.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-3-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-6-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-deflate-9.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-null-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test-snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/test.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/testDataFileMeta.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/avro-files/weather-legacy-generated.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/avro-files/weather-legacy-with-names.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather-snappy.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather-sorted.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.7.4/tests/avro-files/weather.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/conftest.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.958155 fastavro-1.7.4/tests/load_schema_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.960082 fastavro-1.7.4/tests/load_schema_test_10/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_10/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.961957 fastavro-1.7.4/tests/load_schema_test_11/
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_11/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.962265 fastavro-1.7.4/tests/load_schema_test_12/
+-rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.963016 fastavro-1.7.4/tests/load_schema_test_12/com/
+-rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.963704 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_12/com/namespace/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.964621 fastavro-1.7.4/tests/load_schema_test_13/
+-rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_13/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_13/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.965146 fastavro-1.7.4/tests/load_schema_test_14/
+-rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_14/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.966331 fastavro-1.7.4/tests/load_schema_test_15/
+-rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.7.4/tests/load_schema_test_15/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.967059 fastavro-1.7.4/tests/load_schema_test_16/
+-rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/load_schema_test_16/namespace.match.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/load_schema_test_16/namespace.team.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.968178 fastavro-1.7.4/tests/load_schema_test_2/
+-rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.7.4/tests/load_schema_test_2/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.969608 fastavro-1.7.4/tests/load_schema_test_3/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_3/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.970744 fastavro-1.7.4/tests/load_schema_test_4/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_4/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.971558 fastavro-1.7.4/tests/load_schema_test_5/
+-rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_5/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_5/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.972277 fastavro-1.7.4/tests/load_schema_test_6/
+-rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_6/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/load_schema_test_6/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.973160 fastavro-1.7.4/tests/load_schema_test_7/
+-rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_7/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_7/namespace.B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.974183 fastavro-1.7.4/tests/load_schema_test_8/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_8/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.975313 fastavro-1.7.4/tests/load_schema_test_9/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.7.4/tests/load_schema_test_9/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.975685 fastavro-1.7.4/tests/repository/
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-05-04 15:54:08.976436 fastavro-1.7.4/tests/repository/flat_dict_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/flat_dict_test/InvalidJson.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/flat_dict_test/Valid.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/repository/test_flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/test_aliases.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/test_appendable.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.7.4/tests/test_block_reader.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.7.4/tests/test_canonical_form.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_complex.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.7.4/tests/test_compression.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    98991 2023-04-17 20:07:08.000000 fastavro-1.7.4/tests/test_fastavro.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.7.4/tests/test_fingerprint.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    27587 2023-03-16 19:48:58.000000 fastavro-1.7.4/tests/test_json.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.7.4/tests/test_logical_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_main_cli.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_promotion.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    40285 2023-05-04 14:35:44.000000 fastavro-1.7.4/tests/test_schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.7.4/tests/test_schema_evolution.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     8069 2022-09-09 20:03:51.000000 fastavro-1.7.4/tests/test_schemaless.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.7.4/tests/test_str_py3.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_timezone.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.7.4/tests/test_utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.7.4/tests/test_validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.7.4/tests/test_write_block.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      253 2022-10-26 15:21:05.000000 fastavro-1.7.4/tox.ini
```

### Comparing `fastavro-1.7.3/.azure_upload.sh` & `fastavro-1.7.4/.azure_upload.sh`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/ChangeLog` & `fastavro-1.7.4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-05-04 version 1.7.4
+* Fix parsing of namespaces (@scottbelden in PR #692)
+* Be able to specify a reader schema in the json_reader (@scottbelden in PR #681)
+
 2023-03-08 version 1.7.3
 * Create musllinux wheels (@scottbelden in PR #679)
 
 2023-02-22 version 1.7.2
 * Allow default value errors when a reader schema is supplied (@scottbelden in PR #677)
 * Allow values like NaN for default values of float and double types (@scottbelden in PR #675)
```

### Comparing `fastavro-1.7.3/LICENSE` & `fastavro-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/MANIFEST.in` & `fastavro-1.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/Makefile` & `fastavro-1.7.4/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/NOTICE.txt` & `fastavro-1.7.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/PKG-INFO` & `fastavro-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.7.3
+Version: 1.7.4
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fastavro-1.7.3/README.md` & `fastavro-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/developer_requirements.txt` & `fastavro-1.7.4/developer_requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 check-manifest
 Cython
 numpy # used in tests
 pandas; platform_python_implementation!='PyPy' # used in tests; not install on pypy as it takes forever
 wheel
 twine
 coverage
-codecov
 mypy; implementation_name != "pypy"
 black; implementation_name != "pypy"
 
 # codec libraries (snappy is intentionally left off this list as it requires other system libraries to be installed and is non-trivial)
 # Also don't install on windows for similar reasons
 zstandard; sys_platform != 'win32'
 lz4; sys_platform != 'win32'
```

### Comparing `fastavro-1.7.3/docs/Makefile` & `fastavro-1.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/docs/command_line_script.rst` & `fastavro-1.7.4/docs/command_line_script.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/docs/conf.py` & `fastavro-1.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/docs/index.rst` & `fastavro-1.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/docs/logical_types.rst` & `fastavro-1.7.4/docs/logical_types.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/docs/writer.rst` & `fastavro-1.7.4/docs/writer.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/__init__.py` & `fastavro-1.7.4/fastavro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         {u'station': u'012650-99999', u'temp': 111, u'time': 1433275478},
     ]
 
     with open('weather.avro', 'wb') as out:
         writer(out, schema, records)
 """
 
-__version_info__ = (1, 7, 3)
+__version_info__ = (1, 7, 4)
 __version__ = "%s.%s.%s" % __version_info__
 
 
 import fastavro.read
 import fastavro.write
 import fastavro.schema
 import fastavro.validation
```

### Comparing `fastavro-1.7.3/fastavro/__main__.py` & `fastavro-1.7.4/fastavro/__main__.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_readers.c` & `fastavro-1.7.4/fastavro/_logical_readers.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_readers.pyx` & `fastavro-1.7.4/fastavro/_logical_readers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_readers_py.py` & `fastavro-1.7.4/fastavro/_logical_readers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_writers.c` & `fastavro-1.7.4/fastavro/_logical_writers.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_writers.pyx` & `fastavro-1.7.4/fastavro/_logical_writers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_logical_writers_py.py` & `fastavro-1.7.4/fastavro/_logical_writers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_read.c` & `fastavro-1.7.4/fastavro/_read.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_read.pyi` & `fastavro-1.7.4/fastavro/_read.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_read.pyx` & `fastavro-1.7.4/fastavro/_read.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_read_common.py` & `fastavro-1.7.4/fastavro/_read_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_read_py.py` & `fastavro-1.7.4/fastavro/_read_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_schema.c` & `fastavro-1.7.4/fastavro/_schema.c`

 * *Files 0% similar despite different names*

```diff
@@ -1593,25 +1593,25 @@
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_[] = "-";
 static const char __pyx_k_h[] = "h";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k__2[] = "";
 static const char __pyx_k__3[] = ".";
-static const char __pyx_k__6[] = "[";
-static const char __pyx_k__7[] = ",";
-static const char __pyx_k__8[] = "]";
-static const char __pyx_k__9[] = "\"";
+static const char __pyx_k__7[] = "[";
+static const char __pyx_k__8[] = ",";
+static const char __pyx_k__9[] = "]";
 static const char __pyx_k_fo[] = "fo";
 static const char __pyx_k_io[] = "io";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_re[] = "re";
-static const char __pyx_k__10[] = "}";
-static const char __pyx_k__11[] = "]}";
-static const char __pyx_k__12[] = ". ";
+static const char __pyx_k__10[] = "\"";
+static const char __pyx_k__11[] = "}";
+static const char __pyx_k__12[] = "]}";
+static const char __pyx_k__13[] = ". ";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_doc[] = "doc";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_map[] = "map";
@@ -1651,14 +1651,15 @@
 static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_fields[] = "fields";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "{\"name\":\"";
 static const char __pyx_k_name_3[] = "__name__";
 static const char __pyx_k_object[] = "object";
 static const char __pyx_k_record[] = "record";
+static const char __pyx_k_rsplit[] = "rsplit";
 static const char __pyx_k_schema[] = "schema";
 static const char __pyx_k_size_2[] = "\",\"size\":";
 static const char __pyx_k_string[] = "string";
 static const char __pyx_k_symbol[] = "symbol";
 static const char __pyx_k_type_2[] = "{\"type\":\"";
 static const char __pyx_k_type_3[] = "\",\"type\":\"";
 static const char __pyx_k_type_4[] = "\",\"type\":";
@@ -1776,17 +1777,17 @@
 static PyObject *__pyx_n_s_UnknownType;
 static PyObject *__pyx_kp_u_Unknown_schema_fingerprint_algor;
 static PyObject *__pyx_kp_u_Valid_values_include;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_u__10;
 static PyObject *__pyx_kp_u__11;
 static PyObject *__pyx_kp_u__12;
+static PyObject *__pyx_kp_u__13;
 static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_kp_u__3;
-static PyObject *__pyx_kp_u__6;
 static PyObject *__pyx_kp_u__7;
 static PyObject *__pyx_kp_u__8;
 static PyObject *__pyx_kp_u__9;
 static PyObject *__pyx_n_s_add;
 static PyObject *__pyx_n_s_algorithm;
 static PyObject *__pyx_n_u_aliases;
 static PyObject *__pyx_kp_u_aliases_must_be_a_list_not;
@@ -1876,14 +1877,15 @@
 static PyObject *__pyx_n_u_precision;
 static PyObject *__pyx_n_s_rabin_fingerprint;
 static PyObject *__pyx_n_s_re;
 static PyObject *__pyx_n_u_record;
 static PyObject *__pyx_kp_u_redefined_named_type;
 static PyObject *__pyx_n_s_repo;
 static PyObject *__pyx_n_s_repository;
+static PyObject *__pyx_n_s_rsplit;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_u_scale;
 static PyObject *__pyx_n_s_schema;
 static PyObject *__pyx_n_s_schema_common;
 static PyObject *__pyx_n_s_schema_name;
 static PyObject *__pyx_n_s_schema_path;
 static PyObject *__pyx_kp_u_schema_type;
@@ -1926,29 +1928,30 @@
 static PyObject *__pyx_pf_8fastavro_7_schema_20fingerprint(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_parsing_canonical_form, PyObject *__pyx_v_algorithm); /* proto */
 static PyObject *__pyx_pf_8fastavro_7_schema_22_validate_enum_symbols(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_schema); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, &__pyx_n_s_get, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_8;
 static PyObject *__pyx_int_neg_1;
-static PyObject *__pyx_slice__5;
+static PyObject *__pyx_slice__6;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
 /* Late includes */
 
 /* "fastavro/_schema.pyx":31
  * 
  * 
  * cpdef inline is_nullable_union(schema):             # <<<<<<<<<<<<<<
  *     count = 0
@@ -2802,16 +2805,16 @@
     __pyx_L8_try_end:;
   }
 
   /* "fastavro/_schema.pyx":74
  *         )
  * 
  *     namespace = schema.get("namespace", parent_ns)             # <<<<<<<<<<<<<<
- *     if not namespace:
- *         return namespace, name
+ *     if "." in name:
+ *         return name.rsplit(".", 1)[0], name
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
@@ -2858,135 +2861,142 @@
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_namespace = __pyx_t_7;
   __pyx_t_7 = 0;
 
   /* "fastavro/_schema.pyx":75
  * 
  *     namespace = schema.get("namespace", parent_ns)
- *     if not namespace:             # <<<<<<<<<<<<<<
- *         return namespace, name
- *     elif "." in name:
+ *     if "." in name:             # <<<<<<<<<<<<<<
+ *         return name.rsplit(".", 1)[0], name
+ *     elif namespace:
  */
-  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_v_namespace); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_13 = ((!__pyx_t_12) != 0);
+  __pyx_t_12 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__3, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_13 = (__pyx_t_12 != 0);
   if (__pyx_t_13) {
 
     /* "fastavro/_schema.pyx":76
  *     namespace = schema.get("namespace", parent_ns)
- *     if not namespace:
- *         return namespace, name             # <<<<<<<<<<<<<<
- *     elif "." in name:
- *         return "", name
+ *     if "." in name:
+ *         return name.rsplit(".", 1)[0], name             # <<<<<<<<<<<<<<
+ *     elif namespace:
+ *         return namespace, f"{namespace}.{name}"
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_INCREF(__pyx_v_namespace);
-    __Pyx_GIVEREF(__pyx_v_namespace);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_namespace);
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
     __Pyx_INCREF(__pyx_v_name);
     __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_name);
-    __pyx_r = __pyx_t_7;
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_name);
     __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
     goto __pyx_L0;
 
     /* "fastavro/_schema.pyx":75
  * 
  *     namespace = schema.get("namespace", parent_ns)
- *     if not namespace:             # <<<<<<<<<<<<<<
- *         return namespace, name
- *     elif "." in name:
+ *     if "." in name:             # <<<<<<<<<<<<<<
+ *         return name.rsplit(".", 1)[0], name
+ *     elif namespace:
  */
   }
 
   /* "fastavro/_schema.pyx":77
- *     if not namespace:
- *         return namespace, name
- *     elif "." in name:             # <<<<<<<<<<<<<<
- *         return "", name
+ *     if "." in name:
+ *         return name.rsplit(".", 1)[0], name
+ *     elif namespace:             # <<<<<<<<<<<<<<
+ *         return namespace, f"{namespace}.{name}"
  *     else:
  */
-  __pyx_t_13 = (__Pyx_PySequence_ContainsTF(__pyx_kp_u__3, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __pyx_t_12 = (__pyx_t_13 != 0);
-  if (__pyx_t_12) {
+  __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_v_namespace); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (__pyx_t_13) {
 
     /* "fastavro/_schema.pyx":78
- *         return namespace, name
- *     elif "." in name:
- *         return "", name             # <<<<<<<<<<<<<<
+ *         return name.rsplit(".", 1)[0], name
+ *     elif namespace:
+ *         return namespace, f"{namespace}.{name}"             # <<<<<<<<<<<<<<
  *     else:
- *         return namespace, f"{namespace}.{name}"
+ *         return "", name
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_14 = 0;
+    __pyx_t_15 = 127;
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_namespace, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_INCREF(__pyx_kp_u__2);
-    __Pyx_GIVEREF(__pyx_kp_u__2);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_u__2);
-    __Pyx_INCREF(__pyx_v_name);
-    __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_name);
-    __pyx_r = __pyx_t_7;
+    __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_15;
+    __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __Pyx_INCREF(__pyx_kp_u__3);
+    __pyx_t_14 += 1;
+    __Pyx_GIVEREF(__pyx_kp_u__3);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_kp_u__3);
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_15;
+    __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_7);
     __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_6, 3, __pyx_t_14, __pyx_t_15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_INCREF(__pyx_v_namespace);
+    __Pyx_GIVEREF(__pyx_v_namespace);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_namespace);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_6;
+    __pyx_t_6 = 0;
     goto __pyx_L0;
 
     /* "fastavro/_schema.pyx":77
- *     if not namespace:
- *         return namespace, name
- *     elif "." in name:             # <<<<<<<<<<<<<<
- *         return "", name
+ *     if "." in name:
+ *         return name.rsplit(".", 1)[0], name
+ *     elif namespace:             # <<<<<<<<<<<<<<
+ *         return namespace, f"{namespace}.{name}"
  *     else:
  */
   }
 
   /* "fastavro/_schema.pyx":80
- *         return "", name
+ *         return namespace, f"{namespace}.{name}"
  *     else:
- *         return namespace, f"{namespace}.{name}"             # <<<<<<<<<<<<<<
+ *         return "", name             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_14 = 0;
-    __pyx_t_15 = 127;
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_namespace, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_15;
-    __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __Pyx_INCREF(__pyx_kp_u__3);
-    __pyx_t_14 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__3);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_kp_u__3);
-    __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_15 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_15) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_15;
-    __pyx_t_14 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_7, 3, __pyx_t_14, __pyx_t_15); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_INCREF(__pyx_v_namespace);
-    __Pyx_GIVEREF(__pyx_v_namespace);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_namespace);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6);
+    __Pyx_INCREF(__pyx_kp_u__2);
+    __Pyx_GIVEREF(__pyx_kp_u__2);
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u__2);
+    __Pyx_INCREF(__pyx_v_name);
+    __Pyx_GIVEREF(__pyx_v_name);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_name);
+    __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
     goto __pyx_L0;
   }
 
   /* "fastavro/_schema.pyx":66
  * 
  * 
  * cpdef schema_name(schema, parent_ns):             # <<<<<<<<<<<<<<
@@ -9913,15 +9923,15 @@
  * 
  *         else:
  *             raise Exception(             # <<<<<<<<<<<<<<
  *                 "Internal error; "
  *                 + "You should raise an issue in the fastavro github repository"
  */
     /*else*/ {
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 619, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(0, 619, __pyx_L1_error)
     }
   }
 
@@ -10231,15 +10241,15 @@
   /* "fastavro/_schema.pyx":636
  *         loaded_schemas.append(schema)
  * 
  *     top_first_order = loaded_schemas[::-1]             # <<<<<<<<<<<<<<
  *     outer_schema = top_first_order.pop(0)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_loaded_schemas, __pyx_slice__5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_loaded_schemas, __pyx_slice__6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_top_first_order = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "fastavro/_schema.pyx":637
  * 
  *     top_first_order = loaded_schemas[::-1]
@@ -10534,15 +10544,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__6);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__7);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 655, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "fastavro/_schema.pyx":656
@@ -10631,15 +10641,15 @@
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_8, function);
           }
         }
-        __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_kp_u__7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__7);
+        __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_kp_u__8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__8);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 658, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
         /* "fastavro/_schema.pyx":657
@@ -10688,15 +10698,15 @@
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__8);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__9) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__9);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "fastavro/_schema.pyx":654
@@ -10729,29 +10739,29 @@
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_write); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = 0;
     __pyx_t_10 = 127;
-    __Pyx_INCREF(__pyx_kp_u__9);
+    __Pyx_INCREF(__pyx_kp_u__10);
     __pyx_t_6 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__9);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u__9);
+    __Pyx_GIVEREF(__pyx_kp_u__10);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u__10);
     __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_schema, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_10;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
     __pyx_t_8 = 0;
-    __Pyx_INCREF(__pyx_kp_u__9);
+    __Pyx_INCREF(__pyx_kp_u__10);
     __pyx_t_6 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__9);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__9);
+    __Pyx_GIVEREF(__pyx_kp_u__10);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u__10);
     __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_5, 3, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -10880,15 +10890,15 @@
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
-      __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__10) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__10);
+      __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__11);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 673, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "fastavro/_schema.pyx":670
@@ -10989,15 +10999,15 @@
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_kp_u__10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__10);
+      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__11);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 678, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
       /* "fastavro/_schema.pyx":675
@@ -11181,15 +11191,15 @@
             if (likely(__pyx_t_9)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
               __Pyx_INCREF(__pyx_t_9);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_8, function);
             }
           }
-          __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_kp_u__7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__7);
+          __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_kp_u__8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__8);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 686, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
           /* "fastavro/_schema.pyx":685
@@ -11210,29 +11220,29 @@
  */
         __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_write); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 687, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 687, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_11 = 0;
         __pyx_t_10 = 127;
-        __Pyx_INCREF(__pyx_kp_u__9);
+        __Pyx_INCREF(__pyx_kp_u__10);
         __pyx_t_11 += 1;
-        __Pyx_GIVEREF(__pyx_kp_u__9);
-        PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_kp_u__9);
+        __Pyx_GIVEREF(__pyx_kp_u__10);
+        PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_kp_u__10);
         __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_v_symbol, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 687, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_12) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_12) : __pyx_t_10;
         __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_12);
         PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_12);
         __pyx_t_12 = 0;
-        __Pyx_INCREF(__pyx_kp_u__9);
+        __Pyx_INCREF(__pyx_kp_u__10);
         __pyx_t_11 += 1;
-        __Pyx_GIVEREF(__pyx_kp_u__9);
-        PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_kp_u__9);
+        __Pyx_GIVEREF(__pyx_kp_u__10);
+        PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_kp_u__10);
         __pyx_t_12 = __Pyx_PyUnicode_Join(__pyx_t_9, 3, __pyx_t_11, __pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 687, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __pyx_t_9 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
@@ -11276,15 +11286,15 @@
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
-      __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__11);
+      __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_kp_u__12) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__12);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 688, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
       /* "fastavro/_schema.pyx":680
@@ -11373,18 +11383,18 @@
       __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_size, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 693, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_10;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_4, 5, __pyx_t_8);
       __pyx_t_8 = 0;
-      __Pyx_INCREF(__pyx_kp_u__10);
+      __Pyx_INCREF(__pyx_kp_u__11);
       __pyx_t_6 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u__10);
-      PyTuple_SET_ITEM(__pyx_t_4, 6, __pyx_kp_u__10);
+      __Pyx_GIVEREF(__pyx_kp_u__11);
+      PyTuple_SET_ITEM(__pyx_t_4, 6, __pyx_kp_u__11);
       __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_4, 7, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 693, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_4)) {
@@ -11580,15 +11590,15 @@
             if (likely(__pyx_t_12)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
               __Pyx_INCREF(__pyx_t_12);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_8, function);
             }
           }
-          __pyx_t_5 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_12, __pyx_kp_u__7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__7);
+          __pyx_t_5 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_12, __pyx_kp_u__8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u__8);
           __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
           if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 701, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
           /* "fastavro/_schema.pyx":700
@@ -11690,15 +11700,15 @@
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_5, function);
           }
         }
-        __pyx_t_8 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_kp_u__10) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__10);
+        __pyx_t_8 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u__11);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 705, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
         /* "fastavro/_schema.pyx":699
@@ -11727,15 +11737,15 @@
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_kp_u__11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__11);
+      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_kp_u__12) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__12);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 706, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
       /* "fastavro/_schema.pyx":695
@@ -11771,29 +11781,29 @@
  */
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_fo, __pyx_n_s_write); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 709, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 709, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_6 = 0;
       __pyx_t_10 = 127;
-      __Pyx_INCREF(__pyx_kp_u__9);
+      __Pyx_INCREF(__pyx_kp_u__10);
       __pyx_t_6 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u__9);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u__9);
+      __Pyx_GIVEREF(__pyx_kp_u__10);
+      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u__10);
       __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_schema_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 709, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_10;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_5);
       __pyx_t_5 = 0;
-      __Pyx_INCREF(__pyx_kp_u__9);
+      __Pyx_INCREF(__pyx_kp_u__10);
       __pyx_t_6 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u__9);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u__9);
+      __Pyx_GIVEREF(__pyx_kp_u__10);
+      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u__10);
       __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_8, 3, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 709, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_8)) {
@@ -11981,18 +11991,18 @@
     __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_algorithm, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 715, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_6) : __pyx_t_5;
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
     __pyx_t_6 = 0;
-    __Pyx_INCREF(__pyx_kp_u__12);
+    __Pyx_INCREF(__pyx_kp_u__13);
     __pyx_t_4 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__12);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__12);
+    __Pyx_GIVEREF(__pyx_kp_u__13);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__13);
     __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 715, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "fastavro/_schema.pyx":716
  *         raise ValueError(
  *             f"Unknown schema fingerprint algorithm {algorithm}. "
@@ -12741,17 +12751,17 @@
   {&__pyx_n_s_UnknownType, __pyx_k_UnknownType, sizeof(__pyx_k_UnknownType), 0, 0, 1, 1},
   {&__pyx_kp_u_Unknown_schema_fingerprint_algor, __pyx_k_Unknown_schema_fingerprint_algor, sizeof(__pyx_k_Unknown_schema_fingerprint_algor), 0, 1, 0, 0},
   {&__pyx_kp_u_Valid_values_include, __pyx_k_Valid_values_include, sizeof(__pyx_k_Valid_values_include), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
   {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
   {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+  {&__pyx_kp_u__13, __pyx_k__13, sizeof(__pyx_k__13), 0, 1, 0, 0},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
   {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
   {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
   {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
   {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
   {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
   {&__pyx_n_u_aliases, __pyx_k_aliases, sizeof(__pyx_k_aliases), 0, 1, 0, 1},
   {&__pyx_kp_u_aliases_must_be_a_list_not, __pyx_k_aliases_must_be_a_list_not, sizeof(__pyx_k_aliases_must_be_a_list_not), 0, 1, 0, 0},
@@ -12841,14 +12851,15 @@
   {&__pyx_n_u_precision, __pyx_k_precision, sizeof(__pyx_k_precision), 0, 1, 0, 1},
   {&__pyx_n_s_rabin_fingerprint, __pyx_k_rabin_fingerprint, sizeof(__pyx_k_rabin_fingerprint), 0, 0, 1, 1},
   {&__pyx_n_s_re, __pyx_k_re, sizeof(__pyx_k_re), 0, 0, 1, 1},
   {&__pyx_n_u_record, __pyx_k_record, sizeof(__pyx_k_record), 0, 1, 0, 1},
   {&__pyx_kp_u_redefined_named_type, __pyx_k_redefined_named_type, sizeof(__pyx_k_redefined_named_type), 0, 1, 0, 0},
   {&__pyx_n_s_repo, __pyx_k_repo, sizeof(__pyx_k_repo), 0, 0, 1, 1},
   {&__pyx_n_s_repository, __pyx_k_repository, sizeof(__pyx_k_repository), 0, 0, 1, 1},
+  {&__pyx_n_s_rsplit, __pyx_k_rsplit, sizeof(__pyx_k_rsplit), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_u_scale, __pyx_k_scale, sizeof(__pyx_k_scale), 0, 1, 0, 1},
   {&__pyx_n_s_schema, __pyx_k_schema, sizeof(__pyx_k_schema), 0, 0, 1, 1},
   {&__pyx_n_s_schema_common, __pyx_k_schema_common, sizeof(__pyx_k_schema_common), 0, 0, 1, 1},
   {&__pyx_n_s_schema_name, __pyx_k_schema_name, sizeof(__pyx_k_schema_name), 0, 0, 1, 1},
   {&__pyx_n_s_schema_path, __pyx_k_schema_path, sizeof(__pyx_k_schema_path), 0, 0, 1, 1},
   {&__pyx_kp_u_schema_type, __pyx_k_schema_type, sizeof(__pyx_k_schema_type), 0, 1, 0, 0},
@@ -12890,118 +12901,129 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "fastavro/_schema.pyx":76
+ *     namespace = schema.get("namespace", parent_ns)
+ *     if "." in name:
+ *         return name.rsplit(".", 1)[0], name             # <<<<<<<<<<<<<<
+ *     elif namespace:
+ *         return namespace, f"{namespace}.{name}"
+ */
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_kp_u__3, __pyx_int_1); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
   /* "fastavro/_schema.pyx":619
  * 
  *         else:
  *             raise Exception(             # <<<<<<<<<<<<<<
  *                 "Internal error; "
  *                 + "You should raise an issue in the fastavro github repository"
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Internal_error_You_should_raise); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 619, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Internal_error_You_should_raise); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "fastavro/_schema.pyx":636
  *         loaded_schemas.append(schema)
  * 
  *     top_first_order = loaded_schemas[::-1]             # <<<<<<<<<<<<<<
  *     outer_schema = top_first_order.pop(0)
  * 
  */
-  __pyx_slice__5 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__5)) __PYX_ERR(0, 636, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__5);
-  __Pyx_GIVEREF(__pyx_slice__5);
+  __pyx_slice__6 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__6)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__6);
+  __Pyx_GIVEREF(__pyx_slice__6);
 
   /* "fastavro/_schema.pyx":27
  * )
  * 
  * SYMBOL_REGEX = re.compile(r"[A-Za-z_][A-Za-z0-9_]*")             # <<<<<<<<<<<<<<
  * NO_DEFAULT = object()
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_A_Za_z__A_Za_z0_9); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_A_Za_z__A_Za_z0_9); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "fastavro/_schema.pyx":87
  * 
  * 
  * def parse_schema(             # <<<<<<<<<<<<<<
  *     schema,
  *     named_schemas=None,
  */
-  __pyx_tuple__14 = PyTuple_Pack(9, __pyx_n_s_schema, __pyx_n_s_named_schemas, __pyx_n_s_expand, __pyx_n_s_write_hint, __pyx_n_s_force, __pyx_n_s_ignore_default_error, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_s); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 4, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_parse_schema, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_schema, __pyx_n_s_named_schemas, __pyx_n_s_expand, __pyx_n_s_write_hint, __pyx_n_s_force, __pyx_n_s_ignore_default_error, __pyx_n_s_key, __pyx_n_s_value, __pyx_n_s_s); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 4, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_parse_schema, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 87, __pyx_L1_error)
 
   /* "fastavro/_schema.pyx":463
  * 
  * 
  * def load_schema(             # <<<<<<<<<<<<<<
  *     schema_path,
  *     *,
  */
-  __pyx_tuple__16 = PyTuple_Pack(9, __pyx_n_s_schema_path, __pyx_n_s_repo, __pyx_n_s_named_schemas, __pyx_n_s_write_hint, __pyx_n_s_injected_schemas, __pyx_n_s_schema_name, __pyx_n_s_file_dir, __pyx_n_s_file_name, __pyx_n_s_file_ext); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 463, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 4, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_load_schema, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(9, __pyx_n_s_schema_path, __pyx_n_s_repo, __pyx_n_s_named_schemas, __pyx_n_s_write_hint, __pyx_n_s_injected_schemas, __pyx_n_s_schema_name, __pyx_n_s_file_dir, __pyx_n_s_file_name, __pyx_n_s_file_ext); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 4, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_load_schema, 463, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 463, __pyx_L1_error)
 
   /* "fastavro/_schema.pyx":625
  * 
  * 
  * def load_schema_ordered(ordered_schemas, *, _write_hint=True):             # <<<<<<<<<<<<<<
  *     loaded_schemas = []
  *     named_schemas = {}
  */
-  __pyx_tuple__18 = PyTuple_Pack(11, __pyx_n_s_ordered_schemas, __pyx_n_s_write_hint, __pyx_n_s_loaded_schemas, __pyx_n_s_named_schemas, __pyx_n_s_idx, __pyx_n_s_schema_path, __pyx_n_s_last, __pyx_n_s_schema, __pyx_n_s_top_first_order, __pyx_n_s_outer_schema, __pyx_n_s_sub_schema); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 625, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_load_schema_ordered, 625, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(11, __pyx_n_s_ordered_schemas, __pyx_n_s_write_hint, __pyx_n_s_loaded_schemas, __pyx_n_s_named_schemas, __pyx_n_s_idx, __pyx_n_s_schema_path, __pyx_n_s_last, __pyx_n_s_schema, __pyx_n_s_top_first_order, __pyx_n_s_outer_schema, __pyx_n_s_sub_schema); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 1, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_load_schema_ordered, 625, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 625, __pyx_L1_error)
 
   /* "fastavro/_schema.pyx":646
  * 
  * 
  * def to_parsing_canonical_form(schema):             # <<<<<<<<<<<<<<
  *     fo = StringIO()
  *     _to_parsing_canonical_form(parse_schema(schema), fo)
  */
-  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_schema, __pyx_n_s_fo); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 646, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_to_parsing_canonical_form, 646, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_schema, __pyx_n_s_fo); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_to_parsing_canonical_form, 646, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 646, __pyx_L1_error)
 
   /* "fastavro/_schema.pyx":712
  * 
  * 
  * def fingerprint(parsing_canonical_form, algorithm):             # <<<<<<<<<<<<<<
  *     if algorithm not in FINGERPRINT_ALGORITHMS:
  *         raise ValueError(
  */
-  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_parsing_canonical_form, __pyx_n_s_algorithm, __pyx_n_s_h); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 712, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_fingerprint, 712, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(3, __pyx_n_s_parsing_canonical_form, __pyx_n_s_algorithm, __pyx_n_s_h); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_fingerprint, 712, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 712, __pyx_L1_error)
 
   /* "fastavro/_schema.pyx":729
  * 
  * 
  * def _validate_enum_symbols(schema):             # <<<<<<<<<<<<<<
  *     symbols = schema["symbols"]
  *     for symbol in symbols:
  */
-  __pyx_tuple__24 = PyTuple_Pack(3, __pyx_n_s_schema, __pyx_n_s_symbols, __pyx_n_s_symbol); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 729, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_validate_enum_symbols, 729, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 729, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_schema, __pyx_n_s_symbols, __pyx_n_s_symbol); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 729, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastavro__schema_pyx, __pyx_n_s_validate_enum_symbols, 729, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -13530,15 +13552,15 @@
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_re); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_SYMBOL_REGEX, __pyx_t_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "fastavro/_schema.pyx":28
  *
```

### Comparing `fastavro-1.7.3/fastavro/_schema.pyi` & `fastavro-1.7.4/fastavro/_schema.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_schema.pyx` & `fastavro-1.7.4/fastavro/_schema.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -68,20 +68,20 @@
         name = schema["name"]
     except KeyError:
         raise SchemaParseException(
             f'"name" is a required field missing from the schema: {schema}'
         )
 
     namespace = schema.get("namespace", parent_ns)
-    if not namespace:
-        return namespace, name
-    elif "." in name:
-        return "", name
-    else:
+    if "." in name:
+        return name.rsplit(".", 1)[0], name
+    elif namespace:
         return namespace, f"{namespace}.{name}"
+    else:
+        return "", name
 
 
 cpdef expand_schema(schema):
     return parse_schema(schema, expand=True, _write_hint=False)
 
 
 def parse_schema(
```

### Comparing `fastavro-1.7.3/fastavro/_schema_common.py` & `fastavro-1.7.4/fastavro/_schema_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_schema_py.py` & `fastavro-1.7.4/fastavro/_schema_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,20 +99,20 @@
         name = schema["name"]
     except KeyError:
         raise SchemaParseException(
             f'"name" is a required field missing from the schema: {schema}'
         )
 
     namespace = schema.get("namespace", parent_ns)
-    if not namespace:
-        return namespace, name
-    elif "." in name:
-        return "", name
-    else:
+    if "." in name:
+        return name.rsplit(".", 1)[0], name
+    elif namespace:
         return namespace, f"{namespace}.{name}"
+    else:
+        return "", name
 
 
 def expand_schema(schema: Schema) -> Schema:
     """Returns a schema where all named types are expanded to their real schema
 
     NOTE: The output of this function produces a schema that can include
     multiple definitions of the same named type (as per design) which are not
```

### Comparing `fastavro-1.7.3/fastavro/_six.c` & `fastavro-1.7.4/fastavro/_six.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_validate_common.py` & `fastavro-1.7.4/fastavro/_validate_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_validation.c` & `fastavro-1.7.4/fastavro/_validation.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_validation.pyx` & `fastavro-1.7.4/fastavro/_validation.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_validation_py.py` & `fastavro-1.7.4/fastavro/_validation_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_write.c` & `fastavro-1.7.4/fastavro/_write.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_write.pyi` & `fastavro-1.7.4/fastavro/_write.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_write.pyx` & `fastavro-1.7.4/fastavro/_write.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_write_common.py` & `fastavro-1.7.4/fastavro/_write_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/_write_py.py` & `fastavro-1.7.4/fastavro/_write_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/const.py` & `fastavro-1.7.4/fastavro/const.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/binary_decoder.py` & `fastavro-1.7.4/fastavro/io/binary_decoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/binary_encoder.py` & `fastavro-1.7.4/fastavro/io/binary_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/json_decoder.py` & `fastavro-1.7.4/fastavro/io/json_decoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/json_encoder.py` & `fastavro-1.7.4/fastavro/io/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/parser.py` & `fastavro-1.7.4/fastavro/io/parser.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/io/symbols.py` & `fastavro-1.7.4/fastavro/io/symbols.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/json_write.py` & `fastavro-1.7.4/fastavro/json_write.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/read.py` & `fastavro-1.7.4/fastavro/read.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/repository/flat_dict.py` & `fastavro-1.7.4/fastavro/repository/flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/schema.py` & `fastavro-1.7.4/fastavro/schema.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro/utils.py` & `fastavro-1.7.4/fastavro/utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/fastavro.egg-info/PKG-INFO` & `fastavro-1.7.4/fastavro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.7.3
+Version: 1.7.4
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fastavro-1.7.3/fastavro.egg-info/SOURCES.txt` & `fastavro-1.7.4/fastavro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/publish.sh` & `fastavro-1.7.4/publish.sh`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/run-tests.cmd` & `fastavro-1.7.4/run-tests.cmd`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/run-tests.sh` & `fastavro-1.7.4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/setup.py` & `fastavro-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/deflate.avro` & `fastavro-1.7.4/tests/avro-files/deflate.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/java-generated-uuid.avro` & `fastavro-1.7.4/tests/avro-files/java-generated-uuid.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/null.avro` & `fastavro-1.7.4/tests/avro-files/null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/snappy.avro` & `fastavro-1.7.4/tests/avro-files/snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-0.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-0.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-1-A.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-1-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-1.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-1.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-3-A.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-3-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-6-B.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-6-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-deflate-9.avro` & `fastavro-1.7.4/tests/avro-files/test-deflate-9.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-null-B.avro` & `fastavro-1.7.4/tests/avro-files/test-null-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-null.avro` & `fastavro-1.7.4/tests/avro-files/test-null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/test-snappy.avro` & `fastavro-1.7.4/tests/avro-files/test-snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/weather-legacy-generated.avro` & `fastavro-1.7.4/tests/avro-files/weather-legacy-generated.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/avro-files/weather-legacy-with-names.avro` & `fastavro-1.7.4/tests/avro-files/weather-legacy-with-names.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/conftest.py` & `fastavro-1.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/repository/test_flat_dict.py` & `fastavro-1.7.4/tests/repository/test_flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_aliases.py` & `fastavro-1.7.4/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_appendable.py` & `fastavro-1.7.4/tests/test_appendable.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_block_reader.py` & `fastavro-1.7.4/tests/test_block_reader.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_canonical_form.py` & `fastavro-1.7.4/tests/test_canonical_form.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_complex.py` & `fastavro-1.7.4/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_compression.py` & `fastavro-1.7.4/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_fastavro.py` & `fastavro-1.7.4/tests/test_fastavro.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_fingerprint.py` & `fastavro-1.7.4/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_json.py` & `fastavro-1.7.4/tests/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from fastavro.schema import parse_schema
 from fastavro.validation import ValidationError
 from fastavro.io.json_decoder import AvroJSONDecoder
 from fastavro.io.json_encoder import AvroJSONEncoder
 from fastavro.io.symbols import MapKeyMarker, String
 
 
-def roundtrip(schema, records, *, writer_kwargs={}):
+def roundtrip(schema, records, *, reader_schema=None, writer_kwargs={}):
     new_file = StringIO()
     json_writer(new_file, schema, records, **writer_kwargs)
     new_file.seek(0)
 
-    new_records = list(json_reader(new_file, schema))
+    reader = json_reader(new_file, schema, reader_schema)
+
+    new_records = list(reader)
     return new_records
 
 
 def test_json():
     schema = {
         "type": "record",
         "name": "Test",
@@ -870,7 +872,33 @@
         "fields": [{"name": "some_field", "type": "string", "default": "test"}],
     }
 
     test_record = {"eggs": "eggs"}
 
     with pytest.raises(ValueError, match="record contains more fields .*? eggs"):
         roundtrip(schema, [test_record], writer_kwargs={"strict_allow_default": True})
+
+
+def test_json_aliases():
+    """https://github.com/fastavro/fastavro/issues/669"""
+    schema = {
+        "name": "test_json_aliases",
+        "type": "record",
+        "fields": [
+            {"name": "field_1", "type": "string"},
+            {"name": "field_2", "type": "long"},
+        ],
+    }
+
+    reader_schema = {
+        "name": "test_json_aliases",
+        "type": "record",
+        "fields": [
+            {"name": "new_field_1", "type": "string", "aliases": ["field_1"]},
+            {"name": "field_2", "type": "long"},
+        ],
+    }
+
+    records = [{"field_1": "foo", "field_2": 10}]
+
+    output_records = roundtrip(schema, records, reader_schema=reader_schema)
+    assert output_records == [{"new_field_1": "foo", "field_2": 10}]
```

### Comparing `fastavro-1.7.3/tests/test_logical_types.py` & `fastavro-1.7.4/tests/test_logical_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_main_cli.py` & `fastavro-1.7.4/tests/test_main_cli.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_promotion.py` & `fastavro-1.7.4/tests/test_promotion.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_schema.py` & `fastavro-1.7.4/tests/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1330,7 +1330,28 @@
                 "type": field_type,
                 "default": default_value,
             }
         ],
     }
 
     fastavro.parse_schema(schema)
+
+
+def test_namespace_respected():
+    """https://github.com/fastavro/fastavro/issues/690"""
+    schema = {
+        "type": "record",
+        "name": "explicit_namespace.foo",
+        "fields": [
+            {
+                "name": "field1",
+                "type": {
+                    "type": "record",
+                    "name": "bar",
+                    "fields": [{"name": "bar_field", "type": "int"}],
+                },
+            },
+            {"name": "field2", "type": "explicit_namespace.bar"},
+        ],
+    }
+
+    fastavro.parse_schema(schema)
```

### Comparing `fastavro-1.7.3/tests/test_schema_evolution.py` & `fastavro-1.7.4/tests/test_schema_evolution.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_schemaless.py` & `fastavro-1.7.4/tests/test_schemaless.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_str_py3.py` & `fastavro-1.7.4/tests/test_str_py3.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_timezone.py` & `fastavro-1.7.4/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_types.py` & `fastavro-1.7.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_utils.py` & `fastavro-1.7.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_validation.py` & `fastavro-1.7.4/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.7.3/tests/test_write_block.py` & `fastavro-1.7.4/tests/test_write_block.py`

 * *Files identical despite different names*

