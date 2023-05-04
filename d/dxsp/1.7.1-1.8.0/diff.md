# Comparing `tmp/dxsp-1.7.1.tar.gz` & `tmp/dxsp-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.7.1.tar", max compression
+gzip compressed data, was "dxsp-1.8.0.tar", max compression
```

## Comparing `dxsp-1.7.1.tar` & `dxsp-1.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-03 14:54:16.641837 dxsp-1.7.1/LICENSE
--rw-r--r--   0        0        0     3225 2023-05-03 14:54:16.641837 dxsp-1.7.1/README.md
--rw-r--r--   0        0        0       38 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-03 14:54:17.485846 dxsp-1.7.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/config.py
--rw-r--r--   0        0        0      556 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28424 2023-05-03 14:54:16.641837 dxsp-1.7.1/dxsp/main.py
--rw-r--r--   0        0        0     1282 2023-05-03 14:54:17.485846 dxsp-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-04 19:34:22.523761 dxsp-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-05-04 19:34:22.523761 dxsp-1.8.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-04 19:34:23.343767 dxsp-1.8.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/config.py
+-rw-r--r--   0        0        0      556 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28404 2023-05-04 19:34:22.523761 dxsp-1.8.0/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-04 19:34:23.343767 dxsp-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 dxsp-1.8.0/PKG-INFO
```

### Comparing `dxsp-1.7.1/LICENSE` & `dxsp-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.7.1/README.md` & `dxsp-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.7.1/dxsp/assets/blockchains.py` & `dxsp-1.8.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.7.1/dxsp/default_settings.toml` & `dxsp-1.8.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.7.1/dxsp/main.py` & `dxsp-1.8.0/dxsp/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
  DEX SWAP Main
 """
-import json
+
 import logging
-import os
 
 import requests
 from dxsp import __version__
 from dxsp.assets.blockchains import blockchains
 from dxsp.config import settings
 from ping3 import ping
 from pycoingecko import CoinGeckoAPI
@@ -29,22 +28,23 @@
                  dex_exchange: str | None = None,
                  dex_router: str | None = None,
                  amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
-        self.logger.info("Initializing DexSwap for %s on %s", wallet_address, chain_id)
+        self.logger.info("Initializing DexSwap for %s on %s", 
+                         wallet_address, chain_id)
 
         self.chain_id = int(chain_id)
         self.logger.debug("self.chain_id %s", self.chain_id)
-        if self.chain_id  is None:
+        if self.chain_id is None:
             self.logger.warning("self.chain_id not setup")
             return
-        blockchain = blockchains[self.chain_id ]
+        blockchain = blockchains[self.chain_id]
         self.logger.debug("blockchain %s", blockchain)
 
         self.wallet_address = wallet_address
         self.logger.debug("self.wallet_address %s", self.wallet_address)
         self.private_key = private_key
 
         self.block_explorer_api = block_explorer_api
@@ -52,96 +52,96 @@
             self.logger.warning("self.block_explorer_api not setup")
         self.block_explorer_url = block_explorer_url
         self.block_explorer_url = (
             block_explorer_url
             or blockchain.get("block_explorer_url")
             or self.logger.warning("self.block_explorer_url not set up")
         )
-        self.logger.debug("self.block_explorer_url %s", self.block_explorer_url)
+        self.logger.debug("explorer_url %s", self.block_explorer_url)
 
         self.rpc = rpc or blockchain.get("rpc")
-        self.logger.debug("self.rpc %s",self.rpc)
+        self.logger.debug("self.rpc %s", self.rpc)
         try:
             self.latency = round(ping(self.rpc, unit='ms'), 3)
-            self.logger.debug("self.latency %s",self.latency)
+            self.logger.debug("self.latency %s", self.latency)
         except Exception as e:
-            self.logger.error("Failed to ping %s:%s",self.rpc, e)
+            self.logger.error("Failed to ping %s:%s", self.rpc, e)
 
         self.w3 = w3 or Web3(Web3.HTTPProvider(self.rpc))
         try:
             self.w3.net.listening
-            self.logger.info("connected to %s with w3 %s",self.rpc,self.w3)
+            self.logger.info("connected to %s with w3 %s", self.rpc, self.w3)
         except Exception as e:
-            self.logger.error("connectivity failed using %s", self.rpc)
+            self.logger.error("connectivity failed %s", e)
             return
-        self.logger.debug("self.w3 %s",self.w3)
+        self.logger.debug("self.w3 %s", self.w3)
         self.logger.info("connected")
 
         self.protocol_type = protocol_type or "1inch"
         if self.protocol_type == "0x":
             base_url = blockchain["0x"]
         elif self.protocol_type == "1inch_limit":
             base_url = blockchain["1inch_limit"]
         else:
             base_url = blockchain["1inch"]
         
         self.dex_url = f"{base_url}"
         self.logger.debug("self.dex_url %s", self.dex_url)
-        self.logger.debug("self.protocol_type %s",self.protocol_type)
+        self.logger.debug("self.protocol_type %s", self.protocol_type)
 
         self.dex_exchange = dex_exchange
-        self.logger.debug("self.dex_exchange %s",self.dex_exchange)
+        self.logger.debug("self.dex_exchange %s", self.dex_exchange)
 
         self.dex_router = dex_router
         if self.dex_router is None:
             if (
                 self.dex_exchange is None
                 or self.dex_exchange != blockchain["uniswap_v3"]
             ):
                 self.router = blockchain["uniswap_v2"]
             else:
                 self.router = blockchain["uniswap_v3"]
         else:
             self.router = self.dex_router
-        self.logger.debug("self.router %s",self.router)
+        self.logger.debug("self.router %s", self.router)
 
         self.name = "TBD"
-        self.logger.debug("self.name %s",self.name)
+        self.logger.debug("self.name %s", self.name)
 
-        self.trading_quote_ccy =  settings.trading_quote_ccy
-        self.logger.debug("self.trading_quote_ccy %s",self.trading_quote_ccy)
+        self.trading_quote_ccy = settings.trading_quote_ccy
+        self.logger.debug("self.trading_quote_ccy %s", self.trading_quote_ccy)
 
         self.amount_trading_option = amount_trading_option
-        self.logger.debug("self.amount_trading_option %s",self.amount_trading_option)
+        self.logger.debug("trading_option %s", self.amount_trading_option)
 
         try:
             self.gecko_api = CoinGeckoAPI()
             assetplatform = self.gecko_api.get_asset_platforms()
-            output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
+            output_dict = [x for x in assetplatform if x['chain_identifier']
+                           == int(self.chain_id)]
             self.gecko_platform = output_dict[0]['id']
             self.logger.debug("self.gecko_platform %s",self.gecko_platform)
         except Exception as e:
             self.logger.error("CoinGeckoAPI setup: %s", e)
             return
 
     async def _get(
                 self,
                 url,
                 params=None,
                 headers=None
             ):
-        headers = { "User-Agent": "Mozilla/5.0" }
-        self.logger.debug("_get url %s",url)
+        headers = {"User-Agent": "Mozilla/5.0"}
+        self.logger.debug("_get url %s", url)
         response = requests.get(
                             url,
-                            params =params,
-                            headers=headers,
-                            timeout=10
+                            params = params,
+                            headers = headers,
+                            timeout = 10
                         )
-        #self.logger.debug(f"response _get {response}")
         return response.json()
 
     async def get_quote(
                 self,
                 symbol
             ):
         self.logger.debug("get_quote %s",symbol)
@@ -162,18 +162,19 @@
                 self.logger.debug("asset_out_amount %s",asset_out_amount)
                 quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
                 quote = await self._get(quote_url)
                 self.logger.debug("quote %s",quote)
                 raw_quote = quote['toTokenAmount']
                 self.logger.debug("raw_quote %s",raw_quote)
                 asset_quote_decimals = quote['fromToken']['decimals']
-                self.logger.debug("asset_quote_decimals %s", asset_quote_decimals)
+                self.logger.debug("asset_quote_decimals %s",
+                                  asset_quote_decimals)
                 quote_readable = self.w3.from_wei(int(raw_quote),'wei') /(10 ** asset_quote_decimals)
                 self.logger.debug("quote_readable %s",quote_readable)
-                return round(quote_readable,2)
+                return round(quote_readable, 2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
     async def execute_order(
@@ -184,33 +185,33 @@
                 take_profit=10000,
                 quantity=1,
                 amount_trading_option=1,
                 order_type='swap'
         ):
         """execute swap function"""
         try:
-            self.logger.debug("execute_order %s %s %s",action,instrument, order_type)
+            self.logger.debug("execute_order %s %s %s", action,instrument, order_type)
             if order_type == 'swap':
                 self.logger.debug("execute_order %s",order_type)
 
-                asset_out_symbol = self.trading_quote_ccy if action=="BUY" else instrument
-                asset_in_symbol = instrument if action=="BUY" else self.trading_quote_ccy
+                asset_out_symbol = self.trading_quote_ccy if action == "BUY" else instrument
+                asset_in_symbol = instrument if action == "BUY" else self.trading_quote_ccy
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
                 try:
                     asset_out_decimals = asset_out_contract.functions.decimals().call()
                 except Exception as e:
                     self.logger.error("execute_order decimals: %s", e)
                     asset_out_decimals = 18
                 asset_out_balance = await self.get_token_balance(asset_out_symbol)
                 if amount_trading_option == 1:
-                    #buy or sell %p percentage DEFAULT OPTION
+                    # buy or sell %p percentage DEFAULT OPTION
                     asset_out_amount = ((asset_out_balance)/
                                         (10 ** asset_out_decimals))*(float(quantity)/100)
                 if amount_trading_option == 2:
-                    #SELL all token in case of sell order for example
+                    # SELL all token in case of sell order for example
                     asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
                 order = await self.get_swap(
                         asset_out_symbol,
                         asset_in_symbol,
                         asset_out_amount
                         )
                 if order:
@@ -223,15 +224,14 @@
                 self.logger.debug("execute_order %s", order_type)
                 return
 
         except Exception as e:
             self.logger.debug("error execute_order %s",e)
             return "error processing order in DXSP"
 
-
     async def get_swap(
                 self,
                 asset_out_symbol: str,
                 asset_in_symbol: str,
                 amount: int,
                 slippage_tolerance_percentage = 2
         ):
@@ -583,19 +583,20 @@
             return 0
 
     async def get_stablecoin_balance(
                                 self
                             ):
         stablecoins = settings.stablecoins
         try:
+            msg = ""
             for i in stablecoins:
                 bal_stablecoins = await self.get_token_balance(i)
                 if bal_stablecoins:
                     msg += f"\n💵{bal_stablecoins} {i}"
-                # bal = round(ex.from_wei(bal,'ether'),5)
+            return msg
         except Exception as e:
             self.logger.error("get_stablecoin_balance error: %s", e)
             return 0
 
     async def get_account_balance(
                             self
                         ):
```

### Comparing `dxsp-1.7.1/pyproject.toml` & `dxsp-1.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.7.1"
+version = "1.8.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.10,<3.11"
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
 ping3 = "*"
+#web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
 
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
@@ -48,7 +49,19 @@
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
+commit_parser = "semantic_release.history.emoji_parser"
+use_textual_changelog_sections = true
+
+#patch_emoji
+# 🐛🚑🤖🏁🔒👽🔍💬🥅⚡♿🍏🐧
+#:ambulance:, :lock:, :bug:, :zap:, :goal_net:, :alien:, :wheelchair:, :speech_balloon:, :mag:, :apple:, :penguin:, :checkered_flag:, :robot:, :green_apple
+#minor_emoji
+#✨🥚🚸📱💄📈
+#:sparkles: ✨, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
+#major_emoji¶
+#💥
+# :boom:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dxsp-1.7.1/PKG-INFO` & `dxsp-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.7.1
+Version: 1.8.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: web3 (>=6.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
```

