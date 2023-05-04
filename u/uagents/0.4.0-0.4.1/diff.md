# Comparing `tmp/uagents-0.4.0.tar.gz` & `tmp/uagents-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents-0.4.0.tar", max compression
+gzip compressed data, was "uagents-0.4.1.tar", max compression
```

## Comparing `uagents-0.4.0.tar` & `uagents-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.4.0/LICENSE
--rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.4.0/README.md
--rw-r--r--   0        0        0      909 2023-04-17 14:00:08.389315 uagents-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.4.0/src/uagents/__init__.py
--rw-r--r--   0        0        0    16085 2023-04-17 13:29:50.196085 uagents-0.4.0/src/uagents/agent.py
--rw-r--r--   0        0        0     5651 2023-04-17 13:29:50.200085 uagents-0.4.0/src/uagents/asgi.py
--rw-r--r--   0        0        0     2269 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/config.py
--rw-r--r--   0        0        0     4979 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/context.py
--rw-r--r--   0        0        0        0 2023-03-02 16:19:41.886178 uagents-0.4.0/src/uagents/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-02 16:20:26.910313 uagents-0.4.0/src/uagents/contrib/protocols/__init__.py
--rw-r--r--   0        0        0     1312 2023-03-07 14:38:10.652721 uagents-0.4.0/src/uagents/contrib/protocols/protocol_query.py
--rw-r--r--   0        0        0     4148 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/crypto/__init__.py
--rw-r--r--   0        0        0     1038 2023-02-24 13:37:53.457125 uagents-0.4.0/src/uagents/dispatch.py
--rw-r--r--   0        0        0     1423 2023-02-24 13:37:53.457125 uagents-0.4.0/src/uagents/envelope.py
--rw-r--r--   0        0        0     6796 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/mailbox.py
--rw-r--r--   0        0        0      464 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/models.py
--rw-r--r--   0        0        0     1737 2023-04-17 08:26:12.076548 uagents-0.4.0/src/uagents/network.py
--rw-r--r--   0        0        0     6661 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/protocol.py
--rw-r--r--   0        0        0     2113 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/query.py
--rw-r--r--   0        0        0     1339 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/resolver.py
--rw-r--r--   0        0        0     1153 2023-03-24 09:42:09.546004 uagents-0.4.0/src/uagents/setup.py
--rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.4.0/src/uagents/storage/__init__.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 uagents-0.4.0/setup.py
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 uagents-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.4.1/README.md
+-rw-r--r--   0        0        0      916 2023-05-04 14:30:04.770060 uagents-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.4.1/src/uagents/__init__.py
+-rw-r--r--   0        0        0    16441 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/agent.py
+-rw-r--r--   0        0        0     5651 2023-05-02 11:10:48.559062 uagents-0.4.1/src/uagents/asgi.py
+-rw-r--r--   0        0        0     2363 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/config.py
+-rw-r--r--   0        0        0     4979 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/context.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:19:41.886178 uagents-0.4.1/src/uagents/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-02 16:20:26.910313 uagents-0.4.1/src/uagents/contrib/protocols/__init__.py
+-rw-r--r--   0        0        0     1312 2023-03-07 14:38:10.652721 uagents-0.4.1/src/uagents/contrib/protocols/protocol_query.py
+-rw-r--r--   0        0        0     4148 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/crypto/__init__.py
+-rw-r--r--   0        0        0     1038 2023-02-24 13:37:53.457125 uagents-0.4.1/src/uagents/dispatch.py
+-rw-r--r--   0        0        0     1423 2023-02-24 13:37:53.457125 uagents-0.4.1/src/uagents/envelope.py
+-rw-r--r--   0        0        0     6796 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/mailbox.py
+-rw-r--r--   0        0        0      464 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/models.py
+-rw-r--r--   0        0        0     1737 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/network.py
+-rw-r--r--   0        0        0     6661 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/protocol.py
+-rw-r--r--   0        0        0     2113 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/query.py
+-rw-r--r--   0        0        0     1339 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/resolver.py
+-rw-r--r--   0        0        0     1153 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/setup.py
+-rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.4.1/src/uagents/storage/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 uagents-0.4.1/setup.py
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 uagents-0.4.1/PKG-INFO
```

### Comparing `uagents-0.4.0/LICENSE` & `uagents-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/README.md` & `uagents-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/pyproject.toml` & `uagents-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "uagents"
-version = "0.4.0"
+version = "0.4.1"
 description = "Lightweight framework for rapid agent-based development"
 authors = ["Ed FitzGerald <edward.fitzgerald@fetch.ai>", "James Riehl <james.riehl@fetch.ai>", "Alejandro Morales <alejandro.madrigal@fetch.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.11"
 pydantic = "^1.10.2"
 msgpack = "^1.0.4"
 bech32 = "^1.2.0"
 ecdsa = "^0.18.0"
 apispec = "^6.0.2"
 uvicorn = "^0.19.0"
 aiohttp = "^3.8.3"
-cosmpy = "^0.6.0"
+cosmpy = "^0.7.0"
 websockets = "^10.4"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 pytest = "^7.1.3"
 pylint = "^2.15.3"
 mkdocs = "^1.4.2"
```

### Comparing `uagents-0.4.0/src/uagents/agent.py` & `uagents-0.4.1/src/uagents/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import functools
-from typing import Dict, List, Optional, Set, Union, Type, Tuple
+from typing import Dict, List, Optional, Set, Union, Type, Tuple, Any
 
 from cosmpy.aerial.wallet import LocalWallet, PrivateKey
 from cosmpy.crypto.address import Address
 
 from uagents.asgi import ASGIServer
 from uagents.context import (
     Context,
@@ -50,15 +50,15 @@
 
 class Agent(Sink):
     def __init__(
         self,
         name: Optional[str] = None,
         port: Optional[int] = None,
         seed: Optional[str] = None,
-        endpoint: Optional[Union[List[str], Dict[str, dict]]] = None,
+        endpoint: Optional[Union[str, List[str], Dict[str, dict]]] = None,
         mailbox: Optional[Union[str, Dict[str, str]]] = None,
         resolve: Optional[Resolver] = None,
         version: Optional[str] = None,
     ):
         self._name = name
         self._port = port if port is not None else 8000
         self._background_tasks: Set[asyncio.Task] = set()
@@ -180,14 +180,17 @@
 
     def sign_registration(self) -> str:
         assert self._reg_contract.address is not None
         return self._identity.sign_registration(
             str(self._reg_contract.address), self.get_registration_sequence()
         )
 
+    def update_endpoints(self, endpoints: List[Dict[str, Any]]):
+        self._endpoints = endpoints
+
     def update_loop(self, loop):
         self._loop = loop
 
     def update_queries(self, queries):
         self._queries = queries
 
     async def _register(self, ctx: Context):
@@ -332,14 +335,18 @@
         for handler in self._on_shutdown:
             await handler(self._ctx)
 
     def setup(self):
         # register the internal agent protocol
         self.include(self._protocol)
         self._loop.run_until_complete(self._startup())
+        if self._endpoints is None:
+            self._logger.warning(
+                "I have no endpoint and won't be able to receive external messages"
+            )
         self.start_background_tasks()
 
     def start_background_tasks(self):
         # Start the interval tasks
         for func, period in self._interval_handlers:
             task = self._loop.create_task(_run_interval(func, self._ctx, period))
             self._background_tasks.add(task)
@@ -351,18 +358,14 @@
         task.add_done_callback(self._background_tasks.discard)
 
         # start the contract registration update loop
         if self._endpoints is not None:
             self._loop.create_task(
                 _run_interval(self._register, self._ctx, self._schedule_registration())
             )
-        else:
-            self._logger.warning(
-                "I have no endpoint and won't be able to receive external messages"
-            )
 
     def run(self):
         self.setup()
         try:
             if self._use_mailbox:
                 self._loop.create_task(self._mailbox_client.process_deletion_queue())
                 self._loop.run_until_complete(self._mailbox_client.run())
@@ -419,28 +422,35 @@
                     continue
 
             if handler is not None:
                 await handler(context, sender, recovered)
 
 
 class Bureau:
-    def __init__(self, port: Optional[int] = None):
+    def __init__(
+        self,
+        port: Optional[int] = None,
+        endpoint: Optional[Union[str, List[str], Dict[str, dict]]] = None,
+    ):
         self._loop = asyncio.get_event_loop_policy().get_event_loop()
         self._agents = []
+        self._endpoints = parse_endpoint_config(endpoint)
         self._port = port or 8000
         self._queries: Dict[str, asyncio.Future] = {}
         self._logger = get_logger("bureau")
         self._server = ASGIServer(self._port, self._loop, self._queries, self._logger)
         self._use_mailbox = False
 
     def add(self, agent: Agent):
         agent.update_loop(self._loop)
         agent.update_queries(self._queries)
         if agent.mailbox is not None:
             self._use_mailbox = True
+        else:
+            agent.update_endpoints(self._endpoints)
         self._agents.append(agent)
 
     def run(self):
         tasks = []
         for agent in self._agents:
             agent.setup()
             if agent.mailbox is not None:
```

### Comparing `uagents-0.4.0/src/uagents/asgi.py` & `uagents-0.4.1/src/uagents/asgi.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/config.py` & `uagents-0.4.1/src/uagents/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 MAILBOX_SERVER_URL = "wss://agentverse.ai"
 MAILBOX_POLL_INTERVAL_SECONDS = 1.0
 
 DEFAULT_ENVELOPE_TIMEOUT_SECONDS = 30
 
 
 def parse_endpoint_config(
-    endpoint: Optional[Union[List[str], Dict[str, dict]]]
+    endpoint: Optional[Union[str, List[str], Dict[str, dict]]]
 ) -> List[Dict[str, Any]]:
     if isinstance(endpoint, dict):
         endpoints = [
             {"url": val[0], "weight": val[1].get("weight") or 1}
             for val in endpoint.items()
         ]
     elif isinstance(endpoint, list):
         endpoints = [{"url": val, "weight": 1} for val in endpoint]
+    elif isinstance(endpoint, str):
+        endpoints = [{"url": endpoint, "weight": 1}]
     else:
         endpoints = None
     return endpoints
 
 
 def parse_mailbox_config(mailbox: Union[str, Dict[str, str]]) -> Dict[str, str]:
     api_key = None
```

### Comparing `uagents-0.4.0/src/uagents/context.py` & `uagents-0.4.1/src/uagents/context.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/contrib/protocols/protocol_query.py` & `uagents-0.4.1/src/uagents/contrib/protocols/protocol_query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/crypto/__init__.py` & `uagents-0.4.1/src/uagents/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/dispatch.py` & `uagents-0.4.1/src/uagents/dispatch.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/envelope.py` & `uagents-0.4.1/src/uagents/envelope.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/mailbox.py` & `uagents-0.4.1/src/uagents/mailbox.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/network.py` & `uagents-0.4.1/src/uagents/network.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/protocol.py` & `uagents-0.4.1/src/uagents/protocol.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/query.py` & `uagents-0.4.1/src/uagents/query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/resolver.py` & `uagents-0.4.1/src/uagents/resolver.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/setup.py` & `uagents-0.4.1/src/uagents/setup.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/src/uagents/storage/__init__.py` & `uagents-0.4.1/src/uagents/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.0/setup.py` & `uagents-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0',
  'apispec>=6.0.2,<7.0.0',
  'bech32>=1.2.0,<2.0.0',
- 'cosmpy>=0.6.0,<0.7.0',
+ 'cosmpy>=0.7.0,<0.8.0',
  'ecdsa>=0.18.0,<0.19.0',
  'msgpack>=1.0.4,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'uvicorn>=0.19.0,<0.20.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'uagents',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Lightweight framework for rapid agent-based development',
     'long_description': 'The **μAgents** (micro-Agents) project is a fast and lightweight framework that makes it easy to build agents for all kinds of decentralised use cases.\n\n## Installation\n\nInstall μAgents for Python 3.8, 3.9, or 3.10:\n\n```bash\npoetry install\npoetry shell\n```\n\n## Documentation\n\nBuild and run the docs locally with:\n\n```bash\nmkdocs serve\n```\n\nOr go to the official docs site: https://docs.fetch.ai/uAgents.\n\n## Examples\n\nThe [`examples`](https://github.com/fetchai/uAgents/tree/main/examples) folder contains several examples of how to create and run various types of agents.\n\n## Contributing\n\nAll contributions are welcome! Remember, contribution includes not only code, but any help with docs or issues raised by other developers. See our [contribution guidelines](https://github.com/fetchai/uAgents/blob/main/CONTRIBUTING.md) for more details.\n\n### Development Guidelines\n\nRead our [development guidelines](https://github.com/fetchai/uAgents/blob/main/DEVELOPING.md) to learn some useful tips related to development.\n\n### Issues, Questions and Discussions\n\nWe use [GitHub Issues](https://github.com/fetchai/uAgents/issues) for tracking requests and bugs, and [GitHub Discussions](https://github.com/fetchai/uAgents/discussions) for general questions and discussion.\n\n## License\n\nThe μAgents project is licensed under [Apache License 2.0](https://github.com/fetchai/uAgents/blob/main/LICENSE).\n\n',
     'author': 'Ed FitzGerald',
     'author_email': 'edward.fitzgerald@fetch.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `uagents-0.4.0/PKG-INFO` & `uagents-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: uagents
-Version: 0.4.0
+Version: 0.4.1
 Summary: Lightweight framework for rapid agent-based development
 License: Apache 2.0
 Author: Ed FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: apispec (>=6.0.2,<7.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
-Requires-Dist: cosmpy (>=0.6.0,<0.7.0)
+Requires-Dist: cosmpy (>=0.7.0,<0.8.0)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Description-Content-Type: text/markdown
```

