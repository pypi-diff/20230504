# Comparing `tmp/cb_exchange_lib-3.0.2.tar.gz` & `tmp/cb-exchange-lib-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cb_exchange_lib-3.0.2.tar", last modified: Tue Mar  7 13:18:04 2023, max compression
+gzip compressed data, was "cb-exchange-lib-3.0.3.tar", last modified: Thu May  4 21:28:47 2023, max compression
```

## Comparing `cb_exchange_lib-3.0.2.tar` & `cb-exchange-lib-3.0.3.tar`

### file list

```diff
@@ -1,27 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 13:18:04.594217 cb_exchange_lib-3.0.2/
--rw-rw-rw-   0        0        0     1090 2023-02-01 08:41:29.000000 cb_exchange_lib-3.0.2/LICENSE
--rw-rw-rw-   0        0        0        0 2022-08-01 15:43:54.000000 cb_exchange_lib-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    19868 2023-03-07 13:18:04.595186 cb_exchange_lib-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    18879 2023-03-07 13:11:57.000000 cb_exchange_lib-3.0.2/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cb_exchange_lib-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1263 2023-03-07 13:18:04.595186 cb_exchange_lib-3.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-07 13:18:04.565266 cb_exchange_lib-3.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-07 13:18:04.586238 cb_exchange_lib-3.0.2/src/cb_exchange_lib/
--rw-rw-rw-   0        0        0      804 2023-01-31 19:53:29.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-01-31 18:34:14.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/authentication.py
--rw-rw-rw-   0        0        0     1427 2023-01-31 20:50:42.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/constants.py
--rw-rw-rw-   0        0        0    58518 2023-02-21 12:25:59.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/endpoints.py
--rw-rw-rw-   0        0        0     5008 2023-02-24 12:34:50.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/sessions.py
--rw-rw-rw-   0        0        0     1499 2023-02-19 13:40:07.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/utils.py
--rw-rw-rw-   0        0        0     5987 2023-02-19 13:40:07.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib/websockets.py
-drwxrwxrwx   0        0        0        0 2023-03-07 13:18:04.590200 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/
--rw-rw-rw-   0        0        0    19868 2023-03-07 13:18:04.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-03-07 13:18:04.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 13:18:04.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 08:54:28.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      106 2023-03-07 13:18:04.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-07 13:18:04.000000 cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-07 13:18:04.594217 cb_exchange_lib-3.0.2/tests/
--rw-rw-rw-   0        0        0     8823 2023-02-19 15:52:40.000000 cb_exchange_lib-3.0.2/tests/tests_endpoints.py
--rw-rw-rw-   0        0        0       25 2023-02-19 13:40:07.000000 cb_exchange_lib-3.0.2/tests/tests_others.py
--rw-rw-rw-   0        0        0     1904 2023-02-19 15:55:04.000000 cb_exchange_lib-3.0.2/tests/tests_websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:28:47.825395 cb-exchange-lib-3.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-02-01 08:41:29.000000 cb-exchange-lib-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-04 20:55:53.000000 cb-exchange-lib-3.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    19714 2023-05-04 21:28:47.825395 cb-exchange-lib-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    18879 2023-03-07 13:11:57.000000 cb-exchange-lib-3.0.3/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cb-exchange-lib-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1139 2023-05-04 21:28:47.825395 cb-exchange-lib-3.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 21:28:47.805198 cb-exchange-lib-3.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 21:28:47.825395 cb-exchange-lib-3.0.3/src/cb_exchange_lib/
+-rw-rw-rw-   0        0        0      804 2023-01-31 19:53:29.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-01-31 18:34:14.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/authentication.py
+-rw-rw-rw-   0        0        0     1427 2023-01-31 20:50:42.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/constants.py
+-rw-rw-rw-   0        0        0    58518 2023-02-21 12:25:59.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/endpoints.py
+-rw-rw-rw-   0        0        0     5008 2023-02-24 12:34:50.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/sessions.py
+-rw-rw-rw-   0        0        0     1499 2023-02-19 13:40:07.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/utils.py
+-rw-rw-rw-   0        0        0     5987 2023-02-19 13:40:07.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib/websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:28:47.825395 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/
+-rw-rw-rw-   0        0        0    19714 2023-05-04 21:28:47.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-05-04 21:28:47.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 21:28:47.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-01 08:54:28.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      103 2023-05-04 21:28:47.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 21:28:47.000000 cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/top_level.txt
```

### Comparing `cb_exchange_lib-3.0.2/LICENSE` & `cb-exchange-lib-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/PKG-INFO` & `cb-exchange-lib-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
-Name: cb_exchange_lib
-Version: 3.0.2
+Name: cb-exchange-lib
+Version: 3.0.3
 Summary: Coinbase Exchange API client library.
 Home-page: https://github.com/ClaudiuDrug/cb-exchange-lib
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cb-exchange-lib/issues
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
```

### Comparing `cb_exchange_lib-3.0.2/README.md` & `cb-exchange-lib-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/setup.cfg` & `cb-exchange-lib-3.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2063 625f 6578 6368 616e 6765 5f6c   = cb_exchange_l
+00000010: 203d 2063 622d 6578 6368 616e 6765 2d6c   = cb-exchange-l
 00000020: 6962 0d0a 7665 7273 696f 6e20 3d20 332e  ib..version = 3.
