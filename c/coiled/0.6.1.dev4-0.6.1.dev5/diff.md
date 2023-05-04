# Comparing `tmp/coiled-0.6.1.dev4.tar.gz` & `tmp/coiled-0.6.1.dev5.tar.gz`

## Comparing `coiled-0.6.1.dev4.tar` & `coiled-0.6.1.dev5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_version.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/context.py
--rw-r--r--   0        0        0   111441 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/exceptions.py
--rw-r--r--   0        0        0    19208 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/software.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/types.py
--rw-r--r--   0        0        0    47497 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    83463 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    59978 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/README.md
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/pyproject.toml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 coiled-0.6.1.dev4/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_version.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/context.py
+-rw-r--r--   0        0        0   112046 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/exceptions.py
+-rw-r--r--   0        0        0    19208 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/magic.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/software.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/types.py
+-rw-r--r--   0        0        0    47640 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    84970 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    60439 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 coiled-0.6.1.dev5/PKG-INFO
```

### Comparing `coiled-0.6.1.dev4/coiled/__init__.py` & `coiled-0.6.1.dev5/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/analytics.py` & `coiled-0.6.1.dev5/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cluster.py` & `coiled-0.6.1.dev5/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/coiled.yaml` & `coiled-0.6.1.dev5/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/context.py` & `coiled-0.6.1.dev5/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/core.py` & `coiled-0.6.1.dev5/coiled/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1195,14 +1195,15 @@
         backend: Optional[str] = None,
         min_cores: Optional[int] = None,
         min_gpus: Optional[int] = None,
         min_memory: Optional[Union[int, str, float]] = None,
         cores: Optional[Union[int, List[int]]] = None,
         memory: Optional[Union[int, float, str, List[int], List[str], List[float]]] = None,
         gpus: Optional[Union[int, List[int]]] = None,
+        arch: Optional[Literal["x86_64", "arm64"]] = None,
     ) -> Dict[str, VmType]:
         if backend:
             user_provider = backend
         else:
             user_provider = await self.get_account_provider_name(account=self.default_account)
 
         if user_provider and user_provider not in ALLOWED_PROVIDERS:
@@ -1215,14 +1216,15 @@
             min_cores=min_cores,
             min_gpus=min_gpus,
             min_memory=min_memory,
             cores=cores,
             memory=memory,
             gpus=gpus,
             backend=user_provider.lower(),
+            arch=arch,
         )
 
         return {f"{name}": i for name, i in all_instance_types.items()}
 
     @delete_docstring
     def set_gcp_credentials(
         self: CloudSyncAsync,
@@ -1307,14 +1309,15 @@
         min_cores: Optional[int] = None,
         min_gpus: Optional[int] = None,
         min_memory: Optional[Union[int, str, float]] = None,
         cores: Optional[Union[int, List[int]]] = None,
         memory: Optional[Union[int, str, float, List[int], List[str], List[float]]] = None,
         gpus: Optional[Union[int, List[int]]] = None,
         backend: Optional[str] = None,
+        arch: Optional[Literal["x86_64", "arm64"]] = None,
     ) -> Tuple[dict, Optional[str]]:
         parsed_memory = parse_requested_memory(memory, min_memory)
         params = {"page": page, **parsed_memory}
 
         # This isn't particularly pretty, but we are handling the case
         # where users specify a range for cores/memory/gpus or an exact
         # match
@@ -1335,14 +1338,17 @@
 
         if min_gpus:
             params["gpus__gte"] = min_gpus
 
         if backend:
             params["backend_type"] = backend if backend.startswith("vm_") else f"vm_{backend}"
 
+        if arch:
+            params["arch"] = arch
+
         response = await self._do_request(
             "GET",
             f"{self.server}/api/v1/vm-types/",
             params=params,
         )
 
         if response.status == 200:
@@ -1533,27 +1539,29 @@
         backend: Optional[str],
         min_cores: Optional[int],
         min_gpus: Optional[int],
         min_memory: Optional[Union[int, str, float]],
         cores: Optional[Union[int, List[int]]],
         memory: Optional[Union[int, str, float, List[int], List[str], List[float]]],
         gpus: Optional[Union[int, List[int]]],
