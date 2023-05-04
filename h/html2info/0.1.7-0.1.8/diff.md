# Comparing `tmp/html2info-0.1.7.tar.gz` & `tmp/html2info-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.7.tar", last modified: Tue Apr 25 23:46:31 2023, max compression
+gzip compressed data, was "html2info-0.1.8.tar", last modified: Thu May  4 19:16:16 2023, max compression
```

## Comparing `html2info-0.1.7.tar` & `html2info-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-25 23:46:31.169025 html2info-0.1.7/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-25 23:46:31.169025 html2info-0.1.7/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.7/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-25 23:46:31.169025 html2info-0.1.7/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.7/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5117 2023-04-25 23:43:58.000000 html2info-0.1.7/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.7/html2info/types.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.7/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-04-25 23:46:31.169025 html2info-0.1.7/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-04-25 23:46:31.000000 html2info-0.1.7/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-04-25 23:46:31.000000 html2info-0.1.7/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-04-25 23:46:31.000000 html2info-0.1.7/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-04-25 23:46:31.000000 html2info-0.1.7/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-04-25 23:46:31.000000 html2info-0.1.7/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.7/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-04-25 23:46:31.169025 html2info-0.1.7/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-04-25 23:44:57.000000 html2info-0.1.7/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-04 19:16:16.553869 html2info-0.1.8/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.8/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.8/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5191 2023-05-04 19:14:11.000000 html2info-0.1.8/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.8/html2info/types.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.8/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.8/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-04 19:16:16.553869 html2info-0.1.8/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-05-04 19:15:27.000000 html2info-0.1.8/setup.py
```

### Comparing `html2info-0.1.7/PKG-INFO` & `html2info-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.7/README.md` & `html2info-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `html2info-0.1.7/html2info/linkedin.py` & `html2info-0.1.8/html2info/linkedin.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 
         experience_items = experience_section.find_all("li", class_="artdeco-list__item")
 
         for item in experience_items:
             title = item.find("span", class_="t-bold")
             company = item.find("span", class_="t-14 t-normal")
             image_link = item.find("img")["src"] if item.find("img") else None
-            company_link = item.find("a", class_="optional-action-target-wrapper")["href"]
+
+            company_link = item.find("a", class_="optional-action-target-wrapper")
+            if company_link:
+                company_link = company_link["href"]
 
             dates = item.find("span", {"class": "t-14 t-normal t-black--light"})
 
             description = item.find("div", class_="inline-show-more-text")
 
             self.experience += [
                 {
```

### Comparing `html2info-0.1.7/html2info.egg-info/PKG-INFO` & `html2info-0.1.8/html2info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.7/pyproject.toml` & `html2info-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.7/setup.py` & `html2info-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.7",  # Replace with your package version
+    version="0.1.8",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