-00000030: 302e 320d 0a61 7574 686f 7220 3d20 436c  0.2..author = Cl
+00000030: 302e 330d 0a61 7574 686f 7220 3d20 436c  0.3..author = Cl
 00000040: 6175 6469 7520 4452 5547 0d0a 6175 7468  audiu DRUG..auth
 00000050: 6f72 5f65 6d61 696c 203d 2063 6c61 7564  or_email = claud
 00000060: 6975 2e64 7275 6740 6f75 746c 6f6f 6b2e  iu.drug@outlook.
 00000070: 636f 6d0d 0a6c 6963 656e 7365 203d 204d  com..license = M
 00000080: 4954 204c 6963 656e 7365 0d0a 6465 7363  IT License..desc
 00000090: 7269 7074 696f 6e20 3d20 436f 696e 6261  ription = Coinba
 000000a0: 7365 2045 7863 6861 6e67 6520 4150 4920  se Exchange API 
@@ -23,57 +23,50 @@
 00000160: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
 00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6c61  //github.com/Cla
 00000180: 7564 6975 4472 7567 2f63 622d 6578 6368  udiuDrug/cb-exch
 00000190: 616e 6765 2d6c 6962 2f69 7373 7565 730d  ange-lib/issues.
 000001a0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
 000001b0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001d0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000230: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000240: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000250: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000260: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000270: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000280: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000290: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
