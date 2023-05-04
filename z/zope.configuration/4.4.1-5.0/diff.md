# Comparing `tmp/zope.configuration-4.4.1.tar.gz` & `tmp/zope.configuration-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.configuration-4.4.1.tar", last modified: Thu Apr  7 06:28:23 2022, max compression
+gzip compressed data, was "zope.configuration-5.0.tar", last modified: Thu May  4 06:17:21 2023, max compression
```

## Comparing `zope.configuration-4.4.1.tar` & `zope.configuration-5.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.706361 zope.configuration-4.4.1/
--rw-r--r--   0 mac        (513) staff       (20)     8270 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      400 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    10704 2022-04-07 06:28:23.706489 zope.configuration-4.4.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1045 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      194 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.684133 zope.configuration-4.4.1/docs/
--rw-r--r--   0 mac        (513) staff       (20)     5608 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/Makefile
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.686725 zope.configuration-4.4.1/docs/api/
--rw-r--r--   0 mac        (513) staff       (20)      126 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/config.rst
--rw-r--r--   0 mac        (513) staff       (20)      134 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/docutils.rst
--rw-r--r--   0 mac        (513) staff       (20)      142 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/exceptions.rst
--rw-r--r--   0 mac        (513) staff       (20)      126 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/fields.rst
--rw-r--r--   0 mac        (513) staff       (20)      156 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/interfaces.rst
--rw-r--r--   0 mac        (513) staff       (20)      118 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/name.rst
--rw-r--r--   0 mac        (513) staff       (20)      138 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/xmlconfig.rst
--rw-r--r--   0 mac        (513) staff       (20)      154 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api/zopeconfigure.rst
--rw-r--r--   0 mac        (513) staff       (20)      242 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)     8429 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     9273 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)      242 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5118 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)    39621 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/docs/narr.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      296 2022-04-07 06:28:23.706994 zope.configuration-4.4.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3368 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.676299 zope.configuration-4.4.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.687054 zope.configuration-4.4.1/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.693152 zope.configuration-4.4.1/src/zope/configuration/
--rw-r--r--   0 mac        (513) staff       (20)      845 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2295 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)    64311 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/config.py
--rw-r--r--   0 mac        (513) staff       (20)     2995 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/docutils.py
--rw-r--r--   0 mac        (513) staff       (20)     2343 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/exceptions.py
--rw-r--r--   0 mac        (513) staff       (20)    17845 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/fields.py
--rw-r--r--   0 mac        (513) staff       (20)     5134 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     2722 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/name.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.699888 zope.configuration-4.4.1/src/zope/configuration/tests/
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       74 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/bad.py
--rw-r--r--   0 mac        (513) staff       (20)     1171 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/conditions.py
--rw-r--r--   0 mac        (513) staff       (20)     2036 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/conditions.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2330 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/directives.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.700842 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/
--rw-r--r--   0 mac        (513) staff       (20)        2 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       83 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)       14 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/spam.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.701475 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/sub/
--rw-r--r--   0 mac        (513) staff       (20)        2 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/sub/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       14 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/excludedemo/sub/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     4120 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/nested.py
--rw-r--r--   0 mac        (513) staff       (20)       38 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/notyet.py
--rw-r--r--   0 mac        (513) staff       (20)      291 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/sample.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.705780 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/
--rw-r--r--   0 mac        (513) staff       (20)      102 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/NamedForClass.py
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       92 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/bar.zcml
--rw-r--r--   0 mac        (513) staff       (20)      132 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/bar1.zcml
--rw-r--r--   0 mac        (513) staff       (20)      153 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/bar2.zcml
--rw-r--r--   0 mac        (513) staff       (20)      120 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/bar21.zcml
--rw-r--r--   0 mac        (513) staff       (20)      101 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/baro.zcml
--rw-r--r--   0 mac        (513) staff       (20)      100 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/baro2.zcml
--rw-r--r--   0 mac        (513) staff       (20)      412 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/baz1.zcml
--rw-r--r--   0 mac        (513) staff       (20)      159 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/baz2.zcml
--rw-r--r--   0 mac        (513) staff       (20)      159 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/baz3.zcml
--rw-r--r--   0 mac        (513) staff       (20)      443 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)       65 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/configure.zcml.in
--rw-r--r--   0 mac        (513) staff       (20)     1323 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/foo.py
--rw-r--r--   0 mac        (513) staff       (20)      442 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/foo.zcml.in
--rw-r--r--   0 mac        (513) staff       (20)     1560 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/schema.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1646 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/simple.py
--rw-r--r--   0 mac        (513) staff       (20)      883 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/simple.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1126 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test___init__.py
--rw-r--r--   0 mac        (513) staff       (20)    75577 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_config.py
--rw-r--r--   0 mac        (513) staff       (20)     3302 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_docs.py
--rw-r--r--   0 mac        (513) staff       (20)     4776 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_docutils.py
--rw-r--r--   0 mac        (513) staff       (20)    11233 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_fields.py
--rw-r--r--   0 mac        (513) staff       (20)     4511 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_name.py
--rw-r--r--   0 mac        (513) staff       (20)    47753 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_xmlconfig.py
--rw-r--r--   0 mac        (513) staff       (20)     1339 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/test_zopeconfigure.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.706142 zope.configuration-4.4.1/src/zope/configuration/tests/unicode_all/
--rw-r--r--   0 mac        (513) staff       (20)       77 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/unicode_all/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      112 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/tests/victim.py
--rw-r--r--   0 mac        (513) staff       (20)    23156 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/xmlconfig.py
--rw-r--r--   0 mac        (513) staff       (20)     6250 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/src/zope/configuration/zopeconfigure.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-07 06:28:23.689610 zope.configuration-4.4.1/src/zope.configuration.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    10704 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     3099 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      168 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-04-07 06:28:23.000000 zope.configuration-4.4.1/src/zope.configuration.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1655 2022-04-07 06:28:21.000000 zope.configuration-4.4.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.037047 zope.configuration-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     8380 2023-05-04 06:17:20.000000 zope.configuration-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-04 06:17:20.000000 zope.configuration-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-04 06:17:20.000000 zope.configuration-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-04 06:17:20.000000 zope.configuration-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      400 2023-05-04 06:17:20.000000 zope.configuration-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    10668 2023-05-04 06:17:21.037183 zope.configuration-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1045 2023-05-04 06:17:20.000000 zope.configuration-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      194 2023-05-04 06:17:20.000000 zope.configuration-5.0/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.017195 zope.configuration-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5608 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/Makefile
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.019522 zope.configuration-5.0/docs/api/
+-rw-r--r--   0 mac        (513) staff       (20)      126 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/config.rst
+-rw-r--r--   0 mac        (513) staff       (20)      134 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/docutils.rst
+-rw-r--r--   0 mac        (513) staff       (20)      142 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/exceptions.rst
+-rw-r--r--   0 mac        (513) staff       (20)      126 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/fields.rst
+-rw-r--r--   0 mac        (513) staff       (20)      156 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/interfaces.rst
+-rw-r--r--   0 mac        (513) staff       (20)      118 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/name.rst
+-rw-r--r--   0 mac        (513) staff       (20)      138 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/xmlconfig.rst
+-rw-r--r--   0 mac        (513) staff       (20)      154 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api/zopeconfigure.rst
+-rw-r--r--   0 mac        (513) staff       (20)      242 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)     8390 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     9273 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/hacking.rst
+-rw-r--r--   0 mac        (513) staff       (20)      242 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5118 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)    39590 2023-05-04 06:17:20.000000 zope.configuration-5.0/docs/narr.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-05-04 06:17:20.000000 zope.configuration-5.0/rtd.txt
+-rw-r--r--   0 mac        (513) staff       (20)      569 2023-05-04 06:17:21.037865 zope.configuration-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3281 2023-05-04 06:17:20.000000 zope.configuration-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.010961 zope.configuration-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.019796 zope.configuration-5.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.024798 zope.configuration-5.0/src/zope/configuration/
+-rw-r--r--   0 mac        (513) staff       (20)      845 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1461 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)    63632 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/config.py
+-rw-r--r--   0 mac        (513) staff       (20)     2996 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/docutils.py
+-rw-r--r--   0 mac        (513) staff       (20)     2265 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/exceptions.py
+-rw-r--r--   0 mac        (513) staff       (20)    17724 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/fields.py
+-rw-r--r--   0 mac        (513) staff       (20)     5133 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     2723 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/name.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.030724 zope.configuration-5.0/src/zope/configuration/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       61 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       74 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/bad.py
+-rw-r--r--   0 mac        (513) staff       (20)     1169 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/conditions.py
+-rw-r--r--   0 mac        (513) staff       (20)     2036 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/conditions.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     2311 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/directives.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.031587 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/
+-rw-r--r--   0 mac        (513) staff       (20)        2 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       83 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)       14 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/spam.zcml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.032162 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/sub/
+-rw-r--r--   0 mac        (513) staff       (20)        2 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/sub/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       14 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/excludedemo/sub/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     4100 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/nested.py
+-rw-r--r--   0 mac        (513) staff       (20)       38 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/notyet.py
+-rw-r--r--   0 mac        (513) staff       (20)      291 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/sample.zcml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.036515 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/
+-rw-r--r--   0 mac        (513) staff       (20)       94 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/NamedForClass.py
+-rw-r--r--   0 mac        (513) staff       (20)       61 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       92 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/bar.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      132 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/bar1.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      153 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/bar2.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      120 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/bar21.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      101 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/baro.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      100 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/baro2.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      412 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/baz1.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      159 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/baz2.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      159 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/baz3.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      443 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)       65 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/configure.zcml.in
+-rw-r--r--   0 mac        (513) staff       (20)     1317 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/foo.py
+-rw-r--r--   0 mac        (513) staff       (20)      442 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/samplepackage/foo.zcml.in
+-rw-r--r--   0 mac        (513) staff       (20)     1560 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/schema.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1633 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/simple.py
+-rw-r--r--   0 mac        (513) staff       (20)      883 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/simple.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1126 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test___init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    75452 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_config.py
+-rw-r--r--   0 mac        (513) staff       (20)     2853 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_docs.py
+-rw-r--r--   0 mac        (513) staff       (20)     4760 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_docutils.py
+-rw-r--r--   0 mac        (513) staff       (20)    11161 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_fields.py
+-rw-r--r--   0 mac        (513) staff       (20)     4512 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_name.py
+-rw-r--r--   0 mac        (513) staff       (20)    47704 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_xmlconfig.py
+-rw-r--r--   0 mac        (513) staff       (20)     1332 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/test_zopeconfigure.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.036799 zope.configuration-5.0/src/zope/configuration/tests/unicode_all/
+-rw-r--r--   0 mac        (513) staff       (20)       36 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/unicode_all/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       73 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/tests/victim.py
+-rw-r--r--   0 mac        (513) staff       (20)    23025 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/xmlconfig.py
+-rw-r--r--   0 mac        (513) staff       (20)     6222 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope/configuration/zopeconfigure.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-04 06:17:21.021859 zope.configuration-5.0/src/zope.configuration.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    10668 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     3099 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      168 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-04 06:17:20.000000 zope.configuration-5.0/src/zope.configuration.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1832 2023-05-04 06:17:20.000000 zope.configuration-5.0/tox.ini
```

### Comparing `zope.configuration-4.4.1/CHANGES.rst` & `zope.configuration-5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+5.0 (2023-05-04)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4.1 (2022-04-07)
 ------------------
 
 - Avoid creating reference cycles through tracebacks in ``reraise`` (change
   imported from ``six``).
 
 - Add support for Python 3.9, 3.10.
```

### Comparing `zope.configuration-4.4.1/CONTRIBUTING.md` & `zope.configuration-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/LICENSE.txt` & `zope.configuration-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/PKG-INFO` & `zope.configuration-5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.configuration
-Version: 4.4.1
+Version: 5.0
 Summary: Zope Configuration Markup Language (ZCML)
 Home-page: https://github.com/zopefoundation/zope.configuration
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope configuration zcml
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ``zope.configuration``
 ======================
 
@@ -58,14 +55,22 @@
 
 
 
 
 Changes
 =======
 
