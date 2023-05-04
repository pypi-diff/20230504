# Comparing `tmp/vnfaker-0.0.3.tar.gz` & `tmp/vnfaker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnfaker-0.0.3.tar", last modified: Thu May  4 08:39:49 2023, max compression
+gzip compressed data, was "vnfaker-0.0.4.tar", last modified: Thu May  4 09:54:59 2023, max compression
```

## Comparing `vnfaker-0.0.3.tar` & `vnfaker-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.559720 vnfaker-0.0.3/
--rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.3/LICENSE.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 08:39:49.559206 vnfaker-0.0.3/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.3/README.md
--rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-04 08:39:49.559939 vnfaker-0.0.3/setup.cfg
--rw-r--r--   0 ducquang   (501) admin       (80)     1033 2023-05-04 08:23:44.000000 vnfaker-0.0.3/setup.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.515515 vnfaker-0.0.3/src/
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.520598 vnfaker-0.0.3/src/vnfaker/
--rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.3/src/vnfaker/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     3102 2023-05-04 08:37:58.000000 vnfaker-0.0.3/src/vnfaker/commonUtils.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.524644 vnfaker-0.0.3/src/vnfaker/data/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.3/src/vnfaker/data/__init__.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.525374 vnfaker-0.0.3/src/vnfaker/data/company/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/company/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    14530 2023-05-01 04:39:51.000000 vnfaker-0.0.3/src/vnfaker/data/company/company.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.526574 vnfaker-0.0.3/src/vnfaker/data/occupation/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/occupation/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.3/src/vnfaker/data/occupation/occupation.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.532832 vnfaker-0.0.3/src/vnfaker/data/person/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/person/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     1132 2023-05-01 04:04:14.000000 vnfaker-0.0.3/src/vnfaker/data/person/female.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-05-01 04:04:55.000000 vnfaker-0.0.3/src/vnfaker/data/person/female_middle.name
--rw-r--r--   0 ducquang   (501) admin       (80)      439 2023-05-02 10:33:11.000000 vnfaker-0.0.3/src/vnfaker/data/person/last.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1778 2023-05-01 03:46:35.000000 vnfaker-0.0.3/src/vnfaker/data/person/male.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1172 2023-05-01 04:09:43.000000 vnfaker-0.0.3/src/vnfaker/data/person/male_middle.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.543090 vnfaker-0.0.3/src/vnfaker/data/provinces/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/flat-divisions.json
--rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.3/src/vnfaker/data/provinces/nested-divisions.json
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.553657 vnfaker-0.0.3/src/vnfaker/data/religion/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-05-04 08:18:11.000000 vnfaker-0.0.3/src/vnfaker/data/religion/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)      363 2023-05-04 08:20:57.000000 vnfaker-0.0.3/src/vnfaker/data/religion/religion.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.555331 vnfaker-0.0.3/src/vnfaker/data/sentence/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.3/src/vnfaker/data/sentence/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.3/src/vnfaker/data/sentence/sentence.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     9682 2023-05-04 08:32:39.000000 vnfaker-0.0.3/src/vnfaker/generator.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 08:39:49.524177 vnfaker-0.0.3/src/vnfaker.egg-info/
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)      982 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/SOURCES.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/dependency_links.txt
--rw-r--r--   0 ducquang   (501) admin       (80)       32 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/requires.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-04 08:39:49.000000 vnfaker-0.0.3/src/vnfaker.egg-info/top_level.txt
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.605848 vnfaker-0.0.4/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.4/LICENSE.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 09:54:59.605461 vnfaker-0.0.4/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.4/README.md
+-rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-04 09:54:59.606043 vnfaker-0.0.4/setup.cfg
+-rw-r--r--   0 ducquang   (501) admin       (80)     1033 2023-05-04 09:54:41.000000 vnfaker-0.0.4/setup.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.570328 vnfaker-0.0.4/src/
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.575322 vnfaker-0.0.4/src/vnfaker/
+-rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.4/src/vnfaker/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     3102 2023-05-04 09:14:37.000000 vnfaker-0.0.4/src/vnfaker/commonUtils.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.579537 vnfaker-0.0.4/src/vnfaker/data/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.4/src/vnfaker/data/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.581898 vnfaker-0.0.4/src/vnfaker/data/company/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/company/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    14530 2023-05-01 04:39:51.000000 vnfaker-0.0.4/src/vnfaker/data/company/company.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.584691 vnfaker-0.0.4/src/vnfaker/data/occupation/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/occupation/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.4/src/vnfaker/data/occupation/occupation.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.588488 vnfaker-0.0.4/src/vnfaker/data/person/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/person/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     1132 2023-05-01 04:04:14.000000 vnfaker-0.0.4/src/vnfaker/data/person/female.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-05-01 04:04:55.000000 vnfaker-0.0.4/src/vnfaker/data/person/female_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      439 2023-05-02 10:33:11.000000 vnfaker-0.0.4/src/vnfaker/data/person/last.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1778 2023-05-01 03:46:35.000000 vnfaker-0.0.4/src/vnfaker/data/person/male.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1172 2023-05-01 04:09:43.000000 vnfaker-0.0.4/src/vnfaker/data/person/male_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      363 2023-05-04 08:20:57.000000 vnfaker-0.0.4/src/vnfaker/data/person/religion.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.599377 vnfaker-0.0.4/src/vnfaker/data/provinces/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/flat-divisions.json
+-rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.4/src/vnfaker/data/provinces/nested-divisions.json
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.603540 vnfaker-0.0.4/src/vnfaker/data/religion/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-05-04 08:18:11.000000 vnfaker-0.0.4/src/vnfaker/data/religion/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.604384 vnfaker-0.0.4/src/vnfaker/data/sentence/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.4/src/vnfaker/data/sentence/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.4/src/vnfaker/data/sentence/sentence.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     9674 2023-05-04 09:54:41.000000 vnfaker-0.0.4/src/vnfaker/generator.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-04 09:54:59.578824 vnfaker-0.0.4/src/vnfaker.egg-info/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)      980 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/SOURCES.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/dependency_links.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)       32 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/requires.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-04 09:54:59.000000 vnfaker-0.0.4/src/vnfaker.egg-info/top_level.txt
```

### Comparing `vnfaker-0.0.3/LICENSE.txt` & `vnfaker-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/PKG-INFO` & `vnfaker-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.3
+Version: 0.0.4
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.3/README.md` & `vnfaker-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/setup.py` & `vnfaker-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     README = fh.read()
 
 setuptools.setup(
     name="vnfaker",
-    version="0.0.3",
+    version="0.0.4",
     author="Phan Duc Quang",
     author_email="phanducquang07@gmail.com",
     description="vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/phanducquang/vnfaker",
     project_urls={
```

### Comparing `vnfaker-0.0.3/src/vnfaker/commonUtils.py` & `vnfaker-0.0.4/src/vnfaker/commonUtils.py`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/company/company.name` & `vnfaker-0.0.4/src/vnfaker/data/company/company.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/occupation/occupation.name` & `vnfaker-0.0.4/src/vnfaker/data/occupation/occupation.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/person/female.name` & `vnfaker-0.0.4/src/vnfaker/data/person/female.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/person/female_middle.name` & `vnfaker-0.0.4/src/vnfaker/data/person/female_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/person/male.name` & `vnfaker-0.0.4/src/vnfaker/data/person/male.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/person/male_middle.name` & `vnfaker-0.0.4/src/vnfaker/data/person/male_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/provinces/flat-divisions.json` & `vnfaker-0.0.4/src/vnfaker/data/provinces/flat-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/provinces/nested-divisions.json` & `vnfaker-0.0.4/src/vnfaker/data/provinces/nested-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/data/sentence/sentence.txt` & `vnfaker-0.0.4/src/vnfaker/data/sentence/sentence.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.3/src/vnfaker/generator.py` & `vnfaker-0.0.4/src/vnfaker/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,17 +171,17 @@
         if timestamp:
             return datetime.fromisoformat(self.__birth_date.isoformat()).timestamp() * 1000
         return self.__birth_date
 
     def address(self):
         if self.__address_value is None:
             address_value_obj = random.choice(CommonUtils.address)
-            self.__province_name = address_value_obj.get("__province_name")
-            self.__ward_name = address_value_obj.get("__ward_name")
-            self.__district_name = address_value_obj.get("__district_name")
+            self.__province_name = address_value_obj.get("province_name")
+            self.__ward_name = address_value_obj.get("ward_name")
+            self.__district_name = address_value_obj.get("district_name")
             self.__address_value = "{}, {}, {}".format(self.__ward_name,
                                                        self.__district_name,
                                                        self.__province_name)
         return self.__address_value
 
     def address_province(self):
         if self.__address_value is None:
@@ -201,15 +201,15 @@
     def company(self):
         if self.__company_value is None:
             self.__company_value = random.choice(CommonUtils.companyNames)
         return self.__company_value
 
     def known_location(self):
         if self.__known_location_value is None:
-            self.__known_location_value = [random.choice(CommonUtils.address).get("__province_name") for _ in
+            self.__known_location_value = [random.choice(CommonUtils.address).get("province_name") for _ in
                                            range(random.randint(1, 5))]
         return self.__known_location_value
 
     def occupation(self):
         if self.__occupation_value is None:
             self.__occupation_value = random.choice(CommonUtils.occupationNames)
         return self.__occupation_value
```

### Comparing `vnfaker-0.0.3/src/vnfaker.egg-info/PKG-INFO` & `vnfaker-0.0.4/src/vnfaker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.3
+Version: 0.0.4
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.3/src/vnfaker.egg-info/SOURCES.txt` & `vnfaker-0.0.4/src/vnfaker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 src/vnfaker/data/occupation/occupation.name
 src/vnfaker/data/person/__init__.py
 src/vnfaker/data/person/female.name
 src/vnfaker/data/person/female_middle.name
 src/vnfaker/data/person/last.name
 src/vnfaker/data/person/male.name
 src/vnfaker/data/person/male_middle.name
+src/vnfaker/data/person/religion.name
 src/vnfaker/data/provinces/__init__.py
 src/vnfaker/data/provinces/flat-divisions.json
 src/vnfaker/data/provinces/nested-divisions.json
 src/vnfaker/data/religion/__init__.py
-src/vnfaker/data/religion/religion.name
 src/vnfaker/data/sentence/__init__.py
 src/vnfaker/data/sentence/sentence.txt
```

