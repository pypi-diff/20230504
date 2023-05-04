# Comparing `tmp/design.plone.policy-5.0.0a4.tar.gz` & `tmp/design.plone.policy-5.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.0a4.tar", last modified: Mon Feb 20 09:44:36 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.0a5.tar", last modified: Wed Mar  1 11:08:31 2023, max compression
```

## Comparing `design.plone.policy-5.0.0a4.tar` & `design.plone.policy-5.0.0a5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.369116 design.plone.policy-5.0.0a4/
--rw-r--r--   0 lucabel    (501) staff       (20)     4656 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       73 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      670 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      107 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    17946 2023-02-20 09:44:36.369372 design.plone.policy-5.0.0a4/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)     7757 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/README.rst
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.353615 design.plone.policy-5.0.0a4/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       31 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      346 2023-02-20 09:44:36.369896 design.plone.policy-5.0.0a4/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2931 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.347595 design.plone.policy-5.0.0a4/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.353939 design.plone.policy-5.0.0a4/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.356714 design.plone.policy-5.0.0a4/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.359724 design.plone.policy-5.0.0a4/src/design/plone/policy/
--rw-r--r--   0 lucabel    (501) staff       (20)      173 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.360937 design.plone.policy-5.0.0a4/src/design/plone/policy/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)      119 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19901 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/browser/config.py
--rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/browser/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5624 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/browser/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1431 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      442 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.362232 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/design.plone.policy.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.348545 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.362521 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-r--r--   0 lucabel    (501) staff       (20)     1748 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      494 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/locales/update.sh
--rw-r--r--   0 lucabel    (501) staff       (20)      273 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.349154 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.364187 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      584 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/actions.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      175 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1032 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/metadata.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1473 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/registry.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      137 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.364469 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/to_1400/
--rw-r--r--   0 lucabel    (501) staff       (20)      237 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/to_1400/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.365026 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      268 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/uninstall/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.365510 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.366238 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      534 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      996 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)      288 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.366960 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3831 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.367656 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      513 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6582 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2342 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/sensitive.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3306 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7250 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.368897 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4288 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3762 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_initial_structure.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3860 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_search_filters_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3721 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10660 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4196 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/upgrades.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    13045 2023-02-20 09:44:35.000000 design.plone.policy-5.0.0a4/src/design/plone/policy/utils.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-02-20 09:44:36.356407 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    17946 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)     2825 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      144 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      505 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-02-20 09:44:36.000000 design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.307893 design.plone.policy-5.0.0a5/
+-rw-r--r--   0 lucabel    (501) staff       (20)     4867 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       73 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      670 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      107 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    18229 2023-03-01 11:08:31.308197 design.plone.policy-5.0.0a5/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     7757 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/README.rst
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.292265 design.plone.policy-5.0.0a5/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       31 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      367 2023-03-01 11:08:31.308839 design.plone.policy-5.0.0a5/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2919 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.285831 design.plone.policy-5.0.0a5/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.292588 design.plone.policy-5.0.0a5/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.295382 design.plone.policy-5.0.0a5/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.298086 design.plone.policy-5.0.0a5/src/design/plone/policy/
+-rw-r--r--   0 lucabel    (501) staff       (20)      173 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.299258 design.plone.policy-5.0.0a5/src/design/plone/policy/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)      119 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19901 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/browser/config.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      540 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/browser/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5622 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/browser/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1431 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      441 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.300302 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/design.plone.policy.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.287183 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.300539 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1748 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      494 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      273 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.287683 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.302281 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      584 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      175 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1027 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/metadata.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1473 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/registry.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      137 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.302504 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/to_1400/
+-rw-r--r--   0 lucabel    (501) staff       (20)      237 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/to_1400/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.303342 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      122 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      268 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/uninstall/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.303971 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.304777 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      534 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      996 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      288 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.305659 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      519 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3831 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.306403 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      513 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6581 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2342 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/sensitive.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3306 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5712 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.307648 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4287 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4324 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_initial_structure.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3858 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3720 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11068 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4462 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/upgrades.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    13045 2023-03-01 11:08:30.000000 design.plone.policy-5.0.0a5/src/design/plone/policy/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2023-03-01 11:08:31.295117 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    18229 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)     2825 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      144 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      493 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2023-03-01 11:08:31.000000 design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.0a4/CHANGES.rst` & `design.plone.policy-5.0.0a5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.0.0a5 (2023-03-01)
+--------------------
+
+- Update upgrade scripts to call design.plone.contenttypes
+  upgrade steps to version 7008
+  Install collective.feedback when install design.plone.policy
+  [lucabel]
+
+
 5.0.0a4 (2023-02-20)
 --------------------
 
 - Upgrade script to generate first and second level menu
   due to a couple of typo
   [lucabel]
