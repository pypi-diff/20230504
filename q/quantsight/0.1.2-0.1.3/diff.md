# Comparing `tmp/quantsight-0.1.2.linux-x86_64.tar.gz` & `tmp/quantsight-0.1.3.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantsight-0.1.2.linux-x86_64.tar", last modified: Thu May  4 13:32:40 2023, max compression
+gzip compressed data, was "quantsight-0.1.3.linux-x86_64.tar", last modified: Thu May  4 18:24:35 2023, max compression
```

## Comparing `quantsight-0.1.2.linux-x86_64.tar` & `quantsight-0.1.3.linux-x86_64.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.931388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.939388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 13:32:30.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 13:32:39.935388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/client.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-04 13:32:30.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:32:39.939388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 13:32:39.815388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 13:32:39.795388 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.203635 ./
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.203635 ./opt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.215634 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 18:24:24.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 18:24:24.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.215634 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 18:24:35.095635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/top_level.txt
```

### ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py

```diff
@@ -1 +1 @@
-from client import QuantsightClient as Quantsight
+from .client import QuantsightClient as Quantsight
```

### ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/__init__.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,28 +1,28 @@
 magic:    0xa70d0d0a
-moddate:  0xeeb35364 (Thu May  4 13:32:30 2023 UTC)
-files sz: 50
+moddate:  0x58f85364 (Thu May  4 18:24:24 2023 UTC)
+files sz: 51
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c006d015a02010064025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (0)
+     1           2 LOAD_CONST               0 (1)
                  4 LOAD_CONST               1 (('QuantsightClient',))
                  6 IMPORT_NAME              0 (client)
                  8 IMPORT_FROM              1 (QuantsightClient)
                 10 STORE_NAME               2 (Quantsight)
                 12 POP_TOP
                 14 LOAD_CONST               2 (None)
                 16 RETURN_VALUE
    consts
-      0
+      1
       ('QuantsightClient',)
       None
    names      ('client', 'QuantsightClient', 'Quantsight')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py'
```

### ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/client.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,399 +1,595 @@
 magic:    0xa70d0d0a
-moddate:  0xeeb35364 (Thu May  4 13:32:30 2023 UTC)
-files sz: 2928
+moddate:  0x58f85364 (Thu May  4 18:24:24 2023 UTC)
+files sz: 3682
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a02640064016c035a03640064
-      026c046d055a050100640064036c066d065a060100020047006404840064
-      05a6020000ab0200000000000000005a0764015300
+      0x9700640064016c005a00640064016c015a01640064016c025a03640064
+      016c045a04640064026c056d065a060100640064036c076d075a076d085a
+      080100640064046c096d0a5a0a0100640064056c0b6d0c5a0c0100640064
+      016c005a0002004700640684006407a6020000ab0200000000000000005a
+      0d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (requests)
-                 8 STORE_NAME               0 (requests)
+                 6 IMPORT_NAME              0 (os)
+                 8 STORE_NAME               0 (os)
    
-     2          10 LOAD_CONST               0 (0)
+     3          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (pandas)
-                16 STORE_NAME               2 (pd)
+                14 IMPORT_NAME              1 (requests)
+                16 STORE_NAME               1 (requests)
    
-     3          18 LOAD_CONST               0 (0)
+     4          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              3 (json)
-                24 STORE_NAME               3 (json)
+                22 IMPORT_NAME              2 (pandas)
+                24 STORE_NAME               3 (pd)
    
-     4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               2 (('Optional',))
-                30 IMPORT_NAME              4 (typing)
-                32 IMPORT_FROM              5 (Optional)
-                34 STORE_NAME               5 (Optional)
-                36 POP_TOP
+     5          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               1 (None)
+                30 IMPORT_NAME              4 (json)
+                32 STORE_NAME               4 (json)
    
-     5          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('datetime',))
-                42 IMPORT_NAME              6 (datetime)
-                44 IMPORT_FROM              6 (datetime)
-                46 STORE_NAME               6 (datetime)
-                48 POP_TOP
+     6          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               2 (('Optional',))
+                38 IMPORT_NAME              5 (typing)
+                40 IMPORT_FROM              6 (Optional)
+                42 STORE_NAME               6 (Optional)
+                44 POP_TOP
    
