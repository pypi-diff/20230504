# Comparing `tmp/nobuco-0.4.3.tar.gz` & `tmp/nobuco-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.3.tar", last modified: Mon May  1 14:07:08 2023, max compression
+gzip compressed data, was "nobuco-0.4.4.tar", last modified: Thu May  4 09:30:16 2023, max compression
```

## Comparing `nobuco-0.4.3.tar` & `nobuco-0.4.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.183214 nobuco-0.4.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-05-01 14:07:08.183214 nobuco-0.4.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20054 2023-04-25 18:07:04.000000 nobuco-0.4.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.175214 nobuco-0.4.3/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.3/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.179214 nobuco-0.4.3/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.179214 nobuco-0.4.3/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.179214 nobuco-0.4.3/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.179214 nobuco-0.4.3/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.183214 nobuco-0.4.3/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.3/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10661 2023-05-01 14:06:24.000000 nobuco-0.4.3/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-01 14:05:35.000000 nobuco-0.4.3/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10637 2023-05-01 11:14:44.000000 nobuco-0.4.3/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.183214 nobuco-0.4.3/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.183214 nobuco-0.4.3/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.3/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 14:07:08.179214 nobuco-0.4.3/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-05-01 14:07:08.000000 nobuco-0.4.3/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-01 14:07:08.000000 nobuco-0.4.3/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-01 14:07:08.000000 nobuco-0.4.3/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-01 14:07:08.000000 nobuco-0.4.3/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-01 14:07:08.000000 nobuco-0.4.3/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-01 14:06:24.000000 nobuco-0.4.3/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-01 14:07:08.183214 nobuco-0.4.3/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.513416 nobuco-0.4.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22073 2023-05-04 09:30:16.513416 nobuco-0.4.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20239 2023-05-04 09:21:44.000000 nobuco-0.4.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.505416 nobuco-0.4.4/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.4/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.505416 nobuco-0.4.4/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.505416 nobuco-0.4.4/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.509416 nobuco-0.4.4/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.509416 nobuco-0.4.4/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.513416 nobuco-0.4.4/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.4/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.4/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.4/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10661 2023-05-01 14:06:24.000000 nobuco-0.4.4/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-01 14:05:35.000000 nobuco-0.4.4/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10637 2023-05-01 11:14:44.000000 nobuco-0.4.4/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.513416 nobuco-0.4.4/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.513416 nobuco-0.4.4/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.4/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:30:16.505416 nobuco-0.4.4/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22073 2023-05-04 09:30:16.000000 nobuco-0.4.4/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-04 09:30:16.000000 nobuco-0.4.4/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-04 09:30:16.000000 nobuco-0.4.4/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-04 09:30:16.000000 nobuco-0.4.4/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-04 09:30:16.000000 nobuco-0.4.4/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-04 09:30:02.000000 nobuco-0.4.4/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-04 09:30:16.513416 nobuco-0.4.4/setup.cfg
```

### Comparing `nobuco-0.4.3/LICENSE` & `nobuco-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/PKG-INFO` & `nobuco-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.3
+Version: 0.4.4
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,16 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
+<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
```

### Comparing `nobuco-0.4.3/README.md` & `nobuco-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
+<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
```

### Comparing `nobuco-0.4.3/nobuco/__init__.py` & `nobuco-0.4.4/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/commons.py` & `nobuco-0.4.4/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/convert.py` & `nobuco-0.4.4/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/converters/channel_ordering.py` & `nobuco-0.4.4/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/converters/node_converter.py` & `nobuco-0.4.4/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/converters/tensor.py` & `nobuco-0.4.4/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/converters/type_cast.py` & `nobuco-0.4.4/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/converters/validation.py` & `nobuco-0.4.4/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/entity/keras.py` & `nobuco-0.4.4/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/entity/pytorch.py` & `nobuco-0.4.4/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/funcs.py` & `nobuco-0.4.4/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/layers/channel_order.py` & `nobuco-0.4.4/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/layers/container.py` & `nobuco-0.4.4/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/layers/weight.py` & `nobuco-0.4.4/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/locate/link.py` & `nobuco-0.4.4/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/locate/locate.py` & `nobuco-0.4.4/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/activation.py` & `nobuco-0.4.4/nobuco/node_converters/linear.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,133 @@
+from numbers import Number
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
+from nobuco.converters.tensor import dim_pytorch2keras
+from nobuco.converters.channel_ordering import get_channel_order
 from torch import Tensor
