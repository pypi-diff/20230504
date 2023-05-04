# Comparing `tmp/qlat_cps-0.28.tar.gz` & `tmp/qlat_cps-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat_cps-0.28.tar", last modified: Mon Apr 17 05:43:13 2023, max compression
+gzip compressed data, was "qlat_cps-0.31.tar", last modified: Thu May  4 04:33:31 2023, max compression
```

## Comparing `qlat_cps-0.28.tar` & `qlat_cps-0.31.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_cps-0.28/README.md
--rwxrwxr-x   0        0        0       96 1970-01-01 00:00:00.000000 qlat_cps-0.28/bin/qlat-cps-include
--rw-rw-r--   0        0        0     1393 1970-01-01 00:00:00.000000 qlat_cps-0.28/depend-cps/meson.build
--rw-rw-r--   0        0        0     2382 1970-01-01 00:00:00.000000 qlat_cps-0.28/depend-qlat/meson.build
--rw-rw-r--   0        0        0       54 1970-01-01 00:00:00.000000 qlat_cps-0.28/include/meson.build
--rw-rw-r--   0        0        0      274 1970-01-01 00:00:00.000000 qlat_cps-0.28/include/qlat-cps/meson.build
--rw-rw-r--   0        0        0      413 1970-01-01 00:00:00.000000 qlat_cps-0.28/include/qlat-cps/qlat-cps.h
--rw-rw-r--   0        0        0      570 1970-01-01 00:00:00.000000 qlat_cps-0.28/lib/init.cpp
--rw-rw-r--   0        0        0      361 1970-01-01 00:00:00.000000 qlat_cps-0.28/lib/meson.build
--rw-rw-r--   0        0        0     2041 1970-01-01 00:00:00.000000 qlat_cps-0.28/lib/prop.cpp
--rw-rw-r--   0        0        0     1235 1970-01-01 00:00:00.000000 qlat_cps-0.28/meson.build
--rw-rw-r--   0        0        0       19 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/meson.build
--rw-rw-r--   0        0        0      117 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/__init__.py
--rw-rw-r--   0        0        0       70 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/all.pxd
--rw-rw-r--   0        0        0      147 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/c.py
--rw-rw-r--   0        0        0       67 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/cp.pxd
--rw-rw-r--   0        0        0      858 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/cp.pyx
--rw-rw-r--   0        0        0      430 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/everything.pxd
--rw-rw-r--   0        0        0      876 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/get_include_dir.py
--rw-rw-r--   0        0        0       44 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/init.py
--rw-rw-r--   0        0        0     1277 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/meson.build
--rw-rw-r--   0        0        0       58 1970-01-01 00:00:00.000000 qlat_cps-0.28/pylib/qlat_cps/prop.py
--rw-rw-r--   0        0        0      485 1970-01-01 00:00:00.000000 qlat_cps-0.28/pyproject.toml
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 qlat_cps-0.28/PKG-INFO
+-rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_cps-0.31/README.md
+-rwxrwxr-x   0        0        0       96 1970-01-01 00:00:00.000000 qlat_cps-0.31/bin/qlat-cps-include
+-rw-rw-r--   0        0        0     1393 1970-01-01 00:00:00.000000 qlat_cps-0.31/depend-cps/meson.build
+-rw-rw-r--   0        0        0     2382 1970-01-01 00:00:00.000000 qlat_cps-0.31/depend-qlat/meson.build
+-rw-rw-r--   0        0        0       54 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/meson.build
+-rw-rw-r--   0        0        0      293 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/qlat-cps/meson.build
+-rw-rw-r--   0        0        0      413 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/qlat-cps/qlat-cps.h
+-rw-rw-r--   0        0        0      570 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/init.cpp
+-rw-rw-r--   0        0        0      380 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/meson.build
+-rw-rw-r--   0        0        0     2041 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/prop.cpp
+-rw-rw-r--   0        0        0     1267 1970-01-01 00:00:00.000000 qlat_cps-0.31/meson.build
+-rw-rw-r--   0        0        0       19 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/meson.build
+-rw-rw-r--   0        0        0      117 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/__init__.py
+-rw-rw-r--   0        0        0       70 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/all.pxd
+-rw-rw-r--   0        0        0      147 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/c.py
+-rw-rw-r--   0        0        0       67 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/cp.pxd
+-rw-rw-r--   0        0        0      858 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/cp.pyx
+-rw-rw-r--   0        0        0      430 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/everything.pxd
+-rw-rw-r--   0        0        0      876 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/get_include_dir.py
+-rw-rw-r--   0        0        0       44 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/init.py
+-rw-rw-r--   0        0        0     1315 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/meson.build
+-rw-rw-r--   0        0        0       58 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/prop.py
+-rw-rw-r--   0        0        0      529 1970-01-01 00:00:00.000000 qlat_cps-0.31/pyproject.toml
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 qlat_cps-0.31/PKG-INFO
```

### Comparing `qlat_cps-0.28/depend-cps/meson.build` & `qlat_cps-0.31/depend-cps/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/depend-qlat/meson.build` & `qlat_cps-0.31/depend-qlat/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/lib/init.cpp` & `qlat_cps-0.31/lib/init.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/lib/prop.cpp` & `qlat_cps-0.31/lib/prop.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/meson.build` & `qlat_cps-0.31/meson.build`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 project('qlat-cps', 'cpp', 'cython',
-  version: '0.28',
+  version: '0.31',
   license: 'GPL-3.0-or-later',
   default_options: [
     'warning_level=3',
     'cpp_std=c++14',
     'libdir=lib',
     'optimization=2',
     'debug=false',
     'cython_language=cpp',
     ])
 
 add_project_arguments('-fno-strict-aliasing', language: ['c', 'cpp'])
 
 py_mod = import('python')
-py3 = py_mod.find_installation('python3')
+py3 = py_mod.find_installation('python3', pure: false)
 message(py3.path())
 message(py3.get_install_dir())
 
 cxx = run_command('bash', '-c', 'echo "$CXX"', check: true).stdout().strip()
 mpicxx = run_command('bash', '-c', 'echo "$MPICXX"', check: true).stdout().strip()
 
 if cxx != '' and mpicxx == cxx
@@ -33,10 +33,10 @@
 
 deps = [ mpic, qlat, cps, ]
 
 subdir('include')
 subdir('lib')
 subdir('pylib')
 
-c = run_command('bash', '-c', 'cd "$MESON_SUBDIR" ; ls bin/*', check: true)
+c = run_command('bash', '-c', 'cd "$MESON_SOURCE_ROOT/$MESON_SUBDIR" ; ls bin/*', check: true)
 scripts = files(c.stdout().strip().split('\n'))
 install_data(scripts, install_dir: get_option('bindir'), install_mode: 'rwxr-xr-x')
```

