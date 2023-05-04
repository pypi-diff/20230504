# Comparing `tmp/pyrfc-2.8.3.tar.gz` & `tmp/pyrfc-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfc-2.8.3.tar", last modified: Tue Apr 25 12:12:10 2023, max compression
+gzip compressed data, was "pyrfc-3.0.0a0.tar", last modified: Thu May  4 13:07:31 2023, max compression
```

## Comparing `pyrfc-2.8.3.tar` & `pyrfc-3.0.0a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.271593 pyrfc-2.8.3/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.088322 pyrfc-2.8.3/LICENSES/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-24 08:04:52.000000 pyrfc-2.8.3/LICENSES/Apache-2.0.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 11:34:22.000000 pyrfc-2.8.3/MANIFEST.in
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23387 2023-04-25 12:12:10.268527 pyrfc-2.8.3/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10174 2023-04-24 17:43:16.000000 pyrfc-2.8.3/README.md
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1814 2023-04-25 11:44:27.000000 pyrfc-2.8.3/pyproject.toml
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-04-25 12:12:10.272447 pyrfc-2.8.3/setup.cfg
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)     5727 2023-04-25 11:38:06.000000 pyrfc-2.8.3/setup.py
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.061019 pyrfc-2.8.3/src/
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.185932 pyrfc-2.8.3/src/pyrfc/
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1330 2023-04-25 11:34:43.000000 pyrfc-2.8.3/src/pyrfc/__init__.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313573 2023-04-25 12:12:04.000000 pyrfc-2.8.3/src/pyrfc/_cyrfc.cpp
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129750 2023-04-24 08:04:53.000000 pyrfc-2.8.3/src/pyrfc/_cyrfc.pyx
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5596 2023-04-25 11:38:52.000000 pyrfc-2.8.3/src/pyrfc/_exception.py
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      293 2023-04-25 11:38:47.000000 pyrfc-2.8.3/src/pyrfc/_utils.py
--rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-04-24 08:04:53.000000 pyrfc-2.8.3/src/pyrfc/csapnwrfc.pxd
-drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-04-25 12:12:10.259500 pyrfc-2.8.3/src/pyrfc.egg-info/
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23387 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/PKG-INFO
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-04-25 12:12:10.000000 pyrfc-2.8.3/src/pyrfc.egg-info/SOURCES.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/dependency_links.txt
--rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-04-25 12:12:09.000000 pyrfc-2.8.3/src/pyrfc.egg-info/top_level.txt
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:07:31.686866 pyrfc-3.0.0a0/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:07:31.542696 pyrfc-3.0.0a0/LICENSES/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10283 2023-04-25 13:34:15.000000 pyrfc-3.0.0a0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       58 2023-04-25 13:34:15.000000 pyrfc-3.0.0a0/MANIFEST.in
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:07:31.683633 pyrfc-3.0.0a0/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    10452 2023-05-03 06:15:18.000000 pyrfc-3.0.0a0/README.md
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     1744 2023-05-04 13:05:59.000000 pyrfc-3.0.0a0/pyproject.toml
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)       38 2023-05-04 13:07:31.688464 pyrfc-3.0.0a0/setup.cfg
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)     6318 2023-05-04 10:39:57.000000 pyrfc-3.0.0a0/setup.py
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:07:31.501909 pyrfc-3.0.0a0/src/
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:07:31.648897 pyrfc-3.0.0a0/src/pyrfc/
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     1480 2023-05-04 10:40:57.000000 pyrfc-3.0.0a0/src/pyrfc/__init__.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)  2313697 2023-05-04 13:07:25.000000 pyrfc-3.0.0a0/src/pyrfc/_cyrfc.cpp
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)   129762 2023-05-03 12:19:55.000000 pyrfc-3.0.0a0/src/pyrfc/_cyrfc.pyx
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)     5675 2023-05-04 07:59:09.000000 pyrfc-3.0.0a0/src/pyrfc/_exception.py
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      317 2023-05-04 09:19:28.000000 pyrfc-3.0.0a0/src/pyrfc/_utils.py
+-rwxr-xr-x   0 www-admin  (1000) www-admin  (1000)    23820 2023-05-03 10:59:40.000000 pyrfc-3.0.0a0/src/pyrfc/csapnwrfc.pxd
+drwxr-xr-x   0 www-admin  (1000) www-admin  (1000)        0 2023-05-04 13:07:31.674567 pyrfc-3.0.0a0/src/pyrfc.egg-info/
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)    23719 2023-05-04 13:07:31.000000 pyrfc-3.0.0a0/src/pyrfc.egg-info/PKG-INFO
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)      333 2023-05-04 13:07:31.000000 pyrfc-3.0.0a0/src/pyrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        1 2023-05-04 13:07:31.000000 pyrfc-3.0.0a0/src/pyrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 www-admin  (1000) www-admin  (1000)        6 2023-05-04 13:07:31.000000 pyrfc-3.0.0a0/src/pyrfc.egg-info/top_level.txt
```

### Comparing `pyrfc-2.8.3/LICENSES/Apache-2.0.txt` & `pyrfc-3.0.0a0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyrfc-2.8.3/PKG-INFO` & `pyrfc-3.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 2.8.3
+Version: 3.0.0a0
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
+Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
         http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
         AND DISTRIBUTION
@@ -209,48 +210,49 @@
         
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         
         See the License for the specific language governing permissions and
         
         limitations under the License.
         
