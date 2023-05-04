# Comparing `tmp/dexie_rewards-0.0.1.tar.gz` & `tmp/dexie_rewards-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-0.0.1.tar", max compression
+gzip compressed data, was "dexie_rewards-0.0.2.tar", max compression
```

## Comparing `dexie_rewards-0.0.1.tar` & `dexie_rewards-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.1/LICENSE
--rw-r--r--   0        0        0     9619 2023-05-04 04:01:30.597086 dexie_rewards-0.0.1/README.md
--rw-r--r--   0        0        0      643 2023-05-04 04:09:35.322418 dexie_rewards-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-04 04:07:48.529750 dexie_rewards-0.0.1/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-02 08:44:23.928205 dexie_rewards-0.0.1/src/dexie_rewards/config.py
--rw-r--r--   0        0        0     1133 2023-05-02 08:44:23.929217 dexie_rewards-0.0.1/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      272 2023-05-04 04:08:54.737867 dexie_rewards-0.0.1/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     2866 2023-05-02 08:44:23.931726 dexie_rewards-0.0.1/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1122 2023-05-02 08:44:23.929570 dexie_rewards-0.0.1/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      310 2023-05-02 08:44:23.932210 dexie_rewards-0.0.1/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     2596 2023-05-02 08:44:23.931954 dexie_rewards-0.0.1/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2329 2023-05-02 08:44:23.936658 dexie_rewards-0.0.1/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     1224 2023-05-02 08:44:23.935671 dexie_rewards-0.0.1/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0     1606 2023-05-02 08:44:23.935051 dexie_rewards-0.0.1/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0    10330 1970-01-01 00:00:00.000000 dexie_rewards-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9721 2023-05-04 04:25:10.558427 dexie_rewards-0.0.2/README.md
+-rw-r--r--   0        0        0      643 2023-05-04 04:23:49.780610 dexie_rewards-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.2/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-02 08:44:23.928205 dexie_rewards-0.0.2/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0     1133 2023-05-02 08:44:23.929217 dexie_rewards-0.0.2/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      272 2023-05-04 04:08:54.737867 dexie_rewards-0.0.2/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     2866 2023-05-02 08:44:23.931726 dexie_rewards-0.0.2/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1122 2023-05-02 08:44:23.929570 dexie_rewards-0.0.2/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      310 2023-05-02 08:44:23.932210 dexie_rewards-0.0.2/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     2596 2023-05-02 08:44:23.931954 dexie_rewards-0.0.2/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2329 2023-05-02 08:44:23.936658 dexie_rewards-0.0.2/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     1224 2023-05-02 08:44:23.935671 dexie_rewards-0.0.2/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0     1606 2023-05-02 08:44:23.935051 dexie_rewards-0.0.2/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0    10432 1970-01-01 00:00:00.000000 dexie_rewards-0.0.2/PKG-INFO
```

### Comparing `dexie_rewards-0.0.1/LICENSE` & `dexie_rewards-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/README.md` & `dexie_rewards-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 ```sh
 ❯ dexie --help
 
  Usage: dexie [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
+│ --version      Show the version and exit.                                                     │
 │ --help      Show this message and exit.                                                       │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────╮
 │ rewards           Manage your dexie rewards for offers                                        │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
```

### Comparing `dexie_rewards-0.0.1/pyproject.toml` & `dexie_rewards-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "0.0.1"
+version = "0.0.2"
 description = "An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/config.py` & `dexie_rewards-0.0.2/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-0.0.2/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-0.0.2/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/rewards/list.py` & `dexie_rewards-0.0.2/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-0.0.2/src/dexie_rewards/rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-0.0.2/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-0.0.2/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/src/dexie_rewards/utils.py` & `dexie_rewards-0.0.2/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.1/PKG-INFO` & `dexie_rewards-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 0.0.1
+Version: 0.0.2
 Summary: An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -75,14 +75,15 @@
 
 ```sh
 ❯ dexie --help
 
  Usage: dexie [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────╮
+│ --version      Show the version and exit.                                                     │
 │ --help      Show this message and exit.                                                       │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────╮
 │ rewards           Manage your dexie rewards for offers                                        │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
```

