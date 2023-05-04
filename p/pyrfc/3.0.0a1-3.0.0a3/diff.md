# Comparing `tmp/pyrfc-3.0.0a1.tar.gz` & `tmp/pyrfc-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-3.0.0a1.tar", last modified: Thu May  4 13:39:13 2023, max compression
+gzip compressed data, was "pyrfc-3.0.0a3.tar", last modified: Thu May  4 13:53:34 2023, max compression
```

## Comparing `pyrfc-3.0.0a1.tar` & `pyrfc-3.0.0a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:39:13.932875 pyrfc-3.0.0a1/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:39:13.789604 pyrfc-3.0.0a1/LICENSES/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-25 13:34:15.000000 pyrfc-3.0.0a1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 13:34:15.000000 pyrfc-3.0.0a1/MANIFEST.in
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:39:13.929508 pyrfc-3.0.0a1/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10452 2023-05-04 13:30:21.000000 pyrfc-3.0.0a1/README.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1744 2023-05-04 13:37:37.000000 pyrfc-3.0.0a1/pyproject.toml
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-04 13:39:13.933859 pyrfc-3.0.0a1/setup.cfg
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     6347 2023-05-04 13:37:07.000000 pyrfc-3.0.0a1/setup.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:39:13.761964 pyrfc-3.0.0a1/src/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:39:13.889301 pyrfc-3.0.0a1/src/pyrfc/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1480 2023-05-04 10:40:57.000000 pyrfc-3.0.0a1/src/pyrfc/__init__.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313697 2023-05-04 13:39:08.000000 pyrfc-3.0.0a1/src/pyrfc/_cyrfc.cpp
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129762 2023-05-03 12:19:55.000000 pyrfc-3.0.0a1/src/pyrfc/_cyrfc.pyx
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5675 2023-05-04 07:59:09.000000 pyrfc-3.0.0a1/src/pyrfc/_exception.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-04 09:19:28.000000 pyrfc-3.0.0a1/src/pyrfc/_utils.py
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-03 10:59:40.000000 pyrfc-3.0.0a1/src/pyrfc/csapnwrfc.pxd
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:39:13.922225 pyrfc-3.0.0a1/src/pyrfc.egg-info/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:39:13.000000 pyrfc-3.0.0a1/src/pyrfc.egg-info/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-04 13:39:13.000000 pyrfc-3.0.0a1/src/pyrfc.egg-info/SOURCES.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-04 13:39:13.000000 pyrfc-3.0.0a1/src/pyrfc.egg-info/dependency_links.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-04 13:39:13.000000 pyrfc-3.0.0a1/src/pyrfc.egg-info/top_level.txt
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.854441 pyrfc-3.0.0a3/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.714288 pyrfc-3.0.0a3/LICENSES/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-25 13:34:15.000000 pyrfc-3.0.0a3/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 13:34:15.000000 pyrfc-3.0.0a3/MANIFEST.in
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:53:34.847091 pyrfc-3.0.0a3/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10452 2023-05-04 13:30:21.000000 pyrfc-3.0.0a3/README.md
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1744 2023-05-04 13:52:27.000000 pyrfc-3.0.0a3/pyproject.toml
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-04 13:53:34.855564 pyrfc-3.0.0a3/setup.cfg
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5747 2023-05-04 13:52:23.000000 pyrfc-3.0.0a3/setup.py
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.686978 pyrfc-3.0.0a3/src/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.811531 pyrfc-3.0.0a3/src/pyrfc/
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1480 2023-05-04 10:40:57.000000 pyrfc-3.0.0a3/src/pyrfc/__init__.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313697 2023-05-04 13:53:29.000000 pyrfc-3.0.0a3/src/pyrfc/_cyrfc.cpp
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129762 2023-05-03 12:19:55.000000 pyrfc-3.0.0a3/src/pyrfc/_cyrfc.pyx
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5675 2023-05-04 07:59:09.000000 pyrfc-3.0.0a3/src/pyrfc/_exception.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-04 09:19:28.000000 pyrfc-3.0.0a3/src/pyrfc/_utils.py
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-03 10:59:40.000000 pyrfc-3.0.0a3/src/pyrfc/csapnwrfc.pxd
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:53:34.840577 pyrfc-3.0.0a3/src/pyrfc.egg-info/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-04 13:53:34.000000 pyrfc-3.0.0a3/src/pyrfc.egg-info/top_level.txt
```

### Comparing `pyrfc-3.0.0a1/LICENSES/Apache-2.0.txt` & `pyrfc-3.0.0a3/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/PKG-INFO` & `pyrfc-3.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0.0a1
+Version: 3.0.0a3
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

