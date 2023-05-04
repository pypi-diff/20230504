# Comparing `tmp/dictIO-0.2.6.tar.gz` & `tmp/dictIO-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictIO-0.2.6.tar", last modified: Wed Jan 11 11:45:29 2023, max compression
+gzip compressed data, was "dictIO-0.2.7.tar", last modified: Thu May  4 12:12:35 2023, max compression
```

## Comparing `dictIO-0.2.6.tar` & `dictIO-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.780087 dictIO-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-11 11:45:11.000000 dictIO-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-11 11:45:11.000000 dictIO-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-01-11 11:45:29.780087 dictIO-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-01-11 11:45:11.000000 dictIO-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-01-11 11:45:11.000000 dictIO-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-11 11:45:29.780087 dictIO-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.776086 dictIO-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.780087 dictIO-0.2.6/src/dictIO/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.780087 dictIO-0.2.6/src/dictIO/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/cli/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/cppDict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/dictReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/dictWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41900 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    70089 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.780087 dictIO-0.2.6/src/dictIO/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-11 11:45:11.000000 dictIO-0.2.6/src/dictIO/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:45:29.780087 dictIO-0.2.6/src/dictIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-11 11:45:29.000000 dictIO-0.2.6/src/dictIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 12:12:17.000000 dictIO-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 12:12:17.000000 dictIO-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 12:12:35.847202 dictIO-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-04 12:12:17.000000 dictIO-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 12:12:17.000000 dictIO-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-04 12:12:35.851202 dictIO-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.839202 dictIO-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.843202 dictIO-0.2.7/src/dictIO/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/src/dictIO/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cli/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23370 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cppDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69630 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/src/dictIO/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.843202 dictIO-0.2.7/src/dictIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22497 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22074 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55082 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_parser.py
```

### Comparing `dictIO-0.2.6/LICENSE` & `dictIO-0.2.7/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dictIO-0.2.6/PKG-INFO` & `dictIO-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.2.6
+Version: 0.2.7
 Summary: Read, write and manipulate dictionary text files.
 Home-page: https://dnv-opensource.github.io/dictIO/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/dictIO
 Platform: Python3.x
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -120,15 +121,15 @@
     Install dictIO's dependencies:
     ~~~sh
     $ pip install -r requirements-dev.txt
     ~~~
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

### Comparing `dictIO-0.2.6/README.md` & `dictIO-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     Install dictIO's dependencies:
     ~~~sh
     $ pip install -r requirements-dev.txt
     ~~~
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

### Comparing `dictIO-0.2.6/pyproject.toml` & `dictIO-0.2.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -52,126 +52,174 @@
 00000330: 6e67 2073 756d 6d61 7279 2073 686f 756c  ng summary shoul
 00000340: 6420 7374 6172 7420 6174 2074 6865 2066  d start at the f
 00000350: 6972 7374 206c 696e 650d 0a20 2020 2022  irst line..    "
 00000360: 4432 3133 222c 2020 2320 4d75 6c74 692d  D213",  # Multi-
 00000370: 6c69 6e65 2064 6f63 7374 7269 6e67 2073  line docstring s
 00000380: 756d 6d61 7279 2073 686f 756c 6420 7374  ummary should st
 00000390: 6172 7420 6174 2074 6865 2073 6563 6f6e  art at the secon
