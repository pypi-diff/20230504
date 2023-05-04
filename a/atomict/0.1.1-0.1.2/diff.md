# Comparing `tmp/atomict-0.1.1.tar.gz` & `tmp/atomict-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomict-0.1.1.tar", last modified: Thu May  4 06:17:10 2023, max compression
+gzip compressed data, was "atomict-0.1.2.tar", last modified: Thu May  4 06:24:31 2023, max compression
```

## Comparing `atomict-0.1.1.tar` & `atomict-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1075 2023-04-23 02:34:41.000000 atomict-0.1.1/LICENSE
--rw-r--r--   0 alainr    (1000) alainr    (1000)       25 2023-05-04 06:16:54.000000 atomict-0.1.1/MANIFEST.in
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1309 2023-05-04 06:17:10.506263 atomict-0.1.1/PKG-INFO
--rw-r--r--   0 alainr    (1000) alainr    (1000)      441 2023-05-04 05:52:06.000000 atomict-0.1.1/README.md
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/atomict/
--rw-r--r--   0 alainr    (1000) alainr    (1000)       33 2023-04-23 02:50:32.000000 atomict-0.1.1/atomict/__init__.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)       30 2023-04-23 04:07:33.000000 atomict-0.1.1/atomict/__main__.py
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/atomict/auth/
--rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-04-23 02:52:03.000000 atomict-0.1.1/atomict/auth/__init__.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1379 2023-05-02 04:57:20.000000 atomict-0.1.1/atomict/cli.py
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/atomict/datasets/
--rw-r--r--   0 alainr    (1000) alainr    (1000)      614 2023-05-02 04:48:34.000000 atomict-0.1.1/atomict/datasets/__init__.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1143 2023-05-02 04:52:49.000000 atomict-0.1.1/atomict/datasets/io.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1255 2023-05-02 04:08:05.000000 atomict-0.1.1/atomict/datasets/public.py
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/atomict/utils/
--rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:49:52.000000 atomict-0.1.1/atomict/utils/__init__.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)      656 2023-05-02 04:54:29.000000 atomict-0.1.1/atomict/utils/requests.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)       75 2023-04-23 02:51:00.000000 atomict-0.1.1/atomict/version.py
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/atomict.egg-info/
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1309 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/PKG-INFO
--rw-r--r--   0 alainr    (1000) alainr    (1000)      527 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/SOURCES.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)        1 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/dependency_links.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)       40 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/entry_points.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)      733 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/requires.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)       14 2023-05-04 06:17:10.000000 atomict-0.1.1/atomict.egg-info/top_level.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)      733 2023-05-04 06:12:09.000000 atomict-0.1.1/requirements.txt
--rw-r--r--   0 alainr    (1000) alainr    (1000)       38 2023-05-04 06:17:10.506263 atomict-0.1.1/setup.cfg
--rw-r--r--   0 alainr    (1000) alainr    (1000)     1416 2023-05-04 05:46:39.000000 atomict-0.1.1/setup.py
-drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:17:10.506263 atomict-0.1.1/tests/
--rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:29:48.000000 atomict-0.1.1/tests/__init__.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:38:14.000000 atomict-0.1.1/tests/test_cli.py
--rw-r--r--   0 alainr    (1000) alainr    (1000)      215 2023-05-02 04:44:45.000000 atomict-0.1.1/tests/test_sdk.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1075 2023-04-23 02:34:41.000000 atomict-0.1.2/LICENSE
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       25 2023-05-04 06:16:54.000000 atomict-0.1.2/MANIFEST.in
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1309 2023-05-04 06:24:31.162303 atomict-0.1.2/PKG-INFO
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      441 2023-05-04 05:52:06.000000 atomict-0.1.2/README.md
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/atomict/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       33 2023-04-23 02:50:32.000000 atomict-0.1.2/atomict/__init__.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       30 2023-04-23 04:07:33.000000 atomict-0.1.2/atomict/__main__.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/atomict/auth/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-04-23 02:52:03.000000 atomict-0.1.2/atomict/auth/__init__.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1379 2023-05-02 04:57:20.000000 atomict-0.1.2/atomict/cli.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/atomict/datasets/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      614 2023-05-02 04:48:34.000000 atomict-0.1.2/atomict/datasets/__init__.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1143 2023-05-02 04:52:49.000000 atomict-0.1.2/atomict/datasets/io.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1255 2023-05-02 04:08:05.000000 atomict-0.1.2/atomict/datasets/public.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/atomict/utils/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:49:52.000000 atomict-0.1.2/atomict/utils/__init__.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      656 2023-05-02 04:54:29.000000 atomict-0.1.2/atomict/utils/requests.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       75 2023-05-04 06:22:51.000000 atomict-0.1.2/atomict/version.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/atomict.egg-info/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1309 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/PKG-INFO
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      527 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/SOURCES.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)        1 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/dependency_links.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       40 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/entry_points.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      712 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/requires.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       14 2023-05-04 06:24:31.000000 atomict-0.1.2/atomict.egg-info/top_level.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      712 2023-05-04 06:22:32.000000 atomict-0.1.2/requirements.txt
+-rw-r--r--   0 alainr    (1000) alainr    (1000)       38 2023-05-04 06:24:31.162303 atomict-0.1.2/setup.cfg
+-rw-r--r--   0 alainr    (1000) alainr    (1000)     1416 2023-05-04 06:22:40.000000 atomict-0.1.2/setup.py
+drwxr-xr-x   0 alainr    (1000) alainr    (1000)        0 2023-05-04 06:24:31.162303 atomict-0.1.2/tests/
+-rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:29:48.000000 atomict-0.1.2/tests/__init__.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)        0 2023-05-02 04:38:14.000000 atomict-0.1.2/tests/test_cli.py
+-rw-r--r--   0 alainr    (1000) alainr    (1000)      215 2023-05-02 04:44:45.000000 atomict-0.1.2/tests/test_sdk.py
```

### Comparing `atomict-0.1.1/LICENSE` & `atomict-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/PKG-INFO` & `atomict-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomict
-Version: 0.1.1
+Version: 0.1.2
 Summary: The client application for the https://atomictessellator.com/
 Home-page: https://github.com/AtomicTessellator/atomic_cli
 Author: Alain Richardt
 Author-email: alain@atomictessellator.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atomict-0.1.1/atomict/cli.py` & `atomict-0.1.2/atomict/cli.py`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict/datasets/__init__.py` & `atomict-0.1.2/atomict/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict/datasets/io.py` & `atomict-0.1.2/atomict/datasets/io.py`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict/datasets/public.py` & `atomict-0.1.2/atomict/datasets/public.py`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict/utils/requests.py` & `atomict-0.1.2/atomict/utils/requests.py`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict.egg-info/PKG-INFO` & `atomict-0.1.2/atomict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomict
