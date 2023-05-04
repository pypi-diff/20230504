# Comparing `tmp/deepclient-0.0.1.tar.gz` & `tmp/deepclient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepclient-0.0.1.tar", last modified: Thu May  4 14:54:43 2023, max compression
+gzip compressed data, was "deepclient-1.0.0.tar", last modified: Mon Apr 18 14:48:59 2022, max compression
```

## Comparing `deepclient-0.0.1.tar` & `deepclient-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:43.885583 deepclient-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-04 14:54:43.885583 deepclient-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:43.885583 deepclient-0.0.1/deep_client/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 14:54:18.000000 deepclient-0.0.1/deep_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 14:54:18.000000 deepclient-0.0.1/deep_client/deep_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 14:54:18.000000 deepclient-0.0.1/deep_client/deep_client_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:43.885583 deepclient-0.0.1/deepclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-04 14:54:43.000000 deepclient-0.0.1/deepclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 14:54:43.000000 deepclient-0.0.1/deepclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:54:43.000000 deepclient-0.0.1/deepclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 14:54:43.000000 deepclient-0.0.1/deepclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:54:43.885583 deepclient-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-04 14:54:18.000000 deepclient-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:43.885583 deepclient-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:54:18.000000 deepclient-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 14:54:18.000000 deepclient-0.0.1/tests/test_deep_client.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.169434 deepclient-1.0.0/
+-rw-rw-rw-   0        0        0      998 2022-04-18 14:48:59.169434 deepclient-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2022-01-27 09:13:39.000000 deepclient-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.148453 deepclient-1.0.0/deepclient/
+-rw-rw-rw-   0        0        0      148 2022-04-17 05:33:45.000000 deepclient-1.0.0/deepclient/__init__.py
+-rw-rw-rw-   0        0        0     7406 2022-04-18 14:47:20.000000 deepclient-1.0.0/deepclient/client.py
+-rw-rw-rw-   0        0        0      258 2022-04-17 05:25:40.000000 deepclient-1.0.0/deepclient/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.165432 deepclient-1.0.0/deepclient.egg-info/
+-rw-rw-rw-   0        0        0      998 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-04-18 14:48:58.000000 deepclient-1.0.0/deepclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-04-18 14:48:59.169434 deepclient-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2022-04-18 14:48:37.000000 deepclient-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-18 14:48:59.168433 deepclient-1.0.0/tests/
+-rw-rw-rw-   0        0        0      103 2022-03-13 07:21:35.000000 deepclient-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      371 2022-04-17 05:12:27.000000 deepclient-1.0.0/tests/config.py
+-rw-rw-rw-   0        0        0     4332 2022-04-17 09:37:26.000000 deepclient-1.0.0/tests/test_client.py
```

