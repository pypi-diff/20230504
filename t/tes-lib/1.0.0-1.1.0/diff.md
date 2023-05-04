# Comparing `tmp/tes-lib-1.0.0.tar.gz` & `tmp/tes-lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tes-lib-1.0.0.tar", last modified: Mon Mar 27 09:18:15 2023, max compression
+gzip compressed data, was "tes-lib-1.1.0.tar", last modified: Thu May  4 10:44:16 2023, max compression
```

## Comparing `tes-lib-1.0.0.tar` & `tes-lib-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-03-27 09:18:15.151299 tes-lib-1.0.0/
--rw-r--r--   0 laurence   (501) staff       (20)     1074 2022-07-24 15:19:12.000000 tes-lib-1.0.0/LICENSE
--rw-r--r--   0 laurence   (501) staff       (20)     1199 2023-03-27 09:18:15.150800 tes-lib-1.0.0/PKG-INFO
--rw-r--r--   0 laurence   (501) staff       (20)      732 2022-07-26 18:38:19.000000 tes-lib-1.0.0/README.md
--rw-r--r--   0 laurence   (501) staff       (20)       38 2023-03-27 09:18:15.151563 tes-lib-1.0.0/setup.cfg
--rw-r--r--   0 laurence   (501) staff       (20)      757 2023-03-27 09:17:32.000000 tes-lib-1.0.0/setup.py
-drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-03-27 09:18:15.144822 tes-lib-1.0.0/tes_lib/
--rw-r--r--   0 laurence   (501) staff       (20)     4737 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/__init__.py
--rw-r--r--   0 laurence   (501) staff       (20)     3548 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/add_event_web_server.py
--rw-r--r--   0 laurence   (501) staff       (20)      522 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/constants.py
--rw-r--r--   0 laurence   (501) staff       (20)     2648 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/defaults.py
--rw-r--r--   0 laurence   (501) staff       (20)     4669 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/errors.py
--rw-r--r--   0 laurence   (501) staff       (20)    23268 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/event_helpers.py
--rw-r--r--   0 laurence   (501) staff       (20)     1871 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/expectation.py
--rw-r--r--   0 laurence   (501) staff       (20)      217 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/formatting.py
--rw-r--r--   0 laurence   (501) staff       (20)     6102 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/library_settings.py
--rw-r--r--   0 laurence   (501) staff       (20)     2138 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/messages.py
--rw-r--r--   0 laurence   (501) staff       (20)      881 2022-07-24 15:19:12.000000 tes-lib-1.0.0/tes_lib/test_event.py
--rw-r--r--   0 laurence   (501) staff       (20)    11456 2023-03-27 09:17:32.000000 tes-lib-1.0.0/tes_lib/test_event_store.py
-drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-03-27 09:18:15.149700 tes-lib-1.0.0/tes_lib.egg-info/
--rw-r--r--   0 laurence   (501) staff       (20)     1199 2023-03-27 09:18:15.000000 tes-lib-1.0.0/tes_lib.egg-info/PKG-INFO
--rw-r--r--   0 laurence   (501) staff       (20)      459 2023-03-27 09:18:15.000000 tes-lib-1.0.0/tes_lib.egg-info/SOURCES.txt
--rw-r--r--   0 laurence   (501) staff       (20)        1 2023-03-27 09:18:15.000000 tes-lib-1.0.0/tes_lib.egg-info/dependency_links.txt
--rw-r--r--   0 laurence   (501) staff       (20)        9 2023-03-27 09:18:15.000000 tes-lib-1.0.0/tes_lib.egg-info/requires.txt
--rw-r--r--   0 laurence   (501) staff       (20)        8 2023-03-27 09:18:15.000000 tes-lib-1.0.0/tes_lib.egg-info/top_level.txt
+drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-05-04 10:44:16.868472 tes-lib-1.1.0/
+-rw-r--r--   0 laurence   (501) staff       (20)     1074 2022-07-24 15:19:12.000000 tes-lib-1.1.0/LICENSE
+-rw-r--r--   0 laurence   (501) staff       (20)     1199 2023-05-04 10:44:16.868154 tes-lib-1.1.0/PKG-INFO
+-rw-r--r--   0 laurence   (501) staff       (20)      732 2022-07-26 18:38:19.000000 tes-lib-1.1.0/README.md
+-rw-r--r--   0 laurence   (501) staff       (20)       38 2023-05-04 10:44:16.868659 tes-lib-1.1.0/setup.cfg
+-rw-r--r--   0 laurence   (501) staff       (20)      757 2023-05-04 10:35:38.000000 tes-lib-1.1.0/setup.py
+drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-05-04 10:44:16.866047 tes-lib-1.1.0/tes_lib/
+-rw-r--r--   0 laurence   (501) staff       (20)     4737 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/__init__.py
+-rw-r--r--   0 laurence   (501) staff       (20)     3548 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/add_event_web_server.py
+-rw-r--r--   0 laurence   (501) staff       (20)      522 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/constants.py
+-rw-r--r--   0 laurence   (501) staff       (20)     2648 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/defaults.py
+-rw-r--r--   0 laurence   (501) staff       (20)     4669 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/errors.py
+-rw-r--r--   0 laurence   (501) staff       (20)    23268 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/event_helpers.py
+-rw-r--r--   0 laurence   (501) staff       (20)     1871 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/expectation.py
+-rw-r--r--   0 laurence   (501) staff       (20)      217 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/formatting.py
+-rw-r--r--   0 laurence   (501) staff       (20)     6102 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/library_settings.py
+-rw-r--r--   0 laurence   (501) staff       (20)     2138 2023-03-27 09:17:32.000000 tes-lib-1.1.0/tes_lib/messages.py
+-rw-r--r--   0 laurence   (501) staff       (20)     1939 2023-05-04 10:35:38.000000 tes-lib-1.1.0/tes_lib/test_event.py
+-rw-r--r--   0 laurence   (501) staff       (20)    11463 2023-05-04 10:35:38.000000 tes-lib-1.1.0/tes_lib/test_event_store.py
+drwxr-xr-x   0 laurence   (501) staff       (20)        0 2023-05-04 10:44:16.867751 tes-lib-1.1.0/tes_lib.egg-info/
+-rw-r--r--   0 laurence   (501) staff       (20)     1199 2023-05-04 10:44:16.000000 tes-lib-1.1.0/tes_lib.egg-info/PKG-INFO
+-rw-r--r--   0 laurence   (501) staff       (20)      459 2023-05-04 10:44:16.000000 tes-lib-1.1.0/tes_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 laurence   (501) staff       (20)        1 2023-05-04 10:44:16.000000 tes-lib-1.1.0/tes_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 laurence   (501) staff       (20)        9 2023-05-04 10:44:16.000000 tes-lib-1.1.0/tes_lib.egg-info/requires.txt
+-rw-r--r--   0 laurence   (501) staff       (20)        8 2023-05-04 10:44:16.000000 tes-lib-1.1.0/tes_lib.egg-info/top_level.txt
```

### Comparing `tes-lib-1.0.0/LICENSE` & `tes-lib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/PKG-INFO` & `tes-lib-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tes-lib
-Version: 1.0.0
+Version: 1.1.0
 Summary: Test Event Store LIBrary (tes-lib)
 Home-page: https://gitlab.com/LCaraccio/tes-lib
 Author: Laurence Caraccio
 Author-email: laurencecaraccio@hotmail.co.uk
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tes-lib-1.0.0/README.md` & `tes-lib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/setup.py` & `tes-lib-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setuptools.setup(
     name="tes-lib",
-    version="1.0.0",
+    version="1.1.0",
     author="Laurence Caraccio",
     author_email="laurencecaraccio@hotmail.co.uk",
     description="Test Event Store LIBrary (tes-lib)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/LCaraccio/tes-lib",
     packages=setuptools.find_packages(),
```

### Comparing `tes-lib-1.0.0/tes_lib/__init__.py` & `tes-lib-1.1.0/tes_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/add_event_web_server.py` & `tes-lib-1.1.0/tes_lib/add_event_web_server.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/constants.py` & `tes-lib-1.1.0/tes_lib/constants.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/defaults.py` & `tes-lib-1.1.0/tes_lib/defaults.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/errors.py` & `tes-lib-1.1.0/tes_lib/errors.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/event_helpers.py` & `tes-lib-1.1.0/tes_lib/event_helpers.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/expectation.py` & `tes-lib-1.1.0/tes_lib/expectation.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/library_settings.py` & `tes-lib-1.1.0/tes_lib/library_settings.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/messages.py` & `tes-lib-1.1.0/tes_lib/messages.py`

 * *Files identical despite different names*

### Comparing `tes-lib-1.0.0/tes_lib/test_event_store.py` & `tes-lib-1.1.0/tes_lib/test_event_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The test event store and run loop
 """
 import copy
 import multiprocessing
 from multiprocessing import connection
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Tuple
 import logging
 import traceback
 
 from .expectation import Expectation, FailedExpectation, ExpectationFailureType, PartialMatch
 from .constants import (
     NO_MATCHING_EVENT_FOUND,
     EVENT_ID_KEY,
@@ -194,15 +194,15 @@
 
         return NO_MATCHING_EVENT_FOUND
 
     def extended_expect_event(
         self,
         expectations: List[Expectation],
         partial_filter_field_expectations: List[Expectation],
-    ) -> tuple[Union[str, Dict], List[PartialMatch]]:
+    ) -> Tuple[Union[str, Dict], List[PartialMatch]]:
         """Find an event matching the expectations, if no event is found, details of events that
         partially match and the expectations that failed will be returned.
 
         :param expectations: A list of expectations
         :param partial_filter_fields: Which fields should be used to perform the partial
           filtering if any
         :return: A tuple of the matching event or an error message as well as a list of events
```

### Comparing `tes-lib-1.0.0/tes_lib.egg-info/PKG-INFO` & `tes-lib-1.1.0/tes_lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tes-lib
-Version: 1.0.0
+Version: 1.1.0
 Summary: Test Event Store LIBrary (tes-lib)
 Home-page: https://gitlab.com/LCaraccio/tes-lib
 Author: Laurence Caraccio
 Author-email: laurencecaraccio@hotmail.co.uk
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

