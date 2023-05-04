# Comparing `tmp/ovos_stt_plugin_server-0.0.3-py3-none-any.whl.zip` & `tmp/ovos_stt_plugin_server-0.0.3a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9299 bytes, number of entries: 9
--rw-r--r--  2.0 unx     7339 b- defN 23-May-04 14:46 ovos_stt_plugin_server/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-May-04 14:46 ovos_stt_plugin_server/version.py
--rw-r--r--  2.0 unx    11343 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1652 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      278 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      854 b- defN 23-May-04 14:46 ovos_stt_plugin_server-0.0.3.dist-info/RECORD
-9 files, 21759 bytes uncompressed, 7787 bytes compressed:  64.2%
+Zip file size: 9336 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     7339 b- defN 23-May-04 14:45 ovos_stt_plugin_server/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-May-04 14:45 ovos_stt_plugin_server/version.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1654 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      278 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD
+9 files, 21775 bytes uncompressed, 7796 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_stt_plugin_server/__init__.py
 Comment: 
 
 Filename: ovos_stt_plugin_server/version.py
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/LICENSE
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/METADATA
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/WHEEL
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/entry_points.txt
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/top_level.txt
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/zip-safe
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3.dist-info/RECORD
+Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_stt_plugin_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 3
-VERSION_ALPHA = 0
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_stt_plugin_server-0.0.3.dist-info/LICENSE` & `ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_stt_plugin_server-0.0.3.dist-info/METADATA` & `ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-plugin-server
-Version: 0.0.3
+Version: 0.0.3a2
 Summary: ovos stt server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin stt
 Platform: UNKNOWN
```

## Comparing `ovos_stt_plugin_server-0.0.3.dist-info/RECORD` & `ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ovos_stt_plugin_server/__init__.py,sha256=u-r0X0RL8lScF3Nbxzyfg-kCBAJsar9chPVz69hmsmw,7339
-ovos_stt_plugin_server/version.py,sha256=X2CYWfGoY1aNmDex4N_vNwEZzxv6fwcrc6sz_dkgn4Y,177
-ovos_stt_plugin_server-0.0.3.dist-info/LICENSE,sha256=M9sXAhWHy6YjXEeyFSN_YfpvOMVPbVa1PLyadopawAY,11343
-ovos_stt_plugin_server-0.0.3.dist-info/METADATA,sha256=Lc8pbVN8DjL6LOn6KmxjY5I3dYJJGmlQp2W4XGxKeZk,1652
-ovos_stt_plugin_server-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_stt_plugin_server-0.0.3.dist-info/entry_points.txt,sha256=tRhDlbaFzDlXQr7eb1ylkLQ16qQisWyzyHyTPJmWdpM,278
-ovos_stt_plugin_server-0.0.3.dist-info/top_level.txt,sha256=xYXEI1jyZ75hmVvJRKlb3xTJQkj90aIMWljfLKuW5No,23
-ovos_stt_plugin_server-0.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_stt_plugin_server-0.0.3.dist-info/RECORD,,
+ovos_stt_plugin_server/version.py,sha256=WOoCeelQ8hsh3tlEpOt7Dn1yIpKGXKPTCvd8ILMk3Ck,177
+ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE,sha256=M9sXAhWHy6YjXEeyFSN_YfpvOMVPbVa1PLyadopawAY,11343
+ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA,sha256=v2YyvbTosnk-vjXCveJNaSMJxMepvEy5rYMD3JCX2GU,1654
+ovos_stt_plugin_server-0.0.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_stt_plugin_server-0.0.3a2.dist-info/entry_points.txt,sha256=tRhDlbaFzDlXQr7eb1ylkLQ16qQisWyzyHyTPJmWdpM,278
+ovos_stt_plugin_server-0.0.3a2.dist-info/top_level.txt,sha256=xYXEI1jyZ75hmVvJRKlb3xTJQkj90aIMWljfLKuW5No,23
+ovos_stt_plugin_server-0.0.3a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD,,
```