### Comparing `pyrfc-3.0.0a1/README.md` & `pyrfc-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/pyproject.toml` & `pyrfc-3.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["Cython >= 0.29", "setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfc"
-version = "3.0.0.a1"
+version = "3.0.0.a3"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"}, { email = "srdjan.boskovic@sap.com" } ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.8"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
```

### Comparing `pyrfc-3.0.0a1/setup.py` & `pyrfc-3.0.0a3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,168 +3,20 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import inspect
 import sys
 import os
 from setuptools import setup, Extension
 
+PACKAGE_NAME = "pyrfc"
+MODULE_NAME = "_cyrfc"
+CMDCLASS = {}
 
-def get_build_options(SAPNWRFC_HOME, platform):
-    """Build options for supported wheels."""
-
-    if platform.startswith("linux"):
-        # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.so | grep "Patch Level"')
-        LIBS = ["sapnwrfc", "sapucum"]
-        MACROS = [
-            ("NDEBUG", None),
-            ("_LARGEFILE_SOURCE", None),
-            ("_CONSOLE", None),
-            ("_FILE_OFFSET_BITS", 64),
-            ("SAPonUNIX", None),
-            ("SAPwithUNICODE", None),
-            ("SAPwithTHREADS", None),
-            ("SAPonLIN", None),
-        ]
-        COMPILE_ARGS = [
-            "-Wall",
-            "-O2",
-            "-fexceptions",
-            "-funsigned-char",
-            "-fno-strict-aliasing",
-            "-Wall",
-            "-Wno-uninitialized",
-            "-Wno-deprecated-declarations",
-            "-Wno-unused-function",
-            "-Wcast-align",
-            "-fPIC",
-            "-pthread",
-            "-minline-all-stringops",
-            f"-I{SAPNWRFC_HOME}/include",
-        ]
-        LINK_ARGS = [f"-L{SAPNWRFC_HOME}/lib"]
-    elif platform.startswith("win"):
-        # https://docs.microsoft.com/en-us/cpp/build/reference/compiler-options-listed-alphabetically
-
-        # Python sources
-        PYTHONSOURCE = os.environ.get("PYTHONSOURCE")
-        if not PYTHONSOURCE:
-            PYTHONSOURCE = inspect.getfile(inspect).split("/inspect.py")[0]
-            # sys.exit(
-            #   "Environment variable PYTHONSOURCE not set."
-            #   "Please specify this variable with the root directory of PYTHONSOURCE Library."
-            # )
-
-        # os.system("findstr Patch %SAPNWRFC_HOME%\\lib\\sapnwrfc.dll")
-        LIBS = ["sapnwrfc", "libsapucum"]
-
-        MACROS = [
-            ("SAPonNT", None),
-            ("_CRT_NON_CONFORMING_SWPRINTFS", None),
-            ("_CRT_SECURE_NO_DEPRECATES", None),
-            ("_CRT_NONSTDC_NO_DEPRECATE", None),
-            ("_AFXDLL", None),
-            ("WIN32", None),
-            ("_WIN32_WINNT", "0x0502"),
-            ("WIN64", None),
-            ("_AMD64_", None),
-            ("NDEBUG", None),
-            ("SAPwithUNICODE", None),
-            ("UNICODE", None),
-            ("_UNICODE", None),
-            ("SAPwithTHREADS", None),
-            ("_ATL_ALLOW_CHAR_UNSIGNED", None),
-            ("_LARGEFILE_SOURCE", None),
-            ("_CONSOLE", None),
-            ("SAP_PLATFORM_MAKENAME", "ntintel"),
-        ]
-
-        COMPILE_ARGS = [
-            f"-I{SAPNWRFC_HOME}\\include",
-            f"-I{PYTHONSOURCE}\\Include",
-            f"-I{PYTHONSOURCE}\\Include\\PC",
-            "/EHs",
-            "/GL",
-            "/Gy",
-            "/J",
-            "/MD",
-            "/nologo",
-            "/O2",
-            "/Oy-",
-            "/we4552",
-            "/we4700",
-            "/we4789",
-            "/W3",
-            "/Z7",
-        ]
-
-        LINK_ARGS = [
-            f"-LIBPATH:{SAPNWRFC_HOME}\\lib",
-            f"-LIBPATH:{PYTHONSOURCE}\\PCbuild",
-            "/NXCOMPAT",
-            "/STACK:0x2000000",
-            "/SWAPRUN:NET",
-            "/DEBUG",
-            "/OPT:REF",
-            "/DEBUGTYPE:CV,FIXUP",
-            "/MACHINE:amd64",
-            "/nologo",
-            "/LTCG",
-        ]
-    elif platform.startswith("darwin"):
-        # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.dylib | grep "Patch Level"')
-        MACOS_VERSION_MIN = "10.15"
-
-        LIBS = ["sapnwrfc", "sapucum"]
-        MACROS = [
-            ("NDEBUG", None),
-            ("_LARGEFILE_SOURCE", None),
-            ("_CONSOLE", None),
-            ("_FILE_OFFSET_BITS", 64),
-            ("SAPonUNIX", None),
-            ("SAPwithUNICODE", None),
-            ("SAPwithTHREADS", None),
-            ("SAPonDARW", None),
-        ]
-        COMPILE_ARGS = [
-            "-Wall",
-            "-O2",
-            "-fexceptions",
-            "-funsigned-char",
-            "-fno-strict-aliasing",
-            "-Wno-uninitialized",
-            "-Wcast-align",
-            "-fPIC",
-            "-pthread",
-            "-minline-all-stringops",
-            "-isystem",
-            "-std=c++11",
-            f"-mmacosx-version-min={MACOS_VERSION_MIN}",
-            f"-I{SAPNWRFC_HOME}/include",
-            "-Wno-cast-align",
-            "-Wno-deprecated-declarations",
-            "-Wno-unused-function",
-            "-Wno-nullability-completeness",
-            "-Wno-expansion-to-defined",
-            "-Wno-unreachable-code-fallthrough",
-        ]
-        LINK_ARGS = [
-            f"-L{SAPNWRFC_HOME}/lib",
-            "-stdlib=libc++",
-            f"-mmacosx-version-min={MACOS_VERSION_MIN}",
-            f"-Wl,-rpath,{SAPNWRFC_HOME}/lib",
-        ]
-    else:
-        sys.exit(f"Platform not supported: {platform}.")
-    return {"LIBS": LIBS, "MACROS": MACROS, "COMPILE_ARGS": COMPILE_ARGS, "LINK_ARGS": LINK_ARGS}
-
-
-package_name = "pyrfc"
 build_cython = sys.platform.startswith("linux")
 
