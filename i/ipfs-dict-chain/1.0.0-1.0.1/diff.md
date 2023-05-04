# Comparing `tmp/ipfs_dict_chain-1.0.0.tar.gz` & `tmp/ipfs_dict_chain-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfs_dict_chain-1.0.0.tar", last modified: Thu May  4 00:16:33 2023, max compression
+gzip compressed data, was "ipfs_dict_chain-1.0.1.tar", last modified: Thu May  4 00:46:42 2023, max compression
```

## Comparing `ipfs_dict_chain-1.0.0.tar` & `ipfs_dict_chain-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 00:16:33.952143 ipfs_dict_chain-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      575 2023-05-04 00:16:33.951143 ipfs_dict_chain-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2383 2023-05-03 23:43:55.000000 ipfs_dict_chain-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 00:16:33.933145 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/
--rw-rw-rw-   0        0        0      575 2023-05-04 00:16:33.000000 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-05-04 00:16:33.000000 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 00:16:33.000000 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-04 00:16:33.000000 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 00:16:33.000000 ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 00:16:33.952143 ipfs_dict_chain-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-04 00:09:24.000000 ipfs_dict_chain-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 00:16:33.949141 ipfs_dict_chain-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-05-02 23:06:34.000000 ipfs_dict_chain-1.0.0/tests/test_CID.py
--rw-rw-rw-   0        0        0     1129 2023-05-02 22:56:08.000000 ipfs_dict_chain-1.0.0/tests/test_IPFS.py
--rw-rw-rw-   0        0        0     1453 2023-05-03 22:29:23.000000 ipfs_dict_chain-1.0.0/tests/test_IPFSDict.py
--rw-rw-rw-   0        0        0     1628 2023-05-03 22:39:19.000000 ipfs_dict_chain-1.0.0/tests/test_IPFSDictChain.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:42.352255 ipfs_dict_chain-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-04 00:46:33.000000 ipfs_dict_chain-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      575 2023-05-04 00:46:42.352255 ipfs_dict_chain-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2383 2023-05-03 23:43:55.000000 ipfs_dict_chain-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:42.340578 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-05-04 00:46:42.000000 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-05-04 00:46:42.000000 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 00:46:42.000000 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-04 00:46:42.000000 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 00:46:42.000000 ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 00:46:42.352255 ipfs_dict_chain-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-04 00:46:33.000000 ipfs_dict_chain-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:46:42.350257 ipfs_dict_chain-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-05-02 23:06:34.000000 ipfs_dict_chain-1.0.1/tests/test_CID.py
+-rw-rw-rw-   0        0        0     1129 2023-05-02 22:56:08.000000 ipfs_dict_chain-1.0.1/tests/test_IPFS.py
+-rw-rw-rw-   0        0        0     1453 2023-05-03 22:29:23.000000 ipfs_dict_chain-1.0.1/tests/test_IPFSDict.py
+-rw-rw-rw-   0        0        0     1628 2023-05-03 22:39:19.000000 ipfs_dict_chain-1.0.1/tests/test_IPFSDictChain.py
```

### Comparing `ipfs_dict_chain-1.0.0/LICENSE` & `ipfs_dict_chain-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.0/PKG-INFO` & `ipfs_dict_chain-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfs_dict_chain
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.
 Home-page: https://github.com/ValyrianTech/ipfs_dict_chain
 Author: Wouter Glorieux
 Author-email: info@valyrian.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfs_dict_chain-1.0.0/README.md` & `ipfs_dict_chain-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.0/ipfs_dict_chain.egg-info/PKG-INFO` & `ipfs_dict_chain-1.0.1/ipfs_dict_chain.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfs-dict-chain
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.
 Home-page: https://github.com/ValyrianTech/ipfs_dict_chain
 Author: Wouter Glorieux
 Author-email: info@valyrian.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfs_dict_chain-1.0.0/setup.py` & `ipfs_dict_chain-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipfs_dict_chain',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.',
     author='Wouter Glorieux',
     author_email='info@valyrian.tech',
     url='https://github.com/ValyrianTech/ipfs_dict_chain',
     packages=find_packages(),
     install_requires=[
         'aioipfs>=0.6.3',
```

### Comparing `ipfs_dict_chain-1.0.0/tests/test_CID.py` & `ipfs_dict_chain-1.0.1/tests/test_CID.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.0/tests/test_IPFS.py` & `ipfs_dict_chain-1.0.1/tests/test_IPFS.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.0/tests/test_IPFSDict.py` & `ipfs_dict_chain-1.0.1/tests/test_IPFSDict.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.0/tests/test_IPFSDictChain.py` & `ipfs_dict_chain-1.0.1/tests/test_IPFSDictChain.py`

 * *Files identical despite different names*

