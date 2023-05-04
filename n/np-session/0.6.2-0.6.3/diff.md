# Comparing `tmp/np-session-0.6.2.tar.gz` & `tmp/np-session-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.6.2.tar", last modified: Thu May  4 00:08:35 2023, max compression
+gzip compressed data, was "np-session-0.6.3.tar", last modified: Thu May  4 19:22:17 2023, max compression
```

## Comparing `np-session-0.6.2.tar` & `np-session-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2289 2023-05-04 00:08:30.670540 np-session-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.2/README.md
--rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.2/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.2/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.2/src/np_session/components/info.py
--rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.2/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.2/src/np_session/components/mixins.py
--rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.2/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.2/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.2/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.2/src/np_session/components/state.py
--rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.2/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.2/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.2/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.2/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.2/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.2/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.2/src/np_session/exceptions.py
--rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.2/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.2/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.2/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.2/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0     8942 2023-05-04 00:08:23.244576 np-session-0.6.2/src/np_session/session.py
--rw-r--r--   0        0        0      181 2023-05-02 22:19:28.306490 np-session-0.6.2/src/np_session/subclasses/__init__.py
--rw-r--r--   0        0        0     5016 2023-05-03 22:31:26.830412 np-session-0.6.2/src/np_session/subclasses/dynamic_routing_pilot.py
--rw-r--r--   0        0        0    21636 2023-05-03 21:32:03.275128 np-session-0.6.2/src/np_session/subclasses/pipeline.py
--rw-r--r--   0        0        0     5446 2023-05-03 22:31:00.408944 np-session-0.6.2/src/np_session/subclasses/templeton_pilot.py
--rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.2/src/np_session/tasks.py
--rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.2/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.2/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.2/tests/test_platform_json.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2289 2023-05-04 19:22:12.488063 np-session-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.3/README.md
+-rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.3/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.3/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.3/src/np_session/components/info.py
+-rw-r--r--   0        0        0     9191 2023-05-02 22:17:19.176981 np-session-0.6.3/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.3/src/np_session/components/mixins.py
+-rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.3/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.3/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.3/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.3/src/np_session/components/state.py
+-rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.3/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.3/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.3/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.3/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.3/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.3/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.3/src/np_session/exceptions.py
+-rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.3/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.3/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.3/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.3/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0     8942 2023-05-04 00:08:23.244576 np-session-0.6.3/src/np_session/session.py
+-rw-r--r--   0        0        0      279 2023-05-04 19:21:42.017380 np-session-0.6.3/src/np_session/subclasses/__init__.py
+-rw-r--r--   0        0        0     4954 2023-05-04 02:16:46.922126 np-session-0.6.3/src/np_session/subclasses/dynamic_routing_pilot.py
+-rw-r--r--   0        0        0    21567 2023-05-04 02:17:18.728472 np-session-0.6.3/src/np_session/subclasses/pipeline.py
+-rw-r--r--   0        0        0     5384 2023-05-04 02:16:59.475311 np-session-0.6.3/src/np_session/subclasses/templeton_pilot.py
+-rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.3/src/np_session/tasks.py
+-rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.3/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.3/tests/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.3/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.3/tests/test_platform_json.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.3/PKG-INFO
```

### Comparing `np-session-0.6.2/pyproject.toml` & `np-session-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.6.2"
+version = "0.6.3"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-session-0.6.2/README.md` & `np-session-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/info.py` & `np-session-0.6.3/src/np_session/components/info.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/lims_manifests.py` & `np-session-0.6.3/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/mixins.py` & `np-session-0.6.3/src/np_session/components/mixins.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/paths.py` & `np-session-0.6.3/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/platform_json.py` & `np-session-0.6.3/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/settings_xml.py` & `np-session-0.6.3/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/components/state.py` & `np-session-0.6.3/src/np_session/components/state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/databases/data_getters.py` & `np-session-0.6.3/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/databases/firebase_state.py` & `np-session-0.6.3/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/databases/lims2.py` & `np-session-0.6.3/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/databases/mtrain.py` & `np-session-0.6.3/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/databases/redis_state.py` & `np-session-0.6.3/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/jobs/lims_upload.py` & `np-session-0.6.3/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/jobs/sessions.json` & `np-session-0.6.3/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/jobs/sync_states.py` & `np-session-0.6.3/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/session.py` & `np-session-0.6.3/src/np_session/session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/subclasses/dynamic_routing_pilot.py` & `np-session-0.6.3/src/np_session/subclasses/dynamic_routing_pilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     >>> str(session.project)
     'DRPilot'
     >>> str(session.rig)        # see np_config.Rig
     'NP.3'
     """
 
     is_ecephys = True   # not dealing with habs
-    is_ecephys_session = is_ecephys   # not dealing with habs
     project = 'DRPilot'
 
     storage_dirs: ClassVar[tuple[pathlib.Path, ...]] = tuple(
         pathlib.Path(_)
         for _ in (
             '//10.128.50.140/Data2',
             '//allen/programs/mindscope/workgroups/dynamicrouting/PilotEphys/Task 2 pilot',
```

### Comparing `np-session-0.6.2/src/np_session/subclasses/pipeline.py` & `np-session-0.6.3/src/np_session/subclasses/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,16 +216,14 @@
 
         Note that habs are classed as ecephys sessions: use `is_hab`.
         """
         if not self.lims or not self.lims.get('ecephys_session'):
             return None
         return 'ecephys_session' in self.lims['ecephys_session']
 
-    is_ecephys_session = is_ecephys   # for backwards compatibility
-
     @property
     def is_hab(self) -> bool | None:
         """False if hab session, None if unsure."""
         if not self.lims:
             return None
         return self.lims.get('name', '').startswith('HAB')
```

### Comparing `np-session-0.6.2/src/np_session/subclasses/templeton_pilot.py` & `np-session-0.6.3/src/np_session/subclasses/templeton_pilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     >>> str(session.project)
     'TempletonPilot'
     >>> str(session.rig)        # see np_config.Rig
     'NP.3'
     """
 
     is_ecephys = True   # not dealing with habs
-    is_ecephys_session = is_ecephys   # not dealing with habs
     project = 'TempletonPilot'
     
     datetime_format: ClassVar[str] = '%Y-%m-%d_%H-%M-%S'
     
     storage_dirs: ClassVar[tuple[pathlib.Path, ...]] = tuple(
         pathlib.Path(_)
         for _ in (
```

### Comparing `np-session-0.6.2/src/np_session/tasks.py` & `np-session-0.6.3/src/np_session/tasks.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/src/np_session/utils.py` & `np-session-0.6.3/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/tests/test_np_session.py` & `np-session-0.6.3/tests/test_np_session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/tests/test_platform_json.py` & `np-session-0.6.3/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.2/PKG-INFO` & `np-session-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

