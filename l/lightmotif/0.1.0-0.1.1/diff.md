# Comparing `tmp/lightmotif-0.1.0.tar.gz` & `tmp/lightmotif-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightmotif-0.1.0.tar", last modified: Wed May  3 23:49:27 2023, max compression
+gzip compressed data, was "lightmotif-0.1.1.tar", last modified: Thu May  4 01:38:59 2023, max compression
```

## Comparing `lightmotif-0.1.0.tar` & `lightmotif-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.034422 lightmotif-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 23:49:23.000000 lightmotif-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-03 23:49:23.000000 lightmotif-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 23:49:23.000000 lightmotif-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-03 23:49:27.034422 lightmotif-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-03 23:49:23.000000 lightmotif-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.030422 lightmotif-0.1.0/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.034422 lightmotif-0.1.0/lightmotif/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/benches/ecoli.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.034422 lightmotif-0.1.0/lightmotif/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/abc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/dense.rs
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/err.rs
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/pli.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/pwm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/src/seq.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.034422 lightmotif-0.1.0/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif/tests/dna.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.030422 lightmotif-0.1.0/lightmotif-py/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.030422 lightmotif-0.1.0/lightmotif-py/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.030422 lightmotif-0.1.0/lightmotif-py/lightmotif/avx2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/avx2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.034422 lightmotif-0.1.0/lightmotif-py/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/tests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 23:49:23.000000 lightmotif-0.1.0/lightmotif-py/lightmotif/tests/unittest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:49:27.030422 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-03 23:49:27.000000 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 23:49:27.000000 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:49:27.000000 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 23:49:27.000000 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:49:27.000000 lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 23:49:26.000000 lightmotif-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-03 23:49:27.034422 lightmotif-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-03 23:49:23.000000 lightmotif-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 01:38:54.000000 lightmotif-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-04 01:38:54.000000 lightmotif-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 01:38:54.000000 lightmotif-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-04 01:38:59.253166 lightmotif-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-04 01:38:54.000000 lightmotif-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/benches/ecoli.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/lightmotif/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/abc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/dense.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/err.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/pli.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/pwm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/src/seq.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.253166 lightmotif-0.1.1/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif/tests/dna.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/arch/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/avx2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/avx2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/test_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-04 01:38:54.000000 lightmotif-0.1.1/lightmotif-py/lightmotif/tests/unittest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:38:59.249166 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:38:59.000000 lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 01:38:59.000000 lightmotif-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-04 01:38:59.253166 lightmotif-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-04 01:38:54.000000 lightmotif-0.1.1/setup.py
```

### Comparing `lightmotif-0.1.0/COPYING` & `lightmotif-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/PKG-INFO` & `lightmotif-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
```

### Comparing `lightmotif-0.1.0/README.md` & `lightmotif-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 *A lightweight [platform-accelerated](https://en.wikipedia.org/wiki/Single_instruction,_multiple_data) library for [biological motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning using [position weight matrices](https://en.wikipedia.org/wiki/Position_weight_matrix)*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/lightmotif/rust.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/lightmotif/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/lightmotif?logo=codecov&style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/lightmotif/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Crate](https://img.shields.io/crates/v/lightmotif.svg?maxAge=600&style=flat-square)](https://crates.io/crates/lightmotif)
+[![Docs](https://img.shields.io/docsrs/lightmotif?maxAge=600&style=flat-square)](https://docs.rs/lightmotif)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/lightmotif/)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/lightmotif.svg?style=flat-square&maxAge=600)](https://github.com/althonos/lightmotif/issues)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md)
 
 ## 🗺️ Overview
```

### Comparing `lightmotif-0.1.0/lightmotif/README.md` & `lightmotif-0.1.1/lightmotif/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 *A lightweight [platform-accelerated](https://en.wikipedia.org/wiki/Single_instruction,_multiple_data) library for [biological motif](https://en.wikipedia.org/wiki/Sequence_motif) scanning using [position weight matrices](https://en.wikipedia.org/wiki/Position_weight_matrix)*.
 
 [![Actions](https://img.shields.io/github/actions/workflow/status/althonos/lightmotif/rust.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/lightmotif/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/lightmotif?logo=codecov&style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/lightmotif/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![Crate](https://img.shields.io/crates/v/lightmotif.svg?maxAge=600&style=flat-square)](https://crates.io/crates/lightmotif)
+[![Docs](https://img.shields.io/docsrs/lightmotif?maxAge=600&style=flat-square)](https://docs.rs/lightmotif)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/lightmotif/)
 [![GitHub issues](https://img.shields.io/github/issues/althonos/lightmotif.svg?style=flat-square&maxAge=600)](https://github.com/althonos/lightmotif/issues)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md)
 
 ## 🗺️ Overview
```

### Comparing `lightmotif-0.1.0/lightmotif/benches/ecoli.rs` & `lightmotif-0.1.1/lightmotif/benches/ecoli.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/abc.rs` & `lightmotif-0.1.1/lightmotif/src/abc.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/dense.rs` & `lightmotif-0.1.1/lightmotif/src/dense.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/err.rs` & `lightmotif-0.1.1/lightmotif/src/err.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/lib.rs` & `lightmotif-0.1.1/lightmotif/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/pli.rs` & `lightmotif-0.1.1/lightmotif/src/pli.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/pwm.rs` & `lightmotif-0.1.1/lightmotif/src/pwm.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/src/seq.rs` & `lightmotif-0.1.1/lightmotif/src/seq.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif/tests/dna.rs` & `lightmotif-0.1.1/lightmotif/tests/dna.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif-py/Cargo.toml` & `lightmotif-0.1.1/lightmotif-py/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 [package]
 name = "lightmotif-py"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 edition = "2021"
 license = "MIT"
 description = "PyO3 bindings and Python interface to the lightmotif crate."
 repository = "https://github.com/althonos/lightmotif"
 homepage = "https://github.com/althonos/lightmotif"
 readme = "README.md"
 categories = ["science"]
 keywords = ["bioinformatics", "python", "bindings", "pssm"]
-build = "build.rs"
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 path = "lightmotif/lib.rs"
 
-[build-dependencies.built]
-version = "0.6"
-features = ["chrono"]
-[build-dependencies]
-project-root = "0.2.2"
-
 [dependencies.lightmotif]
 path = "../lightmotif"
-version = "0.1.0"
+version = "0.1.1"
 [dependencies]
 pyo3 = "0.18.3"
-pyo3-built = "0.4.7"
 
 [features]
 default = []
+built = []
 extension-module = ["pyo3/extension-module"]
 nightly = ["pyo3/nightly"]
 
 [[test]]
 name = "unittest"
 path = "lightmotif/tests/unittest.rs"
 harness = false
```

### Comparing `lightmotif-0.1.0/lightmotif-py/README.md` & `lightmotif-0.1.1/lightmotif-py/README.md`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif-py/lightmotif/lib.rs` & `lightmotif-0.1.1/lightmotif-py/lightmotif/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #![doc = include_str!("../README.md")]
 
-#[macro_use]
-extern crate pyo3_built;
 extern crate lightmotif;
 extern crate pyo3;
 
 #[cfg(target_feature = "avx2")]
 use std::arch::x86_64::__m256;
 #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
 use std::arch::x86_64::__m256i;
@@ -23,19 +21,14 @@
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_ssize_t;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use pyo3::types::PyString;
 use pyo3::AsPyPointer;
 
-#[allow(dead_code)]
-mod build {
-    include!(concat!(env!("OUT_DIR"), "/built.rs"));
-}
-
 // --- Compile-time constants --------------------------------------------------
 
 #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
 const C: usize = std::mem::size_of::<__m256i>();
 #[cfg(not(any(target_arch = "x86", target_arch = "x86_64")))]
 const C: usize = 1;
 
@@ -347,15 +340,14 @@
 /// The API is similar to the `Bio.motifs` module from Biopython on purpose.
 #[pymodule]
 #[pyo3(name = "lib")]
 pub fn init(py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__package__", "lightmotif")?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add("__author__", env!("CARGO_PKG_AUTHORS").replace(':', "\n"))?;
-    m.add("__build__", pyo3_built!(py, build))?;
 
     m.add_class::<EncodedSequence>()?;
     m.add_class::<StripedSequence>()?;
 
     m.add_class::<CountMatrix>()?;
     m.add_class::<WeightMatrix>()?;
     m.add_class::<ScoringMatrix>()?;
```

### Comparing `lightmotif-0.1.0/lightmotif-py/lightmotif/tests/test_dna.py` & `lightmotif-0.1.1/lightmotif-py/lightmotif/tests/test_dna.py`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/lightmotif-py/lightmotif/tests/unittest.rs` & `lightmotif-0.1.1/lightmotif-py/lightmotif/tests/unittest.rs`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,21 @@
         // create a Python module from our rust code with debug symbols
         let module = PyModule::new(py, "lightmotif.lib")?;
         lightmotif_py::init(py, &module).unwrap();
         sys.getattr("modules")?
             .downcast::<PyDict>()?
             .set_item("lightmotif.lib", module)?;
 
+        // create a Python module from our rust code with debug symbols
+        let arch = PyModule::new(py, "lightmotif.arch")?;
+        arch.add("AVX2_SUPPORTED", false)?;
+        sys.getattr("modules")?
+            .downcast::<PyDict>()?
+            .set_item("lightmotif.arch", arch)?;
+
         // run unittest on the tests
         let kwargs = PyDict::new(py);
         kwargs.set_item("exit", false).unwrap();
         kwargs.set_item("verbosity", 2u8).unwrap();
         py.import("unittest").unwrap().call_method(
             "TestProgram",
             ("lightmotif.tests",),
```

### Comparing `lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/PKG-INFO` & `lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
```

### Comparing `lightmotif-0.1.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt` & `lightmotif-0.1.1/lightmotif-py/lightmotif.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 pyproject.toml
 setup.cfg
 setup.py
 lightmotif/Cargo.toml
 lightmotif/README.md
 lightmotif-py/Cargo.toml
 lightmotif-py/README.md
-lightmotif-py/build.rs
 lightmotif-py/lightmotif/__init__.py
 lightmotif-py/lightmotif/lib.rs
 lightmotif-py/lightmotif.egg-info/PKG-INFO
 lightmotif-py/lightmotif.egg-info/SOURCES.txt
 lightmotif-py/lightmotif.egg-info/dependency_links.txt
 lightmotif-py/lightmotif.egg-info/top_level.txt
 lightmotif-py/lightmotif.egg-info/zip-safe
+lightmotif-py/lightmotif/arch/Cargo.toml
+lightmotif-py/lightmotif/arch/lib.rs
 lightmotif-py/lightmotif/avx2/__init__.py
 lightmotif-py/lightmotif/tests/__init__.py
 lightmotif-py/lightmotif/tests/test_dna.py
 lightmotif-py/lightmotif/tests/unittest.rs
 lightmotif/benches/ecoli.rs
 lightmotif/src/abc.rs
 lightmotif/src/dense.rs
```

### Comparing `lightmotif-0.1.0/setup.cfg` & `lightmotif-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lightmotif-0.1.0/setup.py` & `lightmotif-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,20 +127,27 @@
 
 
 # --- Setup ---------------------------------------------------------------------
 
 
 RUST_EXTENSIONS = [
     rust.RustExtension(
+        "lightmotif.arch",
+        path=os.path.join("lightmotif-py", "lightmotif", "arch", "Cargo.toml"),
+        binding=rust.Binding.PyO3,
+        strip=rust.Strip.Debug,
+        features=["extension-module"],
+    ),
+    rust.RustExtension(
         "lightmotif.lib",
         path=os.path.join("lightmotif-py", "Cargo.toml"),
         binding=rust.Binding.PyO3,
         strip=rust.Strip.Debug,
         features=["extension-module"],
-    )
+    ),
 ]
 
 if re.match("(x86_64)|(x86)|(AMD64|amd64)|(^i.86$)", MACHINE):
     RUST_EXTENSIONS.append(
         rust.RustExtension(
             "lightmotif.avx2.lib",
             path=os.path.join("lightmotif-py", "Cargo.toml"),
```

