# Comparing `tmp/defichain-3.0.0b0.tar.gz` & `tmp/defichain-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defichain-3.0.0b0.tar", last modified: Thu Mar 23 00:05:07 2023, max compression
+gzip compressed data, was "defichain-3.0.0b1.tar", last modified: Thu May  4 20:14:01 2023, max compression
```

## Comparing `defichain-3.0.0b0.tar` & `defichain-3.0.0b1.tar`

### file list

```diff
@@ -1,199 +1,204 @@
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/
--rw-rw-r--   0 executor  (1000) executor  (1000)     1066 2023-03-22 22:44:20.000000 defichain-3.0.0b0/LICENSE
--rw-rw-r--   0 executor  (1000) executor  (1000)      121 2022-12-10 21:33:06.000000 defichain-3.0.0b0/MANIFEST.in
--rw-rw-r--   0 executor  (1000) executor  (1000)     3493 2023-03-23 00:05:07.600380 defichain-3.0.0b0/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     2723 2022-12-10 21:33:06.000000 defichain-3.0.0b0/README.md
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.588380 defichain-3.0.0b0/defichain/
--rw-rw-r--   0 executor  (1000) executor  (1000)      406 2023-02-21 20:41:21.000000 defichain-3.0.0b0/defichain/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.588380 defichain-3.0.0b0/defichain/exceptions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.588380 defichain-3.0.0b0/defichain/exceptions/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)      427 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/hdwallet/DerivationError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)       96 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/hdwallet/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.588380 defichain-3.0.0b0/defichain/exceptions/http/
--rw-rw-r--   0 executor  (1000) executor  (1000)      199 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/BadMethod.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      249 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/BadRequest.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/Forbidden.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1978 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/HTTPStatusCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      302 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/InternalServerError.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      240 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/NotFound.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3982 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/RPCErrorCode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      220 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/ServiceUnavailable.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      306 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/Unauthorized.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/UnprocessableEntity.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      215 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/WrongParmeters.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      615 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/exceptions/http/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/exceptions/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      430 2023-02-25 15:35:00.000000 defichain-3.0.0b0/defichain/exceptions/transactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      110 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/addresserror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-02-13 02:06:15.000000 defichain-3.0.0b0/defichain/exceptions/transactions/defitxerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      116 2023-02-25 15:35:00.000000 defichain-3.0.0b0/defichain/exceptions/transactions/deserializeerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/inputerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      103 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/keyerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      114 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/notsupported.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      124 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/rawtransactionerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/tokenerror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      112 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/exceptions/transactions/txbuildererror.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-02-13 02:10:22.000000 defichain-3.0.0b0/defichain/exceptions/transactions/verifyerror.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/hdwallet/
--rw-rw-r--   0 executor  (1000) executor  (1000)       93 2023-02-21 17:33:21.000000 defichain-3.0.0b0/defichain/hdwallet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2149 2023-03-20 22:26:11.000000 defichain-3.0.0b0/defichain/hdwallet/account.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3808 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/hdwallet/derivations.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1198 2023-03-14 23:46:26.000000 defichain-3.0.0b0/defichain/hdwallet/encryption.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10519 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/hdwallet/utils.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    55798 2023-02-21 20:38:41.000000 defichain-3.0.0b0/defichain/hdwallet/wallet.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/libs/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2222 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/libs/base58.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4356 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/libs/bech32.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14136 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/libs/ecc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5376 2023-01-30 16:15:03.000000 defichain-3.0.0b0/defichain/libs/ripemd160.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4660 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/logger.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/mnemonic/
--rw-rw-r--   0 executor  (1000) executor  (1000)       32 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10817 2023-03-14 21:50:04.000000 defichain-3.0.0b0/defichain/mnemonic/mnemonic.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/mnemonic/wordlist/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/chinese_simplified.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/chinese_traditional.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13116 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/english.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16776 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/french.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    16033 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/italian.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    26423 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/japanese.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    37832 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/korean.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)    13996 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/mnemonic/wordlist/spanish.txt
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/networks/
--rw-rw-r--   0 executor  (1000) executor  (1000)       84 2023-03-17 23:34:07.000000 defichain-3.0.0b0/defichain/networks/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4060 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/networks/networks.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.592380 defichain-3.0.0b0/defichain/node/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2888 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/RPCErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1081 2022-12-12 22:24:40.000000 defichain-3.0.0b0/defichain/node/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/node/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)    21262 2023-03-18 22:57:44.000000 defichain-3.0.0b0/defichain/node/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    53564 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/blockchain.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5563 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/control.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      856 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/generating.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14857 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8435 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12054 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/mining.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    16833 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/network.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    12270 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    13718 2023-03-18 22:58:05.000000 defichain-3.0.0b0/defichain/node/modules/poolpair.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5632 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/proposals.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    40311 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/rawtransactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      144 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/spv.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2530 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    10291 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8691 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/util.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    15447 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    86413 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/modules/wallet.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      848 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/node/modules/zmq.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6030 2023-01-30 14:33:11.000000 defichain-3.0.0b0/defichain/node/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2114 2023-01-30 14:33:11.000000 defichain-3.0.0b0/defichain/node/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4216 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/node/util.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/ocean/
--rw-rw-r--   0 executor  (1000) executor  (1000)     2775 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/OceanErrorHandler.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      690 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2262 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/connection.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/ocean/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)     6077 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/ocean/modules/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2458 2022-12-28 14:30:10.000000 defichain-3.0.0b0/defichain/ocean/modules/blocks.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      641 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/modules/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6104 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/ocean/modules/loan.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1464 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/modules/masternodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2492 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/ocean/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     7224 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/modules/poolpairs.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5362 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/ocean/modules/prices.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1691 2023-02-14 10:46:13.000000 defichain-3.0.0b0/defichain/ocean/modules/rawTx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      697 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/modules/rpc.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2405 2022-12-23 22:10:17.000000 defichain-3.0.0b0/defichain/ocean/modules/stats.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1588 2022-12-10 21:33:06.000000 defichain-3.0.0b0/defichain/ocean/modules/tokens.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2360 2022-12-28 14:30:13.000000 defichain-3.0.0b0/defichain/ocean/modules/transactions.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2801 2023-02-25 14:42:13.000000 defichain-3.0.0b0/defichain/ocean/ocean.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-11 22:41:37.000000 defichain-3.0.0b0/defichain/transactions/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/address/
--rw-rw-r--   0 executor  (1000) executor  (1000)      288 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/address/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4009 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2702 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/base58address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     5796 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/baseaddress.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2306 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/bech32address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2599 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/p2pkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2535 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/p2sh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2667 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/address/p2wpkh.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1073 2023-03-17 23:40:52.000000 defichain-3.0.0b0/defichain/transactions/address/script.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/builder/
--rw-rw-r--   0 executor  (1000) executor  (1000)       33 2023-03-20 22:03:11.000000 defichain-3.0.0b0/defichain/transactions/builder/__init__.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/builder/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)       77 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/builder/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1881 2023-03-21 23:52:15.000000 defichain-3.0.0b0/defichain/transactions/builder/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1855 2023-03-18 22:53:20.000000 defichain-3.0.0b0/defichain/transactions/builder/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3176 2023-03-22 21:31:49.000000 defichain-3.0.0b0/defichain/transactions/builder/modules/utxo.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4029 2023-03-20 21:51:06.000000 defichain-3.0.0b0/defichain/transactions/builder/rawtransactionbuilder.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6796 2023-03-21 17:54:58.000000 defichain-3.0.0b0/defichain/transactions/builder/txbuilder.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/constants/
--rw-rw-r--   0 executor  (1000) executor  (1000)      373 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/constants/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      245 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/constants/address.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2826 2023-03-11 23:42:53.000000 defichain-3.0.0b0/defichain/transactions/constants/defitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      382 2023-03-17 23:04:52.000000 defichain-3.0.0b0/defichain/transactions/constants/fees.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/constants/mainnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)     8212 2023-03-09 02:47:17.000000 defichain-3.0.0b0/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     8966 2023-03-09 02:47:17.000000 defichain-3.0.0b0/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     5622 2023-03-09 02:47:17.000000 defichain-3.0.0b0/defichain/transactions/constants/mainnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     7116 2023-03-09 02:47:17.000000 defichain-3.0.0b0/defichain/transactions/constants/mainnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-22 23:34:03.000000 defichain-3.0.0b0/defichain/transactions/constants/mainnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3265 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/constants/opcodes.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/constants/rawtransactions.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.596380 defichain-3.0.0b0/defichain/transactions/constants/testnet/
--rw-rw-r--   0 executor  (1000) executor  (1000)    18521 2023-03-09 02:47:21.000000 defichain-3.0.0b0/defichain/transactions/constants/testnet/CUSTOM_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1385 2023-03-09 02:47:21.000000 defichain-3.0.0b0/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)      598 2023-03-09 02:47:21.000000 defichain-3.0.0b0/defichain/transactions/constants/testnet/LOAN_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)     1516 2023-03-09 02:47:21.000000 defichain-3.0.0b0/defichain/transactions/constants/testnet/STANDARD_tokens.json
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-22 23:34:13.000000 defichain-3.0.0b0/defichain/transactions/constants/testnet/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     3321 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/constants/tokens.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/defichain/transactions/defitx/
--rw-rw-r--   0 executor  (1000) executor  (1000)      300 2023-03-20 22:03:11.000000 defichain-3.0.0b0/defichain/transactions/defitx/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2010 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/defitx/builddefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1336 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/defitx/defitx.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/defichain/transactions/defitx/modules/
--rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6516 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/accounts.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      672 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/basedefitx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     6673 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/baseinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      264 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/governance.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      440 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/loans.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      217 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/masternode.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      209 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/oracles.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     9200 2023-03-18 22:25:30.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/pool.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      204 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      358 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/defitx/modules/vault.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4808 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/keys.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/defichain/transactions/rawtransactions/
--rw-rw-r--   0 executor  (1000) executor  (1000)      338 2023-03-17 22:57:36.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      954 2023-03-17 22:57:36.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/fee.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1438 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/sign.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    19717 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/tx.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     4252 2023-03-18 11:20:22.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/txbase.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    14476 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/txinput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)    11295 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/txoutput.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     8303 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/rawtransactions/witness.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/defichain/transactions/remotedata/
--rw-rw-r--   0 executor  (1000) executor  (1000)       89 2023-03-14 15:42:12.000000 defichain-3.0.0b0/defichain/transactions/remotedata/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1432 2023-03-20 22:42:53.000000 defichain-3.0.0b0/defichain/transactions/remotedata/node.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1068 2023-03-22 20:28:01.000000 defichain-3.0.0b0/defichain/transactions/remotedata/ocean.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     1146 2023-03-20 22:42:53.000000 defichain-3.0.0b0/defichain/transactions/remotedata/remotedata.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.600380 defichain-3.0.0b0/defichain/transactions/utils/
--rw-rw-r--   0 executor  (1000) executor  (1000)      236 2023-02-26 18:19:11.000000 defichain-3.0.0b0/defichain/transactions/utils/__init__.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2660 2023-03-17 23:51:59.000000 defichain-3.0.0b0/defichain/transactions/utils/calculate.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2148 2023-03-18 22:07:03.000000 defichain-3.0.0b0/defichain/transactions/utils/converter.py
--rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-03-18 11:40:02.000000 defichain-3.0.0b0/defichain/transactions/utils/token.py
--rw-rw-r--   0 executor  (1000) executor  (1000)      987 2023-02-24 17:37:25.000000 defichain-3.0.0b0/defichain/transactions/utils/verify.py
-drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-03-23 00:05:07.588380 defichain-3.0.0b0/defichain.egg-info/
--rw-rw-r--   0 executor  (1000) executor  (1000)     3493 2023-03-23 00:05:07.000000 defichain-3.0.0b0/defichain.egg-info/PKG-INFO
--rw-rw-r--   0 executor  (1000) executor  (1000)     6733 2023-03-23 00:05:07.000000 defichain-3.0.0b0/defichain.egg-info/SOURCES.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-23 00:05:07.000000 defichain-3.0.0b0/defichain.egg-info/dependency_links.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       57 2023-03-23 00:05:07.000000 defichain-3.0.0b0/defichain.egg-info/requires.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       10 2023-03-23 00:05:07.000000 defichain-3.0.0b0/defichain.egg-info/top_level.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)      174 2022-12-10 21:33:06.000000 defichain-3.0.0b0/pyproject.toml
--rw-rw-r--   0 executor  (1000) executor  (1000)       56 2022-12-10 21:33:06.000000 defichain-3.0.0b0/requirements.txt
--rw-rw-r--   0 executor  (1000) executor  (1000)       38 2023-03-23 00:05:07.600380 defichain-3.0.0b0/setup.cfg
--rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-03-22 23:54:38.000000 defichain-3.0.0b0/setup.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1066 2023-03-23 01:00:00.000000 defichain-3.0.0b1/LICENSE
+-rw-rw-r--   0 executor  (1000) executor  (1000)      121 2022-12-10 21:33:06.000000 defichain-3.0.0b1/MANIFEST.in
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-05-04 20:14:01.230239 defichain-3.0.0b1/PKG-INFO
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2723 2022-12-10 21:33:06.000000 defichain-3.0.0b1/README.md
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      406 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/exceptions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain/exceptions/hdwallet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      427 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/hdwallet/DerivationError.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)       96 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/hdwallet/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.186239 defichain-3.0.0b1/defichain/exceptions/http/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      199 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/BadMethod.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      249 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/BadRequest.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/Forbidden.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1978 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/HTTPStatusCode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      302 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/InternalServerError.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      240 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/NotFound.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3982 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/RPCErrorCode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      220 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/ServiceUnavailable.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      306 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/Unauthorized.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      266 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/UnprocessableEntity.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      215 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/WrongParmeters.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      615 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/exceptions/http/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/exceptions/transactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      430 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      110 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/addresserror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/defitxerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      116 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/deserializeerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/inputerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      103 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/keyerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      114 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/notsupported.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      124 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/rawtransactionerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      105 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/tokenerror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      112 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/txbuildererror.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      106 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/exceptions/transactions/verifyerror.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/hdwallet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       93 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2149 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/account.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3808 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/hdwallet/derivations.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1198 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/hdwallet/encryption.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10519 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/hdwallet/utils.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    55798 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/hdwallet/wallet.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.190239 defichain-3.0.0b1/defichain/libs/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2222 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/base58.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4356 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/bech32.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14136 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/ecc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5376 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/libs/ripemd160.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4660 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/logger.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/mnemonic/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       32 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10817 2023-03-14 21:50:04.000000 defichain-3.0.0b1/defichain/mnemonic/mnemonic.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/mnemonic/wordlist/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_simplified.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8192 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_traditional.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13116 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/english.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16776 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/french.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16033 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/italian.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    26423 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/japanese.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    37832 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/korean.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13996 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/mnemonic/wordlist/spanish.txt
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.194239 defichain-3.0.0b1/defichain/networks/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       84 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/networks/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4060 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/networks/networks.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.198239 defichain-3.0.0b1/defichain/node/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2888 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/RPCErrorHandler.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1081 2022-12-12 22:24:40.000000 defichain-3.0.0b1/defichain/node/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.206239 defichain-3.0.0b1/defichain/node/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)    21262 2023-03-18 22:57:44.000000 defichain-3.0.0b1/defichain/node/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    53564 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/blockchain.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5563 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/control.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      856 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/generating.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14857 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/loan.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8435 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/masternodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    12054 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/mining.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16833 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/network.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    12270 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    13718 2023-03-18 22:58:05.000000 defichain-3.0.0b1/defichain/node/modules/poolpair.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5632 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/proposals.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    40311 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/rawtransactions.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      144 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/spv.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2530 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/stats.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    10291 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/tokens.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8691 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/util.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    15447 2023-04-24 23:36:41.000000 defichain-3.0.0b1/defichain/node/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    86413 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/modules/wallet.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      848 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/node/modules/zmq.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6802 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/node/node.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2182 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/node/rpc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4216 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/node/util.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.206239 defichain-3.0.0b1/defichain/ocean/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2775 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/OceanErrorHandler.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      806 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2357 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/connection.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.210239 defichain-3.0.0b1/defichain/ocean/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6077 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2458 2022-12-28 14:30:10.000000 defichain-3.0.0b1/defichain/ocean/modules/blocks.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2163 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/modules/consortium.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      641 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/fee.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5499 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/modules/governance.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6104 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/loan.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1464 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/masternodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2492 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7224 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/poolpairs.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5362 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/prices.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1691 2023-02-14 10:46:13.000000 defichain-3.0.0b1/defichain/ocean/modules/rawTx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      697 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/rpc.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2405 2022-12-23 22:10:17.000000 defichain-3.0.0b1/defichain/ocean/modules/stats.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1588 2022-12-10 21:33:06.000000 defichain-3.0.0b1/defichain/ocean/modules/tokens.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2360 2022-12-28 14:30:13.000000 defichain-3.0.0b1/defichain/ocean/modules/transactions.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2973 2023-04-24 22:47:23.000000 defichain-3.0.0b1/defichain/ocean/ocean.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.210239 defichain-3.0.0b1/defichain/transactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.214239 defichain-3.0.0b1/defichain/transactions/address/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      288 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4009 2023-04-29 17:23:24.000000 defichain-3.0.0b1/defichain/transactions/address/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2667 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/address/base58address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5796 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/baseaddress.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2306 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/bech32address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3320 2023-05-01 20:04:00.000000 defichain-3.0.0b1/defichain/transactions/address/p2pkh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2535 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/p2sh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3073 2023-04-29 17:19:29.000000 defichain-3.0.0b1/defichain/transactions/address/p2wpkh.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1073 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/address/script.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.214239 defichain-3.0.0b1/defichain/transactions/builder/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       33 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/__init__.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.218239 defichain-3.0.0b1/defichain/transactions/builder/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      163 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1881 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2028 2023-04-24 23:35:56.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/loans.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1341 2023-04-29 16:28:12.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/masternode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4685 2023-04-01 19:19:45.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/pool.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3176 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/utxo.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:52:35.000000 defichain-3.0.0b1/defichain/transactions/builder/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5465 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/rawtransactionbuilder.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6932 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/builder/txbuilder.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.218239 defichain-3.0.0b1/defichain/transactions/constants/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      440 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      245 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/address.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2511 2023-04-13 22:45:28.000000 defichain-3.0.0b1/defichain/transactions/constants/defitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      382 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/fees.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/constants/mainnet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8734 2023-04-29 16:23:23.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     9370 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     5622 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/LOAN_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7346 2023-03-26 16:27:39.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/mainnet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3265 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/opcodes.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      188 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/rawtransactions.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/constants/testnet/
+-rw-rw-r--   0 executor  (1000) executor  (1000)    18208 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1630 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      598 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/LOAN_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1623 2023-03-26 16:27:43.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/STANDARD_tokens.json
+-rw-rw-r--   0 executor  (1000) executor  (1000)      177 2023-04-01 23:11:49.000000 defichain-3.0.0b1/defichain/transactions/constants/testnet/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3321 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/constants/tokens.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.222239 defichain-3.0.0b1/defichain/transactions/defitx/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      300 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2010 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/builddefitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2863 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/defitx/defitx.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.226239 defichain-3.0.0b1/defichain/transactions/defitx/modules/
+-rw-rw-r--   0 executor  (1000) executor  (1000)        0 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6516 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/accounts.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      672 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/basedefitx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     7538 2023-04-13 22:18:28.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/baseinput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      264 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/governance.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8707 2023-04-24 23:35:56.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/loans.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6124 2023-04-29 17:26:17.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/masternode.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      209 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/oracles.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    16975 2023-04-13 22:05:54.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/pool.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      204 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/token.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     9907 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/defitx/modules/vault.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4808 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/keys.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.226239 defichain-3.0.0b1/defichain/transactions/rawtransactions/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      338 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      954 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/fee.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1438 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/sign.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    19708 2023-04-01 19:35:42.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/tx.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     4252 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txbase.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    14476 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txinput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)    11292 2023-04-01 16:54:42.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/txoutput.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     8303 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/rawtransactions/witness.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/defichain/transactions/remotedata/
+-rw-rw-r--   0 executor  (1000) executor  (1000)       89 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/remotedata/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1747 2023-04-30 09:04:11.000000 defichain-3.0.0b1/defichain/transactions/remotedata/node.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1332 2023-04-29 16:23:24.000000 defichain-3.0.0b1/defichain/transactions/remotedata/ocean.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     1469 2023-05-01 20:06:53.000000 defichain-3.0.0b1/defichain/transactions/remotedata/remotedata.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.230239 defichain-3.0.0b1/defichain/transactions/utils/
+-rw-rw-r--   0 executor  (1000) executor  (1000)      236 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/utils/__init__.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3239 2023-04-01 17:21:08.000000 defichain-3.0.0b1/defichain/transactions/utils/calculate.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2634 2023-04-12 23:08:52.000000 defichain-3.0.0b1/defichain/transactions/utils/converter.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3017 2023-03-31 19:16:18.000000 defichain-3.0.0b1/defichain/transactions/utils/token.py
+-rw-rw-r--   0 executor  (1000) executor  (1000)      987 2023-03-23 01:00:00.000000 defichain-3.0.0b1/defichain/transactions/utils/verify.py
+drwxrwxr-x   0 executor  (1000) executor  (1000)        0 2023-05-04 20:14:01.182239 defichain-3.0.0b1/defichain.egg-info/
+-rw-rw-r--   0 executor  (1000) executor  (1000)     3456 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/PKG-INFO
+-rw-rw-r--   0 executor  (1000) executor  (1000)     6958 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/SOURCES.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)        1 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/dependency_links.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       57 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/requires.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       10 2023-05-04 20:14:01.000000 defichain-3.0.0b1/defichain.egg-info/top_level.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)      174 2022-12-10 21:33:06.000000 defichain-3.0.0b1/pyproject.toml
+-rw-rw-r--   0 executor  (1000) executor  (1000)       56 2022-12-10 21:33:06.000000 defichain-3.0.0b1/requirements.txt
+-rw-rw-r--   0 executor  (1000) executor  (1000)       38 2023-05-04 20:14:01.230239 defichain-3.0.0b1/setup.cfg
+-rw-rw-r--   0 executor  (1000) executor  (1000)     2717 2023-05-04 20:13:13.000000 defichain-3.0.0b1/setup.py
```

### Comparing `defichain-3.0.0b0/LICENSE` & `defichain-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/PKG-INFO` & `defichain-3.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
-License: UNKNOWN
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -61,9 +59,7 @@
 or other ideas open an [issue](https://github.com/eric-volz/DefichainPython/issues), 
 write me on [Twitter](https://twitter.com/Intr0c) or via email (introc@volz.link)!
 
 ## [License & Disclaimer](https://docs.defichain-python.de/build/html/legal/licenseAndDisclaimer.html)
 
 By using (this repo), you (the user) agree to be bound by the 
 [terms of this license](https://github.com/eric-volz/defichainLibrary/blob/main/LICENSE) (MIT License).
-
-
```

### Comparing `defichain-3.0.0b0/README.md` & `defichain-3.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/exceptions/http/HTTPStatusCode.py` & `defichain-3.0.0b1/defichain/exceptions/http/HTTPStatusCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/exceptions/http/RPCErrorCode.py` & `defichain-3.0.0b1/defichain/exceptions/http/RPCErrorCode.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/exceptions/http/__init__.py` & `defichain-3.0.0b1/defichain/exceptions/http/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/hdwallet/account.py` & `defichain-3.0.0b1/defichain/hdwallet/account.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/hdwallet/derivations.py` & `defichain-3.0.0b1/defichain/hdwallet/derivations.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/hdwallet/encryption.py` & `defichain-3.0.0b1/defichain/hdwallet/encryption.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/hdwallet/utils.py` & `defichain-3.0.0b1/defichain/hdwallet/utils.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/hdwallet/wallet.py` & `defichain-3.0.0b1/defichain/hdwallet/wallet.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/libs/base58.py` & `defichain-3.0.0b1/defichain/libs/base58.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/libs/bech32.py` & `defichain-3.0.0b1/defichain/libs/bech32.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/libs/ecc.py` & `defichain-3.0.0b1/defichain/libs/ecc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/libs/ripemd160.py` & `defichain-3.0.0b1/defichain/libs/ripemd160.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/logger.py` & `defichain-3.0.0b1/defichain/logger.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/mnemonic.py` & `defichain-3.0.0b1/defichain/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/chinese_simplified.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/chinese_traditional.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/english.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/french.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/italian.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/japanese.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/korean.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/mnemonic/wordlist/spanish.txt` & `defichain-3.0.0b1/defichain/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/networks/networks.py` & `defichain-3.0.0b1/defichain/networks/networks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/RPCErrorHandler.py` & `defichain-3.0.0b1/defichain/node/RPCErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/__init__.py` & `defichain-3.0.0b1/defichain/node/__init__.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/accounts.py` & `defichain-3.0.0b1/defichain/node/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/blockchain.py` & `defichain-3.0.0b1/defichain/node/modules/blockchain.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/control.py` & `defichain-3.0.0b1/defichain/node/modules/control.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/generating.py` & `defichain-3.0.0b1/defichain/node/modules/generating.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/loan.py` & `defichain-3.0.0b1/defichain/node/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/masternodes.py` & `defichain-3.0.0b1/defichain/node/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/mining.py` & `defichain-3.0.0b1/defichain/node/modules/mining.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/network.py` & `defichain-3.0.0b1/defichain/node/modules/network.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/oracles.py` & `defichain-3.0.0b1/defichain/node/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/poolpair.py` & `defichain-3.0.0b1/defichain/node/modules/poolpair.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/proposals.py` & `defichain-3.0.0b1/defichain/node/modules/proposals.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/rawtransactions.py` & `defichain-3.0.0b1/defichain/node/modules/rawtransactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/stats.py` & `defichain-3.0.0b1/defichain/node/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/tokens.py` & `defichain-3.0.0b1/defichain/node/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/util.py` & `defichain-3.0.0b1/defichain/node/modules/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/vault.py` & `defichain-3.0.0b1/defichain/node/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/wallet.py` & `defichain-3.0.0b1/defichain/node/modules/wallet.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/modules/zmq.py` & `defichain-3.0.0b1/defichain/node/modules/zmq.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/node/node.py` & `defichain-3.0.0b1/defichain/node/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,16 @@
             >>> node = Node(user="user", password="password", url="127.0.0.1", port=8554, wallet_name="myWallet", wallet_password="yourPassword", wallet_timeout=60)
             >>> blockcount = node.blockchain.getblockcount()  #  returns block height of the latest block
             >>> print(blockcount)
     """
 
     def __init__(self, user: str, password: str, url: str = "127.0.0.1", port: int = 8554, wallet_name: str = "",
                  wallet_path: str = None, wallet_password: str = "", wallet_timeout: int = 60,
-                 protocol: str = "http", logger: Logger = None) -> "Node":
+                 protocol: str = "http", logger: Logger = None):
+
         # Parameter Check
         if wallet_name != "" and wallet_path is not None:
             raise WrongParameters(f"Only one parameter of wallet_name or wallet_path may be given at a time!")
         elif wallet_name == "" and wallet_path is not None:
             wallet_name = wallet_path
 
         # Setup URL
@@ -100,14 +101,28 @@
         self.vault = Vault(self)
         self.wallet = Wallet(self)
         self.zmq = Zmq(self)
 
         # Test Connection to Node
         self.test_connection()
 
+        # Check if only one wallet
+        wallets = self.wallet.listwallets()
+        if len(wallets) == 1:  # Only one wallet is loaded
+            url = f"{protocol}://{user}:{password}@{url}:{port}/wallet/{wallets[0]}"
+            self._rpc.update_url(url)
+        # If more than one wallet is loaded the default wallet "" will be used. If you want tu use a specific wallet you
+        # have zu specify the wallet in the wallet_name parameter
+        elif len(wallets) > 1 and not "" in wallets:
+            msg = "Warning: You have not specified an wallet in the wallet_name parameter. If you use an method where " \
+                  "an wallet is needed an error will accrue!"
+            print(msg)
+            if logger:
+                logger.error("NodeWarning", msg)
+
         # Prepare Wallet
         self.load_wallet(wallet_path)
         self.decrypt_wallet(wallet_password, wallet_timeout)
 
     def decrypt_wallet(self, wallet_password: str, wallet_timeout: int):
         """
         Decrypts wallet for a specific time if a password is given
```

### Comparing `defichain-3.0.0b0/defichain/node/rpc.py` & `defichain-3.0.0b1/defichain/node/rpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             if param is not None:
                 filtered_params.append(param)
 
         payload = json.dumps({"method": rpc_method, "params": list(filtered_params), "jsonrpc": "2.0"})
         tries = 3
         hadConnectionFailures = False
 
-        # Logging of Ocean get request url
+        # Logging of Node get request url
         if self._logger:
             if self._logger.log_level == "input" or self._logger.log_level == "all":
                 self._logger.input("NodeInput", f"Node request URL: {self._url} | Headers: {self._headers} | Payload: {payload}")
 
         while True:
             try:
                 response = self._session.post(self._url, headers=self._headers, data=payload)
@@ -49,7 +49,10 @@
 
         # Logging of Ocean get request result
         if self._logger:
             if self._logger.log_level == "output" or self._logger.log_level == "all":
                 self._logger.output("NodeOutput", f"Node requests result: {result}")
 
         return result
+
+    def update_url(self, url: str) -> None:
+        self._url = url
```

### Comparing `defichain-3.0.0b0/defichain/node/util.py` & `defichain-3.0.0b1/defichain/node/util.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/OceanErrorHandler.py` & `defichain-3.0.0b1/defichain/ocean/OceanErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/__init__.py` & `defichain-3.0.0b1/defichain/ocean/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Just to be present: Ocean
 from defichain.ocean.modules.address import Address
 from defichain.ocean.modules.blocks import Blocks
+from defichain.ocean.modules.consortium import Consortium
 from defichain.ocean.modules.fee import Fee
+from defichain.ocean.modules.governance import Governance
 from defichain.ocean.modules.loan import Loan
 from defichain.ocean.modules.masternodes import Masternodes
 from defichain.ocean.modules.oracles import Oracles
 from defichain.ocean.modules.poolpairs import Poolpairs
 from defichain.ocean.modules.prices import Prices
 from defichain.ocean.modules.rawTx import RawTx
 from defichain.ocean.modules.rpc import Rpc
```

### Comparing `defichain-3.0.0b0/defichain/ocean/connection.py` & `defichain-3.0.0b1/defichain/ocean/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,26 @@
     def __init__(self, url, logger: Logger):
         self._url = url
         self._session = requests.Session()
         self._headers = {'content-type': 'application/json'}
         self._logger = logger
 
     def get(self, data, size=None, next=None):
+        if "?" in data:
+            sep = "&"
+        else:
+            sep = "?"
+
         url = self._url + data
         if size is not None and next is not None:
-            url += f"?size={size}&next={next}"
+            url += f"{sep}size={size}&next={next}"
         elif size is not None:
-            url += f"?size={size}"
+            url += f"{sep}size={size}"
         elif next is not None:
-            url += f"?next={next}"
+            url += f"{sep}next={next}"
 
         # Logging of Ocean get request url
         if self._logger:
             if self._logger.log_level == "input" or self._logger.log_level == "all":
                 self._logger.input("OceanInput", f"Get request url: {url}")
 
         response = requests.get(url)
```

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/address.py` & `defichain-3.0.0b1/defichain/ocean/modules/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/blocks.py` & `defichain-3.0.0b1/defichain/ocean/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/fee.py` & `defichain-3.0.0b1/defichain/ocean/modules/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/loan.py` & `defichain-3.0.0b1/defichain/ocean/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/masternodes.py` & `defichain-3.0.0b1/defichain/ocean/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/oracles.py` & `defichain-3.0.0b1/defichain/ocean/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/poolpairs.py` & `defichain-3.0.0b1/defichain/ocean/modules/poolpairs.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/prices.py` & `defichain-3.0.0b1/defichain/ocean/modules/prices.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/rawTx.py` & `defichain-3.0.0b1/defichain/ocean/modules/rawTx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/rpc.py` & `defichain-3.0.0b1/defichain/ocean/modules/rpc.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/stats.py` & `defichain-3.0.0b1/defichain/ocean/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/tokens.py` & `defichain-3.0.0b1/defichain/ocean/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/modules/transactions.py` & `defichain-3.0.0b1/defichain/ocean/modules/transactions.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/ocean/ocean.py` & `defichain-3.0.0b1/defichain/ocean/ocean.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 from defichain.logger import Logger
 from .connection import Connection
 
 from .modules.address import Address
 from .modules.blocks import Blocks
+from .modules.consortium import Consortium
 from .modules.fee import Fee
+from .modules.governance import Governance
 from .modules.loan import Loan
 from .modules.masternodes import Masternodes
 from .modules.oracles import Oracles
 from .modules.poolpairs import Poolpairs
 from .modules.prices import Prices
 from .modules.rawTx import RawTx
 from .modules.rpc import Rpc
@@ -48,15 +50,17 @@
         self._attachedURL = url + "/" + version + "/" + network + "/"
         self._test_connection()
 
         self._conn = Connection(self._attachedURL, logger)
 
         self.address = Address(self)
         self.blocks = Blocks(self)
+        self.consortium = Consortium(self)
         self.fee = Fee(self)
+        self.governance = Governance(self)
         self.loan = Loan(self)
         self.masternodes = Masternodes(self)
         self.oracles = Oracles(self)
         self.poolpairs = Poolpairs(self)
         self.prices = Prices(self)
         self.rawTx = RawTx(self)
         self.rpc = Rpc(self)
```

### Comparing `defichain-3.0.0b0/defichain/transactions/address/address.py` & `defichain-3.0.0b1/defichain/transactions/address/address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/address/base58address.py` & `defichain-3.0.0b1/defichain/transactions/address/base58address.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         return base58.decode(address).hex()
 
     @staticmethod
     def encode(network: Any, scriptPublicKey: str) -> str:
         return base58.check_encode(Converter.hex_to_bytes(scriptPublicKey))
 
     @staticmethod
-    def scriptPublicKey_to_address(network: Any,
-                                   scriptPublicKey: str) -> str:
+    def scriptPublicKey_to_address(network: Any, scriptPublicKey: str) -> str:
         Base58Address._is_scriptPublicKey(scriptPublicKey)
         if scriptPublicKey[0:6] == "76a914":  # P2PKH
             script = Converter.int_to_hex(network.PUBLIC_KEY_ADDRESS, 1) + scriptPublicKey[6:46]
             return Base58Address.encode(network, script)
         elif scriptPublicKey[0:4] == "a914":  # P2SH
             script = Converter.int_to_hex(network.SCRIPT_ADDRESS, 1) + scriptPublicKey[4:44]
             return Base58Address.encode(network, script)
```

### Comparing `defichain-3.0.0b0/defichain/transactions/address/baseaddress.py` & `defichain-3.0.0b1/defichain/transactions/address/baseaddress.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/address/bech32address.py` & `defichain-3.0.0b1/defichain/transactions/address/bech32address.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/address/p2pkh.py` & `defichain-3.0.0b1/defichain/transactions/address/p2wpkh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 from typing import Any
 
 from defichain.networks import Network
 from defichain.transactions.constants import AddressTypes, OPCodes
 from defichain.transactions.keys import PrivateKey, PublicKey
-from .base58address import Base58Address
+from .bech32address import Bech32Address
 from .script import Script
 
 
-class P2PKH(Base58Address):  # Legacy
-
+class P2WPKH(Bech32Address):  # Native Segwit
     @staticmethod
-    def from_publicKey(network: Any, publicKey: str) -> "P2PKH":
+    def from_publicKey(network: Any, publicKey: str) -> "P2WPKH":
         """
-        Generates a P2PKH address object from the given public key
+        Generates a P2WPKH address object from the given public key
 
         :param network: (required) The network in witch the public key should be used
         :type network: Network
         :param publicKey: (required) public key
         :type publicKey: str
-        :return: P2PKH - returns the P2PKH address object
+        :return: P2WPKH - returns the P2WPKH address object
         """
-        return P2PKH(network, PublicKey(network, publicKey).p2pkh_address())
+        return P2WPKH(network, PublicKey(network, publicKey).p2wpkh_address())
 
     @staticmethod
-    def from_privateKey(network: Any, privateKey: str) -> "P2PKH":
+    def from_privateKey(network: Any, privateKey: str) -> "P2WPKH":
         """
-        Generates a P2PKH address object from the given private key
+        Generates a P2WPKH address object from the given private key
 
         :param network: (required) The network in witch the private key should be used
         :type network: Network
         :param privateKey: (required) private key
         :type privateKey: str
-        :return: P2PKH - returns the P2PKH address object
+        :return: P2WPKH - returns the P2WPKH address object
         """
-        return P2PKH(network, PrivateKey(network, privateKey).p2pkh_address())
+        return P2WPKH(network, PrivateKey(network, privateKey).p2wpkh_address())
 
     @staticmethod
-    def from_scriptPublicKey(network: Any, scriptPublicKey: str) -> "P2PKH":
+    def from_scriptPublicKey(network: Any, scriptPublicKey: str) -> "P2WPKH":
         """
-        Generates a P2PKH address object from the given script private key
+        Generates a P2WPKH address object from the given script private key
 
         :param network: (required) The network in witch the script public key should be used
         :type network: Network
         :param scriptPublicKey: (required) script public key
         :type scriptPublicKey: str
-        :return: P2PKH - returns the P2PKH address object
+        :return: P2WPKH - returns the P2WPKH address object
         """
-        return P2PKH(network, Base58Address.scriptPublicKey_to_address(network, scriptPublicKey))
+        return P2WPKH(network, Bech32Address.scriptPublicKey_to_address(network, scriptPublicKey))
+
+    @staticmethod
+    def from_publicKeyHash(network: Any, publicKeyHash: str) -> "P2WPKH":
+        address = Bech32Address.encode(network, "0014" + publicKeyHash)
+        return P2WPKH(network, address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network, address)
 
     def get_addressType(self) -> str:
-        return AddressTypes.P2PKH
+        return AddressTypes.P2WPKH
 
     def get_scriptPublicKey(self) -> str:
-        return Script.build_script([OPCodes.OP_DUP, OPCodes.OP_HASH160, Base58Address.decode(self.get_address())[2:42],
-                                    OPCodes.OP_EQUALVERIFY, OPCodes.OP_CHECKSIG])
+        return Script.build_script([OPCodes.OP_0, Bech32Address.decode(self.get_address())])
 
     def get_redeemScript(self) -> str:
-        return self.get_scriptPublicKey()
+        return Script.build_script([OPCodes.OP_DUP, OPCodes.OP_HASH160, Bech32Address.decode(self.get_address()),
+                                    OPCodes.OP_EQUALVERIFY, OPCodes.OP_CHECKSIG])
+
+    def get_publicKeyHash(self) -> str:
+        return Bech32Address.decode(self.get_address())
 
     def get_bytes_scriptPublicKey(self) -> bytes:
         return bytes.fromhex(self.get_scriptPublicKey())
 
     def get_bytes_redeemScript(self) -> bytes:
         return bytes.fromhex(self.get_redeemScript())
 
-
+    def get_bytes_publicKeyHash(self) -> bytes:
+        return bytes.fromhex(self.get_publicKeyHash())
```

### Comparing `defichain-3.0.0b0/defichain/transactions/address/p2sh.py` & `defichain-3.0.0b1/defichain/transactions/address/p2sh.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/address/p2wpkh.py` & `defichain-3.0.0b1/defichain/transactions/address/p2pkh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,90 @@
 from typing import Any
 
+import hashlib
+import binascii
+
 from defichain.networks import Network
 from defichain.transactions.constants import AddressTypes, OPCodes
 from defichain.transactions.keys import PrivateKey, PublicKey
-from .bech32address import Bech32Address
+from defichain.libs import base58
+from .base58address import Base58Address
 from .script import Script
 
 
-class P2WPKH(Bech32Address):  # Native Segwit
+class P2PKH(Base58Address):  # Legacy
+
     @staticmethod
-    def from_publicKey(network: Any, publicKey: str) -> "P2WPKH":
+    def from_publicKey(network: Any, publicKey: str) -> "P2PKH":
         """
-        Generates a P2WPKH address object from the given public key
+        Generates a P2PKH address object from the given public key
 
         :param network: (required) The network in witch the public key should be used
         :type network: Network
         :param publicKey: (required) public key
         :type publicKey: str
-        :return: P2WPKH - returns the P2WPKH address object
+        :return: P2PKH - returns the P2PKH address object
         """
-        return P2WPKH(network, PublicKey(network, publicKey).p2wpkh_address())
+        return P2PKH(network, PublicKey(network, publicKey).p2pkh_address())
 
     @staticmethod
-    def from_privateKey(network: Any, privateKey: str) -> "P2WPKH":
+    def from_privateKey(network: Any, privateKey: str) -> "P2PKH":
         """
-        Generates a P2WPKH address object from the given private key
+        Generates a P2PKH address object from the given private key
 
         :param network: (required) The network in witch the private key should be used
         :type network: Network
         :param privateKey: (required) private key
         :type privateKey: str
-        :return: P2WPKH - returns the P2WPKH address object
+        :return: P2PKH - returns the P2PKH address object
         """
-        return P2WPKH(network, PrivateKey(network, privateKey).p2wpkh_address())
+        return P2PKH(network, PrivateKey(network, privateKey).p2pkh_address())
 
     @staticmethod
-    def from_scriptPublicKey(network: Any, scriptPublicKey: str) -> "P2WPKH":
+    def from_scriptPublicKey(network: Any, scriptPublicKey: str) -> "P2PKH":
         """
-        Generates a P2WPKH address object from the given script private key
+        Generates a P2PKH address object from the given script private key
 
         :param network: (required) The network in witch the script public key should be used
         :type network: Network
         :param scriptPublicKey: (required) script public key
         :type scriptPublicKey: str
-        :return: P2WPKH - returns the P2WPKH address object
+        :return: P2PKH - returns the P2PKH address object
         """
-        return P2WPKH(network, Bech32Address.scriptPublicKey_to_address(network, scriptPublicKey))
+        return P2PKH(network, Base58Address.scriptPublicKey_to_address(network, scriptPublicKey))
+
+    @staticmethod
+    def from_publicKeyHash(network: Any, publicKeyHash: str) -> "P2PKH":
+        checksumHash = "12" + publicKeyHash
+        for _ in range(2):
+            checksumHash = hashlib.sha256(binascii.unhexlify(checksumHash)).hexdigest()
+        checksum = checksumHash[:8]
+        hash = "12" + publicKeyHash + checksum
+        address = base58.encode(bytes.fromhex(hash))
+        return P2PKH(network, address)
 
     def __init__(self, network: Any, address: str):
         super().__init__(network, address)
 
     def get_addressType(self) -> str:
-        return AddressTypes.P2WPKH
+        return AddressTypes.P2PKH
 
     def get_scriptPublicKey(self) -> str:
-        return Script.build_script([OPCodes.OP_0, Bech32Address.decode(self.get_address())])
+        return Script.build_script([OPCodes.OP_DUP, OPCodes.OP_HASH160, Base58Address.decode(self.get_address())[2:42],
+                                    OPCodes.OP_EQUALVERIFY, OPCodes.OP_CHECKSIG])
 
     def get_redeemScript(self) -> str:
-        return Script.build_script([OPCodes.OP_DUP, OPCodes.OP_HASH160, Bech32Address.decode(self.get_address()),
-                                    OPCodes.OP_EQUALVERIFY, OPCodes.OP_CHECKSIG])
+        return self.get_scriptPublicKey()
+
+    def get_publicKeyHash(self) -> str:
+        return Base58Address.decode(self.get_address())[2:42]
 
     def get_bytes_scriptPublicKey(self) -> bytes:
         return bytes.fromhex(self.get_scriptPublicKey())
 
     def get_bytes_redeemScript(self) -> bytes:
         return bytes.fromhex(self.get_redeemScript())
+
+    def get_bytes_publicKeyHash(self) -> bytes:
+        return bytes.fromhex(Base58Address.decode(self.get_address())[2:42])
+
+
```

### Comparing `defichain-3.0.0b0/defichain/transactions/address/script.py` & `defichain-3.0.0b1/defichain/transactions/address/script.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/builder/modules/accounts.py` & `defichain-3.0.0b1/defichain/transactions/builder/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/builder/modules/utxo.py` & `defichain-3.0.0b1/defichain/transactions/builder/modules/utxo.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/builder/rawtransactionbuilder.py` & `defichain-3.0.0b1/defichain/transactions/builder/rawtransactionbuilder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from defichain import Account
 from defichain.exceptions.transactions import TxBuilderError, NotYetSupportedError
 
 from defichain.transactions.address import Address
-from defichain.transactions.constants import AddressTypes
+from defichain.transactions.constants import AddressTypes, DefiTxType
 from defichain.networks import Network
 from defichain.transactions.remotedata.remotedata import RemoteData
-from defichain.transactions.rawtransactions import Transaction, TxP2WPKHInput, TxP2SHInput, TxAddressOutput, \
+from defichain.transactions.rawtransactions import Transaction, TxInput, TxP2WPKHInput, TxP2SHInput, TxAddressOutput, \
     TxDefiOutput, estimate_fee
 from defichain.transactions.defitx.modules.basedefitx import BaseDefiTx
 
 
 class RawTransactionBuilder:
 
     @staticmethod
@@ -22,57 +22,88 @@
         self.set_account(account)
         self.set_dataSource(dataSource)
         self.set_feePerByte(feePerByte)
 
     # Build Transaction
     def build_transactionInputs(self, inputs=[]) -> Transaction:
         tx = self.new_transaction()
+
         if inputs or self.get_dataSource() is None:
             tx.set_inputs(inputs)
         else:
             for input in self.get_dataSource().get_unspent(self.get_address()):
                 address = Address.from_scriptPublicKey(self.get_account().get_network(), input["scriptPubKey"])
                 # Build P2PKH Input
                 if address.get_addressType() == AddressTypes.P2PKH:
                     raise NotYetSupportedError()
                 # Build P2SH Input
                 elif address.get_addressType() == AddressTypes.P2SH:
                     tx.add_input(TxP2SHInput(input["txid"], input["vout"], self.get_account().get_p2wpkh(),
                                              input["value"]))
-                # build P2WPKH Input
+                # Build P2WPKH Input
                 elif address.get_addressType() == AddressTypes.P2WPKH:
                     tx.add_input(TxP2WPKHInput(input["txid"], input["vout"], self.get_address(), input["value"]))
+            # Check Inputs for masternode collateral
+            tx.set_inputs(self.checkMasternodeInputs(tx.get_inputs()))
         return tx
 
     def build_defiTx(self, value: int, defiTx: BaseDefiTx, inputs=[]) -> Transaction:
         tx = self.build_transactionInputs(inputs)
-        defitx_output = TxDefiOutput(value, defiTx)
+
+        # Check for errors in Inputs
+        # Check masternode creation errors
+        if defiTx.get_defiTxType() == DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE:
+            if tx.get_inputsValue() - value < 2000000000000:
+                raise TxBuilderError("The address holds not enough DFI to create a masternode")
+            if tx.get_inputsValue() < 2001000000000:
+                raise TxBuilderError("The address holds not enough DFI to pay the 10 DFI fee to create a masternode")
         if tx.get_inputsValue() - value < 0:
             raise TxBuilderError("The value of the output is bigger then the value of the input")
+        # Adding Outputs to the transaction
+        # DefiTx Output
+        defitxOutput = TxDefiOutput(value, defiTx)
+        tx.add_output(defitxOutput)
+
+        # Masternode Output
+        if defiTx.get_defiTxType() == DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE:
+            masternodeOutput = TxAddressOutput(2000000000000, self.get_address())
+            value = masternodeOutput.get_value() + value
+            tx.add_output(masternodeOutput)
 
+        # Change Output
         change_output = TxAddressOutput(tx.get_inputsValue() - value, self.get_address())
-        tx.add_output(defitx_output)
         tx.add_output(change_output)
 
         # Calculate fee
         fee = estimate_fee(tx, self.get_feePerByte())
 
         # Subtract fee from output
-        value = tx.get_outputs()[1].get_value() - fee
+        value = tx.get_outputs()[-1].get_value() - fee
         if value < 0:
             raise TxBuilderError("The used address has not enough UTXO to pay the transaction fee")
-        tx.get_outputs()[1].set_value(value)
+        tx.get_outputs()[-1].set_value(value)
 
         # Sign and Return
         self.sign(tx)
         return tx
 
     def sign(self, tx: Transaction) -> None:
         tx.sign(self.get_account().get_network(), [self.get_account().get_privateKey()])
 
+    def checkMasternodeInputs(self, inputs: [TxInput]) -> []:
+        newInputs = []
+        for input in inputs:
+            # Check Value
+            if input.get_value() == 2000000000000:
+                # Check transaction txid with data source
+                if self.get_dataSource().check_masternode(input.get_txid()):
+                    continue
+            newInputs.append(input)
+        return newInputs
+
     # Get Information
     def get_address(self) -> str:
         return self._address
 
     def get_addressType(self) -> str:
         return Address.from_address(self.get_address()).get_addressType()
```

### Comparing `defichain-3.0.0b0/defichain/transactions/builder/txbuilder.py` & `defichain-3.0.0b1/defichain/transactions/builder/txbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,20 @@
         self._set_feePerByte(feePerByte)
 
         self._builder = RawTransactionBuilder(self.get_address(), self.get_account(), self.get_dataSource(),
                                               self.get_feePerByte())
 
         self.utxo = UTXO(self._builder)
         self.accounts = Accounts(self._builder)
+        self.loan = Loans(self._builder)
+        self.masternode = Masternode(self._builder)
         self.pool = Pool(self._builder)
 
+        self.vault = Vault(self._builder)
+
         # Verify if address is represented by provided account
         self._verify()
 
     # Methods
     def send_tx(self, tx: "Transaction | str", maxFeeRate: float = None) -> str:
         """
         Broadcasts the created transaction to the blockchain using the provided data source
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/defitx.py` & `defichain-3.0.0b1/defichain/transactions/constants/defitx.py`

 * *Files 21% similar despite different names*

```diff
@@ -59,30 +59,18 @@
     OP_DEFI_TX_TOKEN_UPDATE: str = "4e"  # N
     OP_DEFI_TX_TOKEN_UPDATE_ANY: str = "6e"  # n
 
     # Vault
     OP_DEFI_TX_CREATE_VAULT: str = "56"  # V
     OP_DEFI_TX_UPDATE_VAULT: str = "76"  # v
     OP_DEFI_TX_DEPOSIT_TO_VAULT: str = "53"  # S
-    OP_DEFI_TX_WITHDRAW_FROM_VAULT: str = "4A"  # J
+    OP_DEFI_TX_WITHDRAW_FROM_VAULT: str = "4a"  # J
     OP_DEFI_TX_CLOSE_VAULT: str = "65"  # e
     OP_DEFI_TX_AUCTION_BID: str = "49"  # I
 
     @staticmethod
     def from_hex(hex: str) -> str:
-        # Accounts
-        if hex == "55":
-            return "OP_DEFI_TX_UTXOS_TO_ACCOUNT"
-        elif hex == "62":
-            return "OP_DEFI_TX_ACCOUNT_TO_UTXOS"
-        elif hex == "42":
-            return "OP_DEFI_TX_ACCOUNT_TO_ACCOUNT"
-        elif hex == "61":
-            return "OP_DEFI_TX_ANY_ACCOUNT_TO_ACCOUNT"
-        elif hex == "51":
-            return "OP_DEFI_TX_FUTURE_SWAP"
-
-        # Pool
-        elif hex == "73":
-            return "OP_DEFI_TX_POOL_SWAP"
-
-
+        dict = DefiTxType.__dict__
+        for key in dict:
+            if key[0:7] == "OP_DEFI":
+                if dict[key] == hex:
+                    return key
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/mainnet/CUSTOM_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9367088607594937%*

 * *Differences: {'insert': "[(74, OrderedDict([('id', '221'), ('symbol', 'BTC'), ('name', 'Its'), ('isDAT', "*

 * *           "False), ('isLPS', False), ('isLoanToken', False)])), (75, OrderedDict([('id', '222'), "*

 * *           "('symbol', 'ETH'), ('name', 'even'), ('isDAT', False), ('isLPS', False), "*

 * *           "('isLoanToken', False)])), (76, OrderedDict([('id', '223'), ('symbol', 'USDT'), "*

 * *           "('name', 'funnier'), ('isDAT', False), ('isLPS', False), ('isLoanToken', False)])), "*

 * *           "(77, OrderedDict([('id', '2 […]*

```diff
@@ -586,9 +586,49 @@
     {
         "id": "201",
         "isDAT": false,
         "isLPS": false,
         "isLoanToken": false,
         "name": "Decentralized USD",
         "symbol": "DUSD"
+    },
+    {
+        "id": "221",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "Its",
+        "symbol": "BTC"
+    },
+    {
+        "id": "222",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "even",
+        "symbol": "ETH"
+    },
+    {
+        "id": "223",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "funnier",
+        "symbol": "USDT"
+    },
+    {
+        "id": "224",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "the second",
+        "symbol": "USDC"
+    },
+    {
+        "id": "225",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "time",
+        "symbol": "EUROC"
     }
 ]
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96%*

 * *Differences: {'insert': "[(72, OrderedDict([('id', '217'), ('symbol', 'EUROC-DFI'), ('name', 'Euro Coin-Default "*

 * *           "Defi token'), ('isDAT', True), ('isLPS', True), ('isLoanToken', False)])), (73, "*

 * *           "OrderedDict([('id', '218'), ('symbol', 'EUROC-DUSD'), ('name', 'Euro "*

 * *           "Coin-Decentralized USD'), ('isDAT', True), ('isLPS', True), ('isLoanToken', False)])), "*

 * *           "(74, OrderedDict([('id', '220'), ('symbol', 'BURN2-DUSD'), ('name', 'Burner for "*

 * *           "Buy-Burn Bot-Decentralized  […]*

```diff
@@ -570,9 +570,33 @@
     {
         "id": "215",
         "isDAT": true,
         "isLPS": true,
         "isLoanToken": false,
         "name": "dBITI-Decentralized USD",
         "symbol": "BITI-DUSD"
+    },
+    {
+        "id": "217",
+        "isDAT": true,
+        "isLPS": true,
+        "isLoanToken": false,
+        "name": "Euro Coin-Default Defi token",
+        "symbol": "EUROC-DFI"
+    },
+    {
+        "id": "218",
+        "isDAT": true,
+        "isLPS": true,
+        "isLoanToken": false,
+        "name": "Euro Coin-Decentralized USD",
+        "symbol": "EUROC-DUSD"
+    },
+    {
+        "id": "220",
+        "isDAT": true,
+        "isLPS": true,
+        "isLoanToken": false,
+        "name": "Burner for Buy-Burn Bot-Decentralized USD",
+        "symbol": "BURN2-DUSD"
     }
 ]
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/mainnet/LOAN_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/mainnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/mainnet/STANDARD_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {'insert': "[(70, OrderedDict([('id', '216'), ('symbol', 'EUROC'), ('name', 'Euro Coin'), "*

 * *           "('isDAT', True), ('isLPS', False), ('isLoanToken', False)])), (71, OrderedDict([('id', "*

 * *           "'219'), ('symbol', 'BURN2'), ('name', 'Burner for Buy-Burn Bot'), ('isDAT', True), "*

 * *           "('isLPS', False), ('isLoanToken', False)]))]"}*

```diff
@@ -554,9 +554,25 @@
     {
         "id": "211",
         "isDAT": true,
         "isLPS": false,
         "isLoanToken": true,
         "name": "dSHEL",
         "symbol": "SHEL"
+    },
+    {
+        "id": "216",
+        "isDAT": true,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "Euro Coin",
+        "symbol": "EUROC"
+    },
+    {
+        "id": "219",
+        "isDAT": true,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "Burner for Buy-Burn Bot",
+        "symbol": "BURN2"
     }
 ]
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/opcodes.py` & `defichain-3.0.0b1/defichain/transactions/constants/opcodes.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/testnet/CUSTOM_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9823529411764705%*

 * *Differences: {'delete': '[138, 137, 136]'}*

```diff
@@ -1084,38 +1084,14 @@
         "isDAT": false,
         "isLPS": false,
         "isLoanToken": false,
         "name": "AdultBabyToken",
         "symbol": "ABT"
     },
     {
-        "id": "163",
-        "isDAT": false,
-        "isLPS": false,
-        "isLoanToken": false,
-        "name": "STP123",
-        "symbol": "STP123"
-    },
-    {
-        "id": "164",
-        "isDAT": false,
-        "isLPS": false,
-        "isLoanToken": false,
-        "name": "STP",
-        "symbol": "STP"
-    },
-    {
-        "id": "165",
-        "isDAT": false,
-        "isLPS": false,
-        "isLoanToken": false,
-        "name": "JJBTC",
-        "symbol": "JJTOK"
-    },
-    {
         "id": "166",
         "isDAT": false,
         "isLPS": false,
         "isLoanToken": false,
         "name": "",
         "symbol": "MyToken1"
     },
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'insert': "[(12, OrderedDict([('id', '26'), ('symbol', 'EUROC-DFI'), ('name', 'Euro Coin-Default "*

 * *           "Defi token'), ('isDAT', True), ('isLPS', True), ('isLoanToken', False)])), (13, "*

 * *           "OrderedDict([('id', '27'), ('symbol', 'EUROC-DUSD'), ('name', 'Euro Coin-DUSD'), "*

 * *           "('isDAT', True), ('isLPS', True), ('isLoanToken', False)]))]"}*

```diff
@@ -90,9 +90,25 @@
     {
         "id": "24",
         "isDAT": true,
         "isLPS": true,
         "isLoanToken": false,
         "name": "DUSD-USD Coin",
         "symbol": "DUSD-USDC"
+    },
+    {
+        "id": "26",
+        "isDAT": true,
+        "isLPS": true,
+        "isLoanToken": false,
+        "name": "Euro Coin-Default Defi token",
+        "symbol": "EUROC-DFI"
+    },
+    {
+        "id": "27",
+        "isDAT": true,
+        "isLPS": true,
+        "isLoanToken": false,
+        "name": "Euro Coin-DUSD",
+        "symbol": "EUROC-DUSD"
     }
 ]
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/testnet/LOAN_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/testnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/testnet/STANDARD_tokens.json` & `defichain-3.0.0b1/defichain/transactions/constants/testnet/STANDARD_tokens.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {'insert': "[(13, OrderedDict([('id', '25'), ('symbol', 'EUROC'), ('name', 'Euro Coin'), ('isDAT', "*

 * *           "True), ('isLPS', False), ('isLoanToken', False)]))]"}*

```diff
@@ -100,14 +100,22 @@
         "isDAT": true,
         "isLPS": false,
         "isLoanToken": false,
         "name": "USD Coin",
         "symbol": "USDC"
     },
     {
+        "id": "25",
+        "isDAT": true,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "Euro Coin",
+        "symbol": "EUROC"
+    },
+    {
         "id": "158",
         "isDAT": true,
         "isLPS": false,
         "isLoanToken": false,
         "name": "",
         "symbol": "AhmedTok"
     },
```

### Comparing `defichain-3.0.0b0/defichain/transactions/constants/tokens.py` & `defichain-3.0.0b1/defichain/transactions/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/builddefitx.py` & `defichain-3.0.0b1/defichain/transactions/defitx/builddefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/defitx.py` & `defichain-3.0.0b1/defichain/transactions/defitx/defitx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Any
 
 from defichain.exceptions.transactions import NotYetSupportedError
 from defichain.transactions.constants import DefiTx_SIGNATURE
 from .modules.accounts import *
+from .modules.loans import *
+from .modules.masternode import *
 from .modules.pool import *
 
+from .modules.vault import *
+
 
 class DefiTx:
 
     @staticmethod
     def deserialize(network: Any, hex: str) -> "BaseDefiTx":
         position = 0
 
@@ -32,13 +36,39 @@
 
         # Account
         if DefiTxType.OP_DEFI_TX_UTXOS_TO_ACCOUNT == defiTxType:
             return UtxosToAccount.deserialize(network, hex[position:])
         elif DefiTxType.OP_DEFI_TX_ACCOUNT_TO_ACCOUNT == defiTxType:
             return AccountToAccount.deserialize(network, hex[position:])
 
+        # Loans
+        elif DefiTxType.OP_DEFI_TX_TAKE_LOAN == defiTxType:
+            return TakeLoan.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_PAYBACK_LOAN == defiTxType:
+            return PaybackLoan.deserialize(network, hex[position:])
+
+        # Masternode
+        elif DefiTxType.OP_DEFI_TX_CREATE_MASTER_NODE == defiTxType:
+            return CreateMasternode.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_RESIGN_MASTER_NODE == defiTxType:
+            return ResignMasternode.deserialize(network, hex[position:])
+
         # Pool
         elif DefiTxType.OP_DEFI_TX_POOL_SWAP == defiTxType:
-            return Poolswap.deserialize(network, hex[position:])
+            return PoolSwap.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_COMPOSITE_SWAP == defiTxType:
+            return CompositeSwap.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_POOL_ADD_LIQUIDITY == defiTxType:
+            return AddPoolLiquidity.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_POOL_REMOVE_LIQUIDITY == defiTxType:
+            return RemovePoolLiquidity.deserialize(network, hex[position:])
+
+        # Vault
+        elif DefiTxType.OP_DEFI_TX_CREATE_VAULT == defiTxType:
+            return CreateVault.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_DEPOSIT_TO_VAULT == defiTxType:
+            return DepositToVault.deserialize(network, hex[position:])
+        elif DefiTxType.OP_DEFI_TX_WITHDRAW_FROM_VAULT == defiTxType:
+            return WithdrawFromVault.deserialize(network, hex[position:])
 
         raise NotYetSupportedError()
```

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/modules/accounts.py` & `defichain-3.0.0b1/defichain/transactions/defitx/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/modules/basedefitx.py` & `defichain-3.0.0b1/defichain/transactions/defitx/modules/basedefitx.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/modules/baseinput.py` & `defichain-3.0.0b1/defichain/transactions/defitx/modules/baseinput.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
 from defichain.exceptions.transactions import AddressError
 from defichain.transactions.utils import Token, Verify, BuildAddressAmounts
 from defichain.transactions.address import Address
-from defichain.transactions.utils import Converter
+from defichain.transactions.utils import Converter, Calculate
 
 
 class BaseInput(ABC):
 
     @staticmethod
     @abstractmethod
     def deserialize(network: Any, hex: str) -> "BaseInput":
@@ -64,15 +64,38 @@
         return Converter.int_to_bytes(self.get_tokenId(), 4)
 
     def get_bytes_amount(self) -> bytes:
         return Converter.int_to_bytes(self.get_amount(), 8)
 
 
 class TokenBalanceVarInt(BaseInput):
-    pass
+    @staticmethod
+    def deserialize(network: Any, hex: str) -> "TokenBalanceVarInt":
+        tokenId = Calculate.read_varInt(hex[0: Calculate.length_varInt(hex) * 2])
+        amount = Converter.hex_to_int(hex[Calculate.length_varInt(hex) * 2: Calculate.length_varInt(hex) * 2 + 16])
+        return TokenBalanceVarInt(tokenId, amount)
+
+    def __init__(self, tokenId: int, amount: int):
+        self._token = tokenId
+        self._amount = amount
+
+    def __bytes__(self) -> bytes:
+        return self.get_bytes_tokenId() + self.get_bytes_amount()
+
+    def get_tokenId(self) -> int:
+        return self._token
+
+    def get_amount(self) -> int:
+        return self._amount
+
+    def get_bytes_tokenId(self) -> bytes:
+        return Converter.hex_to_bytes(Calculate.write_varInt(self.get_tokenId()))
+
+    def get_bytes_amount(self) -> bytes:
+        return Converter.int_to_bytes(self.get_amount(), 8)
 
 
 class ScriptBalances(BaseInput):
     @staticmethod
     def from_json(addressAmount: {}) -> ["ScriptBalances"]:
         network = None
         scriptBalances = []
@@ -187,10 +210,7 @@
 
     def get_script(self) -> str:
         return Address.from_address(self._address).get_scriptPublicKey()
 
     def get_bytes_script(self) -> bytes:
         return Converter.hex_to_bytes(self.get_script())
 
-
-if __name__ == "__main__":
-    pass
```

### Comparing `defichain-3.0.0b0/defichain/transactions/defitx/modules/pool.py` & `defichain-3.0.0b1/defichain/transactions/defitx/modules/vault.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,258 +1,284 @@
 from typing import Any
 
 from defichain.exceptions.transactions import AddressError
 from defichain.transactions.constants import DefiTxType
 from defichain.transactions.address import Address
-from defichain.transactions.utils import Converter, Token, Verify
-from .basedefitx import BaseDefiTx
+from defichain.transactions.utils import Converter, Token, Calculate
 from ..builddefitx import BuildDefiTx
+from .baseinput import TokenBalanceVarInt
+from .basedefitx import BaseDefiTx
 
 
-class Poolswap(BaseDefiTx):
+class CreateVault(BaseDefiTx):
     """
-    Builds the defi transaction for a poolswap
+    Builds the defi transaction: Create Vault
 
-    :param addressFrom: (required) the address where the tokens are located
-    :param tokenFrom: (required) the token that should be exchanged
-    :param amountFrom: (required) the amount that should be exchanged
-    :param addressTo: (required) the address where the exchanged tokens are sent to
-    :param tokenTo: (required) the token to change into
-    :param maxPrice: (required) maximum acceptable price
-    :return: "hex" (string) -- returns the finished defi transaction
+    :param ownerAddress: (required) the address where vault will be created
+    :type ownerAddress: str
+    :param schemeId: (required) the scheme id for the vault
+    :type schemeId: str
     """
 
     @staticmethod
-    def deserialize(network: Any, hex: str) -> "Poolswap":
+    def deserialize(network: Any, hex: str) -> "BaseDefiTx":
         position = 0
 
-        lengthAddressFrom = Converter.hex_to_int(hex[position: position + 2]) * 2
+        lengthOwnerAddress = Converter.hex_to_int(hex[position: position + 2]) * 2
         position += 2
 
-        addressFrom = Address.from_scriptPublicKey(network, hex[position: position + lengthAddressFrom])
-        position += lengthAddressFrom
+        ownerAddress = Address.from_scriptPublicKey(network, hex[position: position + lengthOwnerAddress])
+        position += lengthOwnerAddress
 
-        tokenFrom = Converter.hex_to_int(hex[position: position + 2])
+        lengthSchemeId = Converter.hex_to_int(hex[position: position + 2]) * 2
         position += 2
 
-        amountFrom = Converter.hex_to_int(hex[position: position + 16])
-        position += 16
+        schemeId = Converter.hex_to_str(hex[position: position + lengthSchemeId])
+        position += lengthSchemeId
 
-        lengthAddressTo = Converter.hex_to_int(hex[position: position + 2]) * 2
-        position += 2
+        return CreateVault(ownerAddress.get_address(), schemeId)
 
-        addressTo = Address.from_scriptPublicKey(network, hex[position: position + lengthAddressTo])
-        position += lengthAddressTo
+    def __init__(self, ownerAddress: str, schemeId: str):
+        self._ownerAddress, self._schemeId = None, None
+        self.set_ownerAddress(ownerAddress)
+        self.set_schemeId(schemeId)
 
-        tokenTo = Converter.hex_to_int(hex[position: position + 2])
-        position += 2
+    def __bytes__(self) -> bytes:
+        # Convert to Bytes
+        defiTxType = Converter.hex_to_bytes(self.get_defiTxType())
+        ownerAddress = Converter.hex_to_bytes(Address.from_address(self.get_ownerAddress()).get_scriptPublicKey())
+        schemeId = Converter.hex_to_bytes(Converter.str_to_hex(self.get_schemeId()))
 
-        maxPriceInteger = Converter.hex_to_int(hex[position: position + 16])
-        position += 16
+        lengthOwnerAddress = Converter.int_to_bytes(len(ownerAddress), 1)
+        lengthSchemeId = Converter.int_to_bytes(len(schemeId), 1)
 
-        maxPriceFraction = str(Converter.hex_to_int(hex[position: position + 16]))
-        position += 16
+        # Build PoolSwapDefiTx
+        result = defiTxType
+        result += lengthOwnerAddress
+        result += ownerAddress
+        result += lengthSchemeId
+        result += schemeId
 
-        while len(maxPriceFraction) < 8:
-            maxPriceFraction += "0"
+        return BuildDefiTx.build_defiTx(result)
 
-        maxPrice = int(str(maxPriceInteger) + maxPriceFraction)
+    def to_json(self) -> {}:
+        json = {}
+        json.update({"defiTxType": {"typeName": DefiTxType.from_hex(self.get_defiTxType()),
+                                    "typeHex": self.get_defiTxType()}})
+        json.update({"ownerAddress": self.get_ownerAddress()})
+        json.update({"schemeId": self.get_schemeId()})
+        return json
+
+    # Get Information
+    def get_defiTxType(self) -> str:
+        return DefiTxType.OP_DEFI_TX_CREATE_VAULT
+
+    def get_ownerAddress(self):
+        return self._ownerAddress
 
-        return Poolswap(addressFrom.get_address(), tokenFrom, amountFrom, addressTo.get_address(), tokenTo, maxPrice)
+    def get_schemeId(self):
+        return self._schemeId
+
+    # Set Information
+    def set_ownerAddress(self, ownerAddress: str):
+        self._ownerAddress = ownerAddress
+
+    def set_schemeId(self, schemeId: str):
+        self._schemeId = schemeId
+
+
+class UpdateVault(BaseDefiTx):
+    pass
 
-    def __init__(self, addressFrom: str, tokenFrom: int, amountFrom: int, addressTo: str, tokenTo: int,
-                 maxPrice: int):
 
-        self._addressFrom, self._tokenFrom, self._amountFrom, self._addressTo, self._tokenTo, self._maxPrice = None, \
-            None, None, None, None, None
+class DepositToVault(BaseDefiTx):
+    """
+    Builds the defi transaction: Deposit To Vault
+
+    :param vaultId: (required) vault id
+    :type vaultId: str
+    :param addressFrom: (required) address containing collateral
+    :type addressFrom: str
+    :param amount: (required) Amount of collateral in amount@symbol format
+    :type amount: str
+    """
+
+    @staticmethod
+    def deserialize(network: Any, hex: str) -> "DepositToVault":
+        position = 0
+
+        vaultId = Converter.bytes_to_hex(bytes(reversed(Converter.hex_to_bytes(hex[position: position + 64]))))
+        position += 64
+
+        lenghtAddressFrom = Converter.hex_to_int(hex[position: position + 2]) * 2
+        position += 2
+
+        addressFrom = Address.from_scriptPublicKey(network, hex[position: position + lenghtAddressFrom])
+        position += lenghtAddressFrom
+
+        lengthTokenId = Calculate.length_varInt(hex[position:]) * 2
+        tokenId = Calculate.read_varInt(hex[position: position + lengthTokenId])
+        position += lengthTokenId
+        amount = Converter.hex_to_int(hex[position: position + 16])
+
+        return DepositToVault(vaultId, addressFrom.get_address(), f"{amount}@{tokenId}")
+
+    def __init__(self, vaultId: str, addressFrom: str, amount: str):
+        self._vaultId, self._addressFrom, self._amount = None, None, None
         self._network = None
+        self.set_vaultId(vaultId)
         self.set_addressFrom(addressFrom)
-        self.set_tokenFrom(tokenFrom)
-        self.set_amountFrom(amountFrom)
-        self.set_addressTo(addressTo)
-        self.set_tokenTo(tokenTo)
-        self.set_maxPrice(maxPrice)
+        self.set_amount(amount)
 
     def __bytes__(self) -> bytes:
         # Convert to Bytes
-        defiTxType = Converter.hex_to_bytes(DefiTxType.OP_DEFI_TX_POOL_SWAP)
+        defiTxType = Converter.hex_to_bytes(self.get_defiTxType())
+        vaultId = bytes(reversed(Converter.hex_to_bytes(self.get_vaultId())))
         addressFrom = Converter.hex_to_bytes(Address.from_address(self.get_addressFrom()).get_scriptPublicKey())
-        tokenFrom = Converter.int_to_bytes(self.get_tokenFrom(), 1)
-        amountFrom = Converter.int_to_bytes(self.get_amountFrom(), 8)
-        addressTo = Converter.hex_to_bytes(Address.from_address(self.get_addressTo()).get_scriptPublicKey())
-        tokenTo = Converter.int_to_bytes(self.get_tokenTo(), 1)
-
-        maxPriceInteger = int(str(self.get_maxPrice())[:-8]) if str(self.get_maxPrice())[:-8] != "" else 0
-        maxPriceFraction = int(str(self.get_maxPrice())[-8:])
-        maxPriceInteger = Converter.int_to_bytes(maxPriceInteger, 8)
-        maxPriceFraction = Converter.int_to_bytes(maxPriceFraction, 8)
+        amountSplit = self.get_amount().split("@")
+        tokenAmount = TokenBalanceVarInt(int(amountSplit[1]), int(amountSplit[0])).bytes()
 
         length_addressFrom = Converter.int_to_bytes(len(addressFrom), 1)
-        length_addressTo = Converter.int_to_bytes(len(addressTo), 1)
 
-        # Build PoolSwapDefiTx
+        # Build DepositToVaultDefiTx
         result = defiTxType
+        result += vaultId
         result += length_addressFrom
         result += addressFrom
-        result += tokenFrom
-        result += amountFrom
-        result += length_addressTo
-        result += addressTo
-        result += tokenTo
-        result += maxPriceInteger
-        result += maxPriceFraction
+        result += tokenAmount
 
         return BuildDefiTx.build_defiTx(result)
 
     def to_json(self) -> {}:
         json = {}
         json.update({"defiTxType": {"typeName": DefiTxType.from_hex(self.get_defiTxType()),
                                     "typeHex": self.get_defiTxType()}})
+        json.update({"vaultId": self.get_vaultId()})
         json.update({"addressFrom": self.get_addressFrom()})
-        json.update({"tokenFrom": self.get_tokenFrom()})
-        json.update({"amountFrom": self.get_amountFrom()})
-        json.update({"addressTo": self.get_addressTo()})
-        json.update({"tokenTo": self.get_tokenTo()})
-        json.update({"maxPrice": self.get_maxPrice()})
+        json.update({"amount": self.get_amount()})
         return json
 
-    # Get information
+    # Get Information
     def get_defiTxType(self) -> str:
-        return DefiTxType.OP_DEFI_TX_POOL_SWAP
+        return DefiTxType.OP_DEFI_TX_DEPOSIT_TO_VAULT
+
+    def get_vaultId(self) -> str:
+        return self._vaultId
 
     def get_addressFrom(self) -> str:
         return self._addressFrom
 
-    def get_tokenFrom(self) -> int:
-        return self._tokenFrom
-
-    def get_amountFrom(self) -> int:
-        return self._amountFrom
-
-    def get_addressTo(self) -> str:
-        return self._addressTo
-
-    def get_tokenTo(self) -> int:
-        return self._tokenTo
-
-    def get_maxPrice(self) -> int:
-        return self._maxPrice
+    def get_amount(self) -> str:
+        return self._amount
 
     # Set Information
+    def set_vaultId(self, vaultId: str) -> None:
+        self._vaultId = vaultId
+
     def set_addressFrom(self, addressFrom: str) -> None:
         address = Address.from_address(addressFrom)
         self._network = address.get_network()
-        self._addressFrom = address.get_address()
-
-    def set_tokenFrom(self, tokenFrom: "int | str") -> None:
-        self._tokenFrom = Token.checkAndConvert(self._network, tokenFrom)
-
-    def set_amountFrom(self, amountFrom: int) -> None:
-        Verify.is_int(amountFrom)
-        self._amountFrom = amountFrom
-
-    def set_addressTo(self, addressTo: str) -> None:
-        address = Address.from_address(addressTo)
-        if address.get_network() != self._network:
-            raise AddressError("The given addresses in the poolswap are not from the same network")
-        self._addressTo = address.get_address()
-
-    def set_tokenTo(self, tokenTo: "int | str") -> None:
-        self._tokenTo = Token.checkAndConvert(self._network, tokenTo)
+        self._addressFrom = addressFrom
 
-    def set_maxPrice(self, maxPrice: int) -> None:
-        Verify.is_int(maxPrice)
-        self._maxPrice = maxPrice
+    def set_amount(self, amount: str) -> None:
+        self._amount = f'{amount.split("@")[0]}@{Token.checkAndConvert(self._network, amount.split("@")[1])}'
 
 
-class CompositeSwap(BaseDefiTx):
-    """TODO: MVP"""
-    pass
-
-
-class PoolAddLiquidity(BaseDefiTx):
+class WithdrawFromVault(BaseDefiTx):
     """
-    TODO: MVP
-
-        Builds the defi transaction for addpoolliquidity
-
-        :param addressAmount: (required) :ref:`Node Address Amount`
-        :param shareAddress: (required) the address where the pool shares are placed
-        :return: "hex" (string) -- returns the finished defi transaction
-
+    Builds the defi transaction: Withdraw From Vault
 
-        number_of_entries = Converter.int_to_bytes(len(addressAmount), 1)
+    :param vaultId: (required) vault id
+    :type vaultId: str
+    :param addressTo: (required) destination address for withdraw of collateral
+    :type addressTo: str
+    :param amount: (required) Amount of collateral in amount@symbol format
+    :type amount: str
+    """
 
-        result = Converter.hex_to_bytes(DefiTxType.OP_DEFI_TX_POOL_ADD_LIQUIDITY)
-        result += number_of_entries
+    @staticmethod
+    def deserialize(network: Any, hex: str) -> "WithdrawFromVault":
+        position = 0
 
-        for address in addressAmount:
-            address_script = Converter.hex_to_bytes(Address.from_address(address).get_scriptPublicKey())
-            length_of_script = Converter.int_to_bytes(len(address_script), 1)
-            result += length_of_script + address_script
+        vaultId = Converter.bytes_to_hex(bytes(reversed(Converter.hex_to_bytes(hex[position: position + 64]))))
+        position += 64
 
-            number_of_tokens = Converter.int_to_bytes(len(addressAmount[address]), 1)
-            result += number_of_tokens
-            for amount in addressAmount[address]:
-                split = amount.split('@')
-                value = Converter.int_to_bytes(int(split[0]), 8)
-                token = Converter.int_to_bytes(int(split[1]), 4)
-                result += token + value
+        lenghtAddressTo = Converter.hex_to_int(hex[position: position + 2]) * 2
+        position += 2
 
-        share_address_script = Converter.hex_to_bytes(Address.from_address(shareAddress).get_scriptPublicKey())
-        length_of_share_script = Converter.int_to_bytes(len(share_address_script), 1)
-        result += length_of_share_script + share_address_script
+        addressTo = Address.from_scriptPublicKey(network, hex[position: position + lenghtAddressTo])
+        position += lenghtAddressTo
 
-        return self._defitx.package_defiTx(result)
-    """
+        lengthTokenId = Calculate.length_varInt(hex[position:]) * 2
+        tokenId = Calculate.read_varInt(hex[position: position + lengthTokenId])
+        position += lengthTokenId
+        amount = Converter.hex_to_int(hex[position: position + 16])
 
-    @staticmethod
-    def deserialize(network: Any, hex: str) -> "BaseDefiTx":
-        pass
+        return WithdrawFromVault(vaultId, addressTo.get_address(), f"{amount}@{tokenId}")
 
-    def __init__(self, addressAmount: {}, shareAddress: str):
-        self._addressAmount, self._shareAddress = None, None
-        self.set_addressAmount(addressAmount)
-        self.set_shareAddress(shareAddress)
+    def __init__(self, vaultId: str, addressTo: str, amount: str):
+        self._vaultId, self._addressTo, self._amount = None, None, None
+        self._network = None
+        self.set_vaultId(vaultId)
+        self.set_addressTo(addressTo)
+        self.set_amount(amount)
 
     def __bytes__(self) -> bytes:
         # Convert to Bytes
-        defiTxType = Converter.hex_to_bytes(DefiTxType.OP_DEFI_TX_POOL_ADD_LIQUIDITY)
-        numberOfEntries = Converter.int_to_bytes(len(self.get_addressAmount()), 1)
+        defiTxType = Converter.hex_to_bytes(self.get_defiTxType())
+        vaultId = bytes(reversed(Converter.hex_to_bytes(self.get_vaultId())))
+        addressTo = Converter.hex_to_bytes(Address.from_address(self.get_addressTo()).get_scriptPublicKey())
+        amountSplit = self.get_amount().split("@")
+        tokenAmount = TokenBalanceVarInt(int(amountSplit[1]), int(amountSplit[0])).bytes()
 
-        # Build PoolSwapDefiTx
+        length_addressTo = Converter.int_to_bytes(len(addressTo), 1)
+
+        # Build DepositToVaultDefiTx
         result = defiTxType
+        result += vaultId
+        result += length_addressTo
+        result += addressTo
+        result += tokenAmount
 
         return BuildDefiTx.build_defiTx(result)
 
+    def to_json(self) -> {}:
+        json = {}
+        json.update({"defiTxType": {"typeName": DefiTxType.from_hex(self.get_defiTxType()),
+                                    "typeHex": self.get_defiTxType()}})
+        json.update({"vaultId": self.get_vaultId()})
+        json.update({"addressTo": self.get_addressTo()})
+        json.update({"amount": self.get_amount()})
+        return json
+
     # Get Information
     def get_defiTxType(self) -> str:
-        pass
+        return DefiTxType.OP_DEFI_TX_WITHDRAW_FROM_VAULT
 
-    def get_addressAmount(self):
-        return self._addressAmount
+    def get_vaultId(self) -> str:
+        return self._vaultId
 
-    def get_shareAddress(self):
-        return self._shareAddress
+    def get_addressTo(self) -> str:
+        return self._addressTo
 
-    def to_json(self) -> {}:
-        pass
+    def get_amount(self) -> str:
+        return self._amount
 
     # Set Information
-    def set_addressAmount(self, addressAmount: {}):
-        self._addressAmount = addressAmount
-
-    def set_shareAddress(self, shareAddress: str):
-        self._shareAddress = shareAddress
+    def set_vaultId(self, vaultId: str) -> None:
+        self._vaultId = vaultId
 
+    def set_addressTo(self, addressTo: str) -> None:
+        address = Address.from_address(addressTo)
+        self._network = address.get_network()
+        self._addressTo = addressTo
 
-class PoolRemoveLiquidity(BaseDefiTx):
-    """TODO: MVP"""
-    pass
+    def set_amount(self, amount: str) -> None:
+        self._amount = f'{amount.split("@")[0]}@{Token.checkAndConvert(self._network, amount.split("@")[1])}'
 
 
-class PoolCreatePair(BaseDefiTx):
+class CloseVault(BaseDefiTx):
     pass
 
 
-class PoolUpdatePair(BaseDefiTx):
+class PlaceAuctionBid(BaseDefiTx):
     pass
```

### Comparing `defichain-3.0.0b0/defichain/transactions/keys.py` & `defichain-3.0.0b1/defichain/transactions/keys.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/fee.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/fee.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/sign.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/sign.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/tx.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,35 +250,35 @@
                 position += 2
                 flag = Converter.hex_to_int(hex[position: position + 2])
                 tx.set_flag(flag)
                 position += 2
                 tx._segwit = True
 
             # Find number of inputs
-            length_numberOfInputs = Calculate.get_lengthCompactSize(hex[position: position + 2])
+            length_numberOfInputs = Calculate.length_compactSize(hex[position: position + 2])
             numberOfInputs = Calculate.read_compactSize(hex[position: position + length_numberOfInputs * 2])
             position += length_numberOfInputs * 2
 
             # Iterate through all inputs
             inputs = []
             for _ in range(numberOfInputs):
                 length_scriptSig = Converter.hex_to_int(hex[position + 72: position + 72 + 2]) * 2
                 input = TxInput.deserialize(network, hex[position: position + 82 + length_scriptSig])
                 inputs.append(input)
                 position += 82 + length_scriptSig
 
             # Find number of outputs
-            length_numberOfOutputs = Calculate.get_lengthCompactSize(hex[position: position + 2])
+            length_numberOfOutputs = Calculate.length_compactSize(hex[position: position + 2])
             numberOfOutputs = Calculate.read_compactSize(hex[position: position + length_numberOfOutputs * 2])
             position += length_numberOfOutputs * 2
 
             # Iterate through all outputs
             outputs = []
             for _ in range(numberOfOutputs):
-                scriptLengthSize = Calculate.get_lengthCompactSize(hex[position + 16: position + 18])
+                scriptLengthSize = Calculate.length_compactSize(hex[position + 16: position + 18])
                 length_script = Calculate.read_compactSize(hex[position + 16: position + 16 + scriptLengthSize * 2]) * 2
 
                 # If transaction version is 1 or 2 there is no token id at the back of an output
                 if tx.get_version() == 1 or tx.get_version() == 2:
                     length_script -= 2
 
                 output = TxOutput.deserialize(network, hex[position: position + 20 + length_script])
```

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/txbase.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/txbase.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/txinput.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/txinput.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/txoutput.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/txoutput.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @staticmethod
     def deserialize(network: Any, hex: str) -> "TxOutput":
         position = 0
 
         value = Converter.hex_to_int(hex[position: position + 16])
         position += 16
 
-        scriptSize = Calculate.get_lengthCompactSize(hex[position: position + 2])
+        scriptSize = Calculate.length_compactSize(hex[position: position + 2])
         length_script = Calculate.read_compactSize(hex[position: position + scriptSize * 2]) * 2
         position += scriptSize * 2
 
         script = hex[position: position + length_script]
         position += length_script
 
         tokenId = Converter.hex_to_int(hex[position: position + 2]) if hex[position: position + 2] != "" else None
```

### Comparing `defichain-3.0.0b0/defichain/transactions/rawtransactions/witness.py` & `defichain-3.0.0b1/defichain/transactions/rawtransactions/witness.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain/transactions/remotedata/node.py` & `defichain-3.0.0b1/defichain/transactions/remotedata/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from defichain.exceptions.transactions import TxBuilderError
 from .remotedata import RemoteData
 from defichain import Node
 
 
 class RemoteDataNode(RemoteData):
+
     def __init__(self, source: Node):
         self.node = source
 
     def get_unspent(self, address: str) -> [{}]:
         # Check if address is indexed by node / wallet
         if not self.node.wallet.getaddressinfo(address)["labels"]:
             error_string = f"To build a raw transaction from the given address: {address} the node needs to index " \
@@ -20,14 +21,23 @@
             txid = u["txid"]
             index = u["vout"]
             value = int(round(float(u["amount"]) * 100000000))
             script = u["scriptPubKey"]
             unspent.append({"txid": txid, "vout": index, "value": value, "scriptPubKey": script})
         return unspent
 
+    def check_masternode(self, masternodeId: str) -> bool:
+        try:
+            data = self.node.masternodes.getmasternode(masternodeId)[masternodeId]
+            if data["state"] in ('PRE_ENABLED', 'ENABLED', 'PRE_RESIGNED'):
+                return True
+        except:
+            pass
+        return False
+
     def test_tx(self, hex: str, maxFeeRate: float = None) -> bool:
         try:
             self.node.rawtransactions.testmempoolaccept([hex], maxFeeRate)
             return True
         except:
             return False
```

### Comparing `defichain-3.0.0b0/defichain/transactions/remotedata/ocean.py` & `defichain-3.0.0b1/defichain/transactions/remotedata/ocean.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,20 @@
             txid = u["vout"]["txid"]
             index = u["vout"]["n"]
             value = int(round(float(u["vout"]["value"]) * 100000000))
             script = u["script"]["hex"]
             unspent.append({"txid": txid, "vout": index, "value": value, "scriptPubKey": script})
         return unspent
 
+    def check_masternode(self, masternodeId: str) -> bool:
+        data = self.ocean.masternodes.get(masternodeId)["data"]
+        if "error" in data or data["state"] not in ('PRE_ENABLED', 'ENABLED', 'PRE_RESIGNED'):
+            return False
+        return True
+
     def test_tx(self, hex: str, maxFeeRate: float = None) -> bool:
         try:
             self.ocean.rawTx.test(hex, maxFeeRate)
             return True
         except:
             return False
```

### Comparing `defichain-3.0.0b0/defichain/transactions/utils/calculate.py` & `defichain-3.0.0b1/defichain/transactions/utils/calculate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 import hashlib
+import io
 
 
 class Calculate:
 
     @staticmethod
     def dHash256(h: hex) -> bytes:
         return hashlib.sha256(hashlib.sha256(h).digest()).digest()
 
     @staticmethod
-    def write_varint(n: int) -> str:
+    def length_varInt(hex: str) -> int:
+        size = 0
+        split = [hex[i:i + 2] for i in range(0, len(hex), 2)]
+        for s in split:
+            integer = int.from_bytes(bytes.fromhex(s), byteorder="little")
+            if integer < 0x80:
+                size += 1
+                break
+            else:
+                size += 1
+        return size
+
+    @staticmethod
+    def write_varInt(n: int) -> str:
         # https://github.com/JellyfishSDK/jellyfish/blob/d57b37bb2b10dfb44389c0d1f6a0c6428fa82d7e/packages/jellyfish-buffer/src/VarInt.ts#L21
         # https://github.com/DeFiCh/ain/blob/0edc8e002ddc634dcb80785b9e9e01606fd8e4f7/src/serialize.h#L355
         buffer = [None for _ in range(20)]
         length = 0
 
         while True:
             buffer[length] = (n & 0x7F) | (0x80 if length else 0x00)
@@ -24,19 +38,28 @@
         for b in list(reversed(buffer)):
             result.append(int(b).to_bytes(length=1, byteorder="little").hex()) if b else None
         if not length + 1 == len(result):
             result.append("00")
         return "".join(result)
 
     @staticmethod
-    def read_varint(hex: str) -> int:
-        pass
+    def read_varInt(hex: str) -> int:
+        buffer = io.BytesIO(bytes.fromhex(hex))
+
+        n = 0
+        while True:
+            buff = buffer.read(1)[0]
+            n = (n << 7) | (buff & 0x7f)
+            if (buff & 0x80) != 0:
+                n += 1
+            else:
+                return n
 
     @staticmethod
-    def get_lengthCompactSize(hex: str) -> int:
+    def length_compactSize(hex: str) -> int:
         indicator = hex[0:2]
         if indicator == "fd":
             return 3
         elif indicator == "fe":
             return 5
         elif indicator == "ff":
             return 9
@@ -69,12 +92,11 @@
         elif hex[0:2] == "ff":
             return int.from_bytes(bytes.fromhex(hex[2:18]), byteorder="little")
         else:
             return int.from_bytes(bytes.fromhex(hex), byteorder="little")
 
 
 if __name__ == "__main__":
-    print(Calculate.write_compactSize(299))
-    print(Calculate.read_compactSize("52"))
-
-    from converter import Converter
-    print(Converter.hex_to_int("50"))
+    c = Calculate.write_varInt(2 ** 32)
+    print(c)
+    print(Calculate.read_varInt(c))
+    print(2**32)
```

### Comparing `defichain-3.0.0b0/defichain/transactions/utils/converter.py` & `defichain-3.0.0b1/defichain/transactions/utils/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,16 +62,26 @@
 
         :param f: Float number
         :return: returns the integer number shifted by eight decimal places
         """
         return int(round(f * 100000000))
 
     @staticmethod
+    def amount_float_to_int(amount: str) -> str:
+        return f'{Converter.float_to_int(float(amount.split("@")[0]))}@{amount.split("@")[1]}'
+
+    @staticmethod
     def addressAmount_float_to_int(addressAmount: {}) -> {}:
         from . import BuildAddressAmounts
         newAddressAmount = BuildAddressAmounts()
         for address in addressAmount:
-            value, token = addressAmount[address].split('@')
-            value = Converter.float_to_int(float(value))
-            newAddressAmount.add(address, token, value)
+            if isinstance(addressAmount[address], list):
+                for amount in addressAmount[address]:
+                    value, token = amount.split('@')
+                    value = Converter.float_to_int(float(value))
+                    newAddressAmount.add(address, token, value)
+            else:
+                value, token = addressAmount[address].split('@')
+                value = Converter.float_to_int(float(value))
+                newAddressAmount.add(address, token, value)
         return newAddressAmount.build()
```

### Comparing `defichain-3.0.0b0/defichain/transactions/utils/token.py` & `defichain-3.0.0b1/defichain/transactions/utils/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,19 @@
         raise TokenError(f"The given id: {tokenId} does not exist. Check your token id input.")
 
     @staticmethod
     def get_id_from_symbol(network: Any, symbol: str) -> int:
         for _type in Token.TOKEN_TYPES:
             tokens = Token._get_tokens(network, _type)
             for token in tokens:
+                if _type == TokenTypes.LIQUIDITY:
+                    if token["symbol"] == str(symbol):
+                        return int(token["id"])
+                    elif token["symbol"] == str(f"{symbol.split('-')[1]}-{symbol.split('-')[0]}"):
+                        return int(token["id"])
                 if token["symbol"] == str(symbol):
                     return int(token["id"])
         raise TokenError(f"The given symbol: {symbol} does not exist. Check your input.")
 
     @staticmethod
     def get_name_from_id(network: Any, tokenId: int) -> str:
         for _type in Token.TOKEN_TYPES:
```

### Comparing `defichain-3.0.0b0/defichain/transactions/utils/verify.py` & `defichain-3.0.0b1/defichain/transactions/utils/verify.py`

 * *Files identical despite different names*

### Comparing `defichain-3.0.0b0/defichain.egg-info/PKG-INFO` & `defichain-3.0.0b1/defichain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: defichain
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: Defichain Python Library
 Home-page: https://github.com/eric-volz/DefichainPython
 Author: Intr0c
 Author-email: introc@volz.link
-License: UNKNOWN
 Keywords: python,defichain,node,ocean,mnemonic,wallet,privateKey,transactions,raw transactions,P2PKH,P2SH,P2WPKH,DefiTx,custom transaction
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -61,9 +59,7 @@
 or other ideas open an [issue](https://github.com/eric-volz/DefichainPython/issues), 
 write me on [Twitter](https://twitter.com/Intr0c) or via email (introc@volz.link)!
 
 ## [License & Disclaimer](https://docs.defichain-python.de/build/html/legal/licenseAndDisclaimer.html)
 
 By using (this repo), you (the user) agree to be bound by the 
 [terms of this license](https://github.com/eric-volz/defichainLibrary/blob/main/LICENSE) (MIT License).
-
-
```

### Comparing `defichain-3.0.0b0/defichain.egg-info/SOURCES.txt` & `defichain-3.0.0b1/defichain.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,17 @@
 defichain/node/modules/zmq.py
 defichain/ocean/OceanErrorHandler.py
 defichain/ocean/__init__.py
 defichain/ocean/connection.py
 defichain/ocean/ocean.py
 defichain/ocean/modules/address.py
 defichain/ocean/modules/blocks.py
+defichain/ocean/modules/consortium.py
 defichain/ocean/modules/fee.py
+defichain/ocean/modules/governance.py
 defichain/ocean/modules/loan.py
 defichain/ocean/modules/masternodes.py
 defichain/ocean/modules/oracles.py
 defichain/ocean/modules/poolpairs.py
 defichain/ocean/modules/prices.py
 defichain/ocean/modules/rawTx.py
 defichain/ocean/modules/rpc.py
@@ -113,16 +115,19 @@
 defichain/transactions/address/p2wpkh.py
 defichain/transactions/address/script.py
 defichain/transactions/builder/__init__.py
 defichain/transactions/builder/rawtransactionbuilder.py
 defichain/transactions/builder/txbuilder.py
 defichain/transactions/builder/modules/__init__.py
 defichain/transactions/builder/modules/accounts.py
+defichain/transactions/builder/modules/loans.py
+defichain/transactions/builder/modules/masternode.py
 defichain/transactions/builder/modules/pool.py
 defichain/transactions/builder/modules/utxo.py
+defichain/transactions/builder/modules/vault.py
 defichain/transactions/constants/__init__.py
 defichain/transactions/constants/address.py
 defichain/transactions/constants/defitx.py
 defichain/transactions/constants/fees.py
 defichain/transactions/constants/opcodes.py
 defichain/transactions/constants/rawtransactions.py
 defichain/transactions/constants/tokens.py
```

### Comparing `defichain-3.0.0b0/setup.py` & `defichain-3.0.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from os import path
 
-VERSION = '3.0.0b0'
+VERSION = '3.0.0b1'
 DESCRIPTION = 'Defichain Python Library'
 
 # Project URLs
 project_urls = {
     "Tracker": "https://github.com/eric-volz/DefichainPython",
     "Documentation": "https://docs.defichain-python.de"
 }
```

