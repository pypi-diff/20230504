# Comparing `tmp/tybase-0.0.1.tar.gz` & `tmp/tybase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.0.1.tar", last modified: Wed May  3 23:49:14 2023, max compression
+gzip compressed data, was "tybase-0.0.2.tar", last modified: Thu May  4 00:03:59 2023, max compression
```

## Comparing `tybase-0.0.1.tar` & `tybase-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-03 23:49:14.029723 tybase-0.0.1/
--rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-03 23:49:14.029318 tybase-0.0.1/PKG-INFO
--rw-r--r--   0 zhangte    (501) staff       (20)       10 2023-05-03 23:47:36.000000 tybase-0.0.1/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-03 23:49:14.029871 tybase-0.0.1/setup.cfg
--rw-r--r--   0 zhangte    (501) staff       (20)      758 2023-05-03 23:49:11.000000 tybase-0.0.1/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-03 23:49:14.025986 tybase-0.0.1/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.1/tybase/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.1/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-03 23:49:14.028687 tybase-0.0.1/tybase.egg-info/
--rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-03 23:49:13.000000 tybase-0.0.1/tybase.egg-info/PKG-INFO
--rw-r--r--   0 zhangte    (501) staff       (20)      203 2023-05-03 23:49:14.000000 tybase-0.0.1/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-05-03 23:49:13.000000 tybase-0.0.1/tybase.egg-info/dependency_links.txt
--rw-r--r--   0 zhangte    (501) staff       (20)       20 2023-05-03 23:49:13.000000 tybase-0.0.1/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-05-03 23:49:13.000000 tybase-0.0.1/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.636821 tybase-0.0.2/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.2/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-04 00:03:59.636521 tybase-0.0.2/PKG-INFO
+-rw-r--r--   0 zhangte    (501) staff       (20)       10 2023-05-03 23:47:36.000000 tybase-0.0.2/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-04 00:03:59.636929 tybase-0.0.2/setup.cfg
+-rw-r--r--   0 zhangte    (501) staff       (20)      789 2023-05-04 00:03:27.000000 tybase-0.0.2/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.633835 tybase-0.0.2/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.2/tybase/__init__.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.2/tybase/datatest.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.2/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-04 00:03:59.635906 tybase-0.0.2/tybase.egg-info/
+-rw-r--r--   0 zhangte    (501) staff       (20)      438 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/PKG-INFO
+-rw-r--r--   0 zhangte    (501) staff       (20)      235 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)       20 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-05-04 00:03:59.000000 tybase-0.0.2/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.0.1/setup.py` & `tybase-0.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.0.1',
+    version='0.0.2',
+    include_package_data=True,
     description='用于存放自己常用的安装包',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
```

