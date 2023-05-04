# Comparing `tmp/bodosdk-1.2.9.tar.gz` & `tmp/bodosdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.2.9.tar", last modified: Wed Apr 19 11:27:10 2023, max compression
+gzip compressed data, was "bodosdk-1.3.0.tar", last modified: Thu May  4 04:38:57 2023, max compression
```

## Comparing `bodosdk-1.2.9.tar` & `bodosdk-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-19 11:27:05.000000 bodosdk-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-19 11:27:05.000000 bodosdk-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-04-19 11:27:10.780630 bodosdk-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    34206 2023-04-19 11:27:05.000000 bodosdk-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.776630 bodosdk-1.2.9/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7389 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    11856 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5931 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     8896 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    12486 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.776630 bodosdk-1.2.9/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-19 11:27:10.780630 bodosdk-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 11:27:05.000000 bodosdk-1.2.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-04-19 11:27:05.000000 bodosdk-1.2.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-04 04:38:51.000000 bodosdk-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-04 04:38:51.000000 bodosdk-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-04 04:38:57.904533 bodosdk-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-04 04:38:51.000000 bodosdk-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12693 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.900533 bodosdk-1.3.0/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-04 04:38:57.904533 bodosdk-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-04 04:38:51.000000 bodosdk-1.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-04 04:38:51.000000 bodosdk-1.3.0/versioneer.py
```

### Comparing `bodosdk-1.2.9/LICENSE` & `bodosdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/PKG-INFO` & `bodosdk-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.2.9
+Version: 1.3.0
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -419,14 +419,15 @@
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
 - [get cluster](#get-cluster)
 - [remove cluster](#remove-cluster)
 - [scale cluster](#scale-cluster)
 - [get jobs for cluster](#list-jobs-for-cluster)
+- [modify cluster metadata](#modify-cluster-metadata)
 
 ### Available instance types<a id="available-instance-types"></a>
 
 `BodoClient.cluster.get_available_instance_types(region:str)`
 
 Returns list of instance types available for given region
 
@@ -595,14 +596,45 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.cluster.list_jobs(uuid, status=[JobStatus.NEW, JobStatus.INPROGRESS])
 ```
 
+### Modify Cluster metadata <a id="modify-cluster-metadata"></a>
+```BodoClient.cluster.modify(uuid)```
+This function can be used to edit cluster metadata for a given cluster. The properties that we can edit are
+description, autopause time, autoshutdown time and the number of workers. Changing the number of workers will
+kick off a scaling event on the cluster, which will resume the cluster if it is in paused state.
+The ModifyCluster object has the 4 properties as optional keys, meaning you can change just a subset of the 4 properties in a
+request too.
+
+```python3
+from bodosdk.models import WorkspaceKeys, ModifyCluster, ClusterResponse
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    auto_pause=60,
+    auto_shutdown=0,
+    workers_quantity=4,
+    description="using the SDK"
+)
+partial_modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    autopause=120,
+)
+new_cluster: List[ClusterResponse] = client.cluster.modify(modify_cluster)
+new_cluster_partial: List[ClusterResponse] = client.cluster.modify(partial_modify_cluster)
+```
 
 ### Workspace resource<a id="workspace-resource"></a>
 Module responsible for managing workspaces in an organization.
 
 - [workspace getting started](#workspace-getting-started)
 - [create workspace](#create-workspace)
 - [list workspaces](#list-workspaces)
```

### Comparing `bodosdk-1.2.9/README.md` & `bodosdk-1.3.0/bodosdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: bodosdk
+Version: 1.3.0
+Summary: Bodo Platform SDK
+Home-page: https://github.com/Bodo-inc/bodo-sdk
+Author: Bodo, Inc.
+Author-email: noreply@bodo.ai
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Bodo Platform SDK
 
 A simple SDK for Bodo Cloud Platform.
 
 List of contents:
 
 - [Getting Started](#getting-started)
@@ -398,14 +419,15 @@
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
 - [get cluster](#get-cluster)
 - [remove cluster](#remove-cluster)
 - [scale cluster](#scale-cluster)
 - [get jobs for cluster](#list-jobs-for-cluster)
+- [modify cluster metadata](#modify-cluster-metadata)
 
 ### Available instance types<a id="available-instance-types"></a>
 
 `BodoClient.cluster.get_available_instance_types(region:str)`
 
 Returns list of instance types available for given region
 
@@ -574,14 +596,45 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.cluster.list_jobs(uuid, status=[JobStatus.NEW, JobStatus.INPROGRESS])
 ```
 
+### Modify Cluster metadata <a id="modify-cluster-metadata"></a>
+```BodoClient.cluster.modify(uuid)```
+This function can be used to edit cluster metadata for a given cluster. The properties that we can edit are
+description, autopause time, autoshutdown time and the number of workers. Changing the number of workers will
+kick off a scaling event on the cluster, which will resume the cluster if it is in paused state.
+The ModifyCluster object has the 4 properties as optional keys, meaning you can change just a subset of the 4 properties in a
+request too.
+
+```python3
+from bodosdk.models import WorkspaceKeys, ModifyCluster, ClusterResponse
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    auto_pause=60,
+    auto_shutdown=0,
+    workers_quantity=4,
+    description="using the SDK"
+)
+partial_modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    autopause=120,
+)
+new_cluster: List[ClusterResponse] = client.cluster.modify(modify_cluster)
+new_cluster_partial: List[ClusterResponse] = client.cluster.modify(partial_modify_cluster)
+```
 
 ### Workspace resource<a id="workspace-resource"></a>
 Module responsible for managing workspaces in an organization.
 
 - [workspace getting started](#workspace-getting-started)
 - [create workspace](#create-workspace)
 - [list workspaces](#list-workspaces)
@@ -1295,7 +1348,9 @@
 keys = WorkspaceKeys(
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 secret_info: SecretInfo = client.secrets.remove("<secret-uuid>")
 ```
+
+
```

### Comparing `bodosdk-1.2.9/bodosdk/api/auth.py` & `bodosdk-1.3.0/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/base.py` & `bodosdk-1.3.0/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/catalog.py` & `bodosdk-1.3.0/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/cloud_config.py` & `bodosdk-1.3.0/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/cluster.py` & `bodosdk-1.3.0/bodosdk/api/cluster.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from bodosdk.models.cluster import (
     ClusterDefinition,
     ClusterTaskInfo,
     InstanceType,
     InstanceCategory,
     BodoImage,
     ClusterResponse,
+    ModifyCluster,
     ScaleCluster,
 )
 from bodosdk.models.job import JobResponse, JobStatus
 
 
 class ClusterApi(BackendApi):
     def __init__(self, *args, **kwargs):
@@ -157,14 +158,33 @@
             headers=headers,
         )
 
         if str(resp.status_code).startswith("2"):
             return ClusterResponse(**resp.json())
         if resp.status_code == 404:
             raise ResourceNotFound()
+        if resp.status_code in (400, 422):
+            raise ValidationError(resp.json())
+        if resp.status_code == 503:
+            raise ServiceUnavailable
+        raise UnknownError
+
+    def modify_cluster(self, modify_cluster: ModifyCluster):
+        headers = {"Content-type": "application/json"}
+        headers.update(self.get_auth_header())
+        resp = self._requests.patch(
+            f"{self.get_resource_url()}/modify/{modify_cluster.uuid}",
+            data=modify_cluster.json(by_alias=True, exclude={"uuid": True}),
+            headers=headers,
+        )
+
+        if str(resp.status_code).startswith("2"):
+            return ClusterResponse(**resp.json())
+        if resp.status_code == 404:
+            raise ResourceNotFound()
         if resp.status_code in (400, 422):
             raise ValidationError(resp.json())
         if resp.status_code == 503:
             raise ServiceUnavailable
         raise UnknownError
 
     def pause(self, uuid):
```

### Comparing `bodosdk-1.2.9/bodosdk/api/instance_role.py` & `bodosdk-1.3.0/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/job.py` & `bodosdk-1.3.0/bodosdk/api/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,48 +8,49 @@
 from bodosdk.exc import (
     ResourceNotFound,
     ServiceUnavailable,
     UnknownError,
     ValidationError,
 )
 from bodosdk.models.job import (
+    LIST_QUERY_PARAMS,
+    PaginationOrder,
+    DEFAULT_PAGE,
+    DEFAULT_PAGE_SIZE,
+    DEFAULT_ORDER,
+)
+from bodosdk.models.job import (
     JobDefinition,
     JobResponse,
     JobExecution,
     JobCreateResponse,
     CreateBatchJobDefinition,
     BatchJobDefinitionResponse,
     JobConfigOverride,
     JobRunResponse,
-    PaginationDetails,
     JobRunType,
     CreateJobRun,
     JobRunStatus,
+    CreateSQLJobRun,
 )
 
 
 # helper function to compose query string from query parameters
 def build_query_string(args):
-    if len(args) == 0:
-        return ""
-    query_string = "?"
-    counter = 0
+    query_params = []
     for k, v in args.items():
-        if v is not None:
+        if v:
             if isinstance(v, list):
-                query_string += f"{k}="
-                for item in v[:-2]:
-                    query_string += {item} + ","
-                query_string += f"{v[-1]}&"
+                param = f"{k}[]={','.join(f'{x}' for x in v)}"
             else:
-                query_string += f"{k}={v}&"
-            counter += 1
-    if counter == 0:
-        return ""
-    return query_string
+                param = f"{k}={v}"
+            query_params.append(param)
+    if query_params:
+        return "?" + "&".join(query_params)
+    return ""
 
 
 class JobApi(BackendApi):
     def __init__(self, *args, **kwargs):
         super(JobApi, self).__init__(*args, **kwargs)
         self._resource_url = "job"
 
@@ -178,28 +179,27 @@
             raise ServiceUnavailable
         raise UnknownError(resp.content)
 
     # Todo: add query semantics for filtering
     @validate_arguments
     def list_batch_job_definitions(
         self,
-        pagination_details: PaginationDetails = None,
+        page: int = DEFAULT_PAGE,
+        page_size: int = DEFAULT_PAGE_SIZE,
+        sort_order: PaginationOrder = DEFAULT_ORDER,
     ) -> List[BatchJobDefinitionResponse]:
-        args = locals()
-        args_keys = list(args.keys())
-        args_keys.remove("self")
-        query_string_args = dict([(key, args[key]) for key in args_keys])
+        query_string_args = {
+            k: v for k, v in locals().items() if v and k in LIST_QUERY_PARAMS
+        }
         headers = self.get_auth_header()
-        resource_url = (
-            f"{self.get_resource_url()}/batch_job_def{build_query_string(args)}"
-        )
+        resource_url = f"{self.get_resource_url()}/batch_job_def{build_query_string(query_string_args)}"
         resp = self._requests.get(resource_url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
-        if self(resp.status_code).startswith("4"):
+        if str(resp.status_code).startswith("4"):
             raise ResourceNotFound(resp.json()["message"])
 
         result = []
         for json_data in resp.json():
             result.append(BatchJobDefinitionResponse(**json_data))
         return result
 
@@ -258,14 +258,33 @@
                 "May have specified a default cluster which doesn't belong the workspace"
             )
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         raise UnknownError(resp.content)
 
     @validate_arguments
+    def create_sql_job_run(self, create_sql_job_run: CreateSQLJobRun) -> JobRunResponse:
+        headers = {"Content-type": "application/json"}
+        headers.update(self.get_auth_header())
+        resp = self._requests.post(
+            f"{self.get_resource_url()}/run/sql",
+            data=create_sql_job_run.json(by_alias=True),
+            headers=headers,
+        )
+        if str(resp.status_code).startswith("2"):
+            return JobRunResponse(**resp.json())
+        if resp.status_code == 404:
+            raise ResourceNotFound("Cluster or Catalog not found")
+        if resp.status_code == 409:
+            raise ResourceNotFound("Cluster can't accept job")
+        if str(resp.status_code).startswith("5"):
+            raise ServiceUnavailable
+        raise UnknownError(resp.content)
+
+    @validate_arguments
     def get_job_run(self, uuid: UUID, job_type: JobRunType = "BATCH") -> JobRunResponse:
         job_type_url_suffix = job_type.lower()
         headers = self.get_auth_header()
         resp = self._requests.get(
             f"{self.get_resource_url()}/run/{job_type_url_suffix}/{uuid}",
             headers=headers,
         )
@@ -292,21 +311,22 @@
         self,
         job_type: List[JobRunType] = None,
         batch_job_id: Union[List[UUID], None] = None,
         status: Union[List[JobRunStatus], None] = None,
         cluster_id: Union[List[UUID], None] = None,
         started_at: Union[datetime, None] = None,
         finished_at: Union[datetime, None] = None,
-        pagination_details=None,
+        page: int = 1,
+        page_size: int = 100,
+        order: PaginationOrder = PaginationOrder.ASC,
     ) -> List[JobRunResponse]:
-        args = locals()
-        args_keys = list(args.keys())
-        args_keys.remove("self")
-        query_string_args = dict([(key, args[key]) for key in args_keys])
-        headers = self.get_auth_header()
+        args = LIST_QUERY_PARAMS
+        query_string_args = {
+            k: v for k, v in locals().items() if k in args and v is not None
+        }
         headers = self.get_auth_header()
         query_string = build_query_string(query_string_args)
         url = f"{self.get_resource_url()}/run{query_string}"
         resp = self._requests.get(url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable()
         if str(resp.status_code).startswith("4"):
```

### Comparing `bodosdk-1.2.9/bodosdk/api/request_wrapper.py` & `bodosdk-1.3.0/bodosdk/api/request_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, print_logs=False):
         self.print_logs = print_logs
         self._session = requests.Session()
         # Retry for:
         # Request Timeout, Locked, Too Early, Too Many Requests, Conflict
         # Internal Server Error, Gateway Timeout
         retries = Retry(
-            total=5,
+            total=10,
             backoff_factor=0.2,
             status_forcelist=[408, 423, 425, 429, 409, 500, 504],
         )
 
         self._session.mount("http://", HTTPAdapter(max_retries=retries))
         self._session.mount("https://", HTTPAdapter(max_retries=retries))
```

### Comparing `bodosdk-1.2.9/bodosdk/api/secret_group.py` & `bodosdk-1.3.0/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/secrets.py` & `bodosdk-1.3.0/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/api/workspace.py` & `bodosdk-1.3.0/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/base.py` & `bodosdk-1.3.0/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/catalog.py` & `bodosdk-1.3.0/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/cloud_config.py` & `bodosdk-1.3.0/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/cluster.py` & `bodosdk-1.3.0/bodosdk/client/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bodosdk.models.cluster import (
     ClusterDefinition,
     ClusterMetadata,
     ClusterResponse,
     ClusterTaskInfo,
     InstanceCategory,
     BodoImage,
+    ModifyCluster,
     ScaleCluster,
 )
 from bodosdk.models.job import JobClusterDefinition, JobResponse
 
 
 class ClusterClient:
     def __init__(self, api: ClusterApi):
@@ -130,14 +131,29 @@
         :input: uuid and new scale
         :type: str and ScaleCluster object
         :return: the updates metadata about the cluster after the api call
         :rtype: ClusterResponse
         """
         return self._api.scale_cluster(scale_cluster)
 
+    def modify(self, modify_cluster: ModifyCluster) -> ClusterResponse:
+        """
+        Allows the client to the edit cluster metadata, which includes the description, auto pause time
+        autoshutdown time and also the number of workers in the cluster with `uuid` to the specified
+        new scale, which will trigger a scale task on the cluster
+
+        :input uuid
+        :input modify_cluster ModifyCluster object which fields description(string), auto_pause(minutes, int)
+                auto_shutdown(minutes, int) and workers_quantity(int)
+        :type: str and ModifyClusteobject
+        :return: the updates metadata about the cluster after the api call
+        :rtype: ClusterResponse
+        """
+        return self._api.modify_cluster(modify_cluster)
+
     def pause(self, uuid) -> ClusterResponse:
         """
         Stops cluster, cluster may be resumed later on.
 
         :input: uuid
         :type: uuid
         :return: the updates metadata about the cluster after the api call
```

### Comparing `bodosdk-1.2.9/bodosdk/client/instance_role.py` & `bodosdk-1.3.0/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/job.py` & `bodosdk-1.3.0/bodosdk/client/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     JobCreateResponse,
     BatchJobDefinitionResponse,
     CreateBatchJobDefinition,
     JobRunResponse,
     JobRunType,
     CreateJobRun,
     JobRunStatus,
+    CreateSQLJobRun,
 )
 
 
 class JobWaiter:
     def __init__(self, client):
         """
         Object for waiting till job finishes
@@ -277,7 +278,26 @@
         :raises ResourceNotFound:
         """
         try:
             job_run = self._api.get_job_run(batch_job_run_uuid)
             return job_run.status
         except Exception as exception:
             raise exception
+
+    def submit_sql_job_run(self, create_sql_job_run: CreateSQLJobRun) -> JobRunResponse:
+        """
+        Creates a sql job run
+
+        :param create_sql_job_run:
+            definition of sql job run
+        :type create_sql_job_run: CreateSQLJobRun
+        :return: created sql job run
+        :rtype: JobRunResponse
+        :raises Unauthorized: when keys are invalid
+        :raises ValidationError: when SqlJobRun is invalid
+        """
+        try:
+            job_run = self._api.create_sql_job_run(create_sql_job_run)
+            logging.info(f"Sql job run {job_run.uuid} submitted.")
+            return job_run
+        except Exception as exception:
+            raise exception
```

### Comparing `bodosdk-1.2.9/bodosdk/client/secret_group.py` & `bodosdk-1.3.0/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/secrets.py` & `bodosdk-1.3.0/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/client/workspace.py` & `bodosdk-1.3.0/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/models/__init__.py` & `bodosdk-1.3.0/bodosdk/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     InstanceCategory,
     BodoImage,
     ClusterMetadata,
     ClusterDefinition,
     ClusterResponse,
     ClusterTaskInfo,
     ScaleCluster,
+    ModifyCluster,
 )
 
 from bodosdk.models.workspace import (
     WorkspaceDefinition,
     WorkspaceCreatedResponse,
     WorkspaceInfo,
     WorkspaceListItem,
@@ -60,8 +61,12 @@
     JobConfig,
     JobConfigOverride,
     WorkspaceDef,
     SourceCodeType,
     RetryStrategy,
     JobSource,
     JobSourceType,
+    CreateJobRun,
+    JobRunResponse,
+    JobRunStatus,
+    CreateSQLJobRun,
 )
```

### Comparing `bodosdk-1.2.9/bodosdk/models/base.py` & `bodosdk-1.3.0/bodosdk/models/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/models/catalog.py` & `bodosdk-1.3.0/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/models/cloud_config.py` & `bodosdk-1.3.0/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk/models/cluster.py` & `bodosdk-1.3.0/bodosdk/models/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,7 +80,15 @@
     task_type: str = Field(..., alias="taskType")
     logs: str
 
 
 class ScaleCluster(CamelCaseBase):
     uuid: Union[str, UUID]
     workers_quantity: int = Field(..., alias="workersQuantity")
+
+
+class ModifyCluster(CamelCaseBase):
+    uuid: Union[str, UUID]
+    auto_shutdown: Optional[int] = Field(None, alias="autoshutdown")
+    auto_pause: Optional[int] = Field(None, alias="autopause")
+    description: Optional[str] = Field(None, alias="description")
+    workers_quantity: Optional[int] = Field(-1, alias="workersQuantity")
```

### Comparing `bodosdk-1.2.9/bodosdk/models/job.py` & `bodosdk-1.3.0/bodosdk/models/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     uuid: Union[str, UUID]
 
 
 class JobSourceType(enum.Enum):
     GIT = "GIT"
     S3 = "S3"
     WORKSPACE = "WORKSPACE"
+    SQL = "SQL"
+
+    def __repr__(self):
+        return self.value
 
 
 class GitRepoSource(CamelCaseBase):
     type: JobSourceType = Field(JobSourceType.GIT, const=True)
     repo_url: str = Field(..., alias="repoUrl")
     reference: Optional[str] = ""
     username: str
@@ -176,14 +180,22 @@
     path: str
         Workspace path.
     """
 
     path: str
 
 
+class SQLDef(CamelCaseBase):
+    """
+    SQL source definition.
+
+    ...
+    """
+
+
 class JobSource(CamelCaseBase):
     """
     Job source.
 
     ...
 
     Attributes
@@ -192,15 +204,17 @@
         Job source type.
 
     definition: Union[GitDef, S3Def, WorkspaceDef]
         Job source definition.
     """
 
     type: JobSourceType
-    definition: Union[GitDef, S3Def, WorkspaceDef] = Field(..., alias="def")
+    definition: Union[GitDef, S3Def, WorkspaceDef, SQLDef] = Field(
+        ..., alias="sourceDef"
+    )
 
 
 class RetryStrategy(CamelCaseBase):
     """
     Retry strategy for a job.
 
     ...
@@ -224,14 +238,20 @@
 
 
 class SourceCodeType(enum.Enum):
     PYTHON = "PYTHON"
     IPYNB = "IPYNB"
     SQL = "SQL"
 
+    def __repr__(self):
+        return self.value
+
+    def __str__(self):
+        return self.value
+
 
 class JobConfig(CamelCaseBase):
     """
     Job configuration.
 
     ...
 
@@ -239,38 +259,56 @@
     ----------
     source: JobSource
         Job source.
 
     source_code_type: SourceCodeType
         Job source code type.
 
-    sourceLocation: str
+    sourceLocation: Optional[str]
         Job source location.
 
     args: Union[str, Dict]
         Job arguments. (Default: {})
 
-    retry_strategy: RetryStrategy
+    retry_strategy: Optional[RetryStrategy]
         Job retry strategy. (Default: {num_retries: 0, delay_between_retries: 1, retry_on_timeout: False})
 
     timeout: int
         Job timeout in minutes. (Default: 60)
 
     env_vars: Dict
         Job environment variables. (Default: {})
 
+    catalog: Optional[str]
+        Catalog name. (Default: None)
+
     """
 
     source: JobSource
     source_code_type: SourceCodeType = Field(..., alias="type")
-    sourceLocation: str
+    sourceLocation: Optional[str]
     args: Union[str, Dict, None] = Field(default_factory=dict)
-    retry_strategy: RetryStrategy = Field(RetryStrategy(), alias="retryStrategy")
+    retry_strategy: Optional[RetryStrategy] = Field(
+        RetryStrategy(), alias="retryStrategy"
+    )
     timeout: int = 60
     env_vars: Union[None, Dict] = Field(default_factory=dict, alias="envVars")
+    catalog: Optional[str] = None
+
+    def __repr__(self):
+        repr_str = ""
+        for k, v in self.dict().items():
+            if v is not None:
+                repr_str += f"{k}: {v}\n"
+            else:
+                repr_str += f"{k}: None\n"
+        return repr_str[:-1]  # remove last newline
+
+    def __str__(self):
+        return self.__repr__()
 
 
 class JobConfigOverride(CamelCaseBase):
     """
     Job configuration override.
 
     ...
@@ -330,30 +368,34 @@
     clusterUUID: Optional[str]
         Job cluster.
     """
 
     name: str
     description: str
     config: JobConfig
-    cluster_config: JobClusterDefinition = Field(..., alias="clusterConfig")
-    clusterUUID: Optional[str] = None  # Todo(Ritwika): Confirm
+    cluster_config: JobClusterDefinition = Field(default=None, alias="clusterConfig")
+    clusterUUID: Optional[Union[str, UUID]] = None  # Todo(Ritwika): Confirm
 
 
 class JobRunType(str, enum.Enum):
     BATCH = "BATCH"
     INTERACTIVE = "INTERACTIVE"
 
 
 class JobRunStatus(str, enum.Enum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
     CANCELLED = "CANCELLED"
     CANCELLING = "CANCELLING"
+    TIMED_OUT = "TIMEOUT"
+
+    def __repr__(self):
+        return self.value
 
 
 class JobRunResponse(CamelCaseBase):
     """
     Job run response.
 
     ...
@@ -417,24 +459,36 @@
     lastHealthCheck: Optional[Union[datetime, None]] = Field(
         default=None, alias="lastHealthCheck"
     )
     lastKnownActivity: Optional[Union[datetime, None]] = Field(
         default=None, alias="lastknownActivity"
     )
 
+    def __repr__(self):
+        repr_string = ""
+        for key, value in self.__dict__.items():
+            if value is not None:
+                repr_string += f"{key}: {value}\n"
+            else:
+                repr_string += f"{key}: None\n"
+        return repr_string[:-1]  # remove last newline
+
+    def __str__(self):
+        return self.__repr__()
+
 
 class BatchJobDefinitionResponse(CamelCaseBase):
     """
     Batch job definition response.
 
     ...
 
     Attributes
     ----------
-    job_def_id: UUID
+    uuid: UUID
         Job definition ID.
 
     name: str
         Job definition name.
 
     description: str
         Job definition description.
@@ -449,21 +503,21 @@
         Job cluster UUID.
 
     created_by: str
         Job definition creator.
 
     """
 
-    job_def_id: UUID = Field(..., alias="uuid")
+    uuid: UUID
     name: str
     description: str
     config: JobConfig
     clusterConfig: JobClusterDefinition = Field(..., alias="clusterConfig")
-    clusterUUID: Optional[str]  # Todo(Ritwika): Confirm
-    created_by: str = Field(..., alias="createdBy")
+    clusterUUID: Optional[Union[UUID, str]]  # Todo(Ritwika): Confirm
+    created_by: Optional[str] = Field(alias="createdBy")
     job_runs: List[JobRunResponse] = Field(default_factory=list, alias="jobRuns")
     # Run related fields
     # Rules related fields
 
 
 class CreateJobRun(CamelCaseBase):
     """
@@ -472,50 +526,92 @@
     ...
 
     Attributes
     ----------
     type: JobRunType
         Job run type.
 
-    clusterUUID: Optional[str]
+    clusterUUID: Optional[Union[UUID, str]]
         Job cluster UUID.
 
-    batchJobUUID: Optional[str]
+    batchJobUUID: Optional[Union[UUID, str]]
         Batch job UUID.
 
     batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
         Batch job definition configuration overrides.
     """
 
     type: JobRunType = JobRunType.BATCH
-    clusterUUID: Optional[str]  # Todo(Ritwika): Confirm
-    batchJobDefinitionUUID: Optional[str] = Field(..., alias="batchJobDefinitionUUID")
+    clusterUUID: Optional[Union[UUID, str]]  # Todo(Ritwika): Confirm
+    batchJobDefinitionUUID: Optional[Union[UUID, str]] = Field(
+        ..., alias="batchJobDefinitionUUID"
+    )
     batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
 
 
-class PaginationOrder(str, enum.Enum):
-    ASC = "ASC"
-    DESC = "DESC"
-
-
-class PaginationDetails(CamelCaseBase):
+class CreateSQLJobRun(CamelCaseBase):
     """
-    Pagination details.
+    Create SQL job run.
 
     ...
 
     Attributes
     ----------
-    page_size: int
-        Total number of items on page.
+    type: JobRunType
+        Job run type.
 
-    page: int
-        Offset of the current page.
+    clusterUUID: Optional[str]
+        Job cluster UUID.
+
+    cluster_config: Optional[JobClusterDefinition]
+        Job cluster configuration.
 
-    order: PaginationOrder
-        order of the page.
+    catalog: str
+        Catalog name.
+
+    retry_strategy: Optional[RetryStrategy]
+        Retry strategy.
+
+    timeout: Optional[int]
+        Job timeout in minutes. (Default: 60)
+
+    env_vars: Optional[Dict]
+        Job environment variables. (Default: {})
 
+    sql_query_text: str
+        SQL query text.
     """
 
-    page_size: int = Field(5, alias="pageSize")
-    page: int = Field(1)
-    order: PaginationOrder = Field(PaginationOrder.ASC)
+    type: JobRunType = JobRunType.BATCH
+    clusterUUID: Optional[Union[UUID, str]]
+    cluster_config: Optional[JobClusterDefinition] = Field(
+        default=None, alias="clusterConfig"
+    )
+    catalog: str
+    retry_strategy: Optional[RetryStrategy] = Field(
+        RetryStrategy(), alias="retryStrategy"
+    )
+    timeout: Optional[int] = 60
+    env_vars: Optional[Dict] = Field(default_factory=dict, alias="envVars")
+    sql_query_text: str = Field(..., alias="sqlQueryText")
+
+
+class PaginationOrder(str, enum.Enum):
+    ASC = "ASC"
+    DESC = "DESC"
+
+
+DEFAULT_PAGE_SIZE = 5
+DEFAULT_PAGE = 1
+DEFAULT_ORDER = PaginationOrder.ASC
+
+LIST_QUERY_PARAMS = [
+    "job_type",
+    "batch_job_id",
+    "status",
+    "cluster_id",
+    "started_at",
+    "finished_at",
+    "page",
+    "page_size",
+    "order",
+]
```

### Comparing `bodosdk-1.2.9/bodosdk/models/workspace.py` & `bodosdk-1.3.0/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: bodosdk
-Version: 1.2.9
-Summary: Bodo Platform SDK
-Home-page: https://github.com/Bodo-inc/bodo-sdk
-Author: Bodo, Inc.
-Author-email: noreply@bodo.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Bodo Platform SDK
 
 A simple SDK for Bodo Cloud Platform.
 
 List of contents:
 
 - [Getting Started](#getting-started)
@@ -419,14 +398,15 @@
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
 - [get cluster](#get-cluster)
 - [remove cluster](#remove-cluster)
 - [scale cluster](#scale-cluster)
 - [get jobs for cluster](#list-jobs-for-cluster)
+- [modify cluster metadata](#modify-cluster-metadata)
 
 ### Available instance types<a id="available-instance-types"></a>
 
 `BodoClient.cluster.get_available_instance_types(region:str)`
 
 Returns list of instance types available for given region
 
@@ -595,14 +575,45 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.cluster.list_jobs(uuid, status=[JobStatus.NEW, JobStatus.INPROGRESS])
 ```
 
+### Modify Cluster metadata <a id="modify-cluster-metadata"></a>
+```BodoClient.cluster.modify(uuid)```
+This function can be used to edit cluster metadata for a given cluster. The properties that we can edit are
+description, autopause time, autoshutdown time and the number of workers. Changing the number of workers will
+kick off a scaling event on the cluster, which will resume the cluster if it is in paused state.
+The ModifyCluster object has the 4 properties as optional keys, meaning you can change just a subset of the 4 properties in a
+request too.
+
+```python3
+from bodosdk.models import WorkspaceKeys, ModifyCluster, ClusterResponse
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    auto_pause=60,
+    auto_shutdown=0,
+    workers_quantity=4,
+    description="using the SDK"
+)
+partial_modify_cluster = ModifyCluster(
+    uuid=<cluster-uuid>,
+    autopause=120,
+)
+new_cluster: List[ClusterResponse] = client.cluster.modify(modify_cluster)
+new_cluster_partial: List[ClusterResponse] = client.cluster.modify(partial_modify_cluster)
+```
 
 ### Workspace resource<a id="workspace-resource"></a>
 Module responsible for managing workspaces in an organization.
 
 - [workspace getting started](#workspace-getting-started)
 - [create workspace](#create-workspace)
 - [list workspaces](#list-workspaces)
@@ -1316,9 +1327,7 @@
 keys = WorkspaceKeys(
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 secret_info: SecretInfo = client.secrets.remove("<secret-uuid>")
 ```
-
-
```

### Comparing `bodosdk-1.2.9/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.3.0/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/setup.py` & `bodosdk-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.9/versioneer.py` & `bodosdk-1.3.0/versioneer.py`

 * *Files identical despite different names*

