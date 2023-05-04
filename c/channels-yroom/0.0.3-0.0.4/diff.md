# Comparing `tmp/channels_yroom-0.0.3.tar.gz` & `tmp/channels_yroom-0.0.4.tar.gz`

## Comparing `channels_yroom-0.0.3.tar` & `channels_yroom-0.0.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.dockerignore
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/Dockerfile
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docker-compose.yml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/admin.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/apps.py
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/channel.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/conf.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/consumer.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/models.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/proxy.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/storage.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/utils.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/worker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/commands/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/management/commands/yroom.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/channels_yroom/migrations/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/api.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/explanation.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/index.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/requirements.in
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/requirements.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/settings.md
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/tutorial.md
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/docs/howto/tiptap.md
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/manage.py
--rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/package-lock.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/package.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/requirements.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/vite.config.js
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/main.js
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/prosemirror.js
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/schema.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/frontend/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/apps.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/consumers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/models.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/routing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/tests.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/urls.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/views.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/migrations/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/templates/textcollab/index.html
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab/templates/textcollab/room.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/asgi.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/settings.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/urls.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/example/textcollab_project/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/tests/test_consumer.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 channels_yroom-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.dockerignore
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/Dockerfile
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docker-compose.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/admin.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/apps.py
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/channel.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/conf.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/consumer.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/models.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/proxy.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/storage.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/utils.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/commands/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/management/commands/yroom.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/channels_yroom/migrations/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/api.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/explanation.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/index.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/requirements.in
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/requirements.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/settings.md
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/tutorial.md
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/docs/howto/tiptap.md
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/manage.py
+-rw-r--r--   0        0        0    75131 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/package-lock.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/package.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/requirements.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/vite.config.js
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/main.js
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/prosemirror.js
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/schema.js
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/frontend/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/apps.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/consumers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/models.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/routing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/tests.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/urls.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/views.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/migrations/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/templates/textcollab/index.html
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab/templates/textcollab/room.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/asgi.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/settings.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/urls.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/example/textcollab_project/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/tests/test_consumer.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 channels_yroom-0.0.4/PKG-INFO
```

### Comparing `channels_yroom-0.0.3/Dockerfile` & `channels_yroom-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docker-compose.yml` & `channels_yroom-0.0.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/mkdocs.yml` & `channels_yroom-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/.github/workflows/release.yml` & `channels_yroom-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/.github/workflows/test.yml` & `channels_yroom-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/channel.py` & `channels_yroom-0.0.4/channels_yroom/channel.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/consumer.py` & `channels_yroom-0.0.4/channels_yroom/consumer.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/models.py` & `channels_yroom-0.0.4/channels_yroom/models.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/proxy.py` & `channels_yroom-0.0.4/channels_yroom/proxy.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/storage.py` & `channels_yroom-0.0.4/channels_yroom/storage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/utils.py` & `channels_yroom-0.0.4/channels_yroom/utils.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/channels_yroom/worker.py` & `channels_yroom-0.0.4/channels_yroom/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import asyncio
 import logging
 import signal
 
+from channels.routing import get_default_application
+
 logger = logging.getLogger(__name__)
 
 
 class YroomWorker:
     SIGNALS = (
         signal.SIGHUP,
         signal.SIGTERM,
         signal.SIGINT,
     )
 
-    def __init__(self, application, channel, channel_layer):
-        self.application = application
+    def __init__(self, channel, channel_layer, application=None):
         self.channel = channel
         self.channel_layer = channel_layer
+        if application is None:
+            self.application = get_default_application()
+        else:
+            self.application = application
 
     def run(self):
         """
         Runs the asyncio event loop with our handler loop.
         """
         loop = asyncio.get_event_loop()
         self._setup_signal_handlers(loop)
```

### Comparing `channels_yroom-0.0.3/channels_yroom/management/commands/yroom.py` & `channels_yroom-0.0.4/channels_yroom/management/commands/yroom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from channels import DEFAULT_CHANNEL_LAYER
 from channels.layers import get_channel_layer
-from channels.routing import get_default_application
 from django.core.management import BaseCommand, CommandError
 
 from ...conf import get_default_room_settings
 from ...worker import YroomWorker
 
 logger = logging.getLogger("django.channels.worker")
 
