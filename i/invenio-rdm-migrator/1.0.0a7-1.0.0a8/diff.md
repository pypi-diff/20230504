# Comparing `tmp/invenio-rdm-migrator-1.0.0a7.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a7.tar", last modified: Thu May  4 07:34:53 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a8.tar", last modified: Thu May  4 13:04:10 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a7.tar` & `invenio-rdm-migrator-1.0.0a8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/test_records_table_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/test_records_table_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/test_cache.py
```

### Comparing `invenio-rdm-migrator-1.0.0a7/.editorconfig` & `invenio-rdm-migrator-1.0.0a8/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a8/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/LICENSE` & `invenio-rdm-migrator-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/PKG-INFO` & `invenio-rdm-migrator-1.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a7/README.rst` & `invenio-rdm-migrator-1.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/docs/Makefile` & `invenio-rdm-migrator-1.0.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/docs/conf.py` & `invenio-rdm-migrator-1.0.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/docs/index.rst` & `invenio-rdm-migrator-1.0.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/docs/make.bat` & `invenio-rdm-migrator-1.0.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/ids.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/ids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/postgresql.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/cache.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,38 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Cache module."""
 
+import json
 from abc import ABC, abstractmethod
 
 
 class Cache(ABC):
     """Cache interface."""
 
-    def __init__(self):
+    def __init__(self, filepath=None, validate=False):
         """Constructor."""
         self._data = {}
 
+        if filepath:  # load cache from file
+            with open(filepath, "r") as file:
+                self._data = json.loads(file.read())
+
+            if validate:
+                for _, entry in self._data.items():
+                    self._validate(entry)
+
+    def dump(self, filepath):
+        """Dump cache data into a json file."""
+        with open(filepath, "w") as outfile:
+            outfile.write(json.dumps(self._data))
+
     def get(self, key):
         """Get data from the cache."""
         key = str(key)  # in case they are numbers
         return self._data.get(key, {})
 
     def all(self):
         """Get all the data from the cache."""
```

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/table_generator.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/drafts.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/drafts.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/parents.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/parents.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/records.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/versions.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/runner.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/run-tests.sh` & `invenio-rdm-migrator-1.0.0a8/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/setup.cfg` & `invenio-rdm-migrator-1.0.0a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/files/conftest.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/records/conftest.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/records/test_records_table_generator.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/records/test_records_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

