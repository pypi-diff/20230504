# Comparing `tmp/pyneweb-0.1.0.tar.gz` & `tmp/pyneweb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneweb-0.1.0.tar", last modified: Thu May  4 18:49:55 2023, max compression
+gzip compressed data, was "pyneweb-0.2.0.tar", last modified: Thu May  4 19:30:20 2023, max compression
```

## Comparing `pyneweb-0.1.0.tar` & `pyneweb-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 18:49:55.454424 pyneweb-0.1.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.1.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 18:49:55.454204 pyneweb-0.1.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.1.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 18:49:55.451736 pyneweb-0.1.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.1.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1262 2023-05-04 18:25:55.000000 pyneweb-0.1.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-04 17:09:49.000000 pyneweb-0.1.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.1.0/logic/states.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6206 2023-05-04 18:29:03.000000 pyneweb-0.1.0/logic/utilities.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 18:49:55.453461 pyneweb-0.1.0/pyneweb.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       51 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-04 18:49:55.000000 pyneweb-0.1.0/pyneweb.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-04 18:49:55.454476 pyneweb-0.1.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-04 18:48:45.000000 pyneweb-0.1.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 18:49:55.453659 pyneweb-0.1.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.1.0/tests/test_pass.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.437101 pyneweb-0.2.0/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-05-04 18:35:57.000000 pyneweb-0.2.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 19:30:20.436877 pyneweb-0.2.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4042 2023-05-04 18:48:17.000000 pyneweb-0.2.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.434897 pyneweb-0.2.0/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-02 16:20:24.000000 pyneweb-0.2.0/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1253 2023-05-04 18:56:48.000000 pyneweb-0.2.0/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5504 2023-05-04 17:09:49.000000 pyneweb-0.2.0/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      197 2023-05-04 18:00:23.000000 pyneweb-0.2.0/logic/states.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6206 2023-05-04 18:29:03.000000 pyneweb-0.2.0/logic/utilities.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.436277 pyneweb-0.2.0/pyneweb.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      315 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-04 19:30:20.000000 pyneweb-0.2.0/pyneweb.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-04 19:30:20.437166 pyneweb-0.2.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1107 2023-05-04 19:29:48.000000 pyneweb-0.2.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-04 19:30:20.436471 pyneweb-0.2.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-04 18:31:36.000000 pyneweb-0.2.0/tests/test_pass.py
```

### Comparing `pyneweb-0.1.0/LICENSE` & `pyneweb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneweb-0.1.0/PKG-INFO` & `pyneweb-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.1.0
+Version: 0.2.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.1.0/README.md` & `pyneweb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyneweb-0.1.0/logic/cli.py` & `pyneweb-0.2.0/logic/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     click.echo(f"Generated {len(file_list)} files in the 'logic' directory:")
     for files in file_list:
         click.echo(f"● {files}")
     click.echo()
 
 
 @click.group()
-def pynescript():
+def pyneweb():
     pass
 
 
-pynescript.add_command(init)
+pyneweb.add_command(init)
 
 if __name__ == "__main__":
-    pynescript()
+    pyneweb()
```

### Comparing `pyneweb-0.1.0/logic/script.py` & `pyneweb-0.2.0/logic/script.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.1.0/logic/utilities.py` & `pyneweb-0.2.0/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `pyneweb-0.1.0/pyneweb.egg-info/PKG-INFO` & `pyneweb-0.2.0/pyneweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneweb
-Version: 0.1.0
+Version: 0.2.0
 Summary: Web Boilerplate for Pynecone
 Home-page: https://github.com/LineIndent/pyneweb
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneweb-0.1.0/setup.py` & `pyneweb-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name="pyneweb",
-    version="0.1.0",
+    version="0.2.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Pynecone",
     long_description="Pyneweb is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Pynecone. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their web applications, without the need to spend time setting up infrastructure or configuration.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/pyneweb",
     packages=["logic"],
     install_requires=["click==8.1.3", "pynecone==0.1.28", "PyYAML==6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
-        "console_scripts": ["pynescript-init=logic.cli:init"],
+        "console_scripts": ["pyneweb-init=logic.cli:init"],
     },
     keywords=["python web template", "web application", "development"],
 )
```

