# Comparing `tmp/betweens-0.1.1.1.tar.gz` & `tmp/betweens-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.1.1.1.tar", last modified: Thu May  4 10:27:34 2023, max compression
+gzip compressed data, was "betweens-0.1.1.dev1.tar", last modified: Thu May  4 10:21:35 2023, max compression
```

## Comparing `betweens-0.1.1.1.tar` & `betweens-0.1.1.dev1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:34.437759 betweens-0.1.1.1/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.1.1.1/LICENSE
--rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1182 2023-05-04 10:27:34.437759 betweens-0.1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:34.422114 betweens-0.1.1.1/betweens/
--rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.1.1.1/betweens/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-05-03 12:10:19.000000 betweens-0.1.1.1/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-03 10:18:54.000000 betweens-0.1.1.1/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:34.437759 betweens-0.1.1.1/betweens.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-05-04 10:27:34.000000 betweens-0.1.1.1/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-04 10:27:34.000000 betweens-0.1.1.1/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:27:34.000000 betweens-0.1.1.1/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 10:27:34.000000 betweens-0.1.1.1/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-04 10:26:37.000000 betweens-0.1.1.1/new.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 10:27:34.437759 betweens-0.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1505 2023-05-04 10:26:15.000000 betweens-0.1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.1.1.dev1/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.1.1.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1166 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.1.1.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.255052 betweens-0.1.1.dev1/betweens/
+-rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.1.1.dev1/betweens/__init__.py
+-rw-rw-rw-   0        0        0     1678 2023-05-03 12:10:19.000000 betweens-0.1.1.dev1/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-03 10:18:54.000000 betweens-0.1.1.dev1/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2023-05-04 10:20:34.000000 betweens-0.1.1.dev1/new.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1506 2023-05-04 10:20:43.000000 betweens-0.1.1.dev1/setup.py
```

### Comparing `betweens-0.1.1.1/LICENSE` & `betweens-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.1.1.1/PKG-INFO` & `betweens-0.1.1.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.1.1.1
-Author: yuanbaoge
+Version: 0.1.1.dev1
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `betweens-0.1.1.1/betweens/betweens.py` & `betweens-0.1.1.dev1/betweens/betweens.py`

 * *Files identical despite different names*

### Comparing `betweens-0.1.1.1/betweens.egg-info/PKG-INFO` & `betweens-0.1.1.dev1/betweens.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 Metadata-Version: 2.1
 Name: betweens
-Version: 0.1.1.1
-Author: yuanbaoge
+Version: 0.1.1.dev1
 Author-email: yuanbaoge@outlook.com
 Keywords: pimm source manager
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `betweens-0.1.1.1/setup.py` & `betweens-0.1.1.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 long_description = None
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='betweens', # 包名称
       packages=find_packages(), # 需要处理的包目录
-      version='0.1.1.1', # 版本
+      version='0.1.1.dev1', # 版本
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python', 'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Operating System :: MacOS :: MacOS X',
           'Operating System :: Microsoft :: Windows :: Windows 10',
@@ -25,10 +25,10 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11'
       ],
       long_description=long_description,
       long_description_content_type='text/markdown',
-      author='yuanbaoge', # 作者
+      auth='yuanbaoge', # 作者
       author_email='yuanbaoge@outlook.com', # 作者邮箱
       keywords='pimm source manager')
```

