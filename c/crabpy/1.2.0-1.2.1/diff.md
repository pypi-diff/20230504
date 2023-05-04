# Comparing `tmp/crabpy-1.2.0.tar.gz` & `tmp/crabpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy-1.2.0.tar", last modified: Thu May  4 09:43:24 2023, max compression
+gzip compressed data, was "crabpy-1.2.1.tar", last modified: Thu May  4 13:36:33 2023, max compression
```

## Comparing `crabpy-1.2.0.tar` & `crabpy-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 09:43:24.480880 crabpy-1.2.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6573 2023-05-04 09:43:10.000000 crabpy-1.2.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8224 2023-05-04 09:43:24.480880 crabpy-1.2.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 09:43:24.476880 crabpy-1.2.0/crabpy/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/client.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 09:43:24.480880 crabpy-1.2.0/crabpy/data/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.2.0/crabpy/data/deelgemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.0/crabpy/data/gemeenten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.0/crabpy/data/gewesten.json
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.0/crabpy/data/provincies.json
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 09:43:24.480880 crabpy-1.2.0/crabpy/gateway/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/gateway/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30060 2023-05-04 09:43:10.000000 crabpy-1.2.0/crabpy/gateway/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/gateway/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/gateway/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/gateway/exception.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/wsa.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.0/crabpy/wsse.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 09:43:24.476880 crabpy-1.2.0/crabpy.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8224 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.0/crabpy.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-04 09:43:24.000000 crabpy-1.2.0/crabpy.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-04 09:43:24.480880 crabpy-1.2.0/setup.cfg
--rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-04 09:43:10.000000 crabpy-1.2.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6641 2023-05-04 13:36:14.000000 crabpy-1.2.1/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 12:57:29.000000 crabpy-1.2.1/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       76 2023-04-13 12:57:29.000000 crabpy-1.2.1/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8292 2023-05-04 13:36:33.274009 crabpy-1.2.1/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      941 2023-04-13 12:57:29.000000 crabpy-1.2.1/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.270009 crabpy-1.2.1/crabpy/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7372 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/client.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy/data/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   238209 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/deelgemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)   167480 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/gemeenten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      547 2023-05-03 12:29:06.000000 crabpy-1.2.1/crabpy/data/gewesten.json
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      803 2023-05-04 09:43:10.000000 crabpy-1.2.1/crabpy/data/provincies.json
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy/gateway/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    30229 2023-05-04 13:36:14.000000 crabpy-1.2.1/crabpy/gateway/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    28420 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    85501 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      991 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/gateway/exception.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1083 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/wsa.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2719 2023-04-13 12:57:29.000000 crabpy-1.2.1/crabpy/wsse.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-04 13:36:33.274009 crabpy-1.2.1/crabpy.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     8292 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      578 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 12:57:59.000000 crabpy-1.2.1/crabpy.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       41 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        7 2023-05-04 13:36:33.000000 crabpy-1.2.1/crabpy.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       38 2023-05-04 13:36:33.274009 crabpy-1.2.1/setup.cfg
+-rwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)     1278 2023-05-04 13:36:14.000000 crabpy-1.2.1/setup.py
```

### Comparing `crabpy-1.2.0/CHANGES.rst` & `crabpy-1.2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.2.1 (04-05-2023)
+------------------
+
+- Adressenregister bugfixes
+
 1.2.0 (04-05-2023)
 ------------------
 
 - uniformiseer alles naar niscodes en check dat alle niscodes strings zijn (#208)
 - errors checken en fine tunen (#209)
 
 1.1.0 (03-05-2023)
```

### Comparing `crabpy-1.2.0/LICENSE` & `crabpy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/PKG-INFO` & `crabpy-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.1 (04-05-2023)
+------------------
+
+- Adressenregister bugfixes
+
 1.2.0 (04-05-2023)
 ------------------
 
 - uniformiseer alles naar niscodes en check dat alle niscodes strings zijn (#208)
 - errors checken en fine tunen (#209)
 
 1.1.0 (03-05-2023)
```

### Comparing `crabpy-1.2.0/README.rst` & `crabpy-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/client.py` & `crabpy-1.2.1/crabpy/client.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/data/deelgemeenten.json` & `crabpy-1.2.1/crabpy/data/deelgemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/data/gemeenten.json` & `crabpy-1.2.1/crabpy/data/gemeenten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/data/gewesten.json` & `crabpy-1.2.1/crabpy/data/gewesten.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/data/provincies.json` & `crabpy-1.2.1/crabpy/data/provincies.json`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/gateway/adressenregister.py` & `crabpy-1.2.1/crabpy/gateway/adressenregister.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         """
         return [
             provincie
             for provincie in self.provincies
             if provincie.gewest_niscode == gewest_niscode
         ]
 
-    def get_provincie_by_id(self, niscode):
+    def get_provincie_by_niscode(self, niscode):
         """
         Retrieve a `provincie` by the niscode.
 
         :param str niscode: The niscode of the provincie.
         :rtype: :class:`Provincie`
         """
         niscode = niscode
@@ -202,15 +202,17 @@
         List all `gemeenten` in a `provincie`.
 
         :param provincie: The :class:`Provincie` for which the \
             `gemeenten` are wanted.
         :rtype: A :class:`list` of :class:`Gemeente`.
         """
         if not isinstance(provincie, Provincie):
-            provincie = self.get_provincie_by_id(provincie)
+            provincie = self.get_provincie_by_niscode(provincie)
+        if provincie is None:
+            return []
         provincie_niscode = provincie.niscode
         return [
             gemeente
             for gemeente in self.gemeenten
             if gemeente.provincie_niscode == provincie_niscode
         ]
 
@@ -300,14 +302,16 @@
 
         :param gemeente: The :class:`Gemeente` for which the \
             `deelgemeenten` are wanted. Currently only Flanders is supported.
         :rtype: A :class:`list` of :class:`Deelgemeente`.
         """
         if not isinstance(gemeente, Gemeente):
             gemeente = self.get_gemeente_by_niscode(gemeente)
+        if gemeente is None:
+            return []
         return [
             deelgemeente
             for deelgemeente in self.deelgemeenten
             if deelgemeente.gemeente_niscode == gemeente.niscode
         ]
 
     def get_deelgemeente_by_id(self, deelgemeente_id):
@@ -333,14 +337,16 @@
 
         :param gemeente: The :class:`Gemeente` for which the \
             `straten` are wanted.
         :rtype: A :class:`list` of :class:`Straat`
         """
         if not isinstance(gemeente, Gemeente):
             gemeente = self.get_gemeente_by_niscode(gemeente)
+        if gemeente is None:
+            return []
         return [
             Straat.from_list_response(straat, self)
             for straat in self.client.get_straatnamen(niscode=gemeente.niscode)
         ]
 
     @LONG_CACHE.cache_on_arguments()
     def get_straat_by_id(self, straat_id):
@@ -572,15 +578,15 @@
     @LazyProperty
     def postinfo(self):
         gemeente_naam = self.naam() if not isinstance(self.naam, str) else self.naam
         return self.gateway.get_postinfo_by_gemeentenaam(gemeente_naam)
 
     @LazyProperty
     def provincie(self):
-        return self.gateway.get_provincie_by_id(self.provincie_niscode)
+        return self.gateway.get_provincie_by_niscode(self.provincie_niscode)
 
     @LazyProperty
     def gewest(self):
         return self.gateway.get_gewest_by_niscode(self.provincie.gewest_niscode)
 
     def __str__(self):
         return f"{self.naam} ({self.niscode})"
```

### Comparing `crabpy-1.2.0/crabpy/gateway/capakey.py` & `crabpy-1.2.1/crabpy/gateway/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/gateway/crab.py` & `crabpy-1.2.1/crabpy/gateway/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/gateway/exception.py` & `crabpy-1.2.1/crabpy/gateway/exception.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/wsa.py` & `crabpy-1.2.1/crabpy/wsa.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy/wsse.py` & `crabpy-1.2.1/crabpy/wsse.py`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/crabpy.egg-info/PKG-INFO` & `crabpy-1.2.1/crabpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Interact with geographical webservices by Informatie Vlaanderen.
 Home-page: http://github.com/onroerenderfgoed/crabpy
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
         :target: https://travis-ci.org/OnroerendErfgoed/crabpy
 .. image:: https://coveralls.io/repos/OnroerendErfgoed/crabpy/badge.png?branch=master
         :target: https://coveralls.io/r/OnroerendErfgoed/crabpy?branch=master
 .. image:: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/badges/quality-score.png?b=master
         :target: https://scrutinizer-ci.com/g/OnroerendErfgoed/crabpy/?branch=master
 
 
+1.2.1 (04-05-2023)
+------------------
+
+- Adressenregister bugfixes
+
 1.2.0 (04-05-2023)
 ------------------
 
 - uniformiseer alles naar niscodes en check dat alle niscodes strings zijn (#208)
 - errors checken en fine tunen (#209)
 
 1.1.0 (03-05-2023)
```

### Comparing `crabpy-1.2.0/crabpy.egg-info/SOURCES.txt` & `crabpy-1.2.1/crabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy-1.2.0/setup.py` & `crabpy-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "crabpy",
 ]
 
 requires = ["suds-py3>=1.4.4.1", "dogpile.cache", "requests"]
 
 setup(
     name="crabpy",
-    version="1.2.0",
+    version="1.2.1",
     description="Interact with geographical webservices by Informatie Vlaanderen.",
     long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
     author="Onroerend Erfgoed",
     author_email="ict@onroerenderfgoed.be",
     url="http://github.com/onroerenderfgoed/crabpy",
     packages=find_packages(exclude=["tests*"]),
     package_data={"": ["LICENSE"]},
```

