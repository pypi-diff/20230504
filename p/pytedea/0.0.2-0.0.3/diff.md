# Comparing `tmp/pytedea-0.0.2.tar.gz` & `tmp/pytedea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedea-0.0.2.tar", last modified: Wed May  3 15:40:42 2023, max compression
+gzip compressed data, was "pytedea-0.0.3.tar", last modified: Thu May  4 14:31:56 2023, max compression
```

## Comparing `pytedea-0.0.2.tar` & `pytedea-0.0.3.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.985329 pytedea-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-03 15:40:24.000000 pytedea-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 15:40:24.000000 pytedea-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-03 15:40:42.985329 pytedea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 15:40:24.000000 pytedea-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.977330 pytedea-0.0.2/pytedea/
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DDFt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23332 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DEA.py
--rw-r--r--   0 runner    (1001) docker     (123)   139489 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/DEAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/HYPER.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/NDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/pytedea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.985329 pytedea-0.0.2/pytedea/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/CQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/sweet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCNLSxZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-03 15:40:24.000000 pytedea-0.0.2/pytedea/utils/weakCQERxZG2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:40:42.981330 pytedea-0.0.2/pytedea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:40:42.000000 pytedea-0.0.2/pytedea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 15:40:24.000000 pytedea-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-03 15:40:42.985329 pytedea-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-03 15:40:24.000000 pytedea-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.983391 pytedea-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 14:31:38.000000 pytedea-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 14:31:38.000000 pytedea-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-04 14:31:56.983391 pytedea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 14:31:38.000000 pytedea-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.975391 pytedea-0.0.3/pytedea/
+-rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23332 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138273 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/HYPER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/HYPERt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/NDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/pytedea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.983391 pytedea-0.0.3/pytedea/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxZG2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.975391 pytedea-0.0.3/pytedea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:31:38.000000 pytedea-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 14:31:56.983391 pytedea-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 14:31:38.000000 pytedea-0.0.3/setup.py
```

### Comparing `pytedea-0.0.2/LICENSE` & `pytedea-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/PKG-INFO` & `pytedea-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.2/pytedea/DDF.py` & `pytedea-0.0.3/pytedea/DDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/DDFt.py` & `pytedea-0.0.3/pytedea/DDFt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/DEA.py` & `pytedea-0.0.3/pytedea/DEA.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/DEAt.py` & `pytedea-0.0.3/pytedea/DEAt.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         self.rts = rts
         self.outputvars, self.inputvars ,self.y, self.x,self.yref, self.xref= tools.assert_valid_deat(sent,data,baseindex,refindex )
 
         self.xcol = self.x.columns
         self.ycol = self.y.columns
         if orient in [ORIENT_IO, ORIENT_OO, ORIENT_HYPERYX]:
             self.orient = orient
+            self.xindexs = None
+            self.yindexs = None
         else:
             self.orient = None
             if orient in self.xcol:
                 self.xindexs = list(self.xcol).index(orient)
                 self.yindexs = None
             elif orient in self.ycol:
                 self.yindexs = list(self.ycol).index(orient)
@@ -64,19 +66,16 @@
             # Setup the objective function and constraints
             if self.orient == ORIENT_IO:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=minimize, doc='objective function')
             elif self.orient == ORIENT_OO:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=maximize, doc='objective function')
