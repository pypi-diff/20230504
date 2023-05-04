# Comparing `tmp/beards_analytics-0.1.9-py3-none-any.whl.zip` & `tmp/beards_analytics-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 10226 bytes, number of entries: 20
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-15 16:32 beards_analytics/__init__.py
+Zip file size: 10649 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       22 b- defN 23-May-04 09:59 beards_analytics/__init__.py
 -rw-r--r--  2.0 unx       19 b- defN 23-Apr-15 14:34 beards_analytics/cloud_functions/__init__.py
--rw-r--r--  2.0 unx     3087 b- defN 23-Apr-15 14:45 beards_analytics/cloud_functions/http.py
+-rw-r--r--  2.0 unx     3608 b- defN 23-Apr-18 14:15 beards_analytics/cloud_functions/http.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Apr-15 14:30 beards_analytics/common/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 15:43 beards_analytics/common/date.py
--rw-r--r--  2.0 unx     2869 b- defN 23-Apr-15 16:33 beards_analytics/common/logger.py
--rw-r--r--  2.0 unx     1342 b- defN 23-Apr-15 14:43 beards_analytics/common/tasks.py
+-rw-r--r--  2.0 unx     4034 b- defN 23-May-04 09:50 beards_analytics/common/logger.py
+-rw-r--r--  2.0 unx     1388 b- defN 23-Apr-18 10:36 beards_analytics/common/tasks.py
 -rw-r--r--  2.0 unx       82 b- defN 23-Apr-14 14:04 beards_analytics/common/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
--rw-r--r--  2.0 unx      782 b- defN 23-Apr-14 21:27 beards_analytics/data/operations.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-18 14:07 beards_analytics/data/operations.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 21:32 beards_analytics/public_api/__init__.py
 -rw-r--r--  2.0 unx     2846 b- defN 23-Apr-15 14:17 beards_analytics/public_api/_metadata.py
--rw-r--r--  2.0 unx     2168 b- defN 23-Apr-15 15:55 beards_analytics/public_api/client.py
+-rw-r--r--  2.0 unx     2107 b- defN 23-Apr-18 12:10 beards_analytics/public_api/client.py
 -rw-r--r--  2.0 unx      202 b- defN 23-Apr-14 20:48 beards_analytics/public_api/models.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-15 16:35 beards_analytics-0.1.9.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      731 b- defN 23-Apr-15 16:35 beards_analytics-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 16:35 beards_analytics-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-15 16:35 beards_analytics-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1798 b- defN 23-Apr-15 16:35 beards_analytics-0.1.9.dist-info/RECORD
-20 files, 18529 bytes uncompressed, 7214 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx     1060 b- defN 23-May-04 09:59 beards_analytics-2.0.0.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      814 b- defN 23-May-04 09:59 beards_analytics-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 09:59 beards_analytics-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-04 09:59 beards_analytics-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1798 b- defN 23-May-04 09:59 beards_analytics-2.0.0.dist-info/RECORD
+20 files, 20283 bytes uncompressed, 7637 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: beards_analytics/public_api/client.py
 Comment: 
 
 Filename: beards_analytics/public_api/models.py
 Comment: 
 
-Filename: beards_analytics-0.1.9.dist-info/LICENCE.txt
+Filename: beards_analytics-2.0.0.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.9.dist-info/METADATA
+Filename: beards_analytics-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.9.dist-info/WHEEL
+Filename: beards_analytics-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.9.dist-info/top_level.txt
+Filename: beards_analytics-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.9.dist-info/RECORD
+Filename: beards_analytics-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.9'
+__version__ = '2.0.0'
```

## beards_analytics/cloud_functions/http.py

```diff
@@ -1,13 +1,15 @@
 import typing as t
 import functools
 import pydantic
 import flask
 import ujson
 import functions_framework
+import werkzeug.exceptions
+from beards_analytics.common.logger import Logger
 
 
 _ENTRY_FUNC = t.Callable[[flask.Request], t.Any]
 _T_MODEL = t.TypeVar('_T_MODEL', bound=pydantic.BaseModel)
 _INPUT_SOURCE = '__input_source__'
 
 class _ConvertableDict(dict):
@@ -75,21 +77,32 @@
     func = functions_framework.http(func)
     func = safe_return(func)
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         _update_flask_request()
         
