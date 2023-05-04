# Comparing `tmp/NJUlogin-3.0.4.tar.gz` & `tmp/NJUlogin-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJUlogin-3.0.4.tar", last modified: Sun Mar  5 02:53:16 2023, max compression
+gzip compressed data, was "NJUlogin-3.0.5.tar", last modified: Thu May  4 03:18:34 2023, max compression
```

## Comparing `NJUlogin-3.0.4.tar` & `NJUlogin-3.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 02:53:16.205364 NJUlogin-3.0.4/
--rw-rw-rw-   0        0        0     1082 2022-11-04 13:26:44.000000 NJUlogin-3.0.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-05 02:53:16.182985 NJUlogin-3.0.4/NJUlogin/
--rw-rw-rw-   0        0        0     5005 2023-02-11 03:29:25.000000 NJUlogin-3.0.4/NJUlogin/QRlogin.py
--rw-rw-rw-   0        0        0      221 2022-11-07 11:22:45.000000 NJUlogin-3.0.4/NJUlogin/__init__.py
--rw-rw-rw-   0        0        0      288 2023-03-05 02:52:08.000000 NJUlogin-3.0.4/NJUlogin/__version__.py
--rw-rw-rw-   0        0        0     1286 2023-02-06 05:06:02.000000 NJUlogin-3.0.4/NJUlogin/_base_.py
--rw-rw-rw-   0        0        0     3974 2023-03-05 02:50:02.000000 NJUlogin-3.0.4/NJUlogin/pwdLogin.py
-drwxrwxrwx   0        0        0        0 2023-03-05 02:53:16.199354 NJUlogin-3.0.4/NJUlogin/utils/
--rw-rw-rw-   0        0        0       15 2022-11-04 09:03:44.000000 NJUlogin-3.0.4/NJUlogin/utils/__init__.py
--rw-rw-rw-   0        0        0       81 2022-11-04 07:34:30.000000 NJUlogin-3.0.4/NJUlogin/utils/clear.py
--rw-rw-rw-   0        0        0      249 2022-11-07 02:43:03.000000 NJUlogin-3.0.4/NJUlogin/utils/config.py
--rw-rw-rw-   0        0        0      858 2023-03-05 02:48:50.000000 NJUlogin-3.0.4/NJUlogin/utils/get_post.py
--rw-rw-rw-   0        0        0      652 2023-03-03 16:25:08.000000 NJUlogin-3.0.4/NJUlogin/utils/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-05 02:53:16.190988 NJUlogin-3.0.4/NJUlogin.egg-info/
--rw-rw-rw-   0        0        0     2267 2023-03-05 02:53:16.000000 NJUlogin-3.0.4/NJUlogin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-03-05 02:53:16.000000 NJUlogin-3.0.4/NJUlogin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 02:53:16.000000 NJUlogin-3.0.4/NJUlogin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-03-05 02:53:16.000000 NJUlogin-3.0.4/NJUlogin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-05 02:53:16.000000 NJUlogin-3.0.4/NJUlogin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2267 2023-03-05 02:53:16.204364 NJUlogin-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-03-03 16:25:49.000000 NJUlogin-3.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-03-05 02:53:16.205364 NJUlogin-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0      853 2023-02-11 03:33:30.000000 NJUlogin-3.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-05 02:53:16.203364 NJUlogin-3.0.4/test/
--rw-rw-rw-   0        0        0     1006 2022-11-05 04:03:41.000000 NJUlogin-3.0.4/test/test.py
--rw-rw-rw-   0        0        0      773 2022-11-25 09:46:41.000000 NJUlogin-3.0.4/test/testlogin.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:18:34.037248 NJUlogin-3.0.5/
+-rw-rw-rw-   0        0        0     1082 2022-11-04 13:26:44.000000 NJUlogin-3.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-04 03:18:33.980024 NJUlogin-3.0.5/NJUlogin/
+-rw-rw-rw-   0        0        0     5005 2023-02-11 03:29:25.000000 NJUlogin-3.0.5/NJUlogin/QRlogin.py
+-rw-rw-rw-   0        0        0      221 2022-11-07 11:22:45.000000 NJUlogin-3.0.5/NJUlogin/__init__.py
+-rw-rw-rw-   0        0        0      288 2023-05-04 03:04:49.000000 NJUlogin-3.0.5/NJUlogin/__version__.py
+-rw-rw-rw-   0        0        0     1286 2023-02-06 05:06:02.000000 NJUlogin-3.0.5/NJUlogin/_base_.py
+-rw-rw-rw-   0        0        0     4074 2023-05-04 03:04:38.000000 NJUlogin-3.0.5/NJUlogin/pwdLogin.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:18:34.025039 NJUlogin-3.0.5/NJUlogin/utils/
+-rw-rw-rw-   0        0        0       15 2022-11-04 09:03:44.000000 NJUlogin-3.0.5/NJUlogin/utils/__init__.py
+-rw-rw-rw-   0        0        0       81 2022-11-04 07:34:30.000000 NJUlogin-3.0.5/NJUlogin/utils/clear.py
+-rw-rw-rw-   0        0        0      249 2022-11-07 02:43:03.000000 NJUlogin-3.0.5/NJUlogin/utils/config.py
+-rw-rw-rw-   0        0        0      858 2023-03-05 02:48:50.000000 NJUlogin-3.0.5/NJUlogin/utils/get_post.py
+-rw-rw-rw-   0        0        0      652 2023-03-03 16:25:08.000000 NJUlogin-3.0.5/NJUlogin/utils/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:18:34.010026 NJUlogin-3.0.5/NJUlogin.egg-info/
+-rw-rw-rw-   0        0        0     2267 2023-05-04 03:18:33.000000 NJUlogin-3.0.5/NJUlogin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-05-04 03:18:33.000000 NJUlogin-3.0.5/NJUlogin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 03:18:33.000000 NJUlogin-3.0.5/NJUlogin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-04 03:18:33.000000 NJUlogin-3.0.5/NJUlogin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 03:18:33.000000 NJUlogin-3.0.5/NJUlogin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2267 2023-05-04 03:18:34.035211 NJUlogin-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2023-03-03 16:25:49.000000 NJUlogin-3.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 03:18:34.038216 NJUlogin-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      853 2023-02-11 03:33:30.000000 NJUlogin-3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:18:34.031215 NJUlogin-3.0.5/test/
+-rw-rw-rw-   0        0        0     1006 2022-11-05 04:03:41.000000 NJUlogin-3.0.5/test/test.py
+-rw-rw-rw-   0        0        0      773 2022-11-25 09:46:41.000000 NJUlogin-3.0.5/test/testlogin.py
```

### Comparing `NJUlogin-3.0.4/LICENSE` & `NJUlogin-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/NJUlogin/QRlogin.py` & `NJUlogin-3.0.5/NJUlogin/QRlogin.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/NJUlogin/_base_.py` & `NJUlogin-3.0.5/NJUlogin/_base_.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/NJUlogin/pwdLogin.py` & `NJUlogin-3.0.5/NJUlogin/pwdLogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,19 @@
         data = (rds1 + self.password).encode('utf-8')
         key = pwdDefaultEncryptSalt.encode('utf-8')
         iv = rds2.encode('utf-8')
         pad_pkcs7 = pad(data, AES.block_size, style='pkcs7')
         aes = AES.new(key, AES.MODE_CBC, iv)
         return b64encode(aes.encrypt(pad_pkcs7)).decode('utf-8')
 
