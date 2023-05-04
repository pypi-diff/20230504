# Comparing `tmp/klu-0.1.1.tar.gz` & `tmp/klu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.1.tar", max compression
+gzip compressed data, was "klu-0.1.2.tar", max compression
```

## Comparing `klu-0.1.1.tar` & `klu-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,55 @@
--rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.1/LICENSE
--rw-r--r--   0        0        0      855 2023-04-02 23:20:08.166063 klu-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-04-02 23:20:08.167536 klu-0.1.1/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.1/klu/action/__init__.py
--rw-r--r--   0        0        0      141 2023-04-19 01:40:08.319896 klu-0.1.1/klu/action/constants.py
--rw-r--r--   0        0        0      554 2023-04-19 01:12:03.785445 klu-0.1.1/klu/action/errors.py
--rw-r--r--   0        0        0     3562 2023-04-19 01:43:36.380453 klu-0.1.1/klu/action/functions.py
--rw-r--r--   0        0        0     1580 2023-04-20 02:03:06.378498 klu-0.1.1/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.1/klu/api/__init__.py
--rw-r--r--   0        0        0     1423 2023-04-18 01:25:20.502447 klu-0.1.1/klu/api/client.py
--rw-r--r--   0        0        0      181 2023-04-18 01:25:20.507799 klu-0.1.1/klu/api/constants.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.1/klu/application/__init__.py
--rw-r--r--   0        0        0       31 2023-04-17 02:43:19.661060 klu-0.1.1/klu/application/constants.py
--rw-r--r--   0        0        0      277 2023-04-18 00:43:03.617342 klu-0.1.1/klu/application/errors.py
--rw-r--r--   0        0        0     1230 2023-04-19 00:20:11.870062 klu-0.1.1/klu/application/functions.py
--rw-r--r--   0        0        0      950 2023-04-20 01:38:29.343123 klu-0.1.1/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.1/klu/common/__init__.py
--rw-r--r--   0        0        0      603 2023-04-19 01:03:24.246070 klu-0.1.1/klu/common/errors.py
--rw-r--r--   0        0        0      276 2023-04-17 22:05:25.341110 klu-0.1.1/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.1/klu/data/__init__.py
--rw-r--r--   0        0        0       24 2023-04-20 00:36:52.119366 klu-0.1.1/klu/data/constants.py
--rw-r--r--   0        0        0      233 2023-04-20 00:39:03.754802 klu-0.1.1/klu/data/errors.py
--rw-r--r--   0        0        0     2841 2023-04-20 01:49:54.044344 klu-0.1.1/klu/data/functions.py
--rw-r--r--   0        0        0     2423 2023-04-20 01:50:46.204978 klu-0.1.1/klu/data/models.py
--rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.1/klu/klu.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.1/klu/workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:49.767000 klu-0.1.1/klu/workspace/functions.py
--rw-r--r--   0        0        0      878 2023-04-20 01:38:29.317735 klu-0.1.1/klu/workspace/models.py
--rw-r--r--   0        0        0     2822 2023-04-20 02:02:38.813853 klu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1535 2023-04-18 01:25:20.513445 klu-0.1.1/tests/action/test_functions.py
--rw-r--r--   0        0        0     1197 2023-04-18 00:21:35.650346 klu-0.1.1/tests/action/utils.py
--rw-r--r--   0        0        0      332 2023-04-18 01:54:53.415395 klu-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      746 2023-04-18 00:53:57.230278 klu-0.1.1/tests/utils/mock.py
--rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 klu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2789 2023-04-28 00:23:44.809946 klu-0.1.2/README.md
+-rw-r--r--   0        0        0      122 2023-04-02 23:20:08.167536 klu-0.1.2/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/action/__init__.py
+-rw-r--r--   0        0        0     3878 2023-05-01 01:27:34.131576 klu-0.1.2/klu/action/client.py
+-rw-r--r--   0        0        0       89 2023-05-01 01:27:34.107788 klu-0.1.2/klu/action/constants.py
+-rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.2/klu/action/errors.py
+-rw-r--r--   0        0        0     1598 2023-05-01 22:54:25.342198 klu-0.1.2/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.2/klu/api/__init__.py
+-rw-r--r--   0        0        0     2442 2023-05-04 00:24:02.829451 klu-0.1.2/klu/api/client.py
+-rw-r--r--   0        0        0      181 2023-05-04 00:24:02.835703 klu-0.1.2/klu/api/constants.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.2/klu/application/__init__.py
+-rw-r--r--   0        0        0     2832 2023-05-01 22:54:25.349515 klu-0.1.2/klu/application/client.py
+-rw-r--r--   0        0        0       31 2023-04-17 02:43:19.661060 klu-0.1.2/klu/application/constants.py
+-rw-r--r--   0        0        0      505 2023-04-24 00:16:52.324992 klu-0.1.2/klu/application/errors.py
+-rw-r--r--   0        0        0     2151 2023-05-01 22:54:25.348278 klu-0.1.2/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/client/__init__.py
+-rw-r--r--   0        0        0      622 2023-04-26 23:27:56.470839 klu-0.1.2/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.2/klu/common/__init__.py
+-rw-r--r--   0        0        0      962 2023-05-04 00:14:10.154872 klu-0.1.2/klu/common/errors.py
+-rw-r--r--   0        0        0     2423 2023-05-01 22:54:25.361631 klu-0.1.2/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/data/__init__.py
+-rw-r--r--   0        0        0     2618 2023-05-01 22:54:25.347409 klu-0.1.2/klu/data/client.py
+-rw-r--r--   0        0        0       24 2023-04-20 00:36:52.119366 klu-0.1.2/klu/data/constants.py
+-rw-r--r--   0        0        0      233 2023-04-20 00:39:03.754802 klu-0.1.2/klu/data/errors.py
+-rw-r--r--   0        0        0     2493 2023-05-01 22:54:25.386540 klu-0.1.2/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     7489 2023-05-04 01:05:05.363207 klu-0.1.2/klu/data_index/client.py
+-rw-r--r--   0        0        0      225 2023-05-04 01:04:40.461055 klu-0.1.2/klu/data_index/constants.py
+-rw-r--r--   0        0        0      268 2023-04-23 21:12:13.268912 klu-0.1.2/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3156 2023-05-01 22:54:25.385064 klu-0.1.2/klu/data_index/models.py
+-rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.2/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/model/__init__.py
+-rw-r--r--   0        0        0     3281 2023-04-28 01:51:36.039852 klu-0.1.2/klu/model/client.py
+-rw-r--r--   0        0        0       27 2023-04-22 00:45:10.009144 klu-0.1.2/klu/model/constants.py
+-rw-r--r--   0        0        0      643 2023-04-23 19:07:01.206218 klu-0.1.2/klu/model/errors.py
+-rw-r--r--   0        0        0      833 2023-05-01 22:54:25.419198 klu-0.1.2/klu/model/models.py
+-rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.2/klu/utils/file_upload.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     4021 2023-05-04 00:25:09.454757 klu-0.1.2/klu/workspace/client.py
+-rw-r--r--   0        0        0      253 2023-05-03 23:42:48.098523 klu-0.1.2/klu/workspace/constants.py
+-rw-r--r--   0        0        0      196 2023-04-23 19:49:57.843593 klu-0.1.2/klu/workspace/errors.py
+-rw-r--r--   0        0        0      669 2023-05-03 23:39:56.994407 klu-0.1.2/klu/workspace/models.py
+-rw-r--r--   0        0        0     2842 2023-05-04 01:08:37.494710 klu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/tests/action/__init__.py
+-rw-r--r--   0        0        0     1588 2023-05-01 01:21:25.458436 klu-0.1.2/tests/action/test_client.py
+-rw-r--r--   0        0        0     1197 2023-04-18 00:21:35.650346 klu-0.1.2/tests/action/utils.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/tests/application/__init__.py
+-rw-r--r--   0        0        0     1349 2023-05-01 01:37:34.296750 klu-0.1.2/tests/application/test_client.py
+-rw-r--r--   0        0        0     1072 2023-05-01 01:38:35.627510 klu-0.1.2/tests/application/utils.py
+-rw-r--r--   0        0        0      489 2023-05-01 01:18:06.958729 klu-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.2/tests/utils/mock.py
+-rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 klu-0.1.2/PKG-INFO
```

### Comparing `klu-0.1.1/LICENSE` & `klu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.1/klu/action/errors.py` & `klu-0.1.2/klu/action/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,11 +6,10 @@
         self.message = f"Action with id {action_id} was not found."
         super().__init__(self.message)
 
 
 class InvalidActionPromptData(Exception):
     def __init__(self, response_message: str):
         self.message = (
-            f"Failed to run the action due to the invalid request parameters. "
-            f"Response message: {response_message}"
+            f"Failed to run the action due to the invalid request parameters. " f"Response message: {response_message}"
         )
         super().__init__(self.message)