-000003a0: 6420 6c69 6e65 0d0a 2020 2020 5d0d 0a6c  d line..    ]..l
-000003b0: 696e 652d 6c65 6e67 7468 203d 2031 3230  ine-length = 120
-000003c0: 0d0a 7365 6c65 6374 203d 205b 0d0a 2020  ..select = [..  
-000003d0: 2020 2245 222c 0d0a 2020 2020 2244 222c    "E",..    "D",
-000003e0: 0d0a 2020 2020 2246 222c 0d0a 2020 2020  ..    "F",..    
-000003f0: 224e 222c 0d0a 2020 2020 2257 222c 0d0a  "N",..    "W",..
-00000400: 2020 2020 2249 222c 0d0a 5d0d 0a74 6172      "I",..]..tar
-00000410: 6765 742d 7665 7273 696f 6e20 3d20 2270  get-version = "p
-00000420: 7933 3922 0d0a 0d0a 5b74 6f6f 6c2e 7275  y39"....[tool.ru
-00000430: 6666 2e70 6570 382d 6e61 6d69 6e67 5d0d  ff.pep8-naming].
-00000440: 0a69 676e 6f72 652d 6e61 6d65 7320 3d20  .ignore-names = 
-00000450: 5b0d 0a20 2020 2022 7465 7374 5f2a 222c  [..    "test_*",
-00000460: 0d0a 2020 2020 2273 6574 5570 222c 0d0a  ..    "setUp",..
-00000470: 2020 2020 2274 6561 7244 6f77 6e22 2c0d      "tearDown",.
-00000480: 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666  .]....[tool.ruff
-00000490: 2e70 7964 6f63 7374 796c 655d 0d0a 636f  .pydocstyle]..co
-000004a0: 6e76 656e 7469 6f6e 203d 2022 6e75 6d70  nvention = "nump
-000004b0: 7922 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666  y"....[tool.ruff
-000004c0: 2e70 6572 2d66 696c 652d 6967 6e6f 7265  .per-file-ignore
-000004d0: 735d 0d0a 225f 5f69 6e69 745f 5f2e 7079  s].."__init__.py
-000004e0: 2220 3d20 5b22 4930 3031 225d 0d0a 222e  " = ["I001"]..".
-000004f0: 2f74 6573 7473 2f2a 2220 3d20 5b22 4422  /tests/*" = ["D"
-00000500: 5d0d 0a0d 0a5b 746f 6f6c 2e70 7972 6967  ]....[tool.pyrig
-00000510: 6874 5d0d 0a65 7863 6c75 6465 203d 205b  ht]..exclude = [
-00000520: 0d0a 2020 2020 222e 6769 7422 2c0d 0a20  ..    ".git",.. 
-00000530: 2020 2022 2e76 656e 7622 2c0d 0a20 2020     ".venv",..   
-00000540: 2022 2e74 6f78 222c 0d0a 2020 2020 2262   ".tox",..    "b
-00000550: 7569 6c64 222c 0d0a 2020 2020 2264 6973  uild",..    "dis
-00000560: 7422 2c0d 0a20 2020 2022 2a2a 2f5f 5f70  t",..    "**/__p
-00000570: 7963 6163 6865 5f5f 222c 0d0a 2020 2020  ycache__",..    
-00000580: 222e 2f64 6f63 732f 736f 7572 6365 2f63  "./docs/source/c
-00000590: 6f6e 662e 7079 222c 0d0a 5d0d 0a65 7874  onf.py",..]..ext
-000005a0: 7261 5061 7468 7320 3d20 5b22 2e2f 7372  raPaths = ["./sr
-000005b0: 6322 5d0d 0a74 7970 6543 6865 636b 696e  c"]..typeCheckin
-000005c0: 674d 6f64 6520 3d20 2262 6173 6963 220d  gMode = "basic".
-000005d0: 0a75 7365 4c69 6272 6172 7943 6f64 6546  .useLibraryCodeF
-000005e0: 6f72 5479 7065 7320 3d20 7472 7565 0d0a  orTypes = true..
-000005f0: 7265 706f 7274 4d69 7373 696e 6750 6172  reportMissingPar
-00000600: 616d 6574 6572 5479 7065 203d 2022 6572  ameterType = "er
-00000610: 726f 7222 0d0a 7265 706f 7274 556e 6b6e  ror"..reportUnkn
-00000620: 6f77 6e50 6172 616d 6574 6572 5479 7065  ownParameterType
-00000630: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
-00000640: 706f 7274 556e 6b6e 6f77 6e4d 656d 6265  portUnknownMembe
-00000650: 7254 7970 6520 3d20 2277 6172 6e69 6e67  rType = "warning
-00000660: 220d 0a72 6570 6f72 744d 6973 7369 6e67  "..reportMissing
-00000670: 5479 7065 4172 6775 6d65 6e74 203d 2022  TypeArgument = "
-00000680: 6572 726f 7222 0d0a 7265 706f 7274 5072  error"..reportPr
-00000690: 6f70 6572 7479 5479 7065 4d69 736d 6174  opertyTypeMismat
-000006a0: 6368 203d 2022 6572 726f 7222 0d0a 7265  ch = "error"..re
-000006b0: 706f 7274 4675 6e63 7469 6f6e 4d65 6d62  portFunctionMemb
-000006c0: 6572 4163 6365 7373 203d 2022 7761 726e  erAccess = "warn
-000006d0: 696e 6722 0d0a 7265 706f 7274 5072 6976  ing"..reportPriv
-000006e0: 6174 6555 7361 6765 203d 2022 7761 726e  ateUsage = "warn
-000006f0: 696e 6722 0d0a 7265 706f 7274 5479 7065  ing"..reportType
-00000700: 436f 6d6d 656e 7455 7361 6765 203d 2022  CommentUsage = "
-00000710: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
-00000720: 496e 636f 6d70 6174 6962 6c65 4d65 7468  IncompatibleMeth
-00000730: 6f64 4f76 6572 7269 6465 203d 2022 7761  odOverride = "wa
-00000740: 726e 696e 6722 0d0a 7265 706f 7274 496e  rning"..reportIn
-00000750: 636f 6d70 6174 6962 6c65 5661 7269 6162  compatibleVariab
-00000760: 6c65 4f76 6572 7269 6465 203d 2022 6572  leOverride = "er
-00000770: 726f 7222 0d0a 7265 706f 7274 496e 636f  ror"..reportInco
-00000780: 6e73 6973 7465 6e74 436f 6e73 7472 7563  nsistentConstruc
-00000790: 746f 7220 3d20 2265 7272 6f72 220d 0a72  tor = "error"..r
-000007a0: 6570 6f72 744f 7665 726c 6170 7069 6e67  eportOverlapping
-000007b0: 4f76 6572 6c6f 6164 203d 2022 7761 726e  Overload = "warn
-000007c0: 696e 6722 0d0a 7265 706f 7274 556e 696e  ing"..reportUnin
-000007d0: 6974 6961 6c69 7a65 6449 6e73 7461 6e63  itializedInstanc
-000007e0: 6556 6172 6961 626c 6520 3d20 2277 6172  eVariable = "war
-000007f0: 6e69 6e67 220d 0a72 6570 6f72 7443 616c  ning"..reportCal
-00000800: 6c49 6e44 6566 6175 6c74 496e 6974 6961  lInDefaultInitia
-00000810: 6c69 7a65 7220 3d20 2277 6172 6e69 6e67  lizer = "warning
-00000820: 220d 0a72 6570 6f72 7455 6e6e 6563 6573  "..reportUnneces
-00000830: 7361 7279 4973 496e 7374 616e 6365 203d  saryIsInstance =
-00000840: 2022 696e 666f 726d 6174 696f 6e22 0d0a   "information"..
-00000850: 7265 706f 7274 556e 6e65 6365 7373 6172  reportUnnecessar
-00000860: 7943 6173 7420 3d20 2277 6172 6e69 6e67  yCast = "warning
-00000870: 220d 0a72 6570 6f72 7455 6e6e 6563 6573  "..reportUnneces
-00000880: 7361 7279 436f 6d70 6172 6973 6f6e 203d  saryComparison =
-00000890: 2022 7761 726e 696e 6722 0d0a 7265 706f   "warning"..repo
-000008a0: 7274 556e 6e65 6365 7373 6172 7943 6f6e  rtUnnecessaryCon
-000008b0: 7461 696e 7320 3d20 2277 6172 6e69 6e67  tains = "warning
-000008c0: 220d 0a72 6570 6f72 7455 6e75 7365 6443  "..reportUnusedC
-000008d0: 616c 6c52 6573 756c 7420 3d20 2277 6172  allResult = "war
-000008e0: 6e69 6e67 220d 0a72 6570 6f72 7455 6e75  ning"..reportUnu
-000008f0: 7365 6445 7870 7265 7373 696f 6e20 3d20  sedExpression = 
-00000900: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
-00000910: 744d 6174 6368 4e6f 7445 7868 6175 7374  tMatchNotExhaust
-00000920: 6976 6520 3d20 2277 6172 6e69 6e67 220d  ive = "warning".
-00000930: 0a72 6570 6f72 7453 6861 646f 7765 6449  .reportShadowedI
-00000940: 6d70 6f72 7473 203d 2022 7761 726e 696e  mports = "warnin
-00000950: 6722 0d0a 7265 706f 7274 556e 7479 7065  g"..reportUntype
-00000960: 6446 756e 6374 696f 6e44 6563 6f72 6174  dFunctionDecorat
-00000970: 6f72 203d 2022 7761 726e 696e 6722 0d0a  or = "warning"..
-00000980: 7265 706f 7274 556e 7479 7065 6442 6173  reportUntypedBas
-00000990: 6543 6c61 7373 203d 2022 6572 726f 7222  eClass = "error"
-000009a0: 0d0a 7265 706f 7274 556e 7479 7065 644e  ..reportUntypedN
-000009b0: 616d 6564 5475 706c 6520 3d20 2277 6172  amedTuple = "war
-000009c0: 6e69 6e67 220d 0a23 2041 6374 6976 6174  ning"..# Activat
-000009d0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-000009e0: 7275 6c65 7320 6f6e 6c79 206c 6f63 616c  rules only local
-000009f0: 6c79 2061 6e64 2074 656d 706f 7261 7279  ly and temporary
-00000a00: 2c20 692e 652e 2066 6f72 2061 2051 4120  , i.e. for a QA 
-00000a10: 7365 7373 696f 6e2e 0d0a 2320 2846 6f72  session...# (For
-00000a20: 2073 6572 7665 7220 7369 6465 2043 4920   server side CI 
-00000a30: 7468 6579 2061 7265 2063 6f6e 7369 6465  they are conside
-00000a40: 7265 6420 746f 6f20 7374 7269 6374 2e29  red too strict.)
-00000a50: 0d0a 2320 7265 706f 7274 436f 6e73 7461  ..# reportConsta
-00000a60: 6e74 5265 6465 6669 6e69 7469 6f6e 203d  ntRedefinition =
-00000a70: 2022 7761 726e 696e 6722 0d0a 2320 7265   "warning"..# re
-00000a80: 706f 7274 556e 6e65 6365 7373 6172 7954  portUnnecessaryT
-00000a90: 7970 6549 676e 6f72 6543 6f6d 6d65 6e74  ypeIgnoreComment
-00000aa0: 203d 2022 696e 666f 726d 6174 696f 6e22   = "information"
-00000ab0: 0d0a 2320 7265 706f 7274 496d 706f 7274  ..# reportImport
-00000ac0: 4379 636c 6573 203d 2022 7761 726e 696e  Cycles = "warnin
-00000ad0: 6722 0d0a 2320 7265 706f 7274 496d 706c  g"..# reportImpl
-00000ae0: 6963 6974 5374 7269 6e67 436f 6e63 6174  icitStringConcat
-00000af0: 656e 6174 696f 6e20 3d20 2277 6172 6e69  enation = "warni
-00000b00: 6e67 220d 0a                             ng"..
+000003a0: 6420 6c69 6e65 0d0a 2020 2020 2320 224e  d line..    # "N
+000003b0: 3830 3222 2c20 2023 2046 756e 6374 696f  802",  # Functio
+000003c0: 6e20 6e61 6d65 2073 686f 756c 6420 6265  n name should be
+000003d0: 206c 6f77 6572 6361 7365 2020 2875 6e63   lowercase  (unc
+000003e0: 6f6d 6d65 6e74 2069 6620 796f 7520 7761  omment if you wa
+000003f0: 6e74 2074 6f20 616c 6c6f 7720 5570 7065  nt to allow Uppe
+00000400: 7263 6173 6520 6675 6e63 7469 6f6e 206e  rcase function n
+00000410: 616d 6573 290d 0a20 2020 2023 2022 4e38  ames)..    # "N8
+00000420: 3033 222c 2020 2320 4172 6775 6d65 6e74  03",  # Argument
+00000430: 206e 616d 6520 7368 6f75 6c64 2062 6520   name should be 
+00000440: 6c6f 7765 7263 6173 6520 2028 756e 636f  lowercase  (unco
+00000450: 6d6d 656e 7420 6966 2079 6f75 2077 616e  mment if you wan
+00000460: 7420 746f 2061 6c6c 6f77 2055 7070 6572  t to allow Upper
+00000470: 6361 7365 2061 7267 756d 656e 7420 6e61  case argument na
+00000480: 6d65 7329 0d0a 2020 2020 224e 3830 3622  mes)..    "N806"
+00000490: 2c20 2023 2056 6172 6961 626c 6520 696e  ,  # Variable in
+000004a0: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
+000004b0: 2062 6520 6c6f 7765 7263 6173 6520 2028   be lowercase  (
+000004c0: 756e 636f 6d6d 656e 7420 6966 2079 6f75  uncomment if you
+000004d0: 2077 616e 7420 746f 2061 6c6c 6f77 2055   want to allow U
+000004e0: 7070 6572 6361 7365 2076 6172 6961 626c  ppercase variabl
+000004f0: 6520 6e61 6d65 7320 696e 2066 756e 6374  e names in funct
+00000500: 696f 6e73 290d 0a20 2020 2023 2022 4e38  ions)..    # "N8
+00000510: 3135 222c 2020 2320 5661 7269 6162 6c65  15",  # Variable
+00000520: 2069 6e20 636c 6173 7320 7363 6f70 6520   in class scope 
+00000530: 7368 6f75 6c64 206e 6f74 2062 6520 6d69  should not be mi
+00000540: 7865 6443 6173 6520 2028 756e 636f 6d6d  xedCase  (uncomm
+00000550: 656e 7420 6966 2079 6f75 2077 616e 7420  ent if you want 
+00000560: 746f 2061 6c6c 6f77 206d 6978 6564 4361  to allow mixedCa
+00000570: 7365 2076 6172 6961 626c 6520 6e61 6d65  se variable name
+00000580: 7320 696e 2063 6c61 7373 2073 636f 7065  s in class scope
+00000590: 290d 0a20 2020 2023 2022 4e38 3136 222c  )..    # "N816",
+000005a0: 2020 2320 5661 7269 6162 6c65 2069 6e20    # Variable in 
+000005b0: 676c 6f62 616c 2073 636f 7065 2073 686f  global scope sho
+000005c0: 756c 6420 6e6f 7420 6265 206d 6978 6564  uld not be mixed
+000005d0: 4361 7365 2020 2875 6e63 6f6d 6d65 6e74  Case  (uncomment
+000005e0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+000005f0: 616c 6c6f 7720 6d69 7865 6443 6173 6520  allow mixedCase 
+00000600: 7661 7269 6162 6c65 206e 616d 6573 2069  variable names i
+00000610: 6e20 676c 6f62 616c 2073 636f 7065 290d  n global scope).
+00000620: 0a20 2020 2022 4e39 3939 222c 2020 2320  .    "N999",  # 
+00000630: 496e 7661 6c69 6420 6d6f 6475 6c65 206e  Invalid module n
+00000640: 616d 650d 0a20 2020 205d 0d0a 6c69 6e65  ame..    ]..line
+00000650: 2d6c 656e 6774 6820 3d20 3132 300d 0a73  -length = 120..s
+00000660: 656c 6563 7420 3d20 5b0d 0a20 2020 2022  elect = [..    "
+00000670: 4522 2c0d 0a20 2020 2022 4422 2c0d 0a20  E",..    "D",.. 
+00000680: 2020 2022 4622 2c0d 0a20 2020 2022 4e22     "F",..    "N"
+00000690: 2c0d 0a20 2020 2022 5722 2c0d 0a20 2020  ,..    "W",..   
+000006a0: 2022 4922 2c0d 0a20 2020 2022 4222 2c0d   "I",..    "B",.
+000006b0: 0a5d 0d0a 7461 7267 6574 2d76 6572 7369  .]..target-versi
+000006c0: 6f6e 203d 2022 7079 3339 220d 0a0d 0a5b  on = "py39"....[
+000006d0: 746f 6f6c 2e72 7566 662e 7065 7038 2d6e  tool.ruff.pep8-n
+000006e0: 616d 696e 675d 0d0a 6967 6e6f 7265 2d6e  aming]..ignore-n
+000006f0: 616d 6573 203d 205b 0d0a 2020 2020 2274  ames = [..    "t
+00000700: 6573 745f 2a22 2c0d 0a20 2020 2022 7365  est_*",..    "se
+00000710: 7455 7022 2c0d 0a20 2020 2022 7465 6172  tUp",..    "tear
+00000720: 446f 776e 222c 0d0a 5d0d 0a0d 0a5b 746f  Down",..]....[to
+00000730: 6f6c 2e72 7566 662e 7079 646f 6373 7479  ol.ruff.pydocsty
+00000740: 6c65 5d0d 0a63 6f6e 7665 6e74 696f 6e20  le]..convention 
+00000750: 3d20 226e 756d 7079 220d 0a0d 0a5b 746f  = "numpy"....[to
+00000760: 6f6c 2e72 7566 662e 7065 722d 6669 6c65  ol.ruff.per-file
+00000770: 2d69 676e 6f72 6573 5d0d 0a22 5f5f 696e  -ignores].."__in
+00000780: 6974 5f5f 2e70 7922 203d 205b 2249 3030  it__.py" = ["I00
+00000790: 3122 5d0d 0a22 2e2f 7465 7374 732f 2a22  1"].."./tests/*"
+000007a0: 203d 205b 2244 225d 0d0a 0d0a 5b74 6f6f   = ["D"]....[too
+000007b0: 6c2e 7079 7269 6768 745d 0d0a 6578 636c  l.pyright]..excl
+000007c0: 7564 6520 3d20 5b0d 0a20 2020 2022 2e67  ude = [..    ".g
+000007d0: 6974 222c 0d0a 2020 2020 222e 7665 6e76  it",..    ".venv
+000007e0: 222c 0d0a 2020 2020 222e 746f 7822 2c0d  ",..    ".tox",.
+000007f0: 0a20 2020 2022 6275 696c 6422 2c0d 0a20  .    "build",.. 
+00000800: 2020 2022 6469 7374 222c 0d0a 2020 2020     "dist",..    
+00000810: 222a 2a2f 5f5f 7079 6361 6368 655f 5f22  "**/__pycache__"
+00000820: 2c0d 0a20 2020 2022 2e2f 646f 6373 2f73  ,..    "./docs/s
+00000830: 6f75 7263 652f 636f 6e66 2e70 7922 2c0d  ource/conf.py",.
+00000840: 0a5d 0d0a 6578 7472 6150 6174 6873 203d  .]..extraPaths =
+00000850: 205b 222e 2f73 7263 225d 0d0a 7479 7065   ["./src"]..type
+00000860: 4368 6563 6b69 6e67 4d6f 6465 203d 2022  CheckingMode = "
+00000870: 6261 7369 6322 0d0a 7573 654c 6962 7261  basic"..useLibra
+00000880: 7279 436f 6465 466f 7254 7970 6573 203d  ryCodeForTypes =
+00000890: 2074 7275 650d 0a72 6570 6f72 744d 6973   true..reportMis
+000008a0: 7369 6e67 5061 7261 6d65 7465 7254 7970  singParameterTyp
+000008b0: 6520 3d20 2265 7272 6f72 220d 0a72 6570  e = "error"..rep
+000008c0: 6f72 7455 6e6b 6e6f 776e 5061 7261 6d65  ortUnknownParame
+000008d0: 7465 7254 7970 6520 3d20 2277 6172 6e69  terType = "warni
+000008e0: 6e67 220d 0a72 6570 6f72 7455 6e6b 6e6f  ng"..reportUnkno
+000008f0: 776e 4d65 6d62 6572 5479 7065 203d 2022  wnMemberType = "
+00000900: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000910: 4d69 7373 696e 6754 7970 6541 7267 756d  MissingTypeArgum
+00000920: 656e 7420 3d20 2265 7272 6f72 220d 0a72  ent = "error"..r
+00000930: 6570 6f72 7450 726f 7065 7274 7954 7970  eportPropertyTyp
+00000940: 654d 6973 6d61 7463 6820 3d20 2265 7272  eMismatch = "err
+00000950: 6f72 220d 0a72 6570 6f72 7446 756e 6374  or"..reportFunct
+00000960: 696f 6e4d 656d 6265 7241 6363 6573 7320  ionMemberAccess 
+00000970: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00000980: 6f72 7450 7269 7661 7465 5573 6167 6520  ortPrivateUsage 
+00000990: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+000009a0: 6f72 7454 7970 6543 6f6d 6d65 6e74 5573  ortTypeCommentUs
+000009b0: 6167 6520 3d20 2277 6172 6e69 6e67 220d  age = "warning".
+000009c0: 0a72 6570 6f72 7449 6e63 6f6d 7061 7469  .reportIncompati
+000009d0: 626c 654d 6574 686f 644f 7665 7272 6964  bleMethodOverrid
+000009e0: 6520 3d20 2277 6172 6e69 6e67 220d 0a72  e = "warning"..r
+000009f0: 6570 6f72 7449 6e63 6f6d 7061 7469 626c  eportIncompatibl
+00000a00: 6556 6172 6961 626c 654f 7665 7272 6964  eVariableOverrid
+00000a10: 6520 3d20 2265 7272 6f72 220d 0a72 6570  e = "error"..rep
+00000a20: 6f72 7449 6e63 6f6e 7369 7374 656e 7443  ortInconsistentC
+00000a30: 6f6e 7374 7275 6374 6f72 203d 2022 6572  onstructor = "er
+00000a40: 726f 7222 0d0a 7265 706f 7274 4f76 6572  ror"..reportOver
+00000a50: 6c61 7070 696e 674f 7665 726c 6f61 6420  lappingOverload 
+00000a60: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00000a70: 6f72 7455 6e69 6e69 7469 616c 697a 6564  ortUninitialized
+00000a80: 496e 7374 616e 6365 5661 7269 6162 6c65  InstanceVariable
+00000a90: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
+00000aa0: 706f 7274 4361 6c6c 496e 4465 6661 756c  portCallInDefaul
+00000ab0: 7449 6e69 7469 616c 697a 6572 203d 2022  tInitializer = "
+00000ac0: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000ad0: 556e 6e65 6365 7373 6172 7949 7349 6e73  UnnecessaryIsIns
+00000ae0: 7461 6e63 6520 3d20 2269 6e66 6f72 6d61  tance = "informa
+00000af0: 7469 6f6e 220d 0a72 6570 6f72 7455 6e6e  tion"..reportUnn
+00000b00: 6563 6573 7361 7279 4361 7374 203d 2022  ecessaryCast = "
+00000b10: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000b20: 556e 6e65 6365 7373 6172 7943 6f6d 7061  UnnecessaryCompa
+00000b30: 7269 736f 6e20 3d20 2277 6172 6e69 6e67  rison = "warning
+00000b40: 220d 0a72 6570 6f72 7455 6e6e 6563 6573  "..reportUnneces
+00000b50: 7361 7279 436f 6e74 6169 6e73 203d 2022  saryContains = "
+00000b60: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000b70: 556e 7573 6564 4361 6c6c 5265 7375 6c74  UnusedCallResult
+00000b80: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
+00000b90: 706f 7274 556e 7573 6564 4578 7072 6573  portUnusedExpres
+00000ba0: 7369 6f6e 203d 2022 7761 726e 696e 6722  sion = "warning"
+00000bb0: 0d0a 7265 706f 7274 4d61 7463 684e 6f74  ..reportMatchNot
+00000bc0: 4578 6861 7573 7469 7665 203d 2022 7761  Exhaustive = "wa
+00000bd0: 726e 696e 6722 0d0a 7265 706f 7274 5368  rning"..reportSh
+00000be0: 6164 6f77 6564 496d 706f 7274 7320 3d20  adowedImports = 
+00000bf0: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
+00000c00: 7455 6e74 7970 6564 4675 6e63 7469 6f6e  tUntypedFunction
+00000c10: 4465 636f 7261 746f 7220 3d20 2277 6172  Decorator = "war
+00000c20: 6e69 6e67 220d 0a72 6570 6f72 7455 6e74  ning"..reportUnt
+00000c30: 7970 6564 4261 7365 436c 6173 7320 3d20  ypedBaseClass = 
+00000c40: 2265 7272 6f72 220d 0a72 6570 6f72 7455  "error"..reportU
+00000c50: 6e74 7970 6564 4e61 6d65 6454 7570 6c65  ntypedNamedTuple
+00000c60: 203d 2022 7761 726e 696e 6722 0d0a 2320   = "warning"..# 
+00000c70: 4163 7469 7661 7465 2074 6865 2066 6f6c  Activate the fol
+00000c80: 6c6f 7769 6e67 2072 756c 6573 206f 6e6c  lowing rules onl
+00000c90: 7920 6c6f 6361 6c6c 7920 616e 6420 7465  y locally and te
+00000ca0: 6d70 6f72 6172 792c 2069 2e65 2e20 666f  mporary, i.e. fo
+00000cb0: 7220 6120 5141 2073 6573 7369 6f6e 2e0d  r a QA session..
+00000cc0: 0a23 2028 466f 7220 7365 7276 6572 2073  .# (For server s
+00000cd0: 6964 6520 4349 2074 6865 7920 6172 6520  ide CI they are 
+00000ce0: 636f 6e73 6964 6572 6564 2074 6f6f 2073  considered too s
+00000cf0: 7472 6963 742e 290d 0a23 2072 6570 6f72  trict.)..# repor
+00000d00: 7443 6f6e 7374 616e 7452 6564 6566 696e  tConstantRedefin
+00000d10: 6974 696f 6e20 3d20 2277 6172 6e69 6e67  ition = "warning
+00000d20: 220d 0a23 2072 6570 6f72 7455 6e6e 6563  "..# reportUnnec
+00000d30: 6573 7361 7279 5479 7065 4967 6e6f 7265  essaryTypeIgnore
+00000d40: 436f 6d6d 656e 7420 3d20 2269 6e66 6f72  Comment = "infor
+00000d50: 6d61 7469 6f6e 220d 0a23 2072 6570 6f72  mation"..# repor
+00000d60: 7449 6d70 6f72 7443 7963 6c65 7320 3d20  tImportCycles = 
+00000d70: 2277 6172 6e69 6e67 220d 0a23 2072 6570  "warning"..# rep
+00000d80: 6f72 7449 6d70 6c69 6369 7453 7472 696e  ortImplicitStrin
+00000d90: 6743 6f6e 6361 7465 6e61 7469 6f6e 203d  gConcatenation =
+00000da0: 2022 7761 726e 696e 6722 0d0a 0d0a 5b74   "warning"....[t
+00000db0: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
+00000dc0: 7074 696f 6e73 5d0d 0a74 6573 7470 6174  ptions]..testpat
+00000dd0: 6873 203d 2022 7465 7374 7322 0d0a 6164  hs = "tests"..ad
+00000de0: 646f 7074 7320 3d20 222d 2d73 7472 6963  dopts = "--stric
+00000df0: 742d 6d61 726b 6572 7322 0d0a 7866 6169  t-markers"..xfai
+00000e00: 6c5f 7374 7269 6374 203d 2074 7275 65    l_strict = true
```

### Comparing `dictIO-0.2.6/setup.cfg` & `dictIO-0.2.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = dictIO
-version = 0.2.6
+version = 0.2.7
 summary = Read, write and manipulate dictionary text files.
 description = Python package to read, write and manipulate dictionary text files. Supports dictIOs dict file format, as well as JSON, XML and OpenFOAM.
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://dnv-opensource.github.io/dictIO/README.html
 project_urls = 
 	GitHub = https://github.com/dnv-opensource/dictIO
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
@@ -34,14 +35,15 @@
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	lxml>=4.9
+	lxml-stubs>=0.4.0
 	jsonschema>=4.17
 	numpy>=1.23
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
@@ -67,19 +69,19 @@
 [coverage:paths]
 source = 
 	src/dictIO
 	*/site-packages/dictIO
 
 [tox:tox]
 isolated_build = True
