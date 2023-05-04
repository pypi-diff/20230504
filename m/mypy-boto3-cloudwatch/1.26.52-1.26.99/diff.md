# Comparing `tmp/mypy-boto3-cloudwatch-1.26.52.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.26.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.26.52.tar", last modified: Wed Jan 18 21:22:51 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.26.99.tar", last modified: Fri Mar 24 19:32:25 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.26.52.tar` & `mypy-boto3-cloudwatch-1.26.99.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.432996 mypy-boto3-cloudwatch-1.26.52/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-01-18 21:22:51.432996 mypy-boto3-cloudwatch-1.26.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.432996 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42770 2023-01-18 21:22:35.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42725 2023-01-18 21:22:35.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-01-18 21:22:34.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.432996 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-18 21:22:51.000000 mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 21:22:51.444996 mypy-boto3-cloudwatch-1.26.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-18 21:22:33.000000 mypy-boto3-cloudwatch-1.26.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-03-24 19:32:02.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-03-24 19:32:02.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/LICENSE` & `mypy-boto3-cloudwatch-1.26.99/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/PKG-INFO` & `mypy-boto3-cloudwatch-1.26.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.26.52
-Summary: Type annotations for boto3.CloudWatch 1.26.52 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.99
+Summary: Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -489,16 +489,14 @@
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PutDashboardInputRequestTypeDef,
-    ServiceResourceAlarmRequestTypeDef,
-    ServiceResourceMetricRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
@@ -571,42 +569,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/README.md` & `mypy-boto3-cloudwatch-1.26.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -457,16 +457,14 @@
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PutDashboardInputRequestTypeDef,
-    ServiceResourceAlarmRequestTypeDef,
-    ServiceResourceMetricRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
@@ -539,42 +537,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.26.52\nVersion:         1.26.52\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.CloudWatch 1.26.99\nVersion:         1.26.99\nBuilder version:"
+        " 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.52")
+    print("1.26.99")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionsSuppressedByType",
     "AlarmExistsWaiterName",
     "AlarmTypeType",
     "AnomalyDetectorStateValueType",
     "AnomalyDetectorTypeType",
     "ComparisonOperatorType",
@@ -46,15 +45,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionsSuppressedByType = Literal["Alarm", "ExtensionPeriod", "WaitPeriod"]
 AlarmExistsWaiterName = Literal["alarm_exists"]
 AlarmTypeType = Literal["CompositeAlarm", "MetricAlarm"]
 AnomalyDetectorStateValueType = Literal["PENDING_TRAINING", "TRAINED", "TRAINED_INSUFFICIENT_DATA"]
 AnomalyDetectorTypeType = Literal["METRIC_MATH", "SINGLE_METRIC"]
 ComparisonOperatorType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -160,14 +158,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -253,14 +252,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -271,14 +271,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -429,14 +430,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -478,14 +480,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionsSuppressedByType",
     "AlarmExistsWaiterName",
     "AlarmTypeType",
     "AnomalyDetectorStateValueType",
     "AnomalyDetectorTypeType",
     "ComparisonOperatorType",
@@ -45,14 +46,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ActionsSuppressedByType = Literal["Alarm", "ExtensionPeriod", "WaitPeriod"]
 AlarmExistsWaiterName = Literal["alarm_exists"]
 AlarmTypeType = Literal["CompositeAlarm", "MetricAlarm"]
 AnomalyDetectorStateValueType = Literal["PENDING_TRAINING", "TRAINED", "TRAINED_INSUFFICIENT_DATA"]
 AnomalyDetectorTypeType = Literal["METRIC_MATH", "SINGLE_METRIC"]
 ComparisonOperatorType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -158,14 +160,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -251,14 +254,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -269,14 +273,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -427,14 +432,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -476,14 +482,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,14 @@
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "ServiceResourceAlarmRequestTypeDef",
-    "ServiceResourceMetricRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
@@ -660,29 +658,14 @@
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-ServiceResourceAlarmRequestTypeDef = TypedDict(
-    "ServiceResourceAlarmRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-
-ServiceResourceMetricRequestTypeDef = TypedDict(
-    "ServiceResourceMetricRequestTypeDef",
-    {
-        "namespace": str,
-        "name": str,
-    },
-)
-
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,14 @@
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "ServiceResourceAlarmRequestTypeDef",
-    "ServiceResourceMetricRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
@@ -647,29 +645,14 @@
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-ServiceResourceAlarmRequestTypeDef = TypedDict(
-    "ServiceResourceAlarmRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-
-ServiceResourceMetricRequestTypeDef = TypedDict(
-    "ServiceResourceMetricRequestTypeDef",
-    {
-        "namespace": str,
-        "name": str,
-    },
-)
-
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.26.52
-Summary: Type annotations for boto3.CloudWatch 1.26.52 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.99
+Summary: Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -489,16 +489,14 @@
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
     PutDashboardInputRequestTypeDef,
-    ServiceResourceAlarmRequestTypeDef,
-    ServiceResourceMetricRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
@@ -571,42 +569,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-cloudwatch-1.26.52/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.52/setup.py` & `mypy-boto3-cloudwatch-1.26.99/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-cloudwatch.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.26.52",
+    version="1.26.99",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.26.52 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder"
+        " 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

