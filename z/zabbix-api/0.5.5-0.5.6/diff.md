# Comparing `tmp/zabbix-api-0.5.5.tar.gz` & `tmp/zabbix-api-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zabbix-api-0.5.5.tar", last modified: Tue Nov  8 21:59:23 2022, max compression
+gzip compressed data, was "zabbix-api-0.5.6.tar", last modified: Thu May  4 06:15:18 2023, max compression
```

## Comparing `zabbix-api-0.5.5.tar` & `zabbix-api-0.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)        0 2022-11-08 21:59:23.524641 zabbix-api-0.5.5/
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       18 2022-11-08 21:55:45.000000 zabbix-api-0.5.5/MANIFEST.in
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)     1223 2022-11-08 21:59:23.524045 zabbix-api-0.5.5/PKG-INFO
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)      809 2022-11-08 21:55:45.000000 zabbix-api-0.5.5/README.md
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       38 2022-11-08 21:59:23.524758 zabbix-api-0.5.5/setup.cfg
--rwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)     1028 2022-11-08 21:55:46.000000 zabbix-api-0.5.5/setup.py
-drwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)        0 2022-11-08 21:59:23.523500 zabbix-api-0.5.5/zabbix_api.egg-info/
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)     1223 2022-11-08 21:59:23.000000 zabbix-api-0.5.5/zabbix_api.egg-info/PKG-INFO
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)      213 2022-11-08 21:59:23.000000 zabbix-api-0.5.5/zabbix_api.egg-info/SOURCES.txt
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)        1 2022-11-08 21:59:23.000000 zabbix-api-0.5.5/zabbix_api.egg-info/dependency_links.txt
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)        1 2022-11-08 21:59:23.000000 zabbix-api-0.5.5/zabbix_api.egg-info/not-zip-safe
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       11 2022-11-08 21:59:23.000000 zabbix-api-0.5.5/zabbix_api.egg-info/top_level.txt
--rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)    12597 2022-11-08 21:55:46.000000 zabbix-api-0.5.5/zabbix_api.py
+drwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)        0 2023-05-04 06:15:18.936938 zabbix-api-0.5.6/
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       18 2022-11-08 21:55:45.000000 zabbix-api-0.5.6/MANIFEST.in
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)     1223 2023-05-04 06:15:18.936356 zabbix-api-0.5.6/PKG-INFO
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)      809 2022-11-08 21:55:45.000000 zabbix-api-0.5.6/README.md
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       38 2023-05-04 06:15:18.937063 zabbix-api-0.5.6/setup.cfg
+-rwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)     1028 2023-04-28 16:17:57.000000 zabbix-api-0.5.6/setup.py
+drwxr-xr-x   0 gescheit (2114722489) LD\Domain Users (593637566)        0 2023-05-04 06:15:18.935492 zabbix-api-0.5.6/zabbix_api.egg-info/
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)     1223 2023-05-04 06:15:18.000000 zabbix-api-0.5.6/zabbix_api.egg-info/PKG-INFO
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)      213 2023-05-04 06:15:18.000000 zabbix-api-0.5.6/zabbix_api.egg-info/SOURCES.txt
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)        1 2023-05-04 06:15:18.000000 zabbix-api-0.5.6/zabbix_api.egg-info/dependency_links.txt
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)        1 2022-11-08 21:59:23.000000 zabbix-api-0.5.6/zabbix_api.egg-info/not-zip-safe
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)       11 2023-05-04 06:15:18.000000 zabbix-api-0.5.6/zabbix_api.egg-info/top_level.txt
+-rw-r--r--   0 gescheit (2114722489) LD\Domain Users (593637566)    13275 2023-04-28 16:06:24.000000 zabbix-api-0.5.6/zabbix_api.py
```

### Comparing `zabbix-api-0.5.5/PKG-INFO` & `zabbix-api-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zabbix-api
-Version: 0.5.5
+Version: 0.5.6
 Summary: Zabbix API
 Home-page: https://github.com/gescheit/scripts
 Author: Aleksandr Balezin
 Author-email: gescheit12@gmail.com
 License: GNU LGPL 2.1
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `zabbix-api-0.5.5/README.md` & `zabbix-api-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `zabbix-api-0.5.5/setup.py` & `zabbix-api-0.5.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     return long_description
 
 
 setup(
     name='zabbix-api',
     url='https://github.com/gescheit/scripts',
-    version='0.5.5',
+    version='0.5.6',
     license='GNU LGPL 2.1',
     author='Aleksandr Balezin',
     author_email='gescheit12@gmail.com',
     description='Zabbix API',
     long_description=read_descr('README.md'),
     py_modules=['zabbix_api'],
     include_package_data=True,
```

### Comparing `zabbix-api-0.5.5/zabbix_api.egg-info/PKG-INFO` & `zabbix-api-0.5.6/zabbix_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zabbix-api
-Version: 0.5.5
+Version: 0.5.6
 Summary: Zabbix API
 Home-page: https://github.com/gescheit/scripts
 Author: Aleksandr Balezin
 Author-email: gescheit12@gmail.com
 License: GNU LGPL 2.1
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `zabbix-api-0.5.5/zabbix_api.py` & `zabbix-api-0.5.6/zabbix_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,32 @@
         self.logger.log(logging.DEBUG,
                 "Going to do_request for %s with opts %s"
                 % (repr(fn), repr(opts)))
         return self.do_request(self.json_obj(method, opts))['result']
     return wrapper
 
 
+def version_compare(v1, v2):
+    """
+    The result is 0 if v1 == v2, -1 if v1 < v2, and +1 if v1 > v2
+    """
+    for v1_part, v2_part in zip(v1.split("."), v2.split(".")):
+        if v1_part.isdecimal() and v2_part.isdecimal():
+            if int(v1_part) > int(v2_part):
+                return 1
+            elif int(v1_part) < int(v2_part):
+                return -1
+        else:
+            if v1 > v2:
+                return 1
+            elif v1 < v2:
+                return -1
+    return 0
+
+
 class ZabbixAPIException(Exception):
 
     """ generic zabbix api exception
     code list:
          -32602 - Invalid params (eg already exists)
          -32500 - no permissions
     """
@@ -209,15 +227,19 @@
         else:
             raise ZabbixAPIException("No authentication information available.")
 
         # don't print the raw password.
         hashed_pw_string = "md5(" + hashlib.md5(l_password.encode('utf-8')).hexdigest() + ")"
         self.debug(logging.DEBUG, "Trying to login with %s:%s" %
                 (repr(l_user), repr(hashed_pw_string)))
-        obj = self.json_obj('user.login', {'user': l_user, 'password': l_password}, auth=False)
+        if version_compare(self.api_version(), '5.4') >= 0:
+            login_arg = {'username': l_user, 'password': l_password}
+        else:
+            login_arg = {'user': l_user, 'password': l_password}
+        obj = self.json_obj('user.login', login_arg, auth=False)
         result = self.do_request(obj)
         self.auth = result['result']
 
     def logout(self):
         if self.__tokenauth__:
             # Do nothing for logout for API tokens.
             self.debug(logging.DEBUG, "Clearing auth information due to use of API Token")
```

