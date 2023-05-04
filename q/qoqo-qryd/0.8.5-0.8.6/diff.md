# Comparing `tmp/qoqo_qryd-0.8.5.tar.gz` & `tmp/qoqo_qryd-0.8.6.tar.gz`

## Comparing `qoqo_qryd-0.8.5.tar` & `qoqo_qryd-0.8.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/LICENSE
--rw-r--r--   0     1001      123     3716 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/README.md
--rw-r--r--   0     1001      123    44177 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/api_backend.rs
--rw-r--r--   0     1001      123    43360 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/api_devices.rs
--rw-r--r--   0     1001      123     4485 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/lib.rs
--rw-r--r--   0     1001      123     6195 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/pragma_operations.rs
--rw-r--r--   0     1001      123    30758 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/qryd_devices.rs
--rw-r--r--   0     1001      123     2510 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/simulator_backend.rs
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.5/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/LICENSE
--rw-r--r--   0     1001      123     4917 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/README.md
--rw-r--r--   0     1001      123     1035 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/examples/README.md
--rw-r--r--   0     1001      123      570 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/pyproject.toml
--rw-r--r--   0     1001      123     1602 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/BSD_LICENSE
--rw-r--r--   0     1001      123  2610151 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/DEPENDENCIES
--rw-r--r--   0     1001      123    36463 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      123     1065 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/MIT_LICENSE
--rw-r--r--   0     1001      123     6119 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/OPENSSLLICENSE
--rw-r--r--   0     1001      123     2404 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/PYTHON_LICENSE
--rw-r--r--   0     1001      123      931 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/qoqo_qryd/__init__.py
--rw-r--r--   0     1001      123    20073 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/api_backend.rs
--rw-r--r--   0     1001      123    27992 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/api_devices.rs
--rw-r--r--   0     1001      123     3860 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/lib.rs
--rw-r--r--   0     1001      123    20306 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/pragma_operations.rs
--rw-r--r--   0     1001      123    19868 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/qryd_devices.rs
--rw-r--r--   0     1001      123    14989 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/src/simulator_backend.rs
--rw-r--r--   0     1001      123    64584 2023-04-06 17:53:18.000000 qoqo_qryd-0.8.5/Cargo.lock
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/LICENSE
+-rw-r--r--   0     1001      123     3716 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/README.md
+-rw-r--r--   0     1001      123    44177 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/api_backend.rs
+-rw-r--r--   0     1001      123    43360 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/api_devices.rs
+-rw-r--r--   0     1001      123     4485 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/lib.rs
+-rw-r--r--   0     1001      123     6195 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/pragma_operations.rs
+-rw-r--r--   0     1001      123    30758 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/qryd_devices.rs
+-rw-r--r--   0     1001      123     2510 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/simulator_backend.rs
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.6/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/LICENSE
+-rw-r--r--   0     1001      123     4917 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/README.md
+-rw-r--r--   0     1001      123     1035 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/examples/README.md
+-rw-r--r--   0     1001      123      570 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/pyproject.toml
+-rw-r--r--   0     1001      123     1602 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/BSD_LICENSE
+-rw-r--r--   0     1001      123  2610151 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/DEPENDENCIES
+-rw-r--r--   0     1001      123    36463 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      123     1065 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/MIT_LICENSE
+-rw-r--r--   0     1001      123     6119 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/OPENSSLLICENSE
+-rw-r--r--   0     1001      123     2404 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/PYTHON_LICENSE
+-rw-r--r--   0     1001      123      931 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/qoqo_qryd/__init__.py
+-rw-r--r--   0     1001      123    20073 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/api_backend.rs
+-rw-r--r--   0     1001      123    27992 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/api_devices.rs
+-rw-r--r--   0     1001      123     3860 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/lib.rs
+-rw-r--r--   0     1001      123    20306 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/pragma_operations.rs
+-rw-r--r--   0     1001      123    19868 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/qryd_devices.rs
+-rw-r--r--   0     1001      123    14989 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/src/simulator_backend.rs
+-rw-r--r--   0     1001      123    64609 2023-05-04 09:04:53.000000 qoqo_qryd-0.8.6/Cargo.lock
+-rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 qoqo_qryd-0.8.6/PKG-INFO
```

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/Cargo.toml` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo-qryd"
-version = "0.8.5"
+version = "0.8.6"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 edition = "2021"
 license = "Apache-2.0"
 rust-version = "1.56"
 categories = ["science", "simulation"]
 readme = "../README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qryd"