-    def login(self, dest: str, trytimes: int = 0) -> requests.Session:
-        url = urls.login % dest
+    def login(self, dest: str = None, trytimes: int = 0) -> requests.Session:
+        if dest is not None:
+            url = urls.login % dest
+        else:
+            url = urls.login.split("?")[0]
         html = self.get(url, timeout=self.getTimeout).text
         captcha = self.getCaptcha()
         selector = etree.HTML(html)
         password = self.pwdEncrypt(self.get_pwdDefaultEncryptSalt(selector))
 
         data = {
             'username': self.username,
```

### Comparing `NJUlogin-3.0.4/NJUlogin/utils/get_post.py` & `NJUlogin-3.0.5/NJUlogin/utils/get_post.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/NJUlogin/utils/urls.py` & `NJUlogin-3.0.5/NJUlogin/utils/urls.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/NJUlogin.egg-info/PKG-INFO` & `NJUlogin-3.0.5/NJUlogin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJUlogin
-Version: 3.0.4
+Version: 3.0.5
 Summary: The Nanjing University login module, which can be used to log on to various campus web sites
 Home-page: https://github.com/Do1e/NJUlogin
 Author: Do1e
 Author-email: dpj.email@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NJUlogin-3.0.4/PKG-INFO` & `NJUlogin-3.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJUlogin
-Version: 3.0.4
+Version: 3.0.5
 Summary: The Nanjing University login module, which can be used to log on to various campus web sites
 Home-page: https://github.com/Do1e/NJUlogin
 Author: Do1e
 Author-email: dpj.email@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NJUlogin-3.0.4/README.md` & `NJUlogin-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/setup.py` & `NJUlogin-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/test/test.py` & `NJUlogin-3.0.5/test/test.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.0.4/test/testlogin.py` & `NJUlogin-3.0.5/test/testlogin.py`

 * *Files identical despite different names*

