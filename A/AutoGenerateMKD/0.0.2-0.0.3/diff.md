# Comparing `tmp/AutoGenerateMKD-0.0.2.tar.gz` & `tmp/AutoGenerateMKD-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoGenerateMKD-0.0.2.tar", last modified: Thu May  4 17:11:09 2023, max compression
+gzip compressed data, was "AutoGenerateMKD-0.0.3.tar", last modified: Thu May  4 17:15:43 2023, max compression
```

## Comparing `AutoGenerateMKD-0.0.2.tar` & `AutoGenerateMKD-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:11:09.321448 AutoGenerateMKD-0.0.2/
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:11:09.315465 AutoGenerateMKD-0.0.2/AutoGenerateMKD/
--rw-r--r--   0 coseto     (501) staff       (20)        0 2023-05-04 17:07:10.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)     2007 2023-05-04 17:06:38.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD/main.py
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:11:09.318782 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)      408 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/SOURCES.txt
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/dependency_links.txt
--rw-r--r--   0 coseto     (501) staff       (20)      163 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/entry_points.txt
--rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/requires.txt
--rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-04 17:11:09.000000 AutoGenerateMKD-0.0.2/AutoGenerateMKD.egg-info/top_level.txt
--rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.2/LICENSE
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:11:09.320947 AutoGenerateMKD-0.0.2/PKG-INFO
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:11:09.320161 AutoGenerateMKD-0.0.2/mkdocs_pagenav_generator/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.2/mkdocs_pagenav_generator/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.2/mkdocs_pagenav_generator/plugin.py
--rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.2/pyproject.toml
--rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.2/requirements.txt
--rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-04 17:11:09.321605 AutoGenerateMKD-0.0.2/setup.cfg
--rw-r--r--   0 coseto     (501) staff       (20)     1173 2023-05-04 17:10:15.000000 AutoGenerateMKD-0.0.2/setup.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.772786 AutoGenerateMKD-0.0.3/
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.765979 AutoGenerateMKD-0.0.3/AutoGenerateMKD/
+-rw-r--r--   0 coseto     (501) staff       (20)        0 2023-05-04 17:07:10.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)     2007 2023-05-04 17:06:38.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD/main.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.769648 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)      408 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/SOURCES.txt
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/dependency_links.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      153 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/entry_points.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/requires.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/top_level.txt
+-rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.3/LICENSE
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:15:43.772297 AutoGenerateMKD-0.0.3/PKG-INFO
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.771150 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/plugin.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.3/pyproject.toml
+-rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.3/requirements.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-04 17:15:43.772917 AutoGenerateMKD-0.0.3/setup.cfg
+-rw-r--r--   0 coseto     (501) staff       (20)     1163 2023-05-04 17:15:24.000000 AutoGenerateMKD-0.0.3/setup.py
```

### Comparing `AutoGenerateMKD-0.0.2/AutoGenerateMKD/main.py` & `AutoGenerateMKD-0.0.3/AutoGenerateMKD/main.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.2/LICENSE` & `AutoGenerateMKD-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.2/mkdocs_pagenav_generator/plugin.py` & `AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/plugin.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.2/pyproject.toml` & `AutoGenerateMKD-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.2/setup.py` & `AutoGenerateMKD-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="AutoGenerateMKD",
-    version="0.0.2",
+    version="0.0.3",
     author="E-NoR,Teng",
     description="Auto generate markdown api docs, base on dosc.",
     packages=find_packages(),
     install_requires=[
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
@@ -22,15 +22,15 @@
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
     ],
     entry_points={
         "mkdocs.plugins": ["pagenav-generator = mkdocs_pagenav_generator.plugin:NavGeneratorPlugin"],
         "console_scripts": [
-            "auto-gen-markdown=your_package.auto_gen_markdown:main",
+            "auto-gen-markdown=AutoGenerateMKD.main:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

