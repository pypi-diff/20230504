# Comparing `tmp/Omar_Style_sel-0.2.tar.gz` & `tmp/Omar_Style_sel-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Omar_Style_sel-0.2.tar", last modified: Tue Apr 25 18:56:22 2023, max compression
+gzip compressed data, was "Omar_Style_sel-0.3.tar", last modified: Thu May  4 21:39:28 2023, max compression
```

## Comparing `Omar_Style_sel-0.2.tar` & `Omar_Style_sel-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:56:22.848091 Omar_Style_sel-0.2/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-25 18:56:22.821089 Omar_Style_sel-0.2/Omar_Style_sel/
--rw-rw-rw-   0        0        0     2201 2023-04-25 18:15:08.000000 Omar_Style_sel-0.2/Omar_Style_sel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:56:22.843092 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/
--rw-rw-rw-   0        0        0     1833 2023-04-25 18:56:22.000000 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-25 18:56:22.000000 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:56:22.000000 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 18:56:22.000000 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 18:56:22.000000 Omar_Style_sel-0.2/Omar_Style_sel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1833 2023-04-25 18:56:22.845090 Omar_Style_sel-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-04-25 18:53:37.000000 Omar_Style_sel-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 18:56:22.849092 Omar_Style_sel-0.2/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-25 18:56:09.000000 Omar_Style_sel-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:39:28.045427 Omar_Style_sel-0.3/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-04 21:39:27.864258 Omar_Style_sel-0.3/Omar_Style_sel/
+-rw-rw-rw-   0        0        0     2756 2023-05-04 21:36:01.000000 Omar_Style_sel-0.3/Omar_Style_sel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:39:28.038272 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/
+-rw-rw-rw-   0        0        0     1833 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 21:39:27.000000 Omar_Style_sel-0.3/Omar_Style_sel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1833 2023-05-04 21:39:28.041269 Omar_Style_sel-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2023-04-25 18:53:37.000000 Omar_Style_sel-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 21:39:28.048269 Omar_Style_sel-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-05-04 21:37:22.000000 Omar_Style_sel-0.3/setup.py
```

### Comparing `Omar_Style_sel-0.2/Omar_Style_sel/__init__.py` & `Omar_Style_sel-0.3/Omar_Style_sel/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Copyright: You are prohibited from publishing this project in another project
 Code developer Omar_Style_ps
 
 Contact for inquiries:
     https://t.me/OmarStyle1
 """
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
 from selenium import webdriver
 #Omar_Style 
 class BrowsersProxy:
     #Omar_Style 
     def proxy_firefox(self, pr, firr):
         try:
@@ -26,15 +28,28 @@
         firefox_profile.set_preference("network.proxy.ssl_port", int(proxy_port))
 
         driver = webdriver.Firefox(firefox_profile=firefox_profile)
         driver.get(firr)
         return driver
 
     def proxy_chrome(self,proxy_address,Link,driver_path=None):
+        options = Options()
+        options.add_argument("window-size=1400,600")
+        from fake_useragent import UserAgent
+        ua = UserAgent()
+        user_agent = ua.random
+        # print(user_agent)
+        options.add_argument(f'user-agent={user_agent}')
+        
+        # driver = webdriver.Chrome(chrome_options=options)
+        # driver.get('https://whoer.net/')
+        # driver.quit()
+
         """
+
         Copyright: You are prohibited from publishing this project in another project
             Code developer Omar_Style_ps
 
         Contact for inquiries:
             https://t.me/OmarStyle1
         """
         try:
@@ -42,22 +57,22 @@
         except ValueError:
             raise ValueError("Please enter the proxy correctly. Example: 95.56.254.139:3128")
 
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument(f'--proxy-server={proxy_host}:{proxy_port}')
 
         if driver_path is None:
-            driver = webdriver.Chrome(options=chrome_options)
+            driver = webdriver.Chrome(options=chrome_options,chrome_options=options)
         else:
-            driver = webdriver.Chrome(driver_path, options=chrome_options)
+            driver = webdriver.Chrome(driver_path, options=chrome_options,chrome_options=options)
         driver.get(Link)
         return driver
 
 
 
 
 
 
-pr = BrowsersProxy()
-pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
+# pr = BrowsersProxy()
+# pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
 # driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com", driver_path='E:\\chroo\\chromedriver.exe')
```

### Comparing `Omar_Style_sel-0.2/Omar_Style_sel.egg-info/PKG-INFO` & `Omar_Style_sel-0.3/Omar_Style_sel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Omar-Style-sel
-Version: 0.2
+Version: 0.3
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Omar_Style_sel-0.2/PKG-INFO` & `Omar_Style_sel-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Omar_Style_sel
-Version: 0.2
+Version: 0.3
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Omar_Style_sel-0.2/README.md` & `Omar_Style_sel-0.3/README.md`

 * *Files identical despite different names*

### Comparing `Omar_Style_sel-0.2/setup.py` & `Omar_Style_sel-0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='Omar_Style_sel',
-    version="0.2",
+    version="0.3",
     author='omar Style',
     author_email='omarllStyle@gmail.com',
     description='Omar_Style _ 〄🇵🇸',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['Omar_Style_sel'],
-    install_requires=["selenium"],
+    install_requires=["selenium","fake_useragent"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License'],
```