+5.0 (2023-05-04)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4.1 (2022-04-07)
 ------------------
 
 - Avoid creating reference cycles through tracebacks in ``reraise`` (change
   imported from ``six``).
 
 - Add support for Python 3.9, 3.10.
@@ -325,9 +330,7 @@
 
 Before 3.4.0
 ------------
 
 This package was part of the Zope 3 distribution and did not have its own
 CHANGES.txt. For earlier changes please refer to either our subversion log or
 the CHANGES.txt of earlier Zope 3 releases.
-
-
```

### Comparing `zope.configuration-4.4.1/README.rst` & `zope.configuration-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/docs/Makefile` & `zope.configuration-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/docs/conf.py` & `zope.configuration-5.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,15 @@
 
 # If false, no module index is generated.
 #texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
-intersphinx_mapping = {
-    'https://docs.python.org/': None,
-    'https://zopeschema.readthedocs.io/en/latest': None,
-}
+# intersphinx_mapping = {
+#     'python': ('https://docs.python.org/', None),
+# }
 
 autodoc_default_flags = [
     'members',
     'show-inheritance',
 ]
```

### Comparing `zope.configuration-4.4.1/docs/hacking.rst` & `zope.configuration-5.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/docs/make.bat` & `zope.configuration-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/docs/narr.rst` & `zope.configuration-5.0/docs/narr.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1165,15 +1165,14 @@
    >>> from zope.configuration.exceptions import ConfigurationError
    >>> v = string(
    ...      '<text xmlns="http://sample.namespaces.zope.org/schema" name="x" />',
    ...      context)
    Traceback (most recent call last):
    ...
    zope.configuration.exceptions.ConfigurationError: The directive ('http://sample.namespaces.zope.org/schema', 'text') cannot be used in this context
-     File "<string>", line 1.0
 
 
 Let's see what happens if we declare duplicate fields:
 
 .. doctest::
 
    >>> try:
```

### Comparing `zope.configuration-4.4.1/setup.py` & `zope.configuration-5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -33,50 +35,49 @@
     # in DottedName that allows underscores.
     'zope.schema >= 4.9.0',
     'zope.testing',
     'zope.testrunner',
 ]
 
 setup(name='zope.configuration',
-      version='4.4.1',
+      version='5.0',
       author='Zope Foundation and Contributors',
-      author_email='zope-dev@zope.org',
+      author_email='zope-dev@zope.dev',
       description='Zope Configuration Markup Language (ZCML)',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
       ),
       keywords="zope configuration zcml",
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
-          "Programming Language :: Python :: 2",
-          'Programming Language :: Python :: 2.7',
-          "Programming Language :: Python :: 3",
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
-          'Framework :: Zope :: 3'],
+          'Framework :: Zope :: 3',
+      ],
       url='https://github.com/zopefoundation/zope.configuration',
       license='ZPL 2.1',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['zope'],
+      python_requires='>=3.7',
       extras_require={
           'docs': ['Sphinx', 'repoze.sphinx.autointerface'],
           'test': TESTS_REQUIRE,
       },
       install_requires=[
           'setuptools',
           'zope.i18nmessageid',
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/__init__.py` & `zope.configuration-5.0/src/zope/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/src/zope/configuration/_compat.py` & `zope.configuration-5.0/src/zope/configuration/_compat.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,55 +7,16 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-import sys
 
-PY3 = sys.version_info[0] >= 3
-
-if PY3:  # pragma: PY3
-
-    import builtins
-
-    string_types = (str,)
-    text_type = str
-
-    # borrowed from 'six'
-    def reraise(tp, value, tb=None):
-        try:  # pragma: no cover
-            if value is None:
-                value = tp
-            if value.__traceback__ is not tb:
-                raise value.with_traceback(tb)
-            raise value
-        finally:
-            value = None
-            tb = None
-
-else:  # pragma: PY2
-
-    import __builtin__ as builtins  # noqa: F401 imported but unused
-
-    text_type = unicode  # noqa: F821 undefined name
-    string_types = (basestring,)  # noqa: F821 undefined name
-
-    # borrowed from 'six'
-    exec("""\
-def reraise(tp, value, tb=None):
-    try:
-        raise tp, value, tb
-    finally:
-        tb = None
-""")
-
-
-class implementer_if_needed(object):
+class implementer_if_needed:
     # Helper to make sure we don't redundantly implement
     # interfaces already inherited. Doing so tends to produce
     # problems with the C3 order. In this package, we could easily
     # statically determine to elide the relevant interfaces, but
     # this is a defense against changes in parent classes and lessens
     # the testing burden.
     def __init__(self, *ifaces):
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/config.py` & `zope.configuration-5.0/src/zope/configuration/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,39 +9,37 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Configuration processor
 """
-from keyword import iskeyword
+import builtins
 import operator
 import os.path
 import sys
+from keyword import iskeyword
 
-from zope.interface.adapter import AdapterRegistry
 from zope.interface import Interface
 from zope.interface import implementer
 from zope.interface import providedBy
-from zope.schema import TextLine
+from zope.interface.adapter import AdapterRegistry
 from zope.schema import URI
+from zope.schema import TextLine
 from zope.schema import ValidationError
 
+from zope.configuration._compat import implementer_if_needed
 from zope.configuration.exceptions import ConfigurationError
 from zope.configuration.exceptions import ConfigurationWrapperError
-from zope.configuration.interfaces import IConfigurationContext
-from zope.configuration.interfaces import IGroupingContext
 from zope.configuration.fields import GlobalInterface
 from zope.configuration.fields import GlobalObject
 from zope.configuration.fields import PathProcessor
-from zope.configuration._compat import builtins
-from zope.configuration._compat import reraise
-from zope.configuration._compat import string_types
-from zope.configuration._compat import text_type
-from zope.configuration._compat import implementer_if_needed
+from zope.configuration.interfaces import IConfigurationContext
+from zope.configuration.interfaces import IGroupingContext
+
 
 __all__ = [
     'ConfigurationContext',
     'ConfigurationAdapterRegistry',
     'ConfigurationMachine',
     'IStackItem',
     'SimpleStackItem',
@@ -70,15 +68,15 @@
 ]
 
 zopens = 'http://namespaces.zope.org/zope'
 metans = 'http://namespaces.zope.org/meta'
 testns = 'http://namespaces.zope.org/test'
 
 
-class ConfigurationContext(object):
+class ConfigurationContext:
     """
     Mix-in for implementing.
     :class:`zope.configuration.interfaces.IConfigurationContext`.
 
     Note that this class itself does not actually declare that it
     implements that interface; the subclass must do that. In addition,
     subclasses must provide a ``package`` attribute and a ``basepath``
@@ -125,15 +123,15 @@
         - ``info``, an object that has descriptive information about
           the action (defaults to '')
     """
 
     # pylint:disable=no-member
 
     def __init__(self):
-        super(ConfigurationContext, self).__init__()
+        super().__init__()
         self._seen_files = set()
         self._features = set()
 
     def resolve(self, dottedname):
         """
         Resolve a dotted name to an object.
 
@@ -225,15 +223,15 @@
             __import__(mname)
             mod = sys.modules[mname]
         except ImportError as v:
             if sys.exc_info()[2].tb_next is not None:
                 # ImportError was caused deeper
                 raise
             raise ConfigurationError(
-                "ImportError: Couldn't import %s, %s" % (mname, v))
+                f"ImportError: Couldn't import {mname}, {v}")
 
         if not oname:
             # see not mname case above
             return mod
 
         try:
             obj = getattr(mod, oname)
@@ -245,15 +243,15 @@
                 __import__(moname)
                 return sys.modules[moname]
             except ImportError:
                 if sys.exc_info()[2].tb_next is not None:
                     # ImportError was caused deeper
                     raise
                 raise ConfigurationError(
-                    "ImportError: Module %s has no global %s" % (mname, oname))
+                    f"ImportError: Module {mname} has no global {oname}")
 
     def path(self, filename):
         """
         Compute package-relative paths.
 
         Examples:
 
@@ -540,15 +538,15 @@
         Declare that a named feature has been provided.
 
         See :meth:`hasFeature` for examples.
         """
         self._features.add(feature)
 
 
-class ConfigurationAdapterRegistry(object):
+class ConfigurationAdapterRegistry:
     """
     Simple adapter registry that manages directives as adapters.
 
     Examples:
 
         >>> from zope.configuration.interfaces import IConfigurationContext
         >>> from zope.configuration.config import ConfigurationAdapterRegistry
@@ -595,30 +593,30 @@
         True
         >>> r.document('all-dir', None, None, None, None)
         >>> r._docRegistry[1][0]
         ('', 'all-dir')
     """
 
     def __init__(self):
-        super(ConfigurationAdapterRegistry, self).__init__()
+        super().__init__()
         self._registry = {}
         # Stores tuples of form:
         #   (namespace, name), schema, usedIn, info, parent
         self._docRegistry = []
 
     def register(self, interface, name, factory):
         r = self._registry.get(name)
         if r is None:
             r = AdapterRegistry()
             self._registry[name] = r
 
         r.register([interface], Interface, '', factory)
 
     def document(self, name, schema, usedIn, handler, info, parent=None):
-        if isinstance(name, string_types):
+        if isinstance(name, str):
             name = ('', name)
         self._docRegistry.append((name, schema, usedIn, handler, info, parent))
 
     def factory(self, context, name):
         r = self._registry.get(name)
         if r is None:
             # Try namespace-independent name
@@ -626,15 +624,15 @@
             r = self._registry.get(n)
             if r is None:
                 raise ConfigurationError("Unknown directive", ns, n)
 
         f = r.lookup1(providedBy(context), Interface)
         if f is None:
             raise ConfigurationError(
-                "The directive %s cannot be used in this context" % (name, ))
+                f"The directive {name} cannot be used in this context")
         return f
 
 
 @implementer(IConfigurationContext)
 class ConfigurationMachine(ConfigurationAdapterRegistry, ConfigurationContext):
     """
     Configuration machine.
@@ -680,15 +678,15 @@
     #: Users of instances of this class may modify this before calling
     #: `execute_actions` if they need to propagate specific exceptions.
     #:
     #: .. versionadded:: 4.2.0
     pass_through_exceptions = ()
 
     def __init__(self):
-        super(ConfigurationMachine, self).__init__()
+        super().__init__()
         self.actions = []
         self.stack = [RootStackItem(self)]
         self.i18n_strings = {}
         _bootstrap(self)
 
     def begin(self, __name, __data=None, __info=None, **kw):
         if __data:
@@ -792,17 +790,15 @@
                 except ConfigurationError as ex:
                     ex.add_details(info)
                     raise
                 except pass_through_exceptions:
                     raise
                 except Exception:
                     # Wrap it up and raise.
-                    reraise(
-                        ConfigurationExecutionError(info, sys.exc_info()[1]),
-                        None, sys.exc_info()[2])
+                    raise ConfigurationExecutionError(info, sys.exc_info()[1])
         finally:
             if clear:
                 del self.actions[:]
 
 
 class ConfigurationExecutionError(ConfigurationWrapperError):
     """
@@ -836,15 +832,15 @@
 
     def finish():
         """Finish processing a directive
         """
 
 
 @implementer(IStackItem)
-class SimpleStackItem(object):
+class SimpleStackItem:
     """
     Simple stack item
 
     A simple stack item can't have anything added after it.  It can
     only be removed.  It is used for simple directives and
     subdirectives, which can't contain other directives.
 
@@ -876,15 +872,15 @@
             for action in actions:
                 if not isinstance(action, dict):
                     action = expand_action(*action)  # b/c
                 context.action(**action)
 
 
 @implementer(IStackItem)
-class RootStackItem(object):
+class RootStackItem:
     """
     A root stack item.
     """
 
     def __init__(self, context):
         self.context = context
 
@@ -1057,15 +1053,15 @@
           'includepath': (),
           'info': '',
           'kw': {},
           'order': 0}]
     """
 
     def __init__(self, context):
-        super(GroupingStackItem, self).__init__(context)
+        super().__init__(context)
 
     def __callBefore(self):
         actions = self.context.before()
         if actions:
             for action in actions:
                 if not isinstance(action, dict):
                     action = expand_action(*action)
@@ -1087,15 +1083,15 @@
 
 
 def noop():
     pass
 
 
 @implementer(IStackItem)