```

### Comparing `design.plone.policy-5.0.0a4/DEVELOP.rst` & `design.plone.policy-5.0.0a5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/LICENSE.GPL` & `design.plone.policy-5.0.0a5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/LICENSE.rst` & `design.plone.policy-5.0.0a5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/PKG-INFO` & `design.plone.policy-5.0.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.0a4
+Version: 5.0.0a5
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -272,14 +272,23 @@
         
         - RedTurtle Technology, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
+        5.0.0a5 (2023-03-01)
+        --------------------
+        
+        - Update upgrade scripts to call design.plone.contenttypes
+          upgrade steps to version 7008
+          Install collective.feedback when install design.plone.policy
+          [lucabel]
+        
+        
         5.0.0a4 (2023-02-20)
         --------------------
         
         - Upgrade script to generate first and second level menu
           due to a couple of typo
           [lucabel]
```

### Comparing `design.plone.policy-5.0.0a4/README.rst` & `design.plone.policy-5.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/docs/conf.py` & `design.plone.policy-5.0.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/setup.py` & `design.plone.policy-5.0.0a5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.0a4",
+    version="5.0.0a5",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -58,17 +58,17 @@
         "collective.volto.formsupport[honeypot]",
         "collective.volto.secondarymenu",
         "collective.volto.socialsettings",
         "collective.volto.subsites",
         "collective.volto.subfooter",
         "eea.api.taxonomy",
         "redturtle.voltoplugin.editablefooter",
-        "rer.customersatisfaction>=1.1.0",
         "redturtle.faq",
         "redturtle.rssservice",
+        "collective.feedback",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/browser/trasparenza.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from Products.CMFCore.WorkflowCore import WorkflowException
 from Products.CMFPlone.utils import _createObjectByType
 from Products.Five.browser import BrowserView
 from uuid import uuid4
 from zope.component import queryUtility
 from zope.interface import alsoProvides
 
-
 import logging
 
 
 logger = logging.getLogger("trasparenza")
 
 
 def set_property(context, prop_name, value):
@@ -43,15 +42,14 @@
         except Exception:
             children = STRUTTURA
         alsoProvides(self.request, IDisableCSRFProtection)
         _createObjects(parent, children)
 
 
 def _createObjects(parent, children):
-
     wftool = getToolByName(parent, "portal_workflow")
 
     for new_obj in children:
         logger.info("Processing object: %s" % new_obj["id"])
 
         #            if new_obj.get('lang', '') == 'neutral':
         #                language = ''
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.0a5/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files 10% similar despite different names*

#### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/metadata.xml`

