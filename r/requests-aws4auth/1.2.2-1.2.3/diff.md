# Comparing `tmp/requests-aws4auth-1.2.2.tar.gz` & `tmp/requests-aws4auth-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-aws4auth-1.2.2.tar", last modified: Fri Feb  3 03:41:33 2023, max compression
+gzip compressed data, was "requests-aws4auth-1.2.3.tar", last modified: Wed May  3 22:43:39 2023, max compression
```

## Comparing `requests-aws4auth-1.2.2.tar` & `requests-aws4auth-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-02-03 03:41:33.000541 requests-aws4auth-1.2.2/
--rw-r--r--   0 ted        (501) staff       (20)     1082 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.2/LICENSE
--rw-r--r--   0 ted        (501) staff       (20)    18015 2023-02-03 03:41:33.000619 requests-aws4auth-1.2.2/PKG-INFO
--rw-r--r--   0 ted        (501) staff       (20)    10619 2023-01-25 17:32:40.000000 requests-aws4auth-1.2.2/README.md
-drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-02-03 03:41:32.999590 requests-aws4auth-1.2.2/requests_aws4auth/
--rw-r--r--   0 ted        (501) staff       (20)     8452 2023-02-03 03:38:36.000000 requests-aws4auth-1.2.2/requests_aws4auth/__init__.py
--rw-r--r--   0 ted        (501) staff       (20)    33951 2023-02-03 03:37:30.000000 requests-aws4auth-1.2.2/requests_aws4auth/aws4auth.py
--rw-r--r--   0 ted        (501) staff       (20)     5437 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.2/requests_aws4auth/aws4signingkey.py
--rw-r--r--   0 ted        (501) staff       (20)      408 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.2/requests_aws4auth/exceptions.py
-drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-02-03 03:41:33.000398 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/
--rw-r--r--   0 ted        (501) staff       (20)    18015 2023-02-03 03:41:32.000000 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/PKG-INFO
--rw-r--r--   0 ted        (501) staff       (20)      368 2023-02-03 03:41:32.000000 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/SOURCES.txt
--rw-r--r--   0 ted        (501) staff       (20)        1 2023-02-03 03:41:32.000000 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/dependency_links.txt
--rw-r--r--   0 ted        (501) staff       (20)       28 2023-02-03 03:41:32.000000 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/requires.txt
--rw-r--r--   0 ted        (501) staff       (20)       18 2023-02-03 03:41:32.000000 requests-aws4auth-1.2.2/requests_aws4auth.egg-info/top_level.txt
--rw-r--r--   0 ted        (501) staff       (20)       67 2023-02-03 03:41:33.001164 requests-aws4auth-1.2.2/setup.cfg
--rw-r--r--   0 ted        (501) staff       (20)     2223 2023-01-20 22:33:41.000000 requests-aws4auth-1.2.2/setup.py
+drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-05-03 22:43:39.782768 requests-aws4auth-1.2.3/
+-rw-r--r--   0 ted        (501) staff       (20)     6310 2023-05-03 22:35:11.000000 requests-aws4auth-1.2.3/HISTORY.md
+-rw-r--r--   0 ted        (501) staff       (20)     1082 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.3/LICENSE
+-rw-r--r--   0 ted        (501) staff       (20)       37 2023-05-03 22:34:02.000000 requests-aws4auth-1.2.3/MANIFEST.in
+-rw-r--r--   0 ted        (501) staff       (20)    18130 2023-05-03 22:43:39.782835 requests-aws4auth-1.2.3/PKG-INFO
+-rw-r--r--   0 ted        (501) staff       (20)    10619 2023-01-25 17:32:40.000000 requests-aws4auth-1.2.3/README.md
+drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-05-03 22:43:39.781891 requests-aws4auth-1.2.3/requests_aws4auth/
+-rw-r--r--   0 ted        (501) staff       (20)     8452 2023-05-03 22:35:17.000000 requests-aws4auth-1.2.3/requests_aws4auth/__init__.py
+-rw-r--r--   0 ted        (501) staff       (20)    33951 2023-02-03 03:37:30.000000 requests-aws4auth-1.2.3/requests_aws4auth/aws4auth.py
+-rw-r--r--   0 ted        (501) staff       (20)     5437 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.3/requests_aws4auth/aws4signingkey.py
+-rw-r--r--   0 ted        (501) staff       (20)      408 2023-01-20 22:14:59.000000 requests-aws4auth-1.2.3/requests_aws4auth/exceptions.py
+drwxr-xr-x   0 ted        (501) staff       (20)        0 2023-05-03 22:43:39.782655 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/
+-rw-r--r--   0 ted        (501) staff       (20)    18130 2023-05-03 22:43:39.000000 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/PKG-INFO
+-rw-r--r--   0 ted        (501) staff       (20)      391 2023-05-03 22:43:39.000000 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/SOURCES.txt
+-rw-r--r--   0 ted        (501) staff       (20)        1 2023-05-03 22:43:39.000000 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/dependency_links.txt
+-rw-r--r--   0 ted        (501) staff       (20)       28 2023-05-03 22:43:39.000000 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/requires.txt
+-rw-r--r--   0 ted        (501) staff       (20)       18 2023-05-03 22:43:39.000000 requests-aws4auth-1.2.3/requests_aws4auth.egg-info/top_level.txt
+-rw-r--r--   0 ted        (501) staff       (20)       67 2023-05-03 22:43:39.783067 requests-aws4auth-1.2.3/setup.cfg
+-rw-r--r--   0 ted        (501) staff       (20)     2223 2023-01-20 22:33:41.000000 requests-aws4auth-1.2.3/setup.py
```

### Comparing `requests-aws4auth-1.2.2/LICENSE` & `requests-aws4auth-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-aws4auth-1.2.2/PKG-INFO` & `requests-aws4auth-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: requests-aws4auth
-Version: 1.2.2
+Version: 1.2.3
 Summary: AWS4 authentication for Requests
 Home-page: https://github.com/tedder/requests-aws4auth
