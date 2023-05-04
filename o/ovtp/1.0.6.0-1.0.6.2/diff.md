# Comparing `tmp/ovtp-1.0.6.0.tar.gz` & `tmp/ovtp-1.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovtp-1.0.6.0.tar", last modified: Thu May  4 02:52:36 2023, max compression
+gzip compressed data, was "ovtp-1.0.6.2.tar", last modified: Thu May  4 03:58:39 2023, max compression
```

## Comparing `ovtp-1.0.6.0.tar` & `ovtp-1.0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.900542 ovtp-1.0.6.0/
--rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/LICENSE.txt
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 02:52:36.900753 ovtp-1.0.6.0/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/README.md
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.892316 ovtp-1.0.6.0/ovtp/
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.6.0/ovtp/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.6.0/ovtp/__main__.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.895606 ovtp-1.0.6.0/ovtp/client/
--rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/client/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/client/config.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.6.0/ovtp/client/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    18883 2023-05-04 02:51:31.000000 ovtp-1.0.6.0/ovtp/client/ovtp_client.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.899414 ovtp-1.0.6.0/ovtp/server/
--rw-r--r--   0 jok4r      (501) staff       (20)      222 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/server/add_auth_keys.py
--rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.6.0/ovtp/server/config.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.900314 ovtp-1.0.6.0/ovtp/server/func/
--rw-r--r--   0 jok4r      (501) staff       (20)       32 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/func/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1586 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/func/check_key.py
--rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/server/keys_conv.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/ovtp/server/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    22371 2023-05-04 02:51:31.000000 ovtp-1.0.6.0/ovtp/server/ovtp_server.py
--rw-r--r--   0 jok4r      (501) staff       (20)      216 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/saved_key.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.893773 ovtp-1.0.6.0/ovtp.egg-info/
--rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.6.0/ovtp.egg-info/.gitignore
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)      562 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/SOURCES.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/dependency_links.txt
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/requires.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        5 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/top_level.txt
--rw-r--r--   0 jok4r      (501) staff       (20)      411 2023-05-04 02:52:36.901226 ovtp-1.0.6.0/setup.cfg
--rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.6.0/setup.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.500763 ovtp-1.0.6.2/
+-rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.6.2/LICENSE.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 03:58:39.500987 ovtp-1.0.6.2/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.6.2/README.md
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.494869 ovtp-1.0.6.2/ovtp/
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.6.2/ovtp/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.6.2/ovtp/__main__.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.497750 ovtp-1.0.6.2/ovtp/client/
+-rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.6.2/ovtp/client/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.6.2/ovtp/client/config.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.6.2/ovtp/client/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    18883 2023-05-04 02:51:31.000000 ovtp-1.0.6.2/ovtp/client/ovtp_client.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.499846 ovtp-1.0.6.2/ovtp/server/
+-rw-r--r--   0 jok4r      (501) staff       (20)      222 2023-05-02 17:58:06.000000 ovtp-1.0.6.2/ovtp/server/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.6.2/ovtp/server/add_auth_keys.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.6.2/ovtp/server/config.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.500584 ovtp-1.0.6.2/ovtp/server/func/
+-rw-r--r--   0 jok4r      (501) staff       (20)       32 2023-05-02 17:58:06.000000 ovtp-1.0.6.2/ovtp/server/func/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1586 2023-05-02 17:58:06.000000 ovtp-1.0.6.2/ovtp/server/func/check_key.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.6.2/ovtp/server/keys_conv.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.6.2/ovtp/server/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    22600 2023-05-04 03:58:06.000000 ovtp-1.0.6.2/ovtp/server/ovtp_server.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      216 2023-05-02 17:58:06.000000 ovtp-1.0.6.2/ovtp/server/saved_key.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:58:39.496555 ovtp-1.0.6.2/ovtp.egg-info/
+-rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.6.2/ovtp.egg-info/.gitignore
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 03:58:39.000000 ovtp-1.0.6.2/ovtp.egg-info/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)      562 2023-05-04 03:58:39.000000 ovtp-1.0.6.2/ovtp.egg-info/SOURCES.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-04 03:58:39.000000 ovtp-1.0.6.2/ovtp.egg-info/dependency_links.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2023-05-04 03:58:39.000000 ovtp-1.0.6.2/ovtp.egg-info/requires.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        5 2023-05-04 03:58:39.000000 ovtp-1.0.6.2/ovtp.egg-info/top_level.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)      411 2023-05-04 03:58:39.501246 ovtp-1.0.6.2/setup.cfg
+-rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.6.2/setup.py
```

### Comparing `ovtp-1.0.6.0/LICENSE.txt` & `ovtp-1.0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/PKG-INFO` & `ovtp-1.0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.6.0
+Version: 1.0.6.2
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ovtp-1.0.6.0/README.md` & `ovtp-1.0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/client/main.py` & `ovtp-1.0.6.2/ovtp/client/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/client/ovtp_client.py` & `ovtp-1.0.6.2/ovtp/client/ovtp_client.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/server/add_auth_keys.py` & `ovtp-1.0.6.2/ovtp/server/add_auth_keys.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/server/config.py` & `ovtp-1.0.6.2/ovtp/server/config.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/server/func/check_key.py` & `ovtp-1.0.6.2/ovtp/server/func/check_key.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/server/main.py` & `ovtp-1.0.6.2/ovtp/server/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.6.0/ovtp/server/ovtp_server.py` & `ovtp-1.0.6.2/ovtp/server/ovtp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import rsa
 import pathlib
 import ovcrypt
 import asyncio
 import ov_aes_cipher
 import oe_common
 from datetime import datetime, timedelta