+        arch: Optional[Literal["x86_64", "arm64"]] = None,
     ) -> Dict[str, VmType]:
         ...
 
     @overload
     def list_instance_types(
         self: Cloud[Async],
         backend: Optional[str],
         min_cores: Optional[int],
         min_gpus: Optional[int],
         min_memory: Optional[Union[int, str, float]],
         cores: Optional[Union[int, List[int]]],
         memory: Optional[Union[int, str, float, List[int], List[str], List[float]]],
         gpus: Optional[Union[int, List[int]]],
+        arch: Optional[Literal["x86_64", "arm64"]] = None,
     ) -> Awaitable[Dict[str, VmType]]:
         ...
 
     def list_instance_types(
         self: CloudSyncAsync,
         backend: Optional[str] = None,
         min_cores: Optional[int] = None,
@@ -1563,24 +1571,26 @@
         memory: Optional[Union[int, str, float, List[int], List[str], List[float]]] = None,
         gpus: Optional[
             Union[
                 int,
                 List[int],
             ]
         ] = None,
+        arch: Optional[Literal["x86_64", "arm64"]] = None,
     ) -> Union[Awaitable[Dict[str, VmType]], Dict[str, VmType]]:
         return self._sync(
             self._list_instance_types,
             backend=backend,
             min_cores=min_cores,
             min_gpus=min_gpus,
             min_memory=min_memory,
             cores=cores,
             memory=memory,
             gpus=gpus,
+            arch=arch,
         )
 
     @overload
     def list_gpu_types(self: Cloud[Sync]) -> dict:
         ...
 
     @overload
@@ -3012,14 +3022,15 @@
     backend: Optional[str] = None,
     min_cores: Optional[int] = None,
     min_gpus: Optional[int] = None,
     min_memory: Optional[Union[int, str, float]] = None,
     cores: Optional[Union[int, List[int]]] = None,
     memory: Optional[Union[int, str, float, List[int], List[str], List[float]]] = None,
     gpus: Optional[Union[int, List[int]]] = None,
+    arch: Optional[Literal["x86_64", "arm64"]] = None,
 ) -> Dict[str, VmType]:
     """List allowed instance types for the cloud provider configured on your account.
 
     This command allows you to get all instance types available for a backend or a filtered
     list of instance types that match your requirements by using the available keyword
     arguments. Please refer to :doc:`tutorials/select_instance_types` for more information.
 
@@ -3037,26 +3048,30 @@
     cores:
         The exact number of cores to filter for example ``cores=1`` or a list containg the
         minimum and maximum amount of cores to filter instances by, for example ``cores=[2,8]``.
     memory:
         The exact amount of memory or a list containing the minimum and maximum
         amount of memory to filter instances by.
     gpus
-        The exaxct number of gpus to filter or a list containing the minimum and maximum number
+        The exact number of gpus to filter or a list containing the minimum and maximum number
         of GPUS to filter instances by.
+    arch
+        CPU architecture, defaults to x86_64. There's no way to get both x86_64 and arm64
+        instances in a single call.
     """
     with Cloud() as cloud:
         return cloud.list_instance_types(
             backend=backend,
             min_cores=min_cores,
             min_gpus=min_gpus,
             min_memory=min_memory,
             cores=cores,
             memory=memory,
             gpus=gpus,
+            arch=arch,
         )
 
 
 def list_gpu_types() -> Dict:
     """List allowed GPU Types.
 
     For AWS the GPU types are tied to the instance type, but for GCP you can
```

### Comparing `coiled-0.6.1.dev4/coiled/exceptions.py` & `coiled-0.6.1.dev5/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/magic.py` & `coiled-0.6.1.dev5/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/scan.py` & `coiled-0.6.1.dev5/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/software.py` & `coiled-0.6.1.dev5/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/types.py` & `coiled-0.6.1.dev5/coiled/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,7 +192,14 @@
 
     @property
     def conda_suffix(self) -> str:
         if self == ArchitectureTypesEnum.X86_64:
             return "64"
         else:
             return self.value
+
+    @property
+    def vm_arch(self) -> Literal["x86_64", "arm64"]:
+        if self == ArchitectureTypesEnum.ARM64:
+            return "arm64"
+        else:
+            return self.value
```

### Comparing `coiled-0.6.1.dev4/coiled/utils.py` & `coiled-0.6.1.dev5/coiled/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 import backoff
 from packaging.version import Version
 
 from coiled.context import get_datadog_trace_link, track_context
 
 if sys.version_info >= (3, 8):
-    from typing import Type, TypedDict, get_args, get_origin, get_type_hints
+    from typing import Literal, Type, TypedDict, get_args, get_origin, get_type_hints
 else:
-    from typing_extensions import Type, TypedDict, get_args, get_origin, get_type_hints
+    from typing_extensions import Literal, Type, TypedDict, get_args, get_origin, get_type_hints
 
 import aiohttp
 import boto3
 import click
 import dask
 import rich
 import urllib3
@@ -69,18 +69,18 @@
 ALLOWED_PROVIDERS = ["aws", "vm_aws", "gcp", "vm_gcp"]
 
 COILED_LOGGER_NAME = "coiled"
 COILED_SERVER = "https://cloud.coiled.io"
 COILED_RUNTIME_REGEX = re.compile(r"^coiled/coiled-runtime-(?P<version>\d+\-\d+\-\d+)-*")
 
 # Dots after family names ensure we do not match t3a or other variants
-AWS_BALANCED_INSTANCES_FAMILY_FILTER = ("t2.", "t3.", "m5.", "m6i.")
+AWS_BALANCED_INSTANCES_FAMILY_FILTER = ("t2.", "t3.", "m5.", "m6i.", "t4g.", "m6g.", "m7g.")
 AWS_INSTANCES_FAMILY_FILTER = AWS_BALANCED_INSTANCES_FAMILY_FILTER  # deprecated
 AWS_GPU_INSTANCE_FAMILIES_FILTER = ("g4dn",)
-AWS_UNBALANCED_INSTANCE_FAMILIES_FILTER = ("c5.", "c6i.", "r6i.")
+AWS_UNBALANCED_INSTANCE_FAMILIES_FILTER = ("c5.", "c6i.", "r6i.", "c7g.", "r7g.")
 
 GCP_SCHEDULER_GPU = {
     "scheduler_accelerator_type": "nvidia-tesla-t4",
     "scheduler_accelerator_count": 1,
 }
 
 
@@ -1072,14 +1072,15 @@
 
 @track_context
 def get_instance_type_from_cpu_memory(
     cpu: Optional[Union[int, List[int]]] = None,
     memory: Optional[Union[int, str, float, List[int], List[str], List[float]]] = None,
     gpus: Optional[int] = None,
     backend: Optional[str] = None,
+    arch: Literal["x86_64", "arm64"] = "x86_64",
 ) -> List[str]:
     """Get instances by cpu/memory combination.
 
     We are using the `list_instance_types` method to get the
     instances that match the cpu/memory specification. If no
     instance can be found we will raise an exception
     informing the user about this.
