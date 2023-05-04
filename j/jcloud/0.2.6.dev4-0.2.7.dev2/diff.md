# Comparing `tmp/jcloud-0.2.6.dev4.tar.gz` & `tmp/jcloud-0.2.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcloud-0.2.6.dev4.tar", last modified: Wed Mar 29 12:26:13 2023, max compression
+gzip compressed data, was "jcloud-0.2.7.dev2.tar", last modified: Thu May  4 08:46:59 2023, max compression
```

## Comparing `jcloud-0.2.6.dev4.tar` & `jcloud-0.2.7.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/parsers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud/resources/project-template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/resources/project-template/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud/resources/project-template/executor1/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/resources/project-template/executor1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/resources/project-template/executor1/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/resources/project-template/executor1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/resources/project-template/flow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/jcloud/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/jcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-29 12:26:13.000000 jcloud-0.2.6.dev4/jcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 12:26:13.378723 jcloud-0.2.6.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-03-29 12:26:09.000000 jcloud-0.2.6.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.199905 jcloud-0.2.7.dev2/jcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 08:46:58.000000 jcloud-0.2.7.dev2/jcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/parsers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.195905 jcloud-0.2.7.dev2/jcloud/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud/resources/project-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/executor1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/resources/project-template/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/jcloud/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:46:59.203905 jcloud-0.2.7.dev2/jcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 08:46:59.000000 jcloud-0.2.7.dev2/jcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:46:59.207906 jcloud-0.2.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-04 08:46:54.000000 jcloud-0.2.7.dev2/setup.py
```

### Comparing `jcloud-0.2.6.dev4/LICENSE` & `jcloud-0.2.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/PKG-INFO` & `jcloud-0.2.7.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.6.dev4
+Version: 0.2.7.dev2
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.6.dev4 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.7.dev2 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.6.dev4/README.md` & `jcloud-0.2.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/__main__.py` & `jcloud-0.2.7.dev2/jcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/api.py` & `jcloud-0.2.7.dev2/jcloud/api.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/constants.py` & `jcloud-0.2.7.dev2/jcloud/constants.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/env_helper.py` & `jcloud-0.2.7.dev2/jcloud/env_helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/flow.py` & `jcloud-0.2.7.dev2/jcloud/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import json
+import yaml
 import os
 from contextlib import suppress
 from dataclasses import dataclass
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
@@ -18,15 +19,15 @@
     get_grafana_from_response,
     get_logger,
     get_or_reuse_loop,
     get_pbar,
     jcloud_logs_from_response,
     normalized,
 )
-from .normalize import validate_flow_yaml_exists
+from .normalize import get_filename_envs, validate_flow_yaml_exists, load_flow_data
 
 logger = get_logger()
 
 pbar, pb_task = get_pbar(
     '', total=2, disable='JCLOUD_NO_PROGRESSBAR' in os.environ
 )  # progress bar for deployment
 
@@ -92,18 +93,22 @@
         _data = aiohttp.FormData()
         _flow_path = Path(self.path)
 
         if _flow_path.is_dir():
             _flow_path = _flow_path / 'flow.yml'
 
         validate_flow_yaml_exists(_flow_path)
-
         if not normalized(_flow_path):
             _flow_path = flow_normalize(_flow_path)
-        _data.add_field(name='spec', value=open(_flow_path))
+            _data.add_field(name='spec', value=open(_flow_path))
+        else:
+            _flow_dict = load_flow_data(
+                _flow_path, get_filename_envs(_flow_path.parent)
+            )
+            _data.add_field(name='spec', value=yaml.dump(_flow_dict).encode())
 
         if _data._fields:
             _post_kwargs['data'] = _data
         _post_kwargs['params'] = params
         return _post_kwargs
 
     async def _deploy(self):
```

### Comparing `jcloud-0.2.6.dev4/jcloud/helper.py` & `jcloud-0.2.7.dev2/jcloud/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/normalize.py` & `jcloud-0.2.7.dev2/jcloud/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/__init__.py` & `jcloud-0.2.7.dev2/jcloud/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/base.py` & `jcloud-0.2.7.dev2/jcloud/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/custom_actions.py` & `jcloud-0.2.7.dev2/jcloud/parsers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/helper.py` & `jcloud-0.2.7.dev2/jcloud/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/list.py` & `jcloud-0.2.7.dev2/jcloud/parsers/list.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/normalize.py` & `jcloud-0.2.7.dev2/jcloud/parsers/normalize.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/parsers/remove.py` & `jcloud-0.2.7.dev2/jcloud/parsers/remove.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud/survey.py` & `jcloud-0.2.7.dev2/jcloud/survey.py`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/jcloud.egg-info/PKG-INFO` & `jcloud-0.2.7.dev2/jcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcloud
-Version: 0.2.6.dev4
+Version: 0.2.7.dev2
 Summary: Simplify deploying and managing Jina projects on Jina Cloud
 Home-page: https://github.com/jina-ai/jcloud
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/jcloud/tags
 Project-URL: Documentation, https://jcloud.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jcloud Version: 0.2.6.dev4 Summary: Simplify
+Metadata-Version: 2.1 Name: jcloud Version: 0.2.7.dev2 Summary: Simplify
 deploying and managing Jina projects on Jina Cloud Home-page: https://
 github.com/jina-ai/jcloud Author: Jina AI Author-email: hello@jina.ai License:
 Apache 2.0 Download-URL: https://github.com/jina-ai/jcloud/tags Project-URL:
 Documentation, https://jcloud.jina.ai Project-URL: Source, https://github.com/
 jina-ai/jcloud/ Project-URL: Tracker, https://github.com/jina-ai/jcloud/issues
 Keywords: jcloud neural-search serverless deployment devops mlops Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
```

### Comparing `jcloud-0.2.6.dev4/jcloud.egg-info/SOURCES.txt` & `jcloud-0.2.7.dev2/jcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcloud-0.2.6.dev4/setup.py` & `jcloud-0.2.7.dev2/setup.py`

 * *Files identical despite different names*