-Download-URL: https://github.com/tedder/requests-aws4auth/tarball/1.2.2
+Download-URL: https://github.com/tedder/requests-aws4auth/tarball/1.2.3
 Author: Ted Timmons
 Author-email: ted@tedder.dev
 License: MIT License
 Keywords: requests authentication amazon web services aws s3 REST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -291,14 +291,21 @@
 python3 setup.py sdist bdist_wheel && \
 python3 -m twine upload --repository testpypi_requests_aws4auth dist/* && \
 python3 -m twine upload --repository pypi dist/*
 ```
 
 
 
+1.2.3 (2023-05-03)
+=========
+
+**Changes**
+
+- Add manifest file so tarball installs succeed, #66. Thanks @jantman.
+
 1.2.2 (2023-02-02)
 =========
 
 **Bugfixes**
 
 - The 1.2.0/1.2.1 releases had a regression error. The fix of #63 has been reverted.
```

### Comparing `requests-aws4auth-1.2.2/README.md` & `requests-aws4auth-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `requests-aws4auth-1.2.2/requests_aws4auth/__init__.py` & `requests-aws4auth-1.2.3/requests_aws4auth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 from .aws4auth import AWS4Auth, StrictAWS4Auth, PassiveAWS4Auth
 from .aws4signingkey import AWS4SigningKey
 from .exceptions import RequestsAws4AuthException, DateMismatchError, NoSecretKeyError
 del aws4auth
 del aws4signingkey
 del exceptions
 
-__version__ = '1.2.2'
+__version__ = '1.2.3'
```

### Comparing `requests-aws4auth-1.2.2/requests_aws4auth/aws4auth.py` & `requests-aws4auth-1.2.3/requests_aws4auth/aws4auth.py`

 * *Files identical despite different names*

### Comparing `requests-aws4auth-1.2.2/requests_aws4auth/aws4signingkey.py` & `requests-aws4auth-1.2.3/requests_aws4auth/aws4signingkey.py`

 * *Files identical despite different names*

### Comparing `requests-aws4auth-1.2.2/requests_aws4auth.egg-info/PKG-INFO` & `requests-aws4auth-1.2.3/requests_aws4auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: requests-aws4auth
-Version: 1.2.2
+Version: 1.2.3
 Summary: AWS4 authentication for Requests
 Home-page: https://github.com/tedder/requests-aws4auth
-Download-URL: https://github.com/tedder/requests-aws4auth/tarball/1.2.2
+Download-URL: https://github.com/tedder/requests-aws4auth/tarball/1.2.3
 Author: Ted Timmons
 Author-email: ted@tedder.dev
 License: MIT License
 Keywords: requests authentication amazon web services aws s3 REST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -291,14 +291,21 @@
 python3 setup.py sdist bdist_wheel && \
 python3 -m twine upload --repository testpypi_requests_aws4auth dist/* && \
 python3 -m twine upload --repository pypi dist/*
 ```
 
 
 
+1.2.3 (2023-05-03)
+=========
+
+**Changes**
+
+- Add manifest file so tarball installs succeed, #66. Thanks @jantman.
+
 1.2.2 (2023-02-02)
 =========
 
 **Bugfixes**
 
 - The 1.2.0/1.2.1 releases had a regression error. The fix of #63 has been reverted.
```

### Comparing `requests-aws4auth-1.2.2/setup.py` & `requests-aws4auth-1.2.3/setup.py`

 * *Files identical despite different names*

