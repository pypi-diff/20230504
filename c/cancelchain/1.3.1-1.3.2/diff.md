# Comparing `tmp/cancelchain-1.3.1.tar.gz` & `tmp/cancelchain-1.3.2.tar.gz`

## Comparing `cancelchain-1.3.1.tar` & `cancelchain-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/__init__.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/api.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/api_client.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/application.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/block.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/browser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/cache.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/chain.py
--rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/command.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/config.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/console.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/database.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/exceptions.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/miller.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/milling.py
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/models.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/node.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/payload.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/schema.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/signals.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/tasks.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/transaction.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/util.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/wallet.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/base.html
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/block.html
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/chains.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/index.html
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.1/src/cancelchain/templates/transaction.html
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.1/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.1/LICENSE
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 cancelchain-1.3.1/README.rst
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 cancelchain-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/__init__.py
+-rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/api.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/api_client.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/application.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/block.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/browser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/cache.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/chain.py
+-rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/command.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/config.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/console.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/database.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/exceptions.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/miller.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/milling.py
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/models.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/node.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/payload.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/schema.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/signals.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/tasks.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/transaction.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/util.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/wallet.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/base.html
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/block.html
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/chains.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/index.html
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/transaction.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.2/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.2/LICENSE
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cancelchain-1.3.2/README.rst
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 cancelchain-1.3.2/PKG-INFO
```

### Comparing `cancelchain-1.3.1/src/cancelchain/__init__.py` & `cancelchain-1.3.2/src/cancelchain/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 
 
 def create_app(app=None, register_browser=True, test_config=None):
     from .application import init_app
     from .cache import cache
     from .config import EnvAppSettings
     from .database import db
```

### Comparing `cancelchain-1.3.1/src/cancelchain/api.py` & `cancelchain-1.3.2/src/cancelchain/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 from enum import Enum
 from functools import wraps
 from urllib.parse import urljoin
 
 import jwt
 from flask import Blueprint, abort, current_app, make_response, request
 from flask.views import MethodView
@@ -46,20 +47,18 @@
 
 def queue_post_process(path, data, visited_hosts):
     host, address = host_address(current_app.config['NODE_HOST'])
     wallet = current_app.wallets.get(address)
     headers = None
     if visited_hosts:
         headers = {PEER_HOST_HEADER: ','.join(visited_hosts)}
