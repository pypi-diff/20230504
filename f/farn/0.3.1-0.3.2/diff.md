# Comparing `tmp/farn-0.3.1.tar.gz` & `tmp/farn-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farn-0.3.1.tar", last modified: Wed Jan 11 13:00:05 2023, max compression
+gzip compressed data, was "farn-0.3.2.tar", last modified: Thu May  4 15:05:02 2023, max compression
```

## Comparing `farn-0.3.1.tar` & `farn-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.632666 farn-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-11 12:59:46.000000 farn-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-11 12:59:46.000000 farn-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-01-11 13:00:05.632666 farn-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-01-11 12:59:46.000000 farn-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-01-11 12:59:46.000000 farn-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-01-11 13:00:05.632666 farn-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.624667 farn-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.624667 farn-0.3.1/src/farn/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9419 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/cli/farn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/core/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/core/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29796 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/farn.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/batchProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/run/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/cli/batchProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/subProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/run/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/run/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/sampling/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.632666 farn-0.3.1/src/farn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-11 12:59:46.000000 farn-0.3.1/src/farn/utils/os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:00:05.628666 farn-0.3.1/src/farn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-11 13:00:05.000000 farn-0.3.1/src/farn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 15:04:38.000000 farn-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:04:38.000000 farn-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-04 15:05:02.891667 farn-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-04 15:04:38.000000 farn-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 15:04:38.000000 farn-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 15:05:02.891667 farn-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.871667 farn-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.879667 farn-0.3.2/src/farn/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9418 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/cli/farn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29786 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/farn.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/batchProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/cli/batchProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/subProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/run/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/run/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.887667 farn-0.3.2/src/farn/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/sampling/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/src/farn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 15:04:38.000000 farn-0.3.2/src/farn/utils/os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.883667 farn-0.3.2/src/farn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 15:05:02.000000 farn-0.3.2/src/farn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:05:02.891667 farn-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-04 15:04:38.000000 farn-0.3.2/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-05-04 15:04:38.000000 farn-0.3.2/tests/test_farn.py
```

### Comparing `farn-0.3.1/LICENSE` & `farn-0.3.2/LICENSE`

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

### Comparing `farn-0.3.1/PKG-INFO` & `farn-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.1
+Version: 0.3.2
 Summary: n-dimensional case generator.
 Home-page: https://dnv-opensource.github.io/farn/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/farn
 Platform: Python3.x
 Classifier: Development Status :: 4 - Beta
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
@@ -125,15 +126,15 @@
     Install farn's dependencies:
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

### Comparing `farn-0.3.1/README.md` & `farn-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     Install farn's dependencies:
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

