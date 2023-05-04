# Comparing `tmp/tcw-0.1.3.tar.gz` & `tmp/tcw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-0.1.3.tar", last modified: Thu May  4 16:18:46 2023, max compression
+gzip compressed data, was "tcw-0.1.4.tar", last modified: Thu May  4 16:32:17 2023, max compression
```

## Comparing `tcw-0.1.3.tar` & `tcw-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.628056 tcw-0.1.3/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.3/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 16:18:46.628056 tcw-0.1.3/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.3/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-05-04 16:18:46.628056 tcw-0.1.3/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-05-04 16:18:25.000000 tcw-0.1.3/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.616056 tcw-0.1.3/tcw/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.3/tcw/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.616056 tcw-0.1.3/tcw/apps/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.620056 tcw-0.1.3/tcw/apps/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.3/tcw/apps/contest/forms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.3/tcw/apps/contest/models.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.620056 tcw-0.1.3/tcw/apps/contest/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.624056 tcw-0.1.3/tcw/apps/contest/templates/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/about.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/animation.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/form.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/index.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/privacy.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2304 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/signup.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/slide1.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/slide2.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/slide3.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/sorry.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/success.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/apps/contest/templates/contest/thanks.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.3/tcw/apps/contest/views.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.3/tcw/config.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-04-14 11:51:00.000000 tcw-0.1.3/tcw/run.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.624056 tcw-0.1.3/tcw/static/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/static/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.624056 tcw-0.1.3/tcw/static/images/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/static/images/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.628056 tcw-0.1.3/tcw/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.3/tcw/templates/404.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.3/tcw/templates/410.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.3/tcw/templates/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2107 2023-05-04 15:45:27.000000 tcw-0.1.3/tcw/templates/base.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.3/tcw/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      186 2023-04-14 11:50:36.000000 tcw-0.1.3/tcw/wsgi.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:18:46.616056 tcw-0.1.3/tcw.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 16:18:46.000000 tcw-0.1.3/tcw.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1170 2023-05-04 16:18:46.000000 tcw-0.1.3/tcw.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-05-04 16:18:46.000000 tcw-0.1.3/tcw.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-05-04 16:18:46.000000 tcw-0.1.3/tcw.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-05-04 16:18:46.000000 tcw-0.1.3/tcw.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.546875 tcw-0.1.4/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.4/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 16:32:17.546875 tcw-0.1.4/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.4/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-05-04 16:32:17.546875 tcw-0.1.4/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      596 2023-05-04 16:31:53.000000 tcw-0.1.4/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.538878 tcw-0.1.4/tcw/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.4/tcw/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.538878 tcw-0.1.4/tcw/apps/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.542876 tcw-0.1.4/tcw/apps/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.4/tcw/apps/contest/forms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.4/tcw/apps/contest/models.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.542876 tcw-0.1.4/tcw/apps/contest/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.542876 tcw-0.1.4/tcw/apps/contest/templates/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1547 2023-04-04 23:59:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/about.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5820 2023-04-13 13:07:38.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/animation.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2078 2023-04-05 05:32:34.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/form.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      303 2023-04-06 18:51:38.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/index.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2222 2023-04-07 12:49:55.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/privacy.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2304 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/signup.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1735 2023-04-13 13:03:09.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/slide1.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      562 2023-04-13 13:03:16.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/slide2.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      219 2023-04-13 13:03:04.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/slide3.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/sorry.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2569 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/success.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      408 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/apps/contest/templates/contest/thanks.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.4/tcw/apps/contest/views.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.4/tcw/config.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-04-14 11:51:00.000000 tcw-0.1.4/tcw/run.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.542876 tcw-0.1.4/tcw/static/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/static/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.542876 tcw-0.1.4/tcw/static/images/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/static/images/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.546875 tcw-0.1.4/tcw/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1971 2023-04-04 18:51:43.000000 tcw-0.1.4/tcw/templates/404.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1960 2023-04-05 14:13:22.000000 tcw-0.1.4/tcw/templates/410.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.4/tcw/templates/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2268 2023-05-04 16:31:45.000000 tcw-0.1.4/tcw/templates/base.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.4/tcw/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      186 2023-04-14 11:50:36.000000 tcw-0.1.4/tcw/wsgi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-05-04 16:32:17.538878 tcw-0.1.4/tcw.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-05-04 16:32:17.000000 tcw-0.1.4/tcw.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1170 2023-05-04 16:32:17.000000 tcw-0.1.4/tcw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-05-04 16:32:17.000000 tcw-0.1.4/tcw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-05-04 16:32:17.000000 tcw-0.1.4/tcw.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-05-04 16:32:17.000000 tcw-0.1.4/tcw.egg-info/top_level.txt
```

### Comparing `tcw-0.1.3/LICENSE` & `tcw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/PKG-INFO` & `tcw-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.3
+Version: 0.1.4
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.3/README.md` & `tcw-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/setup.py` & `tcw-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw',
-    version='0.1.3',
+    version='0.1.4',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='tiny contest winners application',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
```

### Comparing `tcw-0.1.3/tcw/__init__.py` & `tcw-0.1.4/tcw/__init__.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/forms.py` & `tcw-0.1.4/tcw/apps/contest/forms.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/models.py` & `tcw-0.1.4/tcw/apps/contest/models.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/about.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/about.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/animation.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/animation.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/form.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/form.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/privacy.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/privacy.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/signup.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/signup.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/slide1.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/slide1.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/slide2.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/slide2.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/templates/contest/success.html` & `tcw-0.1.4/tcw/apps/contest/templates/contest/success.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/apps/contest/views.py` & `tcw-0.1.4/tcw/apps/contest/views.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/config.py` & `tcw-0.1.4/tcw/config.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/database.py` & `tcw-0.1.4/tcw/database.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/templates/404.html` & `tcw-0.1.4/tcw/templates/404.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/templates/410.html` & `tcw-0.1.4/tcw/templates/410.html`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw/templates/base.html` & `tcw-0.1.4/tcw/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <meta http-equiv="X-UA-Compatible" content="ie=edge">
         <title>Tiny Contest Winners - Create fun raffles and contests!</title>
         <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
         <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
         <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
+        <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-8540525880162386"
+     crossorigin="anonymous"></script>
     </head>
     <body>
         <nav class="navbar navbar-expand-lg py-3 bg-white border-bottom border-info" );">
             <div class="container-fluid bg-transparent">
                 <a class="navbar-brand fw-bold" href="/">Tiny Contest Winners!</a>
                 <span class="small">Create fun raffles and contests</span>
             </div>
```

### Comparing `tcw-0.1.3/tcw/utils.py` & `tcw-0.1.4/tcw/utils.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.3/tcw.egg-info/PKG-INFO` & `tcw-0.1.4/tcw.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.3
+Version: 0.1.4
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.3/tcw.egg-info/SOURCES.txt` & `tcw-0.1.4/tcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

