# Comparing `tmp/django-gcp-0.8.0.tar.gz` & `tmp/django_gcp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gcp-0.8.0.tar", max compression
+gzip compressed data, was "django_gcp-0.9.1.tar", max compression
```

## Comparing `django-gcp-0.8.0.tar` & `django_gcp-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,45 @@
--rw-r--r--   0        0        0     1080 2023-03-28 08:13:53.535144 django-gcp-0.8.0/LICENSE
--rw-r--r--   0        0        0     3746 2023-03-28 08:13:53.535144 django-gcp-0.8.0/README.md
--rw-r--r--   0        0        0       58 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/__init__.py
--rw-r--r--   0        0        0      108 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/admin.py
--rw-r--r--   0        0        0      627 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/apps.py
--rw-r--r--   0        0        0        0 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/events/__init__.py
--rw-r--r--   0        0        0       63 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/events/signals.py
--rw-r--r--   0        0        0     7279 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/events/utils.py
--rw-r--r--   0        0        0     1703 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/events/views.py
--rw-r--r--   0        0        0     1084 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/exceptions.py
--rw-r--r--   0        0        0      189 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/logging/__init__.py
--rw-r--r--   0        0        0     2212 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/logging/error_reporting.py
--rw-r--r--   0        0        0     1765 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/logging/structured_logs.py
--rw-r--r--   0        0        0        0 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/management/commands/__init__.py
--rw-r--r--   0        0        0      816 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/management/commands/_base.py
--rw-r--r--   0        0        0     1760 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/management/commands/task_manager.py
--rw-r--r--   0        0        0       96 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/metadata/__init__.py
--rw-r--r--   0        0        0     3410 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/metadata/metadata.py
--rw-r--r--   0        0        0      170 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/signals.py
--rw-r--r--   0        0        0        0 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/static/.gitignore
--rw-r--r--   0        0        0      328 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/storage/__init__.py
--rw-r--r--   0        0        0     1431 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/storage/compress.py
--rw-r--r--   0        0        0    13882 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/storage/gcloud.py
--rw-r--r--   0        0        0     4427 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/storage/settings.py
--rw-r--r--   0        0        0     3202 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/storage/utils.py
--rw-r--r--   0        0        0      192 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/tasks/__init__.py
--rw-r--r--   0        0        0     1124 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/tasks/_patch_cloud_scheduler.py
--rw-r--r--   0        0        0     1106 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/tasks/_patch_cloud_tasks.py
--rw-r--r--   0        0        0      350 2023-03-28 08:13:53.535144 django-gcp-0.8.0/django_gcp/tasks/helpers.py
--rw-r--r--   0        0        0     8669 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/tasks/manager.py
--rw-r--r--   0        0        0     1307 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/tasks/serializers.py
--rw-r--r--   0        0        0    11229 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/tasks/tasks.py
--rw-r--r--   0        0        0     1836 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/tasks/views.py
--rw-r--r--   0        0        0        0 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/templates/django_gcp/.gitignore
--rw-r--r--   0        0        0      491 2023-03-28 08:13:53.539144 django-gcp-0.8.0/django_gcp/urls.py
--rw-r--r--   0        0        0     1548 2023-03-28 08:13:53.539144 django-gcp-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5037 2023-03-28 08:19:07.195692 django-gcp-0.8.0/setup.py
--rw-r--r--   0        0        0     4985 2023-03-28 08:19:07.196617 django-gcp-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-04 12:22:25.483580 django_gcp-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3746 2023-05-04 12:22:25.483580 django_gcp-0.9.1/README.md
+-rw-r--r--   0        0        0       58 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/apps.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/signals.py
+-rw-r--r--   0        0        0     7279 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/utils.py
+-rw-r--r--   0        0        0     1703 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/views.py
+-rw-r--r--   0        0        0     1342 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/__init__.py
+-rw-r--r--   0        0        0     2212 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/error_reporting.py
+-rw-r--r--   0        0        0     1765 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/structured_logs.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/_base.py
+-rw-r--r--   0        0        0     1637 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/cleanup_tmp_files.py
+-rw-r--r--   0        0        0     1760 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/task_manager.py
+-rw-r--r--   0        0        0       96 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/metadata/__init__.py
+-rw-r--r--   0        0        0     3410 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/metadata/metadata.py
+-rw-r--r--   0        0        0      170 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/signals.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/.gitignore
+-rw-r--r--   0        0        0     2630 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.css
+-rw-r--r--   0        0        0     7686 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.js
+-rw-r--r--   0        0        0      328 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/compress.py
+-rw-r--r--   0        0        0    22857 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/fields.py
+-rw-r--r--   0        0        0     2595 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/forms.py
+-rw-r--r--   0        0        0    14266 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/gcloud.py
+-rw-r--r--   0        0        0     6373 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/operations.py
+-rw-r--r--   0        0        0     4427 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/settings.py
+-rw-r--r--   0        0        0     3202 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/utils.py
+-rw-r--r--   0        0        0     1942 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/widgets.py
+-rw-r--r--   0        0        0      192 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/__init__.py
+-rw-r--r--   0        0        0     1124 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_scheduler.py
+-rw-r--r--   0        0        0     1106 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_tasks.py
+-rw-r--r--   0        0        0      350 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/helpers.py
+-rw-r--r--   0        0        0     8669 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/manager.py
+-rw-r--r--   0        0        0     1307 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/serializers.py
+-rw-r--r--   0        0        0    11229 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/tasks.py
+-rw-r--r--   0        0        0     1836 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/templates/django_gcp/.gitignore
+-rw-r--r--   0        0        0     2571 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/templates/django_gcp/cloud_object_widget.html
+-rw-r--r--   0        0        0      491 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-04 12:22:25.487580 django_gcp-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 django_gcp-0.9.1/PKG-INFO
```

### Comparing `django-gcp-0.8.0/LICENSE` & `django_gcp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/README.md` & `django_gcp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/apps.py` & `django_gcp-0.9.1/django_gcp/apps.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/events/utils.py` & `django_gcp-0.9.1/django_gcp/events/utils.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/events/views.py` & `django_gcp-0.9.1/django_gcp/events/views.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/exceptions.py` & `django_gcp-0.9.1/django_gcp/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,7 +24,15 @@
 
 class UnknownActionError(ValueError):
     """Raised when attempting to create or use a resource not known to django-gcp"""
 
 
 class DuplicateTaskError(Exception):
     """Raised when a unique (non-duplicatable) task is enqueued but already present in the queue"""