-     8          50 PUSH_NULL
-                52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               4 (<code object QuantsightClient, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 8>)
-                56 MAKE_FUNCTION            0
-                58 LOAD_CONST               5 ('QuantsightClient')
-                60 PRECALL                  2
-                64 CALL                     2
-                74 STORE_NAME               7 (QuantsightClient)
-                76 LOAD_CONST               1 (None)
-                78 RETURN_VALUE
+     7          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               3 (('datetime', 'timezone'))
+                50 IMPORT_NAME              7 (datetime)
+                52 IMPORT_FROM              7 (datetime)
+                54 STORE_NAME               7 (datetime)
+                56 IMPORT_FROM              8 (timezone)
+                58 STORE_NAME               8 (timezone)
+                60 POP_TOP
+   
+     8          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               4 (('pandas_cache',))
+                66 IMPORT_NAME              9 (data_cache)
+                68 IMPORT_FROM             10 (pandas_cache)
+                70 STORE_NAME              10 (pandas_cache)
+                72 POP_TOP
+   
+     9          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               5 (('Path',))
+                78 IMPORT_NAME             11 (pathlib)
+                80 IMPORT_FROM             12 (Path)
+                82 STORE_NAME              12 (Path)
+                84 POP_TOP
+   
+    10          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               1 (None)
+                90 IMPORT_NAME              0 (os)
+                92 STORE_NAME               0 (os)
+   
+    13          94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST               6 (<code object QuantsightClient, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 13>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST               7 ('QuantsightClient')
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME              13 (QuantsightClient)
+               120 LOAD_CONST               1 (None)
+               122 RETURN_VALUE
    consts
       0
       None
       ('Optional',)
-      ('datetime',)
+      ('datetime', 'timezone')
+      ('pandas_cache',)
+      ('Path',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 21
+         stacksize : 22
          flags     : 0
          code
-            0x970065005a0164005a02640165036602640284045a0464036503640465
-            05640565066a0700000000000000006606640684045a0809000900641b64
-            096509640a6509640b6503640c650a640d650b6503190000000000000000
-            00640565066a070000000000000000660c640e84055a0c09000900641b64
-            096509640a6509640b6503640f650364106503640c650a640d650b650319
-            000000000000000000640565066a0700000000000000006610641184055a
-            0d09000900641b64096509640a6509640b6503640f650364106503641265
-            036413650a640c650a640d650b650319000000000000000000640565066a
-            0700000000000000006614641484055a0e09000900641c64176503641865
-            0f6419650f640565066a0700000000000000006608641a84055a10640853
-            00
-           8           0 RESUME                   0
+            0x970065005a0164005a0209000900642464026503640365036404650466
+            06640584055a056406650364076506640865076a08000000000000000066
+            06640984045a09650a0200650b640a640b640b650c6a0d00000000000000
+            00ac0ca6040000ab0400000000000000000200650b6a0e00000000000000
+            00650c6a0d0000000000000000ac0da6010000ab01000000000000000064
+            0e640f640166056410650b6411650b641265036413650f64146510650319
+            000000000000000000640865076a080000000000000000660c64158405a6
+            000000ab0000000000000000005a11650a0200650b640a640b640b650c6a
+            0d0000000000000000ac0ca6040000ab0400000000000000000200650b6a
+            0e0000000000000000650c6a0d0000000000000000ac0da6010000ab0100
+            00000000000000640e64166417640f640166076410650b6411650b641265
+            0364186503641965036413650f6414651065031900000000000000000064
+            0865076a0800000000000000006610641a8405a6000000ab000000000000
+            0000005a12650a0900090064256410650b6411650b641265036418650364
+            196503641b6503641c650f6413650f641465106503190000000000000000
+            00640865076a0800000000000000006614641d8405a6000000ab00000000
+            00000000005a13650a090009006426642065036421651464226514640865
+            076a080000000000000000660864238405a6000000ab0000000000000000
+            005a1564015300
+          13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('QuantsightClient')
                        8 STORE_NAME               2 (__qualname__)
          
-           9          10 LOAD_CONST               1 ('api_key')
-                      12 LOAD_NAME                3 (str)
-                      14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object __init__, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 9>)
-                      18 MAKE_FUNCTION            4 (annotations)
-                      20 STORE_NAME               4 (__init__)
+          17          10 NOP
+         
+          18          12 NOP
+         
+          14          14 LOAD_CONST              36 ((None, None))
+                      16 LOAD_CONST               2 ('api_key')
+         
+          16          18 LOAD_NAME                3 (str)
+         
+          14          20 LOAD_CONST               3 ('openai_api_key')
+         
+          17          22 LOAD_NAME                3 (str)
+         
+          14          24 LOAD_CONST               4 ('cache_path')
+         
+          18          26 LOAD_NAME                4 (Path)
+         
+          14          28 BUILD_TUPLE              6
+                      30 LOAD_CONST               5 (<code object __init__, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 14>)
+                      32 MAKE_FUNCTION            5 (defaults, annotations)
+                      34 STORE_NAME               5 (__init__)
+         
+          30          36 LOAD_CONST               6 ('endpoint')
+         
+          32          38 LOAD_NAME                3 (str)
+         
+          30          40 LOAD_CONST               7 ('payload')
+         
+          33          42 LOAD_NAME                6 (dict)
+         
+          30          44 LOAD_CONST               8 ('return')
+         
+          34          46 LOAD_NAME                7 (pd)
+                      48 LOAD_ATTR                8 (DataFrame)
+         
+          30          58 BUILD_TUPLE              6
+                      60 LOAD_CONST               9 (<code object _request, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 30>)
+                      62 MAKE_FUNCTION            4 (annotations)
+                      64 STORE_NAME               9 (_request)
+         
+          49          66 LOAD_NAME               10 (pandas_cache)
          
-          13          22 LOAD_CONST               3 ('endpoint')
+          52          68 PUSH_NULL
+                      70 LOAD_NAME               11 (datetime)
+                      72 LOAD_CONST              10 (2010)
+                      74 LOAD_CONST              11 (1)
+                      76 LOAD_CONST              11 (1)
+                      78 LOAD_NAME               12 (timezone)
+                      80 LOAD_ATTR               13 (utc)
+                      90 KW_NAMES                12
+                      92 PRECALL                  4
+                      96 CALL                     4
          
-          15          24 LOAD_NAME                3 (str)
+          53         106 PUSH_NULL
+                     108 LOAD_NAME               11 (datetime)
+                     110 LOAD_ATTR               14 (now)
+                     120 LOAD_NAME               12 (timezone)
+                     122 LOAD_ATTR               13 (utc)
+                     132 KW_NAMES                13
+                     134 PRECALL                  1
+                     138 CALL                     1
          
-          13          26 LOAD_CONST               4 ('payload')
+          54         148 LOAD_CONST              14 ('okx')
          
-          16          28 LOAD_NAME                5 (dict)
+          55         150 LOAD_CONST              15 (100)
          
-          13          30 LOAD_CONST               5 ('return')
+          56         152 LOAD_CONST               1 (None)
          
-          17          32 LOAD_NAME                6 (pd)
-                      34 LOAD_ATTR                7 (DataFrame)
+          50         154 BUILD_TUPLE              5
+                     156 LOAD_CONST              16 ('from_ts')
          
-          13          44 BUILD_TUPLE              6
-                      46 LOAD_CONST               6 (<code object _request, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 13>)
-                      48 MAKE_FUNCTION            4 (annotations)
-                      50 STORE_NAME               8 (_request)
+          52         158 LOAD_NAME               11 (datetime)
          
-          32          52 NOP
+          50         160 LOAD_CONST              17 ('to_ts')
          
-          33          54 NOP
+          53         162 LOAD_NAME               11 (datetime)
          
-          27          56 LOAD_CONST              27 ((100, None))
-                      58 LOAD_CONST               9 ('from_ts')
+          50         164 LOAD_CONST              18 ('exchange')
          
-          29          60 LOAD_NAME                9 (datetime)
+          54         166 LOAD_NAME                3 (str)
          
-          27          62 LOAD_CONST              10 ('to_ts')
+          50         168 LOAD_CONST              19 ('limit')
          
-          30          64 LOAD_NAME                9 (datetime)
+          55         170 LOAD_NAME               15 (int)
          
-          27          66 LOAD_CONST              11 ('exchange')
+          50         172 LOAD_CONST              20 ('ticker')
          
-          31          68 LOAD_NAME                3 (str)
+          56         174 LOAD_NAME               16 (Optional)
+                     176 LOAD_NAME                3 (str)
+                     178 BINARY_SUBSCR
          
-          27          70 LOAD_CONST              12 ('limit')
+          50         188 LOAD_CONST               8 ('return')
          
-          32          72 LOAD_NAME               10 (int)
+          57         190 LOAD_NAME                7 (pd)
+                     192 LOAD_ATTR                8 (DataFrame)
          
-          27          74 LOAD_CONST              13 ('ticker')
+          50         202 BUILD_TUPLE             12
+                     204 LOAD_CONST              21 (<code object get_funding_rate, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 49>)
+                     206 MAKE_FUNCTION            5 (defaults, annotations)
          
-          33          76 LOAD_NAME               11 (Optional)
-                      78 LOAD_NAME                3 (str)
-                      80 BINARY_SUBSCR
+          49         208 PRECALL                  0
+                     212 CALL                     0
          
-          27          90 LOAD_CONST               5 ('return')
+          50         222 STORE_NAME              17 (get_funding_rate)
          
-          34          92 LOAD_NAME                6 (pd)
-                      94 LOAD_ATTR                7 (DataFrame)
+          67         224 LOAD_NAME               10 (pandas_cache)
          
-          27         104 BUILD_TUPLE             12
-                     106 LOAD_CONST              14 (<code object get_funding_rate, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 27>)
-                     108 MAKE_FUNCTION            5 (defaults, annotations)
-                     110 STORE_NAME              12 (get_funding_rate)
+          70         226 PUSH_NULL
+                     228 LOAD_NAME               11 (datetime)
+                     230 LOAD_CONST              10 (2010)
+                     232 LOAD_CONST              11 (1)
+                     234 LOAD_CONST              11 (1)
+                     236 LOAD_NAME               12 (timezone)
+                     238 LOAD_ATTR               13 (utc)
+                     248 KW_NAMES                12
+                     250 PRECALL                  4
+                     254 CALL                     4
          
-          51         112 NOP
+          71         264 PUSH_NULL
+                     266 LOAD_NAME               11 (datetime)
+                     268 LOAD_ATTR               14 (now)
+                     278 LOAD_NAME               12 (timezone)
+                     280 LOAD_ATTR               13 (utc)
+                     290 KW_NAMES                13
+                     292 PRECALL                  1
+                     296 CALL                     1
          
-          52         114 NOP
+          72         306 LOAD_CONST              14 ('okx')
          
-          44         116 LOAD_CONST              27 ((100, None))
-                     118 LOAD_CONST               9 ('from_ts')
+          73         308 LOAD_CONST              22 ('1d')
          
-          46         120 LOAD_NAME                9 (datetime)
+          74         310 LOAD_CONST              23 ('swap')
          
-          44         122 LOAD_CONST              10 ('to_ts')
+          75         312 LOAD_CONST              15 (100)
          
-          47         124 LOAD_NAME                9 (datetime)
+          76         314 LOAD_CONST               1 (None)
          
-          44         126 LOAD_CONST              11 ('exchange')
+          68         316 BUILD_TUPLE              7
+                     318 LOAD_CONST              16 ('from_ts')
          
-          48         128 LOAD_NAME                3 (str)
+          70         320 LOAD_NAME               11 (datetime)
          
-          44         130 LOAD_CONST              15 ('period')
+          68         322 LOAD_CONST              17 ('to_ts')
          
-          49         132 LOAD_NAME                3 (str)
+          71         324 LOAD_NAME               11 (datetime)
          
-          44         134 LOAD_CONST              16 ('instrument')
+          68         326 LOAD_CONST              18 ('exchange')
          
-          50         136 LOAD_NAME                3 (str)
+          72         328 LOAD_NAME                3 (str)
          
-          44         138 LOAD_CONST              12 ('limit')
+          68         330 LOAD_CONST              24 ('period')
          
-          51         140 LOAD_NAME               10 (int)
+          73         332 LOAD_NAME                3 (str)
          
-          44         142 LOAD_CONST              13 ('ticker')
+          68         334 LOAD_CONST              25 ('instrument')
          
-          52         144 LOAD_NAME               11 (Optional)
-                     146 LOAD_NAME                3 (str)
-                     148 BINARY_SUBSCR
+          74         336 LOAD_NAME                3 (str)
          
-          44         158 LOAD_CONST               5 ('return')
+          68         338 LOAD_CONST              19 ('limit')
          
-          53         160 LOAD_NAME                6 (pd)
-                     162 LOAD_ATTR                7 (DataFrame)
+          75         340 LOAD_NAME               15 (int)
          
-          44         172 BUILD_TUPLE             16
-                     174 LOAD_CONST              17 (<code object get_ohlcv, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 44>)
-                     176 MAKE_FUNCTION            5 (defaults, annotations)
-                     178 STORE_NAME              13 (get_ohlcv)
+          68         342 LOAD_CONST              20 ('ticker')
          
-          74         180 NOP
+          76         344 LOAD_NAME               16 (Optional)
+                     346 LOAD_NAME                3 (str)
+                     348 BINARY_SUBSCR
          
-          75         182 NOP
+          68         358 LOAD_CONST               8 ('return')
          
-          65         184 LOAD_CONST              27 ((100, None))
-                     186 LOAD_CONST               9 ('from_ts')
+          77         360 LOAD_NAME                7 (pd)
+                     362 LOAD_ATTR                8 (DataFrame)
          
-          67         188 LOAD_NAME                9 (datetime)
+          68         372 BUILD_TUPLE             16
+                     374 LOAD_CONST              26 (<code object get_ohlcv, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 67>)
+                     376 MAKE_FUNCTION            5 (defaults, annotations)
          
-          65         190 LOAD_CONST              10 ('to_ts')
+          67         378 PRECALL                  0
+                     382 CALL                     0
          
-          68         192 LOAD_NAME                9 (datetime)
+          68         392 STORE_NAME              18 (get_ohlcv)
          
-          65         194 LOAD_CONST              11 ('exchange')
+          89         394 LOAD_NAME               10 (pandas_cache)
          
-          69         196 LOAD_NAME                3 (str)
+          99         396 NOP
          
-          65         198 LOAD_CONST              15 ('period')
+         100         398 NOP
          
-          70         200 LOAD_NAME                3 (str)
+          90         400 LOAD_CONST              37 ((100, None))
+                     402 LOAD_CONST              16 ('from_ts')
          
-          65         202 LOAD_CONST              16 ('instrument')
+          92         404 LOAD_NAME               11 (datetime)
          
-          71         204 LOAD_NAME                3 (str)
+          90         406 LOAD_CONST              17 ('to_ts')
          
-          65         206 LOAD_CONST              18 ('target_time')
+          93         408 LOAD_NAME               11 (datetime)
          
-          72         208 LOAD_NAME                3 (str)
+          90         410 LOAD_CONST              18 ('exchange')
          
-          65         210 LOAD_CONST              19 ('sample_count')
+          94         412 LOAD_NAME                3 (str)
          
-          73         212 LOAD_NAME               10 (int)
+          90         414 LOAD_CONST              24 ('period')
          
-          65         214 LOAD_CONST              12 ('limit')
+          95         416 LOAD_NAME                3 (str)
          
-          74         216 LOAD_NAME               10 (int)
+          90         418 LOAD_CONST              25 ('instrument')
          
-          65         218 LOAD_CONST              13 ('ticker')
+          96         420 LOAD_NAME                3 (str)
          
-          75         220 LOAD_NAME               11 (Optional)
-                     222 LOAD_NAME                3 (str)
-                     224 BINARY_SUBSCR
+          90         422 LOAD_CONST              27 ('target_time')
          
-          65         234 LOAD_CONST               5 ('return')
+          97         424 LOAD_NAME                3 (str)
          
-          76         236 LOAD_NAME                6 (pd)
-                     238 LOAD_ATTR                7 (DataFrame)
+          90         426 LOAD_CONST              28 ('sample_count')
          
-          65         248 BUILD_TUPLE             20
-                     250 LOAD_CONST              20 (<code object get_ohlcv_around_time, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 65>)
-                     252 MAKE_FUNCTION            5 (defaults, annotations)
-                     254 STORE_NAME              14 (get_ohlcv_around_time)
+          98         428 LOAD_NAME               15 (int)
          
-          93         256 NOP
+          90         430 LOAD_CONST              19 ('limit')
          
-          94         258 NOP
+          99         432 LOAD_NAME               15 (int)
          
-          90         260 LOAD_CONST              28 ((True, False))
-                     262 LOAD_CONST              23 ('query')
+          90         434 LOAD_CONST              20 ('ticker')
          
-          92         264 LOAD_NAME                3 (str)
+         100         436 LOAD_NAME               16 (Optional)
+                     438 LOAD_NAME                3 (str)
+                     440 BINARY_SUBSCR
          
-          90         266 LOAD_CONST              24 ('dry_run')
+          90         450 LOAD_CONST               8 ('return')
          
-          93         268 LOAD_NAME               15 (bool)
+         101         452 LOAD_NAME                7 (pd)
+                     454 LOAD_ATTR                8 (DataFrame)
          
-          90         270 LOAD_CONST              25 ('use_legacy_sql')
+          90         464 BUILD_TUPLE             20
+                     466 LOAD_CONST              29 (<code object get_ohlcv_around_time, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 89>)
+                     468 MAKE_FUNCTION            5 (defaults, annotations)
          
-          94         272 LOAD_NAME               15 (bool)
+          89         470 PRECALL                  0
+                     474 CALL                     0
          
-          90         274 LOAD_CONST               5 ('return')
+          90         484 STORE_NAME              19 (get_ohlcv_around_time)
          
-          95         276 LOAD_NAME                6 (pd)
-                     278 LOAD_ATTR                7 (DataFrame)
+         115         486 LOAD_NAME               10 (pandas_cache)
          
-          90         288 BUILD_TUPLE              8
-                     290 LOAD_CONST              26 (<code object custom_query, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 90>)
-                     292 MAKE_FUNCTION            5 (defaults, annotations)
-                     294 STORE_NAME              16 (custom_query)
-                     296 LOAD_CONST               8 (None)
-                     298 RETURN_VALUE
+         119         488 NOP
+         
+         120         490 NOP
+         
+         116         492 LOAD_CONST              38 ((True, False))
+                     494 LOAD_CONST              32 ('query')
+         
+         118         496 LOAD_NAME                3 (str)
+         
+         116         498 LOAD_CONST              33 ('dry_run')
+         
+         119         500 LOAD_NAME               20 (bool)
+         
+         116         502 LOAD_CONST              34 ('use_legacy_sql')
+         
+         120         504 LOAD_NAME               20 (bool)
+         
+         116         506 LOAD_CONST               8 ('return')
+         
+         121         508 LOAD_NAME                7 (pd)
+                     510 LOAD_ATTR                8 (DataFrame)
+         
+         116         520 BUILD_TUPLE              8
+                     522 LOAD_CONST              35 (<code object custom_query, file "/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py", line 115>)
+                     524 MAKE_FUNCTION            5 (defaults, annotations)
+         
+         115         526 PRECALL                  0
+                     530 CALL                     0
+         
+         116         540 STORE_NAME              21 (custom_query)
+                     542 LOAD_CONST               1 (None)
+                     544 RETURN_VALUE
          consts
             'QuantsightClient'
+            None
             'api_key'
+            'openai_api_key'
+            'cache_path'
             code
-               argcount  : 2
-               nlocals   : 2
+               argcount  : 4
+               nlocals   : 5
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f000000000000000000640264037c019b009d0269017c
-                  005f01000000000000000064005300
-                 9           0 RESUME                   0
+                  005f01000000000000000074050000000000000000000074060000000000
+                  0000000000a6010000ab010000000000000000a004000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000006a05000000
+                  00000000007d047c0380027c047d03740d000000000000000000007c03a6
+                  010000ab010000000000000000740e000000000000000000006a08000000
+                  000000000064043c00000064005300
+                14           0 RESUME                   0
                
-                10           2 LOAD_CONST               1 ('https://api.quantsight.dev')
+                20           2 LOAD_CONST               1 ('https://api.quantsight.dev')
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (base_url)
                
-                11          16 LOAD_CONST               2 ('Authorization')
+                21          16 LOAD_CONST               2 ('Authorization')
                             18 LOAD_CONST               3 ('Bearer ')
                             20 LOAD_FAST                1 (api_key)
                             22 FORMAT_VALUE             0
                             24 BUILD_STRING             2
                             26 BUILD_MAP                1
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (headers)
-                            40 LOAD_CONST               0 (None)
-                            42 RETURN_VALUE
+               
+                23          40 LOAD_GLOBAL              5 (NULL + Path)
+                            52 LOAD_GLOBAL              6 (__file__)
+                            64 PRECALL                  1
+                            68 CALL                     1
+                            78 LOAD_METHOD              4 (resolve)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 LOAD_ATTR                5 (parent)
+                           124 STORE_FAST               4 (file_location)
+               
+                25         126 LOAD_FAST                3 (cache_path)
+                           128 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 134)
+               
+                26         130 LOAD_FAST                4 (file_location)
+                           132 STORE_FAST               3 (cache_path)
+               
+                28     >>  134 LOAD_GLOBAL             13 (NULL + str)
+                           146 LOAD_FAST                3 (cache_path)
+                           148 PRECALL                  1
+                           152 CALL                     1
+                           162 LOAD_GLOBAL             14 (os)
+                           174 LOAD_ATTR                8 (environ)
+                           184 LOAD_CONST               4 ('CACHE_PATH')
+                           186 STORE_SUBSCR
+                           190 LOAD_CONST               0 (None)
+                           192 RETURN_VALUE
                consts
                   None
                   'https://api.quantsight.dev'
                   'Authorization'
                   'Bearer '