-class ComplexStackItem(object):
+class ComplexStackItem:
     """
     Complex stack item
 
     A complex stack item is in the stack when a complex directive is
     being processed. It only allows subdirectives to be used.
 
     A complex stack item is created with a complex directive
@@ -1303,18 +1299,18 @@
 
 
 class IDirectivesInfo(Interface):
     """Schema for the ``directives`` directive
     """
 
     namespace = URI(
-        title=u"Namespace",
+        title="Namespace",
         description=(
-            u"The namespace in which directives' names "
-            u"will be defined"),
+            "The namespace in which directives' names "
+            "will be defined"),
     )
 
 
 class IDirectivesContext(IDirectivesInfo, IConfigurationContext):
     pass
 
 
@@ -1329,39 +1325,39 @@
 
 
 class IDirectiveInfo(Interface):
     """Information common to all directive definitions.
     """
 
     name = TextLine(
-        title=u"Directive name",
-        description=u"The name of the directive being defined",
+        title="Directive name",
+        description="The name of the directive being defined",
     )
 
     schema = DirectiveSchema(
-        title=u"Directive handler",
-        description=u"The dotted name of the directive handler",
+        title="Directive handler",
+        description="The dotted name of the directive handler",
     )
 
 
 class IFullInfo(IDirectiveInfo):
     """Information that all top-level directives (not subdirectives)
     have.
     """
 
     handler = GlobalObject(
-        title=u"Directive handler",
-        description=u"The dotted name of the directive handler",
+        title="Directive handler",
+        description="The dotted name of the directive handler",
     )
 
     usedIn = GlobalInterface(
-        title=u"The directive types the directive can be used in",
+        title="The directive types the directive can be used in",
         description=(
-            u"The interface of the directives that can contain "
-            u"the directive"
+            "The interface of the directives that can contain "
+            "the directive"
         ),
         default=IConfigurationContext,
     )
 
 
 class IStandaloneDirectiveInfo(IDirectivesInfo, IFullInfo):
     """Info for full directives defined outside a directives directives
