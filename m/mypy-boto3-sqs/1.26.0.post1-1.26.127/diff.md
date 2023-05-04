# Comparing `tmp/mypy-boto3-sqs-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-sqs-1.26.127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:02 2022, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.26.127.tar", last modified: Thu May  4 21:08:52 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.26.0.post1.tar` & `mypy-boto3-sqs-1.26.127.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:02.220851 mypy-boto3-sqs-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17517 2022-11-01 21:44:02.220851 mypy-boto3-sqs-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:02.220851 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16063 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9552 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18794 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)    18755 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22419 2022-11-01 21:41:39.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22386 2022-11-01 21:41:39.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:02.220851 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17517 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:44:02.000000 mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:02.220851 mypy-boto3-sqs-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-01 21:41:38.000000 mypy-boto3-sqs-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.652633 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21880 2023-05-04 21:08:29.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 21:08:52.000000 mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:08:52.664633 mypy-boto3-sqs-1.26.127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 21:08:28.000000 mypy-boto3-sqs-1.26.127/setup.py
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/LICENSE` & `mypy-boto3-sqs-1.26.127/LICENSE`

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

### Comparing `mypy-boto3-sqs-1.26.0.post1/PKG-INFO` & `mypy-boto3-sqs-1.26.127/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sqs
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SQS 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,61 +385,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
-    QueueMessageRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    ServiceResourceMessageRequestTypeDef,
-    ServiceResourceQueueRequestTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
@@ -485,42 +451,42 @@
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

### Comparing `mypy-boto3-sqs-1.26.0.post1/README.md` & `mypy-boto3-sqs-1.26.127/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sqs
+Version: 1.26.127
+Summary: Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,61 +417,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
-    QueueMessageRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    ServiceResourceMessageRequestTypeDef,
-    ServiceResourceQueueRequestTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
@@ -454,42 +483,42 @@
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

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SQS 1.26.127\nVersion:         1.26.127\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.127")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,25 +58,36 @@
 
 
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
+    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
+    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
+    InvalidSecurity: Type[BotocoreClientError]
+    KmsAccessDenied: Type[BotocoreClientError]
+    KmsDisabled: Type[BotocoreClientError]
+    KmsInvalidKeyUsage: Type[BotocoreClientError]
+    KmsInvalidState: Type[BotocoreClientError]
+    KmsNotFound: Type[BotocoreClientError]
+    KmsOptInRequired: Type[BotocoreClientError]
+    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    RequestThrottled: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
@@ -171,15 +182,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message_batch)
         """
 
     def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the queue specified by the `QueueUrl` , regardless of the queue's
+        Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_queue)
         """
 
     def generate_presigned_url(
@@ -300,15 +311,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
 
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
 
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/client.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -55,25 +55,36 @@
         self.operation_name: str
 
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
+    InvalidAddress: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
+    InvalidAttributeValue: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
     InvalidIdFormat: Type[BotocoreClientError]
     InvalidMessageContents: Type[BotocoreClientError]
+    InvalidSecurity: Type[BotocoreClientError]
+    KmsAccessDenied: Type[BotocoreClientError]
+    KmsDisabled: Type[BotocoreClientError]
+    KmsInvalidKeyUsage: Type[BotocoreClientError]
+    KmsInvalidState: Type[BotocoreClientError]
+    KmsNotFound: Type[BotocoreClientError]
+    KmsOptInRequired: Type[BotocoreClientError]
+    KmsThrottled: Type[BotocoreClientError]
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    RequestThrottled: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/)
@@ -158,15 +169,15 @@
         Deletes up to ten messages from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_message_batch)
         """
     def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the queue specified by the `QueueUrl` , regardless of the queue's
+        Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#delete_queue)
         """
     def generate_presigned_url(
         self,
@@ -276,15 +287,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -141,27 +142,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -190,14 +195,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -242,51 +248,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -318,28 +330,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -348,14 +365,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -366,55 +384,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -440,21 +466,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -139,27 +140,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -188,14 +193,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -240,51 +246,57 @@
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
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
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
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -316,28 +328,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -346,14 +363,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -364,55 +382,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
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
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -438,21 +464,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.change_message_visibility_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuechange_message_visibility_batch-method)
         """
 
     def delete(self) -> None:
         """
-        Deletes the queue specified by the `QueueUrl` , regardless of the queue's
+        Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuedelete-method)
         """
 
     def delete_messages(
@@ -336,15 +336,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
 
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
 
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         Changes the visibility timeout of multiple messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.change_message_visibility_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuechange_message_visibility_batch-method)
         """
     def delete(self) -> None:
         """
-        Deletes the queue specified by the `QueueUrl` , regardless of the queue's
+        Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuedelete-method)
         """
     def delete_messages(
         self, *, Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef]