-               names      ('base_url', 'headers')
-               varnames   ('self', 'api_key')
+                  'CACHE_PATH'
+               names      ('base_url', 'headers', 'Path', '__file__', 'resolve', 'parent', 'str', 'os', 'environ')
+               varnames   ('self', 'api_key', 'openai_api_key', 'cache_path', 'file_location')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       '__init__'
-               firstlineno 9
-               lnotab 0x02010e01
+               firstlineno 14
+               lnotab 0x02060e011802560204010402
             'endpoint'
             'payload'
             'return'
             code
                argcount  : 3
-               nlocals   : 6
-               stacksize : 5
+               nlocals   : 7
+               stacksize : 7
                flags     : 3
                code
                   0x97007c006a0000000000000000009b007c019b009d027d037403000000
                   000000000000006a0200000000000000007c037c006a0300000000000000
                   007c02ac01a6030000ab0300000000000000007d047c046a040000000000
-                  00000064026b03000000007217740b0000000000000000000064037c046a
-                  0400000000000000009b009d02a6010000ab010000000000000000820174
-                  0d000000000000000000006a0700000000000000007c046a080000000000
-                  000000a6010000ab0100000000000000007d057413000000000000000000
-                  006a0a00000000000000007c05a6010000ab0100000000000000005300
-                13           0 RESUME                   0
+                  00000064026b0300000000722c740b0000000000000000000064037c046a
+                  0400000000000000009b0064047c04a00600000000000000000000000000
+                  00000000000000a6000000ab0000000000000000009b009d04a6010000ab
+                  0100000000000000008201740d000000000000000000006a070000000000
+                  0000007c046a080000000000000000a6010000ab0100000000000000007d
+                  057413000000000000000000006a0a00000000000000007c05a6010000ab
+                  0100000000000000007d0664057c066a0b00000000000000007600721d74
+                  13000000000000000000006a0c00000000000000007c0664051900000000
+                  0000000000a6010000ab0100000000000000007c0664053c0000007c0653
+                  00
+                30           0 RESUME                   0
                