@@ -18,18 +18,18 @@
 name = "roqoqo_qryd"
 path = "src/lib.rs"
 doctest = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-roqoqo = {package = "roqoqo", version="1.3", features=["serialize"]}
+roqoqo = {package = "roqoqo", version="1.4", features=["serialize"]}
 # roqoqo_1_0 = {package = "roqoqo", version="=1.0.0", features=["serialize"], optional=true}
 # roqoqo_1_0 = {package = "roqoqo", version="1.0.0", git = 'https://github.com/HQSquantumsimulations/qoqo', tag="v1.0.0", features=["serialize"], optional=true}
-roqoqo-derive = {package="roqoqo-derive", version="1.3"}
+roqoqo-derive = {package="roqoqo-derive", version="1.4"}
 roqoqo-quest = {version = "0.10", default-features=false, optional=true}
 qoqo_calculator = { version="1.1"}
 serde = {version="1.0", features=["derive"], optional=true}
 serde_json = "1.0"
 ndarray= {version="0.15"}
 bincode = "1.3"
 reqwest = {version="0.11", features = ["json", "blocking", "native-tls-vendored"], optional=true}
```

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/LICENSE` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/README.md` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/api_backend.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/api_backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/api_devices.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/api_devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/lib.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/pragma_operations.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/pragma_operations.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/qryd_devices.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/qryd_devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/local_dependencies/roqoqo-qryd/src/simulator_backend.rs` & `qoqo_qryd-0.8.6/local_dependencies/roqoqo-qryd/src/simulator_backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/Cargo.toml` & `qoqo_qryd-0.8.6/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo-qryd"
-version = "0.8.5"
+version = "0.8.6"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 edition = "2021"
 license = "Apache-2.0"
 rust-version = "1.56"
 categories = ["science", "simulation"]
 readme = "README.md"
 homepage = "https://github.com/HQSquantumsimulations/qoqo_qryd"
@@ -28,20 +28,20 @@
 [dependencies]
 serde = { version = "1.0", features = ["derive"] }
 qoqo_calculator = {version="1.1"}
 numpy = "0.18"
 
 qoqo_calculator_pyo3 = {version="1.1", default-features=false}
 
-qoqo = {package="qoqo", version="1.3", default-features=false}
+qoqo = {package="qoqo", version="1.4", default-features=false}
 
-roqoqo = {package="roqoqo", version="1.3", features = ["serialize"]}
+roqoqo = {package="roqoqo", version="1.4", features = ["serialize"]}
 
 ndarray = "0.15"
-roqoqo-qryd = {version="0.8.5", path= "local_dependencies/roqoqo-qryd", default-features=false, features = ["serialize"]}
+roqoqo-qryd = {version="0.8.6", path= "local_dependencies/roqoqo-qryd", default-features=false, features = ["serialize"]}
 bincode = "1.3"
 serde_json = "1.0"
 
 [build-dependencies]
 pyo3-build-config = "0.18"
 
 [features]
```

### Comparing `qoqo_qryd-0.8.5/LICENSE` & `qoqo_qryd-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/README.md` & `qoqo_qryd-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/examples/README.md` & `qoqo_qryd-0.8.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/pyproject.toml` & `qoqo_qryd-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "qoqo_qryd"
-version = "0.8.5"
+version = "0.8.6"
 dependencies = [
   'numpy',
-  'qoqo>=1.3',
+  'qoqo>=1.4',
   'qoqo_calculator_pyo3>=1.1',
 ]
 license = {text="Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016 AND BSD-2-Clause AND BSD-3-CLause"}
 maintainers = [{name = "HQS Quantum Simulations GmbH", email = "info@quantumsimulations.de"}]
 requires-python = ">=3.7"
 
 [build-system]