@@ -38,19 +37,19 @@
         # Get the channel layer they asked for (or see if one isn't configured)
         if "layer" in options:
             self.channel_layer = get_channel_layer(options["layer"])
         else:
             self.channel_layer = get_channel_layer()
         if self.channel_layer is None:
             raise CommandError("You do not have any CHANNEL_LAYERS configured.")
+        channel = None
         if "channel" in options:
             channel = options["channel"]
-        else:
+        if channel is None:
             channel = get_default_room_settings()["CHANNEL_NAME"]
         # Run the worker
-        logger.info("Running worker for channel '{}'", channel)
+        self.stdout.write("Running worker for channel '%s'\n" % channel)
         worker = self.worker_class(
-            application=get_default_application(),
             channel=channel,
             channel_layer=self.channel_layer,
         )
         worker.run()
```

### Comparing `channels_yroom-0.0.3/channels_yroom/migrations/0001_initial.py` & `channels_yroom-0.0.4/channels_yroom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/explanation.md` & `channels_yroom-0.0.4/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/index.md` & `channels_yroom-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/requirements.txt` & `channels_yroom-0.0.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/settings.md` & `channels_yroom-0.0.4/docs/settings.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/tutorial.md` & `channels_yroom-0.0.4/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/docs/howto/tiptap.md` & `channels_yroom-0.0.4/docs/howto/tiptap.md`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/manage.py` & `channels_yroom-0.0.4/example/manage.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/package-lock.json` & `channels_yroom-0.0.4/example/package-lock.json`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/frontend/prosemirror.js` & `channels_yroom-0.0.4/example/frontend/prosemirror.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/frontend/schema.js` & `channels_yroom-0.0.4/example/frontend/schema.js`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab/views.py` & `channels_yroom-0.0.4/example/textcollab/views.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab/migrations/0001_initial.py` & `channels_yroom-0.0.4/example/textcollab/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab/templates/textcollab/index.html` & `channels_yroom-0.0.4/example/textcollab/templates/textcollab/index.html`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab_project/asgi.py` & `channels_yroom-0.0.4/example/textcollab_project/asgi.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab_project/settings.py` & `channels_yroom-0.0.4/example/textcollab_project/settings.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/example/textcollab_project/urls.py` & `channels_yroom-0.0.4/example/textcollab_project/urls.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/tests/conftest.py` & `channels_yroom-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/tests/test_consumer.py` & `channels_yroom-0.0.4/tests/test_consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import asyncio
 from collections import deque
 from contextlib import asynccontextmanager
+from io import StringIO
 
 import pytest
 import pytest_asyncio
 import y_py as Y
 from asgiref.testing import ApplicationCommunicator
 from channels.layers import get_channel_layer
+from channels.routing import ChannelNameRouter, ProtocolTypeRouter
 from channels.testing import WebsocketCommunicator
+from django.core.management import call_command
 
 from channels_yroom.channel import YRoomChannelConsumer
-from channels_yroom.conf import get_room_settings
+from channels_yroom.conf import get_default_room_settings, get_room_settings
 from channels_yroom.consumer import YroomConsumer
-from channels_yroom.models import YDocUpdate
+from channels_yroom.management.commands.yroom import Command as YroomCommand
 from channels_yroom.proxy import DataUnavailable, YroomDocument
 from channels_yroom.storage import get_ydoc_storage
+from channels_yroom.worker import YroomWorker
+
+SYNC_STEP_1_DATA = b"\x00\x00\x07\x01\xe9\xdb\x9a\x90\x01\x06"
+# state as update of a doc {"test": "hello"}
+DOC_DATA = b"\x01\x01\xe9\xdb\x9a\x90\x01\x00\x04\x01\x04test\x06hello \x00"
 
 
 class FakeWorker:
     def __init__(self, channel_layer, channel, worker_communicator):
         self.channel_layer = channel_layer
         self.channel = channel
         self.worker_communicator = worker_communicator
