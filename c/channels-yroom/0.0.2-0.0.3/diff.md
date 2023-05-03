# Comparing `tmp/channels_yroom-0.0.2.tar.gz` & `tmp/channels_yroom-0.0.3.tar.gz`

## Comparing `channels_yroom-0.0.2.tar` & `channels_yroom-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,68 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.dockerignore
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/Dockerfile
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/docker-compose.yml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/admin.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/apps.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/channel.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/conf.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/consumer.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/models.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/storage.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/utils.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/commands/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/management/commands/yroom.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/channels_yroom/migrations/__init__.py
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/manage.py
--rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/package-lock.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/package.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/requirements.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/vite.config.js
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/main.js
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/prosemirror.js
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/schema.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/frontend/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/apps.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/consumers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/models.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/routing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/tests.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/urls.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/views.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/migrations/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/templates/textcollab/index.html
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab/templates/textcollab/room.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/asgi.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/settings.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/urls.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/example/textcollab_project/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/tests/test_consumer.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/LICENSE
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 channels_yroom-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.dockerignore
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/Dockerfile
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docker-compose.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/admin.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/apps.py
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/channel.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/conf.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/consumer.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/models.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/proxy.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/storage.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/utils.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/commands/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/commands/yroom.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/migrations/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/api.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/explanation.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/index.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/requirements.in
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/settings.md
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/tutorial.md
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/howto/tiptap.md
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/manage.py
+-rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/package-lock.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/package.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/requirements.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/vite.config.js
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/main.js
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/prosemirror.js
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/schema.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/apps.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/consumers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/models.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/routing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/tests.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/urls.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/views.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/migrations/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/templates/textcollab/index.html
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/templates/textcollab/room.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/asgi.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/settings.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/urls.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/test_consumer.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/PKG-INFO
```

### Comparing `channels_yroom-0.0.2/Dockerfile` & `channels_yroom-0.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/docker-compose.yml` & `channels_yroom-0.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/.github/workflows/release.yml` & `channels_yroom-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/.github/workflows/test.yml` & `channels_yroom-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/channels_yroom/channel.py` & `channels_yroom-0.0.3/channels_yroom/channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,75 @@
 import asyncio
 import logging
 from contextlib import asynccontextmanager
+from typing import Optional
 
 from channels.consumer import AsyncConsumer
 from yroom import YRoomManager, YRoomMessage
 
-from .conf import settings
+from .conf import get_room_prefix, get_room_settings, get_settings
 from .storage import YDocStorage, get_ydoc_storage
 from .utils import (
     YroomChannelMessage,
     YroomChannelRPCMessage,
     get_connection_group_name,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class YRoomChannelConsumer(AsyncConsumer):
     def __init__(self) -> None:
-        self.room_manager: YRoomManager = YRoomManager()
-        self.storage: YDocStorage = get_ydoc_storage()
+        self.room_manager: YRoomManager = YRoomManager(get_settings())
         self.cleanup_tasks = {}
+        self.storages: dict[str, YDocStorage] = {}
+
+    def get_storage(self, room_name):
+        prefix = get_room_prefix(room_name)
+        if prefix in self.storages:
+            return self.storages[prefix]
+        storage = get_ydoc_storage(room_name)
+        self.storages[prefix] = storage
+        return storage
 
     async def connect(self, message: YroomChannelMessage) -> None:
         room_name = message["room"]
         conn_id = message["conn_id"]
         logger.debug("yroom consumer connect %s %s", room_name, conn_id)
 
         # Cancel room cleanup task if it exists
         if room_name in self.cleanup_tasks:
             self.cleanup_tasks[room_name].cancel()
 
         result = None
         if not self.room_manager.has_room(room_name):
             result = await self.create_room_from_snapshot(room_name, conn_id)
         if result is None:
-            logger.debug("yroom connect, room present %s %s", room_name, conn_id)
+            logger.debug(
+                "yroom connect, room present or no snapshot %s %s", room_name, conn_id
+            )
             result = self.room_manager.connect(room_name, conn_id)
         await self.respond(conn_id, room_name, result)
 
-    async def create_room_from_snapshot(self, room_name: str, conn_id: int = 0) -> None:
+    async def create_room_from_snapshot(
+        self, room_name: str, conn_id: int = 0
+    ) -> Optional[YRoomMessage]:
         logger.debug("yroom connect, no room yet %s %s", room_name, conn_id)
-        snapshot = await self.storage.get_snapshot(room_name)
+        storage = self.get_storage(room_name)
+        logger.debug("Using yroom storage %s of %s", storage, self.storages)
+        snapshot = await storage.get_snapshot(room_name)
+        logger.debug("Found snapshot %s", snapshot)
         if snapshot:
             logger.debug("yroom connect, snapshot found %s %s", room_name, snapshot)
             return self.room_manager.connect_with_data(room_name, conn_id, snapshot)
 
     async def message(self, message: YroomChannelMessage) -> None:
         room_name = message["room"]
         conn_id = message["conn_id"]
-        # logger.debug("yroom consumer message %s %s", room_name, conn_id)
+        logger.debug("yroom consumer message %s %s: %s", room_name, conn_id, message)
         result = self.room_manager.handle_message(
             room_name, conn_id, message["payload"]
         )
         await self.respond(conn_id, room_name, result)
 
     @asynccontextmanager
     async def try_room(self, room_name: str) -> None:
@@ -98,21 +114,21 @@
             {
                 "type": "rpc_response",
                 "result": result,
             },
         )
 
     async def respond(self, conn_id: int, room_name: str, result: YRoomMessage) -> None:
-        # logger.debug(
-        #     "yroom response in room %s at conection %s (client: %s, broadcast: %s)",
-        #     room_name,
-        #     conn_id,
-        #     bool(result.payload),
-        #     bool(result.broadcast_payload),
-        # )
+        logger.debug(
+            "yroom response in room %s at conection %s (client: %s, broadcast: %s)",
+            room_name,
+            conn_id,
+            result.payload,
+            result.broadcast_payload,
+        )
         if result.payload:
             conn_group_name = get_connection_group_name(conn_id)
             await self.send_response(conn_group_name, result.payload)
         if result.broadcast_payload:
             await self.send_response(room_name, result.broadcast_payload)
 
     async def send_response(self, group_name: str, payload: bytes) -> None:
@@ -144,15 +160,16 @@
 
         task = asyncio.create_task(self.remove_room_soon(room_name))
         self.cleanup_tasks[room_name] = task
         task.add_done_callback(lambda _task: self.cleanup_tasks.pop(room_name, None))
 
     async def remove_room_soon(self, room_name: str):
         # Wait a bit and then check if the room is still alive
-        await asyncio.sleep(settings.YROOM_REMOVE_ROOM_DELAY)
+        room_settings = get_room_settings(room_name)
+        await asyncio.sleep(room_settings["REMOVE_ROOM_DELAY"])
         await self.remove_room(room_name)
 
     async def remove_room(self, room_name: str):
         if self.room_manager.is_room_alive(room_name):
             return
         logger.debug("Snapshot room %s", room_name)
         await self.snapshot_room(room_name)
@@ -167,15 +184,16 @@
         ydoc_bytes = self.room_manager.serialize_room(room_name)
         logger.debug(
             "Snapshot room %s with %s bytes", room_name, len(ydoc_bytes or b"")
         )
         if ydoc_bytes is None:
             # Room is gone!
             return
-        await self.storage.save_snapshot(room_name, ydoc_bytes)
+        storage = self.get_storage(room_name)
+        await storage.save_snapshot(room_name, ydoc_bytes)
 
     async def shutdown(self, message) -> None:
         logger.info("Shutdown event received")
         cleanup_tasks = list(self.cleanup_tasks.values())
         for task in cleanup_tasks:
             task.cancel()
         await asyncio.gather(*cleanup_tasks, return_exceptions=True)
```

### Comparing `channels_yroom-0.0.2/channels_yroom/models.py` & `channels_yroom-0.0.3/channels_yroom/models.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/channels_yroom/storage.py` & `channels_yroom-0.0.3/channels_yroom/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Protocol
 
 from asgiref.sync import sync_to_async
 from django.utils.module_loading import import_string
 
-from .conf import settings
+from .conf import get_room_settings
 from .models import YDocUpdate
 
 
 class YDocStorage(Protocol):
     async def get_snapshot(self, name: str) -> Optional[bytes]:
         ...
 
@@ -48,9 +48,18 @@
     async def get_snapshot(self, name: str) -> Optional[bytes]:
         return await get_db_snapshot(name)
 
     async def save_snapshot(self, name: str, data: bytes) -> None:
         return await save_db_snapshot(name, data)
 
 