### Comparing `farn-0.3.1/pyproject.toml` & `farn-0.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

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
-00000400: 2020 2020 2249 222c 0d0a 2020 2020 2242      "I",..    "B
-00000410: 222c 0d0a 5d0d 0a74 6172 6765 742d 7665  ",..]..target-ve
-00000420: 7273 696f 6e20 3d20 2270 7933 3922 0d0a  rsion = "py39"..
-00000430: 0d0a 5b74 6f6f 6c2e 7275 6666 2e70 6570  ..[tool.ruff.pep
-00000440: 382d 6e61 6d69 6e67 5d0d 0a69 676e 6f72  8-naming]..ignor
-00000450: 652d 6e61 6d65 7320 3d20 5b0d 0a20 2020  e-names = [..   
-00000460: 2022 7465 7374 5f2a 222c 0d0a 2020 2020   "test_*",..    
-00000470: 2273 6574 5570 222c 0d0a 2020 2020 2274  "setUp",..    "t
-00000480: 6561 7244 6f77 6e22 2c0d 0a5d 0d0a 0d0a  earDown",..]....
-00000490: 5b74 6f6f 6c2e 7275 6666 2e70 7964 6f63  [tool.ruff.pydoc
-000004a0: 7374 796c 655d 0d0a 636f 6e76 656e 7469  style]..conventi
-000004b0: 6f6e 203d 2022 6e75 6d70 7922 0d0a 0d0a  on = "numpy"....
-000004c0: 5b74 6f6f 6c2e 7275 6666 2e70 6572 2d66  [tool.ruff.per-f
-000004d0: 696c 652d 6967 6e6f 7265 735d 0d0a 225f  ile-ignores].."_
-000004e0: 5f69 6e69 745f 5f2e 7079 2220 3d20 5b22  _init__.py" = ["
-000004f0: 4930 3031 225d 0d0a 222e 2f74 6573 7473  I001"].."./tests
-00000500: 2f2a 2220 3d20 5b22 4422 5d0d 0a0d 0a5b  /*" = ["D"]....[
-00000510: 746f 6f6c 2e70 7972 6967 6874 5d0d 0a65  tool.pyright]..e
-00000520: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
-00000530: 222e 6769 7422 2c0d 0a20 2020 2022 2e76  ".git",..    ".v
-00000540: 656e 7622 2c0d 0a20 2020 2022 2e74 6f78  env",..    ".tox
-00000550: 222c 0d0a 2020 2020 2262 7569 6c64 222c  ",..    "build",
-00000560: 0d0a 2020 2020 2264 6973 7422 2c0d 0a20  ..    "dist",.. 
-00000570: 2020 2022 2a2a 2f5f 5f70 7963 6163 6865     "**/__pycache
-00000580: 5f5f 222c 0d0a 2020 2020 222e 2f64 6f63  __",..    "./doc
-00000590: 732f 736f 7572 6365 2f63 6f6e 662e 7079  s/source/conf.py
-000005a0: 222c 0d0a 5d0d 0a65 7874 7261 5061 7468  ",..]..extraPath
-000005b0: 7320 3d20 5b22 2e2f 7372 6322 5d0d 0a74  s = ["./src"]..t
-000005c0: 7970 6543 6865 636b 696e 674d 6f64 6520  ypeCheckingMode 
-000005d0: 3d20 2262 6173 6963 220d 0a75 7365 4c69  = "basic"..useLi
-000005e0: 6272 6172 7943 6f64 6546 6f72 5479 7065  braryCodeForType
-000005f0: 7320 3d20 7472 7565 0d0a 7265 706f 7274  s = true..report
-00000600: 4d69 7373 696e 6750 6172 616d 6574 6572  MissingParameter
-00000610: 5479 7065 203d 2022 6572 726f 7222 0d0a  Type = "error"..
-00000620: 7265 706f 7274 556e 6b6e 6f77 6e50 6172  reportUnknownPar
-00000630: 616d 6574 6572 5479 7065 203d 2022 7761  ameterType = "wa
-00000640: 726e 696e 6722 0d0a 7265 706f 7274 556e  rning"..reportUn
-00000650: 6b6e 6f77 6e4d 656d 6265 7254 7970 6520  knownMemberType 
-00000660: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000670: 6f72 744d 6973 7369 6e67 5479 7065 4172  ortMissingTypeAr
-00000680: 6775 6d65 6e74 203d 2022 6572 726f 7222  gument = "error"
-00000690: 0d0a 7265 706f 7274 5072 6f70 6572 7479  ..reportProperty
-000006a0: 5479 7065 4d69 736d 6174 6368 203d 2022  TypeMismatch = "
-000006b0: 6572 726f 7222 0d0a 7265 706f 7274 4675  error"..reportFu
-000006c0: 6e63 7469 6f6e 4d65 6d62 6572 4163 6365  nctionMemberAcce
-000006d0: 7373 203d 2022 7761 726e 696e 6722 0d0a  ss = "warning"..
-000006e0: 7265 706f 7274 5072 6976 6174 6555 7361  reportPrivateUsa
-000006f0: 6765 203d 2022 7761 726e 696e 6722 0d0a  ge = "warning"..
-00000700: 7265 706f 7274 5479 7065 436f 6d6d 656e  reportTypeCommen
-00000710: 7455 7361 6765 203d 2022 7761 726e 696e  tUsage = "warnin
-00000720: 6722 0d0a 7265 706f 7274 496e 636f 6d70  g"..reportIncomp
-00000730: 6174 6962 6c65 4d65 7468 6f64 4f76 6572  atibleMethodOver
-00000740: 7269 6465 203d 2022 7761 726e 696e 6722  ride = "warning"
-00000750: 0d0a 7265 706f 7274 496e 636f 6d70 6174  ..reportIncompat
-00000760: 6962 6c65 5661 7269 6162 6c65 4f76 6572  ibleVariableOver
-00000770: 7269 6465 203d 2022 6572 726f 7222 0d0a  ride = "error"..
-00000780: 7265 706f 7274 496e 636f 6e73 6973 7465  reportInconsiste
-00000790: 6e74 436f 6e73 7472 7563 746f 7220 3d20  ntConstructor = 
-000007a0: 2265 7272 6f72 220d 0a72 6570 6f72 744f  "error"..reportO
-000007b0: 7665 726c 6170 7069 6e67 4f76 6572 6c6f  verlappingOverlo
-000007c0: 6164 203d 2022 7761 726e 696e 6722 0d0a  ad = "warning"..
-000007d0: 7265 706f 7274 556e 696e 6974 6961 6c69  reportUninitiali
-000007e0: 7a65 6449 6e73 7461 6e63 6556 6172 6961  zedInstanceVaria
-000007f0: 626c 6520 3d20 2277 6172 6e69 6e67 220d  ble = "warning".
-00000800: 0a72 6570 6f72 7443 616c 6c49 6e44 6566  .reportCallInDef
-00000810: 6175 6c74 496e 6974 6961 6c69 7a65 7220  aultInitializer 
-00000820: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000830: 6f72 7455 6e6e 6563 6573 7361 7279 4973  ortUnnecessaryIs
-00000840: 496e 7374 616e 6365 203d 2022 696e 666f  Instance = "info
-00000850: 726d 6174 696f 6e22 0d0a 7265 706f 7274  rmation"..report
-00000860: 556e 6e65 6365 7373 6172 7943 6173 7420  UnnecessaryCast 
-00000870: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000880: 6f72 7455 6e6e 6563 6573 7361 7279 436f  ortUnnecessaryCo
-00000890: 6d70 6172 6973 6f6e 203d 2022 7761 726e  mparison = "warn
-000008a0: 696e 6722 0d0a 7265 706f 7274 556e 6e65  ing"..reportUnne
-000008b0: 6365 7373 6172 7943 6f6e 7461 696e 7320  cessaryContains 
-000008c0: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-000008d0: 6f72 7455 6e75 7365 6443 616c 6c52 6573  ortUnusedCallRes
-000008e0: 756c 7420 3d20 2277 6172 6e69 6e67 220d  ult = "warning".
-000008f0: 0a72 6570 6f72 7455 6e75 7365 6445 7870  .reportUnusedExp
-00000900: 7265 7373 696f 6e20 3d20 2277 6172 6e69  ression = "warni
-00000910: 6e67 220d 0a72 6570 6f72 744d 6174 6368  ng"..reportMatch
-00000920: 4e6f 7445 7868 6175 7374 6976 6520 3d20  NotExhaustive = 
-00000930: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
-00000940: 7453 6861 646f 7765 6449 6d70 6f72 7473  tShadowedImports
-00000950: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
-00000960: 706f 7274 556e 7479 7065 6446 756e 6374  portUntypedFunct
-00000970: 696f 6e44 6563 6f72 6174 6f72 203d 2022  ionDecorator = "
-00000980: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
-00000990: 556e 7479 7065 6442 6173 6543 6c61 7373  UntypedBaseClass
-000009a0: 203d 2022 6572 726f 7222 0d0a 7265 706f   = "error"..repo
-000009b0: 7274 556e 7479 7065 644e 616d 6564 5475  rtUntypedNamedTu
-000009c0: 706c 6520 3d20 2277 6172 6e69 6e67 220d  ple = "warning".
-000009d0: 0a23 2041 6374 6976 6174 6520 7468 6520  .# Activate the 
-000009e0: 666f 6c6c 6f77 696e 6720 7275 6c65 7320  following rules 
-000009f0: 6f6e 6c79 206c 6f63 616c 6c79 2061 6e64  only locally and
-00000a00: 2074 656d 706f 7261 7279 2c20 692e 652e   temporary, i.e.
-00000a10: 2066 6f72 2061 2051 4120 7365 7373 696f   for a QA sessio
-00000a20: 6e2e 0d0a 2320 2846 6f72 2073 6572 7665  n...# (For serve
-00000a30: 7220 7369 6465 2043 4920 7468 6579 2061  r side CI they a
-00000a40: 7265 2063 6f6e 7369 6465 7265 6420 746f  re considered to
-00000a50: 6f20 7374 7269 6374 2e29 0d0a 2320 7265  o strict.)..# re
-00000a60: 706f 7274 436f 6e73 7461 6e74 5265 6465  portConstantRede
-00000a70: 6669 6e69 7469 6f6e 203d 2022 7761 726e  finition = "warn
-00000a80: 696e 6722 0d0a 2320 7265 706f 7274 556e  ing"..# reportUn
-00000a90: 6e65 6365 7373 6172 7954 7970 6549 676e  necessaryTypeIgn
-00000aa0: 6f72 6543 6f6d 6d65 6e74 203d 2022 696e  oreComment = "in
-00000ab0: 666f 726d 6174 696f 6e22 0d0a 2320 7265  formation"..# re
-00000ac0: 706f 7274 496d 706f 7274 4379 636c 6573  portImportCycles
-00000ad0: 203d 2022 7761 726e 696e 6722 0d0a 2320   = "warning"..# 
-00000ae0: 7265 706f 7274 496d 706c 6963 6974 5374  reportImplicitSt
-00000af0: 7269 6e67 436f 6e63 6174 656e 6174 696f  ringConcatenatio
-00000b00: 6e20 3d20 2277 6172 6e69 6e67 220d 0a    n = "warning"..
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

