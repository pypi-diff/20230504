# Comparing `tmp/fastapi_async_langchain-0.4.1.tar.gz` & `tmp/fastapi_async_langchain-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.4.1.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.4.2.tar", max compression
```

## Comparing `fastapi_async_langchain-0.4.1.tar` & `fastapi_async_langchain-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-05-03 09:40:30.718850 fastapi_async_langchain-0.4.1/LICENSE
--rw-r--r--   0        0        0     1713 2023-05-03 09:40:30.718850 fastapi_async_langchain-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      509 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      273 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/__init__.py
--rw-r--r--   0        0        0      784 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/base.py
--rw-r--r--   0        0        0      896 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py
--rw-r--r--   0        0        0      257 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/__init__.py
--rw-r--r--   0        0        0      971 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/base.py
--rw-r--r--   0        0        0     1178 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py
--rw-r--r--   0        0        0      171 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2502 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0      725 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0      782 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      536 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0      281 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     2907 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0      927 2023-05-03 09:40:30.898851 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/llm.py
--rw-r--r--   0        0        0      985 2023-05-03 09:40:30.902850 fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/retrieval_qa.py
--rw-r--r--   0        0        0      481 2023-05-03 09:40:30.902850 fastapi_async_langchain-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-03 19:50:26.322104 fastapi_async_langchain-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1713 2023-05-03 19:50:26.322104 fastapi_async_langchain-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 19:50:26.550104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-03 19:50:26.550104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/streaming/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/streaming/base.py
+-rw-r--r--   0        0        0      896 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py
+-rw-r--r--   0        0        0      257 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/websocket/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/websocket/base.py
+-rw-r--r--   0        0        0     1178 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py
+-rw-r--r--   0        0        0      171 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2502 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0      727 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0      782 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      536 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0      281 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     2907 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      928 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/llm.py
+-rw-r--r--   0        0        0      985 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/retrieval_qa.py
+-rw-r--r--   0        0        0      481 2023-05-03 19:50:26.554104 fastapi_async_langchain-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.2/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.4.1/LICENSE` & `fastapi_async_langchain-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/README.md` & `fastapi_async_langchain-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/base.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/base.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/websocket/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/base.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/llm.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
     def _create_chain_executor(
         chain: LLMChain, inputs: Union[Dict[str, Any], Any]
     ) -> Callable[[Send], Awaitable[Any]]:
         async def wrapper(send: Send):
-            return await chain.arun(
-                input=inputs, callbacks=[AsyncLLMChainStreamingCallback(send=send)]
+            return await chain.acall(
+                inputs=inputs, callbacks=[AsyncLLMChainStreamingCallback(send=send)]
             )
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/responses/retrieval_qa.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/responses/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/llm.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @staticmethod
     def _create_chain_executor(
         chain: LLMChain,
         websocket: WebSocket,
         response: WebsocketResponse,
     ) -> Callable[[], Awaitable[Any]]:
         async def wrapper(user_message: str):
-            return await chain.arun(
+            return await chain.acall(
                 inputs=user_message,
                 callbacks=[
                     AsyncLLMChainWebsocketCallback(
                         websocket=websocket, response=response
                     )
                 ],
             )
```

### Comparing `fastapi_async_langchain-0.4.1/fastapi_async_langchain/websockets/retrieval_qa.py` & `fastapi_async_langchain-0.4.2/fastapi_async_langchain/websockets/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.1/PKG-INFO` & `fastapi_async_langchain-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.4.1
+Version: 0.4.2
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

