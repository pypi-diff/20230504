# Comparing `tmp/aioauth-1.5.3.tar.gz` & `tmp/aioauth-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioauth-1.5.3.tar", last modified: Tue Mar 28 21:43:05 2023, max compression
+gzip compressed data, was "aioauth-1.5.4.tar", last modified: Thu May  4 16:19:15 2023, max compression
```

## Comparing `aioauth-1.5.3.tar` & `aioauth-1.5.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:43:05.051872 aioauth-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-28 21:42:50.000000 aioauth-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-28 21:43:05.051872 aioauth-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-28 21:42:50.000000 aioauth-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:43:05.051872 aioauth-1.5.3/aioauth/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/constances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/grant_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-03-28 21:42:50.000000 aioauth-1.5.3/aioauth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:43:05.051872 aioauth-1.5.3/aioauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-28 21:43:04.000000 aioauth-1.5.3/aioauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-28 21:43:04.000000 aioauth-1.5.3/aioauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:43:04.000000 aioauth-1.5.3/aioauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-28 21:43:04.000000 aioauth-1.5.3/aioauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 21:43:04.000000 aioauth-1.5.3/aioauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-28 21:43:05.051872 aioauth-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-28 21:42:50.000000 aioauth-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:19:15.372056 aioauth-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 16:18:51.000000 aioauth-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-04 16:19:15.372056 aioauth-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-04 16:18:51.000000 aioauth-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:19:15.372056 aioauth-1.5.4/aioauth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/constances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/grant_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-05-04 16:18:51.000000 aioauth-1.5.4/aioauth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:19:15.372056 aioauth-1.5.4/aioauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-04 16:19:15.000000 aioauth-1.5.4/aioauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 16:19:15.000000 aioauth-1.5.4/aioauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:19:15.000000 aioauth-1.5.4/aioauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 16:19:15.000000 aioauth-1.5.4/aioauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 16:19:15.000000 aioauth-1.5.4/aioauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 16:19:15.372056 aioauth-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-04 16:18:51.000000 aioauth-1.5.4/setup.py
```

### Comparing `aioauth-1.5.3/LICENSE` & `aioauth-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/PKG-INFO` & `aioauth-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioauth
-Version: 1.5.3
+Version: 1.5.4
 Summary: Asynchronous OAuth 2.0 framework for Python 3.
 Home-page: https://github.com/aliev/aioauth
 Author: Ali Aliyev
 Author-email: ali@aliev.me
 License: The MIT License (MIT)
 Project-URL: Source, https://github.com/aliev/aioauth
 Description: ## Asynchronous OAuth 2.0 framework for Python 3
```

### Comparing `aioauth-1.5.3/README.md` & `aioauth-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/collections.py` & `aioauth-1.5.4/aioauth/collections.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/config.py` & `aioauth-1.5.4/aioauth/config.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/constances.py` & `aioauth-1.5.4/aioauth/constances.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/errors.py` & `aioauth-1.5.4/aioauth/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,17 @@
 
     def __init__(
         self,
         request: TRequest,
         description: Optional[str] = None,
         headers: Optional[HTTPHeaderDict] = None,
     ):
-        super().__init__(request, description, headers or HTTPHeaderDict())
+        super().__init__(
+            request, description, headers or HTTPHeaderDict(default_headers)
+        )
 
         auth_values = [f"error={self.error}"]
         if self.description:
             auth_values.append(f"error_description={self.description}")
         if self.error_uri:
             auth_values.append(f"error_uri={self.error_uri}")
         self.headers["WWW-Authenticate"] = "Basic " + ", ".join(auth_values)
```

### Comparing `aioauth-1.5.3/aioauth/grant_type.py` & `aioauth-1.5.4/aioauth/grant_type.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/models.py` & `aioauth-1.5.4/aioauth/models.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/requests.py` & `aioauth-1.5.4/aioauth/requests.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/response_type.py` & `aioauth-1.5.4/aioauth/response_type.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/responses.py` & `aioauth-1.5.4/aioauth/responses.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/server.py` & `aioauth-1.5.4/aioauth/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         ]
 
         if token and not token.is_expired and not token.revoked:
             token_response = TokenActiveIntrospectionResponse(
                 scope=token.scope,
                 client_id=token.client_id,
                 expires_in=token.expires_in,
-                token_type=token_type,
+                token_type=token.token_type,
             )
         else:
             token_response = TokenInactiveIntrospectionResponse()
 
         content = asdict(token_response)
 
         return Response(
```

### Comparing `aioauth-1.5.3/aioauth/storage.py` & `aioauth-1.5.4/aioauth/storage.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/types.py` & `aioauth-1.5.4/aioauth/types.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth/utils.py` & `aioauth-1.5.4/aioauth/utils.py`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/aioauth.egg-info/PKG-INFO` & `aioauth-1.5.4/aioauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioauth
-Version: 1.5.3
+Version: 1.5.4
 Summary: Asynchronous OAuth 2.0 framework for Python 3.
 Home-page: https://github.com/aliev/aioauth
 Author: Ali Aliyev
 Author-email: ali@aliev.me
 License: The MIT License (MIT)
 Project-URL: Source, https://github.com/aliev/aioauth
 Description: ## Asynchronous OAuth 2.0 framework for Python 3
```

### Comparing `aioauth-1.5.3/setup.cfg` & `aioauth-1.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioauth-1.5.3/setup.py` & `aioauth-1.5.4/setup.py`

 * *Files identical despite different names*

