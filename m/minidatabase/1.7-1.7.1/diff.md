# Comparing `tmp/minidatabase-1.7.tar.gz` & `tmp/minidatabase-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidatabase-1.7.tar", last modified: Wed May  3 09:57:23 2023, max compression
+gzip compressed data, was "minidatabase-1.7.1.tar", last modified: Thu May  4 04:36:55 2023, max compression
```

## Comparing `minidatabase-1.7.tar` & `minidatabase-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:57:23.508322 minidatabase-1.7/
--rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3840 2023-05-03 09:57:23.508322 minidatabase-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-05-03 04:09:53.000000 minidatabase-1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 09:57:23.478568 minidatabase-1.7/minidatabase/
--rw-rw-rw-   0        0        0     1873 2023-05-03 09:53:22.000000 minidatabase-1.7/minidatabase/WebMDB.py
--rw-rw-rw-   0        0        0       85 2023-05-02 13:13:38.000000 minidatabase-1.7/minidatabase/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.7/minidatabase/minidb.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:57:23.506523 minidatabase-1.7/minidatabase.egg-info/
--rw-rw-rw-   0        0        0     3840 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 09:57:23.000000 minidatabase-1.7/minidatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:57:23.509320 minidatabase-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-05-03 09:56:44.000000 minidatabase-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:36:55.034127 minidatabase-1.7.1/
+-rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3842 2023-05-04 04:36:55.033129 minidatabase-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-05-03 04:09:53.000000 minidatabase-1.7.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 04:36:55.019348 minidatabase-1.7.1/minidatabase/
+-rw-rw-rw-   0        0        0     1895 2023-05-04 04:32:23.000000 minidatabase-1.7.1/minidatabase/WebMDB.py
+-rw-rw-rw-   0        0        0       85 2023-05-02 13:13:38.000000 minidatabase-1.7.1/minidatabase/__init__.py
+-rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.7.1/minidatabase/minidb.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:36:55.031248 minidatabase-1.7.1/minidatabase.egg-info/
+-rw-rw-rw-   0        0        0     3842 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 04:36:54.000000 minidatabase-1.7.1/minidatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 04:36:55.034127 minidatabase-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1270 2023-05-04 04:33:27.000000 minidatabase-1.7.1/setup.py
```

### Comparing `minidatabase-1.7/LICENSE.txt` & `minidatabase-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minidatabase-1.7/PKG-INFO` & `minidatabase-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidatabase
-Version: 1.7
+Version: 1.7.1
 Summary: A tiny database system based on  python dictionary.
 Home-page: http://osdn.xyz
 Author: HansenL
 Author-email: hansenl@foxmail.com
 License:  GNU GENERAL PUBLIC LICENSE
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `minidatabase-1.7/README.rst` & `minidatabase-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `minidatabase-1.7/minidatabase/WebMDB.py` & `minidatabase-1.7.1/minidatabase/WebMDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,22 @@
     @app.route('/%s/search_tag/<keyword>'%passwd)
     def search_tags(keyword):
         return str(cursor.search_tag(keyword))
     @app.route('/%s/search_value/<keyword>'%passwd)
     def search_values(keyword):
         return str(cursor.search_value(keyword))
     app.run(port=p)
-
-if __name__ == "__main__":
-    if len(sys.argv)!=1:
+def main():
+    if len(sys.argv)==1:
         p=int(input("Please enter the service port->"))
         nzm=input("Please enter the MiniDataBase File name->")
         passwd=input("Please enter the Database Password ->")
         service(p,nzm,passwd)
     else:
         p=sys.argv[1]
         nzm=sys.argv[2]
         passwd=sys.argv[3]
         service(p,nzm,passwd)
+if __name__ == "__main__":
+    main()
```

### Comparing `minidatabase-1.7/minidatabase/minidb.py` & `minidatabase-1.7.1/minidatabase/minidb.py`

 * *Files identical despite different names*

### Comparing `minidatabase-1.7/minidatabase.egg-info/PKG-INFO` & `minidatabase-1.7.1/minidatabase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidatabase
-Version: 1.7
+Version: 1.7.1
 Summary: A tiny database system based on  python dictionary.
 Home-page: http://osdn.xyz
 Author: HansenL
 Author-email: hansenl@foxmail.com
 License:  GNU GENERAL PUBLIC LICENSE
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `minidatabase-1.7/setup.py` & `minidatabase-1.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r",encoding='gb18030',errors='ignore') as f:
   long_description = f.read()
 setup(name='minidatabase',  
-      version='1.7',  
+      version='1.7.1',  
       description='A tiny database system based on  python dictionary.',
       long_description=long_description,
       author='HansenL',
       author_email='hansenl@foxmail.com',
       url='http://osdn.xyz',
       install_requires=["requests","flask"],
       license=' GNU GENERAL PUBLIC LICENSE',
@@ -22,10 +22,10 @@
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Topic :: Software Development :: Libraries'
       ],
       entry_points={
-"console_scripts":["minidb=minidatabase.minidb:main","webmdb=minidatabase.WebMDB:service",],
+"console_scripts":["minidb=minidatabase.minidb:main","webmdb=minidatabase.WebMDB:main",],
           }
       )
```

