# Comparing `tmp/np-session-0.6.0.tar.gz` & `tmp/np-session-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.6.0.tar", last modified: Tue May  2 22:27:47 2023, max compression
+gzip compressed data, was "np-session-0.6.1.tar", last modified: Wed May  3 22:18:19 2023, max compression
```

## Comparing `np-session-0.6.0.tar` & `np-session-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     2264 2023-05-02 22:27:34.652197 np-session-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.0/README.md
--rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.0/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.0/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.0/src/np_session/components/info.py
--rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.0/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.0/src/np_session/components/mixins.py
--rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.0/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.0/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.0/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.0/src/np_session/components/state.py
--rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.0/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.0/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.0/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.0/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.0/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.0/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.0/src/np_session/exceptions.py
--rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.0/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.0/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.0/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.0/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0     8531 2023-05-02 22:25:42.888002 np-session-0.6.0/src/np_session/session.py
--rw-r--r--   0        0        0      181 2023-05-02 22:19:28.306490 np-session-0.6.0/src/np_session/subclasses/__init__.py
--rw-r--r--   0        0        0     4586 2023-05-02 22:17:18.896118 np-session-0.6.0/src/np_session/subclasses/dynamic_routing_pilot.py
--rw-r--r--   0        0        0    20527 2023-05-02 22:17:19.652824 np-session-0.6.0/src/np_session/subclasses/pipeline.py
--rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.0/src/np_session/tasks.py
--rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.0/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.0/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.0/tests/test_platform_json.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2289 2023-05-03 22:18:14.117745 np-session-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.1/README.md
+-rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.1/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.1/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.1/src/np_session/components/info.py
+-rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.1/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.1/src/np_session/components/mixins.py
+-rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.1/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.1/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.1/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.1/src/np_session/components/state.py
+-rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.1/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.1/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.1/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.1/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.1/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.1/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.1/src/np_session/exceptions.py
+-rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.1/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.1/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.1/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.1/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0     8774 2023-05-03 22:12:17.230094 np-session-0.6.1/src/np_session/session.py
+-rw-r--r--   0        0        0      181 2023-05-02 22:19:28.306490 np-session-0.6.1/src/np_session/subclasses/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-03 21:57:37.747421 np-session-0.6.1/src/np_session/subclasses/dynamic_routing_pilot.py
+-rw-r--r--   0        0        0    21636 2023-05-03 21:32:03.275128 np-session-0.6.1/src/np_session/subclasses/pipeline.py
+-rw-r--r--   0        0        0     5413 2023-05-03 22:03:47.191978 np-session-0.6.1/src/np_session/subclasses/templeton_pilot.py
+-rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.1/src/np_session/tasks.py
+-rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.1/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.1/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.1/tests/test_platform_json.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.1/PKG-INFO
```

### Comparing `np-session-0.6.0/pyproject.toml` & `np-session-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.6.0"
+version = "0.6.1"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -40,18 +40,18 @@
     "pdm>=2.4.9",
     "bump>=1.3.2",
     "types-backports>=0.1.3",
     "ruff>=0.0.260",
 ]
 
 [tool.pdm.scripts]
-ruff = "ruff --fix src"
+ruff = "ruff check src --fix-only"
 blue = "blue src"
 pytest = "pytest --cov"
-bump = "pdm bump patch"
+bump = "bump -p pyproject.toml"
 
 [tool.pdm.scripts.prebuild]
 composite = [
     "blue",
     "ruff",
     "pytest",
 ]
@@ -65,26 +65,27 @@
 [tool.pdm.scripts.dry-run]
 composite = [
     "prebuild",
     "pdm build",
     "pdm publish --no-build --repository https://test.pypi.org/simple",
 ]
 
-[tool.pdm.scripts.pub]
-composite = [
-    "pdm bump patch",
-    "pdm publish",
-]
-
 [tool.pdm.scripts.publish]
 composite = [
+    "prebuild",
     "pdm build",
     "pdm publish --no-build",
 ]
 
+[tool.pdm.scripts.pub]
+composite = [
+    "bump",
+    "pdm publish",
+]
+
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--doctest-modules",
 ]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
```

### Comparing `np-session-0.6.0/README.md` & `np-session-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/info.py` & `np-session-0.6.1/src/np_session/components/info.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/lims_manifests.py` & `np-session-0.6.1/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/mixins.py` & `np-session-0.6.1/src/np_session/components/mixins.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/paths.py` & `np-session-0.6.1/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/platform_json.py` & `np-session-0.6.1/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/settings_xml.py` & `np-session-0.6.1/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/components/state.py` & `np-session-0.6.1/src/np_session/components/state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/databases/data_getters.py` & `np-session-0.6.1/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/databases/firebase_state.py` & `np-session-0.6.1/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/databases/lims2.py` & `np-session-0.6.1/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/databases/mtrain.py` & `np-session-0.6.1/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/databases/redis_state.py` & `np-session-0.6.1/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/jobs/lims_upload.py` & `np-session-0.6.1/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/jobs/sessions.json` & `np-session-0.6.1/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/jobs/sync_states.py` & `np-session-0.6.1/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/session.py` & `np-session-0.6.1/src/np_session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import abc
 import contextlib
 import datetime
 import doctest
 import os
 import pathlib
 from typing import Any, Iterable, Optional, Type, TypeVar, Union
 
