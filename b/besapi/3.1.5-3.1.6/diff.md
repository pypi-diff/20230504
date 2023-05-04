# Comparing `tmp/besapi-3.1.5.tar.gz` & `tmp/besapi-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besapi-3.1.5.tar", last modified: Tue Apr 11 13:25:13 2023, max compression
+gzip compressed data, was "besapi-3.1.6.tar", last modified: Thu May  4 10:32:56 2023, max compression
```

## Comparing `besapi-3.1.5.tar` & `besapi-3.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 13:18:54.000000 besapi-3.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 13:18:54.000000 besapi-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:25:13.386768 besapi-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-11 13:18:54.000000 besapi-3.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 13:18:54.000000 besapi-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-11 13:25:13.386768 besapi-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-11 13:18:54.000000 besapi-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.378768 besapi-3.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/besapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    42635 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BES.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    25664 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BESAPI.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BESActionSettings.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/src/bescli/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/bescli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 13:18:54.000000 besapi-3.1.5/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.218427 besapi-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 10:25:58.000000 besapi-3.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 10:25:58.000000 besapi-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-04 10:32:56.218427 besapi-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-04 10:25:58.000000 besapi-3.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 10:25:58.000000 besapi-3.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 10:32:56.218427 besapi-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 10:25:58.000000 besapi-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.214427 besapi-3.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.214427 besapi-3.1.6/src/besapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35288 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/besapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.218427 besapi-3.1.6/src/besapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    42635 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/schemas/BES.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    25664 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/schemas/BESAPI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-05-04 10:25:58.000000 besapi-3.1.6/src/besapi/schemas/BESActionSettings.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.218427 besapi-3.1.6/src/besapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-04 10:32:56.000000 besapi-3.1.6/src/besapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-04 10:32:56.000000 besapi-3.1.6/src/besapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:32:56.000000 besapi-3.1.6/src/besapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 10:32:56.000000 besapi-3.1.6/src/besapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 10:32:56.000000 besapi-3.1.6/src/besapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.218427 besapi-3.1.6/src/bescli/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-04 10:25:58.000000 besapi-3.1.6/src/bescli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 10:25:58.000000 besapi-3.1.6/src/bescli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-04 10:25:58.000000 besapi-3.1.6/src/bescli/bescli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:32:56.218427 besapi-3.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-04 10:25:58.000000 besapi-3.1.6/tests/tests.py
```

### Comparing `besapi-3.1.5/LICENSE.txt` & `besapi-3.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/PKG-INFO` & `besapi-3.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.1.5
+Version: 3.1.6
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/CLCMacTeam/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.1.5/README.md` & `besapi-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/setup.py` & `besapi-3.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/src/besapi/besapi.py` & `besapi-3.1.6/src/besapi/besapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Library for communicating with the BES (BigFix) REST API.
 """
 
 import configparser
 import datetime
 import hashlib
+import io
 import json
 import logging
 import os
 import random
 import site
 import string
 
@@ -146,14 +147,38 @@
 #             maxsize=maxsize,
 #             block=block,
 #             strict=True,
 #             **pool_kwargs,
 #         )
 
 
+def validate_xsd(doc):
+    """validate results using XML XSDs"""
+    try:
+        xmldoc = etree.fromstring(doc)
+    except BaseException:  # pylint: disable=broad-except
+        return False
+
+    for xsd in ["BES.xsd", "BESAPI.xsd", "BESActionSettings.xsd"]:
+        xmlschema_doc = etree.parse(resource_filename(__name__, "schemas/%s" % xsd))
+
+        # one schema may throw an error while another will validate
+        try:
+            xmlschema = etree.XMLSchema(xmlschema_doc)
+        except etree.XMLSchemaParseError as err:
+            # this should only error if the XSD itself is malformed
+            besapi_logger.error("ERROR with `%s`: %s", xsd, err)
+            raise err
+
+        if xmlschema.validate(xmldoc):
+            return True
+
+    return False
+
+
 def get_bes_conn_using_config_file(conf_file=None):
     """
     read connection values from config file
     return besapi connection
     """
     config_paths = [
         "/etc/besapi.conf",
@@ -169,25 +194,25 @@
 
     found_config_files = configparser_instance.read(config_paths)
 
     if found_config_files and configparser_instance:
         print("Attempting BESAPI Connection using config file:", found_config_files)
         try:
             BES_ROOT_SERVER = configparser_instance.get("besapi", "BES_ROOT_SERVER")
-        except BaseException:
+        except BaseException:  # pylint: disable=broad-except
             BES_ROOT_SERVER = None
 
         try:
             BES_USER_NAME = configparser_instance.get("besapi", "BES_USER_NAME")
-        except BaseException:
+        except BaseException:  # pylint: disable=broad-except
             BES_USER_NAME = None
 
         try:
             BES_PASSWORD = configparser_instance.get("besapi", "BES_PASSWORD")
-        except BaseException:
+        except BaseException:  # pylint: disable=broad-except
             BES_PASSWORD = None
 
         if BES_ROOT_SERVER and BES_USER_NAME and BES_PASSWORD:
             return BESConnection(BES_USER_NAME, BES_PASSWORD, BES_ROOT_SERVER)
 
     return None
 
@@ -218,15 +243,15 @@
         if not rootserver.count(":") == 2:
             rootserver = rootserver + ":52311"
 
         self.rootserver = rootserver
         try:
             # get root server port
             self.rootserver_port = int(rootserver.split("://", 1)[1].split(":", 1)[1])
-        except BaseException:
+        except BaseException:  # pylint: disable=broad-except
             # if error, assume default
             self.rootserver_port = 52311
 
         self.login()
 
     def __repr__(self):
         """object representation"""
@@ -309,20 +334,20 @@
             for item in rel_result.besobj.Query.Result.Answer:
                 result.append(item.text)
         except AttributeError as err:
             # print(err)
             if "no such child: Answer" in str(err):
                 try:
                     result.append("ERROR: " + rel_result.besobj.Query.Error.text)
-                except AttributeError as err:
-                    if "no such child: Error" in str(err):
+                except AttributeError as err2:
+                    if "no such child: Error" in str(err2):
                         result.append("<Nothing> Nothing returned, but no error.")
                         besapi_logger.info("Query did not return any results")
                     else:
-                        besapi_logger.error("%s\n%s", err, rel_result.text)
+                        besapi_logger.error("%s\n%s", err2, rel_result.text)
                         raise
             else:
                 raise
         return result
 
     def session_relevance_string(self, relevance, **kwargs):
         """Get Session Relevance Results string"""
@@ -386,26 +411,26 @@
                     # Invalid: This error should be raised regardless
                     raise ValueError(
                         f"Site path for master actionsite must be `master` not `{site_path}`"
                     )
                 if not check_site_exists:
                     # don't check if site exists first
                     return site_path
-                else:
-                    # check site exists first
-                    site_result = self.get(f"site/{site_path}")
-                    if site_result.request.status_code != 200:
-                        besapi_logger.info("Site `%s` does not exist", site_path)
-                        if not raise_error:
-                            return None
 
-                        raise ValueError(f"Site at path `{site_path}` does not exist!")
+                # check site exists first
+                site_result = self.get(f"site/{site_path}")
+                if site_result.request.status_code != 200:
+                    besapi_logger.info("Site `%s` does not exist", site_path)
+                    if not raise_error:
+                        return None
 
-                    # site_path is valid and exists:
-                    return site_path
+                    raise ValueError(f"Site at path `{site_path}` does not exist!")
+
+                # site_path is valid and exists:
+                return site_path
 
         # Invalid: No valid prefix found
         raise ValueError(
             f"Site Path does not start with a valid prefix! {site_prefixes}"
         )
 
     def get_current_site_path(self, site_path=None):
@@ -426,14 +451,37 @@
     def set_current_site_path(self, site_path):
         """set current site path context"""
 
         if self.validate_site_path(site_path):
             self.site_path = site_path
             return self.site_path
 
+    def import_bes_to_site(self, bes_file_path, site_path=None):
+        """import bes file to site"""
+
+        if not os.access(bes_file_path, os.R_OK):
+            besapi_logger.error("%s is not readable", bes_file_path)
+            raise FileNotFoundError(f"{bes_file_path} is not readable")
+
+        site_path = self.get_current_site_path(site_path)
+
+        self.validate_site_path(site_path, False, True)
+
+        with open(bes_file_path, "rb") as f:
+            content = f.read()
+
+            # validate BES File contents:
+            if not validate_xsd(content):
+                besapi_logger.error("%s is not valid", bes_file_path)
+                return None
+
+            # https://developer.bigfix.com/rest-api/api/import.html
+            result = self.post(f"import/{site_path}", content)
+            return result
+
     def create_site_from_file(self, bes_file_path, site_type="custom"):
         """create new site"""
         xml_parsed = etree.parse(bes_file_path)
         new_site_name = xml_parsed.xpath("/BES/CustomSite/Name/text()")[0]
 
         result_site_path = self.validate_site_path(
             site_type + "/" + new_site_name, True, False
@@ -557,15 +605,15 @@
                     sha1.update(data)
             file_hash = sha1.hexdigest()
 
         check_upload = None
         if file_hash:
             try:
                 check_upload = self.get_upload(str(file_name), str(file_hash))
-            except BaseException as err:
+            except BaseException as err:  # pylint: disable=broad-except
                 print(err)
 
             if check_upload:
                 besapi_logger.warning(
                     "Existing Matching Upload Found, Skipping Upload!"
                 )
                 # return same data as if we had uploaded
@@ -617,14 +665,21 @@
         #     site_path = resource_url.split("/")[-3] + "/" + site_name
         return content
 
     def update_item_from_file(self, file_path, site_path=None):
         """update an item by name and last modified"""
         site_path = self.get_current_site_path(site_path)
         bes_tree = etree.parse(file_path)
+
+        with open(file_path, "rb") as f:
+            content = f.read()
+            if not validate_xsd(content):
+                besapi_logger.error("%s is not valid", file_path)
+                return None
+
         # get name of first child tag of BES
         # - https://stackoverflow.com/a/3601919/861745
         bes_type = str(bes_tree.xpath("name(/BES/*[1])"))
         bes_title = bes_tree.xpath("/BES/*[1]/Title/text()")[0]
         # get last modification time:
         bes_last_mod = bes_tree.xpath(
             '/BES/*[1]/MIMEField[Name[contains(text(), "x-fixlet-modification-time")]]/Value/text()'
@@ -859,15 +914,15 @@
                 self.valid = False
 
     def __str__(self):
         if self.valid:
             # I think this is needed for python3 compatibility:
             try:
                 return self.besxml.decode("utf-8")
-            except BaseException:
+            except BaseException:  # pylint: disable=broad-except
                 return self.besxml
         else:
             return self.text
 
     def __call__(self):
         return self.besobj
 
@@ -904,34 +959,15 @@
         if self._besjson is None:
             self._besjson = json.dumps(self.besdict, indent=2)
 
         return self._besjson
 
     def validate_xsd(self, doc):
         """validate results using XML XSDs"""
-        try:
-            xmldoc = etree.fromstring(doc)
-        except BaseException:
-            return False
-
-        for xsd in ["BES.xsd", "BESAPI.xsd", "BESActionSettings.xsd"]:
-            xmlschema_doc = etree.parse(resource_filename(__name__, "schemas/%s" % xsd))
-
-            # one schema may throw an error while another will validate
-            try:
-                xmlschema = etree.XMLSchema(xmlschema_doc)
-            except etree.XMLSchemaParseError as err:
-                # this should only error if the XSD itself is malformed
-                besapi_logger.error("ERROR with `%s`: %s", xsd, err)
-                raise err
-
-            if xmlschema.validate(xmldoc):
-                return True
-
-        return False
+        return validate_xsd(doc)
 
     def xmlparse_text(self, text):
         """parse response text as xml"""
         if type(text) is str:
             root_xml = etree.fromstring(text.encode("utf-8"))
         else:
             root_xml = text
```

### Comparing `besapi-3.1.5/src/besapi/schemas/BES.xsd` & `besapi-3.1.6/src/besapi/schemas/BES.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/src/besapi/schemas/BESAPI.xsd` & `besapi-3.1.6/src/besapi/schemas/BESAPI.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/src/besapi/schemas/BESActionSettings.xsd` & `besapi-3.1.6/src/besapi/schemas/BESActionSettings.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.5/src/besapi.egg-info/PKG-INFO` & `besapi-3.1.6/src/besapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.1.5
+Version: 3.1.6
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/CLCMacTeam/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.1.5/src/bescli/bescli.py` & `besapi-3.1.6/src/bescli/bescli.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,23 @@
             site_path, verbose=True, include_site_folder=False, include_item_ids=False
         )
 
     def do_export_all_sites(self, statement=None):
         """export site contents to current folder"""
         self.bes_conn.export_all_sites(verbose=False)
 
+    complete_import_bes = Cmd.path_complete
+
+    def do_import_bes(self, statement):
+        """import bes file"""
+
+        self.poutput(f"Import file: {statement.args}")
+
+        self.poutput(self.bes_conn.import_bes_to_site(str(statement.args)))
+
     complete_upload = Cmd.path_complete
 
     def do_upload(self, file_path):
         """upload file to root server"""
         if not os.access(file_path, os.R_OK):
             print(file_path, "is not a readable file")
         else:
```

### Comparing `besapi-3.1.5/tests/tests.py` & `besapi-3.1.6/tests/tests.py`

 * *Files identical despite different names*

