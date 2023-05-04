# Comparing `tmp/carchive-0.0.36.tar.gz` & `tmp/carchive-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.36.tar", last modified: Tue Apr 25 14:12:31 2023, max compression
+gzip compressed data, was "carchive-0.0.37.tar", last modified: Thu May  4 00:09:00 2023, max compression
```

## Comparing `carchive-0.0.36.tar` & `carchive-0.0.37.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 14:12:28.000000 carchive-0.0.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 14:12:31.573751 carchive-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 14:12:28.000000 carchive-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16455 2023-04-25 14:12:28.000000 carchive-0.0.36/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:12:31.573751 carchive-0.0.36/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:12:31.000000 carchive-0.0.36/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:12:31.573751 carchive-0.0.36/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-04-25 14:12:28.000000 carchive-0.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 00:08:53.000000 carchive-0.0.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 00:09:00.231767 carchive-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 00:08:53.000000 carchive-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9118 2023-05-04 00:08:53.000000 carchive-0.0.37/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:09:00.231767 carchive-0.0.37/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3595 2023-05-04 00:08:53.000000 carchive-0.0.37/setup.py
```

### Comparing `carchive-0.0.36/LICENSE` & `carchive-0.0.37/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `carchive-0.0.36/setup.py` & `carchive-0.0.37/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.36"
+VERSION = "0.0.37"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -101,18 +101,23 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
-		"funbelts",
+		#https://pygithub.readthedocs.io/en/latest/introduction.html
+		"PyGithub", #To search for Repositories
+		#https://stackoverflow.com/questions/32688688/how-to-write-setup-py-to-include-a-git-repository-as-a-dependency/54701434#54701434
+		#https://git2net.readthedocs.io/en/latest/
+		"git2net @ git+ssh://git@github.com/franceme/git2net.git", #To gather and run metrics on the Repositories
+		"splittr",
 		"waybackpy",
-		"ghapi",
 		"mystring",
+		"pygit2",
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