@@ -78,15 +77,16 @@
     'NeuropixelVisualBehavior'
     >>> str(session.rig)        # see np_config.Rig
     'NP.0'
     """
 
     def __init__(self, path_or_session: PathLike | int | LIMS2SessionInfo):
         try:
-            self.folder = self.get_folder(path_or_session)
+            # assign directly and folder setter will validate for us
+            self.folder = str(path_or_session)
         except ValueError as exc:
             raise SessionError(
                 f'{path_or_session} does not contain a valid {self.__class__.__name__} session id or session folder string'
             ) from exc
 
         if isinstance(path_or_session, LIMS2SessionInfo):
             self.lims = path_or_session
@@ -166,18 +166,23 @@
     user: Optional[str | User] = None
     """Operator for the session"""
     lims: Optional[dict | LIMS2SessionInfo] = None
     mtrain: Optional[mtrain.MTrain] = None
     foraging_id: Optional[str] = None
 
     @staticmethod
-    @abc.abstractmethod
     def get_folder(path: str | int | PathLike) -> str:
         """Extract the session folder from a path or session ID"""
-
+        return NotImplemented
+    
+    @classmethod
+    def new(cls, *args, **kwargs) -> Self:
+        """Generate a new session (should create a folder and assign to npexp path)"""
+        return NotImplemented
+    
     @property
     def date(self) -> datetime.date:
         d = self.folder.split('_')[2]
         date = datetime.date(
             year=int(d[:4]), month=int(d[4:6]), day=int(d[6:])
         )
         return date
```

### Comparing `np-session-0.6.0/src/np_session/subclasses/dynamic_routing_pilot.py` & `np-session-0.6.1/src/np_session/subclasses/dynamic_routing_pilot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import datetime
 import doctest
 import pathlib
 import warnings
 
 import np_config
 import np_logging
+from typing_extensions import Self
 
+from np_session.components.info import Project, User, Mouse
 from np_session.components.paths import *
 from np_session.components.platform_json import *
 from np_session.utils import *
 from np_session.session import Session
 
 logger = np_logging.getLogger(__name__)
 
@@ -113,14 +115,23 @@
         """
         # from filesystem
         session_reg_exp = R'DRpilot_[0-9]{6}_[0-9]{8}'
         session_folders = re.findall(session_reg_exp, str(path), re.IGNORECASE)
         if session_folders:
             return session_folders[0]
 
+    @classmethod
+    def new(
+        cls,
+        mouse_labtracks_id: int | str | Mouse,
+    ) -> Self:
+        """Create a new session folder for a mouse."""
+        path = cls.storage_dirs[0] / f'DRpilot_{mouse_labtracks_id}_{datetime.date.today().strftime("%Y%m%d")}'
+        return cls(path)
+    
     @property
     def npexp_path(self) -> pathlib.Path:
         with contextlib.suppress(AttributeError):
             return self._npexp_path
         for _ in self.storage_dirs:
             path = _ / self.folder
             if path.exists():
```

### Comparing `np-session-0.6.0/src/np_session/subclasses/pipeline.py` & `np-session-0.6.1/src/np_session/subclasses/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import doctest
 import pathlib
 from typing import Iterable, Optional
 
 import np_config
 import np_logging
 from backports.cached_property import cached_property
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
-from np_session.components.info import Project, User
+from np_session.components.info import Project, User, Mouse
 from np_session.components.lims_manifests import Manifest
 from np_session.components.paths import *
 from np_session.components.platform_json import *
 from np_session.databases import data_getters as dg
 from np_session.databases import lims2 as lims
 from np_session.databases import mtrain
 from np_session.utils import *
@@ -75,14 +75,45 @@
     'NP.0'
     """
 
     @staticmethod
     def get_folder(value: int | str | PathLike) -> str | None:
         return get_lims_session_folder(value)
 
+    @classmethod
+    def new(
+        cls,
+        mouse: str | int | Mouse,
+        user: str | User,
+        session_type: Literal['ephys', 'hab', 'behavior'] = 'ephys',
+    ) -> Self:
+        """Create a new session in LIMS and return a Session instance."""
+        if not isinstance(mouse, Mouse):
+            mouse = Mouse(mouse)
+        if not isinstance(user, User):
+            user = User(user)
+        if (
+            'ephys' in session_type
+        ):   # maintain backwards compatibility with 'ecephys'
+            lims_session = lims.generate_ephys_session(
+                mouse=mouse.lims, user=user.lims
+            )
+        elif session_type == 'hab':
+            lims_session = lims.generate_hab_session(
+                mouse=mouse.lims, user=user.lims
+            )
+        elif session_type == 'behavior':
+            raise ValueError('Generating behavior sessions is not yet supported')
+        session = cls(lims_session)
+        # assign instances with data already fetched from lims:
+        session._mouse = mouse
+        session._user = user
+        return session
+
+
     @property
     def folder(self) -> str:
         """Folder name, e.g. `[lims session ID]_[labtracks ID]_[8-digit date]`."""
         return self._folder
 
     @folder.setter
     def folder(self, value: str | PathLike) -> None:
```

### Comparing `np-session-0.6.0/src/np_session/tasks.py` & `np-session-0.6.1/src/np_session/tasks.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/src/np_session/utils.py` & `np-session-0.6.1/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/tests/test_np_session.py` & `np-session-0.6.1/tests/test_np_session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/tests/test_platform_json.py` & `np-session-0.6.1/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.0/PKG-INFO` & `np-session-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.6.0
+Version: 0.6.1
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

