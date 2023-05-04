# Comparing `tmp/ipfs_dict_chain-1.0.3.tar.gz` & `tmp/ipfs_dict_chain-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfs_dict_chain-1.0.3.tar", last modified: Thu May  4 01:30:37 2023, max compression
+gzip compressed data, was "ipfs_dict_chain-1.0.4.tar", last modified: Thu May  4 01:47:53 2023, max compression
```

## Comparing `ipfs_dict_chain-1.0.3.tar` & `ipfs_dict_chain-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 01:30:37.350613 ipfs_dict_chain-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-04 01:15:25.000000 ipfs_dict_chain-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      575 2023-05-04 01:30:37.349626 ipfs_dict_chain-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2383 2023-05-03 23:43:55.000000 ipfs_dict_chain-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 01:30:37.330612 ipfs_dict_chain-1.0.3/ipfs_dict_chain/
--rw-rw-rw-   0        0        0     1774 2023-05-03 22:46:27.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain/CID.py
--rw-rw-rw-   0        0        0     4416 2023-05-03 23:13:55.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFS.py
--rw-rw-rw-   0        0        0     2334 2023-05-03 22:44:51.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFSDict.py
--rw-rw-rw-   0        0        0     3472 2023-05-03 22:37:20.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFSDictChain.py
--rw-rw-rw-   0        0        0      101 2023-05-03 23:49:50.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:30:37.339612 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/
--rw-rw-rw-   0        0        0      575 2023-05-04 01:30:37.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-04 01:30:37.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 01:30:37.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-04 01:30:37.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 01:30:37.000000 ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 01:30:37.350613 ipfs_dict_chain-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-05-04 01:16:24.000000 ipfs_dict_chain-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:30:37.348611 ipfs_dict_chain-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-05-04 01:27:56.000000 ipfs_dict_chain-1.0.3/tests/test_CID.py
--rw-rw-rw-   0        0        0     1129 2023-05-04 01:29:17.000000 ipfs_dict_chain-1.0.3/tests/test_IPFS.py
--rw-rw-rw-   0        0        0     1453 2023-05-04 01:29:21.000000 ipfs_dict_chain-1.0.3/tests/test_IPFSDict.py
--rw-rw-rw-   0        0        0     1628 2023-05-04 01:29:27.000000 ipfs_dict_chain-1.0.3/tests/test_IPFSDictChain.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:47:53.275295 ipfs_dict_chain-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-21 21:22:08.000000 ipfs_dict_chain-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-04 01:15:25.000000 ipfs_dict_chain-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      575 2023-05-04 01:47:53.275295 ipfs_dict_chain-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2411 2023-05-04 01:47:08.000000 ipfs_dict_chain-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 01:47:53.256064 ipfs_dict_chain-1.0.4/ipfs_dict_chain/
+-rw-rw-rw-   0        0        0     1774 2023-05-03 22:46:27.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain/CID.py
+-rw-rw-rw-   0        0        0     4416 2023-05-03 23:13:55.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFS.py
+-rw-rw-rw-   0        0        0     2336 2023-05-04 01:41:06.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFSDict.py
+-rw-rw-rw-   0        0        0     3474 2023-05-04 01:41:06.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFSDictChain.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 01:46:08.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:47:53.265064 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-05-04 01:47:53.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-04 01:47:53.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:47:53.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-04 01:47:53.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 01:47:53.000000 ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:47:53.276278 ipfs_dict_chain-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      767 2023-05-04 01:47:19.000000 ipfs_dict_chain-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:47:53.273299 ipfs_dict_chain-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 22:39:34.000000 ipfs_dict_chain-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-05-04 01:27:56.000000 ipfs_dict_chain-1.0.4/tests/test_CID.py
+-rw-rw-rw-   0        0        0     1129 2023-05-04 01:29:17.000000 ipfs_dict_chain-1.0.4/tests/test_IPFS.py
+-rw-rw-rw-   0        0        0     1485 2023-05-04 01:44:49.000000 ipfs_dict_chain-1.0.4/tests/test_IPFSDict.py
+-rw-rw-rw-   0        0        0     1644 2023-05-04 01:45:04.000000 ipfs_dict_chain-1.0.4/tests/test_IPFSDictChain.py
```

### Comparing `ipfs_dict_chain-1.0.3/LICENSE` & `ipfs_dict_chain-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.3/PKG-INFO` & `ipfs_dict_chain-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfs_dict_chain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.
 Home-page: https://github.com/ValyrianTech/ipfs_dict_chain
 Author: Wouter Glorieux
 Author-email: info@valyrian.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfs_dict_chain-1.0.3/README.md` & `ipfs_dict_chain-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 ```
 
 ## Usage
 
 If your IPFS node is not running on localhost on the default port, you must first connect to your IPFS node:
 
 ```python