-        # TODO: Add exception handler
         try:
             return func(*args, **kwargs)
-        except pydantic.ValidationError as e:
-            if hasattr(e, _INPUT_SOURCE):
+        except Exception as e:
+            if isinstance(e, pydantic.ValidationError) and hasattr(e, _INPUT_SOURCE):
                 input_source: str = getattr(e, _INPUT_SOURCE)
                 return error_response(message=f'Invalid {input_source}', errors=e.errors(), status_code=400)
+            
+            if isinstance(e, werkzeug.exceptions.HTTPException) or flask.current_app._find_error_handler(e) != None:
+                raise
+
+            logger = Logger()
+            logger.alert(
+                message=f'Unhandled error: {e.__class__.__name__}',
+                labels=dict(unhandled_error=e.__class__.__name__),
+                error_msg=str(e),
+                error_name=e.__class__.__name__
+            )
+            
             raise
 
     return wrapper
 
 def api_key_auth(allowed_api_key: str, api_key_query_param_name: str = 'api_key'):
     def decorator(func: _ENTRY_FUNC):
         @functools.wraps(func)
```

## beards_analytics/common/logger.py

```diff
@@ -3,67 +3,80 @@
 from beards_analytics.public_api._metadata import K_SERVICE, PROJECT_ID
 from google.auth.exceptions import GoogleAuthError
 from google.auth.credentials import Credentials
 import typing as t
 import ujson
 
 
-class Logger:
-    _instance: "Logger" = None
-    
-    def __new__(cls) -> "Logger":
-        if not cls._instance:
-            cls._instance = super().__new__(cls)
-        return cls._instance
-    
-    def __init__(self, credentials: t.Optional[Credentials] = None) -> None:
-        self._ba_api_client = None
+# TODO: move to utils if needed in other modules
+def _singleton(cls):
+    instances = {}
+    def getinstance(*args, **kwargs):
+        if cls not in instances:
+            instances[cls] = cls(*args, **kwargs)
+        return instances[cls]
+    return getinstance
+
+@_singleton
+class Logger:    
+    def __init__(self, credentials: t.Optional[Credentials] = None, send_to_ba: bool = True) -> None:
         self._credentials = credentials
+        self._ba_api_client = None
+        self._send_to_ba = send_to_ba
 