-envlist = py{39,310,311}-{linux,macos,windows}
+envlist = py{39,310,311,312}-{linux,macos,windows}
 
 [testenv]
 deps = 
-	pytest>=7.2
+	pytest>=7.3
 	pytest-cov>=4.0
 	pytest-randomly>=3.12
 commands = 
 	pytest --cov --cov-config setup.cfg {posargs}
 
 [egg_info]
 tag_build =
```

### Comparing `dictIO-0.2.6/src/dictIO/__init__.py` & `dictIO-0.2.7/src/dictIO/__init__.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.6/src/dictIO/cli/dictParser.py` & `dictIO-0.2.7/src/dictIO/cli/dictParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from dictIO import DictParser
 from dictIO.utils.logging import configure_logging
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = argparse.ArgumentParser(
         prog="dictParser",
         usage="%(prog)s dict [options [args]]",
         epilog="_________________dictParser___________________",
         prefix_chars="-",
         add_help=True,
         description=(
```

### Comparing `dictIO-0.2.6/src/dictIO/cppDict.py` & `dictIO-0.2.7/src/dictIO/cppDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             "}",
             "]",
             ")",
         ]
         return
 
     def include(self, dict_to_include: "CppDict"):
-        """Adds an include directive for the passed in dict.
+        """Add an include directive for the passed in dict.
 
         Parameters
         ----------
         dict_to_include : CppDict
             The dict to be included via an include directive
 
         Raises
@@ -152,15 +152,15 @@
             else:
                 break
         self.data[placeholder] = placeholder
         self.includes.update({ii: (include_directive, include_file_name, include_file_path)})
         return
 
     def update(self, __m: Mapping[Any, Any], **kwargs: Any) -> None:
-        """Updates top-level keys with the keys from the passed in dict.
+        """Update top-level keys with the keys from the passed in dict.
 
         Overrides the update() method of UserDict base class in order to include also CppDict class attributes in the update.
 
         If a key already exists, it will be substituted by the key from the passed in dict.
         In order to not substitute top-level keys but recursively merge (potentially nested) content from passed in dict into the existing, use merge() instead.
 
         Note:
@@ -186,15 +186,15 @@
             self.expressions.update(__m.expressions)
             self.includes.update(__m.includes)
         self._clean()
 
         return
 
     def merge(self, dict: MutableMapping[Any, Any]):
-        """Merges the passed in dict into the existing CppDict instance.
+        """Merge the passed in dict into the existing CppDict instance.
 
         In contrast to update(), merge() works recursively. That is, it does not simply substitute top-level keys but
         recursively merges (potentially nested) content from the passed in dict into the existing.
         This prevents nested keys from being deleted.
         Further, existing keys will NOT be overwritten.
 
         Parameters
@@ -216,21 +216,21 @@
             _merge_dicts(self.expressions, dict.expressions)
             _merge_dicts(self.includes, dict.includes)
         self._clean()
 
         return
 
     def __str__(self):
-        """string representation of the CppDict instance in dictIO dict file format.
+        """String representation of the CppDict instance in dictIO dict file format.
 
         Returns
         -------
         str
             the string representation
-        """
+        """  # noqa: D401
         from dictIO import (
             CppFormatter,  # __str__ shall be formatted in default dict file format
         )
 
         formatter = CppFormatter()
         return formatter.to_string(self)
 
@@ -247,15 +247,15 @@
         self.block_comments = order_keys(self.block_comments)
         self.expressions = order_keys(self.expressions)
         self.includes = order_keys(self.includes)
 
         return
 
     def find_global_key(self, query: str = "") -> Union[List[Any], None]:
-        """Returns the global key thread to the first key the value of which matches the passed in query.
+        """Return the global key thread to the first key the value of which matches the passed in query.
 
         Function works recursively on nested dicts and is non-greedy: The key of the first match is returned.
         Return value is a sequence of keys: The 'global key thread'.
         It represents the sequence of keys that one needs to traverse downwards
         in order to arrive at the target key found.
 
         Parameters
@@ -267,15 +267,15 @@
         -------
         Union[List[Any], None]
             global key thread to the first key the value of which matches the passed in query, if found. Otherwise None.
         """
         return find_global_key(self.data, query)
 
     def set_global_key(self, global_key: MutableSequence[Any], value: Any = None):
-        """Sets the value for the passed in global key.
+        """Set the value for the passed in global key.
 
         The global key thread is traversed downwards until arrival at the target key,
         the value of which is then set.
 
         Parameters
         ----------
         global_key : MutableSequence[Any]
@@ -284,15 +284,15 @@
             value the target key shall be set to, by default None
         """
         set_global_key(self.data, global_key, value)
 
         return
 
     def global_key_exists(self, global_key: MutableSequence[Any]) -> bool:
-        """Checks whether the specified global key exists.
+        """Check whether the specified global key exists.
 
         Parameters
         ----------
         global_key : MutableSequence[Any]
             global key the existence of which is checked
 
         Returns
@@ -376,16 +376,17 @@
 
         variables = order_keys(variables)
 
         return variables
 
     def _clean(self, dict: Union[MutableMapping[Any, Any], None] = None):
         # sourcery skip: avoid-builtin-shadow
-        """
-        Finds and removes doublettes of following PLACEHOLDER keys within self.data
+        """Find and remove doublettes of PLACEHOLDER keys.
+
+        Find and remove doublettes of following PLACEHOLDER keys within self.data:
         - BLOCKCOMMENT
         - INCLUDE
         - LINECOMMENT
         By definition, only keys on the same nest level are checked for doublettes.
         Doublettes are identified through equality with their lookup values.
         """
         # START at nest level 0
@@ -475,15 +476,15 @@
     return sorted_dict
 
 
 def find_global_key(
     arg: Union[MutableMapping[Any, Any], MutableSequence[Any]],
     query: str = "",
 ) -> Union[List[Any], None]:
-    """Returns the global key thread to the first key the value of which matches the passed in query.
+    """Return the global key thread to the first key the value of which matches the passed in query.
 
     Parameters
     ----------
     arg : Union[MutableMapping[Any, Any], MutableSequence[Any]]
         dict to search in for the queried value
     query : str, optional
         query string for the value to search for, by default ''
@@ -519,15 +520,15 @@
 
 
 def set_global_key(
     arg: MutableMapping[Any, Any],
     global_key: MutableSequence[Any],
     value: Any = None,
 ):
-    """Sets the value for the passed in global key.
+    """Set the value for the passed in global key.
 
     Parameters
     ----------
     arg : MutableMapping[Any, Any]
         dict the target key in which shall be set
     global_key : MutableSequence[Any], optional
         list of keys defining the global key thread to the target key (such as returned by method find_global_key())
@@ -548,15 +549,15 @@
                 break
         last_branch[remaining_keys[0]] = value
 
     return
 
 
 def global_key_exists(arg: MutableMapping[Any, Any], global_key: MutableSequence[Any]) -> bool:
-    """Checks whether the specified global key exists in the passed in dict.
+    """Check whether the specified global key exists in the passed in dict.
 
     Parameters
     ----------
     arg : MutableMapping[Any, Any]
         dict to check for existence of the specified global key
     global_key : MutableSequence[Any], optional
         global key the existence of which is checked in the passed in dict
@@ -577,15 +578,15 @@
 
 
 def _merge_dicts(
     target_dict: MutableMapping[Any, Any],
     dict_to_merge: MutableMapping[Any, Any],
     overwrite: bool = False,
 ):
-    """Merges dict_to_merge into target_dict.
+    """Merge dict_to_merge into target_dict.
 
     In contrast to dict.update(), _merge_dicts() works recursively. That is, it does not simply substitute top-level keys
     in target_dict but recursively merges (potentially nested) content from dict_to_merge into target_dict.
     This prevents nested keys from being deleted.
 
     Parameters
     ----------
```

### Comparing `dictIO-0.2.6/src/dictIO/dictParser.py` & `dictIO-0.2.7/src/dictIO/dictParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         includes: bool = True,
         mode: str = "w",
         order: bool = False,
         comments: bool = True,
         scope: Union[MutableSequence[str], None] = None,
         output: Union[str, None] = None,
     ) -> Union[CppDict, None]:
-        """Parses a dictionary file and saves it with prefix 'parsed.'.
+        """Parse a dictionary file and save it with prefix 'parsed.'.
 
         DictParser.parse() combines the otherwise atomic operations
         of DictReader.read() and DictWriter.write() in one chunk:
 
         1: parsed_dict = DictReader.read(source_file)
 
         2: DictWriter.write(parsed_dict, target_file)
```

### Comparing `dictIO-0.2.6/src/dictIO/dictReader.py` & `dictIO-0.2.7/src/dictIO/dictReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         source_file: Union[str, os.PathLike[str]],
         includes: bool = True,
         order: bool = False,
         comments: bool = True,
         scope: Union[MutableSequence[str], None] = None,
         parser: Union[Parser, None] = None,
     ) -> CppDict:
-        """Reads a dictionary file in dictIO dict file format, as well as JSON and XML.
+        """Read a dictionary file in dictIO dict file format, as well as JSON and XML.
 
         Reads a dict file, parses it and transforms its content into a dictIO dict object (CppDict).
         Following file formats are supported and interpreted through source_file's file ending:
         no file ending   ->   dictIO dict file
         '.cpp'           ->   dictIO dict file
         '.foam'          ->   Foam dictionary file
         '.json'          ->   Json dictionary file
@@ -131,22 +131,21 @@
         if not includes:
             __class__._remove_include_keys(parsed_dict.data)
 
         return parsed_dict
 
     @staticmethod
     def _merge_includes(dict: CppDict, comments: bool = True):
-        """Parses and merges any (child) dicts that are referenced in the dict file through #include directives."""
+        """Parse and merge any (child) dicts that are referenced in the dict file through #include directives."""
         # Create dejavue string watchdog
         djv = DejaVue()
         djv.reset()
 
         # Inner function: Merge all includes, recursively
         def _merge_includes_recursive(dict: CppDict):
-
             # empty dict to merge in temporarily, avoiding dict-has-change-error inside the for loop
             temp_dict = CppDict()
 
             # loop over all possible includes
             for _, _, path in dict.includes.values():
                 prove_recursive_include = djv(path.name)
 
@@ -175,15 +174,15 @@
 
         # Call inner funtion to merge all includes, recursively
         dict.merge(_merge_includes_recursive(dict))
 
         return
 
     @staticmethod
-    def _resolve_reference(ref: Any, vars: MutableMapping[Any, Any]):
+    def _resolve_reference(ref: Any, vars: MutableMapping[Any, Any]) -> Union[Any, None]:
         # resolves a single reference
         ret: Union[Any, None] = None
         try:
             # extract indices, ugly version, nice version is re.sub with a positive lookahead
             indexing = re.findall(r"\[.+\]$", ref)[0]
         except Exception:
             indexing = ""
```

### Comparing `dictIO-0.2.6/src/dictIO/dictWriter.py` & `dictIO-0.2.7/src/dictIO/dictWriter.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def write(
         source_dict: Union[MutableMapping[Any, Any], CppDict],
         target_file: Union[str, os.PathLike[str], None] = None,
         mode: str = "a",
         order: bool = False,
         formatter: Union[Formatter, None] = None,
     ):
-        """Writes a dictionary file in dictIO dict file format, as well as JSON, XML and OpenFoam.
+        """Write a dictionary file in dictIO dict file format, as well as JSON, XML and OpenFoam.
 
         Writes a dictIO dict (parameter source_dict of type CppDict) to target_file.
         Following file formats are supported and interpreted through target_file's file ending:
         no file ending   ->   dictIO dict file
         '.cpp'           ->   dictIO dict file
         '.foam'          ->   Foam dictionary file
         '.json'          ->   Json dictionary file
@@ -48,18 +48,15 @@
             append to target file ('a') or overwrite target file ('w'), by default 'a'
         order : bool, optional
             if True, the dict will be sorted before writing, by default False
         formatter : Union[Formatter, None], optional
             formatter to be used, by default None
         """
 
-        # Check argument
-        if source_dict is None:
-            logger.warning("dictWriter.write(): argument 'source_dict' is missing. No file written.")
-            return
+        # Check arguments
         if mode not in ["a", "w"]:
             logger.warning(
                 f"dictWriter.write(): argument 'mode' has invalid value '{mode}'. Used default mode 'w' instead as fallback."
             )
 
         # Determine target file name
         if target_file is None:
@@ -130,15 +127,15 @@
     format : Union[str, None], optional
         format of the target dict file. Choices are 'cpp', 'foam', 'xml' and 'json', by default None
 
     Returns
     -------
     Path
         target dict file name
-    """
+    """  # noqa: D401
 
     # Make sure source_file argument is of type Path. If not, cast it to Path type.
     source_file = source_file if isinstance(source_file, Path) else Path(source_file)
 
     # Split source_file into file name and file ending, if existing
     file_name = source_file.stem
     file_ending = source_file.suffix
```

### Comparing `dictIO-0.2.6/src/dictIO/formatter.py` & `dictIO-0.2.7/src/dictIO/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
 
     def __init__(self):
         self.counter = BorgCounter()
 
     @classmethod
     def get_formatter(cls, target_file: Union[Path, None] = None):
-        """Factory method returning a Formatter instance matching the target file type to be formatted.
+        """Return a Formatter instance matching the type of the target file to be formatted (factory method).
 
         Parameters
         ----------
         target_file : Path, optional
             name of the target file to be formatted, by default None
 
         Returns
@@ -67,15 +67,15 @@
         # 2. If no target file is passed, return CppFormatter as default / fallback
         return CppFormatter()  # default
 
     def to_string(
         self,
         dict: Union[MutableMapping[Any, Any], CppDict],
     ) -> str:
-        """Creates a string representation of the passed in dict.
+        """Create a string representation of the passed in dict.
 
         Note: Override this method when implementing a specific Formatter.
 
         Parameters
         ----------
         dict : Union[MutableMapping[Any, Any], CppDict]
             dict to be formatted
@@ -84,15 +84,15 @@
         -------
         str
             string representation of the dict
         """
         return ""
 
     def format_dict(self, arg: Union[MutableMapping[Any, Any], MutableSequence[Any], Any]) -> str:
-        """Formats a dict or list object.
+        """Format a dict or list object.
 
         Note: Override this method when implementing a specific Formatter.
 
         Parameters
         ----------
         arg : Union[MutableMapping[Any, Any], MutableSequence[Any], Any]
             the dict or list to be formatted
@@ -101,15 +101,15 @@
         -------
         str
             the formatted string representation of the passed in dict or list
         """
         return ""
 
     def format_type(self, arg: Any) -> str:
-        """Formats a single value type (str, int, float, boolean or None).
+        """Format a single value type (str, int, float, boolean or None).
 
         Parameters
         ----------
         arg : Any
             the value to be formatted
 
         Returns
@@ -131,15 +131,15 @@
             else:
                 return str(arg)
 
         # String type:
         return self.format_string(arg)
 
     def format_bool(self, arg: bool) -> str:
-        """Formats a boolean.
+        """Format a boolean.
 
         Note: Override this method for specific formatting of booleans when implementing a Formatter.
 
         Parameters
         ----------
         arg : bool
             the boolean value to be formatted
@@ -148,15 +148,15 @@
         -------
         str
             the formatted string representation of the passed in boolean value
         """
         return str(arg)
 
     def format_int(self, arg: int) -> str:
-        """Formats an integer.
+        """Format an integer.
 
         Note: Override this method for specific formatting of integers when implementing a Formatter.
 
         Parameters
         ----------
         arg : int
             the int to be formatted
@@ -165,15 +165,15 @@
         -------
         str
             the formatted string representation of the passed in int
         """
         return str(arg)
 
     def format_float(self, arg: float) -> str:
-        """Formats a floating point number.
+        """Format a floating point number.
 
         Note: Override this method for specific formatting of floating point numbers when implementing a Formatter.
 
         Parameters
         ----------
         arg : float
             the float to be formatted
@@ -182,27 +182,27 @@
         -------
         str
             the formatted string representation of the passed in float
         """
         return str(arg)
 
     def format_none(self) -> str:
-        """Formats None.
+        """Format None value.
 
         Note: Override this method for specific formatting of None when implementing a Formatter.
 
         Returns
         -------
         str
             the formatted string representation of None
         """
         return str(None)
 
     def format_string(self, arg: str) -> str:
-        """Formats a string.
+        """Format a string.
 
         Parameters
         ----------
         arg : str
             the string to be formatted
 
         Returns
@@ -219,15 +219,15 @@
             return self.format_empty_string(arg)
         elif re.search(r"[\s:/\\]", arg):  # contains spaces or path -> complex string
             return self.format_multi_word_string(arg)
         else:  # single word string
             return self.format_single_word_string(arg)
 
     def format_empty_string(self, arg: str) -> str:
-        """Formats an empty string.
+        """Format an empty string.
 
         Note: Override this method for specific formatting of empty strings when implementing a Formatter.
 
         Parameters
         ----------
         arg : str
             the empty string to be formatted
@@ -236,15 +236,15 @@
         -------
         str
             the formatted empty string
         """
         return arg
 
     def format_single_word_string(self, arg: str) -> str:
-        """Formats a single word string.
+        """Format a single word string.
 
         Note: Override this method for specific formatting of single word strings when implementing a Formatter.
 
         Parameters
         ----------
         arg : str
             the single word string to be formatted
@@ -253,15 +253,15 @@
         -------
         str
             the formatted single word string
         """
         return arg
 
     def format_multi_word_string(self, arg: str) -> str:
-        """Formats a multi word string.
+        """Format a multi word string.
 
         Note: Override this method for specific formatting of multi word strings when implementing a Formatter.
 
         Parameters
         ----------
         arg : str
             the multi word string to be formatted
@@ -270,15 +270,15 @@
         -------
         str
             the formatted multi word string
         """
         return arg
 
     def format_reference_string(self, arg: str) -> str:
-        """Formats a reference.
+        """Format a reference.
 
         Note: Override this method for specific formatting of references when implementing a Formatter.
 
         Parameters
         ----------
         arg : str
             the reference to be formatted
@@ -287,15 +287,15 @@
         -------
         str
             the formatted reference
         """
         return arg
 
     def format_expression_string(self, arg: str) -> str:
-        """Formats an expression.
+        """Format an expression.
 
         Note: Override this method for specific formatting of expressions when implementing a Formatter.
 
         Parameters
         ----------
         arg : str
             the expression to be formatted
@@ -304,15 +304,15 @@
         -------
         str
             the formatted expression
         """
         return arg
 
     def add_single_quotes(self, arg: str) -> str:
-        """Adds single quotes to a string.
+        """Add single quotes to a string.
 
         Leading and trailing single quotes will added to the passed in string
         (i.e. it will be wrapped in single quotes).
         Note: Call this base class method from any specific Formatter implementation
         to easily add single quotes to a string when formatting.
 
         Parameters
@@ -324,15 +324,15 @@
         -------
         str
             the string wrapped in single quotes
         """
         return f"'{arg}'"
 
     def add_double_quotes(self, arg: str) -> str:
-        """Adds double quotes to a string.
+        """Add double quotes to a string.
 
         Leading and trailing double quotes will added to the passed in string
         (i.e. it will be wrapped in double quotes).
         Note: Call this base class method from any specific Formatter implementation
         to easily add double quotes to a string when formatting.
 
         Parameters
@@ -348,23 +348,23 @@
         return f'"{arg}"'
 
 
 class CppFormatter(Formatter):
     """Formatter to serialize a dict into a string in dictIO dict file format."""
 
     def __init__(self):
-        """Implementation specific default configuration of CppFormatter."""
+        """Implementation specific default configuration of CppFormatter."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def to_string(
         self,
         dict: Union[MutableMapping[Any, Any], CppDict],
     ) -> str:  # sourcery skip: avoid-builtin-shadow, dict-comprehension
