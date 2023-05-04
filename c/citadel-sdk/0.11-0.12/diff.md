# Comparing `tmp/citadel_sdk-0.11.tar.gz` & `tmp/citadel_sdk-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citadel_sdk-0.11.tar", last modified: Thu May  4 09:43:05 2023, max compression
+gzip compressed data, was "citadel_sdk-0.12.tar", last modified: Thu May  4 10:14:11 2023, max compression
```

## Comparing `citadel_sdk-0.11.tar` & `citadel_sdk-0.12.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-04 09:43:05.867079 citadel_sdk-0.11/
--rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)      881 2023-05-04 09:43:05.867079 citadel_sdk-0.11/PKG-INFO
-drwxrwxr-x   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-04 09:43:05.867079 citadel_sdk-0.11/citadel_sdk/
--rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-02 14:21:37.277678 citadel_sdk-0.11/citadel_sdk/__init__.py
--rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)    28126 2023-05-02 14:21:37.277678 citadel_sdk-0.11/citadel_sdk/client.py
--rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)       62 2023-05-02 14:31:37.916271 citadel_sdk-0.11/setup.cfg
--rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)     1742 2023-05-04 09:43:03.379067 citadel_sdk-0.11/setup.py
+drwxrwxr-x   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-04 10:14:11.083311 citadel_sdk-0.12/
+-rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)      898 2023-05-04 10:14:11.083311 citadel_sdk-0.12/PKG-INFO
+drwxrwxr-x   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-04 10:14:11.083311 citadel_sdk-0.12/citadel_sdk/
+-rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)        0 2023-05-02 14:21:37.277678 citadel_sdk-0.12/citadel_sdk/__init__.py
+-rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)    28126 2023-05-02 14:21:37.277678 citadel_sdk-0.12/citadel_sdk/client.py
+-rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)       62 2023-05-02 14:31:37.916271 citadel_sdk-0.12/setup.cfg
+-rw-rw-r--   0 ksatzke   (1002) ksatzke   (1002)     1759 2023-05-04 10:09:43.710151 citadel_sdk-0.12/setup.py
```

### Comparing `citadel_sdk-0.11/PKG-INFO` & `citadel_sdk-0.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: citadel_sdk
-Version: 0.11
+Version: 0.12
 Summary: Citadel SDK
 Home-page: https://github.com/ksatzke/citadel_sdk
 Author: Citadel authors
 Author-email: ksatzke@msn.com
 License: MIT
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Download-URL: https://github.com/ksatzke/citadel-sdk/archive/refs/tags/v_012.tar.gz
 Description: UNKNOWN
 Keywords: Citadel,SDK,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `citadel_sdk-0.11/citadel_sdk/client.py` & `citadel_sdk-0.12/citadel_sdk/client.py`

 * *Files identical despite different names*

### Comparing `citadel_sdk-0.11/setup.py` & `citadel_sdk-0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'citadel_sdk',         # How you named your package folder (MyLib)
   packages = ['citadel_sdk'],   # Chose the same as "name"
-  version = '0.11',      # Start with a small number and increase it with every change you make
+  version = '0.12',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Citadel SDK',   # Give a short description about your library
   author = 'Citadel authors',            # Type in your name
   author_email = 'ksatzke@msn.com',      # Type in your E-Mail
   url = 'https://github.com/ksatzke/citadel_sdk',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ksatzke/citadel-sdk/archive/refs/tags/v_012.tar.gz',    # I explain this later on
   keywords = ['Citadel', 'SDK', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'urllib3',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

