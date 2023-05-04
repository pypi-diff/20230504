# Comparing `tmp/requests-hawk-1.1.1.tar.gz` & `tmp/requests-hawk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests-hawk-1.1.1.tar", last modified: Fri Jun  4 17:00:08 2021, max compression
+gzip compressed data, was "requests-hawk-1.2.1.tar", last modified: Thu May  4 16:01:38 2023, max compression
```

## Comparing `requests-hawk-1.1.1.tar` & `requests-hawk-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rhubscher  (1000) rhubscher  (1000)        0 2021-06-04 17:00:08.950368 requests-hawk-1.1.1/
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     1132 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/CHANGES.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)      561 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/LICENSE.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)       59 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/MANIFEST.in
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     6802 2021-06-04 17:00:08.950368 requests-hawk-1.1.1/PKG-INFO
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     3486 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/README.rst
-drwxrwxr-x   0 rhubscher  (1000) rhubscher  (1000)        0 2021-06-04 17:00:08.946368 requests-hawk-1.1.1/requests_hawk/
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     4690 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk/__init__.py
-drwxrwxr-x   0 rhubscher  (1000) rhubscher  (1000)        0 2021-06-04 17:00:08.950368 requests-hawk-1.1.1/requests_hawk/tests/
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)        0 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk/tests/__init__.py
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     4949 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk/tests/test_hawkauth.py
-drwxrwxr-x   0 rhubscher  (1000) rhubscher  (1000)        0 2021-06-04 17:00:08.946368 requests-hawk-1.1.1/requests_hawk.egg-info/
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     6802 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/PKG-INFO
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)      420 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/SOURCES.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)        1 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/dependency_links.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)       65 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/entry_points.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)        1 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/not-zip-safe
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)       16 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/requires.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)       14 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/requests_hawk.egg-info/top_level.txt
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)      134 2021-06-04 17:00:08.950368 requests-hawk-1.1.1/setup.cfg
--rw-rw-r--   0 rhubscher  (1000) rhubscher  (1000)     1526 2021-06-04 17:00:08.000000 requests-hawk-1.1.1/setup.py
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     1310 2023-05-03 15:05:50.000000 requests-hawk-1.2.1/CHANGES.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      561 2023-05-03 15:00:44.000000 requests-hawk-1.2.1/LICENSE.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       59 2023-05-03 15:00:44.000000 requests-hawk-1.2.1/MANIFEST.in
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     5551 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/PKG-INFO
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     3486 2023-05-03 15:00:44.000000 requests-hawk-1.2.1/README.rst
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/requests_hawk/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4845 2023-05-03 15:02:55.000000 requests-hawk-1.2.1/requests_hawk/__init__.py
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/requests_hawk/tests/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        0 2023-05-03 15:00:44.000000 requests-hawk-1.2.1/requests_hawk/tests/__init__.py
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4949 2023-05-03 15:00:44.000000 requests-hawk-1.2.1/requests_hawk/tests/test_hawkauth.py
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/requests_hawk.egg-info/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     5551 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/PKG-INFO
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      420 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       64 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/entry_points.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2023-05-04 15:47:07.000000 requests-hawk-1.2.1/requests_hawk.egg-info/not-zip-safe
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       16 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/requires.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       14 2023-05-04 16:01:38.000000 requests-hawk-1.2.1/requests_hawk.egg-info/top_level.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      134 2023-05-04 16:01:38.169404 requests-hawk-1.2.1/setup.cfg
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     1526 2023-05-03 15:02:01.000000 requests-hawk-1.2.1/setup.py
```

### Comparing `requests-hawk-1.1.1/CHANGES.txt` & `requests-hawk-1.2.1/CHANGES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 CHANGELOG
 =========
 
+1.2.1 (2023-05-03)
+------------------
+
+- Add support for ext external data string (#34)
+  (thanks @jtmaclachlan)
+
+1.2.0 (unreleased)
+------------------
+
+- Nothing changed yet.
+
+
 1.1.1 (2021-06-04)
 ------------------
 
 - Handle cases where Content-Type is defined as bytes rather than string. (#25)
 - Allow for app mohawk sender parameter configuration
```

### Comparing `requests-hawk-1.1.1/LICENSE.txt` & `requests-hawk-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `requests-hawk-1.1.1/README.rst` & `requests-hawk-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `requests-hawk-1.1.1/requests_hawk/__init__.py` & `requests-hawk-1.2.1/requests_hawk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,23 @@
       (Optional, defaults to 'sha256').
 
     :param server_url:
       The url of the server, this is useful for hawk when signing the requests.
       In case this is omitted, fallbacks to the value of the "Host" header of
       the request (Optional).
 
+    :param ext:
+      A string of arbitrary data to be sent along with the request (Optional).
+
     Note that the `hawk_session` and `id` parameters are mutually exclusive.
     You should use either `hawk_session` or both `id` and 'key'.
     """
     def __init__(self, hawk_session=None, id=None, key=None, algorithm='sha256',
                  credentials=None, server_url=None, _timestamp=None,
-                 always_hash_content=True, app=None):
+                 always_hash_content=True, ext=None, app=None):
         if credentials is not None:
             raise AttributeError("The 'credentials' param has been removed. "
                                  "Pass 'id' and 'key' instead, or '**credentials_dict'.")
 
         if (hawk_session and (id or key)
                 or not hawk_session and not (id and key)):
             raise AttributeError("You should pass either 'hawk_session' "
@@ -64,14 +67,15 @@
             'id': id,
             'key': key,
             'algorithm': algorithm
         }
         self._timestamp = _timestamp
         self.host = urlparse(server_url).netloc if server_url else None
         self.always_hash_content = always_hash_content
+        self.ext = ext
         self.app = app
 
     def __call__(self, r):
         if self.host is not None:
             r.headers['Host'] = self.host
 
         content_type = r.headers.get("Content-Type") or ""
@@ -82,14 +86,15 @@
             self.credentials,
             r.url,
             r.method,
             content=r.body or EmptyValue,
             content_type=content_type or EmptyValue,
             always_hash_content=self.always_hash_content,
             _timestamp=self._timestamp,
+            ext=self.ext,
             app=self.app
         )
 
         r.headers['Authorization'] = sender.request_header
         return r
```

### Comparing `requests-hawk-1.1.1/requests_hawk/tests/test_hawkauth.py` & `requests-hawk-1.2.1/requests_hawk/tests/test_hawkauth.py`

 * *Files identical despite different names*

### Comparing `requests-hawk-1.1.1/setup.py` & `requests-hawk-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, 'CHANGES.txt'), encoding='utf-8') as f:
     CHANGES = f.read()
 
 requires = ['requests', 'mohawk']
 
 setup(name='requests-hawk',
-      version='1.1.1',
+      version='1.2.1',
       description='requests-hawk',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
           "Intended Audience :: Developers",
           "Programming Language :: Python",
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 2",
```

