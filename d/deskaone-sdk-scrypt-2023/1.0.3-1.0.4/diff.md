# Comparing `tmp/deskaone_sdk_scrypt_2023-1.0.3.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.0.3.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.0.4.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.0.3.tar` & `deskaone_sdk_scrypt_2023-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      734 2023-05-04 06:49:19.751594 deskaone_sdk_scrypt_2023-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.0.3/README.md
--rw-r--r--   0        0        0      388 2023-05-02 07:28:00.336409 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     5987 2023-05-02 09:12:34.116954 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0      823 2023-03-29 02:19:26.852041 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-02 07:26:37.562775 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      477 2023-05-04 06:49:24.014580 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     1901 2023-03-27 01:24:30.967144 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    17776 2023-05-04 06:49:07.198058 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.3/setup.py
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-05-04 07:01:57.726064 deskaone_sdk_scrypt_2023-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.0.4/README.md
+-rw-r--r--   0        0        0      388 2023-05-02 07:28:00.336409 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     5993 2023-05-04 07:01:51.651028 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0      823 2023-03-29 02:19:26.852041 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-02 07:26:37.562775 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      477 2023-05-04 07:02:02.501461 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     1901 2023-03-27 01:24:30.967144 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    17776 2023-05-04 06:49:07.198058 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.4/setup.py
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.4/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.secret_key = secret_key
 
     def __call__(self, request):
         timestamp   = str(int(time.time() * 1000))
         message     = str(timestamp + request.method + request.path_url + (request.body or ''))
         signature   = base64.b64encode(hmac.new(self.secret_key.encode(), message.encode(), 'SHA256').digest()).decode()
         request.headers.update({
-            'User-Agent'    : f'DesKaOne-Scrypt-V4@{__version_code__}',
+            'User-Agent'    : f'DesKaOne-Scrypt-SDK-2023@{__version_code__}',
             'SIGNATURE'     : signature,
             'TIMESTAMP'     : timestamp,
             'VERSION'       : __version_code__
         })
         return request
 
 class Client:
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/setup.py` & `deskaone_sdk_scrypt_2023-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.3/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

