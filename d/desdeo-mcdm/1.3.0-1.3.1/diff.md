# Comparing `tmp/desdeo_mcdm-1.3.0.tar.gz` & `tmp/desdeo_mcdm-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desdeo_mcdm-1.3.0.tar", max compression
+gzip compressed data, was "desdeo_mcdm-1.3.1.tar", max compression
```

## Comparing `desdeo_mcdm-1.3.0.tar` & `desdeo_mcdm-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1098 2022-03-03 13:18:34.104959 desdeo_mcdm-1.3.0/LICENSE
--rw-r--r--   0        0        0      122 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/.readthedocs.yml
--rw-r--r--   0        0        0        0 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/__init__.py
--rw-r--r--   0        0        0    10355 2023-03-02 09:48:02.069442 desdeo_mcdm-1.3.0/desdeo_mcdm/approximation/PAINT.py
--rw-r--r--   0        0        0      202 2023-03-02 09:48:02.069442 desdeo_mcdm-1.3.0/desdeo_mcdm/approximation/__init__.py
--rw-r--r--   0        0        0    18937 2022-03-07 08:39:54.176413 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ENautilus.py
--rw-r--r--   0        0        0      295 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/InteractiveMethod.py
--rw-r--r--   0        0        0    50336 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NIMBUS.py
--rw-r--r--   0        0        0    45226 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/Nautilus.py
--rw-r--r--   0        0        0    26941 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NautilusNavigator.py
--rw-r--r--   0        0        0    49481 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NautilusV2.py
--rw-r--r--   0        0        0    34179 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ParetoNavigator.py
--rw-r--r--   0        0        0    27829 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ReferencePointMethod.py
--rw-r--r--   0        0        0     2506 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/__init__.py
--rw-r--r--   0        0        0      497 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/utilities/__init__.py
--rw-r--r--   0        0        0    15312 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.0/desdeo_mcdm/utilities/solvers.py
--rw-r--r--   0        0        0     1002 2023-03-02 09:51:23.339767 desdeo_mcdm-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 desdeo_mcdm-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2022-03-03 13:18:34.104959 desdeo_mcdm-1.3.1/LICENSE
+-rw-r--r--   0        0        0      122 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/.readthedocs.yml
+-rw-r--r--   0        0        0        0 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/__init__.py
+-rw-r--r--   0        0        0    10355 2023-03-02 09:48:02.069442 desdeo_mcdm-1.3.1/desdeo_mcdm/approximation/PAINT.py
+-rw-r--r--   0        0        0      202 2023-03-02 09:48:02.069442 desdeo_mcdm-1.3.1/desdeo_mcdm/approximation/__init__.py
+-rw-r--r--   0        0        0    18973 2023-05-04 10:43:15.164175 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ENautilus.py
+-rw-r--r--   0        0        0      295 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/InteractiveMethod.py
+-rw-r--r--   0        0        0    50480 2023-05-04 10:48:33.659234 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NIMBUS.py
+-rw-r--r--   0        0        0    45262 2023-05-04 10:44:37.817988 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/Nautilus.py
+-rw-r--r--   0        0        0    26941 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NautilusNavigator.py
+-rw-r--r--   0        0        0    49517 2023-05-04 10:46:08.628488 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NautilusV2.py
+-rw-r--r--   0        0        0    34233 2023-05-04 10:49:58.496314 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ParetoNavigator.py
+-rw-r--r--   0        0        0    27865 2023-05-04 10:50:39.799844 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ReferencePointMethod.py
+-rw-r--r--   0        0        0     2506 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/__init__.py
+-rw-r--r--   0        0        0      497 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/utilities/__init__.py
+-rw-r--r--   0        0        0    15312 2022-03-03 13:18:34.111626 desdeo_mcdm-1.3.1/desdeo_mcdm/utilities/solvers.py
+-rw-r--r--   0        0        0     1002 2023-05-04 10:51:58.850211 desdeo_mcdm-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 desdeo_mcdm-1.3.1/PKG-INFO
```

### Comparing `desdeo_mcdm-1.3.0/LICENSE` & `desdeo_mcdm-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/approximation/PAINT.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/approximation/PAINT.py`

 * *Files identical despite different names*

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ENautilus.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ENautilus.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,17 +250,17 @@
 
     def iterate(
         self, request: Union[ENautilusInitialRequest, ENautilusRequest]
     ) -> Union[ENautilusRequest, ENautilusStopRequest]:
         """Perform the next logical iteration step based on the given request type.
 
         """
-        if type(request) is ENautilusInitialRequest:
+        if type(request).__name__ == ENautilusInitialRequest.__name__:
             return self.handle_initial_request(request)
-        elif type(request) is ENautilusRequest:
+        elif type(request).__name__ == ENautilusRequest.__name__:
             return self.handle_request(request)
         else:
             # if stop request, do nothing
             return request
 
     def handle_initial_request(
         self, request: ENautilusInitialRequest
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NIMBUS.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NIMBUS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1000,56 +1000,56 @@
             NimbusException: If a wrong type of request is supplied based on the current state NIMBUS is in.
         
         Returns:
             Tuple[Union[NimbusClassificationRequest,NimbusSaveRequest,NimbusIntermediateSolutionsRequest,],Union[SimplePlotRequest, None],]:
             The next logically sound request.
         """
         if self._state == "classify":
-            if type(request) != NimbusClassificationRequest:
+            if type(request).__name__ != NimbusClassificationRequest.__name__:
                 raise NimbusException(
                     f"Expected request type {type(NimbusClassificationRequest)}, was {type(request)}."
                 )
 
             requests = self.handle_classification_request(request)
             self._state = "archive"
             return requests
 
         elif self._state == "archive":
-            if type(request) != NimbusSaveRequest:
+            if type(request).__name__ != NimbusSaveRequest.__name__:
                 raise NimbusException(f"Expected request type {type(NimbusSaveRequest)}, was {type(request)}.")
 
             requests = self.handle_save_request(request)
             self._state = "intermediate"
             return requests
 
         elif self._state == "intermediate":
-            if type(request) != NimbusIntermediateSolutionsRequest:
+            if type(request).__name__ != NimbusIntermediateSolutionsRequest.__name__:
                 raise NimbusException(
                     f"Expected request type {type(NimbusIntermediateSolutionsRequest)}, was {type(request)}."
                 )
 
             requests = self.handle_intermediate_solutions_request(request)
 
-            if type(requests[0]) == NimbusSaveRequest:
+            if type(requests[0]).__name__ == NimbusSaveRequest.__name__:
                 self._state = "archive"
-            elif type(requests[0]) == NimbusMostPreferredRequest:
+            elif type(requests[0]).__name__ == NimbusMostPreferredRequest.__name__:
                 self._state = "preferred"
 
             return requests
 
         elif self._state == "preferred":
-            if type(request) != NimbusMostPreferredRequest:
+            if type(request).__name__ != NimbusMostPreferredRequest.__name__:
                 raise NimbusException(f"Expected request type {type(NimbusMostPreferredRequest)}, was {type(request)}.")
 
             requests = self.handle_most_preferred_request(request)
 
-            if type(requests[0]) == NimbusStopRequest:
+            if type(requests[0]).__name__ == NimbusStopRequest.__name__:
                 self._state = "end"
 
-            elif type(requests[0]) == NimbusClassificationRequest:
+            elif type(requests[0]).__name__ == NimbusClassificationRequest.__name__:
                 self._state = "classify"
 
             return requests
 
         elif self._state == "end":
             # end
             return request, None
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/Nautilus.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/Nautilus.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,17 +440,17 @@
 
         Returns:
             Union[NautilusRequest, NautilusStopRequest]: A new request with content depending on the Decision maker's
             preferences.
 
         """
 
-        if type(request) is NautilusInitialRequest:
+        if type(request).__name__ == NautilusInitialRequest.__name__:
             return self.handle_initial_request(request)
-        elif type(request) is NautilusRequest:
+        elif type(request).__name__ == NautilusRequest.__name__:
             return self.handle_request(request)
         else:
             # if stop request, do nothing
             return request
 
     def handle_initial_request(self, request: NautilusInitialRequest) -> NautilusRequest:
         """
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NautilusNavigator.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NautilusNavigator.py`

 * *Files identical despite different names*

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/NautilusV2.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/NautilusV2.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,17 +500,17 @@
 
         Returns:
             Union[NautilusRequest, NautilusStopRequest]: A new request with content depending on the Decision maker's
                 preferences.
 
         """
 
-        if type(request) is NautilusInitialRequest:
+        if type(request).__name__ == NautilusInitialRequest.__name__:
             return self.handle_initial_request(request)
-        elif type(request) is NautilusRequest:
+        elif type(request).__name__ == NautilusRequest.__name__:
             return self.handle_request(request)
         else:
             # if stop request, do nothing
             return request
 
     def handle_initial_request(self, request: NautilusInitialRequest) -> NautilusRequest:
         """
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ParetoNavigator.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ParetoNavigator.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,19 +411,19 @@
                 A ParetoNavigatorRequest
 
         Returns:
             Union[ParetoNavigatorRequest, ParetoNavigatorSolutionRequest, ParetoNavigatorStopRequest]:
                 A new request with content depending on the Decision Maker's preferences.
         """
 
-        if type(request) is ParetoNavigatorInitialRequest:
+        if type(request).__name__ == ParetoNavigatorInitialRequest.__name__:
             return self.handle_initial_request(request)
-        elif type(request) is ParetoNavigatorRequest:
+        elif type(request).__name__ is ParetoNavigatorRequest.__name__:
             return self.handle_request(request)
-        elif type(request) is ParetoNavigatorSolutionRequest:
+        elif type(request).__name__ is ParetoNavigatorSolutionRequest.__name__:
             return self.handle_solution_request(request)
         else:
             # if stop request, do nothing
             return request
 
     def handle_initial_request(
         self, request: ParetoNavigatorInitialRequest
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/ReferencePointMethod.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/ReferencePointMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,17 +333,17 @@
             request (Union[RPMInitialRequest, RPMRequest]): Either initial or intermediate request.
 
         Returns:
             Union[RPMRequest, RPMStopRequest]: A new request with content depending on the Decision Maker's
             preferences.
         """
 