@@ -187,14 +195,16 @@
         await fake_worker.shutdown()
         assert worker_results["shutdown"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.django_db
 async def test_snapshot_yroom_consumer(settings):
+    from channels_yroom.models import YDocUpdate
+
     settings.YROOM_SETTINGS = {
         "default": {
             "STORAGE_BACKEND": "channels_yroom.storage.YDocDatabaseStorage",
             "REMOVE_ROOM_DELAY": 0,
         }
     }
 
@@ -206,16 +216,14 @@
     class TestYRoomChannelConsumer(YRoomChannelConsumer):
         async def shutdown(self, message):
             worker_results["shutdown"] = True
             await super().shutdown(message)
 
     SYNC_STEP_1 = b"\x00\x00\x07\x01\xe9\xdb\x9a\x90\x01\x06"
     SYNC_STEP_2 = b"\x00\x01\x02\x00\x00"
-    # state as update of a doc {"test": "hello"}
-    DOC_DATA = b"\x01\x01\xe9\xdb\x9a\x90\x01\x00\x04\x01\x04test\x06hello \x00"
 
     app = TestConsumer()
     room_name = app.get_room_name()
 
     ydoc_update = await YDocUpdate.objects.acreate(
         name=room_name,
         data=DOC_DATA,
@@ -329,7 +337,83 @@
         await proxy.export_text("text")
     with pytest.raises(DataUnavailable):
         await proxy.export_array("array")
     with pytest.raises(DataUnavailable):
         await proxy.export_map("map")
     with pytest.raises(DataUnavailable):
         await proxy.export_xml_element("xml_element")
+
+
+def test_yroom_command(monkeypatch):
+    class FakeWorker:
+        def __init__(self, channel, channel_layer):
+            self.channel = channel
+            self.channel_layer = channel_layer
+
+        def run(self):
+            pass
+
+    monkeypatch.setattr(YroomCommand, "worker_class", FakeWorker)
+    out = StringIO()
+    call_command(
+        "yroom",
+        stdout=out,
+        stderr=StringIO(),
+    )
+    assert "Running worker for channel 'yroom'\n" == out.getvalue()
+
+    out = StringIO()
+    call_command(
+        "yroom",
+        "--channel",
+        "foobar",
+        stdout=out,
+        stderr=StringIO(),
+    )
+    assert "Running worker for channel 'foobar'\n" == out.getvalue()
+
+
+@pytest.mark.asyncio
+async def test_yroom_worker(settings):
+    settings.YROOM_SETTINGS = {
+        "default": {
+            "STORAGE_BACKEND": "channels_yroom.storage.YDocMemoryStorage",
+            "REMOVE_ROOM_DELAY": 0,
+        }
+    }
+
+    channel_layer = get_channel_layer()
+    channel = get_default_room_settings()["CHANNEL_NAME"]
+
+    application = ProtocolTypeRouter(
+        {
+            "channel": ChannelNameRouter(
+                {
+                    "yroom": YRoomChannelConsumer.as_asgi(),
+                }
+            ),
+        }
+    )
+
+    worker = YroomWorker(
+        channel=channel, channel_layer=channel_layer, application=application
+    )
+    worker_task = asyncio.create_task(worker.run_worker())
+
+    app = YroomConsumer()
+    room_name = app.get_room_name()
+
+    storage = get_ydoc_storage(room_name)
+    await storage.save_snapshot(room_name, DOC_DATA)
+
+    client_1 = WebsocketCommunicator(app, "/testws/")
+    connected, _ = await client_1.connect()
+    assert connected
+
+    payload = await client_1.receive_from()
+    assert payload == SYNC_STEP_1_DATA
+
+    worker_task.cancel()
+    try:
+        await worker_task
+    except asyncio.exceptions.CancelledError:
+        pass
```

### Comparing `channels_yroom-0.0.3/LICENSE` & `channels_yroom-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/pyproject.toml` & `channels_yroom-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `channels_yroom-0.0.3/PKG-INFO` & `channels_yroom-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channels-yroom
-Version: 0.0.3
+Version: 0.0.4
 Summary: Yjs sync protocol server for Django channels
 Project-URL: Documentation, https://github.com/stefanw/channels-yroom#readme
 Project-URL: Issues, https://github.com/stefanw/channels-yroom/issues
 Project-URL: Source, https://github.com/stefanw/channels-yroom
 Author-email: Stefan Wehrmeyer <mail@stefanwehrmeyer.com>
 License-Expression: MIT
 License-File: LICENSE
```