### Comparing `farn-0.3.1/setup.cfg` & `farn-0.3.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = farn
-version = 0.3.1
+version = 0.3.2
 summary = n-dimensional case generator.
 description = Python package to generate an n-dimensional case folder structure applying linear and spatial sampling strategies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://dnv-opensource.github.io/farn/README.html
 project_urls = 
 	GitHub = https://github.com/dnv-opensource/farn
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
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
@@ -34,25 +35,26 @@
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	lxml>=4.9
+	lxml-stubs>=0.4.0
 	numpy>=1.23
-	pandas>=1.5
-	scipy>=1.9
-	matplotlib>=3.6
+	pandas>=2.0
+	scipy>=1.10
+	matplotlib>=3.7
 	pyDOE2>=1.3
-	Pillow>=9.3
+	Pillow>=9.5
 	psutil>=5.9
-	SALib>=1.4.6
+	SALib>=1.4.7
 	sobol-seq>=0.2
-	dictIO>=0.2.6
-	ospx>=0.2.8
+	dictIO>=0.2.7
+	ospx>=0.2.9
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [options.entry_points]
@@ -77,19 +79,19 @@
 [coverage:paths]
 source = 
 	src/farn
 	*/site-packages/farn
 
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

### Comparing `farn-0.3.1/src/farn/cli/farn.py` & `farn-0.3.2/src/farn/cli/farn.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from farn import run_farn  # noqa E402
 from farn.utils.logging import configure_logging  # noqa E402
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = ArgumentParser(
         prog="farn",
         usage="%(prog)s farnDict [options [args]]",
         epilog="_________________farn___________________",
         prefix_chars="-",
         add_help=True,
         description=(
```

### Comparing `farn-0.3.1/src/farn/core/case.py` & `farn-0.3.2/src/farn/core/case.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 )
                 return True
             return False
 
         return True
 
     def to_dict(self) -> Dict[str, Any]:
-        """Returns a dict with all case attributes.
+        """Return a dict with all case attributes.
 
         Returns
         -------
         Dict[str, Any]
             dict with all case attributes
         """
         return {
@@ -247,15 +247,15 @@
     """
 
     def to_pandas(
         self,
         use_path_as_index: bool = True,
         parameters_only: bool = False,
     ) -> DataFrame:
-        """Returns cases as a pandas Dataframe.
+        """Return cases as a pandas Dataframe.
 
         Returns a DataFrame with case properties and case specific parameter values of all cases.
 
         Parameters
         ----------
         use_path_as_index : bool, optional
             turn path column into index column, by default True
@@ -303,15 +303,15 @@
 
         if use_path_as_index:
             df_X.set_index("path", inplace=True)
 
         return df_X
 
     def to_numpy(self) -> ndarray[Any, Any]:
-        """Returns parameter values of all cases as a 2-dimensional numpy array.
+        """Return parameter values of all cases as a 2-dimensional numpy array.
 
         Returns
         -------
         ndarray[Any, Any]
             2-dimensional numpy array with case specific parameter values of all cases.
         """
         df_X: DataFrame = self.to_pandas(parameters_only=True)  # noqa: N806
@@ -319,15 +319,15 @@
         return array
 
     def filter(
         self,
         levels: Union[int, Sequence[int]] = -1,
         valid_only: bool = True,
     ) -> "Cases":
-        """Returns a sub-set of cases according to the passed selection criteria.
+        """Return a sub-set of cases according to the passed in selection criteria.
 
         Parameters
         ----------
         levels : Union[int, Sequence[int]], optional
             return all cases of a distinct level, or a sequence of levels.
             level=-1 returns the last level (the leaf cases), by default -1
         valid_only : bool, optional
```

### Comparing `farn-0.3.1/src/farn/core/parameter.py` & `farn-0.3.2/src/farn/core/parameter.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.1/src/farn/farn.py` & `farn-0.3.2/src/farn/farn.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     farn_dict_file: Union[str, os.PathLike[str]],
     sample: bool = False,
     generate: bool = False,
     command: Union[str, None] = None,
     batch: bool = False,
     test: bool = False,
 ) -> Cases:
-    """Runs farn.
+    """Run farn.
 
     Runs the sampling for all layers as configured in farn dict,
     generates the corresponding case folder structure and
     executes user-defined shell command sets in all case folders.
 
     Parameters
     ----------
@@ -153,15 +153,15 @@
         return
 
     def create_samples_in_layer(
         level: int,
         layer_name: str,
         layer: MutableMapping[str, Any],
     ):
-        """Runs sampling and generates the samples in the passed in layer."""
+        """Run sampling and generate the samples in the passed in layer."""
         if "_sampling" not in layer:
             logger.error("no '_sampling' element in layer")
             return
         if "_type" not in layer["_sampling"]:
             logger.error("no '_type' element in sampling")
             return
 
@@ -203,15 +203,15 @@
 
 
 def create_cases(
     farn_dict: MutableMapping[Any, Any],
     case_dir: Path,
     valid_only: bool = False,
 ) -> Cases:
-    """Creates cases based on the layers, filter expressions and samples defined in the passed farn dict.
+    """Create cases based on the layers, filter expressions and samples defined in the passed farn dict.
 
     Creates case objects for all cases derived by recursive permutation of layers and the case specific samples defined per layer.
     create_cases() creates one distinct case object for each case, holding all case attributes (parameters) set to their case specific values.
 
     Optionally, only _valid_ cases can be returned, i.e. cases which fulfill the filter criteria configured for the respective layer.
     Invalid cases then get excluded.
 
@@ -384,15 +384,15 @@
         log_msg = f"Successfully listed {len(leaf_cases)} case{plural(len(leaf_cases))}. "
     logger.info(log_msg)
 
     return cases
 
 
 def create_case_folders(cases: MutableSequence[Case]) -> int:
-    """Creates the case folder structure for the passed in cases.
+    """Create the case folder structure for the passed in cases.
 
     Parameters
     ----------
     cases : MutableSequence[Case]
         cases the case folders shall be created for.
 
     Returns
@@ -411,15 +411,15 @@
 
     logger.info(f"Successfully created {number_of_case_folders_created} case folders.")
 
     return number_of_case_folders_created
 
 
 def create_param_dict_files(cases: MutableSequence[Case]) -> int:
-    """Creates the case specific paramDict files in the case folders of the passed in cases.
+    """Create the case specific paramDict files in the case folders of the passed in cases.
 
     paramDict files contain the case specific parameters, meaning, via the paramDict files the case specific values
     for all parameters get distributed to and persisted in the case folders.
 
     Parameters
     ----------
     cases : MutableSequence[Case]
@@ -526,15 +526,15 @@
 
 def execute_command_set(
     cases: MutableSequence[Case],
     command_set: str,
     batch: bool = True,
     test: bool = False,
 ) -> int:
-    """Executes the given command set in the case folders of the passed in cases.
+    """Execute the given command set in the case folders of the passed in cases.
 
     Parameters
     ----------
     cases : MutableSequence[Case]
         cases for which the specified command set shall be executed.
     command_set : str
         name of the command set to be executed, as defined in farnDict
@@ -630,15 +630,15 @@
                 f"in {number_of_cases_registered} case folder{plural(number_of_cases_registered)}."
             )
 
     return number_of_cases_registered
 
 
 def _set_up_farn_environment(farn_dict_file: Path) -> Dict[str, Path]:
-    """Reads the '_environment' section from farn dict and sets up the farn environment accordingly.
+    """Read the '_environment' section from farn dict and sets up the farn environment accordingly.
 
     Reads the '_environment' section from farnDict and sets up the farn environment directories as configured therein.
     If the '_environment' section or certain entries therein are missing in farn dict, default values will be used.
 
     Parameters
     ----------
     farn_dict_file : Path
@@ -683,15 +683,15 @@
 
     logger.info("Successfully set up farn environment.")
 
     return farn_dirs
 
 
 def _configure_additional_logging_handler_exclusively_for_farn(log_dir: Path):
-    """Creates an additional logging handler exclusively for the farn log.
+    """Create an additional logging handler exclusively for the farn log.
 
     Parameters
     ----------
     log_dir : Path
         folder in which the log file will be created
     """
     # Create log file
@@ -708,15 +708,15 @@
     file_handler_already_exists: bool = any(handler.name == file_handler.name for handler in root_logger.handlers)
     if not file_handler_already_exists:
         root_logger.addHandler(file_handler)
     return
 
 
 def _remove_old_case_list_files():  # sourcery skip: avoid-builtin-shadow
-    """Removes old case list files, if existing."""
+    """Remove old case list files, if existing."""
     logger.info("Remove old case list files...")
 
     lists = [list for list in Path.cwd().rglob("*") if re.search("(path|queue)List", str(list))]
 
     for list in lists:
         list = Path(list)
         list.unlink()
```

### Comparing `farn-0.3.1/src/farn/run/batchProcess.py` & `farn-0.3.2/src/farn/run/batchProcess.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(
         self,
         case_list_file: Path,
         command: str,
         timeout: int = 3600,
         max_number_of_cpus: int = 0,
     ):
-        """Instantiates an asynchroneous batch processor
+        """Instantiate an asynchroneous batch processor
         to execute a shell command in multiple case folders.
 
         Parameters
         ----------
         case_list_file : Path
             the file containing the list of case folders the shell command shall be executed in
         command : str
@@ -35,15 +35,15 @@
         """
         self.case_list_file: Path = case_list_file
         self.command: str = command
         self.timeout: int = timeout
         self.max_number_of_cpus: int = max_number_of_cpus
 
     def run(self):
-        """Runs the shell command in all case folders."""
+        """Run the shell command in all case folders."""
 
         # Check whether caselist file exists
         if not self.case_list_file.is_file():
             logger.error(f"AsyncBatchProcessor: File {self.case_list_file} not found.")
             return
 
         # Read the case list and fill job queue
```

### Comparing `farn-0.3.1/src/farn/run/cli/batchProcess.py` & `farn-0.3.2/src/farn/run/cli/batchProcess.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from farn.run.batchProcess import AsyncBatchProcessor
 from farn.utils.logging import configure_logging
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = ArgumentParser(
         prog="batchProcess",
         usage="%(prog)s caseList [options [args]]",
         epilog="_________________batchProcess___________________",
         prefix_chars="-",
         add_help=True,
         description=("Batch processes a list of cases, executing the specified shell command in all case folders."),
```

### Comparing `farn-0.3.1/src/farn/run/subProcess.py` & `farn-0.3.2/src/farn/run/subProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 logger = logging.getLogger(__name__)
 
 # Lock for operations that are not intrinsically thread safe
 lock = Lock()
 
 
 def execute_in_sub_process(command: str, path: Union[Path, None] = None, timeout: int = 3600):
-    """Creates a subprocess with cwd = path and executes the given shell command.
+    """Create a subprocess with cwd = path and execute the given shell command.
+
     The subprocess runs asyncroneous. The calling thread waits until the subprocess returns or until timeout is exceeded.
     If the subprocess has not returned after [timeout] seconds, the subprocess gets killed.
     """
 
     path = path or Path.cwd()
 
     # Configure and start subprocess in workDir (this part shall be atomic, hence secured by lock)
     with lock:
-
         command = re.sub(r"(^\'|\'$)", "", command)
 
         args = re.split(r"\s+", command.strip())
 
         sub_process = sub.Popen(args, stdout=sub.PIPE, stderr=sub.PIPE, shell=True, cwd=f"{path}")
 
         if len(command) > 18:
@@ -53,24 +53,22 @@
 
     _log_subprocess_output(command, path, stdout, stderr)
 
     return (stdout, stderr)
 
 
 def _log_subprocess_output(command: str, path: Path, stdout: bytes, stderr: bytes):
-
     if out := str(stdout, encoding="utf-8"):
         _log_subprocess_log(command, path, out)
 
     if err := str(stderr, encoding="utf-8"):
         _log_subprocess_log(command, path, err)
 
 
 def _log_subprocess_log(command: str, path: Path, log: str):
-
     if re.search("error", log, re.I):
         logger.error(f"during execution of {command} in {path}\n{log}")
     elif re.search("warning", log, re.I):
         logger.warning(f"from execution of {command} in {path}\n{log}")
     elif re.search("info", log, re.I):
         logger.info(f"from execution of {command} in {path}\n{log}")
     elif re.search("debug", log, re.I):
```

### Comparing `farn-0.3.1/src/farn/run/utils/threading.py` & `farn-0.3.2/src/farn/run/utils/threading.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 logger = logging.getLogger(__name__)
 
 
 class JobQueue(Queue[Tuple[Any, Sequence[Any], Mapping[str, Any]]]):
     """JobQueue extends threading.Queue, overriding its 'put' method to accept a generic list of arguments."""
 
     def put(self, func: Any, *args: Any, **kwargs: Any):  # pyright: ignore
-        """Puts a callable object (function) in the JobQueue.
+        """Put a callable object (function) in the JobQueue.
 
         Additional positional and keyword arguments provided with *args and *kwargs
         will be passed forward to the called function.
 
         Parameters
         ----------
         func : Any
@@ -24,29 +24,29 @@
 
 
 class Worker(Thread):
     """Worker thread executing jobs from a job queue."""
 
     # Override constructor of Thread class
     def __init__(self, job_queue: JobQueue):
-        """Instantiates a Worker and binds it to the passed in JobQueue instance.
+        """Instantiate a Worker and bind it to the passed in JobQueue instance.
 
         Parameters
         ----------
         job_queue : JobQueue
             the JobQueue this Worker shall be bound to
         """
         Thread.__init__(self)  # invoke base class constructor
         self.job_queue: JobQueue = job_queue
         self.daemon: bool = True
         self.start()
 
     # Override run() method of Thread class
     def run(self):
-        """Runs the next job from the JobQueue this Worker is bound to."""
+        """Run the next job from the JobQueue this Worker is bound to."""
         while True:
             try:
                 func, args, kwargs = self.job_queue.get()
                 func(*args, **kwargs)
             except Exception:
                 logger.exception("Worker: Exeption raised in worker thread.")
             finally:
```

### Comparing `farn-0.3.1/src/farn/sampling/sampling.py` & `farn-0.3.2/src/farn/sampling/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 class DiscreteSampling:
     """Class providing methods to run a discrete sampling of a specific layer,
     i.e. of all variables defined in the given layer.
     """
 
     def __init__(self):
-
         self.layer_name: str = ""
         self.sampling_parameters: Mapping[str, Any] = {}
         self.fields: List[str] = []
         self.values: List[Sequence[Any]] = []
         self.ranges: Sequence[Sequence[Any]] = []
         self.boundingBox: List[List[float]] = []
         self.minVals: List[Any] = []
@@ -81,15 +80,15 @@
             #         "_sigma",  # 2nd order
             #         "_includeBoundingBox",
             #     ]
             # },
         }
 
     def set_sampling_type(self, sampling_type: str):
-        """Sets the sampling type.
+        """Set the sampling type.
 
         Valid values:
             "fixed"
             "linSpace"
             "uniformLhs"
             "normalLhs"
             "sobol"
@@ -102,15 +101,15 @@
             exit(1)
 
     def set_sampling_parameters(
         self,
         sampling_parameters: Mapping[str, Any],
         layer_name: str = "",
     ):
-        """Sets the sampling parameters.
+        """Set the sampling parameters.
 
         The passed-in sampling parameters will be validated.
         Upon successful validation, the sampling is configured using the provided parameters.
         """
 
         self.layer_name = layer_name
         self.sampling_parameters = sampling_parameters
@@ -139,15 +138,15 @@
             self.ranges = self.sampling_parameters["_ranges"]
 
         # extra bounding box samples are not treated by lhs algorithm, however part of the lists
         self.number_of_samples = 0
         self.number_of_bb_samples = 0
 
     def generate_samples(self) -> Dict[str, List[Any]]:
-        """Returns a dict with all generated samples for the layer this sampling is run on.
+        """Return a dict with all generated samples for the layer this sampling is run on.
 
         The first element in the returned dict contains the case names generated.
         All following elements (second to last) contain the values sampled for each variable defined in the layer this sampling is run on.
         I.e.
         "names": (case_name_1, case_name_2, .., case_name_n)
         "variable_1": (value_1, value_2, .., value_n)
         ...
@@ -252,15 +251,15 @@
 
         for index, _ in enumerate(self.fields):
             samples[self.fields[index]] = values[index].tolist()
 
         return samples
 
     def _generate_samples_using_normal_lhs_sampling(self) -> Dict[str, List[Any]]:
-        """lhs using gaussian normal dstributions
+        """LHS using gaussian normal dstributions
         required input arguments:
         * _names: required names template
         * _numberOfSamples: required how many samples
         * _mu: required absolute location vector of distribution center point (origin)
         * _sigma: variation (vector), or required scalar, optional vector, optional cov
         or
         NOT IMPLEMENTED, DOES NOT MAKE MUCH SENSE!
@@ -369,18 +368,18 @@
             "bounds": self.ranges,
         }
 
         sample_set: ndarray[Any, Any] = latin.sample(  # type: ignore
             problem, self.number_of_samples - self.number_of_bb_samples
         )
 