@@ -1535,16 +1531,16 @@
 # Features
 
 
 class IProvidesDirectiveInfo(Interface):
     """Information for a <meta:provides> directive"""
 
     feature = TextLine(
-        title=u"Feature name",
-        description=u"""The name of the feature being provided
+        title="Feature name",
+        description="""The name of the feature being provided
 
         You can test available features with zcml:condition="have featurename".
         """,
     )
 
 
 def provides(context, feature):
@@ -1691,34 +1687,30 @@
         field = field.bind(context)
         n = name
         if n.endswith('_') and iskeyword(n[:-1]):
             n = n[:-1]
 
         s = data.get(n, data)
         if s is not data:
-            s = text_type(s)
+            s = str(s)
             del data[n]
 
             try:
                 args[str(name)] = field.fromUnicode(s)
             except ValidationError as v:
-                reraise(
-                    ConfigurationError(
-                        "Invalid value for %r" % (n)).add_details(v),
-                    None, sys.exc_info()[2])
+                raise ConfigurationError(
+                    "Invalid value for %r" % (n)).add_details(v)
         elif field.required:
             # if the default is valid, we can use that:
             default = field.default
             try:
                 field.validate(default)
             except ValidationError as v:
-                reraise(
-                    ConfigurationError(
-                        "Missing parameter: %r" % (n,)).add_details(v),
-                    None, sys.exc_info()[2])
+                raise ConfigurationError(
+                    f"Missing parameter: {n!r}").add_details(v)
             args[str(name)] = default
 
     if data:
         # we had data left over
         try:
             keyword_arguments = schema.getTaggedValue('keyword_arguments')
         except KeyError:
@@ -1834,27 +1826,27 @@
     # Sort conflict-resolved actions by (order, i) and return them.
     return [x[2] for x in sorted(output, key=operator.itemgetter(0, 1))]
 
 
 class ConfigurationConflictError(ConfigurationError):
 
     def __init__(self, conflicts):
-        super(ConfigurationConflictError, self).__init__()
+        super().__init__()
         self._conflicts = conflicts
 
     def _with_details(self, opening, detail_formatter):
         r = ["Conflicting configuration actions"]
         for discriminator, infos in sorted(self._conflicts.items()):
-            r.append("  For: %s" % (discriminator, ))
+            r.append(f"  For: {discriminator}")
             for info in infos:
-                for line in text_type(info).rstrip().split(u'\n'):
-                    r.append(u"    " + line)
+                for line in str(info).rstrip().split('\n'):
+                    r.append("    " + line)
 
         opening = "\n".join(r)
-        return super(ConfigurationConflictError, self)._with_details(
+        return super()._with_details(
             opening, detail_formatter)
 
 
 ##############################################################################
 # Bootstap code
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/docutils.py` & `zope.configuration-5.0/src/zope/configuration/docutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ##############################################################################
 """Helper Utility to wrap a text to a set width of characters
 """
 __docformat__ = 'restructuredtext'
 
 import re
 
+
 __all__ = [
     'wrap',
     'makeDocStructures',
 ]
 
 para_sep = re.compile('\n{2,}')
 whitespace = re.compile('[ \t\n\r]+')
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/exceptions.py` & `zope.configuration-5.0/src/zope/configuration/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 ##############################################################################
 """Standard configuration errors
 """
 
 import traceback
 
+
 __all__ = [
     'ConfigurationError',
 ]
 
 
 class ConfigurationError(Exception):
     """There was an error in a configuration
@@ -44,28 +45,28 @@
     def _with_details(self, opening, detail_formatter):
         lines = ['    ' + detail_formatter(detail) for detail in self._details]
         lines.append(opening)
         lines.reverse()
         return '\n'.join(lines)
 
     def __str__(self):
-        s = super(ConfigurationError, self).__str__()
+        s = super().__str__()
         return self._with_details(s, str)
 
     def __repr__(self):
-        s = super(ConfigurationError, self).__repr__()
+        s = super().__repr__()
         return self._with_details(s, repr)
 
 
 class ConfigurationWrapperError(ConfigurationError):
 
     USE_INFO_REPR = False
 
     def __init__(self, info, exception):
-        super(ConfigurationWrapperError, self).__init__(
+        super().__init__(
             repr(info) if self.USE_INFO_REPR else info)
         self.add_details(exception)
 
         # This stuff is undocumented and not used but we store
         # for backwards compatibility
         self.info = info
         self.etype = type(exception)
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/fields.py` & `zope.configuration-5.0/src/zope/configuration/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 from zope.schema import List
 from zope.schema import PythonIdentifier as schema_PythonIdentifier
 from zope.schema import Text
 from zope.schema import ValidationError
 from zope.schema.interfaces import IFromUnicode
 from zope.schema.interfaces import InvalidValue
 
+from zope.configuration._compat import implementer_if_needed
 from zope.configuration.exceptions import ConfigurationError
 from zope.configuration.interfaces import InvalidToken
-from zope.configuration._compat import implementer_if_needed
+
 
 __all__ = [
     'Bool',
     'GlobalObject',
     'GlobalInterface',
     'MessageID',
     'Path',
@@ -84,15 +85,15 @@
 
     .. versionchanged:: 4.2.0
        Extend `zope.schema.PythonIdentifier`, which implies that `fromUnicode`
        validates the strings.
     """
 
     def _validate(self, value):
-        super(PythonIdentifier, self)._validate(value)
+        super()._validate(value)
         if not value:
             raise ValidationError(value).with_field_and_value(self, value)
 
 
 @implementer_if_needed(IFromUnicode)
 class GlobalObject(Field):
     """
@@ -102,18 +103,18 @@
     not validated against the *value_type*.
     """
 
     _DOT_VALIDATOR = DottedName()
 
     def __init__(self, value_type=None, **kw):
         self.value_type = value_type
-        super(GlobalObject, self).__init__(**kw)
+        super().__init__(**kw)
 
     def _validate(self, value):
-        super(GlobalObject, self)._validate(value)
+        super()._validate(value)
         if self.value_type is not None:
             self.value_type.validate(value)
 
     def fromUnicode(self, value):
         r"""
         Find and return the module global at the path *value*.
 
@@ -211,15 +212,15 @@
       Traceback (most recent call last):
       ...
       NotAnInterface: (<class 'Foo'>, ...
 
     """
 
     def __init__(self, **kw):
-        super(GlobalInterface, self).__init__(InterfaceField(), **kw)
+        super().__init__(InterfaceField(), **kw)
 
 
 @implementer(IFromUnicode)
 class Tokens(List):
     """
     A list that can be read from a space-separated string.
     """
@@ -267,27 +268,27 @@
             vt = self.value_type.bind(self.context)
             values = []
             for s in value.split():
                 try:
                     v = vt.fromUnicode(s)
                 except ValidationError as ex:
                     raise InvalidToken(
-                        "%s in %r" % (ex, value)).with_field_and_value(
+                        f"{ex} in {value!r}").with_field_and_value(
                             self, s)
                 else:
                     values.append(v)
         else:
             values = []
 
         self.validate(values)
 
         return values
 
 
-class PathProcessor(object):
+class PathProcessor:
     # Internal helper for manipulations on paths
 
     @classmethod
     def expand(cls, filename):
         # Perform the expansions we want to have done. Returns a
         # tuple: (path, needs_processing) If the second value is true,
         # further processing should be done (the path isn't fully
@@ -535,21 +536,21 @@
             domain = 'untranslated'
             warnings.warn(
                 "You did not specify an i18n translation domain for the "
                 "'%s' field in %s" % (self.getName(), context.info.file)
             )
         if not isinstance(domain, str):
             # IZopeConfigure specifies i18n_domain as a BytesLine, but that's
-            # wrong on Python 3, where the filesystem uses str, and hence
+            # wrong as the filesystem uses str, and hence
             # zope.i18n registers ITranslationDomain utilities with str names.
             # If we keep bytes, we can't find those utilities.
             enc = sys.getfilesystemencoding() or sys.getdefaultencoding()
             domain = domain.decode(enc)
 
-        v = super(MessageID, self).fromUnicode(value)
+        v = super().fromUnicode(value)
 
         # Check whether there is an explicit message is specified
         default = None
         if v.startswith('[]'):
             v = v[2:].lstrip()
         elif v.startswith('['):
             end = v.find(']')
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/interfaces.py` & `zope.configuration-5.0/src/zope/configuration/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ##############################################################################
 """Zope Configuration (ZCML) interfaces
 """
 from zope.interface import Interface
 from zope.schema import BytesLine
 from zope.schema.interfaces import ValidationError
 
+
 __all__ = [
     'InvalidToken',
     'IConfigurationContext',
     'IGroupingContext',
 ]
 
 
@@ -34,16 +35,16 @@
     The configuration context manages information about the state of
     the configuration system, such as the package containing the
     configuration file. More importantly, it provides methods for
     importing objects and opening files relative to the package.
     """
 
     package = BytesLine(
-        title=(u"The current package name"),
-        description=(u"""\
+        title=("The current package name"),
+        description=("""\
           This is the name of the package containing the configuration
           file being executed. If the configuration file was not
           included by package, then this is None.
           """),
         required=False,
     )
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/name.py` & `zope.configuration-5.0/src/zope/configuration/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. note:: This module is no longer used by `zope.configuration` and
    may be deprecated soon. Its functions are not documented.
 """
 
 import os
 from types import ModuleType
 
+
 __all__ = [
     'resolve',
     'getNormalizedName',
     'path',
 ]
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/conditions.py` & `zope.configuration-5.0/src/zope/configuration/tests/conditions.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from zope.schema import Id
 
 
 class IRegister(Interface):
     """Trivial sample registry."""
 
     id = Id(
-        title=u"Identifier",
-        description=u"Some identifier that can be checked.",
+        title="Identifier",
+        description="Some identifier that can be checked.",
         required=True,
     )
 
 
 registry = []
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/conditions.zcml` & `zope.configuration-5.0/src/zope/configuration/tests/conditions.zcml`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/directives.py` & `zope.configuration-5.0/src/zope/configuration/tests/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 """
 from zope.interface import Interface
 from zope.interface import implementer
 from zope.schema import NativeStringLine
 from zope.schema import Text
 
 from zope.configuration.config import GroupingContextDecorator
-from zope.configuration.interfaces import IConfigurationContext
 from zope.configuration.fields import GlobalObject
+from zope.configuration.interfaces import IConfigurationContext
 
 
-class F(object):
+class F:
     def __repr__(self):
         return 'f'
 
     def __call__(self, *a, **k):
         raise NotImplementedError
 
 
@@ -37,19 +37,19 @@
 class ISimple(Interface):
 
     a = Text()
     b = Text(required=False)
     c = NativeStringLine()
 
 
-def simple(context, a=None, c=None, b=u"xxx"):
+def simple(context, a=None, c=None, b="xxx"):
     return [(('simple', a, b, c), f, (a, b, c))]
 
 
-def newsimple(context, a, c, b=u"xxx"):
+def newsimple(context, a, c, b="xxx"):
     context.action(('newsimple', a, b, c), f, (a, b, c))
 
 
 class IPackaged(Interface):
 
     package = GlobalObject()
 
@@ -68,17 +68,17 @@
     factory = GlobalObject()
 
 
 def factory(context, factory):
     context.action(('factory', 1, 2), factory)
 
 
-class Complex(object):
+class Complex:
 
-    def __init__(self, context, a, c, b=u"xxx"):
+    def __init__(self, context, a, c, b="xxx"):
         self.a, self.b, self.c = a, b, c
         context.action("Complex.__init__")
 
     def factory(self, context, factory):
         return [(('Complex.factory', 1, 2), factory, (self.a, ))]
 
     def __call__(self):
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/nested.py` & `zope.configuration-5.0/src/zope/configuration/tests/nested.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,36 +13,37 @@
 ##############################################################################
 """ Utilities for the 'nested directive' section in the narrative docs.
 """
 
 from zope.interface import Attribute
 from zope.interface import Interface
 from zope.interface import implementer
-from zope.schema import NativeStringLine
 from zope.schema import Id
 from zope.schema import Int
+from zope.schema import NativeStringLine
 from zope.schema import Text
 from zope.schema import TextLine
+
 from zope.configuration.config import GroupingContextDecorator
 from zope.configuration.fields import Bool
 
 
 schema_registry = {}
 
 
 class ISchemaInfo(Interface):
     """Parameter schema for the schema directive
     """
 
     name = TextLine(
-        title=u"The schema name",
-        description=u"This is a descriptive name for the schema.",
+        title="The schema name",
+        description="This is a descriptive name for the schema.",
     )
 
-    id = Id(title=u"The unique id for the schema")
+    id = Id(title="The unique id for the schema")
 
 
 class ISchema(Interface):
     """Interface that distinguishes the schema directive
     """
 
     fields = Attribute("Dictionary of field definitions")
@@ -70,55 +71,55 @@
             args=(self.id, schema),
         )
 
 
 class IFieldInfo(Interface):
 
     name = NativeStringLine(
-        title=u"The field name",
+        title="The field name",
     )
 
     title = TextLine(
-        title=u"Title",
-        description=u"A short summary or label",
-        default=u"",
+        title="Title",
+        description="A short summary or label",
+        default="",
         required=False,
     )
 
     required = Bool(
-        title=u"Required",
-        description=u"Determines whether a value is required.",
+        title="Required",
+        description="Determines whether a value is required.",
         default=True)
 
     readonly = Bool(
-        title=u"Read Only",
-        description=u"Can the value be modified?",
+        title="Read Only",
+        description="Can the value be modified?",
         required=False,
         default=False)
 
 
 class ITextInfo(IFieldInfo):
 
     min_length = Int(
-        title=u"Minimum length",
+        title="Minimum length",
         description=(
-            u"Value after whitespace processing cannot have less than "
-            u"min_length characters. If min_length is None, there is "
-            u"no minimum."
+            "Value after whitespace processing cannot have less than "
+            "min_length characters. If min_length is None, there is "
+            "no minimum."
         ),
         required=False,
         min=0,  # needs to be a positive number
         default=0)
 
     max_length = Int(
-        title=u"Maximum length",
+        title="Maximum length",
         description=(
-            u"Value after whitespace processing cannot have greater "
-            u"or equal than max_length characters. If max_length is "
-            u"None, there is no maximum."
+            "Value after whitespace processing cannot have greater "
+            "or equal than max_length characters. If max_length is "
+            "None, there is no maximum."
         ),
         required=False,
         min=0,  # needs to be a positive number
         default=None)
 
 
 def field(context, constructor, name, **kw):
@@ -136,21 +137,21 @@
 def textField(context, **kw):
     field(context, Text, **kw)
 
 
 class IIntInfo(IFieldInfo):
 
     min = Int(
-        title=u"Start of the range",
+        title="Start of the range",
         required=False,
         default=None
     )
 
     max = Int(
-        title=u"End of the range (excluding the value itself)",
+        title="End of the range (excluding the value itself)",
         required=False,
         default=None
     )
 
 
 def intField(context, **kw):
     field(context, Int, **kw)
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/samplepackage/foo.py` & `zope.configuration-5.0/src/zope/configuration/tests/samplepackage/foo.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Sample module used for testing
 """
 from zope.interface import Interface
+
 from zope import schema
 
+
 data = []
 
 
 class S1(Interface):
     x = schema.BytesLine()
     y = schema.Int()
 
 
-class stuff(object):
+class stuff:
     def __init__(self, args, info, basepath, package, includepath):
         (self.args, self.info, self.basepath, self.package, self.includepath
          ) = args, info, basepath, package, includepath
 
 
 def handler(_context, **kw):
     args = sorted(kw.items())
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/schema.zcml` & `zope.configuration-5.0/src/zope/configuration/tests/schema.zcml`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/simple.py` & `zope.configuration-5.0/src/zope/configuration/tests/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,35 +19,35 @@
 
 from zope.configuration.fields import Path
 
 
 class IRegisterFile(Interface):
 
     path = Path(
-        title=u"File path",
-        description=u"This is the path name of the file to be registered.",
+        title="File path",
+        description="This is the path name of the file to be registered.",
     )
 
     title = Text(
-        title=u"Short summary of the file",
-        description=u"This will be used in file listings",
+        title="Short summary of the file",
+        description="This will be used in file listings",
         required=False
     )
 
 
-class FileInfo(object):
+class FileInfo:
 
     def __init__(self, path, title, description, info):
         (self.path, self.title, self.description, self.info
          ) = path, title, description, info
 
 
 file_registry = []
 
 
-def registerFile(context, path, title=u""):
+def registerFile(context, path, title=""):
     info = context.info
     description = info.text.strip()
     context.action(discriminator=('RegisterFile', path),
                    callable=file_registry.append,
                    args=(FileInfo(path, title, description, info),)
                    )
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/simple.zcml` & `zope.configuration-5.0/src/zope/configuration/tests/simple.zcml`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test___init__.py` & `zope.configuration-5.0/src/zope/configuration/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_config.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test configuration machinery.
 """
-import unittest
 import sys
+import unittest
+
 
 # pylint:disable=inherit-non-class,protected-access
 # pylint:disable=attribute-defined-outside-init, arguments-differ
 
 
 class ConfigurationContextTests(unittest.TestCase):
 
@@ -70,15 +71,15 @@
         from zope.configuration.exceptions import ConfigurationError
         c = self._makeOne()
         c.package = None
         with self.assertRaises(ConfigurationError):
             c.resolve('.nonesuch')
 
     def test_resolve_relative_miss_w_package_too_many_dots(self):
-        class FauxPackage(object):
+        class FauxPackage:
             __name__ = None
         from zope.configuration.exceptions import ConfigurationError
         c = self._makeOne()
         package = c.package = FauxPackage()
         package.__name__ = 'one.dot'
         with self.assertRaises(ConfigurationError):
             c.resolve('....nonesuch')
@@ -195,14 +196,15 @@
         import os
         c = self._makeOne()
         c.checkDuplicate('/path')  # doesn't raise
         self.assertEqual(list(c._seen_files), [os.path.normpath('/path')])
 
     def test_checkDuplicate_hit(self):
         import os
+
         from zope.configuration.exceptions import ConfigurationError
         c = self._makeOne()
         c.checkDuplicate('/path')
         with self.assertRaises(ConfigurationError):
             c.checkDuplicate('/path')
         self.assertEqual(list(c._seen_files), [os.path.normpath('/path')])
 
@@ -464,15 +466,15 @@
         from zope.interface import Interface
         from zope.interface import implementer
 
         class IFoo(Interface):
             pass
 
         @implementer(IFoo)
-        class Context(object):
+        class Context:
             pass
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         context = Context()
 
         def _factory():
             raise AssertionError("should not be called")
@@ -484,28 +486,29 @@
         from zope.interface import Interface
         from zope.interface import implementer
 
         class IFoo(Interface):
             pass
 
         @implementer(IFoo)
-        class Context(object):
+        class Context:
             pass
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         context = Context()
 
         def _factory():
             raise AssertionError("should not be called")
         reg = self._makeOne()
         reg.register(IFoo, NAME, _factory)
         self.assertEqual(reg.factory(context, (NS, NAME)), _factory)
 
     def test_factory_hit_on_fqn_lookup_fails(self):
         from zope.interface import Interface
+
         from zope.configuration.exceptions import ConfigurationError
 
         class IFoo(Interface):
             pass
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         context = object()  # doesn't provide IFoo
@@ -514,29 +517,31 @@
             raise AssertionError("should not be called")
         reg = self._makeOne()
         reg.register(IFoo, (NS, NAME), _factory)
         with self.assertRaises(ConfigurationError):
             reg.factory(context, (NS, NAME))
 
 
-class _ConformsToIConfigurationContext(object):
+class _ConformsToIConfigurationContext:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kwargs):
         raise NotImplementedError
 
     def test_class_conforms_to_IConfigurationContext(self):
         from zope.interface.verify import verifyClass
+
         from zope.configuration.interfaces import IConfigurationContext
         verifyClass(IConfigurationContext, self._getTargetClass())
 
     def test_instance_conforms_to_IConfigurationContext(self):
         from zope.interface.verify import verifyObject
+
         from zope.configuration.interfaces import IConfigurationContext
         verifyObject(IConfigurationContext, self._makeOne())
 
 
 class ConfigurationMachineTests(_ConformsToIConfigurationContext,
                                 unittest.TestCase,
                                 ):
@@ -580,14 +585,15 @@
         cm = self._makeOne()
         cm.register(IConfigurationContext, (NS, NAME), _factory)
         with self.assertRaises(TypeError):
             cm.begin((NS, NAME), {'foo': 'bar'}, baz='bam')
 
     def test_begin_w___data_no_kw(self):
         from zope.interface import Interface
+
         from zope.configuration.config import IConfigurationContext
         from zope.configuration.config import RootStackItem
 
         class ISchema(Interface):
             pass
 
         class IUsedIn(Interface):
@@ -622,14 +628,15 @@
                              'schema': ISchema,
                              'usedIn': IUsedIn,
                              'handler': _handler,
                          }, 'INFO')])
 
     def test_begin_wo___data_w_kw(self):
         from zope.interface import Interface
+
         from zope.configuration.config import IConfigurationContext
         from zope.configuration.config import RootStackItem
 
         class ISchema(Interface):
             pass
 
         class IUsedIn(Interface):
@@ -666,15 +673,15 @@
                              'usedIn': IUsedIn,
                              'handler': _handler,
                          }, 'INFO')])
 
     def test_end(self):
         from zope.configuration.config import RootStackItem
 
-        class FauxItem(object):
+        class FauxItem:
             _finished = False
 
             def finish(self):
                 self._finished = True
         cm = self._makeOne()
         item = FauxItem()
         cm.stack.append(item)
@@ -682,24 +689,25 @@
         self.assertEqual(len(cm.stack), 1)
         root = cm.stack[0]
         self.assertIsInstance(root, RootStackItem)
         self.assertTrue(item._finished)
 
     def test___call__(self):
         from zope.interface import Interface
+
         from zope.configuration.config import IConfigurationContext
         from zope.configuration.config import RootStackItem
 
         class ISchema(Interface):
             pass
 
         class IUsedIn(Interface):
             pass
 
-        class FauxItem(object):
+        class FauxItem:
             _finished = False
 
             def finish(self):
                 self._finished = True
 
         def _handler(*args, **kw):
             raise AssertionError("should not be called")
@@ -738,30 +746,30 @@
 
     def test_getInfo_only_root(self):
         cm = self._makeOne()
         cm.info = 'INFO'
         self.assertEqual(cm.getInfo(), 'INFO')
 
     def test_getInfo_w_item(self):
-        class FauxItem(object):
+        class FauxItem:
             info = 'FAUX'
 
             def __init__(self):
                 self.context = self
         cm = self._makeOne()
         cm.stack.append(FauxItem())
         self.assertEqual(cm.getInfo(), 'FAUX')
 
     def test_setInfo_only_root(self):
         cm = self._makeOne()
         cm.setInfo('INFO')
         self.assertEqual(cm.info, 'INFO')
 
     def test_setInfo_w_item(self):
-        class FauxItem(object):
+        class FauxItem:
             info = 'FAUX'
 
             def __init__(self):
                 self.context = self
         cm = self._makeOne()
         item = FauxItem()
         cm.stack.append(item)
@@ -877,43 +885,45 @@
 
         # Which makes it easier to define the other directives:
         machine((metans, "directive"),
                 namespace=ns, name="k",
                 schema=".Ik", handler=".k")
 
         machine((ns, "k"), "yee ha",
-                **{"for": u"f", "class": u"c", "x": u"x"})
+                **{"for": "f", "class": "c", "x": "x"})
 
         self.assertEqual(len(machine.actions), 1)
         self.assertEqual(machine.actions[0],
                          {'args': ('f', 'c', 'x'),
                           'callable': f,
                           'discriminator': ('k', 'f'),
                           'includepath': (),
                           'info': 'yee ha',
                           'kw': {},
                           'order': 0,
                           })
 
 
-class _ConformsToIStackItem(object):
+class _ConformsToIStackItem:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kwargs):
         raise NotImplementedError
 
     def test_class_conforms_to_IStackItem(self):
         from zope.interface.verify import verifyClass
+
         from zope.configuration.config import IStackItem
         verifyClass(IStackItem, self._getTargetClass())
 
     def test_instance_conforms_to_IStackItem(self):
         from zope.interface.verify import verifyObject
+
         from zope.configuration.config import IStackItem
         verifyObject(IStackItem, self._makeOne())
 
 
 class SimpleStackItemTests(_ConformsToIStackItem,
                            unittest.TestCase,
                            ):
@@ -937,14 +947,15 @@
             schema = Interface
         if data is None:
             data = {}
         return self._getTargetClass()(context, handler, info, schema, data)
 
     def test_ctor(self):
         from zope.interface import Interface
+
         from zope.configuration.config import GroupingContextDecorator
 
         class ISchema(Interface):
             pass
         context = FauxContext()
 
         def _handler():
@@ -1043,30 +1054,30 @@
         if context is None:
             context = object()
         return self._getTargetClass()(context)
 
     def test_contained_context_factory_fails(self):
         from zope.configuration.exceptions import ConfigurationError
 
-        class _Context(object):
+        class _Context:
             def factory(self, context, name):
                 "does nothing"
         rsi = self._makeOne(_Context())
         with self.assertRaises(ConfigurationError):
             rsi.contained(('ns', 'name'), {}, '')
 
     def test_contained_context_factory_normal(self):
         _called_with = []
         _adapter = object()
 
         def _factory(context, data, info):
             _called_with.append((context, data, info))
             return _adapter
 
-        class _Context(object):
+        class _Context:
             def factory(self, context, name):
                 return _factory
         context = _Context()
         rsi = self._makeOne(context)
         adapter = rsi.contained(('ns', 'name'), {'a': 'b'}, 'INFO')
         self.assertTrue(adapter is _adapter)
         self.assertEqual(_called_with, [(context, {'a': 'b'}, 'INFO')])
@@ -1258,23 +1269,24 @@
         NAME = 'testing'
         csi = self._makeOne()
         with self.assertRaises(ConfigurationError):
             csi.contained((NS, NAME), {}, 'INFO')
 
     def test_contained_hit(self):
         from zope.interface import Interface
+
         from zope.configuration.config import GroupingContextDecorator
         from zope.configuration.config import SimpleStackItem
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
 
         class ISubSchema(Interface):
             pass
 
-        class WithName(object):
+        class WithName:
             def testing(self, *args):
                 raise AssertionError("should not be called")
         meta = self._makeMeta()
         wn = meta._handler = WithName()
         meta[NAME] = (ISubSchema, 'SUBINFO')
         context = FauxContext()
         _data = {'name': 'NAME'}
@@ -1360,29 +1372,31 @@
                           'kw': {},
                           'includepath': (),
                           'info': 'INFO',
                           'order': 0,
                           })
 
 
-class _ConformsToIGroupingContext(object):
+class _ConformsToIGroupingContext:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kwargs):
         raise NotImplementedError
 
     def test_class_conforms_to_IGroupingContext(self):
         from zope.interface.verify import verifyClass
+
         from zope.configuration.interfaces import IGroupingContext
         verifyClass(IGroupingContext, self._getTargetClass())
 
     def test_instance_conforms_to_IGroupingContext(self):
         from zope.interface.verify import verifyObject
+
         from zope.configuration.interfaces import IGroupingContext
         verifyObject(IGroupingContext, self._makeOne())
 
 
 class GroupingContextDecoratorTests(_ConformsToIConfigurationContext,
                                     _ConformsToIGroupingContext,
                                     unittest.TestCase,
@@ -1423,29 +1437,31 @@
         gcd.before()  # noraise
 
     def test_after(self):
         gcd = self._makeOne()
         gcd.after()  # noraise
 
 
-class _ConformsToIDirectivesContext(object):
+class _ConformsToIDirectivesContext:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kwargs):
         raise NotImplementedError
 
     def test_class_conforms_to_IDirectivesContext(self):
         from zope.interface.verify import verifyClass
+
         from zope.configuration.config import IDirectivesContext
         verifyClass(IDirectivesContext, self._getTargetClass())
 
     def test_instance_conforms_to_IDirectivesContext(self):
         from zope.interface.verify import verifyObject
+
         from zope.configuration.config import IDirectivesContext
         verifyObject(IDirectivesContext, self._makeOne())
 
 
 class DirectivesHandlerTests(_ConformsToIDirectivesContext,
                              unittest.TestCase,
                              ):
@@ -1480,14 +1496,15 @@
 
             def document(self, name, schema, usedIn, handler, info):
                 self._documented.append((name, schema, usedIn, handler, info))
         return _Context()
 
     def test_defaults(self):
         from zope.interface import Interface
+
         from zope.configuration.interfaces import IConfigurationContext as ICC
 
         class ISchema(Interface):
             pass
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         context = self._makeContext()
@@ -1567,14 +1584,15 @@
             def document(self, name, schema, usedIn, handler, info):
                 self._documented.append((name, schema, usedIn, handler, info))
         return _Context()
 
     def test_defaults(self):
         from zope.interface import Interface
         from zope.schema import Text
+
         from zope.configuration.interfaces import IConfigurationContext as ICC
 
         class ISchema(Interface):
             arg = Text()
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         context = self._makeContext()
@@ -1638,29 +1656,31 @@
         self.assertEqual(_called_with, [(sub, {'arg': 'val'})])
 
         self.assertEqual(len(context._documented), 1)
         self.assertEqual(context._documented[0],
                          (NAME, ISchema, IUsedIn, _handler, 'INFO'))
 
 
-class _ConformsToIComplexDirectiveContext(object):
+class _ConformsToIComplexDirectiveContext:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kwargs):
         raise NotImplementedError
 
     def test_class_conforms_to_IComplexDirectiveContext(self):
         from zope.interface.verify import verifyClass
+
         from zope.configuration.config import IComplexDirectiveContext
         verifyClass(IComplexDirectiveContext, self._getTargetClass())
 
     def test_instance_conforms_to_IComplexDirectiveContext(self):
         from zope.interface.verify import verifyObject
+
         from zope.configuration.config import IComplexDirectiveContext
         verifyObject(IComplexDirectiveContext, self._makeOne())
 
 
 class ComplexDirectiveDefinitionTests(_ConformsToIComplexDirectiveContext,
                                       unittest.TestCase,
                                       ):
@@ -1740,15 +1760,15 @@
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.config import subdirective
         return subdirective(*args, **kw)
 
     def _makeContext(self, package=None, namespace=None, name=None,
                      schema=None, handler=None, usedIn=None):
-        class _Context(object):
+        class _Context:
             def __init__(self):
                 self.context = {}
                 self._documented = []
 
             def document(self, *args):
                 self._documented.append(args)
         context = _Context()
@@ -1799,15 +1819,15 @@
 
         class ISchema(Interface):
             pass
 
         class IUsedIn(Interface):
             pass
 
-        class Handler(object):
+        class Handler:
             sub = object()
         NS = 'http://namespace.example.com/'
         NAME = 'testing'
         SUBNAME = 'sub'
         handler = Handler()
         context = self._makeContext(None, NS, NAME, ISchema, handler, IUsedIn)
         context.info = 'INFO'
@@ -1856,17 +1876,18 @@
 
         class ISchema(Interface):
             pass
         context = FauxContext()
         self.assertEqual(self._callFUT(context, ISchema, {}), {})
 
     def test_w_empty_schema_w_data_no_kwargs_allowed(self):
-        from zope.configuration.exceptions import ConfigurationError
         from zope.interface import Interface
 
+        from zope.configuration.exceptions import ConfigurationError
+
         class ISchema(Interface):
             pass
         context = FauxContext()
         with self.assertRaises(ConfigurationError) as exc:
             self._callFUT(context, ISchema, {'a': 'b'})
         self.assertEqual(exc.exception.args,
                          ('Unrecognized parameters:', 'a'))
@@ -1890,14 +1911,15 @@
         context = FauxContext()
         self.assertEqual(self._callFUT(context, ISchema, {'for': 'foo'}),
                          {'for_': 'foo'})
 
     def test_w_field_missing_no_default(self):
         from zope.interface import Interface
         from zope.schema import Text
+
         from zope.configuration.exceptions import ConfigurationError
 
         class ISchema(Interface):
             no_default = Text()
         context = FauxContext()
         with self.assertRaises(ConfigurationError) as exc:
             self._callFUT(context, ISchema, {})
@@ -1916,22 +1938,23 @@
         ), exception_str)
 
     def test_w_field_missing_but_default(self):
         from zope.interface import Interface
         from zope.schema import Text
 
         class ISchema(Interface):
-            w_default = Text(default=u'default')
+            w_default = Text(default='default')
         context = FauxContext()
         self.assertEqual(self._callFUT(context, ISchema, {}),
                          {'w_default': 'default'})
 
     def test_w_invalid_value(self):
         from zope.interface import Interface
         from zope.schema import Int
+
         from zope.configuration.exceptions import ConfigurationError
 
         class ISchema(Interface):
             count = Int(min=0)
         context = FauxContext()
         with self.assertRaises(ConfigurationError) as exc:
             self._callFUT(context, ISchema, {'count': '-1'})
@@ -2149,13 +2172,13 @@
             expand_action(None, _c, order=2),
             expand_action(None, _d, order=1),
         ]
         self.assertEqual([x['callable'] for x in self._callFUT(actions)],
                          [_b, _d, _c, _a])
 
 
-class FauxContext(object):
+class FauxContext:
     def __init__(self):
         self.actions = []
 
     def action(self, **kw):
         self.actions.append(kw)
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_docs.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##############################################################################
 #
 # Copyright (c) 2018 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
@@ -11,39 +10,25 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """
 Tests for the documentation.
 """
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
 
-import re
+import doctest
 import os.path
 import unittest
-import doctest
 
 import manuel.capture
 import manuel.codeblock
 import manuel.doctest
 import manuel.ignore
 import manuel.testing
 
-from zope.testing import renormalizing
-
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"), r"\1"),
-    (re.compile('u(".*?")'), r"\1"),
-    # Python 3 bytes added the "b".
-    (re.compile("b('.*?')"), r"\1"),
-    (re.compile('b(".*?")'), r"\1"),
-])
 
 optionflags = (
     doctest.NORMALIZE_WHITESPACE
     | doctest.ELLIPSIS
     | doctest.IGNORE_EXCEPTION_DETAIL
 )
 
@@ -59,15 +44,16 @@
             class SkippedDocTests(unittest.TestCase):  # pragma: no cover
 
                 @unittest.skip('Could not find setup.py')
                 def test_docs(self):
                     pass
 
             suite.addTest(
-                unittest.makeSuite(SkippedDocTests))  # pragma: no cover
+                unittest.defaultTestLoader.loadTestsFromTestCase(
+                    SkippedDocTests))  # pragma: no cover
             return suite  # pragma: no cover
 
     docs = os.path.join(here, 'docs')
     api_docs = os.path.join(docs, 'api')
 
     doc_files_to_test = (
         'narr.rst',
@@ -91,15 +77,15 @@
         'zopeconfigure',
     )
 
     paths = [os.path.join(docs, f) for f in doc_files_to_test]
     paths += [os.path.join(api_docs, f) for f in api_files_to_test]
 
     m = manuel.ignore.Manuel()
-    m += manuel.doctest.Manuel(checker=checker, optionflags=optionflags)
+    m += manuel.doctest.Manuel(optionflags=optionflags)
     m += manuel.codeblock.Manuel()
     m += manuel.capture.Manuel()
 
     suite.addTest(
         manuel.testing.TestSuite(
             m,
             *paths
@@ -107,15 +93,14 @@
     )
 
     for mod_name in api_to_test:
         mod_name = 'zope.configuration.' + mod_name
         suite.addTest(
             doctest.DocTestSuite(
                 mod_name,
-                checker=checker,
                 optionflags=optionflags
             )
         )
 
     return suite
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_docutils.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_docutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 class Test_makeDocStructures(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.docutils import makeDocStructures
         return makeDocStructures(*args, **kw)
 
     def _makeContext(self):
-        class _Context(object):
+        class _Context:
             def __init__(self):
                 self._docRegistry = []
         return _Context()
 
     def test_empty(self):
         context = self._makeContext()
         namespaces, subdirs = self._callFUT(context)
@@ -107,15 +107,15 @@
 
         def _two():
             raise AssertionError("should not be called")
 
         def _three():
             raise AssertionError("should not be called")
 
-        class Parent(object):
+        class Parent:
             namespace = PNS
             name = 'parent'
         parent1 = Parent()
         parent2 = Parent()
         parent2.name = 'parent2'
         context = self._makeContext()
         context._docRegistry.append(
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_fields.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test zope.configuration.fields.
 """
 import unittest
 
+
 # pylint:disable=protected-access
 
 
-class _ConformsToIFromUnicode(object):
+class _ConformsToIFromUnicode:
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self, *args, **kw):
         raise NotImplementedError
 
@@ -44,35 +45,36 @@
         return GlobalObject
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def test__validate_wo_value_type(self):
         go = self._makeOne(value_type=None)
-        for value in [0, 0.0, (), [], set(), frozenset(), u'', b'']:
+        for value in [0, 0.0, (), [], set(), frozenset(), '', b'']:
             go._validate(value)  # noraise
 
     def test__validate_w_value_type(self):
         from zope.schema import Text
         from zope.schema.interfaces import WrongType
         go = self._makeOne(value_type=Text())
-        go.validate(u'')
+        go.validate('')
         for value in [0, 0.0, (), [], set(), frozenset(), b'']:
             with self.assertRaises(WrongType):
                 go._validate(value)
 
     def test_fromUnicode_w_star_and_extra_ws(self):
         go = self._makeOne()
         self.assertEqual(go.fromUnicode(' * '), None)
 
     def test_fromUnicode_w_resolve_fails(self):
         from zope.schema import ValidationError
+
         from zope.configuration.config import ConfigurationError
 
-        class Context(object):
+        class Context:
             _resolved = None
 
             def resolve(self, name):
                 self._resolved = name
                 raise ConfigurationError()
         go = self._makeOne()
         context = Context()
@@ -83,15 +85,15 @@
         ex = exc.exception
         self.assertIs(ex.field, bound)
         self.assertEqual(ex.value, 'tried')
 
     def test_fromUnicode_w_resolve_success(self):
         _target = object()
 
-        class Context(object):
+        class Context:
             _resolved = None
 
             def resolve(self, name):
                 self._resolved = name
                 return _target
         go = self._makeOne()
         context = Context()
@@ -99,15 +101,15 @@
         found = bound.fromUnicode('tried')
         self.assertIs(found, _target)
         self.assertEqual(context._resolved, 'tried')
 
     def test_fromUnicode_w_resolve_dots(self):
         _target = object()
 
-        class Context(object):
+        class Context:
             _resolved = None
 
             def resolve(self, name):
                 self._resolved = name
                 return _target
         go = self._makeOne()
         context = Context()
@@ -124,15 +126,15 @@
             self.assertEqual(context._resolved, name)
 
     def test_fromUnicode_w_resolve_but_validation_fails(self):
         from zope.schema import Text
         from zope.schema import ValidationError
         _target = object()
 
-        class Context(object):
+        class Context:
             _resolved = None
 
             def resolve(self, name):
                 self._resolved = name
                 return _target
         go = self._makeOne(value_type=Text())
         context = Context()
@@ -178,23 +180,24 @@
     def test_fromUnicode_empty(self):
         tok = self._makeOne()
         self.assertEqual(tok.fromUnicode(''), [])
 
     def test_fromUnicode_strips_ws(self):
         from zope.schema import Text
         tok = self._makeOne(value_type=Text())
-        self.assertEqual(tok.fromUnicode(u' one two three '),
-                         [u'one', u'two', u'three'])
+        self.assertEqual(tok.fromUnicode(' one two three '),
+                         ['one', 'two', 'three'])
 
     def test_fromUnicode_invalid(self):
         from zope.schema import Int
+
         from zope.configuration.interfaces import InvalidToken
         tok = self._makeOne(value_type=Int(min=0))
         with self.assertRaises(InvalidToken) as exc:
-            tok.fromUnicode(u' 1 -1 3 ')
+            tok.fromUnicode(' 1 -1 3 ')
 
         ex = exc.exception
         self.assertIs(ex.field, tok)
         self.assertEqual(ex.value, '-1')
 
 
 class PathTests(unittest.TestCase, _ConformsToIFromUnicode):
@@ -208,15 +211,15 @@
 
     def test_fromUnicode_absolute(self):
         import os
         path = self._makeOne()
         self.assertEqual(path.fromUnicode('/'), os.path.normpath('/'))
 
     def test_fromUnicode_relative(self):
-        class Context(object):
+        class Context:
             _pathed = None
 
             def path(self, value):
                 self._pathed = value
                 return '/hard/coded'
         context = Context()
         path = self._makeOne()
@@ -264,33 +267,33 @@
         from zope.configuration.fields import MessageID
         return MessageID
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def _makeContext(self, domain='testing_domain'):
-        class Info(object):
+        class Info:
             file = 'test_file'
             line = 42
 
-        class Context(object):
+        class Context:
             i18n_domain = domain
 
             def __init__(self):
                 self.i18n_strings = {}
                 self.info = Info()
         return Context()
 
     def test_wo_domain(self):
         import warnings
         mid = self._makeOne()
         context = self._makeContext(None)
         bound = mid.bind(context)
         with warnings.catch_warnings(record=True) as log:
-            msgid = bound.fromUnicode(u'testing')
+            msgid = bound.fromUnicode('testing')
         self.assertEqual(len(log), 1)
         self.assertTrue(str(log[0].message).startswith(
             'You did not specify an i18n translation domain'))
         self.assertEqual(msgid, 'testing')
         self.assertEqual(msgid.default, None)
         self.assertEqual(msgid.domain, 'untranslated')
         self.assertEqual(context.i18n_strings,
@@ -298,36 +301,36 @@
 
     def test_w_empty_id(self):
         import warnings
         mid = self._makeOne()
         context = self._makeContext()
         bound = mid.bind(context)
         with warnings.catch_warnings(record=True) as log:
-            msgid = bound.fromUnicode(u'[] testing')
+            msgid = bound.fromUnicode('[] testing')
         self.assertEqual(len(log), 0)
         self.assertEqual(msgid, 'testing')
         self.assertEqual(msgid.default, None)
         self.assertEqual(msgid.domain, 'testing_domain')
         self.assertEqual(context.i18n_strings,
                          {'testing_domain': {'testing': [('test_file', 42)]}})
 
     def test_w_id_and_default(self):
         import warnings
         mid = self._makeOne()
         context = self._makeContext()
         bound = mid.bind(context)
         with warnings.catch_warnings(record=True) as log:
-            msgid = bound.fromUnicode(u'[testing] default')
+            msgid = bound.fromUnicode('[testing] default')
         self.assertEqual(len(log), 0)
         self.assertEqual(msgid, 'testing')
         self.assertEqual(msgid.default, 'default')
         self.assertEqual(msgid.domain, 'testing_domain')
         self.assertEqual(context.i18n_strings,
                          {'testing_domain': {'testing': [('test_file', 42)]}})
 
     def test_domain_decodes_bytes(self):
         mid = self._makeOne()
         context = self._makeContext(domain=b'domain')
         bound = mid.bind(context)
-        msgid = bound.fromUnicode(u'msgid')
+        msgid = bound.fromUnicode('msgid')
         self.assertIsInstance(msgid.domain, str)
         self.assertEqual(msgid.domain, 'domain')
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_name.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     def test_function_in_module(self):
         import os.path
         self.assertTrue(self._callFUT('os.path.join') is os.path.join)
 
     def test_importable_but_not_attr_of_parent(self):
         import sys
+
         import zope.configuration.tests as zct
         self.assertFalse('notyet' in zct.__dict__)
         mod = self._callFUT('zope.configuration.tests.notyet')
         self.assertTrue(mod is zct.notyet)
         del zct.notyet
         del sys.modules['zope.configuration.tests.notyet']
 
@@ -50,16 +51,16 @@
     def test_class_in_module(self):
         from zope.configuration.tests.directives import Complex
         self.assertIs(
             self._callFUT('zope.configuration.tests.directives.Complex'),
             Complex)
 
     def test_class_w_same_name_as_module(self):
-        from zope.configuration.tests.samplepackage.NamedForClass \
-            import NamedForClass
+        from zope.configuration.tests.samplepackage.NamedForClass import \
+            NamedForClass
         self.assertIs(
             self._callFUT(
                 'zope.configuration.tests.samplepackage.NamedForClass+'),
             NamedForClass)
         self.assertIs(
             self._callFUT(
                 'zope.configuration.tests.samplepackage.NamedForClass.'),
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_xmlconfig.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_xmlconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 #
 ##############################################################################
 """Test zope.configuration.xmlconfig.
 """
 import unittest
 
 
-NS = u'ns'
-FOO = u'foo'
-XXX = u'xxx'
-SPLAT = u'splat'
-SPLATV = u'splatv'
-A = u'a'
-AVALUE = u'avalue'
-B = u'b'
-BVALUE = u'bvalue'
+NS = 'ns'
+FOO = 'foo'
+XXX = 'xxx'
+SPLAT = 'splat'
+SPLATV = 'splatv'
+A = 'a'
+AVALUE = 'avalue'
+B = 'b'
+BVALUE = 'bvalue'
 
 # pylint:disable=protected-access
 
 
 class ZopeXMLConfigurationErrorTests(unittest.TestCase):
     maxDiff = None
 
@@ -171,15 +171,15 @@
                                         meth='endElementNS',
                                         meth_args=((NS, FOO), FOO)):
         class ErrorContext(FauxContext):
             def end(self, *args):
                 raise raises("xxx")
             begin = end
 
-        class Info(object):
+        class Info:
             _line = _col = None
 
             def end(self, line, col):
                 self._line, self._col = line, col
         context = ErrorContext()
         info = Info()
         context.setInfo(info)
@@ -362,15 +362,15 @@
         handler = self._makeOne(context)
         with self.assertRaises(ValueError) as exc:
             handler.evaluateCondition('nonesuch')
         self.assertEqual(str(exc.exception.args[0]),
                          "Invalid ZCML condition: 'nonesuch'")
 
     def test_endElementNS_normal(self):
-        class Info(object):
+        class Info:
             _line = _col = None
 
             def end(self, line, col):
                 self._line, self._col = line, col
         context = FauxContext()
         info = Info()
         context.setInfo(info)
@@ -387,30 +387,31 @@
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.xmlconfig import processxmlfile
         return processxmlfile(*args, **kw)
 
     def test_w_empty_xml(self):
         from io import StringIO
+
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.xmlconfig import ZopeSAXParseException
+        from zope.configuration.xmlconfig import registerCommonDirectives
 
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         with self.assertRaises(ZopeSAXParseException) as exc:
             self._callFUT(StringIO(), context)
         self.assertEqual(str(exc.exception.evalue),
                          '<string>:1:0: no element found')
 
     def test_w_valid_xml_fp(self):
         # Integration test, really
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests.samplepackage import foo
+        from zope.configuration.xmlconfig import registerCommonDirectives
 
         context = ConfigurationMachine()
         registerCommonDirectives(context)
 
         with open(path("samplepackage", "configure.zcml")) as file:
             self._callFUT(file, context)
         self.assertEqual(foo.data, [])
@@ -432,14 +433,15 @@
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.xmlconfig import openInOrPlain
         return openInOrPlain(*args, **kw)
 
     def _makeFilename(self, fn):
         import os
+
         from zope.configuration.tests.samplepackage import __file__
         return os.path.join(os.path.dirname(__file__), fn)
 
     def test_file_present(self):
         import os
         with self._callFUT(self._makeFilename('configure.zcml')) as fp:
             self.assertEqual(os.path.basename(fp.name), 'configure.zcml')
@@ -469,33 +471,33 @@
                 context, 'tests//sample.zcml', files=['tests/*.zcml'])
         self.assertEqual(str(exc.exception),
                          "Must specify only one of file or files")
 
     def test_neither_file_nor_files_passed_already_seen(self):
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests import samplepackage
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         context.package = samplepackage
         fqn = _packageFile(samplepackage, 'configure.zcml')
         context._seen_files.add(fqn)
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
             self._callFUT(context)  # skips
         self.assertEqual(len(logger.debugs), 0)
         self.assertEqual(len(context.actions), 0)
 
     def test_neither_file_nor_files_passed(self):
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         before_stack = context.stack[:]
         context.package = samplepackage
         fqn = _packageFile(samplepackage, 'configure.zcml')
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
@@ -507,19 +509,19 @@
         self.assertEqual(action['callable'], foo.data.append)
         self.assertEqual(action['includepath'], (fqn,))
         self.assertEqual(context.stack, before_stack)
         self.assertEqual(len(context._seen_files), 1)
         self.assertIn(fqn, context._seen_files)
 
     def test_w_file_passed(self):
+        from zope.configuration import tests
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
-        from zope.configuration import tests
         from zope.configuration.tests import simple
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         before_stack = context.stack[:]
         context.package = tests
         fqn = _packageFile(tests, 'simple.zcml')
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
@@ -545,17 +547,17 @@
         self.assertEqual(context.stack, before_stack)
         self.assertEqual(len(context._seen_files), 1)
         self.assertIn(fqn, context._seen_files)
 
     def test_w_files_passed_and_package(self):
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         before_stack = context.stack[:]
         fqn1 = _packageFile(samplepackage, 'baz1.zcml')
         fqn2 = _packageFile(samplepackage, 'baz2.zcml')
         fqn3 = _packageFile(samplepackage, 'baz3.zcml')
         logger = LoggerStub()
@@ -605,16 +607,16 @@
         fqn = _packageFile(samplepackage, 'configure.zcml')
         self._callFUT(context)
         self.assertEqual(len(context.actions), 0)
         self.assertEqual(len(context._seen_files), 1)
         self.assertIn(fqn, context._seen_files)
 
     def test_w_file_passed(self):
-        from zope.configuration.config import ConfigurationMachine
         from zope.configuration import tests
+        from zope.configuration.config import ConfigurationMachine
         context = ConfigurationMachine()
         context.package = tests
         fqn = _packageFile(tests, 'simple.zcml')
         self._callFUT(context, 'simple.zcml')
         self.assertEqual(len(context.actions), 0)
         self.assertEqual(len(context._seen_files), 1)
         self.assertIn(fqn, context._seen_files)
@@ -652,19 +654,19 @@
 class Test_includeOverrides(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.xmlconfig import includeOverrides
         return includeOverrides(*args, **kw)
 
     def test_actions_have_parents_includepath(self):
+        from zope.configuration import tests
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
-        from zope.configuration import tests
         from zope.configuration.tests import simple
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         fqp = _packageFile(tests, 'configure.zcml')
         registerCommonDirectives(context)
         before_stack = context.stack[:]
         context.package = tests
         # dummy action, path from "previous" include
         context.includepath = (fqp,)
@@ -744,17 +746,17 @@
         self.assertEqual(action['discriminator'],
                          (('x', (b'blah')), ('y', 0)))
         self.assertEqual(action['callable'], foo.data.append)
 
     def test_wo_execute_w_context(self):
         from zope.configuration import xmlconfig
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         context.package = samplepackage
         registerCommonDirectives(context)
         file_name = path("samplepackage", "configure.zcml")
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
             ret = self._callFUT('configure.zcml', context=context,
@@ -767,14 +769,15 @@
         action = context.actions[0]
         self.assertEqual(action['discriminator'],
                          (('x', (b'blah')), ('y', 0)))
         self.assertEqual(action['callable'], foo.data.append)
 
     def test_w_execute(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests.samplepackage import foo
         file_name = path("samplepackage", "configure.zcml")
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
             self._callFUT(file_name)
         self.assertEqual(len(logger.debugs), 1)
@@ -810,16 +813,16 @@
         action = context.actions[0]
         self.assertEqual(action['discriminator'],
                          (('x', (b'blah')), ('y', 0)))
         self.assertEqual(action['callable'], foo.data.append)
 
     def test_wo_execute_w_context(self):
         from zope.configuration.config import ConfigurationMachine
-        from zope.configuration.xmlconfig import registerCommonDirectives
         from zope.configuration.tests.samplepackage import foo
+        from zope.configuration.xmlconfig import registerCommonDirectives
         context = ConfigurationMachine()
         registerCommonDirectives(context)
         file_name = path("samplepackage", "configure.zcml")
         with open(file_name) as f:
             xml = f.read()
         ret = self._callFUT(xml, context=context, execute=False)
         self.assertTrue(ret is context)
@@ -846,34 +849,35 @@
         self.assertEqual(data.package, None)
         self.assertEqual(data.basepath, None)
 
 
 class XMLConfigTests(unittest.TestCase):
 
     def setUp(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def tearDown(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def _getTargetClass(self):
         from zope.configuration.xmlconfig import XMLConfig
         return XMLConfig
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def test_ctor_w_global_context_missing(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests.samplepackage import foo
         here = os.path.dirname(__file__)
         path = os.path.join(here, "samplepackage", "configure.zcml")
         logger = LoggerStub()
         xmlconfig._context = None
         with _Monkey(xmlconfig, logger=logger):
@@ -902,16 +906,16 @@
         action = xc.context.actions[0]
         self.assertEqual(action['discriminator'],
                          (('x', (b'blah')), ('y', 0)))
         self.assertEqual(action['callable'], foo.data.append)
 
     def test_ctor_w_module(self):
         from zope.configuration import xmlconfig
-        from zope.configuration.tests.samplepackage import foo
         from zope.configuration.tests import samplepackage
+        from zope.configuration.tests.samplepackage import foo
         fqn = _packageFile(samplepackage, 'configure.zcml')
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
             xc = self._makeOne("configure.zcml", samplepackage)
         self.assertEqual(len(logger.debugs), 1)
         self.assertEqual(logger.debugs[0], ('include %s', (fqn,), {}))
         self.assertEqual(len(foo.data), 0)  # no execut_actions
@@ -919,14 +923,15 @@
         action = xc.context.actions[0]
         self.assertEqual(action['discriminator'],
                          (('x', (b'blah')), ('y', 0)))
         self.assertEqual(action['callable'], foo.data.append)
 
     def test___call__(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
         fqn = _packageFile(samplepackage, 'configure.zcml')
         logger = LoggerStub()
         with _Monkey(xmlconfig, logger=logger):
             xc = self._makeOne(fqn)
@@ -945,31 +950,32 @@
         self.assertEqual(data.info.eline, 12)
         self.assertEqual(data.info.ecolumn, 29)
 
 
 class Test_xmlconfig(unittest.TestCase):
 
     def setUp(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def tearDown(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.xmlconfig import xmlconfig
         return xmlconfig(*args, **kw)
 
     def test_wo_testing_passed(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
 
         def _assertTestingFalse(func):
             def _wrapper(*args, **kw):
                 assert not kw['testing']
@@ -991,14 +997,15 @@
         self.assertEqual(data.info.line, 12)
         self.assertEqual(data.info.column, 2)
         self.assertEqual(data.info.eline, 12)
         self.assertEqual(data.info.ecolumn, 29)
 
     def test_w_testing_passed(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
 
         def _assertTestingTrue(func):
             def _wrapper(*args, **kw):
                 assert kw['testing']
@@ -1022,31 +1029,32 @@
         self.assertEqual(data.info.eline, 12)
         self.assertEqual(data.info.ecolumn, 29)
 
 
 class Test_testxmlconfig(unittest.TestCase):
 
     def setUp(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def tearDown(self):
-        from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.tests.samplepackage.foo import data
+        from zope.configuration.xmlconfig import _clearContext
         _clearContext()
         del data[:]
 
     def _callFUT(self, *args, **kw):
         from zope.configuration.xmlconfig import testxmlconfig
         return testxmlconfig(*args, **kw)
 
     def test_w_testing_passed(self):
         import os
+
         from zope.configuration import xmlconfig
         from zope.configuration.tests import samplepackage
         from zope.configuration.tests.samplepackage import foo
 
         def _assertTestingTrue(func):
             def _wrapper(*args, **kw):
                 assert kw['testing']
@@ -1067,29 +1075,29 @@
                 os.path.normpath('tests/samplepackage/configure.zcml')))
         self.assertEqual(data.info.line, 12)
         self.assertEqual(data.info.column, 2)
         self.assertEqual(data.info.eline, 12)
         self.assertEqual(data.info.ecolumn, 29)
 
 
-class FauxLocator(object):
+class FauxLocator:
     def __init__(self, file, line, column):
         self.file, self.line, self.column = file, line, column
 
     def getSystemId(self):
         return self.file
 
     def getLineNumber(self):
         return self.line
 
     def getColumnNumber(self):
         return self.column
 
 
-class FauxContext(object):
+class FauxContext:
     includepath = ()
     _features = ()
     _end_called = False
 
     def setInfo(self, info):
         self.info = info
 
@@ -1154,15 +1162,15 @@
 
 
 def _packageFile(package, filename):
     import os
     return os.path.join(os.path.dirname(package.__file__), filename)
 
 
-class _Monkey(object):
+class _Monkey:
 
     def __init__(self, module, **replacements):
         self.module = module
         self.orig = {}
         self.replacements = replacements
 
     def __enter__(self):
@@ -1176,15 +1184,15 @@
         for k in self.replacements:
             if k in self.orig:
                 setattr(self.module, k, self.orig[k])
             else:  # pragma: no cover
                 delattr(self.module, k)
 
 
-class LoggerStub(object):
+class LoggerStub:
 
     debugs = errors = warnings = infos = ()
 
     def __init__(self):
         def make_append(lst):
             return lambda msg, *args, **kwargs: lst.append((msg, args, kwargs))
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/tests/test_zopeconfigure.py` & `zope.configuration-5.0/src/zope/configuration/tests/test_zopeconfigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
     def test_ctor_wo_package(self):
         zc = self._makeOne(Context())
         self.assertEqual(zc.basepath, None)
 
     def test_ctor_w_package(self):
         import os
+
         import zope.configuration.tests as zct
         zc = self._makeOne(Context(), package=zct)
         self.assertEqual(zc.basepath, os.path.dirname(zct.__file__))
 
 
-class Context(object):
+class Context:
     basepath = None
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/xmlconfig.py` & `zope.configuration-5.0/src/zope/configuration/xmlconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,40 @@
 Note, for a detailed description of the way that conflicting
 configuration actions are resolved, see the detailed example in
 test_includeOverrides in tests/test_xmlconfig.py
 """
 __docformat__ = 'restructuredtext'
 
 import errno
-from glob import glob
-import logging
 import io
+import logging
 import os
 import sys
+from glob import glob
+from xml.sax import SAXParseException
 from xml.sax import make_parser
+from xml.sax.handler import ContentHandler
+from xml.sax.handler import feature_namespaces
 from xml.sax.xmlreader import InputSource
-from xml.sax.handler import ContentHandler, feature_namespaces
-from xml.sax import SAXParseException
 
 from zope.interface import Interface
 from zope.schema import NativeStringLine
 
 from zope.configuration.config import ConfigurationMachine
-from zope.configuration.config import defineGroupingDirective
-from zope.configuration.config import defineSimpleDirective
 from zope.configuration.config import GroupingContextDecorator
 from zope.configuration.config import GroupingStackItem
+from zope.configuration.config import defineGroupingDirective
+from zope.configuration.config import defineSimpleDirective
 from zope.configuration.config import resolveConflicts
 from zope.configuration.exceptions import ConfigurationError
 from zope.configuration.exceptions import ConfigurationWrapperError
 from zope.configuration.fields import GlobalObject
 from zope.configuration.zopeconfigure import IZopeConfigure
 from zope.configuration.zopeconfigure import ZopeConfigure
-from zope.configuration._compat import reraise
+
 
 __all__ = [
     'ParserInfo',
     'ConfigurationHandler',
     'processxmlfile',
     'openInOrPlain',
     'IInclude',
@@ -62,15 +63,15 @@
     'xmlconfig',
     'testxmlconfig',
 ]
 
 logger = logging.getLogger("config")
 
 ZCML_NAMESPACE = "http://namespaces.zope.org/zcml"
-ZCML_CONDITION = (ZCML_NAMESPACE, u"condition")
+ZCML_CONDITION = (ZCML_NAMESPACE, "condition")
 
 
 class ZopeXMLConfigurationError(ConfigurationWrapperError):
     """
     Zope XML Configuration error
 
     These errors are wrappers for other errors. They include
@@ -99,15 +100,15 @@
         ...     "info", Exception("foo.xml:12:3:Not well formed"))
         >>> print(v)
         info
             Exception: foo.xml:12:3:Not well formed
     """
 
 
-class ParserInfo(object):
+class ParserInfo:
     r"""
     Information about a directive based on parser data
 
     This includes the directive location, as well as text data
     contained in the directive.
 
     Example
@@ -135,46 +136,46 @@
             <!-- zope.configure -->
             <directives namespace="http://namespaces.zope.org/zope">
               <directive name="hook" attributes="name implementation module"
                  handler="zope.configuration.metaconfigure.hook" />
             </directives>
           </configure>
     """
-    text = u''
+    text = ''
 
     def __init__(self, file, line, column):
         self.file, self.line, self.column = file, line, column
         self.eline, self.ecolumn = line, column
 
     def end(self, line, column):
         self.eline, self.ecolumn = line, column
 
     def __repr__(self):
         if (self.line, self.column) == (self.eline, self.ecolumn):
-            return 'File "%s", line %s.%s' % (
+            return 'File "{}", line {}.{}'.format(
                 self.file, self.line, self.column)
 
-        return 'File "%s", line %s.%s-%s.%s' % (
+        return 'File "{}", line {}.{}-{}.{}'.format(
             self.file, self.line, self.column, self.eline, self.ecolumn)
 
     def __str__(self):
         if (self.line, self.column) == (self.eline, self.ecolumn):
-            return 'File "%s", line %s.%s' % (
+            return 'File "{}", line {}.{}'.format(
                 self.file, self.line, self.column)
 
         file = self.file
         if file == 'tests//sample.zcml':
             # special case for testing
             file = os.path.join(os.path.dirname(__file__),
                                 'tests', 'sample.zcml')
 
         try:
             with open(file) as f:
                 lines = f.readlines()[self.line - 1:self.eline]
-        except IOError:
+        except OSError:
             src = "  Could not read source."
         else:
             ecolumn = self.ecolumn
             if lines[-1][ecolumn:ecolumn + 2] == '</':  # pragma: no cover
                 # We're pointing to the start of an end tag. Try to find
                 # the end
                 l_ = lines[-1].find('>', ecolumn)
@@ -184,28 +185,28 @@
                 lines[-1] = lines[-1][:ecolumn + 1]
 
             column = self.column
             if lines[0][:column].strip():  # pragma: no cover
                 # Remove text before start if it's noy whitespace
                 lines[0] = lines[0][self.column:]
 
-            pad = u'  '
-            blank = u''
+            pad = '  '
+            blank = ''
             try:
                 src = blank.join([pad + line for line in lines])
             except UnicodeDecodeError:  # pragma: no cover
                 # XXX:
                 # I hope so most internation zcml will use UTF-8 as encoding
                 # otherwise this code must be made more clever
                 src = blank.join([pad + line.decode('utf-8')
                                   for line in lines])
                 # unicode won't be printable, at least on my console
                 src = src.encode('ascii', 'replace')
 
-        return "%s\n%s" % (repr(self), src)
+        return f"{repr(self)}\n{src}"
 
     def characters(self, characters):
         self.text += characters
 
 
 class ConfigurationHandler(ContentHandler):
     """
@@ -229,16 +230,15 @@
     def _handle_exception(self, ex, info):
         if self.testing:
             raise
         if isinstance(ex, ConfigurationError):
             ex.add_details(repr(info))
             raise
 
-        exc = ZopeXMLConfigurationError(info, ex)
-        reraise(exc, None, sys.exc_info()[2])
+        raise ZopeXMLConfigurationError(info, ex)
 
     def startElementNS(self, name, qname, attrs):
         if self.ignore_depth:
             self.ignore_depth += 1
             return
 
         data = {}
@@ -404,27 +404,26 @@
     src.setByteStream(file)
     parser = make_parser()
     parser.setContentHandler(ConfigurationHandler(context, testing=testing))
     parser.setFeature(feature_namespaces, True)
     try:
         parser.parse(src)
     except SAXParseException:
-        reraise(ZopeSAXParseException(file, sys.exc_info()[1]),
-                None, sys.exc_info()[2])
+        raise ZopeSAXParseException(file, sys.exc_info()[1])
 
 
 def openInOrPlain(filename):
     """
     Open a file, falling back to filename.in.
 
     If the requested file does not exist and filename.in does, fall
     back to filename.in. If opening the original filename fails for
-    any other reason, allow the failure to propogate.
+    any other reason, allow the failure to propagate.
 
-    For example, the tests/samplepackage dirextory has files:
+    For example, the tests/samplepackage directory has files:
 
         - configure.zcml
 
         - configure.zcml.in
 
         - foo.zcml.in
 
@@ -460,15 +459,15 @@
         ...     print("passed")
         ... else:
         ...     print("failed")
         passed
     """
     try:
         return open(filename)
-    except IOError as e:
+    except OSError as e:
         code, msg = e.args
         if code == errno.ENOENT:
             fn = filename + ".in"
             if os.path.exists(fn):
                 return open(fn)
         raise
 
@@ -479,26 +478,26 @@
 
     These directives allows you to include or preserve including of
     another ZCML file in the configuration. This enables you to write
     configuration files in each package and then link them together.
     """
 
     file = NativeStringLine(
-        title=u"Configuration file name",
+        title="Configuration file name",
         description=(
-            u"The name of a configuration file to be included/"
-            u"excluded, relative to the directive containing the "
-            u"including configuration file."
+            "The name of a configuration file to be included/"
+            "excluded, relative to the directive containing the "
+            "including configuration file."
         ),
         required=False,
     )
 
     files = NativeStringLine(
-        title=u"Configuration file name pattern",
-        description=u"""
+        title="Configuration file name pattern",
+        description="""
         The names of multiple configuration files to be included/excluded,
         expressed as a file-name pattern, relative to the directive
         containing the including or excluding configuration file.
         The pattern can include:
 
         - ``*`` matches 0 or more characters
 
@@ -511,16 +510,16 @@
         The file names are included in sorted order, where sorting is
         without regard to case.
         """,
         required=False,
     )
 
     package = GlobalObject(
-        title=u"Include or exclude package",
-        description=u"""
+        title="Include or exclude package",
+        description="""
         Include or exclude the named file (or configure.zcml) from the
         directory of this package.
         """,
         required=False,
     )
 
 
@@ -707,15 +706,15 @@
             pass
         else:  # pragma: no cover
             addCleanUp(_clearContext)
             del addCleanUp
     return _context
 
 
-class XMLConfig(object):
+class XMLConfig:
     """Provide high-level handling of configuration files.
 
     See examples in tests/text_xmlconfig.py
     """
 
     def __init__(self, file_name, module=None):
         context = _getContext()
```

### Comparing `zope.configuration-4.4.1/src/zope/configuration/zopeconfigure.py` & `zope.configuration-5.0/src/zope/configuration/zopeconfigure.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
 from zope.interface import Interface
 from zope.schema import BytesLine
 
 from zope.configuration.config import GroupingContextDecorator
 from zope.configuration.fields import GlobalObject
 
+
 __all__ = [
     'IZopeConfigure',
     'ZopeConfigure',
 ]
 
 
 class IZopeConfigure(Interface):
@@ -124,39 +125,39 @@
     information collected is used by subdirectives.
 
     It may seem that this directive can only be used once per file, but it can
     be applied wherever it is convenient.
     """
 
     package = GlobalObject(
-        title=u"Package",
+        title="Package",
         description=(
-            u"The package to be used for evaluating relative imports "
-            u"and file names."
+            "The package to be used for evaluating relative imports "
+            "and file names."
         ),
         required=False)
 
     i18n_domain = BytesLine(
-        title=u"Internationalization domain",
+        title="Internationalization domain",
         description=(
-            u"This is a name for the software project. It must be a "
-            u"legal file-system name as it will be used to contruct "
-            u"names for directories containing translation data. "
-            u"\n"
-            u"The domain defines a namespace for the message ids "
-            u"used by a project."
+            "This is a name for the software project. It must be a "
+            "legal file-system name as it will be used to contruct "
+            "names for directories containing translation data. "
+            "\n"
+            "The domain defines a namespace for the message ids "
+            "used by a project."
         ),
         required=False
     )
 
 
 class ZopeConfigure(GroupingContextDecorator):
     """
     The implementation of `IZopeConfigure`.
     """
 
     def __init__(self, context, **kw):
-        super(ZopeConfigure, self).__init__(context, **kw)
+        super().__init__(context, **kw)
         if 'package' in kw:
             # if we have a package, we want to also define basepath
             # so we don't acquire one
             self.basepath = os.path.dirname(self.package.__file__)
```

### Comparing `zope.configuration-4.4.1/src/zope.configuration.egg-info/PKG-INFO` & `zope.configuration-5.0/src/zope.configuration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.configuration
-Version: 4.4.1
+Version: 5.0
 Summary: Zope Configuration Markup Language (ZCML)
 Home-page: https://github.com/zopefoundation/zope.configuration
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope configuration zcml
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 ``zope.configuration``
 ======================
 
@@ -58,14 +55,22 @@
 
 
 
 
 Changes
 =======
 
+5.0 (2023-05-04)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4.1 (2022-04-07)
 ------------------
 
 - Avoid creating reference cycles through tracebacks in ``reraise`` (change
   imported from ``six``).
 
 - Add support for Python 3.9, 3.10.
@@ -325,9 +330,7 @@
 
 Before 3.4.0
 ------------
 
 This package was part of the Zope 3 distribution and did not have its own
 CHANGES.txt. For earlier changes please refer to either our subversion log or
 the CHANGES.txt of earlier Zope 3 releases.
-
-
```

### Comparing `zope.configuration-4.4.1/src/zope.configuration.egg-info/SOURCES.txt` & `zope.configuration-5.0/src/zope.configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.configuration-4.4.1/tox.ini` & `zope.configuration-5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
-    !py27-!pypy: sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
@@ -49,25 +57,23 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
-    coverage html
-    coverage report -m --fail-under=99.5
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99.5
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.configuration
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

