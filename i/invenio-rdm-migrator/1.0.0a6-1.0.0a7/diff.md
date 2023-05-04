# Comparing `tmp/invenio-rdm-migrator-1.0.0a6.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a6.tar", last modified: Thu Apr 27 15:51:32 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a7.tar", last modified: Thu May  4 07:34:53 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a6.tar` & `invenio-rdm-migrator-1.0.0a7.tar`

### file list

```diff
@@ -1,110 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 07:34:52.000000 invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/records/test_records_table_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:34:53.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 07:34:44.000000 invenio-rdm-migrator-1.0.0a7/tests/streams/test_cache.py
```

### Comparing `invenio-rdm-migrator-1.0.0a6/.editorconfig` & `invenio-rdm-migrator-1.0.0a7/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a7/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/LICENSE` & `invenio-rdm-migrator-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/PKG-INFO` & `invenio-rdm-migrator-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a6/README.rst` & `invenio-rdm-migrator-1.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/docs/Makefile` & `invenio-rdm-migrator-1.0.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/docs/conf.py` & `invenio-rdm-migrator-1.0.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/docs/index.rst` & `invenio-rdm-migrator-1.0.0a7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/docs/make.bat` & `invenio-rdm-migrator-1.0.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/ids.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/ids.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,35 +3,29 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Identifiers generators module."""
 
-import random
 from uuid import uuid4
 
 
 def generate_uuid(data):
     """Generate a UUID."""
     return str(uuid4())
 
 
-# keep track of generated PKs, since there's a chance they collide
-GENERATED_PID_PKS = set()
-
-
 def pid_pk():
-    """Generate a numeric primary key."""
-    while True:
-        # we start at 1M to avoid collisions with existing low-numbered PKs
-        val = random.randint(1_000_000, 2_147_483_647 - 1)
-        if val not in GENERATED_PID_PKS:
-            GENERATED_PID_PKS.add(val)
-            return val
+    """Generate an autoincrementing numeric primary key."""
+    if not hasattr(pid_pk, "value"):
+        pid_pk.value = 1_000_000
+    else:
+        pid_pk.value += 1
+    return pid_pk.value
 
 
 def generate_recid(data, status="R"):
     """Generate a record id object."""
     return {
         "pk": pid_pk(),  # not the pid_value, that comes from rec.json.id in the tg
         "obj_type": "rec",
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/load/postgresql.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 
 import psycopg
 from invenio_records.dictutils import dict_set  # TODO: can we do without?
 
 from .base import Load
 
 
-def _ts(iso=True):
+def _ts(iso=True, fmt=None):
     """Current timestamp string."""
     dt = datetime.now()
+    if fmt:
+        return dt.strftime(fmt)
     return dt.isoformat() if iso else dt.timestamp()
 
 
 def as_csv_row(dc):
     """Serialize a dataclass instance as a CSV-writable row."""
     row = []
     for f in fields(dc):
@@ -47,15 +49,15 @@
 
 class PostgreSQLCopyLoad(Load):
     """PostgreSQL COPY load."""
 
     def __init__(self, db_uri, table_generators, tmp_dir):
         """Constructor."""
         self.db_uri = db_uri
-        self.tmp_dir = Path(tmp_dir) / f"tables{_ts(iso=False)}"
+        self.tmp_dir = Path(tmp_dir) / f"tables-{_ts(fmt='%Y-%m-%dT%H%M%S')}"
         self.table_generators = table_generators
 
     def _cleanup(self, db=False):
         """Cleanup csv files and DB after load."""
         for table in self.table_generators:
             table.cleanup(db=db)
 
@@ -125,14 +127,51 @@
                                 print(f"[{_ts()}] {name}: {progress}")
                             copy.write(block)
                 else:
                     # FIXME: log a WARNING/ERROR
                     print(f"[{_ts()}] {name}: no data to load")
                 conn.commit()
 
+    def _post_load(self):
+        """Post load processing."""
+        tables = set()
+        for tg in self.table_generators:
+            tables = tables.join(set(tg.tables))
+
+        with psycopg.connect(self.db_uri) as conn:
+            sequences = conn.execute(
+                """
+                SELECT
+                    t.oid::regclass AS table_name,
+                    a.attname AS column_name,
+                    s.relname AS sequence_name
+                FROM pg_class AS t
+                    JOIN pg_attribute AS a ON a.attrelid = t.oid
+                    JOIN pg_depend AS d ON d.refobjid = t.oid AND d.refobjsubid = a.attnum
+                    JOIN pg_class AS s ON s.oid = d.objid
+                WHERE
+                    d.classid = 'pg_catalog.pg_class'::regclass
+                    AND d.refclassid = 'pg_catalog.pg_class'::regclass
+                    AND d.deptype IN ('i', 'a')
+                    AND t.relkind IN ('r', 'P')
+                    AND s.relkind = 'S';
+                """
+            )
+
+            for seq in sequences:
+                table_name, column, seq_name = seq
+                if table_name in tables:
+                    max_val = conn.execute(f"SELECT MAX({column}) FROM {table_name}")
+                    max_val = list(max_val)[0][0]  # get actual value from iterator
+                    if max_val:  # if no updates it returns None
+                        conn.execute(
+                            f"ALTER SEQUENCE {seq_name} RESTART WITH {max_val}"
+                        )
+                        # does not require commit as it is a ddl op
+
     def run(self, entries, cleanup=False):
         """Load entries."""
         table_entries = self._prepare(entries)
         self._load(table_entries)
 
         if cleanup:
             self._cleanup()
@@ -147,15 +186,14 @@
         self.pks = pks or []
 
     @abstractmethod
     def _generate_rows(self, **kwargs):
         """Yield generated rows."""
         pass
 
-    @abstractmethod
     def cleanup(self, **kwargs):
         """Cleanup."""
         pass
 
     def _generate_pks(self, data, create=False):
         keys = data.keys()
         for path, pk_func in self.pks:
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/cache.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/cache.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/table_generator.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/table_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,11 +54,7 @@
             member["community_id"] = community_id
             yield CommunityMember(**member)
 
         featured_community = data["featured_community"]
         if featured_community.get("id"):
             featured_community["community_id"] = community_id
             yield FeaturedCommunity(**featured_community)
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,11 +28,7 @@
     def _generate_rows(self, data, **kwargs):
         bucket = data["bucket"]
         object_version = data["object_version"]
         file = data["file"]
         yield FilesInstance(**file)
         yield FilesBucket(**bucket)
         yield FilesObjectVersion(**object_version)
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .table_generators import (
     RDMDraftTableGenerator,
     RDMRecordTableGenerator,
     RDMVersionStateTableGenerator,
 )
 
 
-class RDMRecordCopyLoad(PostgreSQLCopyLoad):  # TODO: abstract SQL from PostgreSQL?
+class RDMRecordCopyLoad(PostgreSQLCopyLoad):
     """PostgreSQL COPY load."""
 
     def __init__(self, cache, db_uri, tmp_dir):
         """Constructor."""
         self.parents_cache = cache.get("parents", ParentsCache())
         self.records_cache = cache.get("records", RecordsCache())
         self.communities_cache = cache.get("communities", {})
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/drafts.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/drafts.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 RDMDraftMetadata,
                 RDMParentMetadata,
                 PersistentIdentifier,
             ],
             pks=[
                 ("draft.id", generate_uuid),
                 ("parent.id", generate_uuid),
-                ("draft.json.pid", partial(generate_recid, status="K")),
+                ("draft.json.pid", partial(generate_recid, status="N")),
                 ("parent.json.pid", generate_recid),
                 ("draft.parent_id", lambda d: d["parent"]["id"]),
             ],
         )
         self.parents_cache = parents_cache
         self.records_cache = records_cache
         self.communities_cache = communities_cache
