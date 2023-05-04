# Comparing `tmp/mebuex-1.1.3.tar.gz` & `tmp/mebuex-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mebuex-1.1.3.tar", last modified: Thu Apr 13 23:41:04 2023, max compression
+gzip compressed data, was "mebuex-1.1.4.tar", last modified: Thu May  4 10:04:30 2023, max compression
```

## Comparing `mebuex-1.1.3.tar` & `mebuex-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-04-13 23:41:04.692325 mebuex-1.1.3/
--rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-10-22 08:39:43.000000 mebuex-1.1.3/LICENSE
--rw-r--r--   0 phd       (1000) phd       (1000)     3287 2023-04-13 23:41:04.692325 mebuex-1.1.3/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)     2544 2023-04-13 23:37:59.000000 mebuex-1.1.3/README.md
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-04-13 23:41:04.688992 mebuex-1.1.3/mebuex/
--rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-10-22 08:39:43.000000 mebuex-1.1.3/mebuex/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     3992 2022-10-22 08:39:43.000000 mebuex-1.1.3/mebuex/build_ext.py
--rw-r--r--   0 phd       (1000) phd       (1000)      799 2022-10-22 08:39:43.000000 mebuex-1.1.3/mebuex/extension.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-04-13 23:41:04.692325 mebuex-1.1.3/mebuex.egg-info/
--rw-r--r--   0 phd       (1000) phd       (1000)     3287 2023-04-13 23:41:04.000000 mebuex-1.1.3/mebuex.egg-info/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)      240 2023-04-13 23:41:04.000000 mebuex-1.1.3/mebuex.egg-info/SOURCES.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-04-13 23:41:04.000000 mebuex-1.1.3/mebuex.egg-info/dependency_links.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        6 2023-04-13 23:41:04.000000 mebuex-1.1.3/mebuex.egg-info/requires.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        7 2023-04-13 23:41:04.000000 mebuex-1.1.3/mebuex.egg-info/top_level.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      829 2023-04-13 23:38:57.000000 mebuex-1.1.3/pyproject.toml
--rw-r--r--   0 phd       (1000) phd       (1000)       38 2023-04-13 23:41:04.692325 mebuex-1.1.3/setup.cfg
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/
+-rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-07-13 11:17:33.000000 mebuex-1.1.4/LICENSE
+-rw-r--r--   0 phd       (1000) phd       (1000)     3397 2023-05-04 10:04:30.501773 mebuex-1.1.4/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)     2654 2023-05-04 10:01:39.000000 mebuex-1.1.4/README.md
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/mebuex/
+-rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-07-13 11:31:24.000000 mebuex-1.1.4/mebuex/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     4150 2023-05-04 09:59:53.000000 mebuex-1.1.4/mebuex/build_ext.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      799 2022-07-13 13:28:44.000000 mebuex-1.1.4/mebuex/extension.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/mebuex.egg-info/
+-rw-r--r--   0 phd       (1000) phd       (1000)     3397 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)      240 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/SOURCES.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/dependency_links.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        6 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/requires.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        7 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/top_level.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      829 2023-05-04 10:01:46.000000 mebuex-1.1.4/pyproject.toml
+-rw-r--r--   0 phd       (1000) phd       (1000)       38 2023-05-04 10:04:30.501773 mebuex-1.1.4/setup.cfg
```

### Comparing `mebuex-1.1.3/LICENSE` & `mebuex-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mebuex-1.1.3/PKG-INFO` & `mebuex-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mebuex
-Version: 1.1.3
+Version: 1.1.4
 Summary: Combining build_ext with the Meson build system
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License: MIT
 Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,18 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.4] - 2023-05-04
+#### Changed
+ - Be more verbose on `destpath` error in `build_ext.build_extension`.
+
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
 
 ### [1.1.2] - 2023-04-13
 #### Changed
  - Change to `pyproject.toml` install workflow.
```

### Comparing `mebuex-1.1.3/README.md` & `mebuex-1.1.4/mebuex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: mebuex
+Version: 1.1.4
+Summary: Combining build_ext with the Meson build system
+Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
+License: MIT
+Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
+Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Framework :: Setuptools Plugin
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Mebuex
 A setuptools `Extension` and `build_ext` wrapper for builds based on Meson.
 
 ## Usage
 Mebuex assumes that the structure of a package is as follows:
 ```
 root
@@ -52,14 +71,18 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.4] - 2023-05-04
+#### Changed
+ - Be more verbose on `destpath` error in `build_ext.build_extension`.
+
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
 
 ### [1.1.2] - 2023-04-13
 #### Changed
  - Change to `pyproject.toml` install workflow.
```

### Comparing `mebuex-1.1.3/mebuex/build_ext.py` & `mebuex-1.1.4/mebuex/build_ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             filename = ext.compiledname + self.get_ext_filename(fullname) \
                                               .split(modname)[-1]
             destpath = Path(cmd.build_lib) / pdir
             if not destpath.is_dir():
                 raise RuntimeError("Cannot copy built extension because the "
                                    "target directory does not exist. This "
                                    "likely indicates a missing sub-package in "
-                                   "the setup configuration.")
+                                   "the setup configuration.\nMore info:\n"
+                                   "  destpath: '" + str(destpath) + "'\n"
+                                   "  pdir:     '" + str(pdir) + "'")
             destname = (destpath / filename).resolve()
             copy_file((Path(buildpath) / filename).resolve(),
                       destname, verbose=self.verbose,
                 dry_run=self.dry_run
             )
             # end of adapted code from setuptools/command/build_ext.py.
         else:
```

### Comparing `mebuex-1.1.3/mebuex/extension.py` & `mebuex-1.1.4/mebuex/extension.py`

 * *Files identical despite different names*

### Comparing `mebuex-1.1.3/mebuex.egg-info/PKG-INFO` & `mebuex-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: mebuex
-Version: 1.1.3
-Summary: Combining build_ext with the Meson build system
-Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
-License: MIT
-Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
-Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Framework :: Setuptools Plugin
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mebuex
 A setuptools `Extension` and `build_ext` wrapper for builds based on Meson.
 
 ## Usage
 Mebuex assumes that the structure of a package is as follows:
 ```
 root
@@ -71,14 +52,18 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.4] - 2023-05-04
+#### Changed
+ - Be more verbose on `destpath` error in `build_ext.build_extension`.
+
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
 
 ### [1.1.2] - 2023-04-13
 #### Changed
  - Change to `pyproject.toml` install workflow.
```