-            elif self.orient == ORIENT_HYPERYX:
-                self.__model__.objective = Objective(
-                    rule=self.__objective_rule(), sense=minimize, doc='objective function')
-            elif type(self.orient) == type(None):
-                if type(self.yindexs)==type(None):
+            else:
+                if type(self.xindexs)!=type(None):
                     self.__model__.objective = Objective(
                         rule=self.__objective_rule(), sense=minimize, doc='objective function')
                 else:
                     self.__model__.objective = Objective(
                         rule=self.__objective_rule(), sense=maximize, doc='objective function')
 
             self.__model__.input = Constraint(
@@ -98,45 +97,40 @@
 
 
         # # Optimize model
 
 
     def __objective_rule(self):
         """Return the proper objective function"""
-        if self.orient != ORIENT_HYPERYX:
-            def objective_rule(model):
-                return model.theta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
-        else:
-            def objective_rule(model):
-                return model.delta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
+        def objective_rule(model):
+            return model.theta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
         return objective_rule
 
 
     def __input_rule(self):
         """Return the proper input constraint"""
         if self.orient == ORIENT_OO:
             def input_rule(model, k):
-                return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= self.x.loc[self.I0,self.xcol[k]]
-        elif self.orient == ORIENT_IO:
-            def input_rule(model, k):
-                return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                    model.theta * self.x.loc[self.I0,self.xcol[k]]
-        elif self.orient == ORIENT_HYPERYX:
-            def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                    model.delta * self.x.loc[self.I0,self.xcol[k]]
-        elif type(self.yindexs) == type(None):
+                    self.x.loc[self.I0,self.xcol[k]]
+        elif self.orient == ORIENT_IO:
             def input_rule(model, k):
-                if k != self.xindexs:
-                    return Constraint.Skip
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                     model.theta * self.x.loc[self.I0,self.xcol[k]]
-        elif type(self.xindexs) == type(None):
-            def input_rule(model, k):
-                return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= self.x.loc[self.I0,self.xcol[k]]
+
+        else:
+            if type(self.xindexs)!=type(None):
+                def input_rule(model, k):
+                    if k != self.xindexs:
+                        return Constraint.Skip
+                    return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
+                        model.theta * self.x.loc[self.I0,self.xcol[k]]
+            else:
+                def input_rule(model, k):
+                    return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= self.x.loc[self.I0,self.xcol[k]]
 
         return input_rule
 
 
 
     def __output_rule(self):
         """Return the proper output constraint"""
@@ -144,63 +138,52 @@
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >=model.theta * self.y.loc[self.I0,self.ycol[l]]
         elif self.orient == ORIENT_IO:
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >= self.y.loc[self.I0,self.ycol[l]]
-        elif self.orient == ORIENT_HYPERYX:
-            def output_rule(model, l):
-                return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
-                    >= self.y.loc[self.I0,self.ycol[l]]
-        elif type(self.yindexs) == type(None):
-            def output_rule(model, l):
-                return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
-                    >= self.y.loc[self.I0,self.ycol[l]]
-        elif type(self.xindexs) == type(None):
-            def output_rule(model, l):
-                if l != self.yindexs:
-                    return Constraint.Skip
-                return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
-                    >=model.theta * self.y.loc[self.I0,self.ycol[l]]
+
+        else:
+            if type(self.yindexs)!=type(None):
+                def output_rule(model, l):
+                    if l != self.yindexs:
+                        return Constraint.Skip
+                    return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
+                        >= model.theta * self.y.loc[self.I0,self.ycol[l]]
+            else:
+                def output_rule(model, l):
+                    return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
+                        >= self.y.loc[self.I0,self.ycol[l]]
 
         return output_rule
 
     def __vrs_rule(self):
-        if self.orient != ORIENT_HYPERYX:
-            def vrs_rule(model):
-                return sum(model.lamda[ i2] for i2 in model.I2) == 1
-        else:
-            def vrs_rule(model):
-                return sum(model.lamda[ i2] for i2 in model.I2) == model.theta[0] *1
+        def vrs_rule(model):
+            return sum(model.lamda[i2] for i2 in model.I2) == 1
         return vrs_rule
 
     def optimize(self,  solver=OPT_DEFAULT):
         """Optimize the function by requested method
 
         Args:
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
         """
         # TODO(error/warning handling): Check problem status after optimization
 
         data2,lamda = pd.DataFrame(),{}
         for ind, problem in self.__modeldict.items():
             _, data2.loc[ind,"optimization_status"] = tools.optimize_model2(problem, ind, solver)
             data2.loc[ind,"theta"] = np.asarray(list(problem.theta[:].value))
-            lamda[ind] = np.asarray(list(problem.lamda[:].value))
 
-        lamda2 =pd.DataFrame(lamda).T
-        lamda2.columns = lamda2.columns.map(lambda x : "lamda"+ str(x) )
-        # data3 = pd.concat([data2,lamda2],axis=1)
-        data3 = data2
         if self.orient==ORIENT_OO:
-            data3["te"] = 1/  data3["theta"]
+            data2["te"] = 1/  data2["theta"]
         else:
-            data3["te"] = data3["theta"]
-        return data3
+            data2["te"] = data2["theta"]
+        return data2
 
     def info(self, dmu = "all"):
         """Show the infomation of the lp model
 
         Args:
             dmu (string): The solver chosen for optimization. Default is "all".
         """
```

### Comparing `pytedea-0.0.2/pytedea/HYPER.py` & `pytedea-0.0.3/pytedea/HYPER.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, data,sent = "inputvar=outputvar",  \
                  orient=ORIENT_HYPERYB, rts=RTS_VRS, baseindex=None,refindex=None):
         """DEA: Directional distance function
 
         Args:
             data (pandas.DataFrame): input pandas.
             sent (str): inputvars=outputvars[: unoutputvars]. e.g.: "K L= Y:CO2"
-            orient(str): ORIENT_IO ORIENT_OO ORIENT_HYPER, or choose some variables in sent
+            orient(str): ORIENT_HYPERYB ORIENT_HYPERYX , or choose some variables in sent,eg:L=Y, Y:CO2
             rts (String): RTS_VRS (variable returns to scale) or RTS_CRS (constant returns to scale)
             baseindex (String, optional): estimate index. Defaults to None. e.g.: "Year=[2010]"
             refindex (String, optional): reference index. Defaults to None. e.g.: "Year=[2010]"
         """
         # Initialize DEA model
 
         self.rts = rts