-Project-URL: homepage, https://github.com/SAP/PyRFC
+Project-URL: bug-tracker, https://github.com/wntrblm/nox/issues
 Project-URL: documentation, http://sap.github.io/PyRFC
+Project-URL: homepage, https://github.com/SAP/PyRFC
 Project-URL: repository, https://github.com/SAP/PyRFC.git
 Keywords: pyrfc,sap,nwrfc,sapnwrfc,abap
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrfc)](https://pypi.org/project/pyrfc/)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyrfc)](https://pypistats.org/packages/pyrfc)
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/PyRFC)](https://api.reuse.software/info/github.com/SAP/PyRFC)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4349/badge)](https://bestpractices.coreinfrastructure.org/projects/4349)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 - [Features](#features)
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
@@ -324,29 +326,31 @@
 
 Cython must be installed upfront because the build from source is standard installation method on Linux.
 
 Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
-# or
-PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
 python -m pip install .
 # or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
+Run ``python`` and type ``from pyrfc import *``. If this finishes silently, without oputput, the installation was successful.
+
+Using virtual environments you can isolate Python/PyRFC projects, working without administrator privileges.
+
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
 
 **Note:** The package must be [installed](#download-and-installation) before use.
```

### Comparing `pyrfc-2.8.3/README.md` & `pyrfc-3.0.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrfc)](https://pypi.org/project/pyrfc/)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyrfc)](https://pypistats.org/packages/pyrfc)
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/PyRFC)](https://api.reuse.software/info/github.com/SAP/PyRFC)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4349/badge)](https://bestpractices.coreinfrastructure.org/projects/4349)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 - [Features](#features)
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
@@ -86,29 +87,31 @@
 
 Cython must be installed upfront because the build from source is standard installation method on Linux.
 
 Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
-# or
-PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
 python -m pip install .
 # or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
+Run ``python`` and type ``from pyrfc import *``. If this finishes silently, without oputput, the installation was successful.
+
+Using virtual environments you can isolate Python/PyRFC projects, working without administrator privileges.
+
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
 
 **Note:** The package must be [installed](#download-and-installation) before use.
```

### Comparing `pyrfc-2.8.3/pyproject.toml` & `pyrfc-3.0.0a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 [build-system]
-requires = ["Cython ~= 0.29.0", "setuptools ~= 67.7.0", "wheel ~= 0.40.0"]
+requires = ["Cython >= 0.29", "setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
-# https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "pyrfc"
-version = "2.8.3"
+version = "3.0.0.a0"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
-authors = [ { name = "SAP SE"} ]
+authors = [ { name = "SAP SE"}, { email = "srdjan.boskovic@sap.com" } ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Cython",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only"
 ]
 dependencies = []
 
 [project.urls]
-homepage = "https://github.com/SAP/PyRFC"
+bug-tracker = "https://github.com/wntrblm/nox/issues"
 documentation = "http://sap.github.io/PyRFC"
+homepage = "https://github.com/SAP/PyRFC"
 repository = "https://github.com/SAP/PyRFC.git"
 
+[tool.black]
+line-length = 120
+
 [tool.cython-lint]
-max-line-length = 148
+max-line-length = 180
 
-# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [tool.setuptools]
 package-dir = {"" = "src"}
 include-package-data = false
 license-files=["LICENSES/*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["pyrfc"]
 
-[tool.setuptools.dynamic]
-readme = {file = "README.md"}
+[tool.pytest.ini_options]
+minversion = "7.3"
+testpaths =["tests"]
```

### Comparing `pyrfc-2.8.3/setup.py` & `pyrfc-3.0.0a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,190 +3,199 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import inspect
 import sys
 import os
 from setuptools import setup, Extension
 
-PACKAGE_NAME = "pyrfc"
-MODULE_NAME = "_cyrfc"
 
-BUILD_CYTHON = bool(os.getenv("PYRFC_BUILD_CYTHON")) or sys.platform.startswith("linux")
-CMDCLASS = {}
 
-if BUILD_CYTHON:
+def get_build_options(platform):
+    """Build options for supported wheels."""
+
+    if platform.startswith("linux"):
+        # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.so | grep "Patch Level"')
+        LIBS = ["sapnwrfc", "sapucum"]
+        MACROS = [
+            ("NDEBUG", None),
+            ("_LARGEFILE_SOURCE", None),
+            ("_CONSOLE", None),
+            ("_FILE_OFFSET_BITS", 64),
+            ("SAPonUNIX", None),
+            ("SAPwithUNICODE", None),
+            ("SAPwithTHREADS", None),
+            ("SAPonLIN", None),
+        ]
+        COMPILE_ARGS = [
+            "-Wall",
+            "-O2",
+            "-fexceptions",
+            "-funsigned-char",
+            "-fno-strict-aliasing",
+            "-Wall",
+            "-Wno-uninitialized",
+            "-Wno-deprecated-declarations",
+            "-Wno-unused-function",
+            "-Wcast-align",
+            "-fPIC",
+            "-pthread",
+            "-minline-all-stringops",
+            f"-I{SAPNWRFC_HOME}/include",
+        ]
+        LINK_ARGS = [f"-L{SAPNWRFC_HOME}/lib"]
+    elif platform.startswith("win"):
+        # https://docs.microsoft.com/en-us/cpp/build/reference/compiler-options-listed-alphabetically
+
+        # Python sources
+        PYTHONSOURCE = os.environ.get("PYTHONSOURCE")
+        if not PYTHONSOURCE:
+            PYTHONSOURCE = inspect.getfile(inspect).split("/inspect.py")[0]
+            # sys.exit(
+            #   "Environment variable PYTHONSOURCE not set."
+            #   "Please specify this variable with the root directory of PYTHONSOURCE Library."
+            # )
+
+        # os.system("findstr Patch %SAPNWRFC_HOME%\\lib\\sapnwrfc.dll")
+        LIBS = ["sapnwrfc", "libsapucum"]
+
+        MACROS = [
+            ("SAPonNT", None),
+            ("_CRT_NON_CONFORMING_SWPRINTFS", None),
+            ("_CRT_SECURE_NO_DEPRECATES", None),
+            ("_CRT_NONSTDC_NO_DEPRECATE", None),
+            ("_AFXDLL", None),
+            ("WIN32", None),
+            ("_WIN32_WINNT", "0x0502"),
+            ("WIN64", None),
+            ("_AMD64_", None),
+            ("NDEBUG", None),
+            ("SAPwithUNICODE", None),
+            ("UNICODE", None),
+            ("_UNICODE", None),
+            ("SAPwithTHREADS", None),
+            ("_ATL_ALLOW_CHAR_UNSIGNED", None),
+            ("_LARGEFILE_SOURCE", None),
+            ("_CONSOLE", None),
+            ("SAP_PLATFORM_MAKENAME", "ntintel"),
+        ]
+
+        COMPILE_ARGS = [
+            f"-I{SAPNWRFC_HOME}\\include",
+            f"-I{PYTHONSOURCE}\\Include",
+            f"-I{PYTHONSOURCE}\\Include\\PC",
+            "/EHs",
+            "/GL",
+            "/Gy",
+            "/J",
+            "/MD",
+            "/nologo",
+            "/O2",
+            "/Oy-",
+            "/we4552",
+            "/we4700",
+            "/we4789",
+            "/W3",
+            "/Z7",
+        ]
+
+        LINK_ARGS = [
+            f"-LIBPATH:{SAPNWRFC_HOME}\\lib",
+            f"-LIBPATH:{PYTHONSOURCE}\\PCbuild",
+            "/NXCOMPAT",
+            "/STACK:0x2000000",
+            "/SWAPRUN:NET",
+            "/DEBUG",
+            "/OPT:REF",
+            "/DEBUGTYPE:CV,FIXUP",
+            "/MACHINE:amd64",
+            "/nologo",
+            "/LTCG",
+        ]
+    elif platform.startswith("darwin"):
+        # os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.dylib | grep "Patch Level"')
+        MACOS_VERSION_MIN = "10.15"
+
+        LIBS = ["sapnwrfc", "sapucum"]
+        MACROS = [
+            ("NDEBUG", None),
+            ("_LARGEFILE_SOURCE", None),
+            ("_CONSOLE", None),
+            ("_FILE_OFFSET_BITS", 64),
+            ("SAPonUNIX", None),
+            ("SAPwithUNICODE", None),
+            ("SAPwithTHREADS", None),
+            ("SAPonDARW", None),
+        ]
+        COMPILE_ARGS = [
+            "-Wall",
+            "-O2",
+            "-fexceptions",
+            "-funsigned-char",
+            "-fno-strict-aliasing",
+            "-Wno-uninitialized",
+            "-Wcast-align",
+            "-fPIC",
+            "-pthread",
+            "-minline-all-stringops",
+            "-isystem",
+            "-std=c++11",
+            f"-mmacosx-version-min={MACOS_VERSION_MIN}",
+            f"-I{SAPNWRFC_HOME}/include",
+            "-Wno-cast-align",
+            "-Wno-deprecated-declarations",
+            "-Wno-unused-function",
+            "-Wno-nullability-completeness",
+            "-Wno-expansion-to-defined",
+            "-Wno-unreachable-code-fallthrough",
+        ]
+        LINK_ARGS = [
+            f"-L{SAPNWRFC_HOME}/lib",
+            "-stdlib=libc++",
+            f"-mmacosx-version-min={MACOS_VERSION_MIN}",
+            f"-Wl,-rpath,{SAPNWRFC_HOME}/lib",
+        ]
+    else:
+        sys.exit(f"Platform not supported: {platform}.")
+    return {"LIBS": LIBS, "MACROS": MACROS, "COMPILE_ARGS": COMPILE_ARGS, "LINK_ARGS": LINK_ARGS}
+
+
+package_name = "pyrfc"
+build_cython = sys.platform.startswith("linux")
+
+CMDCLASS = {}
+if build_cython:
     try:
         from Cython.Distutils import build_ext
         from Cython.Build import cythonize
     except ImportError:
         sys.exit("Cython not installed: https://cython.readthedocs.io/en/latest/src/quickstart/install.html")
     CMDCLASS = {"build_ext": build_ext}
 
 # Check if SAP NWRFC SDK configured
 SAPNWRFC_HOME = os.environ.get("SAPNWRFC_HOME")
 if not SAPNWRFC_HOME:
-    sys.exit("Environment variable SAPNWRFC_HOME not set.\n" "Please specify this variable with the root directory of the SAP NWRFC Library.")
-
-if sys.platform.startswith("linux"):
-    os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.so | grep "Patch Level"')
-    LIBS = ["sapnwrfc", "sapucum"]
-    MACROS = [
-        ("NDEBUG", None),
-        ("_LARGEFILE_SOURCE", None),
-        ("_CONSOLE", None),
-        ("_FILE_OFFSET_BITS", 64),
-        ("SAPonUNIX", None),
-        ("SAPwithUNICODE", None),
-        ("SAPwithTHREADS", None),
-        ("SAPonLIN", None),
-    ]
-    COMPILE_ARGS = [
-        "-Wall",
-        "-O2",
-        "-fexceptions",
-        "-funsigned-char",
-        "-fno-strict-aliasing",
-        "-Wall",
-        "-Wno-uninitialized",
-        "-Wno-deprecated-declarations",
-        "-Wno-unused-function",
-        "-Wcast-align",
-        "-fPIC",
-        "-pthread",
-        "-minline-all-stringops",
-        f"-I{SAPNWRFC_HOME}/include",
-    ]
-    LINK_ARGS = [f"-L{SAPNWRFC_HOME}/lib"]
-elif sys.platform.startswith("win"):
-    # https://docs.microsoft.com/en-us/cpp/build/reference/compiler-options-listed-alphabetically
-
-    # Python sources
-    PYTHONSOURCE = os.environ.get("PYTHONSOURCE")
-    if not PYTHONSOURCE:
-        PYTHONSOURCE = inspect.getfile(inspect).split("/inspect.py")[0]
-        # sys.exit('Environment variable PYTHONSOURCE not set. Please specify this variable with the root directory of the PYTHONSOURCE Library.')
-
-    os.system("findstr Patch %SAPNWRFC_HOME%\\lib\\sapnwrfc.dll")
-    LIBS = ["sapnwrfc", "libsapucum"]
-
-    MACROS = [
-        ("SAPonNT", None),
-        ("_CRT_NON_CONFORMING_SWPRINTFS", None),
-        ("_CRT_SECURE_NO_DEPRECATES", None),
-        ("_CRT_NONSTDC_NO_DEPRECATE", None),
-        ("_AFXDLL", None),
-        ("WIN32", None),
-        ("_WIN32_WINNT", "0x0502"),
-        ("WIN64", None),
-        ("_AMD64_", None),
-        ("NDEBUG", None),
-        ("SAPwithUNICODE", None),
-        ("UNICODE", None),
-        ("_UNICODE", None),
-        ("SAPwithTHREADS", None),
-        ("_ATL_ALLOW_CHAR_UNSIGNED", None),
-        ("_LARGEFILE_SOURCE", None),
-        ("_CONSOLE", None),
-        ("SAP_PLATFORM_MAKENAME", "ntintel"),
-    ]
-
-    COMPILE_ARGS = [
-        f"-I{SAPNWRFC_HOME}\\include",
-        f"-I{PYTHONSOURCE}\\Include",
-        f"-I{PYTHONSOURCE}\\Include\\PC",
-        "/EHs",
-        "/GL",
-        "/Gy",
-        "/J",
-        "/MD",
-        "/nologo",
-        "/O2",
-        "/Oy-",
-        "/we4552",
-        "/we4700",
-        "/we4789",
-        "/W3",
-        "/Z7",
-    ]
-
-    LINK_ARGS = [
-        f"-LIBPATH:{SAPNWRFC_HOME}\\lib",
-        f"-LIBPATH:{PYTHONSOURCE}\\PCbuild",
-        "/NXCOMPAT",
-        "/STACK:0x2000000",
-        "/SWAPRUN:NET",
-        "/DEBUG",
-        "/OPT:REF",
-        "/DEBUGTYPE:CV,FIXUP",
-        "/MACHINE:amd64",
-        "/nologo",
-        "/LTCG",
-    ]
-elif sys.platform.startswith("darwin"):
-    os.system('strings $SAPNWRFC_HOME/lib/libsapnwrfc.dylib | grep "Patch Level"')
-    MACOS_VERSION_MIN = "10.15"
-
-    LIBS = ["sapnwrfc", "sapucum"]
-    MACROS = [
-        ("NDEBUG", None),
-        ("_LARGEFILE_SOURCE", None),
-        ("_CONSOLE", None),
-        ("_FILE_OFFSET_BITS", 64),
-        ("SAPonUNIX", None),
-        ("SAPwithUNICODE", None),
-        ("SAPwithTHREADS", None),
-        ("SAPonDARW", None),
-    ]
-    COMPILE_ARGS = [
-        "-Wall",
-        "-O2",
-        "-fexceptions",
-        "-funsigned-char",
-        "-fno-strict-aliasing",
-        "-Wno-uninitialized",
-        "-Wcast-align",
-        "-fPIC",
-        "-pthread",
-        "-minline-all-stringops",
-        "-isystem",
-        "-std=c++11",
-        f"-mmacosx-version-min={MACOS_VERSION_MIN}",
-        f"-I{SAPNWRFC_HOME}/include",
-        "-Wno-cast-align",
-        "-Wno-deprecated-declarations",
-        "-Wno-unused-function",
-        "-Wno-nullability-completeness",
-        "-Wno-expansion-to-defined",
-        "-Wno-unreachable-code-fallthrough",
-    ]
-    LINK_ARGS = [
-        f"-L{SAPNWRFC_HOME}/lib",
-        "-stdlib=libc++",
-        f"-mmacosx-version-min={MACOS_VERSION_MIN}",
-        # https://stackoverflow.com/questions/6638500/how-to-specify-rpath-in-a-makefile
-        f"-Wl,-rpath,{SAPNWRFC_HOME}/lib",
-    ]
-else:
-    sys.exit(f"Platform not supported: {sys.platform}.")
+    sys.exit(
+        "Environment variable SAPNWRFC_HOME not set.\n"
+        "Please specify this variable with the root directory of the SAP NWRFC Library."
+    )
 
+build_options = get_build_options(sys.platform)
 
-# https://docs.python.org/2/distutils/apiref.html
 PYRFC_EXT = Extension(
     language="c++",
-    name=f"{PACKAGE_NAME}.{MODULE_NAME}",
-    sources=[f"src/{PACKAGE_NAME}/{MODULE_NAME}.pyx"],
-    define_macros=MACROS,
-    extra_compile_args=COMPILE_ARGS,
-    extra_link_args=LINK_ARGS,
-    libraries=LIBS,
+    name=f"{package_name}._cyrfc",
+    sources=[f"src/{package_name}/_cyrfc.pyx"],
+    define_macros=build_options["MACROS"],
+    extra_compile_args=build_options["COMPILE_ARGS"],
+    extra_link_args=build_options["LINK_ARGS"],
+    libraries=build_options["LIBS"],
 )
 
-# cf. http://docs.python.org/distutils/setupscript.html#additional-meta-data
 setup(
-    name=PACKAGE_NAME,
+    name=package_name,
     # install_requires=["setuptools"],
     cmdclass=CMDCLASS,  # type: ignore
     ext_modules=cythonize(PYRFC_EXT, annotate=True, compiler_directives={"language_level": "3"})  # type: ignore
-    if BUILD_CYTHON
+    if build_cython
     else [PYRFC_EXT],  # type: ignore
-    test_suite=MODULE_NAME,
+    test_suite="tests"
 )
```

### Comparing `pyrfc-2.8.3/src/pyrfc/_cyrfc.cpp` & `pyrfc-3.0.0a0/src/pyrfc/_cyrfc.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2197,15 +2197,14 @@
 static const char __pyx_k_serve[] = "serve";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_sysId[] = "sysId";
 static const char __pyx_k_sysid[] = "sysid";
 static const char __pyx_k_trace[] = "trace";
 static const char __pyx_k_upper[] = "upper";
-static const char __pyx_k_utils[] = "_utils";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Server[] = "Server";
 static const char __pyx_k_Thread[] = "Thread";
 static const char __pyx_k_Values[] = "\n Values: ";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_cancel[] = "cancel";
 static const char __pyx_k_client[] = "client";
@@ -2297,15 +2296,14 @@
 static const char __pyx_k_but_found[] = ", but found ";
 static const char __pyx_k_call_type[] = "call_type";
 static const char __pyx_k_committed[] = "committed";
 static const char __pyx_k_confirmed[] = "confirmed";
 static const char __pyx_k_direction[] = "direction";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_errorInfo[] = "errorInfo";
-static const char __pyx_k_exception[] = "_exception";
 static const char __pyx_k_func_name[] = "func_name";
 static const char __pyx_k_int_field[] = "int_field";
 static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_kernelRel[] = "kernelRel";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_msg_class[] = "msg_class";
 static const char __pyx_k_not_found[] = "not_found";
@@ -2393,14 +2391,15 @@
 static const char __pyx_k_UnitCallType[] = "UnitCallType";
 static const char __pyx_k_confirm_unit[] = "_confirm_unit";
 static const char __pyx_k_destroy_unit[] = "_destroy_unit";
 static const char __pyx_k_kernel_trace[] = "kernel_trace";
 static const char __pyx_k_must_be_in_2[] = "' must be in '";
 static const char __pyx_k_protocolType[] = "protocolType";
 static const char __pyx_k_pyrfc__cyrfc[] = "pyrfc._cyrfc";
+static const char __pyx_k_pyrfc__utils[] = "pyrfc._utils";
 static const char __pyx_k_sapnwrfc_ini[] = "sapnwrfc.ini";
 static const char __pyx_k_sending_date[] = "sending_date";
 static const char __pyx_k_sending_time[] = "sending_time";
 static const char __pyx_k_server_log_2[] = "server_log";
 static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_unit_history[] = "unit_history";
@@ -2459,14 +2458,15 @@
 static const char __pyx_k_ABAPRuntimeError[] = "ABAPRuntimeError";
 static const char __pyx_k_ServerConnection[] = "ServerConnection";
 static const char __pyx_k_Unknown_RFC_type[] = "Unknown RFC type ";
 static const char __pyx_k_currentBusyCount[] = "currentBusyCount";
 static const char __pyx_k_direction_string[] = "'direction' (string) '";
 static const char __pyx_k_func_desc_handle[] = "func_desc_handle";
 static const char __pyx_k_is_not_supported[] = "' is not supported";
+static const char __pyx_k_pyrfc__exception[] = "pyrfc._exception";
 static const char __pyx_k_server_functions[] = "server_functions";
 static const char __pyx_k_set_locale_radix[] = "set_locale_radix";
 static const char __pyx_k_type_description[] = "type_description";
 static const char __pyx_k_RFCTYPE_STRUCTURE[] = "RFCTYPE_STRUCTURE";
 static const char __pyx_k_RFCTYPE_UTCMINUTE[] = "RFCTYPE_UTCMINUTE";
 static const char __pyx_k_RFCTYPE_UTCSECOND[] = "RFCTYPE_UTCSECOND";
 static const char __pyx_k_Server_connection[] = "Server connection";
@@ -2837,15 +2837,14 @@
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enum;
 static PyObject *__pyx_n_s_enum_names;
 static PyObject *__pyx_n_s_enum_values;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_errorInfo;
 static PyObject *__pyx_n_s_exc_info;
-static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_executed;
 static PyObject *__pyx_kp_u_field;
 static PyObject *__pyx_kp_u_field_name_string;
 static PyObject *__pyx_kp_u_field_name_string_2;
 static PyObject *__pyx_n_s_field_type;
 static PyObject *__pyx_n_u_field_type;
 static PyObject *__pyx_kp_u_field_type_string;
@@ -2977,14 +2976,16 @@
 static PyObject *__pyx_n_u_port;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_u_progName;
 static PyObject *__pyx_n_u_program;
 static PyObject *__pyx_n_u_protocolType;
 static PyObject *__pyx_n_s_pyrfc__cyrfc;
+static PyObject *__pyx_n_s_pyrfc__exception;
+static PyObject *__pyx_n_s_pyrfc__utils;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_queue_name;
 static PyObject *__pyx_n_s_queue_names;
 static PyObject *__pyx_n_s_queued;
 static PyObject *__pyx_n_u_queued;
 static PyObject *__pyx_kp_u_raises_ABAPApplicationError;
@@ -3087,15 +3088,14 @@
 static PyObject *__pyx_n_u_unit_history;
 static PyObject *__pyx_n_s_unit_id;
 static PyObject *__pyx_n_u_unit_identifier;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_upper;
 static PyObject *__pyx_n_u_user;
 static PyObject *__pyx_n_s_utcnow;
-static PyObject *__pyx_n_s_utils;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_kp_u_when_filling;
 static PyObject *__pyx_kp_u_when_getting_server_context_for;
 static PyObject *__pyx_kp_u_when_wrapping;
 static PyObject *__pyx_kp_u_with;
 static PyObject *__pyx_n_s_wrap;
 static PyObject *__pyx_kp_u_wrapString_uclen_u_utf8_size_u;
@@ -42663,15 +42663,14 @@
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
   {&__pyx_n_s_enum_names, __pyx_k_enum_names, sizeof(__pyx_k_enum_names), 0, 0, 1, 1},
   {&__pyx_n_s_enum_values, __pyx_k_enum_values, sizeof(__pyx_k_enum_values), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_errorInfo, __pyx_k_errorInfo, sizeof(__pyx_k_errorInfo), 0, 0, 1, 1},
   {&__pyx_n_s_exc_info, __pyx_k_exc_info, sizeof(__pyx_k_exc_info), 0, 0, 1, 1},
-  {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_executed, __pyx_k_executed, sizeof(__pyx_k_executed), 0, 0, 1, 1},
   {&__pyx_kp_u_field, __pyx_k_field, sizeof(__pyx_k_field), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string, __pyx_k_field_name_string, sizeof(__pyx_k_field_name_string), 0, 1, 0, 0},
   {&__pyx_kp_u_field_name_string_2, __pyx_k_field_name_string_2, sizeof(__pyx_k_field_name_string_2), 0, 1, 0, 0},
   {&__pyx_n_s_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 0, 1, 1},
   {&__pyx_n_u_field_type, __pyx_k_field_type, sizeof(__pyx_k_field_type), 0, 1, 0, 1},
   {&__pyx_kp_u_field_type_string, __pyx_k_field_type_string, sizeof(__pyx_k_field_type_string), 0, 1, 0, 0},
@@ -42803,14 +42802,16 @@
   {&__pyx_n_u_port, __pyx_k_port, sizeof(__pyx_k_port), 0, 1, 0, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_u_progName, __pyx_k_progName, sizeof(__pyx_k_progName), 0, 1, 0, 1},
   {&__pyx_n_u_program, __pyx_k_program, sizeof(__pyx_k_program), 0, 1, 0, 1},
   {&__pyx_n_u_protocolType, __pyx_k_protocolType, sizeof(__pyx_k_protocolType), 0, 1, 0, 1},
   {&__pyx_n_s_pyrfc__cyrfc, __pyx_k_pyrfc__cyrfc, sizeof(__pyx_k_pyrfc__cyrfc), 0, 0, 1, 1},
+  {&__pyx_n_s_pyrfc__exception, __pyx_k_pyrfc__exception, sizeof(__pyx_k_pyrfc__exception), 0, 0, 1, 1},
+  {&__pyx_n_s_pyrfc__utils, __pyx_k_pyrfc__utils, sizeof(__pyx_k_pyrfc__utils), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_queue_name, __pyx_k_queue_name, sizeof(__pyx_k_queue_name), 0, 0, 1, 1},
   {&__pyx_n_s_queue_names, __pyx_k_queue_names, sizeof(__pyx_k_queue_names), 0, 0, 1, 1},
   {&__pyx_n_s_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 0, 1, 1},
   {&__pyx_n_u_queued, __pyx_k_queued, sizeof(__pyx_k_queued), 0, 1, 0, 1},
   {&__pyx_kp_u_raises_ABAPApplicationError, __pyx_k_raises_ABAPApplicationError, sizeof(__pyx_k_raises_ABAPApplicationError), 0, 1, 0, 0},
@@ -42913,15 +42914,14 @@
   {&__pyx_n_u_unit_history, __pyx_k_unit_history, sizeof(__pyx_k_unit_history), 0, 1, 0, 1},
   {&__pyx_n_s_unit_id, __pyx_k_unit_id, sizeof(__pyx_k_unit_id), 0, 0, 1, 1},
   {&__pyx_n_u_unit_identifier, __pyx_k_unit_identifier, sizeof(__pyx_k_unit_identifier), 0, 1, 0, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_upper, __pyx_k_upper, sizeof(__pyx_k_upper), 0, 0, 1, 1},
   {&__pyx_n_u_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 1, 0, 1},
   {&__pyx_n_s_utcnow, __pyx_k_utcnow, sizeof(__pyx_k_utcnow), 0, 0, 1, 1},
-  {&__pyx_n_s_utils, __pyx_k_utils, sizeof(__pyx_k_utils), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_kp_u_when_filling, __pyx_k_when_filling, sizeof(__pyx_k_when_filling), 0, 1, 0, 0},
   {&__pyx_kp_u_when_getting_server_context_for, __pyx_k_when_getting_server_context_for, sizeof(__pyx_k_when_getting_server_context_for), 0, 1, 0, 0},
   {&__pyx_kp_u_when_wrapping, __pyx_k_when_wrapping, sizeof(__pyx_k_when_wrapping), 0, 1, 0, 0},
   {&__pyx_kp_u_with, __pyx_k_with, sizeof(__pyx_k_with), 0, 1, 0, 0},
   {&__pyx_n_s_wrap, __pyx_k_wrap, sizeof(__pyx_k_wrap), 0, 0, 1, 1},
   {&__pyx_kp_u_wrapString_uclen_u_utf8_size_u, __pyx_k_wrapString_uclen_u_utf8_size_u, sizeof(__pyx_k_wrapString_uclen_u_utf8_size_u), 0, 1, 0, 0},
@@ -44151,15 +44151,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":17
  * from sys import exc_info, platform
  * import socket
  * from threading import Thread, Timer             # <<<<<<<<<<<<<<
  * 
- * from . csapnwrfc cimport *
+ * from pyrfc.csapnwrfc cimport *
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Thread);
   __Pyx_GIVEREF(__pyx_n_s_Thread);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Thread);
   __Pyx_INCREF(__pyx_n_s_Timer);
@@ -44176,46 +44176,46 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Timer, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pyrfc/_cyrfc.pyx":20
  * 
- * from . csapnwrfc cimport *
- * from . _exception import *             # <<<<<<<<<<<<<<
- * from . _utils import enum_names, enum_values
+ * from pyrfc.csapnwrfc cimport *
+ * from pyrfc._exception import *             # <<<<<<<<<<<<<<
+ * from pyrfc._utils import enum_names, enum_values
  * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s__51);
   __Pyx_GIVEREF(__pyx_n_s__51);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__51);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pyrfc__exception, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyrfc/_cyrfc.pyx":21
