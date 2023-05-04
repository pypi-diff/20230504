# Comparing `tmp/prefect-kubernetes-0.2.6.tar.gz` & `tmp/prefect-kubernetes-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-6rqdzdp5/prefect-kubernetes-0.2.6.tar", last modified: Fri Apr 28 14:47:52 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-uuh3r2jr/prefect-kubernetes-0.2.7.tar", last modified: Thu May  4 16:17:35 2023, max compression
```

## Comparing `prefect-kubernetes-0.2.6.tar` & `prefect-kubernetes-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    32697 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_events_replicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    77624 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32770 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:35.000000 prefect-kubernetes-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77624 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-04 16:15:37.000000 prefect-kubernetes-0.2.7/versioneer.py
```

### Comparing `prefect-kubernetes-0.2.6/LICENSE` & `prefect-kubernetes-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/PKG-INFO` & `prefect-kubernetes-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.6/README.md` & `prefect-kubernetes-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/credentials.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/custom_objects.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/deployments.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/events.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,33 @@
     "Completed",
     "DeadlineExceeded",
     "ImageGCFailed",
     "NodeLost",
     "NodeOutOfDisk",
 }
 
+FINAL_PHASES = {"Succeeded", "Failed"}
+
 
 class KubernetesEventsReplicator:
     """Replicates Kubernetes pod events to Prefect events."""
 
     def __init__(
         self,
         client: "ApiClient",
         job_name: str,
         namespace: str,
         worker_resource: Dict[str, str],
         related_resources: List[RelatedResource],
+        timeout_seconds: int,
     ):
         self._client = client
         self._job_name = job_name
         self._namespace = namespace
+        self._timeout_seconds = timeout_seconds
 
         # All events emitted by this replicator have the pod itself as the
         # resource. The `worker_resource` is what the worker uses when it's
         # the primary resource, so here it's turned into a related resource
         # instead.
         worker_resource["prefect.resource.role"] = "worker"
         worker_related_resource = RelatedResource(__root__=worker_resource)
@@ -86,20 +90,23 @@
 
         try:
             core_client = kubernetes.client.CoreV1Api(api_client=self._client)
             for event in self._watch.stream(
                 func=core_client.list_namespaced_pod,
                 namespace=self._namespace,
                 label_selector=f"job-name={self._job_name}",
+                timeout_seconds=self._timeout_seconds,
             ):
                 phase = event["object"].status.phase
 
                 if phase not in seen_phases:
                     last_event = self._emit_pod_event(event, last_event=last_event)
                     seen_phases.add(phase)
+                    if phase in FINAL_PHASES:
+                        self._watch.stop()
         finally:
             self._client.rest_client.pool_manager.clear()
 
     def _emit_pod_event(
         self,
         pod_event: Dict,
         last_event: Optional[Event] = None,
```

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/exceptions.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/flows.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/jobs.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/pods.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/services.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/utilities.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes/worker.py` & `prefect-kubernetes-0.2.7/prefect_kubernetes/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,15 @@
                 client=client,
                 job_name=job.metadata.name,
                 namespace=configuration.namespace,
                 worker_resource=self._event_resource(),
                 related_resources=self._event_related_resources(
                     configuration=configuration
                 ),
+                timeout_seconds=configuration.pod_watch_timeout_seconds,
             )
 
             with events_replicator:
                 status_code = await run_sync_in_worker_thread(
                     self._watch_job, job.metadata.name, configuration, client
                 )
             return KubernetesWorkerResult(identifier=pid, status_code=status_code)
```

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/PKG-INFO` & `prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect-kubernetes-0.2.7/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/setup.cfg` & `prefect-kubernetes-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/setup.py` & `prefect-kubernetes-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_block_standards.py` & `prefect-kubernetes-0.2.7/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_credentials.py` & `prefect-kubernetes-0.2.7/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_custom_objects.py` & `prefect-kubernetes-0.2.7/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_deployments.py` & `prefect-kubernetes-0.2.7/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_events_replicator.py` & `prefect-kubernetes-0.2.7/tests/test_events_replicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 def replicator(client, worker_resource, related_resources):
     return KubernetesEventsReplicator(
         client=client,
         job_name="test-job",
         namespace="test-namespace",
         worker_resource=worker_resource,
         related_resources=related_resources,
+        timeout_seconds=60,
     )
 
 
 def test_lifecycle(replicator):
     mock_watch = MagicMock(spec=kubernetes.watch.Watch)
     mock_thread = MagicMock(spec=threading.Thread)
 
@@ -252,14 +253,15 @@
                         }
                     ),
                 ],
                 follows=2,
             ),
         ]
     )
+    mock_watch.stop.assert_called_once_with()
 
 
 def test_replicate_failed_pod_events(replicator, failed_pod_stream):
     mock_watch = MagicMock(spec=kubernetes.watch.Watch)
     mock_watch.stream.return_value = failed_pod_stream
 
     event_count = 0
@@ -343,14 +345,15 @@
                         }
                     ),
                 ],
                 follows=2,
             ),
         ]
     )
+    mock_watch.stop.assert_called_once_with()
 
 
 def test_replicate_evicted_pod_events(replicator, evicted_pod_stream):
     mock_watch = MagicMock(spec=kubernetes.watch.Watch)
     mock_watch.stream.return_value = evicted_pod_stream
 
     event_count = 0
@@ -435,7 +438,8 @@
                         }
                     ),
                 ],
                 follows=2,
             ),
         ]
     )
+    mock_watch.stop.assert_called_once_with()
```

### Comparing `prefect-kubernetes-0.2.6/tests/test_flows.py` & `prefect-kubernetes-0.2.7/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_jobs.py` & `prefect-kubernetes-0.2.7/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_pods.py` & `prefect-kubernetes-0.2.7/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_services.py` & `prefect-kubernetes-0.2.7/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_utilities.py` & `prefect-kubernetes-0.2.7/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/tests/test_worker.py` & `prefect-kubernetes-0.2.7/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.6/versioneer.py` & `prefect-kubernetes-0.2.7/versioneer.py`

 * *Files identical despite different names*