```

### Comparing `klu-0.1.1/klu/action/functions.py` & `klu-0.1.2/klu/action/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,101 @@
 from typing import Optional
 
 import aiohttp
-
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.common.errors import (
-    UnknownKluError,
-    UnknownKluAPIError,
-    WorkspaceNotFoundError,
-)
 from klu.api.client import APIClient
+from klu.common.models import KluClientBase
+from klu.workspace.errors import WorkspaceOrUserNotFoundError
+from klu.common.errors import UnknownKluAPIError, UnknownKluError
 from klu.action.errors import ActionNotFoundError, InvalidActionPromptData
 from klu.action.models import ActionPromptResponse, PlaygroundPromptResponse
-from klu.action.constants import ACTION_PROMPT_ENDPOINT, PLAYGROUND_PROMPT_ENDPOINT
+from klu.action.constants import ACTION_ENDPOINT, PLAYGROUND_PROMPT_ENDPOINT
 
 
-async def run_action_prompt(
-    action_id: str,
-    prompt: str,
-    filter: Optional[str] = None,
-    streaming: Optional[str] = None,
-) -> ActionPromptResponse:
-    """
-    Run a prompt with an agent, optionally using streaming.
-
-    Args:
-        prompt (str): The prompt to run with the agent.
-        action_id (str): The GUID of the agent to run the prompt with.
-        filter (Optional[str]): The filter to use when running the prompt.
-        streaming (Optional[str]): Whether to use streaming or not. Set to "true" if you want to enable streaming
-
-    Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
-    """
-    async with aiohttp.ClientSession() as session:
-        client = APIClient(session)
-        try:
-            response = await client.post(
-                ACTION_PROMPT_ENDPOINT,
-                {
-                    "filter": filter,
-                    "prompt": prompt,
-                    "agent": action_id,
-                    "streaming": streaming,
-                },
-            )
-        except (HTTPNotFound, ClientResponseError) as e:
-            if e.status == 404:
-                raise ActionNotFoundError(action_id)
-
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
-
-        return ActionPromptResponse(**response)
-
-
-async def run_playground_prompt(
-    prompt: str,
-    model_id: str,
-    tool_ids: Optional[list] = None,
-    index_ids: Optional[list] = None,
-    model_config: Optional[dict] = None,
-) -> PlaygroundPromptResponse:
-    """
-    Run a prompt with an agent, optionally using streaming.
-
-    Args:
-        prompt (str): The prompt to run.
-        model_id (int): The ID of the model to use.
-        tool_ids (list): Optional list of tool IDs to use. Defaults to an empty array
-        index_ids (list): Optional list of index IDs to use. Defaults to an empty array
-        model_config (dict): Optional configuration of the model
-
-    Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
-    """
-    tool_ids = tool_ids or []
-    index_ids = index_ids or []
-
-    async with aiohttp.ClientSession() as session:
-        client = APIClient(session)
-        try:
-            response = await client.post(
-                PLAYGROUND_PROMPT_ENDPOINT,
-                {
-                    "prompt": prompt,
-                    "toolIds": tool_ids,
-                    "modelId": model_id,
-                    "indexIds": index_ids,
-                    "modelConfig": model_config,
-                },
-            )
-        except (HTTPNotFound, ClientResponseError) as e:
-            if e.status == 404:
-                raise WorkspaceNotFoundError()
-            if e.status == 400:
-                raise InvalidActionPromptData(e.message)
-
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
+class ActionsClient(KluClientBase):
+    async def run_action_prompt(
+        self,
+        action_id: str,
+        prompt: str,
+        filter: Optional[str] = None,
+        streaming: Optional[str] = None,
+    ) -> ActionPromptResponse:
+        """
+        Run a prompt with an agent, optionally using streaming.
+
+        Args:
+            prompt (str): The prompt to run with the agent.
+            action_id (str): The GUID of the agent to run the prompt with.
+            filter (Optional[str]): The filter to use when running the prompt.
+            streaming (Optional[str]): Whether to use streaming or not. Set to "true" if you want to enable streaming
+
+        Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
+        """
+        async with aiohttp.ClientSession() as session:
+            client = APIClient(session, self.api_key)
+
+            try:
+                response = await client.post(
+                    ACTION_ENDPOINT,
+                    {
+                        "filter": filter,
+                        "prompt": prompt,
+                        "agent": action_id,
+                        "streaming": streaming,
+                    },
+                )
+            except (HTTPNotFound, ClientResponseError) as e:
+                if e.status == 404:
+                    raise ActionNotFoundError(action_id)
+
+                raise UnknownKluAPIError(e.status, e.message)
+            except Exception:
+                raise UnknownKluError()
+
+            return ActionPromptResponse(**response)
+
+    async def run_playground_prompt(
+        self,
+        prompt: str,
+        model_id: str,
+        tool_ids: Optional[list] = None,
+        index_ids: Optional[list] = None,
+        model_config: Optional[dict] = None,
+    ) -> PlaygroundPromptResponse:
+        """
+        Run a prompt with an agent, optionally using streaming.
+
+        Args:
+            prompt (str): The prompt to run.
+            model_id (int): The ID of the model to use.
+            tool_ids (list): Optional list of tool IDs to use. Defaults to an empty array
+            index_ids (list): Optional list of index IDs to use. Defaults to an empty array
+            model_config (dict): Optional configuration of the model
+
+        Returns: An object result of running the prompt with the message and a feedback_url for providing feedback.
+        """
+        tool_ids = tool_ids or []
+        index_ids = index_ids or []
+
+        async with aiohttp.ClientSession() as session:
+            client = APIClient(session, self.api_key)
+
+            try:
+                response = await client.post(
+                    PLAYGROUND_PROMPT_ENDPOINT,
+                    {
+                        "prompt": prompt,
+                        "toolIds": tool_ids,
+                        "modelId": model_id,
+                        "indexIds": index_ids,
+                        "modelConfig": model_config,
+                    },
+                )
+            except (HTTPNotFound, ClientResponseError) as e:
+                if e.status == 404:
+                    raise WorkspaceOrUserNotFoundError()
+                if e.status == 400:
+                    raise InvalidActionPromptData(e.message)
 