- * from . csapnwrfc cimport *
- * from . _exception import *
- * from . _utils import enum_names, enum_values             # <<<<<<<<<<<<<<
+ * from pyrfc.csapnwrfc cimport *
+ * from pyrfc._exception import *
+ * from pyrfc._utils import enum_names, enum_values             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_enum_names);
   __Pyx_GIVEREF(__pyx_n_s_enum_names);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_enum_names);
   __Pyx_INCREF(__pyx_n_s_enum_values);
   __Pyx_GIVEREF(__pyx_n_s_enum_values);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_enum_values);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_utils, __pyx_t_2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pyrfc__utils, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_enum_names); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_enum_names, __pyx_t_2) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_enum_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
```

### Comparing `pyrfc-2.8.3/src/pyrfc/_cyrfc.pyx` & `pyrfc-3.0.0a0/src/pyrfc/_cyrfc.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from enum import Enum, auto
 from locale import localeconv
 from os.path import isfile, join
 from sys import exc_info, platform
 import socket
 from threading import Thread, Timer
 
-from . csapnwrfc cimport *
-from . _exception import *
-from . _utils import enum_names, enum_values
+from pyrfc.csapnwrfc cimport *
+from pyrfc._exception import *
+from pyrfc._utils import enum_names, enum_values
 
 
 ################################################################################
 # Configuration options
 ################################################################################
 
 # configuration bitmasks, internal use
