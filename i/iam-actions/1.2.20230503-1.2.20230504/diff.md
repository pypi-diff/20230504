# Comparing `tmp/iam_actions-1.2.20230503.tar.gz` & `tmp/iam_actions-1.2.20230504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230503.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230504.tar", max compression
```

## Comparing `iam_actions-1.2.20230503.tar` & `iam_actions-1.2.20230504.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/README.md
--rw-r--r--   0        0        0      228 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/__init__.py
--rw-r--r--   0        0        0  4244063 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545650 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/policies.json
--rw-r--r--   0        0        0   193569 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529184 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-03 02:27:00.281881 iam_actions-1.2.20230503/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230503/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230503/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/README.md
+-rw-r--r--   0        0        0      228 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4244539 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545679 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/policies.json
+-rw-r--r--   0        0        0   193569 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529212 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-04 02:26:19.727753 iam_actions-1.2.20230504/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230504/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230504/PKG-INFO
```

### Comparing `iam_actions-1.2.20230503/LICENSE` & `iam_actions-1.2.20230504/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/README.md` & `iam_actions-1.2.20230504/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/actions.json` & `iam_actions-1.2.20230504/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999669679192431%*

 * *Differences: {"'mediaconnect'": "{'UpdateGatewayInstance': OrderedDict([('access_level', 'Undocumented'), "*

 * *                   "('action', 'UpdateGatewayInstance'), ('condition_keys', []), ('description', "*

 * *                   "'Not Documented by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'wafv2'": '{\'ListAPIKeys\': {\'access_level\': \'List\', \'description\': "Grants permission to '*

 * *            'retrieve a list of the API keys that you\'ve defined for the specified scope"}, '*

 * *            "'CreateAPIKey': {'acc […]*

```diff
@@ -93226,14 +93226,22 @@
         "UpdateFlowSource": {
             "access_level": "Write",
             "action": "UpdateFlowSource",
             "condition_keys": [],
             "description": "Grants permission to update the source of any flow",
             "orphan": false,
             "resources": []
+        },
+        "UpdateGatewayInstance": {
+            "access_level": "Undocumented",
+            "action": "UpdateGatewayInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "mediaconvert": {
         "AssociateCertificate": {
             "access_level": "Write",
             "action": "AssociateCertificate",
             "condition_keys": [],
@@ -146973,18 +146981,18 @@
             "action": "CheckCapacity",
             "condition_keys": [],
             "description": "Grants permission to calculate web ACL capacity unit (WCU) requirements for a specified scope and set of rules",
             "orphan": false,
             "resources": []
         },
         "CreateAPIKey": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateAPIKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create an API key for use in the integration of the CAPTCHA API in your JavaScript client applications",
             "orphan": false,
             "resources": []
         },
         "CreateIPSet": {
             "access_level": "Write",
             "action": "CreateIPSet",
             "condition_keys": [
@@ -147149,18 +147157,18 @@
             "action": "GenerateMobileSdkReleaseUrl",
             "condition_keys": [],
             "description": "Grants permission to generate a presigned download URL for the specified release of the mobile SDK",
             "orphan": false,
             "resources": []
         },
         "GetDecryptedAPIKey": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDecryptedAPIKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return your API key in decrypted form. Use this to check the token domains that you have defined for the key",
             "orphan": false,
             "resources": []
         },
         "GetIPSet": {
             "access_level": "Read",
             "action": "GetIPSet",
             "condition_keys": [
@@ -147281,18 +147289,18 @@
                 "apprunner",
                 "appsync",
                 "loadbalancer/app/",
                 "userpool"
             ]
         },
         "ListAPIKeys": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAPIKeys",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a list of the API keys that you've defined for the specified scope",
             "orphan": false,
             "resources": []
         },
         "ListAvailableManagedRuleGroupVersions": {
             "access_level": "List",
             "action": "ListAvailableManagedRuleGroupVersions",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230504/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230504/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/generate.py` & `iam_actions-1.2.20230504/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230504/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230504/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/generate/services.py` & `iam_actions-1.2.20230504/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/policies.json` & `iam_actions-1.2.20230504/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997477550198%*

 * *Differences: {"'serviceMap'": "{'AWS Elemental MediaConnect': {'Actions': {insert: [(52, "*

 * *                 "'UpdateGatewayInstance')]}}}"}*

```diff
@@ -3408,15 +3408,16 @@
                 "UpdateBridgeOutput",
                 "UpdateBridgeSource",
                 "UpdateBridgeState",
                 "UpdateFlow",
                 "UpdateFlowEntitlement",
                 "UpdateFlowMediaStream",
                 "UpdateFlowOutput",
-                "UpdateFlowSource"
+                "UpdateFlowSource",
+                "UpdateGatewayInstance"
             ],
             "HasResource": true,
             "StringPrefix": "mediaconnect"
         },
         "AWS Elemental MediaConvert": {
             "ARNFormat": "arn:aws:mediaconvert:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:mediaconvert:.+",
```

### Comparing `iam_actions-1.2.20230503/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230504/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230503/iam_actions/services.json` & `iam_actions-1.2.20230504/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999997797861283%*

 * *Differences: {"'mediaconnect'": "{'Actions': {insert: [(52, 'UpdateGatewayInstance')]}}"}*

```diff
@@ -13013,15 +13013,16 @@
             "UpdateBridgeOutput",
             "UpdateBridgeSource",
             "UpdateBridgeState",
             "UpdateFlow",
             "UpdateFlowEntitlement",
             "UpdateFlowMediaStream",
             "UpdateFlowOutput",
-            "UpdateFlowSource"
+            "UpdateFlowSource",
+            "UpdateGatewayInstance"
         ],
         "ConditionKeys": [],
         "HasResource": true,
         "ServiceNames": [
             "AWS Elemental MediaConnect"
         ]
     },
```

### Comparing `iam_actions-1.2.20230503/pyproject.toml` & `iam_actions-1.2.20230504/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230503"
+version = "1.2.20230504"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230503/setup.py` & `iam_actions-1.2.20230504/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230503',
+    'version': '1.2.20230504',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230503/PKG-INFO` & `iam_actions-1.2.20230504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230503
+Version: 1.2.20230504
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

