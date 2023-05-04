# Comparing `tmp/typst_pyimage-0.0.1.tar.gz` & `tmp/typst_pyimage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typst_pyimage-0.0.1.tar", last modified: Thu Apr 27 18:25:54 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `typst_pyimage-0.0.1.tar` & `typst_pyimage-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-27 18:25:54.018011 typst_pyimage-0.0.1/
--rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/LICENSE
--rw-r--r--   0 kidger    (1000) kidger    (1000)    16362 2023-04-27 18:25:54.017011 typst_pyimage-0.0.1/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2706 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/README.md
--rw-r--r--   0 kidger    (1000) kidger    (1000)     1104 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/pyproject.toml
--rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-04-27 18:25:54.018011 typst_pyimage-0.0.1/setup.cfg
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-27 18:25:54.016011 typst_pyimage-0.0.1/typst_pyimage/
--rw-r--r--   0 kidger    (1000) kidger    (1000)       76 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/typst_pyimage/__init__.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)      350 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/typst_pyimage/__main__.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2708 2023-04-27 18:25:15.000000 typst_pyimage-0.0.1/typst_pyimage/run.py
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-27 18:25:54.017011 typst_pyimage-0.0.1/typst_pyimage.egg-info/
--rw-r--r--   0 kidger    (1000) kidger    (1000)    16362 2023-04-27 18:25:53.000000 typst_pyimage-0.0.1/typst_pyimage.egg-info/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)      289 2023-04-27 18:25:53.000000 typst_pyimage-0.0.1/typst_pyimage.egg-info/SOURCES.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-27 18:25:53.000000 typst_pyimage-0.0.1/typst_pyimage.egg-info/dependency_links.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)       18 2023-04-27 18:25:53.000000 typst_pyimage-0.0.1/typst_pyimage.egg-info/requires.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)       14 2023-04-27 18:25:53.000000 typst_pyimage-0.0.1/typst_pyimage.egg-info/top_level.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/typst_pyimage/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/typst_pyimage/__main__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/typst_pyimage/pyimage.typ
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/typst_pyimage/run.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/README.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    17333 2020-02-02 00:00:00.000000 typst_pyimage-0.0.2/PKG-INFO
```

### Comparing `typst_pyimage-0.0.1/LICENSE` & `typst_pyimage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typst_pyimage-0.0.1/PKG-INFO` & `typst_pyimage-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: typst_pyimage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Typst extension, adding support for generating figures using inline Python code
+Project-URL: repository, https://github.com/patrick-kidger/typst_pyimage
 Author-email: Patrick Kidger <contact@kidger.site>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,34 +201,33 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-        
-Project-URL: repository, https://github.com/patrick-kidger/typst_pyimage
-Keywords: typst,matplotlib,plotting
+License-File: LICENSE
+Keywords: matplotlib,plotting,typst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
+Requires-Dist: matplotlib>=3.7.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 <h1 align="center">typst_pyimage</h1>
 
 <p align="center">Wraps <a href="https://github.com/typst/typst">Typst</a> to support inline Python code for generating figures.</p>
 
 ## Example
 
-<img align="right" width="45%" src="./imgs/lotka_volterra.png">
+<img align="right" width="45%" src="https://raw.githubusercontent.com/patrick-kidger/typst_pyimage/main/imgs/lotka_volterra.png">
 
 ```typst
 #import ".typst_pyimage/pyimage.typ": pyimage
 
 Consider the Lotka--Volterra (predator-prey)
 equations:
 
@@ -274,24 +274,50 @@
 
 This requires that you're using Typst locally -- it won't work with the web app.
 
 ## Usage
 
 1. Import `pyimage.typ`. At the start of your `.typ` file, add the line `#import ".typst_pyimage/pyimage.typ": pyimage`.
 
-2. Use the `pyimage` function. This has syntax `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forward on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
+2. Use the `pyimage` function. This has syntax `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
 
 3. Compile or watch. Run either of the following two commands:
     ```
     python -m typst_pyimage compile your_file.typ
     python -m typst_pyimage watch your_file.typ
     ```
     This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
 
     The resulting images are saved in the `.typst_pyimage` folder.
 
