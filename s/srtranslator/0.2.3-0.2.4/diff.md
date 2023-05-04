# Comparing `tmp/srtranslator-0.2.3.tar.gz` & `tmp/srtranslator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtranslator-0.2.3.tar", last modified: Sun Apr 23 15:52:49 2023, max compression
+gzip compressed data, was "srtranslator-0.2.4.tar", last modified: Thu May  4 18:30:58 2023, max compression
```

## Comparing `srtranslator-0.2.3.tar` & `srtranslator-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:52:49.968751 srtranslator-0.2.3/
--rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.3/LICENSE.md
--rw-rw-rw-   0        0        0     2891 2023-04-23 15:52:49.967750 srtranslator-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2023-04-23 15:51:51.000000 srtranslator-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 15:52:49.968751 srtranslator-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-04-23 15:52:06.000000 srtranslator-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:52:49.960744 srtranslator-0.2.3/srtranslator/
--rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.3/srtranslator/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-03-31 14:56:01.000000 srtranslator-0.2.3/srtranslator/__main__.py
--rw-rw-rw-   0        0        0     5952 2023-03-02 13:44:07.000000 srtranslator-0.2.3/srtranslator/srt_file.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:52:49.967750 srtranslator-0.2.3/srtranslator/translators/
--rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.3/srtranslator/translators/__init__.py
--rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.3/srtranslator/translators/base.py
--rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.3/srtranslator/translators/deepl_api.py
--rw-rw-rw-   0        0        0     4572 2023-04-03 17:46:29.000000 srtranslator-0.2.3/srtranslator/translators/deepl_scrap.py
--rw-rw-rw-   0        0        0     4055 2023-02-18 16:26:23.000000 srtranslator-0.2.3/srtranslator/translators/selenium_utils.py
--rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.3/srtranslator/translators/translatepy.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:52:49.963746 srtranslator-0.2.3/srtranslator.egg-info/
--rw-rw-rw-   0        0        0     2891 2023-04-23 15:52:49.000000 srtranslator-0.2.3/srtranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-04-23 15:52:49.000000 srtranslator-0.2.3/srtranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:52:49.000000 srtranslator-0.2.3/srtranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      657 2023-04-23 15:52:49.000000 srtranslator-0.2.3/srtranslator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 15:52:49.000000 srtranslator-0.2.3/srtranslator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:58.078281 srtranslator-0.2.4/
+-rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.4/LICENSE.md
+-rw-rw-rw-   0        0        0     2891 2023-05-04 18:30:58.077280 srtranslator-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2486 2023-04-23 15:51:51.000000 srtranslator-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:30:58.078281 srtranslator-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-05-04 18:27:22.000000 srtranslator-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:58.071495 srtranslator-0.2.4/srtranslator/
+-rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.4/srtranslator/__init__.py
+-rw-rw-rw-   0        0        0     2382 2023-05-04 18:24:01.000000 srtranslator-0.2.4/srtranslator/__main__.py
+-rw-rw-rw-   0        0        0     5952 2023-03-02 13:44:07.000000 srtranslator-0.2.4/srtranslator/srt_file.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:58.077280 srtranslator-0.2.4/srtranslator/translators/
+-rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.4/srtranslator/translators/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.4/srtranslator/translators/base.py
+-rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.4/srtranslator/translators/deepl_api.py
+-rw-rw-rw-   0        0        0     4572 2023-04-03 17:46:29.000000 srtranslator-0.2.4/srtranslator/translators/deepl_scrap.py
+-rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.4/srtranslator/translators/selenium_utils.py
+-rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.4/srtranslator/translators/translatepy.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:30:58.073497 srtranslator-0.2.4/srtranslator.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-05-04 18:30:57.000000 srtranslator-0.2.4/srtranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-04 18:30:58.000000 srtranslator-0.2.4/srtranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 18:30:57.000000 srtranslator-0.2.4/srtranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      657 2023-05-04 18:30:57.000000 srtranslator-0.2.4/srtranslator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 18:30:57.000000 srtranslator-0.2.4/srtranslator.egg-info/top_level.txt
```

### Comparing `srtranslator-0.2.3/PKG-INFO` & `srtranslator-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
```

### Comparing `srtranslator-0.2.3/README.md` & `srtranslator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.3/setup.py` & `srtranslator-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name="srtranslator",
     description="Traslate a .SRT file using any custom translator",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/sinedie/SRTranslator",
-    version="0.2.3",
+    version="0.2.4",
     author="EAR",
     author_email="sinedie@protonmail.com",
     license="FREE",
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages(),
     keywords=["python", "srt", "languages", "translator", "subtitles"],
```

### Comparing `srtranslator-0.2.3/srtranslator/__main__.py` & `srtranslator-0.2.4/srtranslator/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,14 @@
 
 parser.add_argument(
     "--auth",
     type=str,
     help="Api key if needed on translator",
 )
 
-# TODO add custom proxy arg
-
 builtin_translators = {
     "deepl-scrap": DeeplTranslator,
     "deepl-api": DeeplApi,
     "translatepy": TranslatePy,
 }
 
 args = parser.parse_args()
```

### Comparing `srtranslator-0.2.3/srtranslator/srt_file.py` & `srtranslator-0.2.4/srtranslator/srt_file.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.3/srtranslator/translators/deepl_scrap.py` & `srtranslator-0.2.4/srtranslator/translators/deepl_scrap.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.3/srtranslator/translators/selenium_utils.py` & `srtranslator-0.2.4/srtranslator/translators/selenium_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import sys
 import logging
 
-from typing import Optional
+from typing import Optional, List
 from fp.fp import FreeProxy
 from selenium import webdriver
 from webdriverdownloader import GeckoDriverDownloader
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.proxy import Proxy, ProxyType
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver import ActionChains, Keys
 from selenium.webdriver.support import expected_conditions as EC
 
 
-def create_proxy() -> Proxy:
+def create_proxy(country_id: Optional[List[str]] = ["US"]) -> Proxy:
     """Creates a new proxy to use with a selenium driver and avoid get banned
 
+    Args:
+        country_id (Optional[List[str]], optional): Contry id to create proxy. Defaults to ['US'].
+
     Returns:
         Proxy: Selenium WebDriver proxy
     """
     logging.info("Getting a new Proxy from https://www.sslproxies.org/")
-    proxy = FreeProxy().get()
+    proxy = FreeProxy(country_id=country_id).get()
     proxy = Proxy(
         dict(
             proxyType=ProxyType.MANUAL,
             httpProxy=proxy,
             ftpProxy=proxy,
             sslProxy=proxy,
             noProxy="",
```

### Comparing `srtranslator-0.2.3/srtranslator/translators/translatepy.py` & `srtranslator-0.2.4/srtranslator/translators/translatepy.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.3/srtranslator.egg-info/PKG-INFO` & `srtranslator-0.2.4/srtranslator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
```

### Comparing `srtranslator-0.2.3/srtranslator.egg-info/SOURCES.txt` & `srtranslator-0.2.4/srtranslator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.3/srtranslator.egg-info/requires.txt` & `srtranslator-0.2.4/srtranslator.egg-info/requires.txt`

 * *Files identical despite different names*