-        if type(request) is RPMInitialRequest:
+        if type(request).__name__ == RPMInitialRequest.__name__:
             return self.handle_initial_request(request)
-        elif type(request) is RPMRequest:
+        elif type(request).__name__ is RPMRequest.__name__:
             return self.handle_request(request)
         else:
             # if stop request, do nothing
             return request
 
     def handle_initial_request(self, request: RPMInitialRequest) -> RPMRequest:
         """
```

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/interactive/__init__.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `desdeo_mcdm-1.3.0/desdeo_mcdm/utilities/solvers.py` & `desdeo_mcdm-1.3.1/desdeo_mcdm/utilities/solvers.py`

 * *Files identical despite different names*

### Comparing `desdeo_mcdm-1.3.0/pyproject.toml` & `desdeo_mcdm-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "desdeo-mcdm"
-version = "1.3.0"
+version = "1.3.1"
 description = "Contains traditional optimization techniques from the field of Multiple-criteria decision-making. Methods belonging to the NIMBUS and NAUTILUS families can be found here. Part of the DESDEO framework."
 authors = ["Giovanni Misitano", "Antti Luopajärvi"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 desdeo-tools = ">=1.8"
@@ -14,15 +14,15 @@
 pytest = ">=6.2.5"
 black = "^19.10b0"
 flake8 = "^3.7.9"
 pylint = "^2.4.4"
 rope = "^0.16.0"
 sphinx = "^6.1.0"
 rstcheck = "^3.3.1"
-sphinx_rtd_theme = "^0.4.3"
+sphinx_rtd_theme = "^1.2.0"
 sphinx_autodoc_typehints = "^1.10.3"
 sphinx-automodapi = "^0.12"
 recommonmark = "^0.6.0"
 nbsphinx = "^0.8.11"
 IPython = "^7.15.0"
 ipykernel = "^5.3.0"
 # jupyter = "^1.0.0"
```

### Comparing `desdeo_mcdm-1.3.0/PKG-INFO` & `desdeo_mcdm-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desdeo-mcdm
-Version: 1.3.0
+Version: 1.3.1
 Summary: Contains traditional optimization techniques from the field of Multiple-criteria decision-making. Methods belonging to the NIMBUS and NAUTILUS families can be found here. Part of the DESDEO framework.
 License: MIT
 Author: Giovanni Misitano
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