```

### Comparing `pyrfc-2.8.3/src/pyrfc/_exception.py` & `pyrfc-3.0.0a0/src/pyrfc/_exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # SPDX-FileCopyrightText: 2013 SAP SE Srdjan Boskovic <srdjan.boskovic@sap.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-""" :mod:`pyrfc`-specific exception classes
-"""
+""":mod:`pyrfc`-specific exception classes."""
 
 from enum import Enum, auto
-from . _utils import enum_values
+from pyrfc._utils import enum_values
 
 
 class RFCError(Exception):
-    """Exception base class
+    """Exception base class.
 
     Indicates that there was an error in the Python connector.
     """
 
-    pass
-
 
 class RFCLibError(RFCError):
-    """RFC library error
+    """RFC library error.
 
     Base class for exceptions raised by the local underlying C connector (sapnwrfc.c).
     """
 
     def __init__(
         self,
         message=None,
@@ -33,60 +30,58 @@
         msg_type=None,
         msg_number=None,
         msg_v1=None,
         msg_v2=None,
         msg_v3=None,
         msg_v4=None,
     ):
+        """Init RFCLibError class."""
         super(RFCLibError, self).__init__(message)
         self.message = message  # Exception.message removed in Py3
         self.code = code
         self.key = key
         self.msg_class = msg_class
         self.msg_type = msg_type
         self.msg_number = msg_number
         self.msg_v1 = msg_v1
         self.msg_v2 = msg_v2
         self.msg_v3 = msg_v3
         self.msg_v4 = msg_v4
 
     def __str__(self):
+        """Convert RFCLibError object to string."""
         code = 28 if self.code is None else self.code  # 28 = RFC_UNKNOWN_ERROR
         rc_text = RcCodeText(code).value if code in enum_values(RcCodeText) else "??"
         return (
             f"{rc_text} (rc={self.code}): key={self.key}, message={self.message}"
             f" [MSG: class={self.msg_class}, type={self.msg_type}, number={self.msg_number},"
             f" v1-4:={self.msg_v1};{self.msg_v2};{self.msg_v3};{self.msg_v4}]"
         )
 
 
 class ABAPApplicationError(RFCLibError):
-    """ABAP application error
+    """ABAP application error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     ABAP_APPLICATION_FAILURE.
     """
 
