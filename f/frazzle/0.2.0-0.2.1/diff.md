# Comparing `tmp/frazzle-0.2.0.tar.gz` & `tmp/frazzle-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frazzle-0.2.0.tar", max compression
+gzip compressed data, was "frazzle-0.2.1.tar", max compression
```

## Comparing `frazzle-0.2.0.tar` & `frazzle-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     1134 2023-05-04 16:44:44.712519 frazzle-0.2.0/frazzle/client.py
--rw-r--r--   0        0        0      492 2023-05-04 16:43:57.169326 frazzle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       15 2023-05-04 16:45:06.940554 frazzle-0.2.0/README.md
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 frazzle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-04 16:47:23.012784 frazzle-0.2.1/frazzle/__init__.py
+-rw-r--r--   0        0        0       66 2023-05-04 16:48:25.089104 frazzle-0.2.1/frazzle/__main__.py
+-rw-r--r--   0        0        0     1259 2023-05-04 16:48:13.852312 frazzle-0.2.1/frazzle/client.py
+-rw-r--r--   0        0        0      492 2023-05-04 16:48:35.034491 frazzle-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-05-04 16:45:06.940554 frazzle-0.2.1/README.md
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 frazzle-0.2.1/PKG-INFO
```

### Comparing `frazzle-0.2.0/frazzle/client.py` & `frazzle-0.2.1/frazzle/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import argparse
 import json
 import requests
 
-parser = argparse.ArgumentParser()
-parser.add_argument("course", help="The course number you are taking.")
-parser.add_argument("lab", help="The lab number.")
-parser.add_argument(
-    "part", help="The part number of the assignment to get a hint for.")
-parser.add_argument(
-    "source", help="The name of the source file to get a hint for.")
-parser.add_argument("question", help="The question to ask Prof. Frazzle.")
-
-args = parser.parse_args()
-
-with open(args.source, "r") as f:
-    source = f.read()
-    
-# construct json
-api_request = {
-    "course": int(args.course),
-    "lab": int(args.lab),
-    "part": int(args.part),
-    "code":source,
-    "question": args.question,
-}
-
-cloud_function_url = "https://us-central1-frazzle.cloudfunctions.net/frazzle-hinty"
-headers = {'Content-type': 'application/json', 'Accept': 'text/plain'}
-response = requests.post(cloud_function_url, data=json.dumps(api_request), headers=headers)
-
-if response.status_code == 200:
-    feedback = response.text
-else:
-    feedback = "Error: " + response.text
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("course", help="The course number you are taking.")
+    parser.add_argument("lab", help="The lab number.")
+    parser.add_argument(
+        "part", help="The part number of the assignment to get a hint for.")
+    parser.add_argument(
+        "source", help="The name of the source file to get a hint for.")
+    parser.add_argument("question", help="The question to ask Prof. Frazzle.")
+
+    args = parser.parse_args()
+
+    with open(args.source, "r") as f:
+        source = f.read()
+        
+    # construct json
+    api_request = {
+        "course": int(args.course),
+        "lab": int(args.lab),
+        "part": int(args.part),
+        "code":source,
+        "question": args.question,
+    }
+
+    cloud_function_url = "https://us-central1-frazzle.cloudfunctions.net/frazzle-hinty"
+    headers = {'Content-type': 'application/json', 'Accept': 'text/plain'}
+    response = requests.post(cloud_function_url, data=json.dumps(api_request), headers=headers)
+
+    if response.status_code == 200:
+        feedback = response.text
+    else:
+        feedback = "Error: " + response.text
 
-print(feedback)
+    print(feedback)
```

### Comparing `frazzle-0.2.0/PKG-INFO` & `frazzle-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frazzle
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: All rights reserved.
 Author: Daniel DeFreez
 Author-email: defreezd@sou.edu
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

