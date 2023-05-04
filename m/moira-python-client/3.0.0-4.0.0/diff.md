# Comparing `tmp/moira-python-client-3.0.0.tar.gz` & `tmp/moira-python-client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moira-python-client-3.0.0.tar", last modified: Wed Jan 11 16:19:43 2023, max compression
+gzip compressed data, was "moira-python-client-4.0.0.tar", last modified: Thu May  4 11:36:47 2023, max compression
```

## Comparing `moira-python-client-3.0.0.tar` & `moira-python-client-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-11 16:19:43.752290 moira-python-client-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     2632 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2023-01-11 16:19:43.752290 moira-python-client-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2614 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-11 16:19:43.748290 moira-python-client-3.0.0/moira_client/
--rw-r--r--   0 runner    (1001) docker     (116)       37 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3474 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-11 16:19:43.752290 moira-python-client-3.0.0/moira_client/models/
--rw-r--r--   0 runner    (1001) docker     (116)      126 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      385 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     4561 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (116)     1375 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/health.py
--rw-r--r--   0 runner    (1001) docker     (116)     1946 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1619 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/pattern.py
--rw-r--r--   0 runner    (1001) docker     (116)     7891 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (116)     4336 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (116)    16826 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/trigger.py
--rw-r--r--   0 runner    (1001) docker     (116)     1767 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (116)     3601 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/moira_client/moira.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-11 16:19:43.752290 moira-python-client-3.0.0/moira_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2023-01-11 16:19:43.000000 moira-python-client-3.0.0/moira_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      753 2023-01-11 16:19:43.000000 moira-python-client-3.0.0/moira_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-11 16:19:43.000000 moira-python-client-3.0.0/moira_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-01-11 16:19:43.000000 moira-python-client-3.0.0/moira_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-01-11 16:19:43.000000 moira-python-client-3.0.0/moira_python_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2023-01-11 16:19:43.752290 moira-python-client-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1477 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       11 2023-01-11 16:19:27.000000 moira-python-client-3.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 11:36:47.508425 moira-python-client-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-04 11:36:47.508425 moira-python-client-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 11:36:47.504425 moira-python-client-4.0.0/moira_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 11:36:47.504425 moira-python-client-4.0.0/moira_client/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/health.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7891 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4336 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16889 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3601 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/moira_client/moira.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 11:36:47.508425 moira-python-client-4.0.0/moira_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-04 11:36:47.000000 moira-python-client-4.0.0/moira_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-04 11:36:47.000000 moira-python-client-4.0.0/moira_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 11:36:47.000000 moira-python-client-4.0.0/moira_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-04 11:36:47.000000 moira-python-client-4.0.0/moira_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-04 11:36:47.000000 moira-python-client-4.0.0/moira_python_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-04 11:36:47.508425 moira-python-client-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 11:36:47.508425 moira-python-client-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-05-04 11:36:33.000000 moira-python-client-4.0.0/tests/test_client.py
```

### Comparing `moira-python-client-3.0.0/CHANGELOG.md` & `moira-python-client-4.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/LICENSE` & `moira-python-client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/PKG-INFO` & `moira-python-client-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moira-python-client
-Version: 3.0.0
+Version: 4.0.0
 Summary: Client for Moira - Alerting system based on Graphite data
 Home-page: https://github.com/moira-alert/python-moira-client
 Author: Alexander Lukyanchenko
 Author-email: al.lukyanchenko@gmail.com
 Keywords: moira monitoring client metrics alerting
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moira-python-client-3.0.0/README.md` & `moira-python-client-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/client.py` & `moira-python-client-4.0.0/moira_client/client.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/config.py` & `moira-python-client-4.0.0/moira_client/models/config.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/contact.py` & `moira-python-client-4.0.0/moira_client/models/contact.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/event.py` & `moira-python-client-4.0.0/moira_client/models/event.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/health.py` & `moira-python-client-4.0.0/moira_client/models/health.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/notification.py` & `moira-python-client-4.0.0/moira_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/pattern.py` & `moira-python-client-4.0.0/moira_client/models/pattern.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/subscription.py` & `moira-python-client-4.0.0/moira_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/tag.py` & `moira-python-client-4.0.0/moira_client/models/tag.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/models/trigger.py` & `moira-python-client-4.0.0/moira_client/models/trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 RISING_TRIGGER = 'rising'
 FALLING_TRIGGER = 'falling'
 EXPRESSION_TRIGGER = 'expression'
 
 
 class Trigger(Base):