@@ -69,17 +69,17 @@
             self.__model__.I2 = Set(initialize=  self.xref.index)       ## I2 是 参考决策单元的数量
 
             self.__model__.K = Set(initialize=range(len(self.x.iloc[0])))   ## K 是投入个数
             self.__model__.L = Set(initialize=range(len(self.y.iloc[0])))   ## L 是产出个数 被评价单元和参考单元的K，L一样
             self.__model__.J = Set(initialize=range(len(self.b.iloc[0]))) ## J 是非期望产出个数 被评价单元和参考单元的K，L一样
 
             # Initialize variable
-            self.__model__.beta = Var(Set(initialize=range(1)),bounds=(0, 1), doc='efficiency')
-            self.__model__.delta = Var(Set(initialize=range(1)),bounds=(None, None), \
-                                       doc='efficiency**2 or efficiency*theta')
+            self.__model__.gamma = Var(Set(initialize=range(1)),bounds=(0, 1), doc='1/output increase(1/eta)')
+            self.__model__.delta = Var(Set(initialize=range(1)),bounds=(0, 1), \
+                                       doc='bad decrease/output increase(lambda/eta)')
 
             self.__model__.lamda = Var(self.__model__.I2, bounds=(0.0, None), doc='intensity variables')
 
             # Setup the objective function and constraints
             self.__model__.objective = Objective(
                 rule=self.__objective_rule(), sense=minimize, doc='objective function')
 
@@ -120,26 +120,26 @@
         if (self.orient == ORIENT_HYPERYX) :
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                     model.delta * self.x.loc[self.I0,self.xcol[k]]
         elif (self.orient == ORIENT_HYPERYB):
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                    model.beta * self.x.loc[self.I0,self.xcol[k]]
+                    model.gamma * self.x.loc[self.I0,self.xcol[k]]
         else:
             if type(self.xindexs) != type(None):
                 def input_rule(model, k):
                     if k != self.xindexs:
                         return Constraint.Skip
                     return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                         model.delta * self.x.loc[self.I0,self.xcol[k]]
             else:
                 def input_rule(model, k):
                     return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                         model.beta * self.x.loc[self.I0,self.xcol[k]]
+                         model.gamma * self.x.loc[self.I0,self.xcol[k]]
         return input_rule
 
     def __output_rule(self):
         """Return the proper output constraint"""
         def output_rule(model, l):
             return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                 >= self.y.loc[self.I0,self.ycol[l]]