-000002a0: 646f 7773 203a 3a20 5769 6e64 6f77 7320  dows :: Windows 
-000002b0: 3130 0d0a 094f 7065 7261 7469 6e67 2053  10...Operating S
-000002c0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
-000002d0: 3a20 4c69 6e75 780d 0a09 496e 7465 6e64  : Linux...Intend
-000002e0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-000002f0: 6576 656c 6f70 6572 730d 0a09 4e61 7475  evelopers...Natu
-00000300: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-00000310: 456e 676c 6973 680d 0a09 546f 7069 6320  English...Topic 
-00000320: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000330: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000340: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
-00000350: 6f64 756c 6573 0d0a 0954 6f70 6963 203a  odules...Topic :
-00000360: 3a20 5574 696c 6974 6965 730d 0a0d 0a5b  : Utilities....[
-00000370: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
-00000380: 6665 203d 2046 616c 7365 0d0a 7061 636b  fe = False..pack
-00000390: 6167 6573 203d 2066 696e 645f 6e61 6d65  ages = find_name
-000003a0: 7370 6163 653a 0d0a 7061 636b 6167 655f  space:..package_
-000003b0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
-000003c0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-000003d0: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
-000003e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000003f0: 3d20 332e 370d 0a69 6e73 7461 6c6c 5f72  = 3.7..install_r
-00000400: 6571 7569 7265 7320 3d20 0d0a 0972 6571  equires = ...req
-00000410: 7565 7374 7320 3e3d 2032 2e32 382e 320d  uests >= 2.28.2.
-00000420: 0a09 7265 7175 6573 7473 2d63 6163 6865  ..requests-cache
-00000430: 203e 3d20 312e 302e 300d 0a09 7265 7175   >= 1.0.0...requ
-00000440: 6573 7473 2d74 6f6f 6c62 656c 7420 3e3d  ests-toolbelt >=
-00000450: 2030 2e31 302e 310d 0a09 7572 6c6c 6962   0.10.1...urllib
-00000460: 3320 3e3d 2031 2e32 362e 3134 0d0a 0977  3 >= 1.26.14...w
-00000470: 6562 736f 636b 6574 2d63 6c69 656e 7420  ebsocket-client 
-00000480: 3e3d 2031 2e35 2e31 0d0a 0d0a 5b6f 7074  >= 1.5.1....[opt
-00000490: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000004a0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000004b0: 0d0a 6578 636c 7564 6520 3d20 7465 7374  ..exclude = test
-000004c0: 730d 0a0d 0a5b 6567 675f 696e 666f 5d0d  s....[egg_info].
-000004d0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000004e0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000001d0: 203a 3a20 332e 370d 0a09 4c69 6365 6e73   :: 3.7...Licens
+000001e0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001f0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000200: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000210: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+00000220: 203a 3a20 5769 6e64 6f77 7320 3a3a 2057   :: Windows :: W
+00000230: 696e 646f 7773 2031 300d 0a09 4f70 6572  indows 10...Oper
+00000240: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000250: 504f 5349 5820 3a3a 204c 696e 7578 0d0a  POSIX :: Linux..
+00000260: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000270: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000280: 0d0a 094e 6174 7572 616c 204c 616e 6775  ...Natural Langu
+00000290: 6167 6520 3a3a 2045 6e67 6c69 7368 0d0a  age :: English..
+000002a0: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
+000002b0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+000002c0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+000002d0: 7974 686f 6e20 4d6f 6475 6c65 730d 0a09  ython Modules...
+000002e0: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+000002f0: 6573 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  es....[options].
+00000300: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+00000310: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
+00000320: 6e64 5f6e 616d 6573 7061 6365 3a0d 0a70  nd_namespace:..p
+00000330: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000340: 3d20 7372 630d 0a69 6e63 6c75 6465 5f70  = src..include_p
+00000350: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000360: 7565 0d0a 7079 7468 6f6e 5f72 6571 7569  ue..python_requi
+00000370: 7265 7320 3d20 3e3d 2033 2e37 0d0a 696e  res = >= 3.7..in
+00000380: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000390: 200d 0a09 7265 7175 6573 7473 203e 3d20   ...requests >= 
+000003a0: 322e 3330 2e30 0d0a 0972 6571 7565 7374  2.30.0...request
+000003b0: 732d 6361 6368 6520 3e3d 2031 2e30 2e31  s-cache >= 1.0.1
+000003c0: 0d0a 0972 6571 7565 7374 732d 746f 6f6c  ...requests-tool
+000003d0: 6265 6c74 203e 3d20 312e 302e 300d 0a09  belt >= 1.0.0...
+000003e0: 7572 6c6c 6962 3320 3e3d 2032 2e30 2e32  urllib3 >= 2.0.2
+000003f0: 0d0a 0977 6562 736f 636b 6574 2d63 6c69  ...websocket-cli
+00000400: 656e 7420 3e3d 2031 2e35 2e31 0d0a 0d0a  ent >= 1.5.1....
+00000410: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000420: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000430: 2073 7263 0d0a 6578 636c 7564 6520 3d20   src..exclude = 
+00000440: 7465 7374 730d 0a0d 0a5b 6567 675f 696e  tests....[egg_in
+00000450: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000460: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000470: 0a0d 0a                                  ...
```

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/__init__.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/authentication.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/authentication.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/constants.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/constants.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/endpoints.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/sessions.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/sessions.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/utils.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/utils.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib/websockets.py` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib/websockets.py`

 * *Files identical despite different names*

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/PKG-INFO` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: cb-exchange-lib
-Version: 3.0.2
+Version: 3.0.3
 Summary: Coinbase Exchange API client library.
 Home-page: https://github.com/ClaudiuDrug/cb-exchange-lib
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cb-exchange-lib/issues
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
```

### Comparing `cb_exchange_lib-3.0.2/src/cb_exchange_lib.egg-info/SOURCES.txt` & `cb-exchange-lib-3.0.3/src/cb_exchange_lib.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -11,11 +11,8 @@
 src/cb_exchange_lib/utils.py
 src/cb_exchange_lib/websockets.py
 src/cb_exchange_lib.egg-info/PKG-INFO
 src/cb_exchange_lib.egg-info/SOURCES.txt
 src/cb_exchange_lib.egg-info/dependency_links.txt
 src/cb_exchange_lib.egg-info/not-zip-safe
 src/cb_exchange_lib.egg-info/requires.txt
-src/cb_exchange_lib.egg-info/top_level.txt
-tests/tests_endpoints.py
-tests/tests_others.py
-tests/tests_websockets.py
+src/cb_exchange_lib.egg-info/top_level.txt
```

