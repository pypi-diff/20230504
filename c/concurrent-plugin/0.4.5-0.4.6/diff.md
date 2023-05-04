# Comparing `tmp/concurrent_plugin-0.4.5-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 30346 bytes, number of entries: 17
+Zip file size: 30411 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx        2 b- defN 22-Dec-14 21:27 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    31832 b- defN 23-Apr-27 01:05 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    32381 b- defN 23-May-04 12:20 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-14 21:27 concurrent_plugin/concurrent_core.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Apr-27 01:05 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 23-Apr-27 01:05 concurrent_plugin/periodic_run.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 22-Dec-14 21:27 concurrent_plugin/infinfs/mount_main.py
 -rw-rw-r--  2.0 unx    15402 b- defN 23-Apr-28 07:15 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      268 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx      181 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1567 b- defN 23-Apr-28 14:01 concurrent_plugin-0.4.5.dist-info/RECORD
-17 files, 105513 bytes uncompressed, 27712 bytes compressed:  73.7%
+-rw-rw-r--  2.0 unx      268 b- defN 23-May-04 12:21 concurrent_plugin-0.4.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-04 12:21 concurrent_plugin-0.4.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-04 12:21 concurrent_plugin-0.4.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-May-04 12:21 concurrent_plugin-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1567 b- defN 23-May-04 12:21 concurrent_plugin-0.4.6.dist-info/RECORD
+17 files, 106062 bytes uncompressed, 27777 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.4.5.dist-info/METADATA
+Filename: concurrent_plugin-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.4.5.dist-info/WHEEL
+Filename: concurrent_plugin-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.4.5.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.4.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.5.dist-info/top_level.txt
+Filename: concurrent_plugin-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.5.dist-info/RECORD
+Filename: concurrent_plugin-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -312,14 +312,22 @@
                 body['resources.limits.nvidia.com/gpu'] = backend_config['resources.limits.nvidia.com/gpu']
             if "resources.requests.cpu" in backend_config:
                 body['resources.requests.cpu'] = backend_config['resources.requests.cpu']
             if "resources.requests.memory" in backend_config:
                 body['resources.requests.memory'] = backend_config['resources.requests.memory']
             if "resources.requests.hugepages" in backend_config:
                 body['resources.requests.hugepages'] = backend_config['resources.requests.hugepages']
+            if "resources.requests.ephemeral-storage" in backend_config:
+                body['resources.requests.ephemeral-storage'] = backend_config['resources.requests.ephemeral-storage']
+            else:
+                body['resources.requests.ephemeral-storage'] = '8Gi'
+            if "resources.limits.ephemeral-storage" in backend_config:
+                body['resources.limits.ephemeral-storage'] = backend_config['resources.limits.ephemeral-storage']
+            else:
+                body['resources.limits.ephemeral-storage'] = '10Gi'
             if "resources.requests.nvidia.com/gpu" in backend_config:
                 body['resources.requests.nvidia.com/gpu'] = backend_config['resources.requests.nvidia.com/gpu']
             if 'kube-namespace' in backend_config:
                 body['namespace'] = backend_config['kube-namespace']
             else:
                 body['namespace'] = 'default'
         kube_context = backend_config.get('kube-context')
```

## Comparing `concurrent_plugin-0.4.5.dist-info/RECORD` & `concurrent_plugin-0.4.6.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=iIeT_QfncYXoIxuyD76M_kBCb1jUOXGRcK1ls57KtQE,31832
+concurrent_plugin/concurrent_backend.py,sha256=oH1MZSiYPJiwRgY2kLg16CynjXX9cX7nu9mUHsxG_I4,32381
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
 concurrent_plugin/infinfs/mount_service.py,sha256=6dCIqKUzlmR_kDWu67ax5Gbga503AD429RrueacIFOE,15402
-concurrent_plugin-0.4.5.dist-info/METADATA,sha256=ic_lXGzALGwSpAcG2f12-D7sAvIl2nBquNJmiP4kQd8,268
-concurrent_plugin-0.4.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.4.5.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
-concurrent_plugin-0.4.5.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.4.5.dist-info/RECORD,,
+concurrent_plugin-0.4.6.dist-info/METADATA,sha256=8aK64sfYNY1SYTAbLBZAtIZX7FOHMRDXRAPotcr59bo,268
+concurrent_plugin-0.4.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.4.6.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
+concurrent_plugin-0.4.6.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.4.6.dist-info/RECORD,,
```