@@ -47,17 +47,15 @@
         draft = data.get("draft")
         if not draft:
             return
 
         # some legacy records have different pid value in deposit than record
         # however _deposit.pid.value would contain the correct one
         # if it is not legacy we get it from the current field (json.id)
-        recid = (
-            draft.get("_deposit", {}).get("pid", {}).get("value") or draft["json"]["id"]
-        )
+        recid = draft["json"]["id"]
         forked_published = self.records_cache.get(recid)
         cached_parent = self.parents_cache.get(parent["json"]["id"])
         if not cached_parent:
             self.parents_cache.add(
                 parent["json"]["id"],  # recid
                 {
                     "id": parent["id"],
@@ -116,15 +114,15 @@
             )
             # DOI
             if "doi" in draft["json"]["pids"]:
                 yield PersistentIdentifier(
                     id=pid_pk(),
                     pid_type="doi",
                     pid_value=draft["json"]["pids"]["doi"]["identifier"],
-                    status="K",
+                    status="N",
                     object_type="rec",
                     object_uuid=draft["id"],
                     created=now,
                     updated=now,
                 )
 
     # FIXME: deduplicate with records.py
@@ -150,10 +148,9 @@
 
         # resolve parent communities slug
         parent = data["parent"]
         communities = parent["json"].get("communities")
         if communities:
             _resolve_communities(communities)
 
-    def cleanup(self, db, **kwargs):
-        """Cleanup."""
-        pass
+    # FIXME: deduplicate with records.py
+    # assumis records post load alters pidstore_pid_id_seq and pidstore_recid_recid_seq
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/parents.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/parents.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/records.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files 18% similar despite different names*

```diff
@@ -210,49 +210,7 @@
             communities["ids"] = _ids
 
         # resolve parent communities slug
         parent = data["parent"]
         communities = parent["json"].get("communities")
         if communities:
             _resolve_communities(communities)
-
-    def _cleanup_db(self):
-        """Cleanup DB after load."""
-        # FIXME: abstract to tables, can we do without invenio imports
-        # cant fix atm, versions state needs to be deleted in the middle
-        # from invenio_db import db
-        # from invenio_pidstore.models import PersistentIdentifier
-        # from invenio_rdm_records.records.models import (
-        #     RDMDraftMetadata,
-        #     RDMParentMetadata,
-        #     RDMRecordMetadata,
-        #     RDMVersionsState,
-        # )
-        # PersistentIdentifier.query.filter(
-        #     PersistentIdentifier.pid_type.in_(("recid", "doi", "oai")),
-        #     PersistentIdentifier.object_type == "rec",
-        # ).delete()
-        # RDMVersionsState.query.delete()
-        # RDMRecordMetadata.query.delete()
-        # RDMParentMetadata.query.delete()
-        # RDMDraftMetadata.query.delete()
-        # db.session.commit()
-        pass
-
-    def _cleanup_files(self):
-        """Cleanup files after load."""
-        # FIXME: tables does not return the name correct
-        # delegate to table_generators?
-        # for table in self.tables:
-        #     fpath = self.tmp_dir / f"{table._table_name}.csv"
-        #     print(f"Checking {fpath}")
-        #     if fpath.exists():
-        #         print(f"Deleting {fpath}")
-        #         fpath.unlink(missing_ok=True)
-        pass
-
-    def cleanup(self, db, **kwargs):
-        """Cleanup."""
-        self._cleanup_files()
-
-        if db:  # DB cleanup is not always desired
-            self._cleanup_db()
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/versions.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/table_generators/versions.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,11 +33,7 @@
         # overwrite to avoid it using the parent class on a per
         pass
 
     def post_prepare(self, tmp_dir, stack, output_files, **kwargs):
         """Overwrite entries with parent cache entries."""
         for entry in self.parents_cache.all():
             super().prepare(tmp_dir, entry, stack, output_files, **kwargs)
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/records/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,12 +49,7 @@
         community_id = self.communities_cache[request_slug]
 
         data["json"]["receiver"]["community"] = community_id
 
     def prepare(self, tmp_dir, entry, stack, output_files, **kwargs):
         """Compute rows."""
         super().prepare(tmp_dir, entry, stack, output_files, create=True, **kwargs)
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        # TODO
-        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/runner.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,11 +36,7 @@
             )
         identities = data.get("identities", [])
         for identity in identities:
             yield UserIdentity(
                 id_user=user["id"],
                 **identity,
             )
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator/transform/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a7/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,13 @@
 tests/streams/communities/test_communities_load.py
 tests/streams/communities/test_communities_table_generator.py
 tests/streams/communities/test_communities_transform.py
 tests/streams/files/conftest.py
 tests/streams/files/test_files_load.py
 tests/streams/files/test_files_table_generator.py
 tests/streams/files/test_files_transform.py
+tests/streams/records/conftest.py
+tests/streams/records/test_records_table_generator.py
 tests/streams/requests/conftest.py
 tests/streams/requests/test_requests_load.py
 tests/streams/requests/test_requests_table_generator.py
 tests/streams/requests/test_requests_transform.py
```

### Comparing `invenio-rdm-migrator-1.0.0a6/run-tests.sh` & `invenio-rdm-migrator-1.0.0a7/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/setup.cfg` & `invenio-rdm-migrator-1.0.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a7/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,52 +7,66 @@
 
 """Pytest configuration."""
 
 import tempfile
 
 import pytest
 
-from invenio_rdm_migrator.streams.cache import ParentsCache
+from invenio_rdm_migrator.streams.cache import ParentsCache, RecordsCache
 
 
 @pytest.fixture(scope="function")
 def tmp_dir():
     """Yields a temporary directory."""
     tmp_dir = tempfile.TemporaryDirectory()
     yield tmp_dir
     tmp_dir.cleanup()
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture(scope="function")
 def parents_cache():
     """Records parent cache.
 
-    Keys are concept recids and values are UUIDs.
+    Keys are concept recids and values are dictionaries.
     """
     cache = ParentsCache()
     cache.add(
         "123456",
         {
             "id": "1234abcd-1234-5678-abcd-123abc456def",
             "latest_id": "12345678-abcd-1a2b-3c4d-123abc456def",
             "latest_index": 1,
         },
     )
     return cache
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture(scope="function")
+def records_cache():
+    """Records cache.
+
+    Keys are recids and values are dictionaries.
+    """
+    cache = RecordsCache()
+    return cache
+
+
+@pytest.fixture(scope="function")
 def communities_cache():
     """Communities cache.
 
     Keys are community slugs and values are UUIDs.
     """
-    return {"comm": "12345678-abcd-1a2b-3c4d-123abc456def"}
+    return {
+        "comm": "12345678-abcd-1a2b-3c4d-123abc456def",
+        "other-comm": "12345678-abcd-1a2b-3c4d-123abc123abc",
+    }
 
 
-@pytest.fixture(scope="module")
-def cache(parents_cache, communities_cache):
+@pytest.fixture(scope="function")
+def cache(parents_cache, records_cache, communities_cache):
     """Global cache containing the other ones."""
     return {
         "parents": parents_cache,
+        "records": records_cache,
         "communities": communities_cache,
     }
```

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/files/conftest.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a6/tests/streams/test_cache.py` & `invenio-rdm-migrator-1.0.0a7/tests/streams/test_cache.py`

 * *Files identical despite different names*