-                18           2 LOAD_FAST                0 (self)
+                35           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (base_url)
                             14 FORMAT_VALUE             0
                             16 LOAD_FAST                1 (endpoint)
                             18 FORMAT_VALUE             0
                             20 BUILD_STRING             2
                             22 STORE_FAST               3 (url)
                
-                19          24 LOAD_GLOBAL              3 (NULL + requests)
+                36          24 LOAD_GLOBAL              3 (NULL + requests)
                             36 LOAD_ATTR                2 (get)
                             46 LOAD_FAST                3 (url)
                             48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                3 (headers)
                             60 LOAD_FAST                2 (payload)
                             62 KW_NAMES                 1
                             64 PRECALL                  3
                             68 CALL                     3
                             78 STORE_FAST               4 (response)
                
-                21          80 LOAD_FAST                4 (response)
+                38          80 LOAD_FAST                4 (response)
                             82 LOAD_ATTR                4 (status_code)
                             92 LOAD_CONST               2 (200)
                             94 COMPARE_OP               3 (!=)
-                           100 POP_JUMP_FORWARD_IF_FALSE    23 (to 148)
+                           100 POP_JUMP_FORWARD_IF_FALSE    44 (to 190)
                
-                22         102 LOAD_GLOBAL             11 (NULL + Exception)
+                39         102 LOAD_GLOBAL             11 (NULL + Exception)
                            114 LOAD_CONST               3 ('Request failed with status code ')
                            116 LOAD_FAST                4 (response)
                            118 LOAD_ATTR                4 (status_code)
                            128 FORMAT_VALUE             0