+## Notes
+
+It's common to have an initial block of code that is in common to all `#pyimage("...")` calls (such as import statements, defining helpers etc). These can be placed in a `#pyimageinit("...")` directive.
+
+Each `#pyimage("...")` block is executed as a fresh module (i.e. as if each was a separate Python file), but with the same Python interpreter.
+
+Overall, this is essentially equivalent to the following Python code:
+```
+# main.py
+import pyimageinit
+import pyimage1
+import pyimage2
+
+# pyimageinit.py
+...  # your #pyimageinit("...") code
+
+# pyimage1.py
+from pyimageinit import *
+...  # your first #pyimage("...") code
+
+# pyimage2.py
+from pyimageinit import *
+...  # your second #pyimage("...") code
+```
+This means that e.g. any global caches will be shared across all `#pyimage("...")` calls. (Useful when using a library like JAX, which has a JIT compilation cache.)
+
 ## Limitations
 
 1. The watcher just extracts all the `pyimage("...")` blocks via regex, and runs them in the order that they appear in the file. This means that (a) the `"` character may not appear anywhere in the Python code (even if escaped), and (b) trying to call `pyimage` dynamically (i.e. not with a literal string at the top level of your program) will not work.
 2. Only `pyimage("...")` calls inside the single watched file are tracked.
 
 We could probably lift 1a and 2 with a bit of effort. PRs welcome.
```

### Comparing `typst_pyimage-0.0.1/README.md` & `typst_pyimage-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <h1 align="center">typst_pyimage</h1>
 
 <p align="center">Wraps <a href="https://github.com/typst/typst">Typst</a> to support inline Python code for generating figures.</p>
 
 ## Example
 
-<img align="right" width="45%" src="./imgs/lotka_volterra.png">
+<img align="right" width="45%" src="https://raw.githubusercontent.com/patrick-kidger/typst_pyimage/main/imgs/lotka_volterra.png">
 
 ```typst
 #import ".typst_pyimage/pyimage.typ": pyimage
 
 Consider the Lotka--Volterra (predator-prey)
 equations:
 
@@ -55,24 +55,50 @@
 
 This requires that you're using Typst locally -- it won't work with the web app.
 
 ## Usage
 
 1. Import `pyimage.typ`. At the start of your `.typ` file, add the line `#import ".typst_pyimage/pyimage.typ": pyimage`.
 
-2. Use the `pyimage` function. This has syntax `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forward on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
+2. Use the `pyimage` function. This has syntax `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
 
 3. Compile or watch. Run either of the following two commands:
     ```
     python -m typst_pyimage compile your_file.typ
     python -m typst_pyimage watch your_file.typ
     ```
     This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
 
     The resulting images are saved in the `.typst_pyimage` folder.
 
+## Notes
+
+It's common to have an initial block of code that is in common to all `#pyimage("...")` calls (such as import statements, defining helpers etc). These can be placed in a `#pyimageinit("...")` directive.
+
+Each `#pyimage("...")` block is executed as a fresh module (i.e. as if each was a separate Python file), but with the same Python interpreter.
+
+Overall, this is essentially equivalent to the following Python code:
+```
+# main.py
+import pyimageinit
+import pyimage1
+import pyimage2
+
+# pyimageinit.py
+...  # your #pyimageinit("...") code
+
+# pyimage1.py
+from pyimageinit import *
+...  # your first #pyimage("...") code
+
+# pyimage2.py
+from pyimageinit import *
+...  # your second #pyimage("...") code
+```
+This means that e.g. any global caches will be shared across all `#pyimage("...")` calls. (Useful when using a library like JAX, which has a JIT compilation cache.)
+
 ## Limitations
 
 1. The watcher just extracts all the `pyimage("...")` blocks via regex, and runs them in the order that they appear in the file. This means that (a) the `"` character may not appear anywhere in the Python code (even if escaped), and (b) trying to call `pyimage` dynamically (i.e. not with a literal string at the top level of your program) will not work.
 2. Only `pyimage("...")` calls inside the single watched file are tracked.
 
 We could probably lift 1a and 2 with a bit of effort. PRs welcome.
```

