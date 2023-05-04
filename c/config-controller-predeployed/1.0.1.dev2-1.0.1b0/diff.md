# Comparing `tmp/config-controller-predeployed-1.0.1.dev2.tar.gz` & `tmp/config-controller-predeployed-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-controller-predeployed-1.0.1.dev2.tar", last modified: Thu May  4 12:12:49 2023, max compression
+gzip compressed data, was "config-controller-predeployed-1.0.1b0.tar", last modified: Thu Dec 29 15:42:12 2022, max compression
```

## Comparing `config-controller-predeployed-1.0.1.dev2.tar` & `config-controller-predeployed-1.0.1b0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)    42883 2023-05-04 12:12:48.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/artifacts/ConfigController.json
--rw-r--r--   0 runner    (1001) docker     (123)    47543 2023-05-04 12:12:48.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/artifacts/ConfigController.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/config_controller_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-04 12:12:49.000000 config-controller-predeployed-1.0.1.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/test/test_cc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:49.941343 config-controller-predeployed-1.0.1.dev2/test/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/test/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/test/tools/test_predeployed.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-04 12:12:12.000000 config-controller-predeployed-1.0.1.dev2/test/tools/test_solidity_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.441460 config-controller-predeployed-1.0.1b0/config_controller_predeployed/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/config_controller_predeployed/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)    42883 2022-12-29 15:42:09.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed/artifacts/ConfigController.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47543 2022-12-29 15:42:09.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed/artifacts/ConfigController.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed/config_controller_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2022-12-29 15:42:12.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-29 15:42:12.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 15:42:12.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 15:42:12.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-29 15:42:12.000000 config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2022-12-29 15:42:11.000000 config-controller-predeployed-1.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/test/test_cc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 15:42:12.445460 config-controller-predeployed-1.0.1b0/test/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/test/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/test/tools/test_predeployed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-29 15:41:21.000000 config-controller-predeployed-1.0.1b0/test/tools/test_solidity_project.py
```

### Comparing `config-controller-predeployed-1.0.1.dev2/README.md` & `config-controller-predeployed-1.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/artifacts/ConfigController.json` & `config-controller-predeployed-1.0.1b0/config_controller_predeployed/artifacts/ConfigController.json`

 * *Files identical despite different names*

### Comparing `config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/artifacts/ConfigController.meta.json` & `config-controller-predeployed-1.0.1b0/config_controller_predeployed/artifacts/ConfigController.meta.json`

 * *Files identical despite different names*

### Comparing `config-controller-predeployed-1.0.1.dev2/config_controller_predeployed/config_controller_generator.py` & `config-controller-predeployed-1.0.1b0/config_controller_predeployed/config_controller_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 class ConfigControllerGenerator(AccessControlEnumerableGenerator):
     '''Generates ConfigController
     '''
 
     ARTIFACT_FILENAME = 'ConfigController.json'
     META_FILENAME = 'ConfigController.meta.json'
     DEFAULT_ADMIN_ROLE = (0).to_bytes(32, 'big')
-    DEPLOYER_ROLE = w3.solidity_keccak(['string'], ['DEPLOYER_ROLE'])
-    DEPLOYER_ADMIN_ROLE = w3.solidity_keccak(['string'], ['DEPLOYER_ADMIN_ROLE'])
-    MTM_ADMIN_ROLE = w3.solidity_keccak(['string'], ['MTM_ADMIN_ROLE'])
+    DEPLOYER_ROLE = w3.solidityKeccak(['string'], ['DEPLOYER_ROLE'])
+    DEPLOYER_ADMIN_ROLE = w3.solidityKeccak(['string'], ['DEPLOYER_ADMIN_ROLE'])
+    MTM_ADMIN_ROLE = w3.solidityKeccak(['string'], ['MTM_ADMIN_ROLE'])
 
     # ---------- storage ----------
     # --------Initializable--------
     # 0:    _initialized, _initializing;
     # -----ContextUpgradeable------
     # 1:    __gap
     # ...   __gap
