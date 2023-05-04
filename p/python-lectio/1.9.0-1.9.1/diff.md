# Comparing `tmp/python-lectio-1.9.0.tar.gz` & `tmp/python-lectio-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lectio-1.9.0.tar", last modified: Thu Dec 22 12:05:00 2022, max compression
+gzip compressed data, was "python-lectio-1.9.1.tar", last modified: Thu Dec 22 13:01:51 2022, max compression
```

## Comparing `python-lectio-1.9.0.tar` & `python-lectio-1.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 12:05:00.287475 python-lectio-1.9.0/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2995 2022-12-22 12:05:00.287475 python-lectio-1.9.0/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2423 2022-11-13 09:40:50.000000 python-lectio-1.9.0/README.md
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 12:05:00.287475 python-lectio-1.9.0/lectio/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       23 2022-11-12 23:05:07.000000 python-lectio-1.9.0/lectio/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3298 2022-12-15 13:34:54.000000 python-lectio-1.9.0/lectio/_auth.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7130 2022-12-22 12:03:56.000000 python-lectio-1.9.0/lectio/_beskeder.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3107 2022-12-17 13:35:20.000000 python-lectio-1.9.0/lectio/_dokumenter.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       69 2022-11-13 13:47:04.000000 python-lectio-1.9.0/lectio/_filer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3094 2022-12-19 10:26:23.000000 python-lectio-1.9.0/lectio/_forside.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4923 2022-12-05 17:22:39.000000 python-lectio-1.9.0/lectio/_fravær.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2109 2022-12-11 11:33:40.000000 python-lectio-1.9.0/lectio/_informationer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      906 2022-12-17 15:46:10.000000 python-lectio-1.9.0/lectio/_lektier.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2715 2022-12-19 11:40:54.000000 python-lectio-1.9.0/lectio/_modul.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5281 2022-12-17 15:44:38.000000 python-lectio-1.9.0/lectio/_opgaver.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2965 2022-12-17 15:49:52.000000 python-lectio-1.9.0/lectio/_skema.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2102 2022-12-17 15:49:12.000000 python-lectio-1.9.0/lectio/_utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      181 2022-12-22 11:55:48.000000 python-lectio-1.9.0/lectio/imports.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2417 2022-12-22 12:03:38.000000 python-lectio-1.9.0/lectio/lectio.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 12:05:00.287475 python-lectio-1.9.0/python_lectio.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2995 2022-12-22 12:05:00.000000 python-lectio-1.9.0/python_lectio.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      483 2022-12-22 12:05:00.000000 python-lectio-1.9.0/python_lectio.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2022-12-22 12:05:00.000000 python-lectio-1.9.0/python_lectio.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       36 2022-12-22 12:05:00.000000 python-lectio-1.9.0/python_lectio.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        7 2022-12-22 12:05:00.000000 python-lectio-1.9.0/python_lectio.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2022-12-22 12:05:00.287475 python-lectio-1.9.0/setup.cfg
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1013 2022-12-22 12:04:54.000000 python-lectio-1.9.0/setup.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 13:01:51.048242 python-lectio-1.9.1/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2995 2022-12-22 13:01:51.048242 python-lectio-1.9.1/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2423 2022-11-13 09:40:50.000000 python-lectio-1.9.1/README.md
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 13:01:51.048242 python-lectio-1.9.1/lectio/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       23 2022-11-12 23:05:07.000000 python-lectio-1.9.1/lectio/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3298 2022-12-15 13:34:54.000000 python-lectio-1.9.1/lectio/_auth.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7254 2022-12-22 12:51:39.000000 python-lectio-1.9.1/lectio/_beskeder.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3107 2022-12-17 13:35:20.000000 python-lectio-1.9.1/lectio/_dokumenter.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       69 2022-11-13 13:47:04.000000 python-lectio-1.9.1/lectio/_filer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3094 2022-12-19 10:26:23.000000 python-lectio-1.9.1/lectio/_forside.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4923 2022-12-05 17:22:39.000000 python-lectio-1.9.1/lectio/_fravær.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2109 2022-12-11 11:33:40.000000 python-lectio-1.9.1/lectio/_informationer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      906 2022-12-17 15:46:10.000000 python-lectio-1.9.1/lectio/_lektier.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2715 2022-12-19 11:40:54.000000 python-lectio-1.9.1/lectio/_modul.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5281 2022-12-17 15:44:38.000000 python-lectio-1.9.1/lectio/_opgaver.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2965 2022-12-17 15:49:52.000000 python-lectio-1.9.1/lectio/_skema.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2102 2022-12-17 15:49:12.000000 python-lectio-1.9.1/lectio/_utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      181 2022-12-22 11:55:48.000000 python-lectio-1.9.1/lectio/imports.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2512 2022-12-22 13:01:29.000000 python-lectio-1.9.1/lectio/lectio.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2022-12-22 13:01:51.048242 python-lectio-1.9.1/python_lectio.egg-info/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2995 2022-12-22 13:01:51.000000 python-lectio-1.9.1/python_lectio.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      483 2022-12-22 13:01:51.000000 python-lectio-1.9.1/python_lectio.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2022-12-22 13:01:51.000000 python-lectio-1.9.1/python_lectio.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       36 2022-12-22 13:01:51.000000 python-lectio-1.9.1/python_lectio.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        7 2022-12-22 13:01:51.000000 python-lectio-1.9.1/python_lectio.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2022-12-22 13:01:51.048242 python-lectio-1.9.1/setup.cfg
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1013 2022-12-22 13:01:46.000000 python-lectio-1.9.1/setup.py
```

### Comparing `python-lectio-1.9.0/PKG-INFO` & `python-lectio-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lectio
-Version: 1.9.0
+Version: 1.9.1
 Summary: En SDK til gymnasie siden Lectio
 Home-page: https://github.com/jona799t/python-lectio
 Author: jona799t
 License: UNKNOWN
 Keywords: python,lectio,sdk,gymnasie,gymnasium
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `python-lectio-1.9.0/README.md` & `python-lectio-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_auth.py` & `python-lectio-1.9.1/lectio/_auth.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_beskeder.py` & `python-lectio-1.9.1/lectio/_beskeder.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,13 +134,17 @@
     payload["LectioPostbackId"] = ""
 
 
     resp = self.session.post(f"https://www.lectio.dk/lectio/{self.skoleId}/beskeder2.aspx?type=showthread&id={message_id}&elevid={self.elevId}", data=payload)
     soup = BeautifulSoup(resp.text, "html.parser")
 
     payload = _utils.generatePayload(soup, "s$m$Content$Content$CreateAnswerOKBtn")
-
-    resp = self.session.post(f"https://www.lectio.dk/lectio/{self.skoleId}/beskeder2.aspx?type=showthread&id={message_id}&elevid={message_id}", data=f"__LASTFOCUS=&time=0&__EVENTTARGET=s%24m%24Content%24Content%24CreateAnswerOKBtn&__EVENTARGUMENT=&__SCROLLPOSITION=&__VIEWSTATEX={urllib.parse.quote(payload['__VIEWSTATEX'])}&__VIEWSTATEY_KEY=&__VIEWSTATE=&__VIEWSTATEENCRYPTED=&s%24m%24searchinputfield=&s%24m%24Content%24Content%24addRecipientToAnswerDD%24inp=&s%24m%24Content%24Content%24addRecipientToAnswerDD%24inpid=&s%24m%24Content%24Content%24Notification=NotifyBtnAuthor&s%24m%24Content%24Content%24RepliesToResponseAllowed=on&s%24m%24Content%24Content%24CreateAnswerHeading%24tb={urllib.parse.quote(titel)}&s%24m%24Content%24Content%24CreateAnswerDocChooser%24selectedDocumentId=&s%24m%24Content%24Content%24CreateAnswerContent%24TbxNAME%24tb={urllib.parse.quote(content)}&masterfootervalue=X1%21%C3%86%C3%98%C3%85&LectioPostbackId=")
-    print(resp.status_code)
-
-
-    #resp = self.session.get(f"https://www.lectio.dk/lectio/681/beskeder2.aspx?type=liste&elevid=54443315275")
+    print(payload)
+    print(urllib.parse.quote(content))
+    print(urllib.parse.quote(titel))
+
+    resp = self.session.post(f"https://www.lectio.dk/lectio/{self.skoleId}/beskeder2.aspx?type=showthread&id={message_id}&elevid={message_id}", data=f"__LASTFOCUS=&time=0&__EVENTTARGET=s%24m%24Content%24Content%24CreateAnswerOKBtn&__EVENTARGUMENT=&__SCROLLPOSITION=&__VIEWSTATEX={urllib.parse.quote(payload['__VIEWSTATEX'])}&__VIEWSTATEY_KEY=&__VIEWSTATE=&__VIEWSTATEENCRYPTED=&s%24m%24searchinputfield=&s%24m%24Content%24Content%24addRecipientToAnswerDD%24inp=&s%24m%24Content%24Content%24addRecipientToAnswerDD%24inpid=&s%24m%24Content%24Content%24Notification=NotifyBtnAuthor&s%24m%24Content%24Content%24RepliesToResponseAllowed=on&s%24m%24Content%24Content%24CreateAnswerHeading%24tb={urllib.parse.quote(titel)}&s%24m%24Content%24Content%24CreateAnswerDocChooser%24selectedDocumentId=&s%24m%24Content%24Content%24CreateAnswerContent%24TbxNAME%24tb={urllib.parse.quote(content)}&masterfootervalue=X1%21%C3%86%C3%98%C3%85&LectioPostbackId=", allow_redirects=False)
+
+    if resp.status_code == 303:
+        return {"success": True}
+    else:
+        raise Exception("Levering af besvarelsen var ikke succesfuld")
```