-                           130 BUILD_STRING             2
-                           132 PRECALL                  1
-                           136 CALL                     1
-                           146 RAISE_VARARGS            1
-               
-                24     >>  148 LOAD_GLOBAL             13 (NULL + json)
-                           160 LOAD_ATTR                7 (loads)
-                           170 LOAD_FAST                4 (response)
-                           172 LOAD_ATTR                8 (text)
-                           182 PRECALL                  1
-                           186 CALL                     1
-                           196 STORE_FAST               5 (data)
-               
-                25         198 LOAD_GLOBAL             19 (NULL + pd)
-                           210 LOAD_ATTR               10 (DataFrame)
-                           220 LOAD_FAST                5 (data)
-                           222 PRECALL                  1
-                           226 CALL                     1
-                           236 RETURN_VALUE
+                           130 LOAD_CONST               4 (': \n ')
+                           132 LOAD_FAST                4 (response)
+                           134 LOAD_METHOD              6 (json)
+                           156 PRECALL                  0
+                           160 CALL                     0
+                           170 FORMAT_VALUE             0
+                           172 BUILD_STRING             4
+                           174 PRECALL                  1
+                           178 CALL                     1
+                           188 RAISE_VARARGS            1
+               
+                41     >>  190 LOAD_GLOBAL             13 (NULL + json)
+                           202 LOAD_ATTR                7 (loads)
+                           212 LOAD_FAST                4 (response)
+                           214 LOAD_ATTR                8 (text)
+                           224 PRECALL                  1
+                           228 CALL                     1
+                           238 STORE_FAST               5 (data)
+               
+                42         240 LOAD_GLOBAL             19 (NULL + pd)
+                           252 LOAD_ATTR               10 (DataFrame)
+                           262 LOAD_FAST                5 (data)
+                           264 PRECALL                  1
+                           268 CALL                     1
+                           278 STORE_FAST               6 (df)
+               
+                44         280 LOAD_CONST               5 ('ts')
+                           282 LOAD_FAST                6 (df)
+                           284 LOAD_ATTR               11 (columns)
+                           294 CONTAINS_OP              0
+                           296 POP_JUMP_FORWARD_IF_FALSE    29 (to 356)
+               
+                45         298 LOAD_GLOBAL             19 (NULL + pd)
+                           310 LOAD_ATTR               12 (to_datetime)
+                           320 LOAD_FAST                6 (df)
+                           322 LOAD_CONST               5 ('ts')
+                           324 BINARY_SUBSCR
+                           334 PRECALL                  1
+                           338 CALL                     1
+                           348 LOAD_FAST                6 (df)
+                           350 LOAD_CONST               5 ('ts')
+                           352 STORE_SUBSCR
+               
+                47     >>  356 LOAD_FAST                6 (df)
+                           358 RETURN_VALUE
                consts
                   None
                   ('headers', 'json')
                   200
                   'Request failed with status code '