```diff
@@ -1,19 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>3000</version>
+  <version>3001</version>
   <dependencies>
     <dependency>profile-plone.restapi:default</dependency>
     <dependency>profile-design.plone.contenttypes:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-collective.volto.dropdownmenu:default</dependency>
     <dependency>profile-collective.volto.socialsettings:default</dependency>
     <dependency>profile-collective.volto.secondarymenu:default</dependency>
     <dependency>profile-collective.volto.subsites:default</dependency>
     <dependency>profile-redturtle.voltoplugin.editablefooter:default</dependency>
     <dependency>profile-collective.volto.formsupport:default</dependency>
     <dependency>profile-collective.volto.subfooter:default</dependency>
     <dependency>profile-eea.api.taxonomy:default</dependency>
-    <dependency>profile-rer.customersatisfaction:default</dependency>
     <dependency>profile-redturtle.faq:default</dependency>
+    <dependency>profile-collective.feedback:default</dependency>
   </dependencies>
 </metadata>
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/configure.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/restapi/twitter_feed/get.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/restapi/twitter_feed/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     timestamp = time() // (60 * 30 * 1)
     return "{timestamp}:{query}".format(timestamp=timestamp, query=urlencode(query))
 
 
 @implementer(IPublishTraverse)
 class TwitterFeedGet(Service):
     def reply(self):
-
         token = api.portal.get_registry_record(
             "twitter_token", interface=IDesignPlonePolicySettings
         )
         if not token:
             msg = "BEARER token not set: please set it into plone registry to be able to fetch Tweets."  # noqa
             logger.error(msg)
             self.request.response.setStatus(500)
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/testing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,71 @@
 # -*- coding: utf-8 -*-
+from design.plone.contenttypes.testing import DesignPloneContenttypesLayer
+from design.plone.contenttypes.testing import DesignPloneContenttypesRestApiLayer
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.robotframework.testing import REMOTE_LIBRARY_BUNDLE_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import quickInstallProduct
 from plone.testing import z2
-from redturtle.volto.testing import RedturtleVoltoLayer
-from redturtle.volto.testing import RedturtleVoltoRestApiLayer
-from zope.configuration import xmlconfig
 from zope.globalrequest import setRequest
 
-import collective.dexteritytextindexer
 import collective.MockMailHost
 import collective.taxonomy
-import collective.venue
 import collective.volto.cookieconsent
 import collective.volto.dropdownmenu
 import collective.volto.formsupport
 import collective.volto.secondarymenu
 import collective.volto.socialsettings
 import collective.volto.subfooter
 import collective.volto.subsites
+import collective.z3cform.datagridfield
 import design.plone.contenttypes
 import design.plone.policy
 import eea.api.taxonomy
-import plone.app.caching
 import plone.app.contentlisting
-import plone.formwidget.geolocation
-import plone.restapi
-import redturtle.bandi
 import redturtle.faq
-import redturtle.volto
 import redturtle.voltoplugin.editablefooter
-import rer.customersatisfaction
 import souper.plone
 
 
 class FauxRequest(dict):
     URL = "http://nohost"
 
 
-# TODO: dunno how to fix this
-# File "/Users/martina/progetti/docker-compose-dev/src/design.plone.policy/src/
-# design/plone/policy/setuphandlers.py", line 58, in post_install
-#     create_menu()
-#   File "/Users/martina/progetti/docker-compose-dev/src/design.plone.policy/src/
-# design/plone/policy/utils.py", line 318, in create_menu
-#     json_serialized = getMultiAdapter((x, request), ISerializeToJsonSummary)()
-#   File "/opt/buildoutcache/egg-cache/plone.restapi-8.32.4-py3.8.egg/plone/
-# restapi/serializer/summary.py", line 91, in __call__
-#     obj = IContentListingObject(self.context)
-# TypeError: ('Could not adapt', None,
-# <InterfaceClass plone.app.contentlisting.interfaces.IContentListingObject>)
-class DesignPlonePolicyLayer(RedturtleVoltoLayer):
-
-    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
-
+class DesignPlonePolicyLayer(DesignPloneContenttypesLayer):
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
 
+        super().setUpZope(app, configurationContext)
+        self.loadZCML(package=collective.z3cform.datagridfield)
+        self.loadZCML(package=design.plone.policy)
         self.loadZCML(package=collective.volto.formsupport)
-        self.loadZCML(package=collective.venue)
+        self.loadZCML(package=collective.volto.cookieconsent)
         self.loadZCML(package=collective.volto.dropdownmenu)
         self.loadZCML(package=collective.volto.secondarymenu)
         self.loadZCML(package=collective.volto.socialsettings)
         self.loadZCML(package=collective.volto.subsites)
-        self.loadZCML(package=redturtle.volto)
+        self.loadZCML(package=redturtle.voltoplugin.editablefooter)
+        self.loadZCML(package=collective.volto.subfooter)
         self.loadZCML(package=collective.taxonomy)
         self.loadZCML(package=eea.api.taxonomy)
         self.loadZCML(name="overrides.zcml", package=design.plone.contenttypes)
-        xmlconfig.file(
-            "configure.zcml",
-            design.plone.contenttypes,
-            context=configurationContext,
-        )
-        self.loadZCML(package=design.plone.policy)
-        self.loadZCML(package=plone.app.caching)
-        self.loadZCML(package=plone.formwidget.geolocation)
-        self.loadZCML(package=redturtle.bandi)
-        self.loadZCML(package=plone.restapi)
         self.loadZCML(package=plone.app.contentlisting)
-        self.loadZCML(package=redturtle.voltoplugin.editablefooter)
-        self.loadZCML(package=collective.volto.subfooter)
-        self.loadZCML(package=rer.customersatisfaction)
         self.loadZCML(package=souper.plone)
         self.loadZCML(package=redturtle.faq)
 
     def setUpPloneSite(self, portal):
         super().setUpPloneSite(portal)
         request = portal.REQUEST
         setRequest(request)
+        applyProfile(portal, "collective.z3cform.datagridfield:default")
         applyProfile(portal, "plone.app.caching:default")
         applyProfile(portal, "collective.taxonomy:default")
         applyProfile(portal, "eea.api.taxonomy:default")
         applyProfile(portal, "design.plone.policy:default")
 
 
 DESIGN_PLONE_POLICY_FIXTURE = DesignPlonePolicyLayer()
@@ -120,59 +89,48 @@
         REMOTE_LIBRARY_BUNDLE_FIXTURE,
         z2.ZSERVER_FIXTURE,
     ),
     name="DesignPlonePolicyLayer:AcceptanceTesting",
 )
 
 
-class DesignPlonePolicyRestApiLayer(RedturtleVoltoRestApiLayer):
-
+class DesignPlonePolicyRestApiLayer(DesignPloneContenttypesRestApiLayer):
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
-        super(DesignPlonePolicyRestApiLayer, self).setUpZope(app, configurationContext)
-
-        self.loadZCML(package=collective.MockMailHost)
-        self.loadZCML(package=collective.venue)
-        self.loadZCML(package=collective.volto.dropdownmenu)
-        self.loadZCML(package=redturtle.volto)
+        super().setUpZope(app, configurationContext)
+        self.loadZCML(package=collective.z3cform.datagridfield)
+        self.loadZCML(package=design.plone.policy)
         self.loadZCML(package=collective.volto.formsupport)
+        self.loadZCML(package=collective.volto.cookieconsent)
+        self.loadZCML(package=collective.volto.dropdownmenu)
         self.loadZCML(package=collective.volto.secondarymenu)
         self.loadZCML(package=collective.volto.socialsettings)
-        self.loadZCML(package=collective.volto.subfooter)
         self.loadZCML(package=collective.volto.subsites)
+        self.loadZCML(package=redturtle.voltoplugin.editablefooter)
+        self.loadZCML(package=collective.volto.subfooter)
+        self.loadZCML(package=redturtle.volto)
         self.loadZCML(package=collective.taxonomy)
         self.loadZCML(package=eea.api.taxonomy)
         self.loadZCML(name="overrides.zcml", package=design.plone.contenttypes)
-        xmlconfig.file(
-            "configure.zcml",
-            design.plone.contenttypes,
-            context=configurationContext,
-        )
         self.loadZCML(package=design.plone.policy)
-        self.loadZCML(package=plone.app.caching)
-        self.loadZCML(package=plone.formwidget.geolocation)
-        self.loadZCML(package=plone.restapi)
         self.loadZCML(package=plone.app.contentlisting)
-        self.loadZCML(package=redturtle.bandi)
         self.loadZCML(package=redturtle.faq)
-        self.loadZCML(package=redturtle.voltoplugin.editablefooter)
-        self.loadZCML(package=rer.customersatisfaction)
         self.loadZCML(package=souper.plone)
 
     def setUpPloneSite(self, portal):
         super().setUpPloneSite(portal)
         request = portal.REQUEST
         setRequest(request)
+        applyProfile(portal, "collective.z3cform.datagridfield:default")
         applyProfile(portal, "plone.app.caching:default")
-        applyProfile(portal, "collective.taxonomy:default")
-        applyProfile(portal, "eea.api.taxonomy:default")
         applyProfile(portal, "design.plone.policy:default")
         quickInstallProduct(portal, "collective.MockMailHost")
-        applyProfile(portal, "collective.MockMailHost:default")
+        applyProfile(portal, "eea.api.taxonomy:default")
+        applyProfile(portal, "collective.taxonomy:default")
 
 
 DESIGN_PLONE_POLICY_API_FIXTURE = DesignPlonePolicyRestApiLayer()
 DESIGN_PLONE_POLICY_API_INTEGRATION_TESTING = IntegrationTesting(
     bases=(DESIGN_PLONE_POLICY_API_FIXTURE,),
     name="DesignPlonePolicyRestApiLayer:Integration",
 )
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from zope.component import getUtility
 from zope.intid.interfaces import IIntIds
 
 import unittest
 
 
 class BandiSearchFiltersAPITest(unittest.TestCase):
-
     layer = DESIGN_PLONE_POLICY_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 # -*- coding: utf-8 -*-
 from design.plone.policy.testing import DESIGN_PLONE_POLICY_INTEGRATION_TESTING
 from design.plone.policy.utils import TASSONOMIA_AMMINISTRAZIONE
 from design.plone.policy.utils import TASSONOMIA_ARGOMENTI
-from design.plone.policy.utils import TASSONOMIA_DOCUMENTI
 from design.plone.policy.utils import TASSONOMIA_NEWS
 from design.plone.policy.utils import TASSONOMIA_ORGANI_GOVERNO
-from design.plone.policy.utils import TASSONOMIA_PRIMO_LIVELLO
 from design.plone.policy.utils import TASSONOMIA_SERVIZI
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from plone.i18n.normalizer.interfaces import IURLNormalizer
+from zope.component import getUtility
 
 import unittest
 
 
 # TODO: rework tests
 class TestInitialStructureCreation(unittest.TestCase):
-
     layer = DESIGN_PLONE_POLICY_INTEGRATION_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
     def normalize_ids(self, string):
-        return string.replace(" ", "-").lower()
+        return getUtility(IURLNormalizer).normalize(string)
 
     def check_initial_blocks(self, obj):
         self.assertEqual(obj.portal_type, "Document")
         self.assertEqual(len(obj.blocks.values()), 1)
         self.assertEqual(len(obj.blocks_layout["items"]), 1)
 
     def check_children_initial_blocks(self, obj):
         for child in obj.listFolderContents():
             self.check_initial_blocks(child)
 
     def test_first_level_created(self):
-        self.assertEqual(
-            [x.id for x in self.portal.getFolderContents()],
-            [self.normalize_ids(x) for x in TASSONOMIA_PRIMO_LIVELLO],
-        )
-        self.check_children_initial_blocks(self.portal)
+        no_blocks = [
+            "prenotazione-appuntamento",
+            "segnalazione-disservizio",
+            "richiesta-di-assistenza",
+            "amministrazione-trasparente",
+            "informativa-privacy",
+            "note-legali",
+            "media-policy",
+        ]
+        for child in self.portal.listFolderContents():
+            if child.id == "leggi-le-faq":
+                self.assertEqual(child.portal_type, "FaqFolder")
+            elif child.id == "dichiarazione-di-accessiblita":
+                self.assertEqual(child.portal_type, "Link")
+            else:
+                self.assertEqual(child.portal_type, "Document")
+                if child.id not in no_blocks:
+                    self.assertEqual(len(child.blocks.values()), 1)
+                    self.assertEqual(len(child.blocks_layout["items"]), 1)
 
     def test_amministrazione_section(self):
         amministrazione = self.portal["amministrazione"]
         self.assertEqual(
             amministrazione.keys(),
             [self.normalize_ids(x) for x in TASSONOMIA_AMMINISTRAZIONE],
         )
@@ -60,47 +73,38 @@
             [self.normalize_ids(x) for x in TASSONOMIA_ORGANI_GOVERNO],
         )
         for child in amministrazione["organi-di-governo"].listFolderContents():
             self.assertEqual(child.portal_type, "Document")
             self.check_initial_blocks(child)
 
     def test_servizi_section(self):
-
         servizi = self.portal["servizi"]
         self.assertEqual(
             servizi.keys(),
             [self.normalize_ids(x) for x in TASSONOMIA_SERVIZI],
         )
 
         for child in servizi.listFolderContents():
             self.assertEqual(child.portal_type, "Document")
             self.check_initial_blocks(child)
 
     def test_novita_section(self):
-
         folder = self.portal["novita"]
         self.assertEqual(
             folder.keys(), [self.normalize_ids(x) for x in TASSONOMIA_NEWS]
         )
 
         for child in folder.listFolderContents():
             self.assertEqual(child.portal_type, "Document")
             self.check_initial_blocks(child)
 
-    def test_documenti_e_dati_section(self):
-
-        folder = self.portal["documenti-e-dati"]
-        self.assertEqual(
-            folder.keys(),
-            [self.normalize_ids(x) for x in TASSONOMIA_DOCUMENTI],
-        )
-
-        self.check_children_initial_blocks(folder)
-
     def test_argomenti_section(self):
         folder = self.portal["argomenti"]
         self.assertEqual(folder.portal_type, "Document")
         self.assertEqual(
-            folder.keys(),
-            [self.normalize_ids(x) for x in TASSONOMIA_ARGOMENTI],
+            folder.keys(), [self.normalize_ids(x) for x in TASSONOMIA_ARGOMENTI]
         )
-        self.check_children_initial_blocks(folder)
+        self.assertEqual(folder.portal_type, "Document")
+        for child in folder.listFolderContents():
+            self.assertEqual(child.portal_type, "Pagina Argomento")
+            self.assertEqual(len(child.blocks.values()), 1)
+            self.assertEqual(len(child.blocks_layout["items"]), 1)
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from transaction import commit
 from zope.component import getUtility
 
 import unittest
 
 
 class SearchFiltersAPITest(unittest.TestCase):
-
     layer = DESIGN_PLONE_POLICY_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
 
@@ -57,15 +56,14 @@
     def test_endpoint_return_list_of_topics_empty_if_no_topics(self):
         response = self.api_session.get("/@search-filters").json()
 
         self.assertIn("topics", response)
         self.assertEqual(response["topics"], [])
 
     def test_endpoint_return_list_of_topics_based_on_roles(self):
-
         api.content.create(
             container=self.portal, type="Pagina Argomento", title="private topic"
         )
         public_topic = api.content.create(
             container=self.portal, type="Pagina Argomento", title="public topic"
         )
         api.content.transition(obj=public_topic, transition="publish")
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/tests/test_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,31 +73,30 @@
                     "Subsite",
                 )
             ),
         )
 
 
 class TestUninstall(unittest.TestCase):
-
     layer = DESIGN_PLONE_POLICY_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         if get_installer:
             self.installer = get_installer(self.portal, self.layer["request"])
         else:
             self.installer = api.portal.get_tool("portal_quickinstaller")
         roles_before = api.user.get_roles(TEST_USER_ID)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
-        self.installer.uninstallProducts(["design.plone.policy"])
+        self.installer.uninstall_product("design.plone.policy")
         setRoles(self.portal, TEST_USER_ID, roles_before)
 
     def test_product_uninstalled(self):
         """Test if design.plone.policy is cleanly uninstalled."""
-        self.assertFalse(self.installer.isProductInstalled("design.plone.policy"))
+        self.assertFalse(self.installer.is_product_installed("design.plone.policy"))
 
     def test_browserlayer_removed(self):
         """Test that IDesignPlonePolicyLayer is removed."""
         from design.plone.policy.interfaces import IDesignPlonePolicyLayer
         from plone.browserlayer import utils
 
         self.assertNotIn(IDesignPlonePolicyLayer, utils.registered_layers())
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/upgrades.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,7 +311,20 @@
 
 def to_3000(context):
     # run design.plone.contenttypes steps
     context.upgradeProfile(
         "profile-design.plone.contenttypes:default", dest="7001", quiet=False
     )
     update_folders_name_for_pnrr(context)
+
+
+def to_3001(context):
+    # run design.plone.contenttypes steps
+    context.upgradeProfile(
+        "profile-design.plone.contenttypes:default", dest="7008", quiet=False
+    )
+    context.runImportStepFromProfile(
+        "profile-design.plone.contenttypes:default",
+        "plone.app.registry",
+        run_dependencies=False,
+    )
+    installOrReinstallProduct(api.portal.get(), "collective.feedback")
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.0a5/src/design/plone/policy/upgrades.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -147,8 +147,18 @@
       destination="3000"
       >
     <genericsetup:upgradeStep
         title="To PNRR version"
         handler=".upgrades.to_3000"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="design.plone.policy:default"
+      source="3000"
+      destination="3001"
+      >
+    <genericsetup:upgradeStep
+        title="To PNRR version"
+        handler=".upgrades.to_3001"
+        />
+  </genericsetup:upgradeSteps>
 </configure>
```

### Comparing `design.plone.policy-5.0.0a4/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.0a5/src/design/plone/policy/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/PKG-INFO` & `design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.0a4
+Version: 5.0.0a5
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -272,14 +272,23 @@
         
         - RedTurtle Technology, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
+        5.0.0a5 (2023-03-01)
+        --------------------
+        
+        - Update upgrade scripts to call design.plone.contenttypes
+          upgrade steps to version 7008
+          Install collective.feedback when install design.plone.policy
+          [lucabel]
+        
+        
         5.0.0a4 (2023-02-20)
         --------------------
         
         - Upgrade script to generate first and second level menu
           due to a couple of typo
           [lucabel]
```

### Comparing `design.plone.policy-5.0.0a4/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.0a5/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