@@ -305,15 +305,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
         Sets the value of one or more queue attributes.
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,68 +27,64 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
+    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
+    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
+    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
+    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
-    "QueueMessageRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "ServiceResourceMessageRequestTypeDef",
-    "ServiceResourceQueueRequestTypeDef",
+    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
-    "CreateQueueResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetQueueAttributesResultTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesResultTypeDef",
-    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -126,21 +122,19 @@
     "_OptionalBatchResultErrorEntryTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
-
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
-
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -148,40 +142,27 @@
     "_OptionalChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "VisibilityTimeout": int,
     },
     total=False,
 )
 
-
 class ChangeMessageVisibilityBatchRequestEntryTypeDef(
     _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef,
     _OptionalChangeMessageVisibilityBatchRequestEntryTypeDef,
 ):
     pass
 
-
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -205,21 +186,19 @@
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef = TypedDict(
     "_RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef = TypedDict(
@@ -227,21 +206,27 @@
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
@@ -265,35 +250,48 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalGetQueueAttributesRequestRequestTypeDef",
     {
         "AttributeNames": Sequence[QueueAttributeFilterType],
     },
     total=False,
 )
 
-
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
@@ -301,53 +299,67 @@
     "_OptionalGetQueueUrlRequestRequestTypeDef",
     {
         "QueueOwnerAWSAccountId": str,
     },
     total=False,
 )
 
-
 class GetQueueUrlRequestRequestTypeDef(
     _RequiredGetQueueUrlRequestRequestTypeDef, _OptionalGetQueueUrlRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef = TypedDict(
     "_OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     {
         "QueueOwnerAWSAccountId": str,
     },
     total=False,
 )
 
-
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -355,39 +367,72 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -397,21 +442,19 @@
         "BinaryValue": bytes,
         "StringListValues": List[str],
         "BinaryListValues": List[bytes],
     },
     total=False,
 )
 
-
 class MessageAttributeValueTypeDef(
     _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
 ):
     pass
 
-
 _RequiredMessageSystemAttributeValueTypeDef = TypedDict(
     "_RequiredMessageSystemAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageSystemAttributeValueTypeDef = TypedDict(
@@ -421,32 +464,33 @@
         "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
         "StringListValues": Sequence[str],
         "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
     total=False,
 )
 
-
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
-
-PurgeQueueRequestRequestTypeDef = TypedDict(
-    "PurgeQueueRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "QueueUrl": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-QueueMessageRequestTypeDef = TypedDict(
-    "QueueMessageRequestTypeDef",
+PurgeQueueRequestRequestTypeDef = TypedDict(
+    "PurgeQueueRequestRequestTypeDef",
     {
-        "receipt_handle": str,
+        "QueueUrl": str,
     },
 )
 
 ReceiveMessageRequestQueueReceiveMessagesTypeDef = TypedDict(
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     {
         "AttributeNames": Sequence[QueueAttributeFilterType],
@@ -474,21 +518,19 @@
         "VisibilityTimeout": int,
         "WaitTimeSeconds": int,
         "ReceiveRequestAttemptId": str,
     },
     total=False,
 )
 
-
 class ReceiveMessageRequestRequestTypeDef(
     _RequiredReceiveMessageRequestRequestTypeDef, _OptionalReceiveMessageRequestRequestTypeDef
 ):
     pass
 
-
 RemovePermissionRequestQueueRemovePermissionTypeDef = TypedDict(
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     {
         "Label": str,
     },
 )
 
@@ -496,14 +538,25 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -514,33 +567,28 @@
         "MD5OfMessageAttributes": str,
         "MD5OfMessageSystemAttributes": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
-
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
-
-ServiceResourceMessageRequestTypeDef = TypedDict(
-    "ServiceResourceMessageRequestTypeDef",
-    {
-        "queue_url": str,
-        "receipt_handle": str,
-    },
-)
-
-ServiceResourceQueueRequestTypeDef = TypedDict(
-    "ServiceResourceQueueRequestTypeDef",
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
     {
-        "url": str,
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
@@ -587,84 +635,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -680,47 +659,16 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
@@ -750,21 +698,19 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
-
 class SendMessageBatchRequestEntryTypeDef(
     _RequiredSendMessageBatchRequestEntryTypeDef, _OptionalSendMessageBatchRequestEntryTypeDef
 ):
     pass
 
-
 _RequiredSendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "_RequiredSendMessageRequestQueueSendMessageTypeDef",
     {
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestQueueSendMessageTypeDef = TypedDict(
@@ -777,22 +723,20 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
-
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
@@ -806,35 +750,33 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
-
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
-
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,67 +27,65 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
+    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
+    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
+    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
+    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
-    "QueueMessageRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "ServiceResourceMessageRequestTypeDef",
-    "ServiceResourceQueueRequestTypeDef",
+    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
-    "CreateQueueResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetQueueAttributesResultTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesResultTypeDef",
-    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -125,19 +123,21 @@
     "_OptionalBatchResultErrorEntryTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
+
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -145,38 +145,29 @@
     "_OptionalChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "VisibilityTimeout": int,
     },
     total=False,
 )
 
+
 class ChangeMessageVisibilityBatchRequestEntryTypeDef(
     _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef,
     _OptionalChangeMessageVisibilityBatchRequestEntryTypeDef,
 ):
     pass
 
+
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -200,19 +191,21 @@
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef = TypedDict(
     "_RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef = TypedDict(
@@ -220,20 +213,30 @@
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
+
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -256,83 +259,124 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalGetQueueAttributesRequestRequestTypeDef",
     {
         "AttributeNames": Sequence[QueueAttributeFilterType],
     },
     total=False,
 )
 
+
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
+
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_OptionalGetQueueUrlRequestRequestTypeDef",
     {
         "QueueOwnerAWSAccountId": str,
     },
     total=False,
 )
 
+
 class GetQueueUrlRequestRequestTypeDef(
     _RequiredGetQueueUrlRequestRequestTypeDef, _OptionalGetQueueUrlRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef = TypedDict(
     "_OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     {
         "QueueOwnerAWSAccountId": str,
     },
     total=False,
 )
 
+
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -340,37 +384,74 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
+
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -380,19 +461,21 @@
         "BinaryValue": bytes,
         "StringListValues": List[str],
         "BinaryListValues": List[bytes],
     },
     total=False,
 )
 
