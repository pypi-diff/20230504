# Comparing `tmp/carchive-0.0.37.tar.gz` & `tmp/carchive-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.37.tar", last modified: Thu May  4 00:09:00 2023, max compression
+gzip compressed data, was "carchive-0.0.38.tar", last modified: Thu May  4 15:47:14 2023, max compression
```

## Comparing `carchive-0.0.37.tar` & `carchive-0.0.38.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 00:08:53.000000 carchive-0.0.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 00:09:00.231767 carchive-0.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 00:08:53.000000 carchive-0.0.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9118 2023-05-04 00:08:53.000000 carchive-0.0.37/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:09:00.231767 carchive-0.0.37/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 00:09:00.000000 carchive-0.0.37/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:09:00.231767 carchive-0.0.37/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3595 2023-05-04 00:08:53.000000 carchive-0.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.963598 carchive-0.0.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 15:47:10.000000 carchive-0.0.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 15:47:14.963598 carchive-0.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 15:47:10.000000 carchive-0.0.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.959597 carchive-0.0.38/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9118 2023-05-04 15:47:10.000000 carchive-0.0.38/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:14.963598 carchive-0.0.38/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:47:14.000000 carchive-0.0.38/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:47:14.963598 carchive-0.0.38/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3593 2023-05-04 15:47:10.000000 carchive-0.0.38/setup.py
```

### Comparing `carchive-0.0.37/LICENSE` & `carchive-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.37/carchive/__init__.py` & `carchive-0.0.38/carchive/__init__.py`

 * *Files identical despite different names*

### Comparing `carchive-0.0.37/setup.py` & `carchive-0.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.37"
+VERSION = "0.0.38"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -105,15 +105,15 @@
 	entry_points={
 	},
 	install_requires=[
 		#https://pygithub.readthedocs.io/en/latest/introduction.html
 		"PyGithub", #To search for Repositories
 		#https://stackoverflow.com/questions/32688688/how-to-write-setup-py-to-include-a-git-repository-as-a-dependency/54701434#54701434
 		#https://git2net.readthedocs.io/en/latest/
-		"git2net @ git+ssh://git@github.com/franceme/git2net.git", #To gather and run metrics on the Repositories
+		"git2net @ git+https://github.com/franceme/git2net.git", #To gather and run metrics on the Repositories
 		"splittr",
 		"waybackpy",
 		"mystring",
 		"pygit2",
 	],
 	include_package_data=True,
 	classifiers=[
```

