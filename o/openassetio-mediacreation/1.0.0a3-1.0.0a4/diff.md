# Comparing `tmp/openassetio_mediacreation-1.0.0a3-py3-none-any.whl.zip` & `tmp/openassetio_mediacreation-1.0.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 12065 bytes, number of entries: 11
--rw-r--r--  2.0 unx      188 b- defN 22-Dec-14 11:11 openassetio_mediacreation/__init__.py
--rw-r--r--  2.0 unx     5125 b- defN 22-Dec-14 11:11 openassetio_mediacreation/traits.yml
--rw-r--r--  2.0 unx      222 b- defN 22-Dec-14 11:11 openassetio_mediacreation/traits/__init__.py
--rw-r--r--  2.0 unx     1799 b- defN 22-Dec-14 11:11 openassetio_mediacreation/traits/content.py
--rw-r--r--  2.0 unx     3858 b- defN 22-Dec-14 11:11 openassetio_mediacreation/traits/managementPolicy.py
--rw-r--r--  2.0 unx     2266 b- defN 22-Dec-14 11:11 openassetio_mediacreation/traits/timeline.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Dec-14 11:11 openassetio_mediacreation-1.0.0a3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1447 b- defN 22-Dec-14 11:11 openassetio_mediacreation-1.0.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-14 11:11 openassetio_mediacreation-1.0.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 22-Dec-14 11:11 openassetio_mediacreation-1.0.0a3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1083 b- defN 22-Dec-14 11:11 openassetio_mediacreation-1.0.0a3.dist-info/RECORD
-11 files, 27463 bytes uncompressed, 10177 bytes compressed:  62.9%
+Zip file size: 13687 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      188 b- defN 23-May-04 14:06 openassetio_mediacreation/__init__.py
+-rw-r--r--  2.0 unx     6511 b- defN 23-May-04 14:06 openassetio_mediacreation/traits.yml
+-rw-r--r--  2.0 unx      245 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/__init__.py
+-rw-r--r--  2.0 unx     1799 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/content.py
+-rw-r--r--  2.0 unx     3695 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/identity.py
+-rw-r--r--  2.0 unx     3858 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/managementPolicy.py
+-rw-r--r--  2.0 unx     2266 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/timeline.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1435 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1184 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/RECORD
+12 files, 32656 bytes uncompressed, 11635 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: openassetio_mediacreation/traits/__init__.py
 Comment: 
 
 Filename: openassetio_mediacreation/traits/content.py
 Comment: 
 
+Filename: openassetio_mediacreation/traits/identity.py
+Comment: 
+
 Filename: openassetio_mediacreation/traits/managementPolicy.py
 Comment: 
 
 Filename: openassetio_mediacreation/traits/timeline.py
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a3.dist-info/LICENSE
+Filename: openassetio_mediacreation-1.0.0a4.dist-info/LICENSE
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a3.dist-info/METADATA
+Filename: openassetio_mediacreation-1.0.0a4.dist-info/METADATA
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a3.dist-info/WHEEL
+Filename: openassetio_mediacreation-1.0.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a3.dist-info/top_level.txt
+Filename: openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a3.dist-info/RECORD
+Filename: openassetio_mediacreation-1.0.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openassetio_mediacreation/traits.yml

```diff
@@ -69,14 +69,51 @@
             type: string
             description: >
               The location of the entities external content.
 
 
               This must be a valid URL so special characters need to
               be encoded.
+  identity:
+    description: Traits that aid identification of an entity
+    members:
+      DisplayName:
+        description: >
+          Names that can be presented to a user in order to identify
+          and/or disambiguate the entity. These strings are potentially
+          unstable and should not be used as a UUID or other persistent
+          anchor.
+        usage:
+          - entity
+        properties:
+          name:
+            type: string
+            description: |
+              The humanized name of entity itself, not including any
+              hierarchy or classification.
+
+              For example:
+              - `"Cuttlefish v1"` - for a version of an asset
+              - `"seq003"` - for a sequence in a hierarchy
+
+          qualifiedName:
+            type: string
+            description: |
+              An unambiguous, humanised name for the entity.
+
+              The display name may want to consider the host, and any other
+              relevant Context information to form a display name for an
+              entity that can uniquely identify the entity in that context.
+
+              For example:
+              - `"dive / build / cuttlefish / model / v1"` for a version
+                  of an asset in an 'open recent' menu.
+              - `"Sequence 003 [ Dive / Episode 1 ]"` for a sequence in
+                 an hierarchy as a window title.
+
 
   managementPolicy:
     description: Traits used in a Manager's managementPolicy response.
     members:
       Managed:
         description: >
           A trait indicating that the data matching the supplied trait set
```