### Comparing `qlat_cps-0.28/pylib/qlat_cps/cp.pyx` & `qlat_cps-0.31/pylib/qlat_cps/cp.pyx`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/pylib/qlat_cps/get_include_dir.py` & `qlat_cps-0.31/pylib/qlat_cps/get_include_dir.py`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.28/pylib/qlat_cps/meson.build` & `qlat_cps-0.31/pylib/qlat_cps/meson.build`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 py_fns = run_command(
-  'bash', '-c', 'cd "$MESON_SUBDIR" ; ls *.py | grep -v "_template\."',
+  'bash', '-c', 'cd "$MESON_SOURCE_ROOT/$MESON_SUBDIR" ; ls *.py | grep -v "_template\."',
   check: true,
   ).stdout().strip().split('\n')
 py_files = files(py_fns)
 
 pxd_fns = run_command(
-  'bash', '-c', 'cd "$MESON_SUBDIR" ; ls *.pxd | grep -v "_template\."',
+  'bash', '-c', 'cd "$MESON_SOURCE_ROOT/$MESON_SUBDIR" ; ls *.pxd | grep -v "_template\."',
   check: true,
   ).stdout().strip().split('\n')
 pxd_files = files(pxd_fns)
 
 py3.install_sources(py_files + pxd_files, subdir: 'qlat_cps')
 
 pxd_tgts = []
```