```

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/BSD_LICENSE` & `qoqo_qryd-0.8.6/qoqo_qryd/BSD_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/DEPENDENCIES` & `qoqo_qryd-0.8.6/qoqo_qryd/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -91489,15 +91489,15 @@
 00165600: 796f 7572 2061 6363 6570 7469 6e67 2061  your accepting a
 00165610: 6e79 2073 7563 6820 7761 7272 616e 7479  ny such warranty
 00165620: 206f 7220 6164 6469 7469 6f6e 616c 206c   or additional l
 00165630: 6961 6269 6c69 7479 2e0a 0a0a 3d3d 3d3d  iability....====
 00165640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00165650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00165660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00165670: 0a71 6f71 6f20 312e 332e 320a 6874 7470  .qoqo 1.3.2.http
+00165670: 0a71 6f71 6f20 312e 342e 300a 6874 7470  .qoqo 1.4.0.http
 00165680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f48  s://github.com/H
 00165690: 5153 7175 616e 7475 6d73 696d 756c 6174  QSquantumsimulat
 001656a0: 696f 6e73 2f71 6f71 6f0a 6279 2048 5153  ions/qoqo.by HQS
 001656b0: 2051 7561 6e74 756d 2053 696d 756c 6174   Quantum Simulat
 001656c0: 696f 6e73 203c 696e 666f 4071 7561 6e74  ions <info@quant
 001656d0: 756d 7369 6d75 6c61 7469 6f6e 732e 6465  umsimulations.de
 001656e0: 3e0a 5175 616e 7475 6d20 636f 6d70 7574  >.Quantum comput
@@ -92219,15 +92219,15 @@
 001683a0: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
 001683b0: 616e 640a 2020 206c 696d 6974 6174 696f  and.   limitatio
 001683c0: 6e73 2075 6e64 6572 2074 6865 204c 6963  ns under the Lic
 001683d0: 656e 7365 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d  ense....========
 001683e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001683f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00168400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a71 6f71  ============.qoq
-00168410: 6f2d 6d61 6372 6f73 2031 2e33 2e32 0a62  o-macros 1.3.2.b
+00168410: 6f2d 6d61 6372 6f73 2031 2e34 2e30 0a62  o-macros 1.4.0.b
 00168420: 7920 4851 5320 5175 616e 7475 6d20 5369  y HQS Quantum Si
 00168430: 6d75 6c61 7469 6f6e 7320 3c69 6e66 6f40  mulations <info@
 00168440: 7175 616e 7475 6d73 696d 756c 6174 696f  quantumsimulatio
 00168450: 6e73 2e64 653e 0a4d 6163 726f 7320 666f  ns.de>.Macros fo
 00168460: 7220 7468 6520 716f 716f 2063 7261 7465  r the qoqo crate
 00168470: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
 00168480: 2d32 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  -2.0.-----------
@@ -92944,15 +92944,15 @@
 0016b0f0: 6e69 6e67 2070 6572 6d69 7373 696f 6e73  ning permissions
 0016b100: 2061 6e64 0a20 2020 6c69 6d69 7461 7469   and.   limitati
 0016b110: 6f6e 7320 756e 6465 7220 7468 6520 4c69  ons under the Li
 0016b120: 6365 6e73 652e 0a0a 0a3d 3d3d 3d3d 3d3d  cense....=======
 0016b130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0016b140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0016b150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 716f  =============.qo
-0016b160: 716f 2d71 7279 6420 302e 382e 350a 6874  qo-qryd 0.8.5.ht
+0016b160: 716f 2d71 7279 6420 302e 382e 360a 6874  qo-qryd 0.8.6.ht
 0016b170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 0016b180: 2f48 5153 7175 616e 7475 6d73 696d 756c  /HQSquantumsimul
 0016b190: 6174 696f 6e73 2f71 6f71 6f5f 7172 7964  ations/qoqo_qryd
 0016b1a0: 0a62 7920 4851 5320 5175 616e 7475 6d20  .by HQS Quantum 
 0016b1b0: 5369 6d75 6c61 7469 6f6e 7320 3c69 6e66  Simulations <inf
 0016b1c0: 6f40 7175 616e 7475 6d73 696d 756c 6174  o@quantumsimulat
 0016b1d0: 696f 6e73 2e64 653e 0a51 5279 6420 6261  ions.de>.QRyd ba
@@ -103129,15 +103129,15 @@
 00192d80: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
 00192d90: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
 00192da0: 414c 494e 4753 2049 4e0a 5448 4520 534f  ALINGS IN.THE SO
 00192db0: 4654 5741 5245 2e0a 0a0a 0a3d 3d3d 3d3d  FTWARE.....=====
 00192dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00192dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00192de0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00192df0: 726f 716f 716f 2031 2e33 2e32 0a68 7474  roqoqo 1.3.2.htt
+00192df0: 726f 716f 716f 2031 2e34 2e30 0a68 7474  roqoqo 1.4.0.htt
 00192e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00192e10: 4851 5371 7561 6e74 756d 7369 6d75 6c61  HQSquantumsimula
 00192e20: 7469 6f6e 732f 716f 716f 0a62 7920 4851  tions/qoqo.by HQ
 00192e30: 5320 5175 616e 7475 6d20 5369 6d75 6c61  S Quantum Simula
 00192e40: 7469 6f6e 7320 3c69 6e66 6f40 7175 616e  tions <info@quan
 00192e50: 7475 6d73 696d 756c 6174 696f 6e73 2e64  tumsimulations.d
 00192e60: 653e 0a52 7573 7420 5175 616e 7475 6d20  e>.Rust Quantum 
@@ -103858,15 +103858,15 @@
 00195b10: 6d69 7373 696f 6e73 2061 6e64 0a20 2020  missions and.   
 00195b20: 6c69 6d69 7461 7469 6f6e 7320 756e 6465  limitations unde
 00195b30: 7220 7468 6520 4c69 6365 6e73 652e 0a0a  r the License...
 00195b40: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
 00195b50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00195b60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00195b70: 3d3d 3d3d 3d0a 726f 716f 716f 2d64 6572  =====.roqoqo-der
-00195b80: 6976 6520 312e 332e 320a 6279 2048 5153  ive 1.3.2.by HQS
+00195b80: 6976 6520 312e 342e 300a 6279 2048 5153  ive 1.4.0.by HQS
 00195b90: 2051 7561 6e74 756d 2053 696d 756c 6174   Quantum Simulat
 00195ba0: 696f 6e73 203c 696e 666f 4071 7561 6e74  ions <info@quant
 00195bb0: 756d 7369 6d75 6c61 7469 6f6e 732e 6465  umsimulations.de
 00195bc0: 3e0a 4d61 6372 6f73 2066 6f72 2074 6865  >.Macros for the
 00195bd0: 2072 6f71 6f71 6f20 6372 6174 650a 4c69   roqoqo crate.Li
 00195be0: 6365 6e73 653a 2041 7061 6368 652d 322e  cense: Apache-2.
 00195bf0: 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  0.--------------
@@ -104583,15 +104583,15 @@
 00198860: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
 00198870: 640a 2020 206c 696d 6974 6174 696f 6e73  d.   limitations
 00198880: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
 00198890: 7365 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  se....==========
 001988a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001988b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001988c0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a72 6f71 6f71  ==========.roqoq
-001988d0: 6f2d 7172 7964 2030 2e38 2e35 0a68 7474  o-qryd 0.8.5.htt
+001988d0: 6f2d 7172 7964 2030 2e38 2e36 0a68 7474  o-qryd 0.8.6.htt
 001988e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 001988f0: 4851 5371 7561 6e74 756d 7369 6d75 6c61  HQSquantumsimula
 00198900: 7469 6f6e 732f 716f 716f 5f71 7279 640a  tions/qoqo_qryd.
 00198910: 6279 2048 5153 2051 7561 6e74 756d 2053  by HQS Quantum S
 00198920: 696d 756c 6174 696f 6e73 203c 696e 666f  imulations <info
 00198930: 4071 7561 6e74 756d 7369 6d75 6c61 7469  @quantumsimulati
 00198940: 6f6e 732e 6465 3e0a 5152 7964 2069 6e74  ons.de>.QRyd int
@@ -106043,15 +106043,15 @@
 0019e3a0: 726d 6973 7369 6f6e 7320 616e 640a 2020  rmissions and.  
 0019e3b0: 206c 696d 6974 6174 696f 6e73 2075 6e64   limitations und
 0019e3c0: 6572 2074 6865 204c 6963 656e 7365 2e0a  er the License..
 0019e3d0: 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
 0019e3e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0019e3f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0019e400: 3d3d 3d3d 3d3d 0a72 6f71 6f71 6f2d 7465  ======.roqoqo-te
-0019e410: 7374 2031 2e33 2e32 0a68 7474 7073 3a2f  st 1.3.2.https:/
+0019e410: 7374 2031 2e34 2e30 0a68 7474 7073 3a2f  st 1.4.0.https:/
 0019e420: 2f67 6974 6875 622e 636f 6d2f 4851 5371  /github.com/HQSq
 0019e430: 7561 6e74 756d 7369 6d75 6c61 7469 6f6e  uantumsimulation
 0019e440: 732f 716f 716f 0a62 7920 4851 5320 5175  s/qoqo.by HQS Qu
 0019e450: 616e 7475 6d20 5369 6d75 6c61 7469 6f6e  antum Simulation
 0019e460: 7320 3c69 6e66 6f40 7175 616e 7475 6d73  s <info@quantums
 0019e470: 696d 756c 6174 696f 6e73 2e64 653e 0a54  imulations.de>.T
 0019e480: 6573 7469 6e67 2068 656c 7065 7220 6675  esting helper fu
```

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo_qryd-0.8.6/qoqo_qryd/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/MIT_LICENSE` & `qoqo_qryd-0.8.6/qoqo_qryd/MIT_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/OPENSSLLICENSE` & `qoqo_qryd-0.8.6/qoqo_qryd/OPENSSLLICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/PYTHON_LICENSE` & `qoqo_qryd-0.8.6/qoqo_qryd/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/qoqo_qryd/__init__.py` & `qoqo_qryd-0.8.6/qoqo_qryd/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/api_backend.rs` & `qoqo_qryd-0.8.6/src/api_backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/api_devices.rs` & `qoqo_qryd-0.8.6/src/api_devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/lib.rs` & `qoqo_qryd-0.8.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/pragma_operations.rs` & `qoqo_qryd-0.8.6/src/pragma_operations.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/qryd_devices.rs` & `qoqo_qryd-0.8.6/src/qryd_devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/src/simulator_backend.rs` & `qoqo_qryd-0.8.6/src/simulator_backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qryd-0.8.5/Cargo.lock` & `qoqo_qryd-0.8.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "approx"
 version = "0.5.1"