```

### Comparing `config-controller-predeployed-1.0.1.dev2/config_controller_predeployed.egg-info/SOURCES.txt` & `config-controller-predeployed-1.0.1b0/config_controller_predeployed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `config-controller-predeployed-1.0.1.dev2/setup.py` & `config-controller-predeployed-1.0.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev']
 )
 
 setup(
     name='config-controller-predeployed',
-    version='1.0.1dev2',
+    version='1.0.1b0',
     description='A tool for generating predeployed config controller smart contract',
     long_description_content_type="text/markdown",
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/config-controller',
     install_requires=[
-        "predeployed-generator >= 1.1.0"
+        "predeployed-generator >= 1.1.0a0"
     ],
     python_requires='>=3.7,<4',
     extras_require=extras_require,
     keywords=['skale', 'predeployed'],
     packages=find_packages(exclude=['tests']),
     package_data={
         'config_controller_predeployed': [
```

### Comparing `config-controller-predeployed-1.0.1.dev2/test/test_cc_generator.py` & `config-controller-predeployed-1.0.1b0/test/test_cc_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,220 +1,220 @@
 import os
 
 import pytest
 import web3.exceptions
 from web3.auto import w3
-from web3 import Account
 from web3.middleware import geth_poa_middleware
 
 from config_controller_predeployed import ConfigControllerGenerator, CONFIG_CONTROLLER_ADDRESS
 from .tools.test_solidity_project import TestSolidityProject
 
 PRIVATE_KEY = os.environ['ETH_PRIVATE_KEY']
 
 
 class TestEtherbaseGenerator(TestSolidityProject):
-    OWNER_ADDRESS = Account.from_key(bytes.fromhex(PRIVATE_KEY[2:])).address
+    OWNER_ADDRESS = w3.eth.account.privateKeyToAccount(PRIVATE_KEY).address
 
     def get_dc_abi(self):
         return self.get_abi('ConfigController')
 
     def prepare_genesis(self):
