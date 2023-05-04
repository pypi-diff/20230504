# Comparing `tmp/brunns-matchers-2.6.0.tar.gz` & `tmp/brunns-matchers-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunns-matchers-2.6.0.tar", last modified: Wed Oct 19 09:01:15 2022, max compression
+gzip compressed data, was "brunns-matchers-2.7.0.tar", last modified: Thu May  4 12:46:42 2023, max compression
```

## Comparing `brunns-matchers-2.6.0.tar` & `brunns-matchers-2.7.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 brunns     (501) staff       (20)        0 2022-10-19 09:01:15.337688 brunns-matchers-2.6.0/
--rw-r--r--   0 brunns     (501) staff       (20)     1071 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/LICENSE
--rw-r--r--   0 brunns     (501) staff       (20)     4496 2022-10-19 09:01:15.337761 brunns-matchers-2.6.0/PKG-INFO
--rw-r--r--   0 brunns     (501) staff       (20)     3535 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/README.md
--rw-r--r--   0 brunns     (501) staff       (20)      265 2022-10-19 09:01:15.338098 brunns-matchers-2.6.0/setup.cfg
--rw-r--r--   0 brunns     (501) staff       (20)     1937 2022-10-19 08:44:49.000000 brunns-matchers-2.6.0/setup.py
-drwxr-xr-x   0 brunns     (501) staff       (20)        0 2022-10-19 09:01:15.333132 brunns-matchers-2.6.0/src/
-drwxr-xr-x   0 brunns     (501) staff       (20)        0 2022-10-19 09:01:15.334094 brunns-matchers-2.6.0/src/brunns/
--rw-r--r--   0 brunns     (501) staff       (20)       81 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/__init__.py
-drwxr-xr-x   0 brunns     (501) staff       (20)        0 2022-10-19 09:01:15.336464 brunns-matchers-2.6.0/src/brunns/matchers/
--rw-r--r--   0 brunns     (501) staff       (20)        0 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/__init__.py
--rw-r--r--   0 brunns     (501) staff       (20)      950 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/bytestring.py
--rw-r--r--   0 brunns     (501) staff       (20)     1728 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/data.py
--rw-r--r--   0 brunns     (501) staff       (20)     1342 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/datetime.py
--rw-r--r--   0 brunns     (501) staff       (20)     3213 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/dbapi.py
--rw-r--r--   0 brunns     (501) staff       (20)     8678 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/html.py
--rw-r--r--   0 brunns     (501) staff       (20)     4508 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/matcher.py
--rw-r--r--   0 brunns     (501) staff       (20)     5225 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/mock.py
--rw-r--r--   0 brunns     (501) staff       (20)     4961 2022-10-07 07:51:50.000000 brunns-matchers-2.6.0/src/brunns/matchers/object.py
--rw-r--r--   0 brunns     (501) staff       (20)    11221 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/response.py
--rw-r--r--   0 brunns     (501) staff       (20)     7286 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/smtp.py
--rw-r--r--   0 brunns     (501) staff       (20)     8515 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/url.py
--rw-r--r--   0 brunns     (501) staff       (20)     1257 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/matchers/utils.py
--rw-r--r--   0 brunns     (501) staff       (20)        0 2022-06-27 13:56:17.000000 brunns-matchers-2.6.0/src/brunns/py.typed
-drwxr-xr-x   0 brunns     (501) staff       (20)        0 2022-10-19 09:01:15.337569 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/
--rw-r--r--   0 brunns     (501) staff       (20)     4496 2022-10-19 09:01:15.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/PKG-INFO
--rw-r--r--   0 brunns     (501) staff       (20)      723 2022-10-19 09:01:15.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/SOURCES.txt
--rw-r--r--   0 brunns     (501) staff       (20)        1 2022-10-19 09:01:15.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/dependency_links.txt
--rw-r--r--   0 brunns     (501) staff       (20)        1 2022-06-27 13:56:30.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/not-zip-safe
--rw-r--r--   0 brunns     (501) staff       (20)      142 2022-10-19 09:01:15.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/requires.txt
--rw-r--r--   0 brunns     (501) staff       (20)        7 2022-10-19 09:01:15.000000 brunns-matchers-2.6.0/src/brunns_matchers.egg-info/top_level.txt
+drwxr-xr-x   0 brunns     (501) staff       (20)        0 2023-05-04 12:46:42.602474 brunns-matchers-2.7.0/
+-rw-r--r--   0 brunns     (501) staff       (20)     1071 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/LICENSE
+-rw-r--r--   0 brunns     (501) staff       (20)     4644 2023-05-04 12:46:42.602546 brunns-matchers-2.7.0/PKG-INFO
+-rw-r--r--   0 brunns     (501) staff       (20)     3684 2022-10-19 09:05:32.000000 brunns-matchers-2.7.0/README.md
+-rw-r--r--   0 brunns     (501) staff       (20)       28 2023-03-01 13:31:04.000000 brunns-matchers-2.7.0/pyproject.toml
+-rw-r--r--   0 brunns     (501) staff       (20)      317 2023-05-04 12:46:42.602807 brunns-matchers-2.7.0/setup.cfg
+-rw-r--r--   0 brunns     (501) staff       (20)     1983 2023-05-04 12:44:19.000000 brunns-matchers-2.7.0/setup.py
+drwxr-xr-x   0 brunns     (501) staff       (20)        0 2023-05-04 12:46:42.597119 brunns-matchers-2.7.0/src/
+drwxr-xr-x   0 brunns     (501) staff       (20)        0 2023-05-04 12:46:42.598482 brunns-matchers-2.7.0/src/brunns/
+-rw-r--r--   0 brunns     (501) staff       (20)       81 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/__init__.py
+drwxr-xr-x   0 brunns     (501) staff       (20)        0 2023-05-04 12:46:42.601195 brunns-matchers-2.7.0/src/brunns/matchers/
+-rw-r--r--   0 brunns     (501) staff       (20)        0 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/__init__.py
+-rw-r--r--   0 brunns     (501) staff       (20)      950 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/bytestring.py
+-rw-r--r--   0 brunns     (501) staff       (20)     1728 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/data.py
+-rw-r--r--   0 brunns     (501) staff       (20)     1342 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/datetime.py
+-rw-r--r--   0 brunns     (501) staff       (20)     3213 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/dbapi.py
+-rw-r--r--   0 brunns     (501) staff       (20)     8678 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/html.py
+-rw-r--r--   0 brunns     (501) staff       (20)     4508 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/matcher.py
+-rw-r--r--   0 brunns     (501) staff       (20)     5225 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/mock.py
+-rw-r--r--   0 brunns     (501) staff       (20)     4961 2023-02-23 16:54:52.000000 brunns-matchers-2.7.0/src/brunns/matchers/object.py
+-rw-r--r--   0 brunns     (501) staff       (20)    11221 2023-05-04 12:42:32.000000 brunns-matchers-2.7.0/src/brunns/matchers/response.py
+-rw-r--r--   0 brunns     (501) staff       (20)     7286 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/smtp.py
+-rw-r--r--   0 brunns     (501) staff       (20)     8515 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/url.py
+-rw-r--r--   0 brunns     (501) staff       (20)     1257 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/matchers/utils.py
+-rw-r--r--   0 brunns     (501) staff       (20)     4978 2023-05-04 12:42:32.000000 brunns-matchers-2.7.0/src/brunns/matchers/werkzeug.py
+-rw-r--r--   0 brunns     (501) staff       (20)        0 2022-06-27 13:56:17.000000 brunns-matchers-2.7.0/src/brunns/py.typed
+drwxr-xr-x   0 brunns     (501) staff       (20)        0 2023-05-04 12:46:42.602336 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/
+-rw-r--r--   0 brunns     (501) staff       (20)     4644 2023-05-04 12:46:42.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/PKG-INFO
+-rw-r--r--   0 brunns     (501) staff       (20)      770 2023-05-04 12:46:42.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/SOURCES.txt
+-rw-r--r--   0 brunns     (501) staff       (20)        1 2023-05-04 12:46:42.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/dependency_links.txt
+-rw-r--r--   0 brunns     (501) staff       (20)        1 2022-06-27 13:56:30.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/not-zip-safe
+-rw-r--r--   0 brunns     (501) staff       (20)      167 2023-05-04 12:46:42.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/requires.txt
+-rw-r--r--   0 brunns     (501) staff       (20)        7 2023-05-04 12:46:42.000000 brunns-matchers-2.7.0/src/brunns_matchers.egg-info/top_level.txt
```

### Comparing `brunns-matchers-2.6.0/LICENSE` & `brunns-matchers-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/PKG-INFO` & `brunns-matchers-2.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunns-matchers
-Version: 2.6.0
+Version: 2.7.0
 Summary: Custom PyHamcrest matchers
 Home-page: https://github.com/brunns/brunns-matchers/
 Author: Simon Brunning
 Author-email: simon@brunningonline.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7 
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # brunns-matchers
 
 Various custom [PyHamcrest](https://pyhamcrest.readthedocs.io) matchers.
 
@@ -59,15 +59,16 @@
     make help
 
 ## Releasing
 
 Requires [hub](https://hub.github.com/), [setuptools](https://setuptools.readthedocs.io), [wheel](https://pypi.org/project/wheel/) and [twine](https://twine.readthedocs.io). To release `n.n.n`:
 
 ```sh
-version="n.n.n"
-make precommit && git commit -am"Release $version" && git push # If not already all pushed, which it should be.
-hub release create $version -m"Release $version"
+version="n.n.n" # Needs to match new version number in setup.py.
+git checkout -b "release-$version"
+make precommit && git commit -am"Release $version" && git push --set-upstream origin "release-$version" # If not already all pushed, which it should be.
+hub release create "V$version" -t"release-$version" -m"Version $version"
 python setup.py sdist bdist_wheel
 twine upload dist/*$version*
 git checkout master
 git merge "release-$version"
 ```
```

### Comparing `brunns-matchers-2.6.0/README.md` & `brunns-matchers-2.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     make help
 
 ## Releasing
 
 Requires [hub](https://hub.github.com/), [setuptools](https://setuptools.readthedocs.io), [wheel](https://pypi.org/project/wheel/) and [twine](https://twine.readthedocs.io). To release `n.n.n`:
 
 ```sh
-version="n.n.n"
-make precommit && git commit -am"Release $version" && git push # If not already all pushed, which it should be.
-hub release create $version -m"Release $version"
+version="n.n.n" # Needs to match new version number in setup.py.
+git checkout -b "release-$version"
+make precommit && git commit -am"Release $version" && git push --set-upstream origin "release-$version" # If not already all pushed, which it should be.
+hub release create "V$version" -t"release-$version" -m"Version $version"
 python setup.py sdist bdist_wheel
 twine upload dist/*$version*
 git checkout master
 git merge "release-$version"
 ```
```

### Comparing `brunns-matchers-2.6.0/setup.py` & `brunns-matchers-2.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 except IOError:
     logger.warning("README file not found or unreadable.")
     long_description = "See https://github.com/brunns/brunns-matchers/"
 
 setup(
     name="brunns-matchers",
     zip_safe=False,
-    version="2.6.0",
+    version="2.7.0",
     description="Custom PyHamcrest matchers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Simon Brunning",
     author_email="simon@brunningonline.net",
     url="https://github.com/brunns/brunns-matchers/",
     packages=find_packages(where="src"),
@@ -43,18 +43,20 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Testing",
     ],
-    python_requires=">=3.7 ",
+    python_requires=">=3.7",
     install_requires=[
         "beautifulsoup4>=4.0",
         "brunns-row>=2.0",
         "Deprecated>=1.2",
         "furl>=2.0",
+        "imurl>=0.2",
         "pyhamcrest>=2.0",
         "requests>=2.0",
         "typing-extensions>=3.7 ; python_version<'3.8'",
+        "Werkzeug>=2.0",
     ],
 )
```

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/bytestring.py` & `brunns-matchers-2.7.0/src/brunns/matchers/bytestring.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/data.py` & `brunns-matchers-2.7.0/src/brunns/matchers/data.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/datetime.py` & `brunns-matchers-2.7.0/src/brunns/matchers/datetime.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/dbapi.py` & `brunns-matchers-2.7.0/src/brunns/matchers/dbapi.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/html.py` & `brunns-matchers-2.7.0/src/brunns/matchers/html.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/matcher.py` & `brunns-matchers-2.7.0/src/brunns/matchers/matcher.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/mock.py` & `brunns-matchers-2.7.0/src/brunns/matchers/mock.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/object.py` & `brunns-matchers-2.7.0/src/brunns/matchers/object.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/response.py` & `brunns-matchers-2.7.0/src/brunns/matchers/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         try:
             return response.json()
         except ValueError:
             return None
 
     def describe_to(self, description: Description) -> None:
         description.append_text("response with")
-        append_matcher_description(self.status_code, "status_code", description)
+        append_matcher_description(self.status_code, "status code", description)
         append_matcher_description(self.body, "body", description)
         append_matcher_description(self.content, "content", description)
         append_matcher_description(self.json, "json", description)
         append_matcher_description(self.headers, "headers", description)
         append_matcher_description(self.cookies, "cookies", description)
         append_matcher_description(self.elapsed, "elapsed", description)
         append_matcher_description(self.history, "history", description)
```

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/smtp.py` & `brunns-matchers-2.7.0/src/brunns/matchers/smtp.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/url.py` & `brunns-matchers-2.7.0/src/brunns/matchers/url.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns/matchers/utils.py` & `brunns-matchers-2.7.0/src/brunns/matchers/utils.py`

 * *Files identical despite different names*

### Comparing `brunns-matchers-2.6.0/src/brunns_matchers.egg-info/PKG-INFO` & `brunns-matchers-2.7.0/src/brunns_matchers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunns-matchers
-Version: 2.6.0
+Version: 2.7.0
 Summary: Custom PyHamcrest matchers
 Home-page: https://github.com/brunns/brunns-matchers/
 Author: Simon Brunning
 Author-email: simon@brunningonline.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7 
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # brunns-matchers
 
 Various custom [PyHamcrest](https://pyhamcrest.readthedocs.io) matchers.
 
@@ -59,15 +59,16 @@
     make help
 
 ## Releasing
 
 Requires [hub](https://hub.github.com/), [setuptools](https://setuptools.readthedocs.io), [wheel](https://pypi.org/project/wheel/) and [twine](https://twine.readthedocs.io). To release `n.n.n`:
 
 ```sh
-version="n.n.n"
-make precommit && git commit -am"Release $version" && git push # If not already all pushed, which it should be.
-hub release create $version -m"Release $version"
+version="n.n.n" # Needs to match new version number in setup.py.
+git checkout -b "release-$version"
+make precommit && git commit -am"Release $version" && git push --set-upstream origin "release-$version" # If not already all pushed, which it should be.
+hub release create "V$version" -t"release-$version" -m"Version $version"
 python setup.py sdist bdist_wheel
 twine upload dist/*$version*
 git checkout master
 git merge "release-$version"
 ```
```

### Comparing `brunns-matchers-2.6.0/src/brunns_matchers.egg-info/SOURCES.txt` & `brunns-matchers-2.7.0/src/brunns_matchers.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 src/brunns/__init__.py
 src/brunns/py.typed
 src/brunns/matchers/__init__.py
 src/brunns/matchers/bytestring.py
 src/brunns/matchers/data.py
@@ -13,13 +14,14 @@
 src/brunns/matchers/matcher.py
 src/brunns/matchers/mock.py
 src/brunns/matchers/object.py
 src/brunns/matchers/response.py
 src/brunns/matchers/smtp.py
 src/brunns/matchers/url.py
 src/brunns/matchers/utils.py
+src/brunns/matchers/werkzeug.py
 src/brunns_matchers.egg-info/PKG-INFO
 src/brunns_matchers.egg-info/SOURCES.txt
 src/brunns_matchers.egg-info/dependency_links.txt
 src/brunns_matchers.egg-info/not-zip-safe
 src/brunns_matchers.egg-info/requires.txt
 src/brunns_matchers.egg-info/top_level.txt
```

