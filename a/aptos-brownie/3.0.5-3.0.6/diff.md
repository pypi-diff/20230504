# Comparing `tmp/aptos_brownie-3.0.5-py3-none-any.whl.zip` & `tmp/aptos_brownie-3.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 7757 bytes, number of entries: 5
--rw-r--r--  2.0 unx    37346 b- defN 23-May-04 05:11 aptos_brownie.py
--rw-r--r--  2.0 unx      891 b- defN 23-May-04 05:11 aptos_brownie-3.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 05:11 aptos_brownie-3.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-04 05:11 aptos_brownie-3.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-May-04 05:11 aptos_brownie-3.0.5.dist-info/RECORD
-5 files, 38738 bytes uncompressed, 7019 bytes compressed:  81.9%
+-rw-r--r--  2.0 unx    37345 b- defN 23-May-04 08:00 aptos_brownie.py
+-rw-r--r--  2.0 unx      891 b- defN 23-May-04 08:00 aptos_brownie-3.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 08:00 aptos_brownie-3.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-04 08:00 aptos_brownie-3.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      395 b- defN 23-May-04 08:00 aptos_brownie-3.0.6.dist-info/RECORD
+5 files, 38737 bytes uncompressed, 7019 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aptos_brownie.py
 Comment: 
 
-Filename: aptos_brownie-3.0.5.dist-info/METADATA
+Filename: aptos_brownie-3.0.6.dist-info/METADATA
 Comment: 
 
-Filename: aptos_brownie-3.0.5.dist-info/WHEEL
+Filename: aptos_brownie-3.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: aptos_brownie-3.0.5.dist-info/top_level.txt
+Filename: aptos_brownie-3.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: aptos_brownie-3.0.5.dist-info/RECORD
+Filename: aptos_brownie-3.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aptos_brownie.py

```diff
@@ -569,19 +569,20 @@
             sender=self.account,
             payload=TransactionPayload(payload),
             max_gas_amount=int(max_gas_amount),
             gas_unit_price=int(gas_unit_price)
         )
         try:
             result = self.simulate_submit_bcs_transaction(signed_transaction)
-            if not result[0]["success"]:
-                assert False, result
             if return_types is None:
                 return result
-            elif return_types == "gas":
+            if not result[0]["success"]:
+                assert False, result
+
+            if return_types == "gas":
                 if "gas_used" in result[0]:
                     return result[0]["gas_used"]
             else:
                 changes = []
                 for d in result:
                     if "changes" in d:
                         changes.extend(d["changes"])
```

## Comparing `aptos_brownie-3.0.5.dist-info/METADATA` & `aptos_brownie-3.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-brownie
-Version: 3.0.5
+Version: 3.0.6
 Summary: Aptos Package Tool
 Home-page: https://github.com/OmniBTC/OmniSwap/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