-               names      ('base_url', 'requests', 'get', 'headers', 'status_code', 'Exception', 'json', 'loads', 'text', 'pd', 'DataFrame')
-               varnames   ('self', 'endpoint', 'payload', 'url', 'response', 'data')
+                  ': \n '
+                  'ts'
+               names      ('base_url', 'requests', 'get', 'headers', 'status_code', 'Exception', 'json', 'loads', 'text', 'pd', 'DataFrame', 'columns', 'to_datetime')
+               varnames   ('self', 'endpoint', 'payload', 'url', 'response', 'data', 'df')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       '_request'
-               firstlineno 13
-               lnotab 0x02051601380216012e023201
+               firstlineno 30
+               lnotab 0x020516013802160158023201280212013a02
+            2010
+            1
+            ('tzinfo',)
+            ('tz',)
+            'okx'
             100
-            None
             'from_ts'
             'to_ts'
             'exchange'
             'limit'
             'ticker'
             code
                argcount  : 6
@@ -402,37 +598,37 @@
                flags     : 3
                code
                   0x97007c01a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007c02a000000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007c037c047c0564019c057d
                   067c00a001000000000000000000000000000000000000000064027c06a6
                   020000ab0200000000000000005300
-                27           0 RESUME                   0
+                49           0 RESUME                   0
                
-                36           2 LOAD_FAST                1 (from_ts)
+                59           2 LOAD_FAST                1 (from_ts)
                              4 LOAD_METHOD              0 (isoformat)
                             26 PRECALL                  0
                             30 CALL                     0
                
-                37          40 LOAD_FAST                2 (to_ts)
+                60          40 LOAD_FAST                2 (to_ts)
                             42 LOAD_METHOD              0 (isoformat)
                             64 PRECALL                  0
                             68 CALL                     0
                
-                38          78 LOAD_FAST                3 (exchange)
+                61          78 LOAD_FAST                3 (exchange)
                
-                39          80 LOAD_FAST                4 (limit)
+                62          80 LOAD_FAST                4 (limit)
                
-                40          82 LOAD_FAST                5 (ticker)
+                63          82 LOAD_FAST                5 (ticker)
                
-                35          84 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'limit', 'ticker'))
+                58          84 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'limit', 'ticker'))
                             86 BUILD_CONST_KEY_MAP      5
                             88 STORE_FAST               6 (payload)
                
-                42          90 LOAD_FAST                0 (self)
+                65          90 LOAD_FAST                0 (self)
                             92 LOAD_METHOD              1 (_request)
                            114 LOAD_CONST               2 ('/get_funding_rate')
                            116 LOAD_FAST                6 (payload)
                            118 PRECALL                  2
                            122 CALL                     2
                            132 RETURN_VALUE
                consts
@@ -441,56 +637,58 @@
                   '/get_funding_rate'
                names      ('isoformat', '_request')
                varnames   ('self', 'from_ts', 'to_ts', 'exchange', 'limit', 'ticker', 'payload')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       'get_funding_rate'
-               firstlineno 27
-               lnotab 0x0209260126010201020102fb0607
+               firstlineno 49
+               lnotab 0x020a260126010201020102fb0607
+            '1d'
+            'swap'
             'period'
             'instrument'
             code
                argcount  : 8
                nlocals   : 9
                stacksize : 8
                flags     : 3
                code
                   0x97007c01a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007c02a000000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007c037c047c057c067c0764
                   019c077d087c00a001000000000000000000000000000000000000000064
                   027c08a6020000ab0200000000000000005300
-                44           0 RESUME                   0
+                67           0 RESUME                   0
                
-                55           2 LOAD_FAST                1 (from_ts)
+                79           2 LOAD_FAST                1 (from_ts)
                              4 LOAD_METHOD              0 (isoformat)
                             26 PRECALL                  0
                             30 CALL                     0
                
-                56          40 LOAD_FAST                2 (to_ts)
+                80          40 LOAD_FAST                2 (to_ts)
                             42 LOAD_METHOD              0 (isoformat)
                             64 PRECALL                  0
                             68 CALL                     0
                
-                57          78 LOAD_FAST                3 (exchange)
+                81          78 LOAD_FAST                3 (exchange)
                
-                58          80 LOAD_FAST                4 (period)
+                82          80 LOAD_FAST                4 (period)
                