@@ -1088,32 +1089,32 @@
     # Circular imports
     from .core import list_instance_types
 
     if backend == "gcp":
         instance_family = "n1" if gpus else "e2"
         instances = [
             instance_name
-            for instance_name in list_instance_types(cores=cpu, memory=memory, backend=backend)
+            for instance_name in list_instance_types(cores=cpu, memory=memory, backend=backend, arch=arch)
             if instance_name.startswith(instance_family)
         ]
     else:
-        instance_types = list_instance_types(cores=cpu, memory=memory, backend=backend, gpus=gpus)
+        instance_types = list_instance_types(cores=cpu, memory=memory, backend=backend, gpus=gpus, arch=arch)
 
         aws_family_filter = AWS_BALANCED_INSTANCES_FAMILY_FILTER
         if gpus:
             aws_family_filter = AWS_GPU_INSTANCE_FAMILIES_FILTER
         elif cpu and memory:
             aws_family_filter += AWS_UNBALANCED_INSTANCE_FAMILIES_FILTER
 
         instances = [instance_name for instance_name in instance_types if instance_name.startswith(aws_family_filter)]
 
     if not instances:
         error_message = (
             "Unable to find instance types that match the specification: \n"
-            f"\t Cores: {cpu}  Memory: {memory} GPUs: {gpus}\n"
+            f"\t Cores: {cpu}  Memory: {memory} GPUs: {gpus}  Arch: {arch}\n"
         )
 
         if cpu or memory:
             error_message += (
                 "You can try selecting a range for the cpu or memory, for example: "
                 "`cpu=[2, 8]` or `memory=['32Gb','64Gb'] \n"
             )
```

### Comparing `coiled-0.6.1.dev4/coiled/websockets.py` & `coiled-0.6.1.dev5/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/_beta/cluster.py` & `coiled-0.6.1.dev5/coiled/_beta/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,16 @@
         Start a Jupyter server in the same process as Dask scheduler. The Jupyter server will be behind HTTPS
         with authentication (unless you disable ``use_dashboard_https``, which we strongly recommend against).
         Note that ``jupyterlab`` will need to be installed in the software environment used on the cluster
         (or in your local environment if using package sync).
         Once the cluster is running, you can use ``jupyter_link`` to get link to access the Jupyter server.
     region:
         The cloud provider region in which to run the cluster.
