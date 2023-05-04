# Comparing `tmp/cirro-0.6.8.tar.gz` & `tmp/cirro-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-0.6.8.tar", max compression
+gzip compressed data, was "cirro-0.6.9.tar", max compression
```

## Comparing `cirro-0.6.8.tar` & `cirro-0.6.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1086 2023-04-04 21:37:31.152716 cirro-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     4612 2023-04-04 21:37:31.152716 cirro-0.6.8/README.md
--rw-r--r--   0        0        0       65 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/__init__.py
--rw-r--r--   0        0        0       92 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/__init__.py
--rw-r--r--   0        0        0     1908 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/auth/__init__.py
--rw-r--r--   0        0        0      576 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/auth/base.py
--rw-r--r--   0        0        0     1653 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/auth/iam.py
--rw-r--r--   0        0        0     5763 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/auth/oauth_client.py
--rw-r--r--   0        0        0     1856 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/auth/username.py
--rw-r--r--   0        0        0      133 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/clients/__init__.py
--rw-r--r--   0        0        0     1460 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/clients/api.py
--rw-r--r--   0        0        0     1559 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/clients/portal.py
--rw-r--r--   0        0        0     4045 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/clients/s3.py
--rw-r--r--   0        0        0      199 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/clients/utils.py
--rw-r--r--   0        0        0     3012 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/config.py
--rw-r--r--   0        0        0        0 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/__init__.py
--rw-r--r--   0        0        0      101 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/api.py
--rw-r--r--   0        0        0      519 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/auth.py
--rw-r--r--   0        0        0     1706 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/dataset.py
--rw-r--r--   0        0        0      120 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/exceptions.py
--rw-r--r--   0        0        0     4250 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/file.py
--rw-r--r--   0        0        0     2659 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/form_specification.py
--rw-r--r--   0        0        0     3013 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/process.py
--rw-r--r--   0        0        0      539 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/project.py
--rw-r--r--   0        0        0     1425 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/reference.py
--rw-r--r--   0        0        0      430 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/s3_path.py
--rw-r--r--   0        0        0      268 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/status.py
--rw-r--r--   0        0        0      777 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/models/workflow_models.py
--rw-r--r--   0        0        0      382 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/base.py
--rw-r--r--   0        0        0      690 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/common.py
--rw-r--r--   0        0        0     6351 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/dataset.py
--rw-r--r--   0        0        0     4110 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/file.py
--rw-r--r--   0        0        0     6454 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/process.py
--rw-r--r--   0        0        0     2471 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/api/services/project.py
--rw-r--r--   0        0        0      244 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2523 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/cli.py
--rw-r--r--   0        0        0     6458 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      583 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     4610 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      573 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     3507 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2250 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0    12069 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/workflow_args.py
--rw-r--r--   0        0        0     9132 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/interactive/workflow_form_args.py
--rw-r--r--   0        0        0      371 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/cli/models.py
--rw-r--r--   0        0        0     3477 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/file_utils.py
--rw-r--r--   0        0        0      257 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/helpers/form.py
--rw-r--r--   0        0        0     5901 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0     9137 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/helpers/workflow_config.py
--rw-r--r--   0        0        0       73 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2901 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/asset.py
--rw-r--r--   0        0        0     3713 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     4317 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/file.py
--rw-r--r--   0        0        0     1670 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     2779 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/portal.py
--rw-r--r--   0        0        0     1552 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/process.py
--rw-r--r--   0        0        0     6418 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/project.py
--rw-r--r--   0        0        0      861 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/reference.py
--rw-r--r--   0        0        0      964 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0     1215 2023-04-04 21:37:31.152716 cirro-0.6.8/cirro/utils.py
--rw-r--r--   0        0        0      887 2023-04-04 21:37:31.152716 cirro-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 cirro-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-19 22:05:51.562855 cirro-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     4982 2023-04-19 22:05:51.562855 cirro-0.6.9/README.md
+-rw-r--r--   0        0        0       65 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/__init__.py
+-rw-r--r--   0        0        0     1908 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/base.py
+-rw-r--r--   0        0        0     1653 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/iam.py
+-rw-r--r--   0        0        0     6650 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/oauth_client.py
+-rw-r--r--   0        0        0     1856 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/username.py
+-rw-r--r--   0        0        0      133 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/__init__.py
+-rw-r--r--   0        0        0     1460 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/api.py
+-rw-r--r--   0        0        0     1559 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/portal.py
+-rw-r--r--   0        0        0     4045 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/s3.py
+-rw-r--r--   0        0        0      199 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/utils.py
+-rw-r--r--   0        0        0     3304 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/config.py
+-rw-r--r--   0        0        0        0 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/api.py
+-rw-r--r--   0        0        0      566 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/auth.py
+-rw-r--r--   0        0        0     1706 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/dataset.py
+-rw-r--r--   0        0        0      120 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/exceptions.py
+-rw-r--r--   0        0        0     4250 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/file.py
+-rw-r--r--   0        0        0     2659 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/form_specification.py
+-rw-r--r--   0        0        0     3013 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/process.py
+-rw-r--r--   0        0        0      539 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/project.py
+-rw-r--r--   0        0        0     1425 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/reference.py
+-rw-r--r--   0        0        0      430 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/s3_path.py
+-rw-r--r--   0        0        0      268 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/status.py
+-rw-r--r--   0        0        0      777 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/workflow_models.py
+-rw-r--r--   0        0        0      382 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/base.py
+-rw-r--r--   0        0        0      690 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/common.py
+-rw-r--r--   0        0        0     6351 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/dataset.py
+-rw-r--r--   0        0        0     4201 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/file.py
+-rw-r--r--   0        0        0     6454 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/process.py
+-rw-r--r--   0        0        0     2471 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/api/services/project.py
+-rw-r--r--   0        0        0      244 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2523 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6458 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      583 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     4610 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      573 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     3507 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2250 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0    12069 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/workflow_args.py
+-rw-r--r--   0        0        0     9132 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/workflow_form_args.py
+-rw-r--r--   0        0        0      371 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/models.py
+-rw-r--r--   0        0        0     3685 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/file_utils.py
+-rw-r--r--   0        0        0      257 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5901 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0     9137 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/workflow_config.py
+-rw-r--r--   0        0        0       73 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2901 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     3713 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     4317 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1670 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     2779 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     1552 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/process.py
+-rw-r--r--   0        0        0     6418 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/project.py
+-rw-r--r--   0        0        0      861 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/reference.py
+-rw-r--r--   0        0        0      964 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0     1215 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/utils.py
+-rw-r--r--   0        0        0      887 2023-04-19 22:05:51.566855 cirro-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 cirro-0.6.9/PKG-INFO
```

### Comparing `cirro-0.6.8/LICENSE.txt` & `cirro-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/README.md` & `cirro-0.6.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -114,11 +114,16 @@
 
 ### Configuration
 
 The `cirro-cli configure` command creates a file in `PW_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable. 
 
+The `transfer_max_retries` configuration property specifies the maximum number of times to attempt uploading a file to Cirro in the event of a transfer failure. 
+When uploading files to Cirro, network issues or temporary outages can occasionally cause a transfer to fail.
+It will pause for an increasing amount of time for each retry attempt.
+
 ```ini
 [General]
 base_url = data-portal.io
