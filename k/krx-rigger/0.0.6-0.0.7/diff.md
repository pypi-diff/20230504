# Comparing `tmp/krx_rigger-0.0.6.tar.gz` & `tmp/krx_rigger-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_rigger-0.0.6.tar", last modified: Wed May  3 16:10:02 2023, max compression
+gzip compressed data, was "dist/krx_rigger-0.0.7.tar", last modified: Thu May  4 05:28:49 2023, max compression
```

## Comparing `krx_rigger-0.0.6.tar` & `krx_rigger-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx_rigger.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx_rigger.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx_rigger.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx_rigger.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx_rigger.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.6/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/test/
--rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.6/test/test_list.py
--rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.6/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 16:10:01.000000 krx_rigger-0.0.6/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/setup.cfg
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 16:10:02.000000 krx_rigger-0.0.6/krx/
--rw-r--r--   0 nezah      (501) staff       (20)     7250 2023-05-03 16:10:01.000000 krx_rigger-0.0.6/krx/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx_rigger.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx_rigger.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx_rigger.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx_rigger.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx_rigger.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.7/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/test/
+-rw-r--r--   0 nezah      (501) staff       (20)      436 2023-05-03 14:12:55.000000 krx_rigger-0.0.7/test/test_list.py
+-rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.7/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-04 05:28:47.000000 krx_rigger-0.0.7/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-04 05:28:49.000000 krx_rigger-0.0.7/krx/
+-rw-r--r--   0 nezah      (501) staff       (20)     7447 2023-05-04 05:28:47.000000 krx_rigger-0.0.7/krx/__init__.py
```

### Comparing `krx_rigger-0.0.6/LICENSE` & `krx_rigger-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_rigger-0.0.6/setup.py` & `krx_rigger-0.0.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krx_rigger",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="krx web crawler wrapper",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/krx_rigger",
     packages=setuptools.find_packages(),
```

### Comparing `krx_rigger-0.0.6/krx/__init__.py` & `krx_rigger-0.0.7/krx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         logger.info(response.status_code)
 
     def fetch_list(self, dt, time_sleep=0.3):
 
         results = []
         page = 1
         total_page = 1
-        page_no = 0
 
         while page <= total_page:
             items = self._fetch_list(dt, page=page)
 
             if items is not None:
                 total_count = items.get('total_count')
                 total_page = items.get('total_page')
@@ -141,14 +140,18 @@
             'kosdaqSegment': '',
             'selDate': dt,
             'searchCorpName': '',
             'copyUrl': '',
         }
 
         response = self.session.post('https://kind.krx.co.kr/disclosure/todaydisclosure.do', headers=headers, data=data)
+        status = response.status_code
+        if status != 200:
+            logger.error(f"status : {status}, response : {response.text}")
+            raise Exception(f"status : {status}, response : {response.text}")
         soup = BeautifulSoup(response.text, "html.parser")
         return self._parse_list(soup, dt)
 
     def _parse_list(self, soup, dt):
         info_div = soup.select("div.info")
         if len(info_div) < 1:
             return None
```