+
+
+class AttemptedOverwriteError(Exception):
+    """Raised when attempting to overwrite an existing object in GCS with another object"""
+
+
+class MissingBlobError(Exception):
+    """Raised when attempting to access or copy a blob that is not present in GCS"""
```

### Comparing `django-gcp-0.8.0/django_gcp/logging/error_reporting.py` & `django_gcp-0.9.1/django_gcp/logging/error_reporting.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/logging/structured_logs.py` & `django_gcp-0.9.1/django_gcp/logging/structured_logs.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/management/commands/_base.py` & `django_gcp-0.9.1/django_gcp/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/management/commands/task_manager.py` & `django_gcp-0.9.1/django_gcp/management/commands/task_manager.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/metadata/metadata.py` & `django_gcp-0.9.1/django_gcp/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/storage/compress.py` & `django_gcp-0.9.1/django_gcp/storage/compress.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/storage/gcloud.py` & `django_gcp-0.9.1/django_gcp/storage/gcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# TODO Remove this pylint disable and clean up methods
-# pylint: disable=arguments-renamed
 import logging
 import mimetypes
 from tempfile import SpooledTemporaryFile
 from django.core.exceptions import SuspiciousOperation
 from django.core.files.base import File
 from django.core.files.storage import Storage
 from django.utils import timezone
@@ -129,20 +127,29 @@
         """The google-storage client for this store"""
         if self._client is None:
             self._client = Client(project=self.settings.project_id, credentials=self.settings.credentials)
         return self._client
 
     @property
     def bucket(self):
-        """The google-storage bucket object for this store"""
+        """The google-storage bucket object for this store
+        See bucket class information: https://cloud.google.com/python/docs/reference/storage/latest/google.cloud.storage.bucket.Bucket
+        """
         if self._bucket is None:
             self._bucket = self.client.bucket(self.settings.bucket_name)
         return self._bucket
 
     @property
+    def versioning_enabled(self):
+        """True if versioning is enabled on the bucket
+        https://cloud.google.com/python/docs/reference/storage/latest/google.cloud.storage.bucket.Bucket#google_cloud_storage_bucket_Bucket_versioning_enabled
+        """
+        return self.bucket.versioning_enabled
+
+    @property
     def bucket_name(self):
         """The name of the bucket corresponding to this store
 
         A convenience property referring to self.settings.bucket_name but here for backward compatibility
         with django_storages and ease of general use
         """
         return self.settings.bucket_name
