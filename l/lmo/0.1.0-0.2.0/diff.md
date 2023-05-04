# Comparing `tmp/lmo-0.1.0.tar.gz` & `tmp/lmo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.1.0.tar", max compression
+gzip compressed data, was "lmo-0.2.0.tar", max compression
```

## Comparing `lmo-0.1.0.tar` & `lmo-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,12 @@
--rw-r--r--   0        0        0       20 2023-04-29 15:00:30.798379 lmo-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-29 14:44:51.175342 lmo-0.1.0/lmo/__init__.py
--rw-r--r--   0        0        0      456 2023-04-29 15:01:27.823532 lmo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 lmo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.2.0/LICENSE
+-rw-r--r--   0        0        0      480 2023-05-04 08:52:01.271335 lmo-0.2.0/README.md
+-rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.2.0/lmo/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.2.0/lmo/_meta.py
+-rw-r--r--   0        0        0      128 2023-04-30 12:42:37.998900 lmo-0.2.0/lmo/_typing.py
+-rw-r--r--   0        0        0     7036 2023-05-04 02:29:29.090059 lmo-0.2.0/lmo/multivariate.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.2.0/lmo/py.typed
+-rw-r--r--   0        0        0      987 2023-05-04 01:04:36.508186 lmo-0.2.0/lmo/stats.py
+-rw-r--r--   0        0        0     5757 2023-05-04 08:31:49.091411 lmo-0.2.0/lmo/univariate.py
+-rw-r--r--   0        0        0     1482 2023-05-03 23:50:48.397361 lmo-0.2.0/lmo/weights.py
+-rw-r--r--   0        0        0     1916 2023-05-04 09:17:58.820370 lmo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 lmo-0.2.0/PKG-INFO
```

