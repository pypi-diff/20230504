# Comparing `tmp/apify_client-1.0.0b1.tar.gz` & `tmp/apify_client-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.0.0b1.tar", last modified: Mon Mar 13 12:50:39 2023, max compression
+gzip compressed data, was "apify_client-1.1.0a1.tar", last modified: Thu May  4 15:48:30 2023, max compression
```

## Comparing `apify_client-1.0.0b1.tar` & `apify_client-1.1.0a1.tar`

### file list

```diff
@@ -1,60 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.694511 apify_client-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-13 12:50:39.694511 apify_client-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 12:50:39.694511 apify_client-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.686510 apify_client-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.690510 apify_client-1.0.0b1/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.690510 apify_client-1.0.0b1/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.690510 apify_client-1.0.0b1/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.694511 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    46610 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:23.000000 apify_client-1.0.0b1/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:50:39.690510 apify_client-1.0.0b1/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 12:50:39.000000 apify_client-1.0.0b1/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 15:48:27.000000 apify_client-1.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.483518 apify_client-1.1.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.0.0b1/LICENSE` & `apify_client-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/PKG-INFO` & `apify_client-1.1.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.0.0b1
+Version: 1.1.0a1
 Summary: Apify API client for Python
-Home-page: https://github.com/apify/apify-client-python
-Author: Apify Technologies s.r.o.
-Author-email: support@apify.com
+Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
+Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
 Project-URL: Apify Homepage, https://apify.com
 Keywords: apify,api,client,scraping,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -84,16 +83,16 @@
 The documentation is then rendered from the docstrings in the code using Sphinx and some heavy post-processing and saved as `docs/docs.md`.
 To generate the documentation, just run `make docs`.
 
 ### Release process
 
 Publishing new versions to [PyPI](https://pypi.org/project/apify-client) happens automatically through GitHub Actions.
 
-On each commit to the `master` branch, a new beta release is published, taking the version number from `src/apify_client/_version.py`
+On each commit to the `master` branch, a new beta release is published, taking the version number from `pyproject.toml`
 and automatically incrementing the beta version suffix by 1 from the last beta release published to PyPI.
 
-A stable version is published when a new release is created using GitHub Releases, again taking the version number from `src/apify_client/_version.py`. The built package assets are automatically uploaded to the GitHub release.
+A stable version is published when a new release is created using GitHub Releases, again taking the version number from `pyproject.toml`. The built package assets are automatically uploaded to the GitHub release.
 
-If there is already a stable version with the same version number as in `src/apify_client/_version.py` published to PyPI, the publish process fails,
+If there is already a stable version with the same version number as in `pyproject.toml` published to PyPI, the publish process fails,
 so don't forget to update the version number before releasing a new version.
 The release process also fails when the released version is not described in `CHANGELOG.md`,
 so don't forget to describe the changes in the new version there.
```

### Comparing `apify_client-1.0.0b1/README.md` & `apify_client-1.1.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 The documentation is then rendered from the docstrings in the code using Sphinx and some heavy post-processing and saved as `docs/docs.md`.
 To generate the documentation, just run `make docs`.
 
 ### Release process
 
 Publishing new versions to [PyPI](https://pypi.org/project/apify-client) happens automatically through GitHub Actions.
 
-On each commit to the `master` branch, a new beta release is published, taking the version number from `src/apify_client/_version.py`
+On each commit to the `master` branch, a new beta release is published, taking the version number from `pyproject.toml`
 and automatically incrementing the beta version suffix by 1 from the last beta release published to PyPI.
 
-A stable version is published when a new release is created using GitHub Releases, again taking the version number from `src/apify_client/_version.py`. The built package assets are automatically uploaded to the GitHub release.
+A stable version is published when a new release is created using GitHub Releases, again taking the version number from `pyproject.toml`. The built package assets are automatically uploaded to the GitHub release.
 
-If there is already a stable version with the same version number as in `src/apify_client/_version.py` published to PyPI, the publish process fails,
+If there is already a stable version with the same version number as in `pyproject.toml` published to PyPI, the publish process fails,
 so don't forget to update the version number before releasing a new version.
 The release process also fails when the released version is not described in `CHANGELOG.md`,
 so don't forget to describe the changes in the new version there.
```

### Comparing `apify_client-1.0.0b1/src/apify_client/_errors.py` & `apify_client-1.1.0a1/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/src/apify_client/_http_client.py` & `apify_client-1.1.0a1/src/apify_client/_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import gzip
 import json as jsonlib
 import logging
 import os
 import sys
 from http import HTTPStatus
+from importlib import metadata
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import httpx
 
 from ._errors import ApifyApiError, InvalidResponseBodyError, _is_retryable_error
 from ._logging import logger_name
 from ._types import JSONSerializable
@@ -15,15 +16,14 @@
     _is_content_type_json,
     _is_content_type_text,
     _is_content_type_xml,
     _retry_with_exp_backoff,
     _retry_with_exp_backoff_async,
     ignore_docs,
 )
-from ._version import __version__
 
 DEFAULT_BACKOFF_EXPONENTIAL_FACTOR = 2
 DEFAULT_BACKOFF_RANDOM_FACTOR = 1
 
 logger = logging.getLogger(logger_name)
 
 
@@ -45,16 +45,17 @@
 
         workflow_key = os.getenv('APIFY_WORKFLOW_KEY')
         if workflow_key is not None:
             headers['X-Apify-Workflow-Key'] = workflow_key
 
         is_at_home = ('APIFY_IS_AT_HOME' in os.environ)
         python_version = '.'.join([str(x) for x in sys.version_info[:3]])
+        client_version = metadata.version('apify-client')
 
-        user_agent = f'ApifyClient/{__version__} ({sys.platform}; Python/{python_version}); isAtHome/{is_at_home}'
+        user_agent = f'ApifyClient/{client_version} ({sys.platform}; Python/{python_version}); isAtHome/{is_at_home}'
         headers['User-Agent'] = user_agent
 
         if token is not None:
             headers['Authorization'] = f'Bearer {token}'
 
         self.httpx_client = httpx.Client(headers=headers, follow_redirects=True, timeout=timeout_secs)
         self.httpx_async_client = httpx.AsyncClient(headers=headers, follow_redirects=True, timeout=timeout_secs)
```

### Comparing `apify_client-1.0.0b1/src/apify_client/_logging.py` & `apify_client-1.1.0a1/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/src/apify_client/_utils.py` & `apify_client-1.1.0a1/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/src/apify_client/client.py` & `apify_client-1.1.0a1/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/src/apify_client/consts.py` & `apify_client-1.1.0a1/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.0.0b1/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.1.0a1/src/apify_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.0.0b1
+Version: 1.1.0a1
 Summary: Apify API client for Python
-Home-page: https://github.com/apify/apify-client-python
-Author: Apify Technologies s.r.o.
-Author-email: support@apify.com
+Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
+Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
 Project-URL: Apify Homepage, https://apify.com
 Keywords: apify,api,client,scraping,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -84,16 +83,16 @@
 The documentation is then rendered from the docstrings in the code using Sphinx and some heavy post-processing and saved as `docs/docs.md`.
 To generate the documentation, just run `make docs`.
 
 ### Release process
 
 Publishing new versions to [PyPI](https://pypi.org/project/apify-client) happens automatically through GitHub Actions.
 
-On each commit to the `master` branch, a new beta release is published, taking the version number from `src/apify_client/_version.py`
+On each commit to the `master` branch, a new beta release is published, taking the version number from `pyproject.toml`
 and automatically incrementing the beta version suffix by 1 from the last beta release published to PyPI.
 
-A stable version is published when a new release is created using GitHub Releases, again taking the version number from `src/apify_client/_version.py`. The built package assets are automatically uploaded to the GitHub release.
+A stable version is published when a new release is created using GitHub Releases, again taking the version number from `pyproject.toml`. The built package assets are automatically uploaded to the GitHub release.
 
-If there is already a stable version with the same version number as in `src/apify_client/_version.py` published to PyPI, the publish process fails,
+If there is already a stable version with the same version number as in `pyproject.toml` published to PyPI, the publish process fails,
 so don't forget to update the version number before releasing a new version.
 The release process also fails when the released version is not described in `CHANGELOG.md`,
 so don't forget to describe the changes in the new version there.
```

### Comparing `apify_client-1.0.0b1/src/apify_client.egg-info/requires.txt` & `apify_client-1.1.0a1/src/apify_client.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 pytest-randomly~=3.12.0
 pytest-timeout~=2.1.0
 pytest-xdist~=3.2.0
 redbaron~=0.9.2
 sphinx~=6.1.3
 sphinx-autodoc-typehints~=1.22
 sphinx-markdown-builder==0.5.4
-types-setuptools
+twine~=4.0.2
```