-        return PlaygroundPromptResponse(**response)
+            return PlaygroundPromptResponse(**response)
```

### Comparing `klu-0.1.1/klu/action/models.py` & `klu-0.1.2/klu/action/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     model_config: Optional[dict]
     experiment_id: Optional[int] = None
     updated_at: Optional[datetime] = None
     created_at: datetime = datetime.utcnow()
 
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Action":
-        return cls(
+        return cls._create_instance(
             **{
                 "app_id": data.pop("appId", None),
                 "model_id": data.pop("modelId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
                 "experiment_id": data.pop("experimentId", None),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
         base_dict = asdict(self)
 
         return {
             "appId": base_dict.pop("app_id"),
```

### Comparing `klu-0.1.1/klu/application/models.py` & `klu-0.1.2/klu/model/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-from typing import Optional
 from datetime import datetime
 from dataclasses import dataclass, asdict
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Application(BaseEngineModel):
+class Model(BaseEngineModel):
     guid: str
-    name: str
-    app_type: str
-    enabled: bool
-
-    description: Optional[str]
-    model_config: Optional[dict]
-    deleted: Optional[bool] = None
-    updated_at: Optional[datetime] = None
+    provider: str
+    model_name: str
+    updated_at: datetime = datetime.utcnow()
     created_at: datetime = datetime.utcnow()
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Application":
-        return cls(
+    def _from_engine_format(cls, data: dict) -> "Model":
+        return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt"),
                 "created_at": data.pop("createdAt"),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self)
+        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
-        return {
-            "updatedAt": base_dict.pop('updated_at'),
-            "createdAt": base_dict.pop('created_at'),
-            **base_dict,
-        }
+        base_dict.pop("updated_at", None)
+        base_dict.pop("created_at", None)
+
+        return base_dict
```

### Comparing `klu-0.1.1/klu/common/errors.py` & `klu-0.1.2/klu/common/errors.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,11 +8,22 @@
     def __init__(self, status: int, message: str):
         self.message = (
             f"Unknown error in Klu API.\nstatus_code: {status},\nmessage: {message}"
         )
         super().__init__(self.message)
 
 
-class WorkspaceNotFoundError(Exception):
+class UnauthorizedError(Exception):
     def __init__(self):
-        self.message = "Workspace not found for provided API key."
+        self.message = (
+            f"Wrong credentials used to access the API. "
+            f"Please, check you set the correct API key or contact the support team."
+        )
+        super().__init__(self.message)
+
+
+class BadRequestAPIError(Exception):
+    def __init__(self, status: int, message: str):
+        self.message = (
+            f"BadRequest error in Klu API.\nstatus_code: {status},\nmessage: {message}"
+        )
         super().__init__(self.message)
```

### Comparing `klu-0.1.1/klu/data/functions.py` & `klu-0.1.2/klu/data/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,71 @@
-import aiohttp
-
 from typing import List
+
+import aiohttp
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
-from klu.api.client import APIClient
-from klu.data.models import Data, ActionData, DataBaseClass
+from klu.common.models import KluClientBase
 from klu.data.constants import DATA_ENDPOINT
 from klu.data.errors import DataNotFoundError
 from klu.action.errors import ActionNotFoundError
-from klu.common.errors import UnknownKluAPIError, UnknownKluError
+from klu.data.models import DataBaseClass, Data, ActionData
 
 
-async def get_action_data(action_guid: str) -> List[ActionData]:
-    """
-    Retrieves data information for an action.
-
-    Args:
-        action_guid (str): Guid of an action to fetch data for.
-
-    Returns: An array of actions found by provided app id.
-    """
-    async with aiohttp.ClientSession() as session:
-        client = APIClient(session)
-        try:
-            response = await client.get(f"{DATA_ENDPOINT}", {"agent": action_guid})
-        except (HTTPNotFound, ClientResponseError) as e:
-            if e.status == 404:
-                raise ActionNotFoundError(action_guid)
-
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
-
-        return [ActionData._from_engine_format(data) for data in response]
-
-
-async def get_single_datum(datum_id: int) -> Data:
-    """
-    Retrieves data information based on the data ID.
-
-    Args:
-        datum_id (str): ID of a datum object to fetch.
-
-    Returns: An object
-    """
-    async with aiohttp.ClientSession() as session:
-        client = APIClient(session)
-        try:
-            response = await client.get(f"{DATA_ENDPOINT}/{datum_id}")
-        except (HTTPNotFound, ClientResponseError) as e:
-            if e.status == 404:
-                raise DataNotFoundError(datum_id)
-
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
-
-        return Data._from_engine_format(response)
-
-
-async def update_single_datum(datum_id: int, datum_data: DataBaseClass) -> dict:
-    """
-    Updated data information based on the data ID and provided payload.
-
-    Args:
-        datum_id (str): ID of a datum object to update.
-        datum_data (DataBaseClass): datum data to update
-
-    Returns: Dictionary with a 'message' key containing successful update message
-    """
-    async with aiohttp.ClientSession() as session:
-        client = APIClient(session)
-        try:
-            response = await client.post(
-                f"{DATA_ENDPOINT}/{datum_id}", datum_data._to_engine_format()
-            )
-        except (HTTPNotFound, ClientResponseError) as e:
-            if e.status == 404:
-                raise DataNotFoundError(datum_id)
-
-            raise UnknownKluAPIError(e.status, e.message)
-        except Exception:
-            raise UnknownKluError()
+class DataClient(KluClientBase):
+    async def get(self, datum_id: str) -> Data:
+        """
+        Retrieves data information based on the data ID.
+
+        Args:
+            datum_id (str): ID of a datum object to fetch.
+
+        Returns: An object
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self.get_client(session)
+            try:
+                response = await client.get(f"{DATA_ENDPOINT}/{datum_id}")
+            except (HTTPNotFound, ClientResponseError) as e:
+                if e.status == 404:
+                    raise DataNotFoundError(datum_id)
+
+            return Data._from_engine_format(response)
+
+    async def update(self, datum_id: int, datum_data: DataBaseClass) -> dict:
+        """
+        Updated data information based on the data ID and provided payload.
+
+        Args:
+            datum_id (str): ID of a datum object to update.
+            datum_data (DataBaseClass): datum data to update
+
+        Returns: Dictionary with a 'message' key containing successful update message
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self.get_client(session)
+            try:
+                response = await client.post(f"{DATA_ENDPOINT}/{datum_id}", datum_data._to_engine_format())
+            except (HTTPNotFound, ClientResponseError) as e:
+                if e.status == 404:
+                    raise DataNotFoundError(datum_id)
+
+            return {"message": response.get("message")}
+
+    async def get_data_for_action(self, action_guid: str) -> List[ActionData]:
+        """
+        Retrieves data information for an action.
+
+        Args:
+            action_guid (str): Guid of an action to fetch data for.
+
+        Returns: An array of actions found by provided app id.
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self.get_client(session)
+            try:
+                response = await client.get(f"{DATA_ENDPOINT}", {"agent": action_guid})
+            except (HTTPNotFound, ClientResponseError) as e:
+                if e.status == 404:
+                    raise ActionNotFoundError(action_guid)
 
-        return {"message": response.get("message")}
+            return [ActionData._from_engine_format(data) for data in response]
```

### Comparing `klu-0.1.1/klu/data/models.py` & `klu-0.1.2/klu/data/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,71 +25,66 @@
     rating: Optional[int] = None
     metadata: Optional[dict] = None
     correction: Optional[str] = None
     updated_at: datetime = datetime.utcnow()
     created_at: datetime = datetime.utcnow()
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "BaseEngineModel":
-        return cls(
+    def _from_engine_format(cls, data: dict) -> "DataBaseClass":
+        return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt"),
                 "created_at": data.pop("createdAt"),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(
-            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
-        )
+        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
 
 
+# We need this way of inheritance to append optional field after the required ones.
 @dataclass
 class Data(DataBaseClass, DataWithId):
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Data":
-        return cls(
+        return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt"),
                 "created_at": data.pop("createdAt"),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(
-            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
-        )
+        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
 
 
 @dataclass
 class ActionData(DataBaseClass, DataWithFeedbackUrl):
     @classmethod
     def _from_engine_format(cls, data: dict) -> "ActionData":
-        return cls(
+        return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt"),
                 "created_at": data.pop("createdAt"),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(
-            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
-        )
+        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
```

### Comparing `klu-0.1.1/klu/workspace/models.py` & `klu-0.1.2/klu/workspace/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-from typing import Optional
 from uuid import UUID, uuid4
-from datetime import datetime
-from dataclasses import dataclass, field, asdict
+from dataclasses import dataclass, asdict
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class Workspace(BaseEngineModel):
-    id: int
     name: str
-
+    created_by_id: str
     project_guid: UUID = uuid4()
-    updated_at: Optional[datetime] = None
-    created_at: datetime = datetime.utcnow()
 
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Workspace":
-        return cls(
+        return cls._create_instance(
             **{
-                "updated_at": data.pop("updatedAt"),
-                "created_at": data.pop("createdAt"),
+                "created_by_id": data.pop("createdById", None),
             },
-            **data
+            **data,
         )
 
     def _to_engine_format(self) -> dict:
         base_dict = asdict(self)
 
         return {
-            "updatedAt": base_dict.pop('updated_at'),
-            "createdAt": base_dict.pop('created_at'),
+            "createdById": base_dict.pop("created_by_id", None),
             **base_dict,
         }
```

### Comparing `klu-0.1.1/pyproject.toml` & `klu-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.1"
+version = "0.1.2"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
 authors = ["Stefan Sabev <stefan@launchpad.pm>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -22,14 +22,15 @@
     { include = "klu" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4.0"
 aiohttp = "3.8.4"
+aiofiles = "23.1.0"
 
 black  = { version = "^21.5b2", optional = true}
 isort  = { version = "^5.8.0", optional = true}
 flake8  = { version = "^3.9.2", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 mypy = {version = "^0.900", optional = true}
 pytest  = { version = "^6.2.4", optional = true}
```

### Comparing `klu-0.1.1/tests/action/test_functions.py` & `klu-0.1.2/tests/application/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 #!/usr/bin/env python
 """Tests for `action` module functions"""
 import pytest
 
 from aiohttp import web
 from unittest.mock import patch
 
-from tests.action.utils import get_action_data
+from klu.client.klu import KluClient
 from klu.application.errors import ApplicationNotFoundError
-from klu.application.functions import get_application_actions
+from tests.application.utils import get_application_data
 from tests.utils.mock import (
     get_api_client_mock,
     client_get_function_mock,
     get_return_value_side_effect,
 )
 
 
 @pytest.mark.asyncio
-@patch("klu.application.functions.APIClient", new_callable=get_api_client_mock)
-async def test_get_app_actions_converts_response_to_dataclass_provided_valid_response_dicts(
-    client_mock,
+@patch("klu.application.client.APIClient", new_callable=get_api_client_mock)
+async def test_get_app_converts_response_to_dataclass_provided_valid_response_dicts(
+    client_mock, klu_client: KluClient
 ):
-    action_1_guid = "test_action_1"
-    action_2_guid = "test_action_2"
-
-    test_action_1 = get_action_data(guid=action_1_guid)
-    test_action_2 = get_action_data(guid=action_2_guid)
+    test_app_guid = "test-guid"
 
     client_mock.get = client_get_function_mock(
-        get_return_value_side_effect([test_action_1, test_action_2])
+        get_return_value_side_effect(get_application_data(guid=test_app_guid))
     )
-    result = await get_application_actions("test")
+    result = await klu_client.applications.get("test")
 
-    assert len(result) == 2
-    assert result[0].guid == action_1_guid
-    assert result[1].guid == action_2_guid
+    assert result.guid == test_app_guid
 
 
 @pytest.mark.asyncio
-@patch("klu.application.functions.APIClient", new_callable=get_api_client_mock)
-async def test_get_app_actions_raises_klu_error_provided_404_response_from_api(
-    client_mock,
+@patch("klu.application.client.APIClient", new_callable=get_api_client_mock)
+async def test_get_app_raises_klu_error_provided_404_response_from_api(
+    client_mock, klu_client: KluClient
 ):
     client_mock.get = client_get_function_mock(web.HTTPNotFound())
     with pytest.raises(Exception) as exc_info:
-        await get_application_actions("test")
+        await klu_client.applications.get_actions_for_app("test")
 
     assert exc_info.type is ApplicationNotFoundError
```

### Comparing `klu-0.1.1/tests/action/utils.py` & `klu-0.1.2/tests/action/utils.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.1/tests/utils/mock.py` & `klu-0.1.2/tests/utils/mock.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any
-from unittest.mock import MagicMock, AsyncMock
+from unittest.mock import MagicMock
+
+from asyncmock import AsyncMock
 
 
 class APIClientMock:
     def __init__(self, *_args: Any, **_kwargs: Any):
         self.session = MagicMock()
 
     async def get(self):
```