+        print(self.OWNER_ADDRESS)
         dc_generator = ConfigControllerGenerator()
 
         return self.generate_genesis(
             owner=self.OWNER_ADDRESS,
             allocations=dc_generator.generate_allocation(
                 CONFIG_CONTROLLER_ADDRESS,
                 schain_owner=self.OWNER_ADDRESS
             )
         )
 
     def test_default_admin_role(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert dc.functions.getRoleMemberCount(ConfigControllerGenerator.DEFAULT_ADMIN_ROLE).call() == 1
             assert dc.functions.getRoleMember(ConfigControllerGenerator.DEFAULT_ADMIN_ROLE,
                                               0).call() == self.OWNER_ADDRESS
             assert dc.functions.hasRole(ConfigControllerGenerator.DEFAULT_ADMIN_ROLE, self.OWNER_ADDRESS).call()
             assert dc.functions.version().call() == '1.0.1'
 
     def test_deployer_role(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert dc.functions.getRoleMemberCount(ConfigControllerGenerator.DEPLOYER_ROLE).call() == 1
             assert dc.functions.getRoleAdmin(ConfigControllerGenerator.DEPLOYER_ROLE).call() == \
                    ConfigControllerGenerator.DEPLOYER_ADMIN_ROLE
             assert dc.functions.getRoleMember(ConfigControllerGenerator.DEPLOYER_ROLE,
                                               0).call() == self.OWNER_ADDRESS
             assert dc.functions.hasRole(ConfigControllerGenerator.DEPLOYER_ROLE, self.OWNER_ADDRESS).call()
 
     def test_deployer_admin_role(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert dc.functions.getRoleMemberCount(ConfigControllerGenerator.DEPLOYER_ADMIN_ROLE).call() == 1
             assert dc.functions.getRoleMember(ConfigControllerGenerator.DEPLOYER_ADMIN_ROLE,
                                               0).call() == self.OWNER_ADDRESS
             assert dc.functions.hasRole(ConfigControllerGenerator.DEPLOYER_ADMIN_ROLE, self.OWNER_ADDRESS).call()
 
     def test_mtm_admin_role(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert dc.functions.getRoleMemberCount(ConfigControllerGenerator.MTM_ADMIN_ROLE).call() == 1
             assert dc.functions.getRoleMember(ConfigControllerGenerator.MTM_ADMIN_ROLE,
                                               0).call() == self.OWNER_ADDRESS
             assert dc.functions.hasRole(ConfigControllerGenerator.MTM_ADMIN_ROLE, self.OWNER_ADDRESS).call()
 
     def test_add_whitelist(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
-            tx = dc.functions.addToWhitelist('0xD300000000000000000000000000000000000001').build_transaction({
-                'nonce': w3.eth.get_transaction_count(self.OWNER_ADDRESS),
+            tx = dc.functions.addToWhitelist('0xD300000000000000000000000000000000000001').buildTransaction({
+                'nonce': w3.eth.getTransactionCount(self.OWNER_ADDRESS),
                 'from': self.OWNER_ADDRESS
             })
-            signed_tx = w3.eth.account.sign_transaction(tx, private_key=PRIVATE_KEY)
-            tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-            w3.eth.wait_for_transaction_receipt(tx_hash)
+            signed_tx = w3.eth.account.signTransaction(tx, private_key=PRIVATE_KEY)
+            tx_hash = w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+            w3.eth.waitForTransactionReceipt(tx_hash)
             assert dc.functions.isAddressWhitelisted('0xD300000000000000000000000000000000000001').call()
 
     def test_add_whitelist_failed(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
-            with pytest.raises(web3.exceptions.ContractLogicError):
-                dc.functions.addToWhitelist('0xD300000000000000000000000000000000000001').build_transaction({
+            with pytest.raises(web3.exceptions.SolidityError):
+                dc.functions.addToWhitelist('0xD300000000000000000000000000000000000001').buildTransaction({
                     'from': '0xD300000000000000000000000000000000000001'
                 })
 
     def test_enable_and_disable_mtm(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert not dc.functions.isMTMEnabled().call()
 
-            tx = dc.functions.enableMTM().build_transaction({
-                'nonce': w3.eth.get_transaction_count(self.OWNER_ADDRESS),
+            tx = dc.functions.enableMTM().buildTransaction({
+                'nonce': w3.eth.getTransactionCount(self.OWNER_ADDRESS),
                 'from': self.OWNER_ADDRESS
             })
-            signed_tx = w3.eth.account.sign_transaction(tx, private_key=PRIVATE_KEY)
-            tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-            w3.eth.wait_for_transaction_receipt(tx_hash)
+            signed_tx = w3.eth.account.signTransaction(tx, private_key=PRIVATE_KEY)
+            tx_hash = w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+            w3.eth.waitForTransactionReceipt(tx_hash)
             assert dc.functions.isMTMEnabled().call()
 
-            tx = dc.functions.disableMTM().build_transaction({
-                'nonce': w3.eth.get_transaction_count(self.OWNER_ADDRESS),
+            tx = dc.functions.disableMTM().buildTransaction({
+                'nonce': w3.eth.getTransactionCount(self.OWNER_ADDRESS),
                 'from': self.OWNER_ADDRESS
             })
-            signed_tx = w3.eth.account.sign_transaction(tx, private_key=PRIVATE_KEY)
-            tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-            w3.eth.wait_for_transaction_receipt(tx_hash)
+            signed_tx = w3.eth.account.signTransaction(tx, private_key=PRIVATE_KEY)
+            tx_hash = w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+            w3.eth.waitForTransactionReceipt(tx_hash)
             assert not dc.functions.isMTMEnabled().call()
 
     def test_enable_and_disable_mtm_failed(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
 
-            with pytest.raises(web3.exceptions.ContractLogicError):
-                dc.functions.enableMTM().build_transaction({
+            with pytest.raises(web3.exceptions.SolidityError):
+                dc.functions.enableMTM().buildTransaction({
                     'from': '0xD300000000000000000000000000000000000001'
                 })
 
-            with pytest.raises(web3.exceptions.ContractLogicError):
-                dc.functions.disableMTM().build_transaction({
+            with pytest.raises(web3.exceptions.SolidityError):
+                dc.functions.disableMTM().buildTransaction({
                     'from': '0xD300000000000000000000000000000000000001'
                 })
 
     def test_enable_and_disable_fcd(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
             assert not dc.functions.isMTMEnabled().call()
 
-            tx = dc.functions.enableFreeContractDeployment().build_transaction({
-                'nonce': w3.eth.get_transaction_count(self.OWNER_ADDRESS),
+            tx = dc.functions.enableFreeContractDeployment().buildTransaction({
+                'nonce': w3.eth.getTransactionCount(self.OWNER_ADDRESS),
                 'from': self.OWNER_ADDRESS
             })
-            signed_tx = w3.eth.account.sign_transaction(tx, private_key=PRIVATE_KEY)
-            tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-            w3.eth.wait_for_transaction_receipt(tx_hash)
+            signed_tx = w3.eth.account.signTransaction(tx, private_key=PRIVATE_KEY)
+            tx_hash = w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+            w3.eth.waitForTransactionReceipt(tx_hash)
             assert dc.functions.isFCDEnabled().call()
 
-            tx = dc.functions.disableFreeContractDeployment().build_transaction({
-                'nonce': w3.eth.get_transaction_count(self.OWNER_ADDRESS),
+            tx = dc.functions.disableFreeContractDeployment().buildTransaction({
+                'nonce': w3.eth.getTransactionCount(self.OWNER_ADDRESS),
                 'from': self.OWNER_ADDRESS
             })
-            signed_tx = w3.eth.account.sign_transaction(tx, private_key=PRIVATE_KEY)
-            tx_hash = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-            w3.eth.wait_for_transaction_receipt(tx_hash)
+            signed_tx = w3.eth.account.signTransaction(tx, private_key=PRIVATE_KEY)
+            tx_hash = w3.eth.sendRawTransaction(signed_tx.rawTransaction)
+            w3.eth.waitForTransactionReceipt(tx_hash)
             assert not dc.functions.isFCDEnabled().call()
 
     def test_enable_and_disable_fcd_failed(self, tmpdir):
         self.datadir = tmpdir
         genesis = self.prepare_genesis()
 
         with self.run_geth(tmpdir, genesis):
-            assert w3.is_connected()
+            assert w3.isConnected()
             if not w3.middleware_onion.get(geth_poa_middleware):
                 w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             dc = w3.eth.contract(address=CONFIG_CONTROLLER_ADDRESS, abi=self.get_dc_abi())
 
-            with pytest.raises(web3.exceptions.ContractLogicError):
-                dc.functions.enableFreeContractDeployment().build_transaction({
+            with pytest.raises(web3.exceptions.SolidityError):
+                dc.functions.enableFreeContractDeployment().buildTransaction({
                     'from': '0xD300000000000000000000000000000000000001'
                 })
 
-            with pytest.raises(web3.exceptions.ContractLogicError):
-                dc.functions.disableFreeContractDeployment().build_transaction({
+            with pytest.raises(web3.exceptions.SolidityError):
+                dc.functions.disableFreeContractDeployment().buildTransaction({
                     'from': '0xD300000000000000000000000000000000000001'
                 })
```

### Comparing `config-controller-predeployed-1.0.1.dev2/test/tools/test_predeployed.py` & `config-controller-predeployed-1.0.1b0/test/tools/test_predeployed.py`

 * *Files 23% similar despite different names*

```diff
@@ -55,31 +55,29 @@
         with open(genesis_filename, 'w') as f:
             json.dump(genesis, f)
 
         # prepare geth
         process = subprocess.run(['geth', '--datadir', tmpdir, 'init', genesis_filename], capture_output=True)
         assert process.returncode == 0
 
-        # run geth
-        self.geth = subprocess.Popen(['geth', '--datadir', tmpdir, '--http',
-                                      '--miner.etherbase', '0x0000000000000000000000000000000000000001', '--mine',
-                                      '--http.api', 'personal,eth,net,web3,txpool,miner'], stderr=subprocess.PIPE, universal_newlines=True)
-
+        self.geth = subprocess.Popen(['geth', '--datadir', tmpdir, '--http', '--mine',
+                                      '--http.api', 'personal,eth,net,web3,txpool,miner'],
+                                     stderr=subprocess.PIPE, universal_newlines=True)
         time.sleep(5)
 
         # mine blocks
-        process = subprocess.Popen(['curl', '-X', 'POST', '-H', 'Content-Type: application/json',
-                                    '--data', '{"jsonrpc":"2.0","method":"miner_start","params":[],"id":1}', 'http://localhost:8545'])
+        subprocess.Popen(['curl', '-d', '{"method": "miner_start"}', '-H', 'Content-type: application/json',
+                          'http://127.0.0.1:8545'])
 
         while True:
             assert self.geth.poll() is None
             output_line = self.geth.stderr.readline()
             if 'HTTP server started' in output_line:
                 break
 
         return GethInstance(self.geth)
 
     def stop_geth(self):
         if self.geth:
             self.geth.terminate()
             self.geth.communicate()
-            assert self.geth.returncode == 0
+            assert self.geth.returncode == 0
```

### Comparing `config-controller-predeployed-1.0.1.dev2/test/tools/test_solidity_project.py` & `config-controller-predeployed-1.0.1b0/test/tools/test_solidity_project.py`

 * *Files identical despite different names*