@@ -48,17 +48,17 @@
  "concurrent-queue",
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17adb73da160dfb475c183343c8cccd80721ea5a605d3eb57125f0a7b7a92d0b"
+checksum = "6fa3dc5f2a8564f07759c008b9109dc0d39de92a88d5588b8a5036d286383afb"
 dependencies = [
  "async-lock",
  "async-task",
  "concurrent-queue",
  "fastrand",
  "futures-lite",
  "slab",
@@ -115,28 +115,28 @@
 checksum = "aeb901c30ebc2fc4ab46395bbfbdba9542c16559d853645d75190c3056caf3bc"
 dependencies = [
  "async-std",
 ]
 
 [[package]]
 name = "async-process"
-version = "1.6.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6381ead98388605d0d9ff86371043b5aa922a3905824244de40dc263a14fcba4"
+checksum = "7a9d28b1d97e08915212e2e45310d47854eafa69600756fc735fb788f75199c9"
 dependencies = [
  "async-io",
  "async-lock",
  "autocfg",
  "blocking",
  "cfg-if",
  "event-listener",
  "futures-lite",
- "libc",
+ "rustix",
  "signal-hook",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-std"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
@@ -172,22 +172,22 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "atomic-waker"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "debc29dde2e69f9e47506b525f639ed42300fc014a3e007832592448fa8e4599"
+checksum = "1181e1e0d1fce796a03db1ae795d67167da795f9cf4a39c37589e85ef57f26d3"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -254,31 +254,32 @@
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c67b173a56acffd6d2326fb7ab938ba0b00a71480e14902b2591c87bc5741e8"
+checksum = "77231a1c8f801696fc0123ec6150ce92cffb8e164a02afb9c8ddee0e9b65ad65"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-task",
  "atomic-waker",
  "fastrand",
  "futures-lite",
+ "log",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
@@ -304,17 +305,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "concurrent-queue"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
@@ -436,21 +437,21 @@
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -535,17 +536,17 @@
 name = "futures-io"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
+checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
  "fastrand",
  "futures-core",
  "futures-io",
  "memchr",
  "parking",
  "pin-project-lite",
@@ -556,15 +557,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -589,17 +590,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -612,17 +613,17 @@
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.16"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -720,17 +721,17 @@
  "similar",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "hyper"
-version = "0.14.25"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc5e554ff619822309ffd57d8734d77cd5ce6238bc956f037ea06c58238c9899"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -809,22 +810,22 @@
 name = "ipnet"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "256017f749ab3117e93acb91063009e1f1bb56d03965b14c2c8df4eb02c524d8"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "isahc"
 version = "1.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "334e04b4d781f436dc315cb1e7515bd96826426345d498149e4bde36b67f8ee9"
@@ -881,40 +882,39 @@
 checksum = "0de8b303297635ad57c9f5059fd9cee7a47f8e8daa09df0fcd07dd39fb22977f"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "lalrpop"
-version = "0.19.9"
+version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f34313ec00c2eb5c3c87ca6732ea02dcf3af99c3ff7a8fb622ffb99c9d860a87"
+checksum = "0a1cbf952127589f2851ab2046af368fd20645491bb4b376f04b7f94d7a9837b"
 dependencies = [
  "ascii-canvas",
  "bit-set",
  "diff",
  "ena",
  "is-terminal",
  "itertools",
  "lalrpop-util",
  "petgraph",
- "pico-args",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "string_cache",
  "term",
  "tiny-keccak",
  "unicode-xid",
 ]
 
 [[package]]
 name = "lalrpop-util"
-version = "0.19.9"
+version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5c1f7869c94d214466c5fd432dfed12c379fd87786768d36455892d46b18edd"
+checksum = "d3c48237b9604c5a4702de6b824e02006c3214327564636aef27c1028a8fa0ed"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -925,17 +925,17 @@
 name = "levenshtein"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db13adb97ab515a3691f56e4dbab09283d0b86cb45abd991d8634a9d6f501760"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -947,29 +947,29 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.1"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d59d8c75012853d2e872fb56bc8a2e53718e2cafe1a4c823143141c6d90c322f"
+checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -985,18 +985,19 @@
 dependencies = [
  "cfg-if",
  "value-bag",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1164,17 +1165,17 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.49"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d2f106ab837a24e03672c59b1239669a0596406ff657c3c0835b6b7f0f35a33"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1185,50 +1186,50 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.2+1.1.1t"
+version = "111.25.3+1.1.1t"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "320708a054ad9b3bf314688b5db87cf4d6683d64cfc835e2337924ae62bf4431"
+checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.84"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a20eace9dc2d82904039cb76dcf50fb1a0bba071cfd1629720b5d6f1ddba0fa"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "parking"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
+checksum = "14f2252c834a40ed9bb5422029649578e63aa341ac401f74e719dd1afda8394e"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -1279,20 +1280,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
-name = "pico-args"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db8bcd96cb740d03149cbad5518db9fd87126a10ab519c011893b1754134c468"
-
-[[package]]
 name = "pin-project"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
 dependencies = [
  "pin-project-internal",
 ]
@@ -1324,26 +1319,26 @@
 name = "pkg-config"
 version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
 
 [[package]]
 name = "polling"
-version = "2.6.0"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e1f879b2998099c2d69ab9605d145d5b661195627eccc680002c4918a7fb6fa"
+checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
  "autocfg",
  "bitflags",
  "cfg-if",
  "concurrent-queue",
  "libc",
  "log",
  "pin-project-lite",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
@@ -1385,17 +1380,17 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "num-complex",
  "parking_lot",
@@ -1403,60 +1398,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "qoqo"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650bc9a0407f82225893cf52cd75e5b8bf3ba9281024b3a32d5bc3bbdf79b03d"
+checksum = "bf07f3e506270363fc27cd0d64d6a731e16bb541aefe5d6ada33a5eae988abff"
 dependencies = [
  "bincode",
  "ndarray",
  "num-complex",
  "numpy",
  "proc-macro2",
  "pyo3",
@@ -1464,32 +1459,32 @@
  "qoqo-macros",
  "qoqo_calculator",
  "qoqo_calculator_pyo3",
  "quote",
  "roqoqo",
  "serde",
  "serde_json",
- "syn 2.0.13",
+ "syn 2.0.15",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo-macros"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d54feb7ef7d29f95da7bc4261f619092f6ae26281528d83af641df6ac9cfa6e"
+checksum = "d92049ac4baa56a91d6d349714192e8ccb48cbceab7c0ed01a225442e950e492"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "qoqo-qryd"
-version = "0.8.5"
+version = "0.8.6"
 dependencies = [
  "bincode",
  "httpmock",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-build-config",
@@ -1526,17 +1521,17 @@
  "qoqo_calculator",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "quest-sys"
-version = "0.10.0"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c5eb48e6cc892b14aa1f11a4d35d0a1f29e1e18a5928c92c4c097811b7cb7a3"
+checksum = "d0a3b126cb0c2e558ec18bd695792f0879e968d99ae53b4c9f0c37b13fe165a6"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
@@ -1625,34 +1620,40 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
+name = "regex-syntax"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+
+[[package]]
 name = "reqwest"
-version = "0.11.16"
+version = "0.11.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27b71749df584b7f4cac2c426c127a7c785a5106cc98f7a8feb044115f0fa254"
+checksum = "13293b639a097af28fc8a90f22add145a9c954e49d77da06263d58cf44d5fb91"
 dependencies = [
  "base64 0.21.0",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -1679,48 +1680,48 @@
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "roqoqo"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "872066bed44102ab2b010ecdd846ee58165e36c3b96588e929cff7f903c760ce"
+checksum = "64df85d14e330f6ecb7736ef2251cbd86508c50a2edda310edc23054caa76822"
 dependencies = [
  "bincode",
  "nalgebra",
  "ndarray",
  "num-complex",
  "petgraph",
  "proc-macro2",
  "qoqo_calculator",
  "quote",
  "rand",
  "rand_distr",
  "roqoqo-derive",
  "serde",
- "syn 2.0.13",
+ "syn 2.0.15",
  "thiserror",
 ]
 
 [[package]]
 name = "roqoqo-derive"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef32f1343b1e924b2d5ecf057e3ee3d7f2f7834c7bd75e398aa73c7c8e72de4"
+checksum = "74660c4266cc53915499961c19a15e7e558dcce5c39a0c4ea1f3ad41e0dbab44"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "roqoqo-qryd"
-version = "0.8.5"
+version = "0.8.6"
 dependencies = [
  "bincode",
  "bitvec",
  "hex",
  "httpmock",
  "itertools",
  "ndarray",
@@ -1735,61 +1736,61 @@
  "serde_json",
  "serde_test",
  "test-case",
 ]
 
 [[package]]
 name = "roqoqo-quest"
-version = "0.10.0"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c9563627bd1e326b4f745442c55ba4bf725c29528c3f8540df8db168599bdcf"
+checksum = "55b3b2f3ae571419d3d3ced870ddfcda743c8b66dbd4751bb588fc0251f0e373"
 dependencies = [
  "ndarray",
  "num-complex",
  "qoqo_calculator",
  "quest-sys",
  "rand",
  "roqoqo",
  "serde",
 ]
 
 [[package]]
 name = "roqoqo-test"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43a372525057417f40cae9c83f0d73ce6de191b5f9196d0f66e43f8d036b43bf"
+checksum = "3ee833385ef9bef941aaa777026e251128d7ef0a28947f1c1ec326a8e07b6323"
 dependencies = [
  "nalgebra",
  "ndarray",
  "proc-macro2",
  "qoqo_calculator",
  "quote",
  "rand",
  "roqoqo",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.7"
+version = "0.37.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aae838e49b3d63e9274e1c01833cc8139d3fec468c3b84688c628f44b1ae11d"
+checksum = "8bbfc1d1c7c40c01715f47d71444744a81669ca84e8b63e25a55e169b1f86433"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
@@ -1845,37 +1846,37 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1886,17 +1887,17 @@
 dependencies = [
  "regex",
  "serde",
 ]
 
 [[package]]
 name = "serde_test"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f259aa64e48efaf5a4fea11f97cacb109f7fc3ae9db7244cbb40c01c7faf42bc"
+checksum = "3c95a500e3923258f7fc3a16bf29934e403aef5ca1096e184d85e3b1926675e8"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -1926,17 +1927,17 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simba"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50582927ed6f77e4ac020c057f37a268fc6aebc29225050365aacbb9deeeddc4"
+checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
  "num-traits",
  "paste",
  "wide",
 ]
@@ -2011,34 +2012,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
@@ -2095,15 +2096,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
@@ -2124,56 +2125,56 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -2196,21 +2197,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
```

### Comparing `qoqo_qryd-0.8.5/PKG-INFO` & `qoqo_qryd-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qoqo_qryd
-Version: 0.8.5
+Version: 0.8.6
 Requires-Dist: numpy
-Requires-Dist: qoqo>=1.3
+Requires-Dist: qoqo>=1.4
 Requires-Dist: qoqo_calculator_pyo3>=1.1
 License-File: LICENSE
 Summary: QRyd backend for qoqo quantum computing toolkit
 Home-Page: https://github.com/HQSquantumsimulations/qoqo_qryd
 Author: HQS Quantum Simulations <info@quantumsimulations.de>
 Author-email: HQS Quantum Simulations <info@quantumsimulations.de>
 Maintainer-email: HQS Quantum Simulations GmbH <info@quantumsimulations.de>
```

