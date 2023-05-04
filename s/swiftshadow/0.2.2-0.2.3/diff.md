# Comparing `tmp/swiftshadow-0.2.2.tar.gz` & `tmp/swiftshadow-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.2.2.tar", last modified: Tue May  2 06:54:21 2023, max compression
+gzip compressed data, was "swiftshadow-0.2.3.tar", last modified: Thu May  4 07:58:38 2023, max compression
```

## Comparing `swiftshadow-0.2.2.tar` & `swiftshadow-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.390941 swiftshadow-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 06:54:21.390941 swiftshadow-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-02 06:54:04.000000 swiftshadow-0.2.2/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:54:21.386941 swiftshadow-0.2.2/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 06:54:21.000000 swiftshadow-0.2.2/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.225992 swiftshadow-0.2.3/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.2.2/LICENSE` & `swiftshadow-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.2/PKG-INFO` & `swiftshadow-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.2
+Version: 0.2.3
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swiftshadow-0.2.2/README.md` & `swiftshadow-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.2/setup.py` & `swiftshadow-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.2.2"),
+    version=VERSION.get("__version__", "0.2.3"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.2.2/swiftshadow/constants.py` & `swiftshadow-0.2.3/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.2/swiftshadow/providers.py` & `swiftshadow-0.2.3/swiftshadow/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             clean(row[1]) + ":" + clean(row[2]),
             protocol,
             getCountryCode(clean(row[4].split(" ", 1)[1])),
         ]
         if checkProxy(cleaned, countries):
             result.append({cleaned[1]: cleaned[0]})
             count += 1
+    return result
 
 
 def Proxyscrape(max, countries=[], protocol="http"):
     result = []
     count = 0
     query = "https://api.proxyscrape.com/v2/?timeout=5000&request=displayproxies&protocol=http"
     log("info", "Updating proxies from Proxyscrape")
@@ -43,7 +44,11 @@
     for ip in ips.split("\n"):
         if count == max:
             return result
         proxy = [ip.strip(), protocol, "all"]
         if checkProxy(proxy, []):
             result.append({proxy[1]: proxy[0]})
             count += 1
+    return result
+
+
+Providers = [Proxyscrape, Scrapingant]
```

### Comparing `swiftshadow-0.2.2/swiftshadow/swiftshadow.py` & `swiftshadow-0.2.3/swiftshadow/swiftshadow.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.2/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.2.3/swiftshadow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.2
+Version: 0.2.3
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