-    pass
-
 
 class ABAPRuntimeError(RFCLibError):
-    """ABAP runtime error
+    """ABAP runtime error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     ABAP_RUNTIME_FAILURE.
     """
 
-    pass
-
 
 class LogonError(RFCLibError):
-    """Logon error
+    """Logon error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     LOGON_FAILURE.
     """
 
     def __init__(
@@ -98,14 +93,15 @@
         msg_type=None,
         msg_number=None,
         msg_v1=None,
         msg_v2=None,
         msg_v3=None,
         msg_v4=None,
     ):
+        """Init LogonError."""
         # Setting default values allows for raising an error with one parameter.
         super(LogonError, self).__init__(
             message,
             code,
             key,
             msg_class,
             msg_type,
@@ -114,69 +110,61 @@
             msg_v2,
             msg_v3,
             msg_v4,
         )
 
 
 class CommunicationError(RFCLibError):
-    """Communication error
+    """Communication error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     COMMUNICATION_FAILURE.
     """
 
-    pass
-
 
 class ExternalRuntimeError(RFCLibError):
-    """External runtime error
+    """External runtime error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     EXTERNAL_RUNTIME_FAILURE.
     """
 
-    pass
-
 
 class ExternalApplicationError(RFCLibError):
-    """External application error
+    """External application error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     EXTERNAL_APPLICATION_FAILURE.
     """
 
-    pass
-
 
 class ExternalAuthorizationError(RFCLibError):
-    """External authorization error
+    """External authorization error.
 
     This exception is raised if a RFC call returns an RC code greater than 0
     and the error object has an RFC_ERROR_GROUP value of
     EXTERNAL_AUTHORIZATION_FAILURE.
     """
 