-CMDCLASS = {}
 if build_cython:
     try:
         from Cython.Distutils import build_ext
         from Cython.Build import cythonize
     except ImportError:
         sys.exit("Cython not installed: https://cython.readthedocs.io/en/latest/src/quickstart/install.html")
     CMDCLASS = {"build_ext": build_ext}
@@ -173,28 +25,174 @@
 SAPNWRFC_HOME = os.environ.get("SAPNWRFC_HOME")
 if not SAPNWRFC_HOME:
     sys.exit(
         "Environment variable SAPNWRFC_HOME not set.\n"
         "Please specify this variable with the root directory of the SAP NWRFC Library."
     )
 
-build_options = get_build_options(SAPNWRFC_HOME, sys.platform)
+if sys.platform.startswith("linux"):
+    # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.so | grep "Patch Level"')
+    LIBS = ["sapnwrfc", "sapucum"]
+    MACROS = [
+        ("NDEBUG", None),
+        ("_LARGEFILE_SOURCE", None),
+        ("_CONSOLE", None),
+        ("_FILE_OFFSET_BITS", 64),
+        ("SAPonUNIX", None),
+        ("SAPwithUNICODE", None),
+        ("SAPwithTHREADS", None),
+        ("SAPonLIN", None),
+    ]
+    COMPILE_ARGS = [
+        "-Wall",
+        "-O2",
+        "-fexceptions",
+        "-funsigned-char",
+        "-fno-strict-aliasing",
+        "-Wall",
+        "-Wno-uninitialized",
+        "-Wno-deprecated-declarations",
+        "-Wno-unused-function",
+        "-Wcast-align",
+        "-fPIC",
+        "-pthread",
+        "-minline-all-stringops",
+        f"-I{SAPNWRFC_HOME}/include",
+    ]
+    LINK_ARGS = [f"-L{SAPNWRFC_HOME}/lib"]
+elif sys.platform.startswith("win"):
+    # https://docs.microsoft.com/en-us/cpp/build/reference/compiler-options-listed-alphabetically
+
+    # Python sources
+    PYTHONSOURCE = os.environ.get("PYTHONSOURCE")
+    if not PYTHONSOURCE:
+        PYTHONSOURCE = inspect.getfile(inspect).split("/inspect.py")[0]
+        # sys.exit(
+        #   "Environment variable PYTHONSOURCE not set."
+        #   "Please specify this variable with the root directory of PYTHONSOURCE Library."
+        # )
+
+    # os.system("findstr Patch %SAPNWRFC_HOME%\\lib\\sapnwrfc.dll")
+    LIBS = ["sapnwrfc", "libsapucum"]
+
+    MACROS = [
+        ("SAPonNT", None),
+        ("_CRT_NON_CONFORMING_SWPRINTFS", None),
+        ("_CRT_SECURE_NO_DEPRECATES", None),
+        ("_CRT_NONSTDC_NO_DEPRECATE", None),
+        ("_AFXDLL", None),
+        ("WIN32", None),
+        ("_WIN32_WINNT", "0x0502"),
+        ("WIN64", None),
+        ("_AMD64_", None),
+        ("NDEBUG", None),
+        ("SAPwithUNICODE", None),
+        ("UNICODE", None),
+        ("_UNICODE", None),
+        ("SAPwithTHREADS", None),
+        ("_ATL_ALLOW_CHAR_UNSIGNED", None),
+        ("_LARGEFILE_SOURCE", None),
+        ("_CONSOLE", None),
+        ("SAP_PLATFORM_MAKENAME", "ntintel"),
+    ]
+
+    COMPILE_ARGS = [
+        f"-I{SAPNWRFC_HOME}\\include",
+        f"-I{PYTHONSOURCE}\\Include",
+        f"-I{PYTHONSOURCE}\\Include\\PC",
+        "/EHs",
+        "/GL",
+        "/Gy",
+        "/J",
+        "/MD",
+        "/nologo",
+        "/O2",
+        "/Oy-",
+        "/we4552",
+        "/we4700",
+        "/we4789",
+        "/W3",
+        "/Z7",
+    ]
+
+    LINK_ARGS = [
+        f"-LIBPATH:{SAPNWRFC_HOME}\\lib",
+        f"-LIBPATH:{PYTHONSOURCE}\\PCbuild",
+        "/NXCOMPAT",
+        "/STACK:0x2000000",
+        "/SWAPRUN:NET",
+        "/DEBUG",
+        "/OPT:REF",
+        "/DEBUGTYPE:CV,FIXUP",
+        "/MACHINE:amd64",
+        "/nologo",
+        "/LTCG",
+    ]
+elif sys.platform.startswith("darwin"):
+    # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.dylib | grep "Patch Level"')
+    MACOS_VERSION_MIN = "10.15"
+
+    LIBS = ["sapnwrfc", "sapucum"]
+    MACROS = [
+        ("NDEBUG", None),
+        ("_LARGEFILE_SOURCE", None),
+        ("_CONSOLE", None),
+        ("_FILE_OFFSET_BITS", 64),
+        ("SAPonUNIX", None),
+        ("SAPwithUNICODE", None),
+        ("SAPwithTHREADS", None),
+        ("SAPonDARW", None),
+    ]
+    COMPILE_ARGS = [
+        "-Wall",
+        "-O2",
+        "-fexceptions",
+        "-funsigned-char",
+        "-fno-strict-aliasing",
+        "-Wno-uninitialized",
+        "-Wcast-align",
+        "-fPIC",
+        "-pthread",
+        "-minline-all-stringops",
+        "-isystem",
+        "-std=c++11",
+        f"-mmacosx-version-min={MACOS_VERSION_MIN}",
+        f"-I{SAPNWRFC_HOME}/include",
+        "-Wno-cast-align",
+        "-Wno-deprecated-declarations",
+        "-Wno-unused-function",
+        "-Wno-nullability-completeness",
+        "-Wno-expansion-to-defined",
+        "-Wno-unreachable-code-fallthrough",
+    ]
+    LINK_ARGS = [
+        f"-L{SAPNWRFC_HOME}/lib",
+        "-stdlib=libc++",
+        f"-mmacosx-version-min={MACOS_VERSION_MIN}",
+        # https://stackoverflow.com/questions/6638500/how-to-specify-rpath-in-a-makefile
+        f"-Wl,-rpath,{SAPNWRFC_HOME}/lib",
+    ]
+else:
+    sys.exit(f"Platform not supported: {sys.platform}.")
+
 