@@ -229,22 +236,22 @@
                 return True
             except NotFound:
                 return False
 
         name = self._normalize_name(clean_name(name))
         return bool(self.bucket.get_blob(name))
 
-    def listdir(self, name):
-        name = self._normalize_name(clean_name(name))
+    def listdir(self, path):
+        prefix = self._normalize_name(clean_name(path))
         # For bucket.list_blobs and logic below name needs to end in /
         # but for the root path "" we leave it as an empty string
-        if name and not name.endswith("/"):
-            name += "/"
+        if prefix and not prefix.endswith("/"):
+            prefix += "/"
 
-        iterator = self.bucket.list_blobs(prefix=name, delimiter="/")
+        iterator = self.bucket.list_blobs(prefix=prefix, delimiter="/")
         blobs = list(iterator)
         prefixes = iterator.prefixes
 
         files = []
         dirs = []
 
         for blob in blobs:
```

### Comparing `django-gcp-0.8.0/django_gcp/storage/settings.py` & `django_gcp-0.9.1/django_gcp/storage/settings.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/storage/utils.py` & `django_gcp-0.9.1/django_gcp/storage/utils.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/_patch_cloud_scheduler.py` & `django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_scheduler.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/_patch_cloud_tasks.py` & `django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/manager.py` & `django_gcp-0.9.1/django_gcp/tasks/manager.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/serializers.py` & `django_gcp-0.9.1/django_gcp/tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/tasks.py` & `django_gcp-0.9.1/django_gcp/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/django_gcp/tasks/views.py` & `django_gcp-0.9.1/django_gcp/tasks/views.py`

 * *Files identical despite different names*

### Comparing `django-gcp-0.8.0/pyproject.toml` & `django_gcp-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-gcp"
-version = "0.8.0"
+version = "0.9.1"
 description = "Utilities to run Django on Google Cloud Platform"
 authors = ["Tom Clark"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -18,15 +18,15 @@
 keywords = ["django", "google", "cloud", "gcloud", "gcp"]
 packages = [{ include = "django_gcp" },]
 
 
 [tool.poetry.dependencies]
 Django = ">=3.0,<5"
 python = ">=3.9,<3.11"
-google-cloud-storage = "^2.1.0"
+google-cloud-storage = "^2.7.0"
 google-auth = "^2.6.0"
 django-app-settings = "^0.7.1"
 gcp-pilot = "^0.40.0"
 python-dateutil = "^2.8.2"
 google-cloud-tasks = "^2"
 google-cloud-scheduler = "^2"
 google-cloud-pubsub = "^2"
@@ -41,18 +41,21 @@
 pytest = "^7.0.0"
 tox = "^3.24.5"
 tox-gh-actions = "^2.9.1"
 tox-poetry = "^0.4.1"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-tabs = "^3.2.0"
 Sphinx = "^4.4.0"
-django-test-migrations = "^1.2.0"
 django-extensions = "^3.2.0"
 pylint-django = "^2.5.3"
 watchdog = "^2.1.9"
 throttle = "^0.2.2"
 psycopg2-binary = "^2.9.3"
-
+notebook = "^6.5.3"
+django-test-migrations = "^1.2.0"
+django-debug-toolbar = "^3.8.1"
+django-json-widget = "^1.1.1"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django-gcp-0.8.0/setup.py` & `django_gcp-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,134 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-gcp
+Version: 0.9.1
+Summary: Utilities to run Django on Google Cloud Platform
+Home-page: https://github.com/octue/django-gcp
+License: MIT
+Keywords: django,google,cloud,gcloud,gcp
+Author: Tom Clark
+Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django (>=3.0,<5)
+Requires-Dist: django-app-settings (>=0.7.1,<0.8.0)
+Requires-Dist: gcp-pilot (>=0.40.0,<0.41.0)
+Requires-Dist: google-auth (>=2.6.0,<3.0.0)
+Requires-Dist: google-cloud-error-reporting (>=1.9.0,<2.0.0)
+Requires-Dist: google-cloud-pubsub (>=2,<3)
+Requires-Dist: google-cloud-scheduler (>=2,<3)
+Requires-Dist: google-cloud-storage (>=2.7.0,<3.0.0)
+Requires-Dist: google-cloud-tasks (>=2,<3)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Project-URL: Repository, https://github.com/octue/django-gcp
+Description-Content-Type: text/markdown
 
-packages = \
-['django_gcp',
- 'django_gcp.events',
- 'django_gcp.logging',
- 'django_gcp.management',
- 'django_gcp.management.commands',
- 'django_gcp.metadata',
- 'django_gcp.storage',
- 'django_gcp.tasks']
-
-package_data = \
-{'': ['*'], 'django_gcp': ['static/*', 'templates/django_gcp/*']}
-
-install_requires = \
-['Django>=3.0,<5',
- 'django-app-settings>=0.7.1,<0.8.0',
- 'gcp-pilot>=0.40.0,<0.41.0',
- 'google-auth>=2.6.0,<3.0.0',
- 'google-cloud-error-reporting>=1.9.0,<2.0.0',
- 'google-cloud-pubsub>=2,<3',
- 'google-cloud-scheduler>=2,<3',
- 'google-cloud-storage>=2.1.0,<3.0.0',
- 'google-cloud-tasks>=2,<3',
- 'python-dateutil>=2.8.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'django-gcp',
-    'version': '0.8.0',
-    'description': 'Utilities to run Django on Google Cloud Platform',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/django_gcp.svg)](https://badge.fury.io/py/django_gcp)\n[![codecov](https://codecov.io/gh/octue/django-gcp/branch/main/graph/badge.svg?token=H2QLSCF3DU)](https://codecov.io/gh/octue/django-gcp)\n[![Documentation](https://readthedocs.org/projects/django_gcp/badge/?version=latest)](https://django_gcp.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n# DjangoGCP\n\nHelps you to run Django on Google Cloud Platform - Storage, PubSub and Tasks.\n\nRead the [documentation here](https://django_gcp.readthedocs.io/en/latest).\n\nThis app is maintained by Octue - we\'re on a mission to help climate scientists and energy engineers be more efficient. [Find out more](https://www.octue.com).\n\nIf you need some help implementing or updating this, we can help! Raise an issue or [contact us](https://www.octue.com/contact).\n\n## Are you from GCP??\n\nIf so, get in touch for a chat. We\'re doing fun things with Google Cloud. Way funner than boring old django... :)\n\n## All the :heart:\n\nThis app is based heavily on [django-storages](https://django-storages.readthedocs.io/en/latest/), [django-google-cloud-tasks](https://github.com/flamingo-run/django-cloud-tasks) and uses the [django-rabid-armadillo](https://github.com/thclark/django-rabid-armadillo) template. Big love.\n\n## Contributing\n\nIt\'s pretty straightforward to get going, but it\'s good to get in touch first, especially if you\'re planning a big feature.\n\n### Set up\n\nOpen the project in codespaces, a vscode .devcontainer (which is configured out of the box for you) or your favourite IDE or editor (if the latter you\'ll need to set up `docker compose` yourself).\n\nCreate a file `.devcontainer/docker-compose.developer.yml`. This allows you to customise extra services and volumes you make available to the container.\nFor example, you can map your own gcloud config folder into the container to use your own credentials. This example will get you going, but you can just leave the services key empty.\n\n```\nversion: "3.8"\n\nservices:\n  web:\n    volumes:\n      - ..:/workspace:cached\n      - $HOME/.config/gcloud:/gcp/config\n\n    environment:\n      - CLOUDSDK_CONFIG=/gcp/config\n      - GOOGLE_APPLICATION_CREDENTIALS=/gcp/config/your-credentials-file.json\n```\n\n### Initialise gcloud CLI\n\nTo sign in (enabling use of the gcloud CLI tool), do:\n\n```\ngcloud config set project octue-django-gcp\ngcloud auth login\n```\n\n### Run the tests\n\nRun the tests:\n\n```\npytest .\n```\n\nWe use pre-commit to ensure code quality standards (and to help us automate releases using conventional-commits). If you can get on board with this that\'s really helpful - if not, don\'t fret, we can help.\n\n### Use the example app\n\nYou can start the example app (which is useful for seeing how `django-gcp` looks in the admin.\n\nInitially, do:\n\n```\npython manage.py migrate\npython manage.py createsuperuser\n# make yourself a user account at the prompt\n```\n\nThen to run the app, do:\n\n```\npython manage.py runserver\n```\n\n...and visit [http://localhost:8000/admin/](http://localhost:8000/admin/) to sign in.\n\n### Update the docs\n\nWe\'re pretty good on keeping the docs helpful, friendly and up to date. Any contributions should be\nfully documented.\n\nTo help develop the docs quickly, we set up a watcher that rebuilds the docs on save. Start it with:\n\n```\npython docs/watch.py\n```\n\nOnce docs are building, the the vscode live server extension (or whatever the equivalent is in your IDE)\nto live-reload `docs/html/index.html` in your browser, then get started!\n',
-    'author': 'Tom Clark',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/octue/django-gcp',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.11',
-}
+[![PyPI version](https://badge.fury.io/py/django_gcp.svg)](https://badge.fury.io/py/django_gcp)
+[![codecov](https://codecov.io/gh/octue/django-gcp/branch/main/graph/badge.svg?token=H2QLSCF3DU)](https://codecov.io/gh/octue/django-gcp)
+[![Documentation](https://readthedocs.org/projects/django_gcp/badge/?version=latest)](https://django_gcp.readthedocs.io/en/latest/?badge=latest)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
+# DjangoGCP
+
+Helps you to run Django on Google Cloud Platform - Storage, PubSub and Tasks.
+
+Read the [documentation here](https://django_gcp.readthedocs.io/en/latest).
+
+This app is maintained by Octue - we're on a mission to help climate scientists and energy engineers be more efficient. [Find out more](https://www.octue.com).
+
+If you need some help implementing or updating this, we can help! Raise an issue or [contact us](https://www.octue.com/contact).
+
+## Are you from GCP??
+
+If so, get in touch for a chat. We're doing fun things with Google Cloud. Way funner than boring old django... :)
+
+## All the :heart:
+
+This app is based heavily on [django-storages](https://django-storages.readthedocs.io/en/latest/), [django-google-cloud-tasks](https://github.com/flamingo-run/django-cloud-tasks) and uses the [django-rabid-armadillo](https://github.com/thclark/django-rabid-armadillo) template. Big love.
+
+## Contributing
+
+It's pretty straightforward to get going, but it's good to get in touch first, especially if you're planning a big feature.
+
+### Set up
+
+Open the project in codespaces, a vscode .devcontainer (which is configured out of the box for you) or your favourite IDE or editor (if the latter you'll need to set up `docker compose` yourself).
+
+Create a file `.devcontainer/docker-compose.developer.yml`. This allows you to customise extra services and volumes you make available to the container.
+For example, you can map your own gcloud config folder into the container to use your own credentials. This example will get you going, but you can just leave the services key empty.
+
+```
+version: "3.8"
+
+services:
+  web:
+    volumes:
+      - ..:/workspace:cached
+      - $HOME/.config/gcloud:/gcp/config
+
+    environment:
+      - CLOUDSDK_CONFIG=/gcp/config
+      - GOOGLE_APPLICATION_CREDENTIALS=/gcp/config/your-credentials-file.json
+```
+
+### Initialise gcloud CLI
+
+To sign in (enabling use of the gcloud CLI tool), do:
+
+```
+gcloud config set project octue-django-gcp
+gcloud auth login
+```
+
+### Run the tests
+
+Run the tests:
+
+```
+pytest .
+```
+
+We use pre-commit to ensure code quality standards (and to help us automate releases using conventional-commits). If you can get on board with this that's really helpful - if not, don't fret, we can help.
+
+### Use the example app
+
+You can start the example app (which is useful for seeing how `django-gcp` looks in the admin.
+
+Initially, do:
+
+```
+python manage.py migrate
+python manage.py createsuperuser
+# make yourself a user account at the prompt
+```
+
+Then to run the app, do:
+
+```
+python manage.py runserver
+```
+
+...and visit [http://localhost:8000/admin/](http://localhost:8000/admin/) to sign in.
+
+### Update the docs
+
+We're pretty good on keeping the docs helpful, friendly and up to date. Any contributions should be
+fully documented.
+
+To help develop the docs quickly, we set up a watcher that rebuilds the docs on save. Start it with:
+
+```
+python docs/watch.py
+```
+
+Once docs are building, the the vscode live server extension (or whatever the equivalent is in your IDE)
+to live-reload `docs/html/index.html` in your browser, then get started!
 
-setup(**setup_kwargs)
```