@@ -150,39 +150,39 @@
         if (self.orient == ORIENT_HYPERYB):
             def undesirable_output_rule(model, j):
                 return sum(model.lamda[i2] * self.bref.loc[i2, self.bcol[j]] for i2 in model.I2) \
                     == model.delta * self.b.loc[self.I0, self.bcol[j]]
         elif (self.orient == ORIENT_HYPERYX):
             def undesirable_output_rule(model, j):
                 return sum(model.lamda[i2] * self.bref.loc[i2, self.bcol[j]] for i2 in model.I2) \
-                    == model.beta * self.b.loc[self.I0, self.bcol[j]]
+                    == model.gamma * self.b.loc[self.I0, self.bcol[j]]
         else:
             if type(self.bindexs) != type(None):
                 def undesirable_output_rule(model, j):
                     if j != self.bindexs:
                         return Constraint.Skip
                     return sum(model.lamda[i2] * self.bref.loc[i2, self.bcol[j]] for i2 in model.I2) \
                         == model.delta * self.b.loc[self.I0, self.bcol[j]]
             else:
                 def undesirable_output_rule(model, j):
                     return sum(model.lamda[i2] * self.bref.loc[i2, self.bcol[j]] for i2 in model.I2) \
-                        == model.beta * self.b.loc[self.I0, self.bcol[j]]
+                        == model.gamma * self.b.loc[self.I0, self.bcol[j]]
         return undesirable_output_rule
 
     def __vrs_rule(self):
         if (self.orient == ORIENT_HYPERYX) :
             def vrs_rule(model):
                 return sum(model.lamda[ i2] for i2 in model.I2) == model.delta[0] *1
         elif (self.orient == ORIENT_HYPERYB) :
             def vrs_rule(model):
-                return sum(model.lamda[ i2] for i2 in model.I2) == model.beta[0] *1
+                return sum(model.lamda[ i2] for i2 in model.I2) == model.gamma[0] *1
         else:
             if type(self.bindexs) != type(None):
                 def vrs_rule(model):
-                    return sum(model.lamda[i2] for i2 in model.I2) == model.beta[0] * 1
+                    return sum(model.lamda[i2] for i2 in model.I2) == model.gamma[0] * 1
             else:
                 def vrs_rule(model):
                     return sum(model.lamda[i2] for i2 in model.I2) == model.delta[0] * 1
         return vrs_rule
 
     def optimize(self,  solver=OPT_DEFAULT):
         """Optimize the function by requested method
@@ -191,19 +191,19 @@
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
         """
         # TODO(error/warning handling): Check problem status after optimization
         data2 = pd.DataFrame()
         for ind, problem in self.__modeldict.items():
             _, data2.loc[ind,"optimization_status"] = tools.optimize_model2(problem, ind, solver)
             data2.loc[ind, "delta"] = np.asarray(list(problem.delta[:].value))