## openassetio_mediacreation/traits/__init__.py

```diff
@@ -1,9 +1,10 @@
 """
 Traits defined in the 'openassetio-mediacreation' package.
 """
 
 # WARNING: This file is auto-generated by openassetio-traitgen, do not edit.
 
 from . import content
+from . import identity
 from . import managementPolicy
 from . import timeline
```

## Comparing `openassetio_mediacreation-1.0.0a3.dist-info/LICENSE` & `openassetio_mediacreation-1.0.0a4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openassetio_mediacreation-1.0.0a3.dist-info/METADATA` & `openassetio_mediacreation-1.0.0a4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassetio-mediacreation
-Version: 1.0.0a3
+Version: 1.0.0a4
 Author-email: Contributors to the OpenAssetIO project <openassetio-discussion@lists.aswf.io>
 Project-URL: OpenAssetIO, https://github.com/OpenAssetIO/OpenAssetIO
 Project-URL: Source, https://github.com/OpenAssetIO/OpenAssetIO-MediaCreation
 Project-URL: Issues, https://github.com/OpenAssetIO/OpenAssetIO-MediaCreation/issues
 Keywords: openassetio,mediacreation,trait
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,8 +25,8 @@
 OpenAssetIO extensions for use in Media Creation
 
 > Note: This repository is currently in a pre-alpha state, and so should
 > not be used for any production critical applications.
 
 Included are several well-known Traits and Specifications for use in
 OpenAssetIO hosts and managers. For more information on this mechanism,
-see the [OpenAssetIO docs](https://thefoundryvisionmongers.github.io/OpenAssetIO/).
+see the [OpenAssetIO docs](https://openassetio.github.io/OpenAssetIO/).
```

## Comparing `openassetio_mediacreation-1.0.0a3.dist-info/RECORD` & `openassetio_mediacreation-1.0.0a4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 openassetio_mediacreation/__init__.py,sha256=b36NTLJZmYaj3l4k8veMMRaPokuvK14r8uNPrzQHgDM,188
-openassetio_mediacreation/traits.yml,sha256=BFYDgvKOLPA4_NDplkdTPYG0Dt3pklf3VawLFsUYIVg,5125
-openassetio_mediacreation/traits/__init__.py,sha256=jR7P-WXH_LxZenCMPhmrr19zSOrrdr7jr32wgqhy6Cc,222
+openassetio_mediacreation/traits.yml,sha256=pVElMrhNQC-sHZMPbbjTsjzAf9llok7ieTJoZnglovY,6511
+openassetio_mediacreation/traits/__init__.py,sha256=8saXUuM5QygSsob839NLYrMDY95t0GUvkmmecgVFTlM,245
 openassetio_mediacreation/traits/content.py,sha256=iXirrok8GUdDjUJzB_HSYj4wcgpmYv7YmCGzgM_XcfI,1799
+openassetio_mediacreation/traits/identity.py,sha256=SEFLRoVz5EtA1FOQcTbYG4WUug1iFXOHlzyhQuxIVeQ,3695
 openassetio_mediacreation/traits/managementPolicy.py,sha256=L1-2ZQmEjurdK1HqwMQjUZ3tHRaqm4t388a1lw2ejfo,3858
 openassetio_mediacreation/traits/timeline.py,sha256=rBy_oMEjtJGvoLWfoRGPobEHvjxgulp7RDDDn5m2SzY,2266
-openassetio_mediacreation-1.0.0a3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-openassetio_mediacreation-1.0.0a3.dist-info/METADATA,sha256=0WRLCb22nLFgx1k8o-k75Txm1jgkX2YgEcDIVtYz1iM,1447
-openassetio_mediacreation-1.0.0a3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openassetio_mediacreation-1.0.0a3.dist-info/top_level.txt,sha256=6wrwB2f-cI98-MIfAnoKwTFdaYJQv206KEx50rAT7D0,26
-openassetio_mediacreation-1.0.0a3.dist-info/RECORD,,
+openassetio_mediacreation-1.0.0a4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+openassetio_mediacreation-1.0.0a4.dist-info/METADATA,sha256=ZPtwS01GmZpFnXYI3302GrGeiPru1vYhcvKNTu-zF1U,1435
+openassetio_mediacreation-1.0.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt,sha256=6wrwB2f-cI98-MIfAnoKwTFdaYJQv206KEx50rAT7D0,26
+openassetio_mediacreation-1.0.0a4.dist-info/RECORD,,
```