+transfer_max_retries = 15
 ```
```

### Comparing `cirro-0.6.8/cirro/api/auth/__init__.py` & `cirro-0.6.9/cirro/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/auth/base.py` & `cirro-0.6.9/cirro/api/auth/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/auth/iam.py` & `cirro-0.6.9/cirro/api/auth/iam.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/auth/oauth_client.py` & `cirro-0.6.9/cirro/api/auth/oauth_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import logging
 import sys
 import threading
 import time
-from datetime import datetime
+from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Optional
 
 import boto3
 import jwt
 import requests
 from botocore.exceptions import ClientError
 from msal_extensions import FilePersistence
+from msal_extensions.persistence import BasePersistence
 from requests.auth import AuthBase
 
 from cirro.api.auth.base import AuthInfo, RequestAuthWrapper
 from cirro.api.config import Constants
 from cirro.api.models.auth import DeviceTokenResponse, OAuthTokenResponse
 
 logger = logging.getLogger()
@@ -81,21 +82,34 @@
 
     Implements the OAuth device code flow
     This is the preferred way to authenticate
     """
     def __init__(self, client_id: str, region: str, auth_endpoint: str, enable_cache=True):
         self.client_id = client_id
         self.region = region
-        self._token_info = None
-        self._persistence = None
+        self._token_info: Optional[OAuthTokenResponse] = None
+        self._persistence: Optional[BasePersistence] = None
 
         if enable_cache:
             self._persistence = _build_token_persistence(str(TOKEN_PATH), fallback_to_plaintext=True)
             self._token_info = self._load_token_info()
 
+        # Check saved token for change in endpoint
+        if self._token_info and self._token_info.get('client_id') != client_id:
+            logger.debug('Different client ID found, clearing saved token info')
+            self._clear_token_info()
+
+        # Check saved token for refresh token expiry
+        if self._token_info and self._token_info.get('refresh_expires_in'):
+            refresh_expiry_threshold = datetime.fromtimestamp(self._token_info.get('refresh_expires_in'))\
+                                       - timedelta(hours=12)
+            if refresh_expiry_threshold < datetime.now():
+                logger.debug('Refresh token expiry is too soon, re-authenticating')
+                self._clear_token_info()
+
         if not self._token_info:
             self._token_info = _authenticate(client_id=client_id, auth_endpoint=auth_endpoint)
 
         self._save_token_info()
         self._update_token_metadata()
         self._get_token_lock = threading.Lock()
 
@@ -158,7 +172,8 @@
         self._persistence.save(json.dumps(self._token_info))
 
     def _clear_token_info(self):
         if not self._persistence:
             return
 
         Path(self._persistence.get_location()).unlink(missing_ok=True)
+        self._token_info = None
```

### Comparing `cirro-0.6.8/cirro/api/auth/username.py` & `cirro-0.6.9/cirro/api/auth/username.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/clients/api.py` & `cirro-0.6.9/cirro/api/clients/api.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/clients/portal.py` & `cirro-0.6.9/cirro/api/clients/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/clients/s3.py` & `cirro-0.6.9/cirro/api/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/config.py` & `cirro-0.6.9/cirro/api/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 from requests import HTTPError
 
 
 class Constants:
     home = os.environ.get('PW_HOME', '~/.cirro')
     config_path = Path(home, 'config.ini').expanduser()
     default_base_url = "data-portal.io"
+    default_max_retries = 10
 
 
 class UserConfig(NamedTuple):
     auth_method: str
     auth_method_config: Dict  # This needs to match the init params of the auth method
     base_url: Optional[str]
+    transfer_max_retries: Optional[int]
 
 
 def save_user_config(user_config: UserConfig):
     original_user_config = load_user_config()
     ini_config = configparser.SafeConfigParser()
     ini_config['General'] = {
         'auth_method': user_config.auth_method,
-        'base_url': Constants.default_base_url
+        'base_url': Constants.default_base_url,
+        'transfer_max_retries': Constants.default_max_retries
     }
     if original_user_config:
         ini_config['General']['base_url'] = original_user_config.base_url
 
     ini_config[user_config.auth_method] = user_config.auth_method_config
     Constants.config_path.parent.mkdir(exist_ok=True)
     with Constants.config_path.open('w') as configfile:
@@ -41,24 +44,26 @@
 
     try:
         ini_config = configparser.ConfigParser()
         ini_config.read(str(Constants.config_path.absolute()))
         main_config = ini_config['General']
         auth_method = main_config.get('auth_method')
         base_url = main_config.get('base_url')
+        transfer_max_retries = main_config.getint('transfer_max_retries', Constants.default_max_retries)
 
         if auth_method and ini_config.has_section(auth_method):
             auth_method_config = dict(ini_config[auth_method])
         else:
             auth_method_config = {}
 
         return UserConfig(
             auth_method=auth_method,
             auth_method_config=auth_method_config,
-            base_url=base_url
+            base_url=base_url,
+            transfer_max_retries=transfer_max_retries
         )
     except Exception:
         raise RuntimeError('Configuration load error, please re-run configuration')
 
 
 class AppConfig:
     def __init__(self, base_url: str = None):
```

### Comparing `cirro-0.6.8/cirro/api/models/dataset.py` & `cirro-0.6.9/cirro/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/file.py` & `cirro-0.6.9/cirro/api/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/form_specification.py` & `cirro-0.6.9/cirro/api/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/process.py` & `cirro-0.6.9/cirro/api/models/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/project.py` & `cirro-0.6.9/cirro/api/models/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/reference.py` & `cirro-0.6.9/cirro/api/models/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/models/workflow_models.py` & `cirro-0.6.9/cirro/api/models/workflow_models.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/services/base.py` & `cirro-0.6.9/cirro/api/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/services/common.py` & `cirro-0.6.9/cirro/api/services/common.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/services/dataset.py` & `cirro-0.6.9/cirro/api/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/services/file.py` & `cirro-0.6.9/cirro/api/services/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         Uploads a list of files from the specified directory
         :param access_context: File access context, use class methods to generate
         :param directory: base path to upload from
         :param files: relative path of files to upload
         :return:
         """
         s3_client = S3Client(partial(self.get_access_credentials, access_context), self._configuration.region)