-        return sample_set.T
+        return sample_set.T  # pyright: ignore
 
     def _generate_values_using_normal_lhs_sampling(self) -> ndarray[Any, Any]:
-        """gaussnormal lhs."""
+        """Gaussnormal LHS."""
         from pyDOE2 import lhs
         from scipy.stats import norm  # qmc, truncnorm
 
         lhs_distribution: Union[ndarray[Any, Any], None] = lhs(
             self.number_of_fields,
             samples=self.number_of_samples - self.number_of_bb_samples,
             criterion="corr",
@@ -394,15 +393,15 @@
 
         # std of type scalar (scale) or vector (stretch, scale), no rotation
         _std: ndarray[Any, Any] = np.array(self.std)
 
         sample_set: ndarray[Any, Any] = norm(loc=self.mean, scale=_std).ppf(lhs_distribution)  # type: ignore
 
         # transpose to be aligned with uniformLhs output
-        return sample_set.T
+        return sample_set.T  # pyright: ignore
 
     def _generate_values_using_sobol_sampling(self) -> ndarray[Any, Any]:
         # @TODO: Should be reimplemented using the scipy.stats.qmc.sobol
         #        https://scipy.github.io/devdocs/reference/generated/scipy.stats.qmc.Sobol.html#scipy-stats-qmc-sobol
         #        This to substitute the sobol-seq package, which is no longer maintained.
         #        (See https://github.com/naught101/sobol_seq)
         #        CLAROS, 2022-05-27
@@ -471,20 +470,20 @@
             if isinstance(item, Iterable):
                 self.boundingBox.append(list(self._flatten(item)))
             else:
                 self.boundingBox.append([item])
         return
 
     def _flatten(self, iterable: Sequence[Any]) -> Generator[Any, Any, Any]:
-        """flattens sequence... happens why?."""
+        """Flattens sequence... happens why?."""
         for element in iterable:
             if isinstance(element, Sequence) and not isinstance(element, (str, bytes)):
                 yield from self._flatten(element)
             else:
                 yield element
 
     def _min_max_scale(self, field: ndarray[Any, Any], range: Sequence[float]) -> ndarray[Any, Any]:
-        """might belong to different class in future
+        """Might belong to different class in future
         from sklearn.preprocessing import minmax_scale.
         """
         scale = (range[1] - range[0]) / (field.max(axis=0) - field.min(axis=0))  # type: ignore
         return scale * field + range[0] - field.min(axis=0) * scale  # type: ignore
```

### Comparing `farn-0.3.1/src/farn/utils/logging.py` & `farn-0.3.2/src/farn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.1/src/farn.egg-info/PKG-INFO` & `farn-0.3.2/src/farn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.1
+Version: 0.3.2
 Summary: n-dimensional case generator.
 Home-page: https://dnv-opensource.github.io/farn/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/farn
 Platform: Python3.x
 Classifier: Development Status :: 4 - Beta
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
@@ -125,15 +126,15 @@
     Install farn's dependencies:
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

### Comparing `farn-0.3.1/src/farn.egg-info/SOURCES.txt` & `farn-0.3.2/src/farn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 src/farn/run/cli/batchProcess.py
 src/farn/run/utils/__init__.py
 src/farn/run/utils/threading.py
 src/farn/sampling/__init__.py
 src/farn/sampling/sampling.py
 src/farn/utils/__init__.py
 src/farn/utils/logging.py
-src/farn/utils/os.py
+src/farn/utils/os.py
+tests/test_cases.py
+tests/test_farn.py
```

