# Comparing `tmp/kube_api-0.1.58.tar.gz` & `tmp/kube_api-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_api-0.1.58.tar", last modified: Mon Apr  3 20:14:32 2023, max compression
+gzip compressed data, was "kube_api-0.1.59.tar", last modified: Thu May  4 17:11:06 2023, max compression
```

## Comparing `kube_api-0.1.58.tar` & `kube_api-0.1.59.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:14:32.763171 kube_api-0.1.58/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-03 20:14:32.763171 kube_api-0.1.58/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:14:32.763171 kube_api-0.1.58/kube_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-03 20:14:24.000000 kube_api-0.1.58/kube_api/volumeclaims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:14:32.763171 kube_api-0.1.58/kube_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-03 20:14:32.000000 kube_api-0.1.58/kube_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-03 20:14:32.000000 kube_api-0.1.58/kube_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:14:32.000000 kube_api-0.1.58/kube_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 20:14:32.000000 kube_api-0.1.58/kube_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 20:14:32.000000 kube_api-0.1.58/kube_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:14:32.763171 kube_api-0.1.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-03 20:14:24.000000 kube_api-0.1.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 17:11:06.547321 kube_api-0.1.59/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/kube_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-04 17:10:54.000000 kube_api-0.1.59/kube_api/volumeclaims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:06.547321 kube_api-0.1.59/kube_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 17:11:06.000000 kube_api-0.1.59/kube_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:11:06.547321 kube_api-0.1.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-04 17:10:54.000000 kube_api-0.1.59/setup.py
```

### Comparing `kube_api-0.1.58/PKG-INFO` & `kube_api-0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube_api
-Version: 0.1.58
+Version: 0.1.59
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.58/kube_api/config.py` & `kube_api-0.1.59/kube_api/config.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.58/kube_api/jobs.py` & `kube_api-0.1.59/kube_api/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,28 +381,28 @@
 
     "workspace" and "outputs" volumes are shared by all containers.
 
     Attributes:
         workspace_path: The mount path for workspace volume.
         outputs_path: The mount path for outputs volume
     """
-    def __init__(self, job_name, namespace='default', workspace_path="/workspace/", output_path=None, workspace_size="1", output_size="1", shared_claim_name=None):
+    def __init__(self, job_name, namespace='default', workspace_path="/workspace/", output_path=None, workspace_size="1", output_size="1", shared_claim_name=None, backoff_limit=0):
         super().__init__(job_name, namespace)
         self.workspace_path = workspace_path
         if not self.workspace_path.endswith("/"):
             self.workspace_path += "/"
         self.outputs_path = output_path
         if isinstance(self.outputs_path, str) and not self.outputs_path.endswith("/"):
             self.outputs_path += "/"
 
         self.workspace_size = workspace_size
         self.output_size = output_size
         self.shared_claim_name = shared_claim_name
 
-        self.job_spec = dict(backoff_limit=0)
+        self.job_spec = dict(backoff_limit=backoff_limit)
         self.workspace_vc = None
         self.outputs_vc = None
         # envs will be shared by all jobs.
         self.envs = dict()
         if self.outputs_path:
             self.envs["OUTPUT_PATH"] = self.outputs_path
 
@@ -577,14 +577,15 @@
             A job name will be generated with a random string appended to the prefix.
         output_path: A directory for storing output data.
             This volume can be the same as workspace.
             User is responsible for copying the files output of output directory
             output_path will also be stored as a global environment variable OUTPUT_PATH
         workspace_size: Number of GB of storage needed for the workspace directory.
         output_size: Number of GB of storage needed for the output directory.
+        backoff_limit: Number of retries for the job.
 
         In each step, the following additional keys are accepted:
         cpu: The number of cpu requested.
         memory: The memory size (GB) requested.
 
         Examples:
             If the config is stored in a json file, a job can be launched by:
@@ -603,14 +604,16 @@
             kwargs["workspace_size"] = config.get("workspace_size")
         if "output_size" not in kwargs and config.get("output_size"):
             kwargs["output_size"] = config.get("output_size")
         if "preemptible" not in kwargs and config.get("preemptible"):
             kwargs["preemptible"] = config.get("preemptible")
         if "shared_claim_name" not in kwargs and config.get("shared_claim_name"):
             kwargs["shared_claim_name"] = config.get("shared_claim_name")
+        if "backoff_limit" not in kwargs and config.get("backoff_limit"):
+            kwargs["backoff_limit"] = config.get("backoff_limit")
 
         env_dict = dict()
 
         # Initialize job object
         # cls can be a subclass if run_config is called by a subclass.
         job = cls(job_name, **kwargs)
```

### Comparing `kube_api-0.1.58/kube_api/namespaces.py` & `kube_api-0.1.59/kube_api/namespaces.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.58/kube_api/pods.py` & `kube_api-0.1.59/kube_api/pods.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.58/kube_api/utils.py` & `kube_api-0.1.59/kube_api/utils.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.58/kube_api/volumeclaims.py` & `kube_api-0.1.59/kube_api/volumeclaims.py`

 * *Files identical despite different names*

### Comparing `kube_api-0.1.58/kube_api.egg-info/PKG-INFO` & `kube_api-0.1.59/kube_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-api
-Version: 0.1.58
+Version: 0.1.59
 Summary: A simple Kubernetes Python API
 Home-page: https://github.com/labdave/kube_api
 Author: Qiu Qin
 Author-email: qiuosier@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kube_api-0.1.58/setup.py` & `kube_api-0.1.59/setup.py`

 * *Files identical despite different names*