-                59          82 LOAD_FAST                5 (instrument)
+                83          82 LOAD_FAST                5 (instrument)
                
-                60          84 LOAD_FAST                6 (limit)
+                84          84 LOAD_FAST                6 (limit)
                
-                61          86 LOAD_FAST                7 (ticker)
+                85          86 LOAD_FAST                7 (ticker)
                
-                54          88 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'limit', 'ticker'))
+                78          88 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'limit', 'ticker'))
                             90 BUILD_CONST_KEY_MAP      7
                             92 STORE_FAST               8 (payload)
                
-                63          94 LOAD_FAST                0 (self)
+                87          94 LOAD_FAST                0 (self)
                             96 LOAD_METHOD              1 (_request)
                            118 LOAD_CONST               2 ('/get_ohlcv')
                            120 LOAD_FAST                8 (payload)
                            122 PRECALL                  2
                            126 CALL                     2
                            136 RETURN_VALUE
                consts
@@ -499,60 +697,60 @@
                   '/get_ohlcv'
                names      ('isoformat', '_request')
                varnames   ('self', 'from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'limit', 'ticker', 'payload')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       'get_ohlcv'
-               firstlineno 44
-               lnotab 0x020b26012601020102010201020102f90609
+               firstlineno 67
+               lnotab 0x020c26012601020102010201020102f90609
             'target_time'
             'sample_count'
             code
                argcount  : 10
                nlocals   : 11
                stacksize : 10
                flags     : 3
                code
                   0x97007c01a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007c02a000000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007c037c047c057c067c077c
                   087c0964019c097d0a7c00a0010000000000000000000000000000000000
                   00000064027c0aa6020000ab0200000000000000005300
-                65           0 RESUME                   0
+                89           0 RESUME                   0
                
-                78           2 LOAD_FAST                1 (from_ts)
+               103           2 LOAD_FAST                1 (from_ts)
                              4 LOAD_METHOD              0 (isoformat)
                             26 PRECALL                  0
                             30 CALL                     0
                
-                79          40 LOAD_FAST                2 (to_ts)
+               104          40 LOAD_FAST                2 (to_ts)
                             42 LOAD_METHOD              0 (isoformat)
                             64 PRECALL                  0
                             68 CALL                     0
                
-                80          78 LOAD_FAST                3 (exchange)
+               105          78 LOAD_FAST                3 (exchange)
                
-                81          80 LOAD_FAST                4 (period)
+               106          80 LOAD_FAST                4 (period)
                
-                82          82 LOAD_FAST                5 (instrument)
+               107          82 LOAD_FAST                5 (instrument)
                
-                83          84 LOAD_FAST                6 (target_time)
+               108          84 LOAD_FAST                6 (target_time)
                
-                84          86 LOAD_FAST                7 (sample_count)
+               109          86 LOAD_FAST                7 (sample_count)
                
-                85          88 LOAD_FAST                8 (limit)
+               110          88 LOAD_FAST                8 (limit)
                
-                86          90 LOAD_FAST                9 (ticker)
+               111          90 LOAD_FAST                9 (ticker)
                
-                77          92 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'target_time', 'sample_count', 'limit', 'ticker'))
+               102          92 LOAD_CONST               1 (('from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'target_time', 'sample_count', 'limit', 'ticker'))
                             94 BUILD_CONST_KEY_MAP      9
                             96 STORE_FAST              10 (payload)
                
-                88          98 LOAD_FAST                0 (self)
+               113          98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              1 (_request)
                            122 LOAD_CONST               2 ('/get_ohlcv_around_time')
                            124 LOAD_FAST               10 (payload)
                            126 PRECALL                  2
                            130 CALL                     2
                            140 RETURN_VALUE
                consts
@@ -561,42 +759,42 @@
                   '/get_ohlcv_around_time'
                names      ('isoformat', '_request')
                varnames   ('self', 'from_ts', 'to_ts', 'exchange', 'period', 'instrument', 'target_time', 'sample_count', 'limit', 'ticker', 'payload')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       'get_ohlcv_around_time'
-               firstlineno 65
-               lnotab 0x020d2601260102010201020102010201020102f7060b
+               firstlineno 89
+               lnotab 0x020e2601260102010201020102010201020102f7060b
             True
             False
             'query'
             'dry_run'
             'use_legacy_sql'
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 4
                flags     : 3
                code
                   0x97007c017c027c0364019c037d047c00a0000000000000000000000000
                   00000000000000000064027c04a6020000ab0200000000000000005300
-                90           0 RESUME                   0
+               115           0 RESUME                   0
                
-                97           2 LOAD_FAST                1 (query)
+               123           2 LOAD_FAST                1 (query)
                
-                98           4 LOAD_FAST                2 (dry_run)
+               124           4 LOAD_FAST                2 (dry_run)
                
-                99           6 LOAD_FAST                3 (use_legacy_sql)
+               125           6 LOAD_FAST                3 (use_legacy_sql)
                
-                96           8 LOAD_CONST               1 (('query', 'dry_run', 'use_legacy_sql'))
+               122           8 LOAD_CONST               1 (('query', 'dry_run', 'use_legacy_sql'))
                             10 BUILD_CONST_KEY_MAP      3
                             12 STORE_FAST               4 (payload)
                
-               101          14 LOAD_FAST                0 (self)
+               127          14 LOAD_FAST                0 (self)
                             16 LOAD_METHOD              0 (_request)
                             38 LOAD_CONST               2 ('/custom_query')
                             40 LOAD_FAST                4 (payload)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 RETURN_VALUE
                consts
@@ -605,34 +803,36 @@
                   '/custom_query'
                names      ('_request',)
                varnames   ('self', 'query', 'dry_run', 'use_legacy_sql', 'payload')
                freevars   ()
                cellvars   ()
                filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
                name       'custom_query'
-               firstlineno 90
-               lnotab 0x02070201020102fd0605
+               firstlineno 115
+               lnotab 0x02080201020102fd0605
+            (None, None)
             (100, None)
             (True, False)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'dict', 'pd', 'DataFrame', '_request', 'datetime', 'int', 'Optional', 'get_funding_rate', 'get_ohlcv', 'get_ohlcv_around_time', 'bool', 'custom_query')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'Path', '__init__', 'dict', 'pd', 'DataFrame', '_request', 'pandas_cache', 'datetime', 'timezone', 'utc', 'now', 'int', 'Optional', 'get_funding_rate', 'get_ohlcv', 'get_ohlcv_around_time', 'bool', 'custom_query')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
          name       'QuantsightClient'