-    pass
-
 
 class RFCTypeError(RFCLibError):
-    """Type concersion error
+    """Type concersion error.
 
     This exception is raised when invalid data type detected in RFC input (fill) conversion
     and the error object has an RFC_ERROR_GROUP value of
     RFC_TYPE_ERROR
     """
 
-    pass
-
 
 class RcCodeText(Enum):
+    """RFC library return codes."""
+
     RFC_OK = auto()
     RFC_COMMUNICATION_FAILURE = auto()
     RFC_LOGON_FAILURE = auto()
     RFC_ABAP_RUNTIME_FAILURE = auto()
     RFC_ABAP_MESSAGE = auto()
     RFC_ABAP_EXCEPTION = auto()
     RFC_CLOSED = auto()
```

### Comparing `pyrfc-2.8.3/src/pyrfc/csapnwrfc.pxd` & `pyrfc-3.0.0a0/src/pyrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `pyrfc-2.8.3/src/pyrfc.egg-info/PKG-INFO` & `pyrfc-3.0.0a0/src/pyrfc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrfc
-Version: 2.8.3
+Version: 3.0.0a0
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
+Author-email: srdjan.boskovic@sap.com
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
         http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
         AND DISTRIBUTION
@@ -209,48 +210,49 @@
         
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         
         See the License for the specific language governing permissions and
         
         limitations under the License.
         
-Project-URL: homepage, https://github.com/SAP/PyRFC
+Project-URL: bug-tracker, https://github.com/wntrblm/nox/issues
 Project-URL: documentation, http://sap.github.io/PyRFC
+Project-URL: homepage, https://github.com/SAP/PyRFC
 Project-URL: repository, https://github.com/SAP/PyRFC.git
 Keywords: pyrfc,sap,nwrfc,sapnwrfc,abap
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyrfc)](https://pypi.org/project/pyrfc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrfc)](https://pypi.org/project/pyrfc/)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyrfc)](https://pypistats.org/packages/pyrfc)
 [![REUSE status](https://api.reuse.software/badge/github.com/SAP/PyRFC)](https://api.reuse.software/info/github.com/SAP/PyRFC)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4349/badge)](https://bestpractices.coreinfrastructure.org/projects/4349)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 - [Features](#features)
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
@@ -324,29 +326,31 @@
 
 Cython must be installed upfront because the build from source is standard installation method on Linux.
 
 Build from source can be requested also on other platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
-# or
-PYRFC_BUILD_CYTHON=yes pip install pyrfc --no-binary :all:
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
 python -m pip install .
 # or
 python -m build --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
+Run ``python`` and type ``from pyrfc import *``. If this finishes silently, without oputput, the installation was successful.
+
+Using virtual environments you can isolate Python/PyRFC projects, working without administrator privileges.
+
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
 
 **Note:** The package must be [installed](#download-and-installation) before use.
```

