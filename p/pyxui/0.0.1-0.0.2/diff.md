# Comparing `tmp/pyxui-0.0.1.tar.gz` & `tmp/pyxui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxui-0.0.1.tar", last modified: Wed May  3 15:18:38 2023, max compression
+gzip compressed data, was "pyxui-0.0.2.tar", last modified: Thu May  4 20:29:29 2023, max compression
```

## Comparing `pyxui-0.0.1.tar` & `pyxui-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:18:38.744482 pyxui-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-25 11:55:37.000000 pyxui-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5067 2023-05-03 15:18:38.744482 pyxui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-04-27 13:48:38.000000 pyxui-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 15:18:38.733510 pyxui-0.0.1/pyxui/
--rw-rw-rw-   0        0        0       98 2023-04-27 08:47:15.000000 pyxui-0.0.1/pyxui/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-27 08:00:10.000000 pyxui-0.0.1/pyxui/xui.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:18:38.742511 pyxui-0.0.1/pyxui.egg-info/
--rw-rw-rw-   0        0        0     5067 2023-05-03 15:18:38.000000 pyxui-0.0.1/pyxui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-03 15:18:38.000000 pyxui-0.0.1/pyxui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:18:38.000000 pyxui-0.0.1/pyxui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 15:18:38.000000 pyxui-0.0.1/pyxui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 15:18:38.744482 pyxui-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-05-03 15:09:06.000000 pyxui-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.298730 pyxui-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-03 15:10:37.000000 pyxui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5047 2023-05-04 20:29:29.296734 pyxui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4632 2023-05-03 15:10:37.000000 pyxui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.277782 pyxui-0.0.2/pyxui/
+-rw-rw-rw-   0        0        0       26 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.287758 pyxui-0.0.2/pyxui/config_gen/
+-rw-rw-rw-   0        0        0      452 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/config_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.288756 pyxui-0.0.2/pyxui/errors/
+-rw-rw-rw-   0        0        0      917 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.295737 pyxui-0.0.2/pyxui/methods/
+-rw-rw-rw-   0        0        0      247 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/base.py
+-rw-rw-rw-   0        0        0     4913 2023-05-04 08:36:49.000000 pyxui-0.0.2/pyxui/methods/clients.py
+-rw-rw-rw-   0        0        0     1415 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/inbounds.py
+-rw-rw-rw-   0        0        0     1123 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/methods/login.py
+-rw-rw-rw-   0        0        0      482 2023-05-03 15:10:37.000000 pyxui-0.0.2/pyxui/xui.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:29.286764 pyxui-0.0.2/pyxui.egg-info/
+-rw-rw-rw-   0        0        0     5047 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 20:29:29.000000 pyxui-0.0.2/pyxui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:29:29.298730 pyxui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-04 20:28:51.000000 pyxui-0.0.2/setup.py
```

### Comparing `pyxui-0.0.1/LICENSE` & `pyxui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxui-0.0.1/PKG-INFO` & `pyxui-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.1
+Version: 0.0.2
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyXUI 
 An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
 
 ## How To Install
```

### Comparing `pyxui-0.0.1/README.md` & `pyxui-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -161,8 +161,8 @@
     "fp": "chrome"
 }
 
 generate_config = config_generator("vless", config, data)
 
 # Result
 vless://a85def57-0a86-43d1-b15c-0494519067c6@staliox.com:443?security=tls&type=ws&host=staliox.site&path=%2F&tls=tls&sni=staliox.site&alpn=h2%2Chttp%2F1.1&fp=chrome#Staliox-Me
-```
+```
```

### Comparing `pyxui-0.0.1/pyxui.egg-info/PKG-INFO` & `pyxui-0.0.2/pyxui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyxui
-Version: 0.0.1
+Version: 0.0.2
 Summary: An application with python that allows you to modify your xui panel
 Home-page: https://github.com/staliox/pyxui
 Author: Staliox
 License: MIT
 Keywords: pyxui,xui,xui python,xui panel
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyXUI 
 An application with python that allows you to modify your xui panel ([Sanaeii 3x-ui](https://github.com/MHSanaei/3x-ui)) ([alireza0 x-ui](https://github.com/alireza0/x-ui))
 
 ## How To Install
```