+# https://docs.python.org/2/distutils/apiref.html
 PYRFC_EXT = Extension(
     language="c++",
-    name=f"{package_name}._cyrfc",
-    sources=[f"src/{package_name}/_cyrfc.pyx"],
-    define_macros=build_options["MACROS"],
-    extra_compile_args=build_options["COMPILE_ARGS"],
-    extra_link_args=build_options["LINK_ARGS"],
-    libraries=build_options["LIBS"],
+    name=f"{PACKAGE_NAME}.{MODULE_NAME}",
+    sources=[f"src/{PACKAGE_NAME}/{MODULE_NAME}.pyx"],
+    define_macros=MACROS,
+    extra_compile_args=COMPILE_ARGS,
+    extra_link_args=LINK_ARGS,
+    libraries=LIBS,
 )
 
+# cf. http://docs.python.org/distutils/setupscript.html#additional-meta-data
 setup(
-    name=package_name,
+    name=PACKAGE_NAME,
     # install_requires=["setuptools"],
     cmdclass=CMDCLASS,  # type: ignore
     ext_modules=cythonize(PYRFC_EXT, annotate=True, compiler_directives={"language_level": "3"})  # type: ignore
     if build_cython
     else [PYRFC_EXT],  # type: ignore
-    test_suite="tests"
-)
+    test_suite=MODULE_NAME,
+)
```

### Comparing `pyrfc-3.0.0a1/src/pyrfc/__init__.py` & `pyrfc-3.0.0a3/src/pyrfc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/src/pyrfc/_cyrfc.cpp` & `pyrfc-3.0.0a3/src/pyrfc/_cyrfc.cpp`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/src/pyrfc/_cyrfc.pyx` & `pyrfc-3.0.0a3/src/pyrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/src/pyrfc/_exception.py` & `pyrfc-3.0.0a3/src/pyrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/src/pyrfc/csapnwrfc.pxd` & `pyrfc-3.0.0a3/src/pyrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `pyrfc-3.0.0a1/src/pyrfc.egg-info/PKG-INFO` & `pyrfc-3.0.0a3/src/pyrfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 3.0.0a1
+Version: 3.0.0a3
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