-            data2.loc[ind, "beta"] = np.asarray(list(problem.beta[:].value))
+            data2.loc[ind, "gamma"] = np.asarray(list(problem.gamma[:].value))
 
 
-        data2["lambda:bad decrease"] = data2["delta"]/data2["beta"]
-        data2["eta:good increase"] = 1/data2["beta"]
+        data2["lambda:bad decrease"] = data2["delta"]/data2["gamma"]
+        data2["eta:good increase"] = 1/data2["gamma"]
 
 
         return data2
 
     def info(self, dmu = "all"):
         """Show the infomation of the lp model
```

### Comparing `pytedea-0.0.2/pytedea/NDDF.py` & `pytedea-0.0.3/pytedea/NDDF.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                     return -1* sum(model.phi[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2
                         ) + self.gy[l]*self.y.loc[self.I0,self.ycol[l]]*model.betay[l] <= \
                         -1*self.y.loc[self.I0,self.ycol[l]]
             else:
                 raise ValueError("Undefined model parameters.")
         elif self.rts == RTS_CRS:
             def output_rule(model, l):
-                return -1 * sum(model.phi[i2] * self.yref.loc[i2, self.ycol[l]] for i2 in model.I2
+                return -1 * sum(model.lamda[i2] * self.yref.loc[i2, self.ycol[l]] for i2 in model.I2
                                 ) + self.gy[l] * self.y.loc[self.I0, self.ycol[l]] * model.betay[l] <= \
                     -1 * self.y.loc[self.I0, self.ycol[l]]
         else:
             raise ValueError("Undefined model parameters.")
         return output_rule
 
     def __undesirable_output_rule(self):
@@ -244,34 +244,39 @@
         # TODO(error/warning handling): Check problem status after optimization
         if self.rts==RTS_VRS and self.emf==EMF_SAME:
             data2, obj, betax,betax2,theta, betay, betab = pd.DataFrame(), {}, {}, {}, {},{},{}
             for ind, problem in self.__modeldict.items():
                 _, data2.loc[ind, "optimization_status"] = tools.optimize_model2(problem, ind, solver)
 
                 obj[ind] = problem.objective()
-                betax[ind] = np.asarray(list(problem.betax2[:].value))/np.asarray(list(problem.theta[:].value))
-                betax2[ind] = np.asarray(list(problem.betax2[:].value))
+                if abs(np.asarray(self.gx).sum()) >= 1:
+                    betax[ind] = np.asarray(list(problem.betax2[:].value))/np.asarray(list(problem.theta[:].value))
+                    betax2[ind] = np.asarray(list(problem.betax2[:].value))
+                else:
+                    betax[ind] = np.asarray(list(problem.betax[:].value))
                 theta[ind] = np.asarray(list(problem.theta[:].value))
                 betay[ind] = np.asarray(list(problem.betay[:].value))
                 betab[ind] = np.asarray(list(problem.betab[:].value))
 
             obj = pd.DataFrame(obj, index=["obj"]).T
             betax = pd.DataFrame(betax).T
-            betax.columns = betax.columns.map(lambda x: "Input" + str(x) + "'s slack")
-            betax2 = pd.DataFrame(betax2).T
-            betax2.columns = betax2.columns.map(lambda x: "Input" + str(x) + "'s slack2")
+            betax.columns = betax.columns.map(lambda x: "Input" + str(x) + "'s ratio")
+            if abs(np.asarray(self.gx).sum()) >= 1:
+                betax2 = pd.DataFrame(betax2).T
+                betax2.columns = betax2.columns.map(lambda x: "Input" + str(x) + "'s ratio2")
             theta = pd.DataFrame(theta).T
             theta.columns = theta.columns.map(lambda x: "theta")
             betay = pd.DataFrame(betay).T
-            betay.columns = betay.columns.map(lambda y: "Output" + str(y) + "'s slack")
-            beta = pd.concat([betax, betax2], axis=1)
-            beta = pd.concat([beta, theta], axis=1)
+            betay.columns = betay.columns.map(lambda y: "Output" + str(y) + "'s ratio")
+            beta = pd.concat([betax,theta], axis=1)
+            if abs(np.asarray(self.gx).sum()) >= 1:
+                beta = pd.concat([beta, betax2], axis=1)
             beta = pd.concat([beta, betay], axis=1)
             betab = pd.DataFrame(betab).T
-            betab.columns = betab.columns.map(lambda b: "Undesirable Output" + str(b) + "'s slack")
+            betab.columns = betab.columns.map(lambda b: "Undesirable Output" + str(b) + "'s ratio")
             beta = pd.concat([beta, betab], axis=1)
 
             dropcol = []
             for colnum, g in enumerate(
                 self.gx + self.gy + self.gb if type(self.b) != type(None) else self.gx + self.gy):
                 # print(g)
                 if g == 0:
@@ -291,20 +296,20 @@
                 obj[ind]= problem.objective()
                 betax[ind]=np.asarray(list(problem.betax[:].value))
                 betay[ind]=np.asarray(list(problem.betay[:].value))
                 betab[ind]=np.asarray(list(problem.betab[:].value))
 
             obj = pd.DataFrame(obj,index=["obj"]).T
             betax = pd.DataFrame(betax).T
-            betax.columns = betax.columns.map(lambda x : "Input"+ str(x)+"'s slack" )
+            betax.columns = betax.columns.map(lambda x : "Input"+ str(x)+"'s ratio" )
             betay = pd.DataFrame(betay).T
-            betay.columns = betay.columns.map(lambda y : "Output"+ str(y)+"'s slack" )
+            betay.columns = betay.columns.map(lambda y : "Output"+ str(y)+"'s ratio" )
             beta = pd.concat([betax,betay],axis=1)
             betab = pd.DataFrame(betab).T
-            betab.columns = betab.columns.map(lambda b : "Undesirable Output"+ str(b)+"'s slack" )
+            betab.columns = betab.columns.map(lambda b : "Undesirable Output"+ str(b)+"'s ratio" )
             beta = pd.concat([beta,betab],axis=1)
 
             dropcol=[]
             for colnum,g in enumerate(self.gx+self.gy+self.gb if type(self.b) != type(None) else self.gx+self.gy):
                 # print(g)
                 if g==0:
                     dropcol.append(beta.columns[colnum])
```

### Comparing `pytedea-0.0.2/pytedea/__init__.py` & `pytedea-0.0.3/pytedea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """advancehs"""
 __email__ = '1019753743@qq.com'
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 from . import DEAt
 from . import DDFt
 from . import DEA
 from . import DDF
 from . import HYPER
 # from . import CQER
```

### Comparing `pytedea-0.0.2/pytedea/constant.py` & `pytedea-0.0.3/pytedea/constant.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSDDFG1.py` & `pytedea-0.0.3/pytedea/utils/CNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSDDFG2.py` & `pytedea-0.0.3/pytedea/utils/CNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSDDFZG1.py` & `pytedea-0.0.3/pytedea/utils/CNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSDDFZG2.py` & `pytedea-0.0.3/pytedea/utils/CNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSG1.py` & `pytedea-0.0.3/pytedea/utils/CNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSG2.py` & `pytedea-0.0.3/pytedea/utils/CNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSZG1.py` & `pytedea-0.0.3/pytedea/utils/CNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CNLSZG2.py` & `pytedea-0.0.3/pytedea/utils/CNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERDDFG1.py` & `pytedea-0.0.3/pytedea/utils/CQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERDDFG2.py` & `pytedea-0.0.3/pytedea/utils/CQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERDDFZG1.py` & `pytedea-0.0.3/pytedea/utils/CQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERDDFZG2.py` & `pytedea-0.0.3/pytedea/utils/CQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERG1.py` & `pytedea-0.0.3/pytedea/utils/CQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERG2.py` & `pytedea-0.0.3/pytedea/utils/CQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERZG1.py` & `pytedea-0.0.3/pytedea/utils/CQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/CQERZG2.py` & `pytedea-0.0.3/pytedea/utils/CQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/interpolation.py` & `pytedea-0.0.3/pytedea/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/sweet.py` & `pytedea-0.0.3/pytedea/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/tools.py` & `pytedea-0.0.3/pytedea/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSDDFG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSDDFG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSDDFZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSbG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSbG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSbZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSbZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSxG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSxG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSxZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCNLSxZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCNLSxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERDDFG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERDDFG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERDDFZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERDDFZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERbG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERbG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERbZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERbZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERxG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERxG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERxZG1.py` & `pytedea-0.0.3/pytedea/utils/weakCQERxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea/utils/weakCQERxZG2.py` & `pytedea-0.0.3/pytedea/utils/weakCQERxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.2/pytedea.egg-info/PKG-INFO` & `pytedea-0.0.3/pytedea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.2/pytedea.egg-info/SOURCES.txt` & `pytedea-0.0.3/pytedea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 pytedea/DDF.py
 pytedea/DDFt.py
 pytedea/DEA.py
 pytedea/DEAt.py
 pytedea/HYPER.py
+pytedea/HYPERt.py
 pytedea/NDDF.py
 pytedea/__init__.py
 pytedea/constant.py
 pytedea/pytedea.py
 pytedea.egg-info/PKG-INFO
 pytedea.egg-info/SOURCES.txt
 pytedea.egg-info/dependency_links.txt
```

### Comparing `pytedea-0.0.2/setup.py` & `pytedea-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='pytedea',
     name='pytedea',
     packages=find_packages(include=['pytedea', 'pytedea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/advancehs/pytedea',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