+    arm:
+        Use ARM instances for cluster; default is x86 (Intel) instances.
     """
 
     _instances = weakref.WeakSet()
 
     def __init__(
         self: ClusterSyncAsync,
         name: Optional[str] = None,
@@ -323,14 +325,15 @@
         # easier network config
         scheduler_port: Optional[int] = None,
         allow_ingress_from: Optional[str] = None,
         allow_ssh: Optional[bool] = None,
         new_build_backend: bool = False,
         jupyter: Optional[bool] = None,
         region: Optional[str] = None,
+        arm: Optional[bool] = None,
     ):
         # NOTE:
         # this attribute is only updated while we wait for cluster to come up
         self.errored_worker_count: int = 0
         self.init_time = datetime.datetime.now()
         type(self)._instances.add(self)
         self.new_build_backend = new_build_backend
@@ -343,14 +346,16 @@
             self.package_sync_only = set(package_sync)
             self.package_sync_only.add("python")
         else:
             self.package_sync_only = None
         self.package_sync_strict = package_sync_strict
         self.package_sync_fail_on = BEHAVIOR_TO_LEVEL[package_sync_fail_on]
         self.show_widget = show_widget
+        self.arch = ArchitectureTypesEnum.ARM64 if arm else ArchitectureTypesEnum.X86_64
+
         self._cluster_status_logs = []
 
         if region is not None:
             if backend_options is None:
                 backend_options = {}
             # backend_options supports both `region` and `region_name` (for backwards compatibility
             # since we changed it at some point).
@@ -629,14 +634,15 @@
         if (self.worker_cpu or self.worker_memory) and not self.worker_vm_types:
             # match worker types by cpu and/or memory
             worker_vm_types_to_use = get_instance_type_from_cpu_memory(
                 self.worker_cpu,
                 self.worker_memory,
                 gpus=self.worker_gpu_count,
                 backend=await self._get_account_cloud_provider_name(),
+                arch=self.arch.vm_arch,
             )
         elif (self.worker_cpu or self.worker_memory) and self.worker_vm_types:
             raise ArgumentCombinationError(_vm_type_cpu_memory_error_msg.format(kind="worker"))
         else:
             # get default types from dask config
             if self.worker_vm_types is None:
                 self.worker_vm_types = dask.config.get("coiled.worker.vm-types")
@@ -649,14 +655,15 @@
         if (self.scheduler_cpu or self.scheduler_memory) and not self.scheduler_vm_types:
             # match scheduler types by cpu and/or memory
             scheduler_vm_types_to_use = get_instance_type_from_cpu_memory(
                 self.scheduler_cpu,
                 self.scheduler_memory,
                 gpus=1 if self.scheduler_gpu else 0,
                 backend=await self._get_account_cloud_provider_name(),
+                arch=self.arch.vm_arch,
             )
         elif (self.scheduler_cpu or self.scheduler_memory) and self.scheduler_vm_types:
             raise ArgumentCombinationError(_vm_type_cpu_memory_error_msg.format(kind="scheduler"))
         else:
             # get default types from dask config
             if self.scheduler_vm_types is None:
                 self.scheduler_vm_types = dask.config.get("coiled.scheduler.vm_types")
@@ -671,28 +678,31 @@
             provider = await self._get_account_cloud_provider_name()
 
             if not self.scheduler_gpu and not self.worker_gpu_count:
                 # When no GPUs, us same default for scheduler and workers
                 default_vm_types = await cloud._get_default_instance_types(
                     provider=provider,
                     gpu=False,
+                    arch=self.arch.vm_arch,
                 )
                 scheduler_vm_types_to_use = scheduler_vm_types_to_use or default_vm_types
                 worker_vm_types_to_use = worker_vm_types_to_use or default_vm_types
             else:
                 # GPUs so there might be different defaults for scheduler/workers
                 if not scheduler_vm_types_to_use:
                     scheduler_vm_types_to_use = await cloud._get_default_instance_types(
                         provider=provider,
                         gpu=self.scheduler_gpu,
+                        arch=self.arch.vm_arch,
                     )
                 if not worker_vm_types_to_use:
                     worker_vm_types_to_use = await cloud._get_default_instance_types(
                         provider=provider,
                         gpu=bool(self.worker_gpu_count),
+                        arch=self.arch.vm_arch,
                     )
 
         return scheduler_vm_types_to_use, worker_vm_types_to_use
 
     @track_context
     async def _get_account_cloud_provider_name(self) -> str:
         if not hasattr(self, "_cached_account_cloud_provider_name"):
@@ -969,14 +979,29 @@
                             re.search(r"^\w+\d.*g.*", vm_type.split(".")[0], flags=re.IGNORECASE)
                             for vm_type in chain(scheduler_vm_types_to_use, worker_vm_types_to_use)
                         )
                     )
                     else ArchitectureTypesEnum.X86_64
                 )
 
+                # `architecture` is set to ARM64 iff *all* instances are ARM,
+                # so when architecture is X86_64 that could mean all instances are x86
+                # or it could mean that there's a mix (which we want to reject).
+                if architecture == ArchitectureTypesEnum.ARM64:
+                    self.arch = ArchitectureTypesEnum.ARM64
+
+                # This check ensures that if the user asked for ARM cluster (using the `arm` kwarg),
+                # then they didn't also explicitly specify x86 instance type.
+                # (It also catches if our code to pick ARM instances types returns an x86 instance type.)
+                if architecture != self.arch:
+                    # TODO (future PR) more specific error about which instance type doesn't match
+                    raise RuntimeError(
+                        f"Requested cluster architecture ({self.arch.vm_arch}) does not match "
+                        f"architecture of some instance types ({scheduler_vm_types_to_use}, {worker_vm_types_to_use})."
+                    )
                 if platform.machine() == architecture and platform.system() == "Linux":
                     self.package_sync_strict = True
 
                 senv_v2_id = await self._determine_senv(
                     architecture=architecture,
                 )
                 self.cluster_id = await cloud._create_cluster(
```

### Comparing `coiled-0.6.1.dev4/coiled/_beta/core.py` & `coiled-0.6.1.dev5/coiled/_beta/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,21 +241,30 @@
                 return cls(asynchronous=True)
             else:
                 return cls(asynchronous=False)
         else:
             return cloud
 
     @track_context
-    async def _get_default_instance_types(self, provider: str, gpu: bool = False) -> List[str]:
+    async def _get_default_instance_types(self, provider: str, gpu: bool = False, arch: str = "x86_64") -> List[str]:
+        if arch not in ("arm64", "x86_64"):
+            raise ValueError(f"arch '{arch}' is not supported for default instance types")
         if provider == "aws":
+            if arch == "arm64":
+                if gpu:
+                    return ["g5g.xlarge"]
+                else:
+                    return ["m7g.xlarge", "t4g.xlarge"]
             if gpu:
                 return ["g4dn.xlarge"]
             else:
                 return ["m6i.xlarge", "t3.xlarge"]
         elif provider == "gcp":
+            if arch != "x86_64":
+                raise ValueError(f"no default instance type for GCP with {arch} architecture")
             if gpu:
                 # n1-standard-8 with 30GB of memory might be best, but that's big for a default
                 return ["n1-standard-4"]
             else:
                 return ["e2-standard-4"]
         else:
             raise ValueError(f"unexpected provider {provider}; cannot determine default instance types")
```

### Comparing `coiled-0.6.1.dev4/coiled/_beta/cwi_log_link.py` & `coiled-0.6.1.dev5/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/_beta/states.py` & `coiled-0.6.1.dev5/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/_beta/widgets/__init__.py` & `coiled-0.6.1.dev5/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/_beta/widgets/rich.py` & `coiled-0.6.1.dev5/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/_beta/widgets/util.py` & `coiled-0.6.1.dev5/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/config.py` & `coiled-0.6.1.dev5/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/core.py` & `coiled-0.6.1.dev5/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/curl.py` & `coiled-0.6.1.dev5/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/env.py` & `coiled-0.6.1.dev5/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/login.py` & `coiled-0.6.1.dev5/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/package_sync.py` & `coiled-0.6.1.dev5/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/utils.py` & `coiled-0.6.1.dev5/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/cluster/__init__.py` & `coiled-0.6.1.dev5/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/cluster/better_logs.py` & `coiled-0.6.1.dev5/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/cluster/logs.py` & `coiled-0.6.1.dev5/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/cluster/ssh.py` & `coiled-0.6.1.dev5/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/notebook/__init__.py` & `coiled-0.6.1.dev5/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/notebook/notebook.py` & `coiled-0.6.1.dev5/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/__init__.py` & `coiled-0.6.1.dev5/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/amp.py` & `coiled-0.6.1.dev5/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/aws.py` & `coiled-0.6.1.dev5/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/entry.py` & `coiled-0.6.1.dev5/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/gcp.py` & `coiled-0.6.1.dev5/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/cli/setup/prometheus.py` & `coiled-0.6.1.dev5/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/coiled/v2/__init__.py` & `coiled-0.6.1.dev5/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/LICENSE` & `coiled-0.6.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/README.md` & `coiled-0.6.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/pyproject.toml` & `coiled-0.6.1.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.1.dev4/PKG-INFO` & `coiled-0.6.1.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.1.dev4
+Version: 0.6.1.dev5
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.1.dev4 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.1.dev5 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