-from torch.types import _int, _bool, Number, _dtype, _size
 
 import tensorflow as tf
 from tensorflow import keras
 import torch
 import torch.nn.functional as F
 from torch import nn
 
+import numpy as np
+
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
-from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
-from nobuco.converters.tensor import dim_pytorch2keras
 
 
-def hard_sigmoid_pytorch_compatible(x):
-  x = tf.clip_by_value(x/6 + 1/2, clip_value_min=0, clip_value_max=1)
-  return x
+@converter(nn.Linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_Linear(self, input: Tensor):
+    out_filters, in_filters = self.weight.shape
+    weights = self.weight.detach().numpy()
+    weights = weights.transpose(1, 0)
 
+    biases = self.bias
+    if biases is not None:
+        biases = self.bias.detach().numpy()
+        params = [weights, biases]
+    else:
+        params = [weights]
+    return keras.layers.Dense(out_filters, weights=params)
 
-def hard_swish_pytorch_compatible(x):
-  x = x * hard_sigmoid_pytorch_compatible(x)
-  return x
 
+@converter(torch.nn.functional.linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_linear(input, weight, bias, out=None):
+    out_filters, in_filters = weight.shape
+    weights = weight.detach().numpy()
+    weights = weights.transpose(1, 0)
 
-def hard_tanh_pytorch_compatible(x, min_val, max_val):
-  x = tf.clip_by_value(x, clip_value_min=min_val, clip_value_max=max_val)
-  return x
+    if bias is not None:
+        biases = bias.detach().numpy()
+        params = [weights, biases]
+    else:
+        params = [weights]
 
+    layer = keras.layers.Dense(out_filters, weights=params)
 
-@converter(torch.sigmoid, torch.Tensor.sigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_sigmoid(input: Tensor, *, out: Optional[Tensor]=None):
-    def func(input, *, out=None):
-        return keras.layers.Activation(keras.activations.sigmoid)(input)
+    def func(input, weight, bias, out=None):
+        return layer(input)
     return func
 
 
-@converter(torch.tanh, torch.Tensor.tanh, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_tanh(input: Tensor, *, out: Optional[Tensor]=None):
-    def func(input: Tensor, *, out=None):
-        return keras.layers.Activation(keras.activations.tanh)(input)
+@converter(torch.matmul, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_matmul(input: Tensor, other: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, other, *, out=None):
+        return tf.linalg.matmul(input, other)
     return func
 
 
-@converter(nn.ReLU, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_ReLU(self, input: Tensor):
-    return keras.layers.ReLU()
-
-
-@converter(F.relu, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_relu(input: Tensor, inplace: bool = False):
-    def func(input, inplace=False):
-        return tf.nn.relu(input)
+@converter(torch.Tensor.matmul, torch.Tensor.__matmul__, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_matmul(self, tensor2):
+    def func(self, tensor2):
+        return tf.linalg.matmul(self, tensor2)
     return func
 
 
-@converter(torch.relu_, torch.Tensor.relu_, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_relu_(input: Tensor):
-    def func(input):
-        return tf.nn.relu(input)
+@converter(torch.dot, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_dot(input: Tensor, tensor: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, tensor, *, out=None):
+        return tf.linalg.tensordot(input, tensor, axes=1)
     return func
 
 
-@converter(nn.LeakyReLU, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_LeakyRelu(self, input: Tensor):
-    return keras.layers.LeakyReLU(alpha=self.negative_slope)
+@converter(torch.mv, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_mv(input: Tensor, vec: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, vec, *, out=None):
+        return tf.linalg.tensordot(input, vec, axes=1)
+    return func
 
 
-@converter(F.leaky_relu, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_leaky_relu(input: Tensor, negative_slope: float = 0.01, inplace: bool = False):
-    def func(input, negative_slope=0.01, inplace=False):
-        return keras.layers.LeakyReLU(alpha=negative_slope)(input)
+@converter(torch.bmm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_bmm(input: Tensor, mat2: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, mat2, *, out=None):
+        return tf.linalg.matmul(input, mat2)
     return func
 
 
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_hardsigmoid(input: Tensor, inplace: bool = False):
-    def func(input, inplace=False):
-        return hard_sigmoid_pytorch_compatible(input)
+@converter(torch.baddbmm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_baddbmm(input: Tensor, batch1: Tensor, batch2: Tensor, *, beta: Number=1, alpha: Number=1, out: Optional[Tensor]=None):
+    def func(input: Tensor, batch1, batch2, *, beta=1, alpha=1, out=None):
+        return beta*input + alpha*tf.linalg.matmul(batch1, batch2)
     return func
 
 
-@converter(F.hardtanh, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_hardtanh(input: Tensor, min_val: float = -1.0, max_val: float = 1.0, inplace: bool = False):
-    def func(input, min_val=-1.0, max_val=1.0, inplace=False):
-        return hard_tanh_pytorch_compatible(input, min_val, max_val)
+@converter(torch.einsum, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_einsum(*args: Any):
+    def func(*args: Any):
+        equation = args[0]
+        operands = args[1:]
+        return keras.layers.Lambda(lambda operands: tf.einsum(equation, *operands))(operands)
     return func
 
 
-@converter(F.hardswish, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_hardswish(input: Tensor, inplace: bool = False):
-    def func(input, inplace=False):
-        return hard_swish_pytorch_compatible(input)
+@converter(torch.Tensor.triu, torch.Tensor.triu_, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_triu(self, diagonal=0):
+    def func(self, diagonal=0):
+        return keras.layers.Lambda(lambda x: tf.experimental.numpy.triu(x, k=diagonal))(self)
     return func
 
 
-@converter(torch.softmax, torch.Tensor.softmax, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_softmax(input: Tensor, dim: Union[str, None], *, dtype: Optional[_dtype]=None):
+@converter(torch.norm, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_norm(input, p="fro", dim=None, keepdim=False, out=None, dtype=None):
     num_dims = input.dim()
 
-    def func(input: Tensor, dim, *, dtype=None):
+    def func(input, p="fro", dim=None, keepdim=False, out=None, dtype=None):
         if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, num_dims)
-        return tf.nn.softmax(input, axis=dim)
+        return tf.norm(input, ord=p, axis=dim, keepdims=keepdim)
     return func
 
 
-@converter(torch.clip, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_clip(input: Tensor, min: Optional[Tensor]=None, max: Optional[Tensor]=None, *, out: Optional[Tensor]=None):
-    def func(input, min=None, max=None, *, out=None):
-        return tf.clip_by_value(input, min, max)
+@converter(F.embedding, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_embedding(input: Tensor, weight: Tensor, padding_idx: Optional[int] = None, max_norm: Optional[float] = None,
+              norm_type: float = 2.0, scale_grad_by_freq: bool = False, sparse: bool = False):
+    input_dim, output_dim = weight.shape
+    weight = weight.detach().numpy()
+
+    layer = keras.layers.Embedding(input_dim, output_dim, weights=[weight])
+
+    def func(input, weight, padding_idx=None, max_norm=None, norm_type=2.0, scale_grad_by_freq=False, sparse=False):
+        return layer(input)
     return func
```

### Comparing `nobuco-0.4.3/nobuco/node_converters/boolean.py` & `nobuco-0.4.4/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.4/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/comparison.py` & `nobuco-0.4.4/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/convolution.py` & `nobuco-0.4.4/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/dropout.py` & `nobuco-0.4.4/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/interpolation.py` & `nobuco-0.4.4/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/math.py` & `nobuco-0.4.4/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/misc.py` & `nobuco-0.4.4/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/normalization.py` & `nobuco-0.4.4/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/padding.py` & `nobuco-0.4.4/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/pooling.py` & `nobuco-0.4.4/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/recurrent.py` & `nobuco-0.4.4/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/slice.py` & `nobuco-0.4.4/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.4/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.4/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.4/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/trace/tensor_storage.py` & `nobuco-0.4.4/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/trace/trace.py` & `nobuco-0.4.4/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/util.py` & `nobuco-0.4.4/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/vis/console_stylizer.py` & `nobuco-0.4.4/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco/vis/html_stylizer.py` & `nobuco-0.4.4/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.4/nobuco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.3
+Version: 0.4.4
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,16 @@
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
 ## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+<img src="https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=flat&logo=pytorch">
+<img src="https://img.shields.io/badge/TensorFlow-2.10-FF6F00.svg?style=flat&logo=tensorflow">
 
 ```bash
 pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
```

### Comparing `nobuco-0.4.3/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.4/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.3/pyproject.toml` & `nobuco-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.3"
+version = "0.4.4"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