-        """Creates a string representation of the passed in dict in dictIO dict file format.
+        """Create a string representation of the passed in dict in dictIO dict file format.
 
         Parameters
         ----------
         dict : Union[MutableMapping[Any, Any], CppDict]
             dict to be formatted
 
         Returns
@@ -436,31 +436,29 @@
         tab_len: int = 4,
         level: int = 0,
         sep: str = " ",
         items_per_line: int = 10,
         end: str = "\n",
         ancestry: Union[Type[MutableMapping[Any, Any]], Type[MutableSequence[Any]]] = MutableMapping,
     ) -> str:
-        """Formats a dict or list object."""
+        """Format a dict or list object."""
         total_indent = 30
         s = str()
         indent = sep * tab_len * level
 
         # list
         if isinstance(arg, MutableSequence):
-
             # Opening bracket
             s += self.format_dict("(", level=level, end=end)
 
             # List items
             first_item_on_this_line = True
             last_item_on_this_line = False
 
             for index, item in enumerate(arg):
-
                 # ndarray -> list
                 if isinstance(item, ndarray):
                     item = item.tolist()
 
                 # nested list
                 if isinstance(item, MutableSequence):
                     # (recursion)
@@ -523,15 +521,14 @@
                 s += self.format_dict(")", level=level, end=end)
             else:
                 s += self.format_dict(");", level=level, end=end)
 
         # dict
         elif isinstance(arg, MutableMapping):
             for key in arg.keys():