-from ipfs_dict_chain import connect
+from ipfs_dict_chain.IPFS import connect
 
 connect(host='ipfs.example.com', port=5001)
 ```
 
 ### IPFSDict
 
 IPFSDict is a dictionary-like object that stores its data on IPFS. Here's an example of how to use IPFSDict:
 
 ```python
-from ipfs_dict_chain import IPFSDict
+from ipfs_dict_chain.IPFSDict import IPFSDict
 
 my_dict = IPFSDict()
 
 # Add data to the dictionary
 my_dict['key'] = 'value'
 
 # Save the dictionary to IPFS
@@ -48,15 +48,15 @@
 ```
 
 ### IPFSDictChain
 
 IPFSDictChain is a dictionary-like data structure that stores its state on IPFS and keeps track of changes. Here's an example of how to use IPFSDictChain:
 
 ```python
-from ipfs_dict_chain import IPFSDictChain
+from ipfs_dict_chain.IPFSDictChain import IPFSDictChain
 
 my_chain = IPFSDictChain()
 
 # Add data to the dictionary
 my_chain['key'] = 'value'
 
 # Save the current state of the dictionary to IPFS
```

### Comparing `ipfs_dict_chain-1.0.3/ipfs_dict_chain/CID.py` & `ipfs_dict_chain-1.0.4/ipfs_dict_chain/CID.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFS.py` & `ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFS.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFSDict.py` & `ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFSDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict, Any, List, Tuple
 
-from IPFS import IPFSError, add_json, get_json
-from CID import CID
+from .IPFS import IPFSError, add_json, get_json
+from .CID import CID
 
 
 class IPFSDict(Dict):
     """A dictionary-like object that stores its data on IPFS.
 
     :param cid: The IPFS content identifier (CID) of the dictionary data, defaults to None
     :type cid: Optional[str], optional
```

### Comparing `ipfs_dict_chain-1.0.3/ipfs_dict_chain/IPFSDictChain.py` & `ipfs_dict_chain-1.0.4/ipfs_dict_chain/IPFSDictChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict, Any, List
 
-from IPFS import add_json
-from IPFSDict import IPFSDict
+from .IPFS import add_json
+from .IPFSDict import IPFSDict
 
 
 class IPFSDictChain(IPFSDict):
     """A dictionary-like data structure that stores its state on IPFS and keeps track of changes.
 
     :param cid: The IPFS CID to initialize the dictionary with, defaults to None
     :type cid: Optional[str], optional
```

### Comparing `ipfs_dict_chain-1.0.3/ipfs_dict_chain.egg-info/PKG-INFO` & `ipfs_dict_chain-1.0.4/ipfs_dict_chain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfs-dict-chain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.
 Home-page: https://github.com/ValyrianTech/ipfs_dict_chain
 Author: Wouter Glorieux
 Author-email: info@valyrian.tech
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfs_dict_chain-1.0.3/setup.py` & `ipfs_dict_chain-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipfs_dict_chain',
-    version='1.0.3',
+    version='1.0.4',
     description='A Python package that provides IPFSDict and IPFSDictChain objects, which are dictionary-like data structures that store their state on IPFS and keep track of changes.',
     author='Wouter Glorieux',
     author_email='info@valyrian.tech',
     url='https://github.com/ValyrianTech/ipfs_dict_chain',
     packages=['ipfs_dict_chain'],
     install_requires=[
         'aioipfs>=0.6.3',
```

### Comparing `ipfs_dict_chain-1.0.3/tests/test_CID.py` & `ipfs_dict_chain-1.0.4/tests/test_CID.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.3/tests/test_IPFS.py` & `ipfs_dict_chain-1.0.4/tests/test_IPFS.py`

 * *Files identical despite different names*

### Comparing `ipfs_dict_chain-1.0.3/tests/test_IPFSDict.py` & `ipfs_dict_chain-1.0.4/tests/test_IPFSDict.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
-from IPFSDict import IPFSDict
-from IPFS import IPFSError
+from ipfs_dict_chain.IPFSDict import IPFSDict
+from ipfs_dict_chain.IPFS import IPFSError
 
 
 class TestIPFSDict(unittest.TestCase):
 
     def test_init(self):
         ipfs_dict = IPFSDict()
         self.assertIsNone(ipfs_dict.cid())
```

### Comparing `ipfs_dict_chain-1.0.3/tests/test_IPFSDictChain.py` & `ipfs_dict_chain-1.0.4/tests/test_IPFSDictChain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from IPFSDictChain import IPFSDictChain
+from ipfs_dict_chain.IPFSDictChain import IPFSDictChain
 
 
 class TestIPFSDictChain(unittest.TestCase):
 
     def test_init(self):
         ipfs_dict_chain = IPFSDictChain()
         self.assertIsNotNone(ipfs_dict_chain)
```