-def get_ydoc_storage() -> YDocStorage:
-    return import_string(settings.YROOM_STORAGE_BACKEND)()
+storage_cache = {}
+
+
+def get_ydoc_storage(room_name) -> YDocStorage:
+    room_settings = get_room_settings(room_name)
+    backend = room_settings["STORAGE_BACKEND"]
+    if backend in storage_cache:
+        return storage_cache[backend]
+    storage = import_string(backend)()
+    storage_cache[backend] = storage
+    return storage
```

### Comparing `channels_yroom-0.0.2/channels_yroom/worker.py` & `channels_yroom-0.0.3/channels_yroom/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 scope=scope,
                 receive=self.input_queue.get,
                 send=self.receive_from_worker,
             ),
         )
         # The consumer is also listening on a channel layer
         # but only on a new random channel
-        # so we listen on the yroom channel and forward messages
+        # so we listen on the given channel and forward messages
         while True:
             message = await self.channel_layer.receive(self.channel)
             if not message.get("type", None):
                 raise ValueError("Worker received message with no type.")
             # Run the message into the app
             await self.input_queue.put(message)
```

### Comparing `channels_yroom-0.0.2/channels_yroom/management/commands/yroom.py` & `channels_yroom-0.0.3/channels_yroom/management/commands/yroom.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from channels import DEFAULT_CHANNEL_LAYER
 from channels.layers import get_channel_layer
 from channels.routing import get_default_application
 from django.core.management import BaseCommand, CommandError
 
-from ...conf import settings
+from ...conf import get_default_room_settings
 from ...worker import YroomWorker
 
 logger = logging.getLogger("django.channels.worker")
 
 
 class Command(BaseCommand):
     leave_locale_alone = True
@@ -20,26 +20,37 @@
         parser.add_argument(
             "--layer",
             action="store",
             dest="layer",
             default=DEFAULT_CHANNEL_LAYER,
             help="Channel layer alias to use, if not the default.",
         )
+        parser.add_argument(
+            "--channel",
+            action="store",
+            dest="channel",
+            default=None,
+            help="Channel layer alias to use, if not the default.",
+        )
 
     def handle(self, *args, **options):
         # Get the backend to use
         self.verbosity = options.get("verbosity", 1)
         # Get the channel layer they asked for (or see if one isn't configured)
         if "layer" in options:
             self.channel_layer = get_channel_layer(options["layer"])
         else:
             self.channel_layer = get_channel_layer()
         if self.channel_layer is None:
             raise CommandError("You do not have any CHANNEL_LAYERS configured.")
+        if "channel" in options:
+            channel = options["channel"]
+        else:
+            channel = get_default_room_settings()["CHANNEL_NAME"]
         # Run the worker
-        logger.info("Running worker for yroom channel")
+        logger.info("Running worker for channel '{}'", channel)
         worker = self.worker_class(
             application=get_default_application(),
-            channel=settings.YROOM_CHANNEL_NAME,
+            channel=channel,
             channel_layer=self.channel_layer,
         )
         worker.run()
```

### Comparing `channels_yroom-0.0.2/channels_yroom/migrations/0001_initial.py` & `channels_yroom-0.0.3/channels_yroom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/manage.py` & `channels_yroom-0.0.3/example/manage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/package-lock.json` & `channels_yroom-0.0.3/example/package-lock.json`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/frontend/prosemirror.js` & `channels_yroom-0.0.3/example/frontend/prosemirror.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/frontend/schema.js` & `channels_yroom-0.0.3/example/frontend/schema.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/textcollab/views.py` & `channels_yroom-0.0.3/example/textcollab/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing import Optional
+
 from django.http import HttpResponse
 from django.shortcuts import render
 
-from channels_yroom.utils import YroomDocument
+from channels_yroom.proxy import YroomDocument
 
-from .consumers import get_room_group_name
+from .consumers import get_room_name
 
 
 def index(request):
     return render(request, "textcollab/index.html")
 
 
 def room(request, room_name):
@@ -15,13 +17,13 @@
 
 
 YDOC_XML_FRAGMENT_KEY = "prosemirror"
 
 
 async def save_room(request, room_name):
     # Get the XML fragment from the server ydoc
-    room_group_name = get_room_group_name(room_name)
+    room_group_name = get_room_name(room_name)
     doc = YroomDocument(room_group_name)
-    result = await doc.get_xml_fragment(YDOC_XML_FRAGMENT_KEY)
+    result: Optional[str] = await doc.export_xml_fragment(YDOC_XML_FRAGMENT_KEY)
     if result is None:
         return HttpResponse(status=404)
     return HttpResponse(result)
```