-
                 # ndarray -> list
                 if isinstance(arg[key], ndarray):
                     arg[key] = arg[key].tolist()
 
                 # nested dict
                 if isinstance(arg[key], dict):
                     s += self.format_dict(key, level=level)
@@ -567,95 +564,94 @@
         else:
             string = f"{indent}{arg}{end}"
             s += string
 
         return s
 
     def format_bool(self, arg: bool) -> str:
-        """Formats a boolean.
+        """Format a boolean.
 
         Parameters
         ----------
         arg : bool
             the boolean value to be formatted
 
         Returns
         -------
         str
             the formatted string representation of the passed in boolean value
         """
         return str(arg).lower()
 
     def format_none(self) -> str:
-        """Formats None.
+        """Format None.
 
         Returns
         -------
         str
             the formatted string representation of None
         """
         return "NULL"
 
     def format_empty_string(self, arg: str) -> str:
-        """Formats an empty string.
+        """Format an empty string.
 
         Parameters
         ----------
         arg : str
             the empty string to be formatted
 
         Returns
         -------
         str
             the formatted empty string
         """
         return self.add_single_quotes(arg)
 
     def format_multi_word_string(self, arg: str) -> str:
-        """Formats a multi word string.
+        """Format a multi word string.
 
         Parameters
         ----------
         arg : str
             the multi word string to be formatted
 
         Returns
         -------
         str
             the formatted multi word string
         """
         return self.add_single_quotes(arg)
 
     def format_expression_string(self, arg: str) -> str:
-        """Formats an expression.
+        """Format an expression.
 
         Parameters
         ----------
         arg : str
             the expression to be formatted
 
         Returns
         -------
         str
             the formatted expression
         """
         return self.add_double_quotes(arg)
 
     def insert_block_comments(self, dict: CppDict, s: str) -> str:
-        """Inserts back all block comments.
+        """Insert back all block comments.
 
         Replaces all BLOCKCOMMENT placeholders in s with the actual block_comments saved in dict
         str s is expected to contain the CppDict's block_content containing block comment placeholders to substitute (BLOCKCOMMENT... BLOCKCOMMENT...)
         """
 
         # Replace all BLOCKCOMMENT placeholders in s with the actual block_comments saved in dict
         block_comments_inserted_so_far = ""
         first_block_comment = True  # MonoFlop, armed
         for key, block_comment in dict.block_comments.items():
-
             # If this is the first block_comment, make sure it contains the default block comment
             if first_block_comment:
                 # if not re.search(r'\s[Cc]\+{2}\s', block_comment):
                 #     # block_comment = default_block_comment + str(dict.block_comments[key])
                 #     block_comment = default_block_comment + block_comment
                 block_comment = self.make_default_block_comment(block_comment)
                 first_block_comment = False  # disarm MonoFlop
@@ -680,53 +676,53 @@
         # If no block_comment had been inserted, insert the default block comment
         if block_comments_inserted_so_far == "":
             s = self.make_default_block_comment() + s
 
         return s
 
     def make_default_block_comment(self, block_comment: str = "") -> str:
-        """Creates the default block comment (header) for files in dictIO dict file format."""
+        """Create the default block comment (header) for files in dictIO dict file format."""
         # If there is no ' C++ ' contained in block_comment,
         # then insert the C++ default block comment in front:
         # sourcery skip: move-assign
         default_block_comment = (
             "/*---------------------------------*- C++ -*----------------------------------*\\\n"
             "filetype dictionary; coding utf-8; version 0.1; local --; purpose --;\n"
             "\\*----------------------------------------------------------------------------*/\n"
         )
         if not re.search(r"\s[Cc]\+{2}\s", block_comment):
             # block_comment = default_block_comment + str(dict.block_comments[key])
             block_comment = default_block_comment + block_comment
         return block_comment
 
     def insert_includes(self, cpp_dict: CppDict, s: str) -> str:
-        """Inserts back all include directives."""
+        """Insert back all include directives."""
         for key, (include_directive, include_file_name, _) in cpp_dict.includes.items():
             # Search for the placeholder entry we created in _parse_tokenized_dict(),
             # and insert back the original include directive.
             include_file_name = include_file_name.replace("\\", "\\\\")
             include_file_name = self.format_type(include_file_name)
             include_directive = f"#include {include_file_name}"
             search_pattern = r"INCLUDE%06i\s+INCLUDE%06i;" % (key, key)
             s = re.sub(search_pattern, include_directive, s)
 
         return s
 
     def insert_line_comments(self, cpp_dict: CppDict, s: str) -> str:
-        """Inserts back all line directives."""
+        """Insert back all line directives."""
         for key, line_comment in cpp_dict.line_comments.items():
             # Search for the placeholder entry we created in _parse_tokenized_dict(),
             # and insert back the original block_comment.
             search_pattern = r"LINECOMMENT%06i\s+LINECOMMENT%06i;" % (key, key)
             s = re.sub(search_pattern, line_comment, s)
 
         return s
 
     def remove_trailing_spaces(self, s: str) -> str:
-        """Removes trailing spaces from all lines.
+        """Remove trailing spaces from all lines.
 
         Reads all lines from the passed in string, removes trailing spaces from each line and
         returns a new string with trailing spaces removed.
         """
         stream = io.StringIO(newline=None)
         _ = stream.write(s)
         _ = stream.seek(0)
@@ -740,23 +736,23 @@
         return ns
 
 
 class FoamFormatter(CppFormatter):
     """Formatter to serialize a dict into a string in OpenFOAM dictionary format."""
 
     def __init__(self):
-        """Implementation specific default configuration of FoamFormatter."""
+        """Implementation specific default configuration of FoamFormatter."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def to_string(
         self,
         dict: Union[MutableMapping[Any, Any], CppDict],
     ) -> str:
-        """Creates a string representation of the passed in dict in OpenFOAM dictionary format.
+        """Create a string representation of the passed in dict in OpenFOAM dictionary format.
 
         Parameters
         ----------
         dict : Union[MutableMapping[Any, Any], CppDict]
             dict to be formatted
 
         Returns
@@ -787,60 +783,60 @@
 
         # Substitute all remeining single quotes, if any, by double quotes:
         # s = re.sub('\'', '"', s)
 
         return s
 
     def format_empty_string(self, arg: str) -> str:
-        """Formats an empty string.
+        """Format an empty string.
 
         Parameters
         ----------
         arg : str
             the empty string to be formatted
 
         Returns
         -------
         str
             the formatted empty string
         """
         return self.add_double_quotes(arg)
 
     def format_multi_word_string(self, arg: str) -> str:
-        """Formats a multi word string.
+        """Format a multi word string.
 
         Parameters
         ----------
         arg : str
             the multi word string to be formatted
 
         Returns
         -------
         str
             the formatted multi word string
         """
         return self.add_double_quotes(arg)
 
     def format_expression_string(self, arg: str) -> str:
-        """Formats an expression.
+        """Format an expression.
 
         Parameters
         ----------
         arg : str
             the expression to be formatted
 
         Returns
         -------
         str
             the formatted expression
         """
         return self.add_double_quotes(arg)
 
     def make_default_block_comment(self, block_comment: str = "") -> str:
-        """Creates the default block comment (header) for files in OpenFOAM dictionary format."""
+        """Create the default block comment (header) for files in OpenFOAM dictionary format."""
         # If there is no ' C++ ' and 'OpenFoam' contained in block_comment,
         # then insert the OpenFOAM default block comment in front:
         default_block_comment = (
             "/*--------------------------------*- C++ -*----------------------------------*\\\n"
             "| =========                 |                                                 |\n"
             "| \\\\      /  F ield         | OpenFOAM: The Open Source CFD Toolbox           |\n"
             "|  \\\\    /   O peration     | Version:  dev                                   |\n"
@@ -864,23 +860,23 @@
         return block_comment
 
 
 class JsonFormatter(Formatter):
     """Formatter to serialize a dict into a string in JSON dictionary format."""
 
     def __init__(self):
-        """Implementation specific default configuration of JsonFormatter."""
+        """Implementation specific default configuration of JsonFormatter."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def to_string(
         self,
         dict: Union[MutableMapping[Any, Any], CppDict],
     ) -> str:
-        """Creates a string representation of the passed in dict in JSON dictionary format.
+        """Create a string representation of the passed in dict in JSON dictionary format.
 
         Parameters
         ----------
         dict : Union[MutableMapping[Any, Any], CppDict]
             dict to be formatted
 
         Returns
@@ -905,15 +901,15 @@
         )
         if isinstance(dict, CppDict):
             s = self.insert_includes(dict, s)
 
         return s
 
     def insert_includes(self, cpp_dict: CppDict, s: str) -> str:
-        """Inserts back all include directives."""
+        """Insert back all include directives."""
         for key, (include_directive, include_file_name, _) in cpp_dict.includes.items():
             # Search for the placeholder key in the Json string,
             # and insert back the original include directive.
             # include_file_name = include_file_name.replace('\\', '/')
             include_file_name = include_file_name.replace("\\", "\\\\\\\\")
             include_directive = f'"#include{key:06d}":"{include_file_name}"'
             search_pattern = r'"INCLUDE%06i"\s*:\s*"INCLUDE%06i"' % (key, key)
@@ -973,27 +969,27 @@
 
     def __init__(
         self,
         omit_prefix: bool = True,
         integrate_attributes: bool = True,
         remove_node_numbering: bool = True,
     ):
-        """Implementation specific default configuration of XmlFormatter."""
+        """Implementation specific default configuration of XmlFormatter."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
         # Save default configuration as attributes
         self.omit_prefix = omit_prefix
         self.integrate_attributes = integrate_attributes
         self.remove_node_numbering = remove_node_numbering
 
     def to_string(
         self,
         dict: Union[MutableMapping[Any, Any], CppDict],
     ) -> str:
-        """Creates a string representation of the passed in dict in XML format.
+        """Create a string representation of the passed in dict in XML format.
 
         Parameters
         ----------
         dict : Union[MutableMapping[Any, Any], CppDict]
             dict to be formatted
 
         Returns
@@ -1058,15 +1054,15 @@
 
     def populate_into_element(
         self,
         element: Element,
         arg: Union[MutableMapping[Any, Any], MutableSequence[Any], Any],
         xsd_uri: Union[str, None] = None,
     ):
-        """Populates arg into the XML element node.
+        """Populate arg into the XML element node.
 
         If arg is a dict or list, method will call itself recursively until all nested content within the dict or list
         is populated into nested elements, eventually creating an XML dom.
 
         Parameters
         ----------
         element : Element
@@ -1083,15 +1079,14 @@
         if isinstance(arg, MutableSequence):
             element.text = " ".join(str(x) for x in arg)
 
         elif isinstance(arg, MutableMapping):
             child_nodes = list(arg.keys())
 
             for index, (key, item) in enumerate(arg.items()):
-
                 if re.match("_content", key):
                     # Write back content (from the key-value pair "_content <content>;") into xml node.text
                     # In case of multiline content, do not write it inline between opening and closing tag,
                     # but add a line ending at the beginning and at the end, so that content gets formatted
                     # as an indented text block beween the opening and closing tag.
                     text = str(item)
                     if text not in [None, ""] and len(text.splitlines()) > 1:
```

### Comparing `dictIO-0.2.6/src/dictIO/parser.py` & `dictIO-0.2.7/src/dictIO/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def __init__(self):
         self.counter = BorgCounter()
         self.source_file = None
         return
 
     @classmethod
     def get_parser(cls, source_file: Union[Path, None] = None):
-        """Factory method returning a Parser instance matching the source file type to be parsed.
+        """Return a Parser instance matching the type of the source file to be parsed (factory method).
 
         Parameters
         ----------
         source_file : Path, optional
             name of the source file to be parsed, by default None
 
         Returns
@@ -69,15 +69,15 @@
 
     def parse_file(
         self,
         source_file: Union[str, os.PathLike[str]],
         target_dict: Union[CppDict, None] = None,
         comments: bool = True,
     ) -> CppDict:
-        """Parses a file and deserializes it into a dict.
+        """Parse a file and deserialize it into a dict.
 
         Parameters
         ----------
         source_file : Union[str, os.PathLike[str]]
             name of the dict file to be parsed
         target_dict : CppDict, optional
             the target dict the parsed dict file shall be merged into, by default None
@@ -116,34 +116,30 @@
         if target_dict is None:
             target_dict = CppDict(source_file)
         else:
             target_dict.source_file = source_file.absolute()
             target_dict.path = source_file.parent
             target_dict.name = source_file.name
 
-        # one final check only
-        # whether a file exists (can also have zero content)
-        # or a dict was given (can also contain nothing)
-        if not self.source_file.exists() and target_dict is None:
-            logger.error(
-                f"Parser.parse_file(): File or path does not exist ('{source_file}') or no target dict ({target_dict}) was given."
-            )
+        # one final check that the source file exists
+        if not self.source_file.exists():
+            logger.error(f"Parser.parse_file(): Source file does not exist ('{source_file}').")
 
         # Parse file content
         parsed_dict = self.parse_string(file_content, target_dict, comments)
 
         return parsed_dict
 
     def parse_string(
         self,
         string: str,
         target_dict: CppDict,
         comments: bool = True,
     ) -> CppDict:  # sourcery skip: lift-return-into-if
-        """Parses a string and deserializes it into a CppDict.
+        """Parse a string and deserialize it into a CppDict.
 
         Note: Override this method when implementing a specific Parser.
 
         Parameters
         ----------
         string : str
             the string to be parsed (i.e. the content of the file that had been read using parse_file())
@@ -160,21 +156,14 @@
 
         # +++VERIFY STRING CONTENT++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
         # Check that string is not empty.
         if not string:
             logger.warning(f"Parser.parse_string(): String to parse is empty: {string}")
 
-        # Create target dict in case no specific target dict was passed in
-        if target_dict is None:
-            logger.warning(
-                "Parser.parse_string(): Target dict is None. Will create new target dict, however, with empty filename."
-            )
-            target_dict = CppDict()
-
         # Create a local CppDict instance where the stringcontent is temporarily parsed into
         if target_dict.source_file:
             parsed_dict = CppDict(target_dict.source_file)
         else:
             parsed_dict = target_dict
 
         # +++PARSE DICTIONARY+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
@@ -187,15 +176,15 @@
         # (in the base class, however, this does not make sense - hence commented out)
         # target_dict.merge(parsed_dict)
 
         # +++RETURN PARSED DICTIONARY+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
         return parsed_dict
 
     def parse_type(self, arg: Any) -> Any:
-        """Parses a single value.
+        """Parse a single value.
 
         Parses a single value and casts it to its native type (str, int, float, boolean or None).
 
         Parameters
         ----------
         arg : Any
             the value to be parsed
@@ -263,15 +252,15 @@
 
         # Any other string: return 'as is', but make sure extra quotes, if so, are stripped.
         # Note: Also any placeholder strings will fall into this category.
         # Returned 'as is' they are kept unchanged, what is in fact what we want here.
         return __class__.remove_quotes_from_string(arg)
 
     def parse_types(self, arg: Union[MutableMapping[Any, Any], MutableSequence[Any]]):
-        """Parses multiple values.
+        """Parse multiple values.
 
         Parses all values inside a dict or list and casts them to its native types (str, int, float, boolean or None).
         The function traverses the passed in dict or list recursively
         so that all values in also nested dicts and lists are parsed.
 
         Parameters
         ----------
@@ -291,15 +280,15 @@
                     self.parse_types(arg[index])
                 else:
                     arg[index] = self.parse_type(arg[index])
         return
 
     @staticmethod
     def remove_quotes_from_string(arg: str, all: bool = False) -> str:
-        """Removes quotes from a string.
+        """Remove quotes from a string.
 
         Removes quotes (single and double quotes) from the string object passed in.
 
         Parameters
         ----------
         arg : str
             the string with quotes
@@ -322,15 +311,15 @@
 
         return re.sub(search_pattern, "", arg)
 
     @staticmethod
     def remove_quotes_from_strings(
         arg: Union[MutableMapping[Any, Any], MutableSequence[Any]]
     ) -> Union[MutableMapping[Any, Any], MutableSequence[Any]]:
-        """Removes quotes from multiple strings.
+        """Remove quotes from multiple strings.
 
         Removes quotes (single and double quotes) from all string objects inside a dict or list.
         The function traverses the passed in dict or list recursively
         so that all strings in also nested dicts and lists are processed.
 
 
         Parameters
@@ -360,25 +349,25 @@
         return arg
 
 
 class CppParser(Parser):
     """Parser to deserialize a string in dictIO dict file format into a CppDict."""
 
     def __init__(self):
-        """Implementation specific default configuration of CppParser."""
+        """Implementation specific default configuration of CppParser."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def parse_string(
         self,
         string: str,
         target_dict: CppDict,
         comments: bool = True,
     ) -> CppDict:
-        """Parses a string in dictIO dict file format and deserializes it into a CppDict.
+        """Parse a string in dictIO dict file format and deserialize it into a CppDict.
 
         Parameters
         ----------
         string : str
             the string to be parsed (i.e. the content of the file that had been read using parse_file())
         target_dict : CppDict
             the target dict the parsed dict file shall be merged into
@@ -446,15 +435,15 @@
         # +++MERGE PARSED DICTIONARY INTO TARGET DICTIONARY+++++++++++++++++++++++++++++++++++++++++
         target_dict.merge(parsed_dict)
 
         # +++RETURN PARSED DICTIONARY+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
         return parsed_dict
 
     def _extract_line_comments(self, dict: CppDict, comments: bool):
-        """Finds and extracts C++ line comments (// ..) from dict.line_content, and replaces them with Placeholders.
+        """Find and extract C++ line comments (// ..) from dict.line_content, and replace them with Placeholders.
 
         Finds C++ line comments (// line_comment), extracts them,
         and replaces the complete line with a placeholder in the form LINECOMMENT000000 .
         The extracted line comments are stored in .line_comments as key value pairs {index:line_comment}.
         index, therein, corresponds to the integer number in LINECOMMENT000000.
 
         Parameters
@@ -478,15 +467,15 @@
                     placeholder = ""
                 # Replace line comment with placeholder
                 dict.line_content[index] = dict.line_content[index].replace(line_comment, placeholder)
 
         return
 
     def _extract_includes(self, dict: CppDict):
-        """Finds and extracts #include directives from dict.line_content, and replaces them with Placeholders.
+        """Find and extract #include directives from dict.line_content, and replace them with Placeholders.
 
         Finds #includes directives (#include file), extracts them,
         and replaces the complete line where the include directive was found
         with a placeholder in the form #INCLUDE000000.
         The absolute path to the file referenced in the include directive is determined.
         The original line with its include directive as well as the absolute path to the file to include
         is then stored as a key-value pair in dict.includes, in the form {index:(include_directive, include_file_name, include_file_path)}
@@ -519,20 +508,20 @@
     def _convert_line_content_to_block_content(self, dict: CppDict):
         """Concatenates all lines from line_content to one long string (text block) and stores the result in block_content."""
         dict.block_content = "".join(dict.line_content)
         dict.line_content.clear()
         return
 
     def _remove_line_endings_from_block_content(self, dict: CppDict):
-        """Removes all line endings in .block_content and substuitutes them by single spaces."""
+        """Remove all line endings in .block_content and substuitute them by single spaces."""
         dict.block_content = re.sub(r"\n", " ", dict.block_content).strip()
         return
 
     def _extract_block_comments(self, dict: CppDict, comments: bool):
-        """Finds and extracts C++ block comments (/* .. */) from dict.block_content, and replaces them with Placeholders.
+        """Find and extract C++ block comments (/* .. */) from dict.block_content, and replace them with Placeholders.
 
         Finds C++ block comments (/* block_comment */), extracts them,
         and replaces them with a placeholder in the form BLOCKCOMMENT000000.
         The extracted block comments are stored in .block_comments as key value pairs {index:block_comment}.
         index, therein, corresponds to the integer number in BLOCKCOMMENT000000.
 
         Parameters
@@ -553,15 +542,15 @@
                 placeholder = ""
             # Replace block comment with placeholder
             dict.block_content = re.sub(re.escape(block_comment), placeholder, dict.block_content)
 
         return
 
     def _extract_string_literals(self, dict: CppDict):
-        """Finds and extracts string literals from dict.block_content, and replaces them with Placeholders.
+        """Find and extract string literals from dict.block_content, and replace them with Placeholders.
 
         Finds string literals, extracts them,
         and replaces them with a placeholder in the form STRINGLITERAL000000.
         Substrings within .block_content that are surrounded by single quotes are identified as string literals.
         The extracted string literals are stored in .string_literals as key value pairs {index:string_literal}.
         index, therein, corresponds to the integer number in STRINGLITERAL000000.
 
@@ -573,15 +562,14 @@
         search_pattern: Union[str, re.Pattern[str]]
         string_literals: List[str]
 
         # Step 1: Find single quoted string literals in .block_content
         search_pattern = r"\'.*?\'"
         string_literals = re.findall(search_pattern, dict.block_content, re.MULTILINE)
         for string_literal in string_literals:
-
             index = self.counter()
             placeholder = "STRINGLITERAL%06i" % index
 
             # Replace all occurances of the string literal in .block_content with the placeholder (STRINGLITERAL000000)
             # Note: For re.sub() to work properly we need to escape all special characters
             search_pattern = re.compile(re.escape(string_literal))
             dict.block_content = re.sub(
@@ -594,15 +582,14 @@
         # Step 2: Find double quoted string literals in .block_content
         # Double quoted strings are identified as string literals only in case they do not contain a $ character.
         # (double quoted strings containing a $ character are considered expressions, not string literals.)
         search_pattern = r"\".*?\""
         string_literals = re.findall(search_pattern, dict.block_content, re.MULTILINE)
         for string_literal in string_literals:
             if "$" not in string_literal:
-
                 index = self.counter()
                 placeholder = "STRINGLITERAL%06i" % index
 
                 # Replace all occurances of the string literal in .block_content with the placeholder (STRINGLITERAL000000)
                 # Note: For re.sub() to work properly we need to escape all special characters
                 search_pattern = re.compile(re.escape(string_literal))
                 dict.block_content = re.sub(
@@ -611,15 +598,15 @@
 
                 # Register the string literal in .string_literals
                 dict.string_literals.update({index: __class__.remove_quotes_from_string(string_literal)})
 
         return
 
     def _extract_expressions(self, dict: CppDict):
-        """Finds and extracts expressions from dict.block_content, and replaces them with Placeholders.
+        """Find and extract expressions from dict.block_content, and replace them with Placeholders.
 
         Finds expressions, extracts them,
         and replaces them with a placeholder in the form EXPRESSION000000.
         Substrings within .block_content that are surrounded by double quotes and contain minimum one $reference are identified as expressions.
         The extracted expressions are stored in .expressions as a key'd subdict with multiple elements {index:{'index': index, 'expression': expression, 'name': placeholder}}.
         index, therein, corresponds to the integer number in EXPRESSION000000.
 
@@ -634,15 +621,14 @@
         # Step 1: Find expressions in .block_content .
         # Expressions are double quoted strings that contain minimum one reference.
         # References are denoted using the '$' syntax familiar from shell programming.
         # Any key'd entries in a dict are considered variables and can be referenced.
         search_pattern = r'"[^"]*\$.*?"'
         expressions = re.findall(search_pattern, dict.block_content, re.MULTILINE)
         for expression in expressions:
-
             index = self.counter()
             placeholder = "EXPRESSION%06i" % index
 
             # Replace all occurances of the expression in .block_content with the placeholder (EXPRESSION000000)
             # Note: For re.sub() to work properly we need to escape all special characters
             # (covering both '$' as well as any mathematical operators in the expression)
             search_pattern = re.compile(re.escape(expression))
@@ -667,15 +653,15 @@
         return
 
     def _separate_delimiters(
         self,
         dict: CppDict,
         delimiters: Union[List[str], None] = None,
     ):
-        r"""Ensures that delimiters are separated by exactly one space before and after.
+        r"""Ensure that delimiters are separated by exactly one space before and after.
 
         Parses .block_content for occurences of the delimiters passed in, and strips any spaces surrounding each
         delimiter to exactly one single space before and one single space after the delimiter.
         Further, it removes all line endings from .block_content and eventually replaces them with single spaces.
 
         After _separate_delimiters() returns, .block_content contains only
         - words (with single char delimiters also considered a 'word' here)    and
@@ -708,20 +694,19 @@
         dict.tokens = [(0, i) for i in re.split(r"\s", dict.block_content)]
         dict.block_content = ""
 
         return
 
     def _determine_token_hierarchy(self, dict: CppDict):
         # sourcery skip: use-join
-        """Creates the hierarchy among the tokens and tests their indentation."""
+        """Create the hierarchy among the tokens and test their indentation."""
         level = 0
         count_open: List[str] = []
         count_close: List[str] = []
         for index, item in enumerate(dict.tokens):
-
             if item[1] in dict.openingBrackets:
                 push_pop = 1
                 count_open.append(item[1])
             elif item[1] in dict.closingBrackets:
                 push_pop = -1
                 count_close.append(item[1])
             else:
@@ -756,27 +741,27 @@
                 "_determine_token_hierarchy: opening and closing delimiters in dict %s are not balanced:\n%s"
                 % (dict.name, counted)
             )
 
         return
 
     def _convert_tokens_to_dict(self, dict: CppDict):
-        """Converts the hierarchic tokens into a dict."""
+        """Convert the hierarchic tokens into a dict."""
         dict.update(self._parse_tokenized_dict(dict))
         dict.tokens.clear()
 
         return
 
     def _parse_tokenized_dict(
         self,
         dict: CppDict,
         tokens: Union[List[Tuple[int, str]], None] = None,
         level: int = 0,
     ) -> Dict[str, Any]:
-        """Parses a tokenized dict and returns the parsed dict.
+        """Parse a tokenized dict and return the parsed dict.
 
         Parses all tokens, identifies the element within the tokenized dict each token represents or belongs to,
         converts related tokens into the element's type and stores it in local dict (parsed_dict).
 
         Following elements within the tokenized dict are identified and parsed:
         - nested data struct (list or dict)
         - key value pair
@@ -797,15 +782,14 @@
         last_index: Union[int, None] = None
         token_index: int = 0
         while token_index < len(tokens):
             # logger.info('token: %s%s' % ('\t'*tokens[tIndex][0], tokens[tIndex][1]))  # 1
 
             # Nested data struct (list or dict)   '(' = list    '{' = dict
             if tokens[token_index][1] in dict.openingBrackets:
-
                 # The name (key) of the data struct is by convention directly preceeding the opening bracket.
                 # ..except if there are line comments in between. skip those:
                 offset: int = 1
                 while re.match("^.*COMMENT.*$", str(tokens[token_index - offset][1])):
                     offset += 1
                 # name (key) of the data struct:
                 name: str = tokens[token_index - offset][1]
@@ -888,15 +872,14 @@
                 # To close out and move on, fast-forward the index of tokens
                 # to 'after' the data struct we just parsed:
                 if last_index is not None:
                     token_index = last_index + 1
 
             # Key value pair
             elif tokens[token_index][1] == ";" and tokens[token_index - 1][1] != ")":
-
                 # Read the name (key) and the value from the key value pair
                 # Parse from right to left, starting at the identified ';'
                 # and then copy the tokens into a temporary key_value_pair_tokens list:
                 key_value_pair_tokens: MutableSequence[Tuple[int, str]] = [tokens[token_index]]  # ';'
                 # key_value_pair_tokens.append(tokens[token_index])                       # ';'
                 key_value_pair_token_level: int = tokens[token_index][0]
                 i = 1
@@ -988,15 +971,15 @@
 
     def _parse_tokenized_list(
         self,
         dict: CppDict,
         tokens: Union[List[Tuple[int, str]], None] = None,
         level: int = 0,
     ) -> List[Any]:
-        """Parses a tokenized list and returns the parsed list.
+        """Parse a tokenized list and return the parsed list.
 
         Parses all tokens, identifies the element within the tokenized list each token represents or belongs to,
         converts related tokens into the element's type and stores it in local list (parsed_list).
 
         Following elements within the tokenized list are identified and parsed:
         - nested data struct (list or dict)
         - single value type
@@ -1107,15 +1090,15 @@
             # Iterate to next token
             token_index += 1
 
         # Return the parsed list
         return parsed_list
 
     def _find_companion(self, dict: CppDict, bracket: str) -> str:
-        """Returns the companion bracket character for the passed in bracket character.
+        """Return the companion bracket character for the passed in bracket character.
 
         Example: If you pass in '{', _find_companion() will return '}'  (and vice versa)
         """
         companion = ""
         for item in dict.brackets:
             if bracket == item[0]:
                 companion = item[1]
@@ -1140,15 +1123,15 @@
             while global_key := dict.find_global_key(query=placeholder):
                 # Back insert the string literal
                 dict.set_global_key(global_key, value)
         dict.string_literals.clear()
         return
 
     def _clean(self, dict: CppDict):
-        """Removes CppFormatter / CppParser specific internal keys from dict.
+        """Remove CppFormatter / CppParser specific internal keys from dict.
 
         Removes keys written by CppFormatter for documentation purposes
         but which shall not be created as keys in dict.data.
         In specific, it is the following two keys that get deleted if existing:
         _variables
         _includes
         """
@@ -1158,25 +1141,25 @@
             del dict.data["_includes"]
 
 
 class FoamParser(CppParser):
     """Parser to deserialize a string in OpenFOAM dictionary format into a CppDict."""
 
     def __init__(self):
-        """Implementation specific default configuration of FoamParser."""
+        """Implementation specific default configuration of FoamParser."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def parse_string(
         self,
         string: str,
         target_dict: CppDict,
         comments: bool = True,
     ) -> CppDict:
-        """Parses a string in OpenFOAM dictionary format and deserializes it into a CppDict.
+        """Parse a string in OpenFOAM dictionary format and deserialize it into a CppDict.
 
         Parameters
         ----------
         string : str
             the string to be parsed (i.e. the content of the file that had been read using parse_file())
         target_dict : CppDict
             the target dict the parsed dict file shall be merged into
@@ -1200,25 +1183,25 @@
         return parsed_dict
 
 
 class JsonParser(Parser):
     """Parser to deserialize a string in JSON dictionary format into a CppDict."""
 
     def __init__(self):
-        """Implementation specific default configuration of JsonParser."""
+        """Implementation specific default configuration of JsonParser."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
 
     def parse_string(
         self,
         string: str,
         target_dict: CppDict,
         comments: bool = True,
     ) -> CppDict:
-        """Parses a string in JSON dictionary format and deserializes it into a CppDict.
+        """Parse a string in JSON dictionary format and deserialize it into a CppDict.
 
         Parameters
         ----------
         string : str
             the string to be parsed (i.e. the content of the file that had been read using parse_file())
         target_dict : CppDict
             the target dict the parsed dict file shall be merged into
@@ -1279,15 +1262,15 @@
         return
 
     def _extract_expression(
         self,
         parsed_dict: CppDict,
         string: str,
     ) -> str:
-        """Extracts a single expression.
+        """Extract a single expression.
 
         Parses a string, checks whether it contains an expression, and if so,
         extracts the expression and replaces it with a placeholder.
 
         Parameters
         ----------
         parsed_dict : CppDict
@@ -1328,16 +1311,16 @@
 
     def _replace_and_register_expression(
         self,
         parsed_dict: CppDict,
         string: str,
         expression: str,
     ) -> str:
-        """Replaces all occurances of expression in string with a placeholder (EXPRESSION000000)
-        and registers the expression in parsed_dict.
+        """Replace all occurances of expression in string with a placeholder (EXPRESSION000000)
+        and register the expression in parsed_dict.
 
         Parameters
         ----------
         parsed_dict : CppDict
             the CppDict instance the expression will be registered in
         string : str
             the string in which expression shall be found and replaced
@@ -1360,15 +1343,15 @@
         return modified_string
 
     def _extract_expressions(
         self,
         parsed_dict: CppDict,
         arg: Union[MutableMapping[Any, Any], MutableSequence[Any]],
     ):
-        """Finds and extracts expressions in a dict or list and replaces them with Placeholders.
+        """Find and extract expressions in a dict or list and replace them with Placeholders.
 
         Finds expressions, extracts them, and replaces them with a placeholder in the form EXPRESSION000000.
         String values that contain minimum one $reference are identified as expressions.
         The extracted expressions are stored in .expressions as a key'd subdict with multiple elements {index:{'index': index, 'expression': expression, 'name': placeholder}}.
         index, therein, corresponds to the integer number in EXPRESSION000000.
 
         Parameters
@@ -1400,27 +1383,27 @@
 class XmlParser(Parser):
     """Parser to deserialize a string in XML format into a CppDict."""
 
     def __init__(
         self,
         add_node_numbering: bool = True,
     ):
-        """Implementation specific default configuration of XmlParser."""
+        """Implementation specific default configuration of XmlParser."""  # noqa: D401
         # Invoke base class constructor
         super().__init__()
         # Save default configuration as attributes
         self.add_node_numbering = add_node_numbering
 
     def parse_string(
         self,
         string: str,
         target_dict: CppDict,
         comments: bool = True,
     ) -> CppDict:
-        """Parses a string in XML format and deserializes it into a CppDict.
+        """Parse a string in XML format and deserialize it into a CppDict.
 
         Parameters
         ----------
         string : str
             the string to be parsed (i.e. the content of the file that had been read using parse_file())
         target_dict : CppDict
             the target dict the parsed dict file shall be merged into
@@ -1442,30 +1425,30 @@
         # Default configuration
         namespaces: Dict[str, str] = {"xs": "https://www.w3.org/2009/XMLSchema/XMLSchema.xsd"}
         root_tag: str = "NOTSPECIFIED"
 
         # Create XML parser
         parser: XMLParser = ETCompatXMLParser()
         # Read root element from XML string
-        root_element: Element = fromstring(string.encode("utf-8"), parser)
+        root_element: Element = fromstring(string.encode("utf-8"), parser)  # type: ignore
         # Read root tag from XML string
         # there is a problem with .tag :
         # fromstring does not completely push all attributes into .attrib
         # only version, not xmlns
         # xmlns remains as {XMLNSCONTENT}ROOTTAG
         # re.sub to fix that temporarily
         # solution needed
         _root_tag: str = root_element.tag
         root_tag = re.sub(r"\{.*\}", "", _root_tag) or root_tag
         # Read namespaces from XML string
         namespaces = dict(root_element.nsmap) or namespaces  # pyright: ignore
         # Reformat None keys in namespaces to key 'None' (as string)
         temp_keys_copy: List[str] = list(namespaces)
         for key in temp_keys_copy:
-            if key is None:
+            if key is None:  # pyright: ignore
                 try:
                     value = namespaces[key]
                     del namespaces[key]
                     namespaces["None"] = value
                 except Exception:
                     logger.exception(
                         "XmlParser.parseString(): Reformatting None keys in namespaces to key 'None' failed"
```

### Comparing `dictIO-0.2.6/src/dictIO/utils/counter.py` & `dictIO-0.2.7/src/dictIO/utils/counter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.6/src/dictIO/utils/logging.py` & `dictIO-0.2.7/src/dictIO/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.6/src/dictIO/utils/path.py` & `dictIO-0.2.7/src/dictIO/utils/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 __all__ = ["highest_common_root_folder", "relative_path"]
 
 logger = logging.getLogger(__name__)
 
 
 def highest_common_root_folder(paths: Sequence[Path]) -> Path:
-    """Returns the highest common root folder among the passed in paths.
+    """Return the highest common root folder among the passed in paths.
 
     Parameters
     ----------
     paths : Sequence[Path]
         A sequence of path objects. Can be files or folders, or both.
 
     Returns
@@ -51,15 +51,15 @@
     if common_parts:
         return Path(*tuple(common_parts))
     else:
         raise ValueError("The passed in paths do not share a common root folder.")
 
 
 def relative_path(from_path: Path, to_path: Path) -> Path:
-    """Returns the relative path from one path to another.
+    """Return the relative path from one path to another.
 
     Parameters
     ----------
     from_path : Path
         The start point path.
     to_path : Path
         The end point path.
```

### Comparing `dictIO-0.2.6/src/dictIO/utils/strings.py` & `dictIO-0.2.7/src/dictIO/utils/strings.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 __all__ = ["remove_quotes", "string_diff"]
 
 
 logger = logging.getLogger(__name__)
 
 
 def remove_quotes(string: str):
-    """
-    Removes quotes (single or double quotes) from the string object passed in.
+    """Remove quotes (single or double quotes) from the string object passed in.
+
     Not only leading and trailing quotes are removed; also any quotes inside a string, if so, are removed.
     """
-    # search_pattern = re.compile(r'(^[\'\\"]{1}|[\'\\"]{1}$)')  #Removes only leading and trailing quotes. Quotes inside a string are kept.
-    search_pattern = re.compile(
-        r"[\'\"]"
-    )  # Removes ALL quotes in a string. Meaning, not only leading and trailing quotes, but also quotes inside a string are removed.
+    # Pattern 1 removes only leading and trailing quotes. Quotes inside a string are kept.
+    # @NOTE: Left here for documentation purposes only. Pattern 2 is the one used.
+    # search_pattern = re.compile(r'(^[\'\\"]{1}|[\'\\"]{1}$)')
+
+    # Pattern 2 removes ALL quotes in a string.
+    # Meaning, not only leading and trailing quotes, but also quotes inside a string are removed.
+    search_pattern = re.compile(r"[\'\"]")
     return re.sub(search_pattern, "", string)
 
 
 def string_diff(text_1: str, text_2: str):
     """
     diff line by line
     printing only diff.
```

### Comparing `dictIO-0.2.6/src/dictIO.egg-info/PKG-INFO` & `dictIO-0.2.7/src/dictIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.2.6
+Version: 0.2.7
 Summary: Read, write and manipulate dictionary text files.
 Home-page: https://dnv-opensource.github.io/dictIO/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/dictIO
 Platform: Python3.x
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -120,15 +121,15 @@
     Install dictIO's dependencies:
     ~~~sh
     $ pip install -r requirements-dev.txt
     ~~~
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