-Version: 0.1.1
+Version: 0.1.2
 Summary: The client application for the https://atomictessellator.com/
 Home-page: https://github.com/AtomicTessellator/atomic_cli
 Author: Alain Richardt
 Author-email: alain@atomictessellator.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atomict-0.1.1/atomict.egg-info/SOURCES.txt` & `atomict-0.1.2/atomict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomict-0.1.1/atomict.egg-info/requires.txt` & `atomict-0.1.2/atomict.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 keyring==23.13.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 numpy==1.24.3
 packaging==23.1
 pandas==2.0.0
-pkg_resources==0.0.0
 pkginfo==1.9.6
 prettytable==3.7.0
 pycparser==2.21
 Pygments==2.15.1
 pyproject_hooks==1.0.0
 python-dateutil==2.8.2
 pytz==2023.3
```

### Comparing `atomict-0.1.1/requirements.txt` & `atomict-0.1.2/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 keyring==23.13.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 numpy==1.24.3
 packaging==23.1
 pandas==2.0.0
-pkg_resources==0.0.0
 pkginfo==1.9.6
 prettytable==3.7.0
 pycparser==2.21
 Pygments==2.15.1
 pyproject_hooks==1.0.0
 python-dateutil==2.8.2
 pytz==2023.3
```

### Comparing `atomict-0.1.1/setup.py` & `atomict-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     install_requires = [line.strip() for line in fh.readlines() if line.strip()]
 
 exec(open('atomict/version.py').read())
 
 setuptools.setup(
     name="atomict",
-    version="0.1.1",
+    version="0.1.2",
     author="Alain Richardt",
     author_email="alain@atomictessellator.com",
     description="The client application for the https://atomictessellator.com/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AtomicTessellator/atomic_cli",
     packages=setuptools.find_packages(),
```