### Comparing `channels_yroom-0.0.2/example/textcollab/migrations/0001_initial.py` & `channels_yroom-0.0.3/example/textcollab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/textcollab/templates/textcollab/index.html` & `channels_yroom-0.0.3/example/textcollab/templates/textcollab/index.html`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/textcollab_project/asgi.py` & `channels_yroom-0.0.3/example/textcollab_project/asgi.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/textcollab_project/settings.py` & `channels_yroom-0.0.3/example/textcollab_project/settings.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/example/textcollab_project/urls.py` & `channels_yroom-0.0.3/example/textcollab_project/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/tests/conftest.py` & `channels_yroom-0.0.3/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,10 +10,14 @@
             "django.contrib.sessions",
             "django.contrib.admin",
             "channels",
             "channels_yroom",
         ],
         SECRET_KEY="Not_a_secret_key",
         CHANNEL_LAYERS={"default": {"BACKEND": "channels.layers.InMemoryChannelLayer"}},
-        YROOM_STORAGE_BACKEND="channels_yroom.storage.YDocDummyStorage",
-        YROOM_REMOVE_ROOM_DELAY=0,
+        YROOM_SETTINGS={
+            "default": {
+                "STORAGE_BACKEND": "channels_yroom.storage.YDocDummyStorage",
+                "REMOVE_ROOM_DELAY": 0,
+            }
+        },
     )
```

### Comparing `channels_yroom-0.0.2/LICENSE` & `channels_yroom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.2/pyproject.toml` & `channels_yroom-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,77 +21,83 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "Django >= 3.2",
   "channels >= 4.0",
-  "yroom >= 0.0.2",
-  "django-appconf",
+  "yroom >= 0.0.6",
 ]
 dynamic = ["version"]
 
+[project.urls]
+Documentation = "https://github.com/stefanw/channels-yroom#readme"
+Issues = "https://github.com/stefanw/channels-yroom/issues"
+Source = "https://github.com/stefanw/channels-yroom"
+
+[tool.hatch.version]
+path = "channels_yroom/__about__.py"
+
+[tool.hatch.build.targets.wheel]
+packages = ["channels_yroom"]
+
 [tool.hatch.envs.test]
 dependencies = [
   "async-timeout",
   "daphne",
   "pytest-asyncio",
   "pytest-cov",
   "pytest-django",
   "pytest",
+  "y-py",
+]
+
+[tool.hatch.envs.test.scripts]
+test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=channels_yroom --cov=tests {args}"
+no-cov = "test --no-cov {args}"
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11"]
+
+[tool.hatch.envs.docs]
+skip-install = true
+detached = true
+dependencies = [
+  "mkdocs",
+  "mkdocstrings[python]",
+  "mkdocs-mermaid2-plugin",
+]
+[tool.hatch.envs.docs.scripts]
+serve = [
+  "mkdocs serve -a 127.0.0.1:8001",
+]
+freeze = [
+  "pip freeze > docs/requirements.txt",
 ]
 
 [tool.hatch.envs.lint]
 skip-install = true
 detached = true
 dependencies = [
   "black",
-  "isort",
-  "flake8",
-  "Flake8-pyproject",
+  "ruff",
 ]
 
 [tool.hatch.envs.lint.scripts]
 check = [
-  "flake8 channels_yroom tests",
+  "ruff channels_yroom tests",
   "black --check --diff channels_yroom tests",
-  "isort --check-only --diff channels_yroom tests",
 ]
 
-[project.urls]
-Documentation = "https://github.com/stefanw/channels-yroom#readme"
-Issues = "https://github.com/stefanw/channels-yroom/issues"
-Source = "https://github.com/stefanw/channels-yroom"
-
-[tool.hatch.version]
-path = "channels_yroom/__about__.py"
-
-[tool.hatch.build.targets.wheel]
-packages = ["channels_yroom"]
-
-[tool.hatch.envs.test.scripts]
-test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=channels_yroom --cov=tests {args}"
-no-cov = "test --no-cov {args}"
-
-[[tool.hatch.envs.test.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
-
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "channels_yroom/__about__.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
-
-[tool.flake8]
-extend-ignore = ['E203']
-max-line-length = 88
-
-[tool.isort]
-profile = 'black'
```