### Comparing `python-lectio-1.9.0/lectio/_dokumenter.py` & `python-lectio-1.9.1/lectio/_dokumenter.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_forside.py` & `python-lectio-1.9.1/lectio/_forside.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_fravær.py` & `python-lectio-1.9.1/lectio/_fravær.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_informationer.py` & `python-lectio-1.9.1/lectio/_informationer.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_lektier.py` & `python-lectio-1.9.1/lectio/_lektier.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_modul.py` & `python-lectio-1.9.1/lectio/_modul.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_opgaver.py` & `python-lectio-1.9.1/lectio/_opgaver.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_skema.py` & `python-lectio-1.9.1/lectio/_skema.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/_utils.py` & `python-lectio-1.9.1/lectio/_utils.py`

 * *Files identical despite different names*

### Comparing `python-lectio-1.9.0/lectio/lectio.py` & `python-lectio-1.9.1/lectio/lectio.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             cookie = json.loads(base64.b64decode(base64Cookie))
             self.skoleId = cookie["LastLoginExamno"]
             self.elevId = cookie["LastLoginElevId"]
 
             for identifier, value in cookie.items():
                 self.session.cookies.set(identifier, value, domain="lectio.dk")
 
+            self.session.headers.update({"content-type": "application/x-www-form-urlencoded"})
     def login(self):
         return _auth.login(self)
 
     def base64Cookie(self):
         return _auth.base64Cookie(self)
 
     def lektier(self):
```

### Comparing `python-lectio-1.9.0/python_lectio.egg-info/PKG-INFO` & `python-lectio-1.9.1/python_lectio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lectio
-Version: 1.9.0
+Version: 1.9.1
 Summary: En SDK til gymnasie siden Lectio
 Home-page: https://github.com/jona799t/python-lectio
 Author: jona799t
 License: UNKNOWN
 Keywords: python,lectio,sdk,gymnasie,gymnasium
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `python-lectio-1.9.0/setup.py` & `python-lectio-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = '1.9.0'
+VERSION = '1.9.1'
 DESCRIPTION = 'En SDK til gymnasie siden Lectio'
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 # Setting up
 setup(
     name="python-lectio",
     version=VERSION,
```