-        upload_directory(directory, files, s3_client, access_context.bucket, access_context.path_prefix)
+        upload_directory(directory, files, s3_client, access_context.bucket, access_context.path_prefix,
+                         max_retries=self._configuration.user_config.transfer_max_retries)
 
     def download_files(self, access_context: FileAccessContext, directory: str, files: List[str]):
         """
         Download a list of files to the specified directory
         :param access_context: File access context, use class methods to generate
         :param directory: download location
         :param files: relative path of files to download
```

### Comparing `cirro-0.6.8/cirro/api/services/process.py` & `cirro-0.6.9/cirro/api/services/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/api/services/project.py` & `cirro-0.6.9/cirro/api/services/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/cli.py` & `cirro-0.6.9/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/controller.py` & `cirro-0.6.9/cirro/cli/controller.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/auth_args.py` & `cirro-0.6.9/cirro/cli/interactive/auth_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/common_args.py` & `cirro-0.6.9/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/download_args.py` & `cirro-0.6.9/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/list_dataset_args.py` & `cirro-0.6.9/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/upload_args.py` & `cirro-0.6.9/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/utils.py` & `cirro-0.6.9/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/workflow_args.py` & `cirro-0.6.9/cirro/cli/interactive/workflow_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/cli/interactive/workflow_form_args.py` & `cirro-0.6.9/cirro/cli/interactive/workflow_form_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/file_utils.py` & `cirro-0.6.9/cirro/file_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
+import random
+import time
 from pathlib import Path, PurePath
 from typing import List, Union
 
 from boto3.exceptions import S3UploadFailedError
+from botocore.exceptions import ConnectionError
 
 from cirro.api.clients import S3Client
 from cirro.api.models.file import DirectoryStatistics, File
 
 if os.name == 'nt':
     import win32api
     import win32con
@@ -82,19 +85,20 @@
                     bucket=bucket,
                     key=key
                 )
 
                 success = True
 
             # Catch the upload error
-            except S3UploadFailedError as e:
-
+            except (S3UploadFailedError, ConnectionError) as e:
+                delay = random.uniform(0, 60) + retry * 60
                 # Report the error
                 print(f"Encountered error:\n{str(e)}\n"
-                      f"Retrying ({max_retries - (retry + 1)} attempts remaining)")
+                      f"Retrying in {delay:.0f} seconds ({max_retries - (retry + 1)} attempts remaining)")
+                time.sleep(delay)
 
             if success:
                 break
 
 
 def download_directory(directory: str, files: List[str], s3_client: S3Client, bucket: str, prefix: str):
     for file in files:
```

### Comparing `cirro-0.6.8/cirro/helpers/constants.py` & `cirro-0.6.9/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/helpers/form.py` & `cirro-0.6.9/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/helpers/preprocess_dataset.py` & `cirro-0.6.9/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/helpers/workflow_config.py` & `cirro-0.6.9/cirro/helpers/workflow_config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/asset.py` & `cirro-0.6.9/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/dataset.py` & `cirro-0.6.9/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/file.py` & `cirro-0.6.9/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/helpers.py` & `cirro-0.6.9/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/portal.py` & `cirro-0.6.9/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/process.py` & `cirro-0.6.9/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/project.py` & `cirro-0.6.9/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/reference.py` & `cirro-0.6.9/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/sdk/reference_type.py` & `cirro-0.6.9/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/cirro/utils.py` & `cirro-0.6.9/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.8/pyproject.toml` & `cirro-0.6.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro"
-version = "0.6.8"
+version = "0.6.9"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Fred Hutch <cirro@fredhutch.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FredHutch/Cirro-client"
 packages = [{include = "cirro"}]
```

### Comparing `cirro-0.6.8/PKG-INFO` & `cirro-0.6.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 0.6.8
+Version: 0.6.9
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/FredHutch/Cirro-client
 License: MIT
 Author: Fred Hutch
 Author-email: cirro@fredhutch.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -146,11 +146,16 @@
 
 ### Configuration
 
 The `cirro-cli configure` command creates a file in `PW_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable. 
 
+The `transfer_max_retries` configuration property specifies the maximum number of times to attempt uploading a file to Cirro in the event of a transfer failure. 
+When uploading files to Cirro, network issues or temporary outages can occasionally cause a transfer to fail.
+It will pause for an increasing amount of time for each retry attempt.
+
 ```ini
 [General]
 base_url = data-portal.io
+transfer_max_retries = 15
 ```
```