+    QUERY_PARAM_VALIDATE_FLAG = 'validate'
 
     def __init__(
             self,
             client,
             name,
             tags,
             targets,
@@ -145,46 +146,45 @@
         }
 
         if trigger_id:
             data['id'] = trigger_id
             api_response = TriggerManager(self._client).fetch_by_id(trigger_id)
 
         if trigger_id and api_response:
-            res = self._client.put('trigger/{id}'.format(id=trigger_id), json=data)
+            res = self._client.put(f'trigger/{trigger_id}?{self.QUERY_PARAM_VALIDATE_FLAG}', json=data)
         else:
-            res = self._client.put('trigger', json=data)
-        
+            res = self._client.put(f'trigger?{self.QUERY_PARAM_VALIDATE_FLAG}', json=data)
+
         if 'id' not in res:
             raise ResponseStructureError('id not in response', res)
-        
+
         self._id = res['id']
-        return self._id
+        return res
 
     def save(self):
         """
         Save trigger
 
-        :return: trigger_id
+        :return: response object
         """
         if self._id:
             return self.update()
         trigger = self.check_exists()
 
         if trigger:
             self._id = trigger.id
-            self.update()
-            return trigger.id
+            return self.update()
 
         return self._send_request()
 
     def update(self):
         """
         Update trigger
 
-        :return: trigger id
+        :return: response object
         """
         return self._send_request(self._id)
 
     def set_start_hour(self, hour):
         """
         Set start hour
```

### Comparing `moira-python-client-3.0.0/moira_client/models/user.py` & `moira-python-client-4.0.0/moira_client/models/user.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_client/moira.py` & `moira-python-client-4.0.0/moira_client/moira.py`

 * *Files identical despite different names*

### Comparing `moira-python-client-3.0.0/moira_python_client.egg-info/PKG-INFO` & `moira-python-client-4.0.0/moira_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moira-python-client
-Version: 3.0.0
+Version: 4.0.0
 Summary: Client for Moira - Alerting system based on Graphite data
 Home-page: https://github.com/moira-alert/python-moira-client
 Author: Alexander Lukyanchenko
 Author-email: al.lukyanchenko@gmail.com
 Keywords: moira monitoring client metrics alerting
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moira-python-client-3.0.0/moira_python_client.egg-info/SOURCES.txt` & `moira-python-client-4.0.0/moira_python_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 moira_client/models/tag.py
 moira_client/models/trigger.py
 moira_client/models/user.py
 moira_python_client.egg-info/PKG-INFO
 moira_python_client.egg-info/SOURCES.txt
 moira_python_client.egg-info/dependency_links.txt
 moira_python_client.egg-info/requires.txt
-moira_python_client.egg-info/top_level.txt
+moira_python_client.egg-info/top_level.txt
+tests/test_client.py
```

### Comparing `moira-python-client-3.0.0/setup.py` & `moira-python-client-4.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='moira-python-client',
-    version='3.0.0',
+    version='4.0.0',
     description='Client for Moira - Alerting system based on Graphite data',
     keywords='moira monitoring client metrics alerting',
     long_description="""
         Moira is a real-time alerting tool, based on Graphite data.
         moira-client is a python client for Moira API.
         Key features:
         - create, update, delete, manage triggers
```

