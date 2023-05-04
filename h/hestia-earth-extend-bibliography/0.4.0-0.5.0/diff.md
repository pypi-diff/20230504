# Comparing `tmp/hestia-earth-extend-bibliography-0.4.0.tar.gz` & `tmp/hestia-earth-extend-bibliography-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-extend-bibliography-0.4.0.tar", last modified: Wed Apr  5 15:07:42 2023, max compression
+gzip compressed data, was "hestia-earth-extend-bibliography-0.5.0.tar", last modified: Thu May  4 09:15:48 2023, max compression
```

## Comparing `hestia-earth-extend-bibliography-0.4.0.tar` & `hestia-earth-extend-bibliography-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.978537 hestia-earth-extend-bibliography-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-05 15:07:42.978537 hestia-earth-extend-bibliography-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.966536 hestia-earth-extend-bibliography-0.4.0/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.967536 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/
--rw-rw-rw-   0 root         (0) root         (0)    10025 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.969537 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py
--rw-rw-rw-   0 root         (0) root         (0)     2050 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.970537 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.970537 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3111 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py
--rw-rw-rw-   0 root         (0) root         (0)     4352 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.971537 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.972537 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/log.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.973537 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-05 15:07:42.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2088 2023-04-05 15:07:42.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-05 15:07:42.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-05 15:07:42.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-05 15:07:42.000000 hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-05 15:07:42.978537 hestia-earth-extend-bibliography-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1005 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.962536 hestia-earth-extend-bibliography-0.4.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.975537 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.976537 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_api/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.976537 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_sdk/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_crossref.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_mendeley.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_unpaywall.py
--rw-rw-rw-   0 root         (0) root         (0)     2159 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_wos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.977537 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_rest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_rest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_rest/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 15:07:42.977537 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_soap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_soap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-04-05 15:07:22.000000 hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_soap/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-04 09:15:48.480318 hestia-earth-extend-bibliography-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.468456 hestia-earth-extend-bibliography-0.5.0/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.469445 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/
+-rw-rw-rw-   0 root         (0) root         (0)    10025 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.471422 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4225 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.472410 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.472410 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     4376 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.473399 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.473399 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/log.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.475376 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-04 09:15:48.000000 hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-04 09:15:48.480318 hestia-earth-extend-bibliography-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.465491 hestia-earth-extend-bibliography-0.5.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.477352 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.477352 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.478341 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_crossref.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_mendeley.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_unpaywall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_wos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:48.479329 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-04 09:15:27.000000 hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/test_client.py
```

### Comparing `hestia-earth-extend-bibliography-0.4.0/LICENSE` & `hestia-earth-extend-bibliography-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/PKG-INFO` & `hestia-earth-extend-bibliography-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-extend-bibliography
-Version: 0.4.0
+Version: 0.5.0
 Summary: Hestia library to extend Bibliography Nodes with different APIs
 Home-page: https://gitlab.com/hestia-earth/hestia-data-validation
 Author: Guillaume Royer
 Author-email: guillaumeroyer.mail@gmail.com
 License: MIT
 Keywords: hestia,mendeley
 Platform: UNKNOWN
```

### Comparing `hestia-earth-extend-bibliography-0.4.0/README.md` & `hestia-earth-extend-bibliography-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/__init__.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/crossref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 import habanero
-from hestia_earth.schema import Bibliography, SourceLicense
+from hestia_earth.schema import Bibliography, SourceOriginalLicense
 
 from hestia_earth.extend_bibliography.log import logger
 from hestia_earth.extend_bibliography.utils import current_time_ms
 from .utils import (
     ORINGAL_FIELD, MAXIMUM_DISTANCE, find_closest_result, extend_bibliography, remove_empty_values,
     capitalize, update_actor_names, update_node_value
 )
@@ -28,15 +28,15 @@
     return '-'.join(['cc', suffix]).upper()
 
 
 def _parse_license(licenses: list):
     license_url = licenses[0].get('URL') if len(licenses) else None
     return None if license_url is None else (
         _extract_cc_license(license_url) if license_url.startswith('https://creativecommons.org/licenses') else
-        SourceLicense.OTHER_LICENSE.value
+        SourceOriginalLicense.OTHER_PUBLIC_LICENSE.value
     )
 
 
 def item_to_bibliography(item: dict, include_license: bool = False):
     outlet = item.get('short-container-title')
     return {
         'title': capitalize(item.get('title')[0]),
```

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_api/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/mendeley_sdk/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/unpaywall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import traceback
 import requests
 from concurrent.futures import ThreadPoolExecutor
 from random import randrange
-from hestia_earth.schema import Bibliography, SourceLicense
+from hestia_earth.schema import Bibliography, SourceOriginalLicense
 
 from hestia_earth.extend_bibliography.log import logger
 from hestia_earth.extend_bibliography.utils import current_time_ms
 from .utils import (
     ORINGAL_FIELD, MAXIMUM_DISTANCE, find_closest_result, extend_bibliography, remove_empty_values,
     capitalize, update_actor_names, update_node_value
 )
@@ -26,15 +26,18 @@
         'firstName': capitalize(author.get('given')),
         'lastName': capitalize(author.get('family'))
     })
 
 
 def _parse_license(license: str = None):
     return None if license is None else (
-        SourceLicense.OTHER_LICENSE.value if license == 'implied-oa' or license.startswith('acs-specific') else
+        SourceOriginalLicense.OTHER_PUBLIC_LICENSE.value if any([
+            license == 'implied-oa',
+            license.startswith('acs-specific')
+        ]) else
         license.upper()
     )
 
 
 def _item_to_bibliography(item: dict, include_license: bool = False):
     oa = item.get('best_oa_location', None)
     return {
```

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_rest/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/bibliography_apis/wos_soap/client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth/extend_bibliography/log.py` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth/extend_bibliography/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-extend-bibliography
-Version: 0.4.0
+Version: 0.5.0
 Summary: Hestia library to extend Bibliography Nodes with different APIs
 Home-page: https://gitlab.com/hestia-earth/hestia-data-validation
 Author: Guillaume Royer
 Author-email: guillaumeroyer.mail@gmail.com
 License: MIT
 Keywords: hestia,mendeley
 Platform: UNKNOWN
```

### Comparing `hestia-earth-extend-bibliography-0.4.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt` & `hestia-earth-extend-bibliography-0.5.0/hestia_earth_extend_bibliography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/setup.py` & `hestia-earth-extend-bibliography-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_api/test_client.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_api/test_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/mendeley_sdk/test_client.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/mendeley_sdk/test_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_crossref.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_crossref.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_mendeley.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_mendeley.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_unpaywall.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_unpaywall.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_utils.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/test_wos.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/test_wos.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_rest/test_client.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_rest/test_client.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-extend-bibliography-0.4.0/tests/bibliography_apis/wos_soap/test_client.py` & `hestia-earth-extend-bibliography-0.5.0/tests/bibliography_apis/wos_soap/test_client.py`

 * *Files identical despite different names*