-    client = ApiClient(host, wallet)
-    headers = client.auth_header(headers=headers)
+    headers = ApiClient(host, wallet).auth_header(headers=headers)
     url = urljoin(host, path)
     http_post_signal.send(
-        current_app._get_current_object(),
-        url=url, data=data, headers=headers
+        current_app._get_current_object(), url=url, data=data, headers=headers
     )
 
 
 def queue_block_post_process(block, visited_hosts):
     queue_post_process(
         f'/api/block/{block.block_hash}/process',
         block.to_json(),
@@ -109,15 +108,17 @@
     ADMIN = 4
 
     def addresses(self):
         return current_app.config.get(f'{self.name}_ADDRESSES')
 
     @classmethod
     def address_roles(cls, address):
-        return [role for role in Role if address in role.addresses()]
+        return [role for role in Role if any(
+            re.fullmatch(x, address) for x in role.addresses()
+        )]
 
     @classmethod
     def address_role(cls, address):
         roles = cls.address_roles(address)
         return roles[-1] if roles else None
 
 
@@ -289,16 +290,15 @@
             process = process == 'process'
             if not process:
                 process = not current_app.config.get('API_ASYNC_PROCESSING')
             node, _, _ = node_lc_dao()
             vhosts = visited_hosts()
             received = now_iso()
             txn = node.receive_transaction(
-                txid, request.data,
-                visited_hosts=vhosts, process=process
+                txid, request.data, visited_hosts=vhosts, process=process
             )
             if process is False and txn is not None:
                 queue_txn_post_process(txn, vhosts)
         except CCError as err:
             return make_error_response(err)
         except Exception as e:
             exception_response(e)
@@ -461,16 +461,15 @@
 class PendingTxnView(MethodView):
     def get(self, **kwargs):
         try:
             node, _, _ = node_lc_dao()
             node.discard_expired_pending_txns()
             args = PendingTxnQuerySchema().load(request.args)
             earliest = args.get('earliest')
-            expired = now()
-            expired -= TXN_TIMEOUT
+            expired = now() - TXN_TIMEOUT
             pending_json = node.pending_txns.query_json(
                 earliest=earliest, expired=expired
             )
             return make_json_response([json.loads(j) for j in pending_json])
         except (ValidationError, CCError) as err:
             return make_error_response(err)
         except Exception as e:
```

### Comparing `cancelchain-1.3.1/src/cancelchain/api_client.py` & `cancelchain-1.3.2/src/cancelchain/api_client.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/application.py` & `cancelchain-1.3.2/src/cancelchain/application.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/block.py` & `cancelchain-1.3.2/src/cancelchain/block.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/browser.py` & `cancelchain-1.3.2/src/cancelchain/browser.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/chain.py` & `cancelchain-1.3.2/src/cancelchain/chain.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/command.py` & `cancelchain-1.3.2/src/cancelchain/command.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/config.py` & `cancelchain-1.3.2/src/cancelchain/config.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/exceptions.py` & `cancelchain-1.3.2/src/cancelchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/miller.py` & `cancelchain-1.3.2/src/cancelchain/miller.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/milling.py` & `cancelchain-1.3.2/src/cancelchain/milling.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/models.py` & `cancelchain-1.3.2/src/cancelchain/models.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/node.py` & `cancelchain-1.3.2/src/cancelchain/node.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/payload.py` & `cancelchain-1.3.2/src/cancelchain/payload.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/schema.py` & `cancelchain-1.3.2/src/cancelchain/schema.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/tasks.py` & `cancelchain-1.3.2/src/cancelchain/tasks.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/transaction.py` & `cancelchain-1.3.2/src/cancelchain/transaction.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/util.py` & `cancelchain-1.3.2/src/cancelchain/util.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/wallet.py` & `cancelchain-1.3.2/src/cancelchain/wallet.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/templates/base.html` & `cancelchain-1.3.2/src/cancelchain/templates/base.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/templates/block.html` & `cancelchain-1.3.2/src/cancelchain/templates/block.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/templates/chains.html` & `cancelchain-1.3.2/src/cancelchain/templates/chains.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/templates/index.html` & `cancelchain-1.3.2/src/cancelchain/templates/index.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/src/cancelchain/templates/transaction.html` & `cancelchain-1.3.2/src/cancelchain/templates/transaction.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/.gitignore` & `cancelchain-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/LICENSE` & `cancelchain-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.1/README.rst` & `cancelchain-1.3.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 ----------
 
 Create a local database by running the `init command`_:
 
 .. code-block:: console
 
   $ cancelchain init
-  Initialized the database.
 
 The `CC_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
 
 
 Import
 ------
 
@@ -88,79 +87,108 @@
 
 This command could take a while to run depending on your computer and the number of blocks imported. A progress bar will display with estimated time remaining. You can run the ``import`` command multiple times and it will only import new blocks that are not yet in the database.
 
 
 Run
 ---
 
-You run the ``cancelchain`` application by issuing the ``cancelchain run`` command:
+Run the ``cancelchain`` application by issuing the ``run`` command:
 
 .. code-block:: console
 
   $ cancelchain run
-   * Serving Flask app 'cancelchain'
-   * Debug mode: off
-  WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
-   * Running on all addresses (0.0.0.0)
-   * Running on http://127.0.0.1:5000
-  Press CTRL+C to quit
 
 Open `http://localhost:5000 <http://localhost:5000>`_ in a browser to explore the local copy of the blockchain.
 
-Home (Current Chain)
-^^^^^^^^^^^^^^^^^^^^
+Home Page (Current Chain)
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
-.. image:: readme-assets/browser-chain.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-chain.png?raw=true
    :width: 500pt
 
-Block
-^^^^^
+Block Page
+^^^^^^^^^^
 
-.. image:: readme-assets/browser-block.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-block.png?raw=true
    :width: 500pt
 
-Transaction
-^^^^^^^^^^^
+Transaction Page
+^^^^^^^^^^^^^^^^
 
-.. image:: readme-assets/browser-txn.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-txn.png?raw=true
    :width: 500pt
 
-Running the ``cancelchain`` application also exposes a number of web service endpoints that comprise the communications layer of the blockchain. See the  `API Documentation`_ for much more information.
+Running the ``cancelchain`` application also exposes a set of web service endpoints that comprise the communications layer of the blockchain. See the  `API Documentation`_ for more information.
 
-There are also many other ``cancelchain`` commands for interacting with the blockchain. See the `Command Line Interface Documentation`_ or run ``cancelchain --help``.
+There are other ``cancelchain`` commands for interacting with the blockchain. See the `Command Line Interface Documentation`_ for more information or run ``cancelchain --help``.
 
 
 Joining The CancelChain Network
 ===============================
 
-The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
+The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `miller`_ or `transactor`_ role `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
 
-If you would like to be granted API access to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of access you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
+`The Cancel Button`_ allows `reader`_ role `API access`_ to any account that completes at least one transaction on the blockchain:
+
+1) `Register for an account`_.
+2) Submit a successful transaction for any subject. Access won't be granted until the sentiment transaction successfully completes.
+3) Click `Download Account Key`_ on the `Account`_ page to download the account's key (`PEM`_) file.
+4) Create a directory called ``wallets`` and copy the downloaded key file into it.
+5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `Account`_ page and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
+
+  .. code-block:: console
+
+    # Network Settings
+    CC_NODE_HOST=http://CCTheCancelButtonAddressCC@localhost:5000
+    CC_PEERS=["https://CCTheCancelButtonAddressCC@thecancelbutton.com"]
+    CC_DEFAULT_COMMAND_HOST=https://CCTheCancelButtonAddressCC@thecancelbutton.com
+    CC_WALLET_DIR=/path/to/wallets
+
+6) Restart to load the new configuration.
+
+See `Configuration Documentation`_ for more detailed information about these settings.
+
+The `reader`_ role `API access`_ allows the `sync command`_ to update to the most recent peer block data:
+
+.. code-block:: console
+
+  $ cancelchain sync
+
+This command could take a while to run depending on your computer, internet access, and the number of blocks synchronized. A progress bar will display with estimated time remaining. You can run the `sync command`_ multiple times and it will only synchronize new blocks that are not yet in the database.
+
+Reader access also allows querying data (i.e. subject counts and balances) using the CLI. See `Command Line Interface Documentation`_ for more information.
+
+If you would like to be granted other `API access`_ to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of role you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
 
 See the `documentation`_ for some potential development ideas.
 
 
-.. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
+.. _Account: https://thecancelbutton.com/account
 .. _API access: https://docs.cancelchain.org/en/latest/api.html#api-roles
+.. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
 .. _Blog: https://blog.cancelchain.org
 .. _CancelChain data: https://storage.googleapis.com/blocks.cancelchain.org/cancelchain.jsonl
 .. _CC_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
 .. _CC_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
 .. _Command Line Interface Documentation: https://docs.cancelchain.org/en/latest/usage.html#command-line-interface
 .. _Configuration Documentation: https://docs.cancelchain.org/en/latest/usage.html#configuration
 .. _documentation: https://docs.cancelchain.org
 .. _Documentation: https://docs.cancelchain.org
+.. _Download Account Key: https://thecancelbutton.com/pem
 .. _import command: https://docs.cancelchain.org/en/latest/usage.html#import
 .. _init command: https://docs.cancelchain.org/en/latest/usage.html#init
 .. _instance folder: https://flask.palletsprojects.com/en/2.2.x/config/#instance-folders
 .. _JSON Lines: https://jsonlines.org/
 .. _miller: https://docs.cancelchain.org/en/latest/api.html#miller
+.. _PEM: https://en.wikipedia.org/wiki/Privacy-Enhanced_Mail
 .. _Project Home Page: https://cancelchain.org
-.. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _python virtual environment: https://docs.python.org/3/library/venv.html
+.. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _reader: https://docs.cancelchain.org/en/latest/api.html#reader
+.. _Register for an account: https://thecancelbutton.com/register
 .. _running milling processes: https://docs.cancelchain.org/en/latest/usage.html#mill
 .. _shell command: https://flask.palletsprojects.com/en/2.2.x/cli/#open-a-shell
 .. _sock puppet accounts: https://en.wikipedia.org/wiki/Sock_puppet_account
 .. _SQLite: https://sqlite.org/index.html
+.. _sync command: https://docs.cancelchain.org/en/latest/usage.html#sync
 .. _The Cancel Button: https://thecancelbutton.com
 .. _transactor: https://docs.cancelchain.org/en/latest/api.html#transactor
```

### Comparing `cancelchain-1.3.1/pyproject.toml` & `cancelchain-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # PROJECT
 [project]
 name = "cancelchain"
 dynamic = ["version"]
-description = "A Blockchain of Accountability, Support, and Forgiveness"
+description = "A Blockchain of Accountability, Forgiveness, and Support"
 readme = "README.rst"
 license = "MIT"
 requires-python = ">=3.9"
 authors = [
   { name = "Thomas Bohmbach Jr", email = "tom@cancelchain.org" }
 ]
 keywords = [
@@ -28,28 +28,28 @@
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "base58check>=1.0",
   "blinker>=1.6",
   "celery>=5.2",
   "click>=8.1",
-  "Flask>=2.2",
+  "Flask>=2.3",
   "Flask-Caching>=2.0",
   "Flask-SQLAlchemy>=3.0",
   "gunicorn>=20.1",
   "humanfriendly>=10.0",
   "marshmallow>=3.19",
   "millify>=0.1",
   "passlib[argon2]>=1.7",
   "pg8000>=1.29",
   "pycryptodome>=3.17",
   "pyjwt>=2.6",
   "pymerkle>=4.0",
   "python-dotenv>=1.0",
-  "requests>=2.28",
+  "requests>=2.29",
   "rich>=13.3",
   "sqlalchemy<2.0",
 ]
 
 [project.scripts]
 cancelchain = "cancelchain:cli"
 
@@ -75,15 +75,15 @@
 dependencies = [
   "coverage[toml]>=7.2",
   "pytest>=7.3",
   "pytest-cov>=4.0",
   "pytest-dotenv>=0.5",
   "requests-mock>=1.10",
   "time-machine>=2.9",
-  "ruff>=0.0.261",
+  "ruff>=0.0.264",
 ]
 
 [tool.hatch.envs.test.scripts]
 run-coverage = "pytest --cov-config=pyproject.toml --cov=cancelchain"
 run = "run-coverage --no-cov"
 
 # RUFF
```

### Comparing `cancelchain-1.3.1/PKG-INFO` & `cancelchain-1.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cancelchain
-Version: 1.3.1
-Summary: A Blockchain of Accountability, Support, and Forgiveness
+Version: 1.3.2
+Summary: A Blockchain of Accountability, Forgiveness, and Support
 Project-URL: Homepage, https://cancelchain.org
 Project-URL: Documentation, https://docs.cancelchain.org
 Project-URL: Source, https://github.com/cancelchain/cancelchain
 Project-URL: Tracker, https://github.com/cancelchain/cancelchain/issues
 Author-email: Thomas Bohmbach Jr <tom@cancelchain.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -21,26 +21,26 @@
 Requires-Python: >=3.9
 Requires-Dist: base58check>=1.0
 Requires-Dist: blinker>=1.6
 Requires-Dist: celery>=5.2
 Requires-Dist: click>=8.1
 Requires-Dist: flask-caching>=2.0
 Requires-Dist: flask-sqlalchemy>=3.0
-Requires-Dist: flask>=2.2
+Requires-Dist: flask>=2.3
 Requires-Dist: gunicorn>=20.1
 Requires-Dist: humanfriendly>=10.0
 Requires-Dist: marshmallow>=3.19
 Requires-Dist: millify>=0.1
 Requires-Dist: passlib[argon2]>=1.7
 Requires-Dist: pg8000>=1.29
 Requires-Dist: pycryptodome>=3.17
 Requires-Dist: pyjwt>=2.6
 Requires-Dist: pymerkle>=4.0
 Requires-Dist: python-dotenv>=1.0
-Requires-Dist: requests>=2.28
+Requires-Dist: requests>=2.29
 Requires-Dist: rich>=13.3
 Requires-Dist: sqlalchemy<2.0
 Description-Content-Type: text/x-rst
 
 CancelChain
 ###########
 
@@ -109,15 +109,14 @@
 ----------
 
 Create a local database by running the `init command`_:
 
 .. code-block:: console
 
   $ cancelchain init
-  Initialized the database.
 
 The `CC_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
 
 
 Import
 ------
 
@@ -131,79 +130,108 @@
 
 This command could take a while to run depending on your computer and the number of blocks imported. A progress bar will display with estimated time remaining. You can run the ``import`` command multiple times and it will only import new blocks that are not yet in the database.
 
 
 Run
 ---
 
-You run the ``cancelchain`` application by issuing the ``cancelchain run`` command:
+Run the ``cancelchain`` application by issuing the ``run`` command:
 
 .. code-block:: console
 
   $ cancelchain run
-   * Serving Flask app 'cancelchain'
-   * Debug mode: off
-  WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
-   * Running on all addresses (0.0.0.0)
-   * Running on http://127.0.0.1:5000
-  Press CTRL+C to quit
 
 Open `http://localhost:5000 <http://localhost:5000>`_ in a browser to explore the local copy of the blockchain.
 
-Home (Current Chain)
-^^^^^^^^^^^^^^^^^^^^
+Home Page (Current Chain)
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
-.. image:: readme-assets/browser-chain.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-chain.png?raw=true
    :width: 500pt
 
-Block
-^^^^^
+Block Page
+^^^^^^^^^^
 
-.. image:: readme-assets/browser-block.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-block.png?raw=true
    :width: 500pt
 
-Transaction
-^^^^^^^^^^^
+Transaction Page
+^^^^^^^^^^^^^^^^
 
-.. image:: readme-assets/browser-txn.png
+.. image:: https://github.com/cancelchain/cancelchain/blob/7a4fab66dfe6026e56c79df3e147b1ecbdbb6158/readme-assets/browser-txn.png?raw=true
    :width: 500pt
 
-Running the ``cancelchain`` application also exposes a number of web service endpoints that comprise the communications layer of the blockchain. See the  `API Documentation`_ for much more information.
+Running the ``cancelchain`` application also exposes a set of web service endpoints that comprise the communications layer of the blockchain. See the  `API Documentation`_ for more information.
 
-There are also many other ``cancelchain`` commands for interacting with the blockchain. See the `Command Line Interface Documentation`_ or run ``cancelchain --help``.
+There are other ``cancelchain`` commands for interacting with the blockchain. See the `Command Line Interface Documentation`_ for more information or run ``cancelchain --help``.
 
 
 Joining The CancelChain Network
 ===============================
 
-The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
+The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `miller`_ or `transactor`_ role `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
 
-If you would like to be granted API access to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of access you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
+`The Cancel Button`_ allows `reader`_ role `API access`_ to any account that completes at least one transaction on the blockchain:
+
+1) `Register for an account`_.
+2) Submit a successful transaction for any subject. Access won't be granted until the sentiment transaction successfully completes.
+3) Click `Download Account Key`_ on the `Account`_ page to download the account's key (`PEM`_) file.
+4) Create a directory called ``wallets`` and copy the downloaded key file into it.
+5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `Account`_ page and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
+
+  .. code-block:: console
+
+    # Network Settings
+    CC_NODE_HOST=http://CCTheCancelButtonAddressCC@localhost:5000
+    CC_PEERS=["https://CCTheCancelButtonAddressCC@thecancelbutton.com"]
+    CC_DEFAULT_COMMAND_HOST=https://CCTheCancelButtonAddressCC@thecancelbutton.com
+    CC_WALLET_DIR=/path/to/wallets
+
+6) Restart to load the new configuration.
+
+See `Configuration Documentation`_ for more detailed information about these settings.
+
+The `reader`_ role `API access`_ allows the `sync command`_ to update to the most recent peer block data:
+
+.. code-block:: console
+
+  $ cancelchain sync
+
+This command could take a while to run depending on your computer, internet access, and the number of blocks synchronized. A progress bar will display with estimated time remaining. You can run the `sync command`_ multiple times and it will only synchronize new blocks that are not yet in the database.
+
+Reader access also allows querying data (i.e. subject counts and balances) using the CLI. See `Command Line Interface Documentation`_ for more information.
+
+If you would like to be granted other `API access`_ to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of role you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
 
 See the `documentation`_ for some potential development ideas.
 
 
-.. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
+.. _Account: https://thecancelbutton.com/account
 .. _API access: https://docs.cancelchain.org/en/latest/api.html#api-roles
+.. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
 .. _Blog: https://blog.cancelchain.org
 .. _CancelChain data: https://storage.googleapis.com/blocks.cancelchain.org/cancelchain.jsonl
 .. _CC_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
 .. _CC_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
 .. _Command Line Interface Documentation: https://docs.cancelchain.org/en/latest/usage.html#command-line-interface
 .. _Configuration Documentation: https://docs.cancelchain.org/en/latest/usage.html#configuration
 .. _documentation: https://docs.cancelchain.org
 .. _Documentation: https://docs.cancelchain.org
+.. _Download Account Key: https://thecancelbutton.com/pem
 .. _import command: https://docs.cancelchain.org/en/latest/usage.html#import
 .. _init command: https://docs.cancelchain.org/en/latest/usage.html#init
 .. _instance folder: https://flask.palletsprojects.com/en/2.2.x/config/#instance-folders
 .. _JSON Lines: https://jsonlines.org/
 .. _miller: https://docs.cancelchain.org/en/latest/api.html#miller
+.. _PEM: https://en.wikipedia.org/wiki/Privacy-Enhanced_Mail
 .. _Project Home Page: https://cancelchain.org
-.. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _python virtual environment: https://docs.python.org/3/library/venv.html
+.. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _reader: https://docs.cancelchain.org/en/latest/api.html#reader
+.. _Register for an account: https://thecancelbutton.com/register
 .. _running milling processes: https://docs.cancelchain.org/en/latest/usage.html#mill
 .. _shell command: https://flask.palletsprojects.com/en/2.2.x/cli/#open-a-shell
 .. _sock puppet accounts: https://en.wikipedia.org/wiki/Sock_puppet_account
 .. _SQLite: https://sqlite.org/index.html
+.. _sync command: https://docs.cancelchain.org/en/latest/usage.html#sync
 .. _The Cancel Button: https://thecancelbutton.com
 .. _transactor: https://docs.cancelchain.org/en/latest/api.html#transactor
```