-    def _log(self, severity: LogSeverity, message: str, send_to_ba=False, log_name=None, **kwargs):
+    def _log(self, severity: LogSeverity, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
         message = str(message)
         log_obj = dict(severity=severity.name, message=message, **kwargs)
+        
+        if labels:
+            log_obj.update(dict(labels=labels))
+        
+        # print log object to stdout
         print(ujson.dumps(log_obj))
+
+        send_to_ba = send_to_ba and self._send_to_ba
         
         if not send_to_ba or not K_SERVICE or not PROJECT_ID:
             return
         
         client = self._ba_api_client or BaPublicApiClient(credentials=self._credentials)
         self._ba_api_client = client
-        
-        if not log_name:
-            log_name = 'cloud_service'
             
         try:
-            client.create_cloud_log(log_name, message, severity, k_service=K_SERVICE, project_id=PROJECT_ID, extra=kwargs)
+            if len(message) < 3:
+                self.warning(f'Log message "{message}" must be at least 3 chars to be sent to BA.')
+                return
+            
+            client.create_cloud_log(message, severity, k_service=K_SERVICE, project_id=PROJECT_ID, labels=labels, extra=kwargs)
         except (GoogleAuthError, RuntimeWarning) as e:
             self.warning(e, send_to_ba=False)
             
-    def deafult(self, message: str, send_to_ba=False, **kwargs):
-        return self._log(LogSeverity.DEFAULT, message, send_to_ba, **kwargs)
+    def deafult(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
+        return self._log(LogSeverity.DEFAULT, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def debug(self, message: str, send_to_ba=False, **kwargs):
-        return self._log(LogSeverity.DEBUG, message, send_to_ba, **kwargs)
+    def debug(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
+        return self._log(LogSeverity.DEBUG, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def info(self, message: str, send_to_ba=False, **kwargs):
-        return self._log(LogSeverity.INFO, message, send_to_ba, **kwargs)
+    def info(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
+        return self._log(LogSeverity.INFO, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def notice(self, message: str, send_to_ba=False, **kwargs):
-        return self._log(LogSeverity.NOTICE, message, send_to_ba, **kwargs)
+    def notice(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
+        return self._log(LogSeverity.NOTICE, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
         
-    def warning(self, message: str, send_to_ba=False, **kwargs):
-        return self._log(LogSeverity.WARNING, message, send_to_ba, **kwargs)
+    def warning(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=False, **kwargs):
+        return self._log(LogSeverity.WARNING, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def error(self, message: str, send_to_ba=True, **kwargs):
-        return self._log(LogSeverity.ERROR, message, send_to_ba, **kwargs)
+    def error(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=True, **kwargs):
+        return self._log(LogSeverity.ERROR, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def critical(self, message: str, send_to_ba=True, **kwargs):
-        return self._log(LogSeverity.CRITICAL, message, send_to_ba, **kwargs)
+    def critical(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=True, **kwargs):
+        return self._log(LogSeverity.CRITICAL, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def alert(self, message: str, send_to_ba=True, **kwargs):
-        return self._log(LogSeverity.ALERT, message, send_to_ba, **kwargs)
+    def alert(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=True, **kwargs):
+        return self._log(LogSeverity.ALERT, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
-    def emergency(self, message: str, send_to_ba=True, **kwargs):
-        return self._log(LogSeverity.EMERGENCY, message, send_to_ba, **kwargs)
+    def emergency(self, message: str, labels: t.Optional[t.Mapping[str, str]] = None, send_to_ba=True, **kwargs):
+        return self._log(LogSeverity.EMERGENCY, message, send_to_ba=send_to_ba, labels=labels, **kwargs)
     
     def log_dbt_output(self, output: str):
+        # add dbt=true label
         raise NotImplementedError()
```

## beards_analytics/common/tasks.py

```diff
@@ -1,32 +1,33 @@
 from threading import Thread
 import functools
 import typing as t
 from .types import T, RT, P
 
 
 class Task(Thread, t.Generic[T]):
-    def __init__(self, group=None, target=None, name=None, args=None, kwargs=None):
+    def __init__(self, daemon=True, group=None, target=None, name=None, args=None, kwargs=None):
         args = args or tuple()
         kwargs = kwargs or dict()
         
         Thread.__init__(self, group, target, name, args, kwargs)
 
         self._result: t.Optional[T] = None
+        self.daemon = daemon
 
     @property
     def result(self) -> t.Optional[T]:
         return self._result
 
     def run(self):
         try:
             if self._target is not None:
                 self._result = self._target(*self._args, **self._kwargs)
         finally:
-            del self._target, self._result, self._args, self._kwargs
+            del self._target, self._args, self._kwargs
 
     def wait(self, timeout: t.Optional[float] = None) -> T:
         if self.result:
             return self.result
         Thread.join(self, timeout=timeout)
         return self.result
 
@@ -35,12 +36,12 @@
         results = []
         for task in tasks:
             results.append(task.wait())
         return results
 
 def task(func: t.Callable[P, RT]) -> t.Callable[P, Task[RT]]:
     @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> Task[RT]:
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Task[RT]:
         thread = Task(target=func, args=args, kwargs=kwargs)
         thread.start()
         return thread
     return wrapper
```

## beards_analytics/public_api/client.py

```diff
@@ -21,29 +21,28 @@
                 
         if self._credentials.expired or not self._credentials.token:
             self._credentials.refresh(GoogleRequest())
             
         res = requests.request(method, self._url_base + endpoint, json=json, params=params, headers={'x-id-token': self._credentials.token})
         
         if res.status_code == 403:
-            raise GoogleAuthError(f'Failed to use a BA service: {res.json()}')
+            raise GoogleAuthError(f'Forbidden to use a BA service: {res.json()}')
         
-        if res.status_code >= 500:
+        if res.status_code != 200:
             raise RuntimeWarning('Failed to use a BA service. Please report the issue to developers of Beards Analytics.')
         
         return res.json()
     
-    def create_cloud_log(self, log_name: str, message: str, severity: LogSeverity, k_service: str, project_id: Optional[str] = None, labels: Optional[Mapping[str, str]] = None, extra: Optional[Any] = None):
+    def create_cloud_log(self, message: str, severity: LogSeverity, k_service: str, project_id: Optional[str] = None, labels: Optional[Mapping[str, str]] = None, extra: Optional[Any] = None):
         payload = {
-            'logName': log_name,
             'message': message,
             'kService': k_service,
             'severity': severity.value,
             'projectId': project_id or self._project_id or 'UNKNOWN',
             'labels': labels,
             'extra': extra
         }
 
         response = self._request('POST', '/create-cloud-log', json=payload)
-                
+
         if not response.get('success'):
             raise RuntimeWarning(response)
```

## Comparing `beards_analytics-0.1.9.dist-info/LICENCE.txt` & `beards_analytics-2.0.0.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.9.dist-info/RECORD` & `beards_analytics-2.0.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-beards_analytics/__init__.py,sha256=2uYVJ4eLF8kKOzfX6k2Go3u7xIwcGSuemAueAoXn-5o,22
+beards_analytics/__init__.py,sha256=hwOJuFUEKtsgiOt4l6op9s-hviovM6TK1uCdtRNWY4E,22
 beards_analytics/cloud_functions/__init__.py,sha256=VmjSBaoSqXDln4jRE0CLkl_3OHZSs7hhNWcKx2B77hY,19
-beards_analytics/cloud_functions/http.py,sha256=JMIPreFkfLdLLmHKPbPrZbJVwro_-iqAtWOUxJXXVYo,3087
+beards_analytics/cloud_functions/http.py,sha256=jkIZNbKnsv5rRecSgpTlaD-7qGj6H8UC76exyDghP7c,3608
 beards_analytics/common/__init__.py,sha256=NeB4cKiZbcqp0STfAXFSD4iJ3DhoWxFFamzES17ldA4,51
 beards_analytics/common/date.py,sha256=amLlla8Smayw8ZnEAS0lJebusnIaBBAdxA0u-h_tl7M,847
-beards_analytics/common/logger.py,sha256=r8Hhr_J7iVrG8fhWCCadloNbfagwZdjd9h8lv7DsE38,2869
-beards_analytics/common/tasks.py,sha256=AtqrXtAGLQglvZ_F-jiiO7QBE1gLmaTOs-QAfvkaM8w,1342
+beards_analytics/common/logger.py,sha256=SezkNf96PanSjDj0MYv02FxcH8Ep39ReJkc1n4SPGq0,4034
+beards_analytics/common/tasks.py,sha256=cz-ut_xDs1Frha0wz5hMGXyI67IVsyDpS0GTaApFUio,1388
 beards_analytics/common/types.py,sha256=xZytT7TyUMhpYvYjlAPQd5mcn56nn6npq_EcEPF3Hs4,82
 beards_analytics/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/data/models.py,sha256=79oHvRbMaWTz_o1GK2dIqL6Uh2cIIVbnel4JcxUkHxk,514
 beards_analytics/data/operations.py,sha256=QwIoW6LXlhAVH7RGM8xkW7DgC7qAD1De_1sulm_zBLU,782
 beards_analytics/public_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/public_api/_metadata.py,sha256=J_DTAsBfsssGvp09MY9y_pUQQqpbdVpwOE_H2RFJZh0,2846
-beards_analytics/public_api/client.py,sha256=YQ8qD7QJB3M05-eS5Tt4om26mxdRtEJDFYZgA_xZYtk,2168
+beards_analytics/public_api/client.py,sha256=RwBmr9UYDHQ2R0bxfKZ43jzLNlQLy13hFEGlqgGLT3M,2107
 beards_analytics/public_api/models.py,sha256=E4CLlm9ddN3r5w1S-GDmxBGLbWhStNJG85u-jgBXZUk,202
-beards_analytics-0.1.9.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
-beards_analytics-0.1.9.dist-info/METADATA,sha256=UqV4Q6VmfLuQU714hjBoW4rwjFMMwp_dljgpym-vAls,731
-beards_analytics-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-beards_analytics-0.1.9.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
-beards_analytics-0.1.9.dist-info/RECORD,,
+beards_analytics-2.0.0.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
+beards_analytics-2.0.0.dist-info/METADATA,sha256=qoQvoToMIaJfmdSnO93Yo3txN8jTCBE-5IUhs_ax4tg,814
+beards_analytics-2.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+beards_analytics-2.0.0.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
+beards_analytics-2.0.0.dist-info/RECORD,,
```