-         firstlineno 8
+         firstlineno 13
          lnotab
-            0x0a010c04020202fe020302fd02040cfc0813020102fa040202fe020302
-            fd020402fc020502fb02060efa02070cf90818020102f8040202fe020302
-            fd020402fc020502fb020602fa020702f902080ef802090cf7081e020102
-            f6040202fe020302fd020402fc020502fb020602fa020702f9020802f802
-            0902f7020a0ef6020b0cf5081c020102fc040202fe020302fd020402fc02
-            050cfb
+            0x0a04020102fc040202fe020302fd020402fc0810020202fe020302fd02
+            040cfc0813020326012a010201020102fa040202fe020302fd020402fc02
+            0502fb02060efa02070cf906ff0e010211020326012a0102010201020102
+            0102f8040202fe020302fd020402fc020502fb020602fa020702f902080e
+            f802090cf706ff0e010215020a020102f6040202fe020302fd020402fc02
+            0502fb020602fa020702f9020802f8020902f7020a0ef6020b0cf506ff0e
+            0102190204020102fc040202fe020302fd020402fc02050cfb06ff0e01
       'QuantsightClient'
-   names      ('requests', 'pandas', 'pd', 'json', 'typing', 'Optional', 'datetime', 'QuantsightClient')
+   names      ('os', 'requests', 'pandas', 'pd', 'json', 'typing', 'Optional', 'datetime', 'timezone', 'data_cache', 'pandas_cache', 'pathlib', 'Path', 'QuantsightClient')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080108010c010c03
+   lnotab 0x00ff020108020801080108010c0110010c010c010803
```

### ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py

```diff
@@ -1,71 +1,96 @@
+import os
+
 import requests
 import pandas as pd
 import json
 from typing import Optional
-from datetime import datetime
+from datetime import datetime, timezone
+from data_cache import pandas_cache
+from pathlib import Path
+import os
 
 
 class QuantsightClient:
-    def __init__(self, api_key: str):
+    def __init__(
+            self,
+            api_key: str,
+            openai_api_key: str = None,
+            cache_path: Path = None
+    ):
         self.base_url = "https://api.quantsight.dev"
         self.headers = {"Authorization": f"Bearer {api_key}"}
 
+        file_location = Path(__file__).resolve().parent
+
+        if cache_path is None:
+            cache_path = file_location
+
+        os.environ["CACHE_PATH"] = str(cache_path)
+
     def _request(
             self,
             endpoint: str,
             payload: dict
     ) -> pd.DataFrame:
         url = f"{self.base_url}{endpoint}"
         response = requests.get(url, headers=self.headers, json=payload)
 
         if response.status_code != 200:
-            raise Exception(f"Request failed with status code {response.status_code}")
+            raise Exception(f"Request failed with status code {response.status_code}: \n {response.json()}")
 
         data = json.loads(response.text)
-        return pd.DataFrame(data)
+        df = pd.DataFrame(data)
+
+        if "ts" in df.columns:
+            df['ts'] = pd.to_datetime(df['ts'])
 
+        return df
+
+    @pandas_cache
     def get_funding_rate(
             self,
-            from_ts: datetime,
-            to_ts: datetime,
-            exchange: str,
+            from_ts: datetime = datetime(2010, 1, 1, tzinfo=timezone.utc),
+            to_ts: datetime = datetime.now(tz=timezone.utc),
+            exchange: str = "okx",
             limit: int = 100,
             ticker: Optional[str] = None
     ) -> pd.DataFrame:
         payload = {
             "from_ts": from_ts.isoformat(),
             "to_ts": to_ts.isoformat(),
             "exchange": exchange,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_funding_rate", payload)
 
+    @pandas_cache
     def get_ohlcv(
             self,
-            from_ts: datetime,
-            to_ts: datetime,
-            exchange: str,
-            period: str,
-            instrument: str,
+            from_ts: datetime = datetime(2010, 1, 1, tzinfo=timezone.utc),
+            to_ts: datetime = datetime.now(tz=timezone.utc),
+            exchange: str = "okx",
+            period: str = "1d",
+            instrument: str = "swap",
             limit: int = 100,
             ticker: Optional[str] = None
     ) -> pd.DataFrame:
         payload = {
             "from_ts": from_ts.isoformat(),
             "to_ts": to_ts.isoformat(),
             "exchange": exchange,
             "period": period,
             "instrument": instrument,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_ohlcv", payload)
 
+    @pandas_cache
     def get_ohlcv_around_time(
             self,
             from_ts: datetime,
             to_ts: datetime,
             exchange: str,
             period: str,
             instrument: str,
@@ -83,14 +108,15 @@
             "target_time": target_time,
             "sample_count": sample_count,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_ohlcv_around_time", payload)
 
+    @pandas_cache
     def custom_query(
             self,
             query: str,
             dry_run: bool = True,
             use_legacy_sql: bool = False
     ) -> pd.DataFrame:
         payload = {
```

### Comparing `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.2-py3.11.egg-info/PKG-INFO` & `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 2.1
 Name: quantsight
-Version: 0.1.2
+Version: 0.1.3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml) [![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
+[![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml)
+[![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
+[![PyPI version](https://img.shields.io/badge/Quantsight-Visit%20Website-blue.svg)](https://www.quantsight.dev/)
 
 <img height="60" src="https://www.quantsight.dev/static/media/trades.2cd0b7149637f5303dd5.png"/>
 
 This is a Python client for the Quantsight Data API, which allows you to fetch historical funding rates, candle data, and perform custom queries from supported exchanges. The client is easy to use and supports fetching data into a Pandas DataFrame for further analysis.
 
+### Key features:
+
+
+#### ✅ Pull data from API directly as a pandas DataFrame
+#### ✅ Automatically cached data for faster retrieval and saved credits
+#### ✅ Integrated OpenAI for querying data in natural language prompts
+
+
 ## Installation
 
 To install the Quantsight Data API Python client, use `pip`:
 
 ```bash
 pip install quantsight
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