-from pathlib import Path
 from ovtp.server import cfg, SavedKey, func
 
 
 class OvtpServer:
     class Handler:
         def __init__(self, server, reader, writer):
             self.server = server
@@ -113,18 +112,20 @@
                     self.aes = ov_aes_cipher.AESCipher(
                         hash_key=rsa.decrypt(header_key, self.cr.private_key),
                         iv=rsa.decrypt(header_iv, self.cr.private_key)
                     )
                 else:
                     self.aes = ov_aes_cipher.AESCipher('pass')
 
-                if data_type == b'file' and os.path.isfile(filename):
-                    os.remove(filename)
-                elif data_type == b'link' and os.path.isfile(filename):
-                    os.remove(filename)
+                if data_type == b'file' and os.path.exists(filename):
+                    print(f'File exists, deleting: "{filename}"')
+                    oe_common.rm(filename)
+                elif data_type == b'link' and os.path.exists(filename):
+                    print(f'Link exists, deleting: "{filename}"')
+                    oe_common.rm(filename)
 
                 if address in self.server.saved_keys:
                     ov_sign = ovcrypt.OvSign(self.server.saved_keys[address].key)
                 part_data = b''
                 msg_pad = b''
                 dc = oe_common.DinConsole()
                 sc = oe_common.SpeedChecker('bits / second', 4096)
@@ -353,14 +354,16 @@
                     send_data = json.dumps({'status': 'OK', 'description': 'Temp key added'}).encode()
                     await self.write_with_prefix(self.aes.encrypt(send_data))
                     print("Temp key added")
                 elif data_type == b'file':
                     print(f'Received "{filename}"')
                     if not os.path.isfile(filename):
                         print(f'File not exist, creating: "{filename}"')
+                        oe_common.check_create_dir(filename)
+                        pathlib.Path(filename).touch()
                 elif data_type == b'link':
                     data = b''.join(data_parts)
                     del data_parts
                     print(f'Received link: "{filename}" to "{data.decode()}"')
                     oe_common.check_create_dir(filename)
                     os.symlink(data.decode(), filename)
                     ov_sign.update_hash(data)
```

### Comparing `ovtp-1.0.6.0/ovtp.egg-info/PKG-INFO` & `ovtp-1.0.6.2/ovtp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.6.0
+Version: 1.0.6.2
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ovtp-1.0.6.0/ovtp.egg-info/SOURCES.txt` & `ovtp-1.0.6.2/ovtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