+
 class MessageAttributeValueTypeDef(
     _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
 ):
     pass
 
+
 _RequiredMessageSystemAttributeValueTypeDef = TypedDict(
     "_RequiredMessageSystemAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageSystemAttributeValueTypeDef = TypedDict(
@@ -402,30 +485,35 @@
         "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
         "StringListValues": Sequence[str],
         "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
     total=False,
 )
 
+
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
-PurgeQueueRequestRequestTypeDef = TypedDict(
-    "PurgeQueueRequestRequestTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "QueueUrl": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-QueueMessageRequestTypeDef = TypedDict(
-    "QueueMessageRequestTypeDef",
+PurgeQueueRequestRequestTypeDef = TypedDict(
+    "PurgeQueueRequestRequestTypeDef",
     {
-        "receipt_handle": str,
+        "QueueUrl": str,
     },
 )
 
 ReceiveMessageRequestQueueReceiveMessagesTypeDef = TypedDict(
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     {
         "AttributeNames": Sequence[QueueAttributeFilterType],
@@ -453,19 +541,21 @@
         "VisibilityTimeout": int,
         "WaitTimeSeconds": int,
         "ReceiveRequestAttemptId": str,
     },
     total=False,
 )
 
+
 class ReceiveMessageRequestRequestTypeDef(
     _RequiredReceiveMessageRequestRequestTypeDef, _OptionalReceiveMessageRequestRequestTypeDef
 ):
     pass
 
+
 RemovePermissionRequestQueueRemovePermissionTypeDef = TypedDict(
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     {
         "Label": str,
     },
 )
 
@@ -473,14 +563,25 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -491,31 +592,30 @@
         "MD5OfMessageAttributes": str,
         "MD5OfMessageSystemAttributes": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
+
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
-ServiceResourceMessageRequestTypeDef = TypedDict(
-    "ServiceResourceMessageRequestTypeDef",
-    {
-        "queue_url": str,
-        "receipt_handle": str,
-    },
-)
 
-ServiceResourceQueueRequestTypeDef = TypedDict(
-    "ServiceResourceQueueRequestTypeDef",
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
     {
-        "url": str,
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
@@ -562,84 +662,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -655,47 +686,18 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
@@ -723,19 +725,21 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
+
 class SendMessageBatchRequestEntryTypeDef(
     _RequiredSendMessageBatchRequestEntryTypeDef, _OptionalSendMessageBatchRequestEntryTypeDef
 ):
     pass
 
+
 _RequiredSendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "_RequiredSendMessageRequestQueueSendMessageTypeDef",
     {
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestQueueSendMessageTypeDef = TypedDict(
@@ -748,20 +752,22 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
+
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
+
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
@@ -775,33 +781,35 @@
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
+
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
+
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SQS 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.127
+Summary: Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.127](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,61 +417,58 @@
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
-    QueueMessageRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    ServiceResourceMessageRequestTypeDef,
-    ServiceResourceQueueRequestTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
@@ -485,42 +483,42 @@
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

### Comparing `mypy-boto3-sqs-1.26.0.post1/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.26.127/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.0.post1/setup.py` & `mypy-boto3-sqs-1.26.127/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-sqs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.26.0.post1",
+    version="1.26.127",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.SQS 1.26.127 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_sqs": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_sqs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/",
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

