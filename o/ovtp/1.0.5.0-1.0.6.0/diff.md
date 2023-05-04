# Comparing `tmp/ovtp-1.0.5.0.tar.gz` & `tmp/ovtp-1.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovtp-1.0.5.0.tar", last modified: Tue May  2 18:07:21 2023, max compression
+gzip compressed data, was "ovtp-1.0.6.0.tar", last modified: Thu May  4 02:52:36 2023, max compression
```

## Comparing `ovtp-1.0.5.0.tar` & `ovtp-1.0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826962 ovtp-1.0.5.0/
--rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/LICENSE.txt
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-02 18:07:21.827014 ovtp-1.0.5.0/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/README.md
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.823017 ovtp-1.0.5.0/ovtp/
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.5.0/ovtp/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.5.0/ovtp/__main__.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.825005 ovtp-1.0.5.0/ovtp/client/
--rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/client/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/client/config.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.5.0/ovtp/client/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    19825 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/client/ovtp_client.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826519 ovtp-1.0.5.0/ovtp/server/
--rw-r--r--   0 jok4r      (501) staff       (20)      222 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/server/add_auth_keys.py
--rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.5.0/ovtp/server/config.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.826815 ovtp-1.0.5.0/ovtp/server/func/
--rw-r--r--   0 jok4r      (501) staff       (20)       32 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/func/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1586 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/func/check_key.py
--rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.5.0/ovtp/server/keys_conv.py
--rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.5.0/ovtp/server/main.py
--rwxr-xr-x   0 jok4r      (501) staff       (20)    21649 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/ovtp_server.py
--rw-r--r--   0 jok4r      (501) staff       (20)      216 2023-05-02 17:58:06.000000 ovtp-1.0.5.0/ovtp/server/saved_key.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-02 18:07:21.824111 ovtp-1.0.5.0/ovtp.egg-info/
--rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.5.0/ovtp.egg-info/.gitignore
--rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)      562 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/SOURCES.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/dependency_links.txt
--rw-r--r--   0 jok4r      (501) staff       (20)       42 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/requires.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        5 2023-05-02 18:07:21.000000 ovtp-1.0.5.0/ovtp.egg-info/top_level.txt
--rw-r--r--   0 jok4r      (501) staff       (20)      411 2023-05-02 18:07:21.827233 ovtp-1.0.5.0/setup.cfg
--rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.5.0/setup.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.900542 ovtp-1.0.6.0/
+-rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/LICENSE.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 02:52:36.900753 ovtp-1.0.6.0/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)     5420 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/README.md
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.892316 ovtp-1.0.6.0/ovtp/
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2022-08-01 18:29:36.000000 ovtp-1.0.6.0/ovtp/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      351 2022-08-01 18:29:19.000000 ovtp-1.0.6.0/ovtp/__main__.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.895606 ovtp-1.0.6.0/ovtp/client/
+-rw-r--r--   0 jok4r      (501) staff       (20)       89 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/client/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      173 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/client/config.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1019 2022-08-01 18:29:05.000000 ovtp-1.0.6.0/ovtp/client/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    18883 2023-05-04 02:51:31.000000 ovtp-1.0.6.0/ovtp/client/ovtp_client.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.899414 ovtp-1.0.6.0/ovtp/server/
+-rw-r--r--   0 jok4r      (501) staff       (20)      222 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1116 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/server/add_auth_keys.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      846 2022-11-20 20:43:32.000000 ovtp-1.0.6.0/ovtp/server/config.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.900314 ovtp-1.0.6.0/ovtp/server/func/
+-rw-r--r--   0 jok4r      (501) staff       (20)       32 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/func/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1586 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/func/check_key.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      386 2022-08-01 22:18:27.000000 ovtp-1.0.6.0/ovtp/server/keys_conv.py
+-rw-r--r--   0 jok4r      (501) staff       (20)     1226 2022-10-24 22:47:16.000000 ovtp-1.0.6.0/ovtp/server/main.py
+-rwxr-xr-x   0 jok4r      (501) staff       (20)    22371 2023-05-04 02:51:31.000000 ovtp-1.0.6.0/ovtp/server/ovtp_server.py
+-rw-r--r--   0 jok4r      (501) staff       (20)      216 2023-05-02 17:58:06.000000 ovtp-1.0.6.0/ovtp/server/saved_key.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 02:52:36.893773 ovtp-1.0.6.0/ovtp.egg-info/
+-rw-r--r--   0 jok4r      (501) staff       (20)        2 2022-08-02 02:52:00.000000 ovtp-1.0.6.0/ovtp.egg-info/.gitignore
+-rw-r--r--   0 jok4r      (501) staff       (20)     6735 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)      562 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/SOURCES.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/dependency_links.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)       42 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/requires.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        5 2023-05-04 02:52:36.000000 ovtp-1.0.6.0/ovtp.egg-info/top_level.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)      411 2023-05-04 02:52:36.901226 ovtp-1.0.6.0/setup.cfg
+-rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-07-31 23:53:24.000000 ovtp-1.0.6.0/setup.py
```

### Comparing `ovtp-1.0.5.0/LICENSE.txt` & `ovtp-1.0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/PKG-INFO` & `ovtp-1.0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.5.0
+Version: 1.0.6.0
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ovtp-1.0.5.0/README.md` & `ovtp-1.0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/client/main.py` & `ovtp-1.0.6.0/ovtp/client/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/client/ovtp_client.py` & `ovtp-1.0.6.0/ovtp/client/ovtp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         ]
         return b''.join(ba)
 
     @staticmethod
     def _validate_input(data_type, filename):
         error = 'Unknown error'
         if data_type == 'file':
-            if os.path.isfile(filename):
+            if os.path.isfile(filename) or os.path.islink(filename):
                 return True
             else:
                 error = f"File {filename} does not exists!"
         raise RuntimeError(error)
 
     async def read_with_prefix(self, timeout=5, retries=0):
         prefix_timeout = 30
@@ -260,103 +260,81 @@
                             print(f'File not exists on server: {path_from}')
                         os.remove(path_to)
                         return False
                 dec_part = self.aes.unpad(self.aes.decrypt_part(part))
                 ov_sign.update_hash(dec_part)
                 f.write(dec_part)
 
-    async def send_file(self, path_from, path_to=None):
+    async def send_file(self, path_from, path_to=None, follow_symlinks=False):
         if not path_to:
             path_to = path_from
         await self.check_connection()
         self._validate_input('file', path_from)
         self.aes = ov_aes_cipher.AESCipher(key=oe_common.get_rnd_string(60))
-        with open(path_from, 'rb') as f:
-            file_size = os.path.getsize(path_from)
-            '''if file_size > 1024*1024*500:  # 500 Mb
-                signed = False
-                sign = None
-            else:
-                signed = True
-                sign = rsa.sign(f.read(), self.cr.private_key, 'SHA-1')
-            f.seek(0)'''
-            signed = True
-            #self.reader, self.writer = await asyncio.open_connection(
-                #self.server_address,
-                #self.server_port
-            #)
-            self.writer.write(self._get_ov_header(
-                'file',
-                filename=path_to,
-                key=rsa.encrypt(self.aes.key, self.server_public_key),
-                iv=rsa.encrypt(self.aes.iv, self.server_public_key),
-                signed=signed,
-                # sign=sign,
-                size=file_size
-            ))
-            # chunk_num = 0
-
-            dc = oe_common.DinConsole()
-            sc = oe_common.SpeedChecker('bits / second', 4096)
-            ov_sign = ovcrypt.OvSign(self.cr.private_key)
-            prefix_pad = b'\x00' * 3
-            tx_bytes = 0
-            file_size_str = oe_common.convert_size(file_size)
-            for chunk in iter(lambda: f.read(4096), b''):
-                # chunk_num += 1
-                ov_sign.update_hash(chunk)
-                if f.tell() >= file_size:
-                    # print(f'\npadding chunk {chunk_num}')
-                    chunk = self.aes.pad(chunk)
-                    # prefix_pad = b'pad'
-                    prefix_pad = True
-                else:
-                    # prefix_pad = b'\x00' * len(prefix_pad)
-                    prefix_pad = False
-                # self.writer.write(b'%d%b\n' % (len(chunk), prefix_pad))
-                # self.writer.write(aes.encrypt_part(chunk))
-                await self.write_with_prefix(self.aes.encrypt_part(chunk), prefix=prefix_pad)
-                # await self.writer.drain()
-                '''if chunk_num % 1000 == 0:
-                    c_time_new = time.perf_counter()
-                    c_diff = c_time_new - c_time
-                    c_time = c_time_new
-                    network_speed = 4096 * 1000 / c_diff * 8'''
-                tx_bytes = tx_bytes + len(chunk)
-                if self.debug or self.verbose:
-                    dc.update('  Sent %s / %s, %s%%, speed: %s' % (
-                        oe_common.convert_size(tx_bytes),
-                        file_size_str,
-                        round(tx_bytes / file_size * 100),
-                        sc.get_speed()
-                    ))
-            if self.debug or self.verbose:
-                dc.stay()
+        file_size = os.path.getsize(path_from)
+        signed = True
+        self.writer.write(self._get_ov_header(
+            'link' if not follow_symlinks and os.path.islink(path_from) else 'file',
+            filename=path_to,
+            key=rsa.encrypt(self.aes.key, self.server_public_key),
+            iv=rsa.encrypt(self.aes.iv, self.server_public_key),
+            signed=signed,
+            size=file_size
+        ))
+
+        dc = oe_common.DinConsole()
+        sc = oe_common.SpeedChecker('bits / second', 4096)
+        ov_sign = ovcrypt.OvSign(self.cr.private_key)
+        prefix_pad = b'\x00' * 3
+        tx_bytes = 0
+        file_size_str = oe_common.convert_size(file_size)
+
+        if os.path.islink(path_from):
+            link_path = os.readlink(path_from).encode()
+            await self.write_with_prefix(self.aes.encrypt(link_path), prefix=False)
+            ov_sign.update_hash(link_path)
+        else:
+            with open(path_from, 'rb') as f:
+                for chunk in iter(lambda: f.read(4096), b''):
+                    ov_sign.update_hash(chunk)
+                    if f.tell() >= file_size:
+                        chunk = self.aes.pad(chunk)
+                        prefix_pad = True
+                    else:
+                        prefix_pad = False
+                    await self.write_with_prefix(self.aes.encrypt_part(chunk), prefix=prefix_pad)
+                    tx_bytes = tx_bytes + len(chunk)
+                    if self.debug or self.verbose:
+                        dc.update('  Sent %s / %s, %s%%, speed: %s' % (
+                            oe_common.convert_size(tx_bytes),
+                            file_size_str,
+                            round(tx_bytes / file_size * 100),
+                            sc.get_speed()
+                        ))
+        if self.debug or self.verbose:
+            dc.stay()
+        await self.writer.drain()
+        if self.debug:
+            print("Data sent")
+        if signed:
+            sign = ov_sign.get_sign()
+            prefix = b'\x00' * 3
+            self.writer.write(b'%d%b\n' % (len(sign), prefix))
+            sign_message = b'ovsign'
+            padded_sign_message = sign_message + b'\x00' * (256 - len(sign_message))
+            self.writer.write(padded_sign_message)
+            self.writer.write(sign)
             await self.writer.drain()
             if self.debug:
-                print("Data sent")
-            if signed:
-                sign = ov_sign.get_sign()
-                prefix = b'\x00' * 3
-                self.writer.write(b'%d%b\n' % (len(sign), prefix))
-                sign_message = b'ovsign'
-                padded_sign_message = sign_message + b'\x00' * (256 - len(sign_message))
-                self.writer.write(padded_sign_message)
-                self.writer.write(sign)
-                await self.writer.drain()
-                if self.debug:
-                    print("Sign sent")
-            # self.writer.write_eof()
-
-            rcv_data = oe_common.fix_block_encoding_errors(self.aes.decrypt((await self.read_with_prefix())[0]))
-            if self.debug or self.verbose:
-                print(f'Answer: {rcv_data}')
-            # self.writer.close()
-            # await self.writer.wait_closed()
-            return rcv_data
+                print("Sign sent")
+
+        rcv_data = oe_common.fix_block_encoding_errors(self.aes.decrypt((await self.read_with_prefix())[0]))
+        if self.debug or self.verbose:
+            print(f'Answer: {rcv_data}')
+        return rcv_data
 
     def send_message_sync(self, message, timeout=2, retries=0):
         return self.loop.run_until_complete(
             self.send_message(message, timeout, retries)
         )
 
     async def send_add_temp_auth_key(self, key: bytes, remote_address: str):
```

### Comparing `ovtp-1.0.5.0/ovtp/server/add_auth_keys.py` & `ovtp-1.0.6.0/ovtp/server/add_auth_keys.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/server/config.py` & `ovtp-1.0.6.0/ovtp/server/config.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/server/func/check_key.py` & `ovtp-1.0.6.0/ovtp/server/func/check_key.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/server/main.py` & `ovtp-1.0.6.0/ovtp/server/main.py`

 * *Files identical despite different names*

### Comparing `ovtp-1.0.5.0/ovtp/server/ovtp_server.py` & `ovtp-1.0.6.0/ovtp/server/ovtp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import rsa
 import pathlib
 import ovcrypt
 import asyncio
 import ov_aes_cipher
 import oe_common
 from datetime import datetime, timedelta
+from pathlib import Path
 from ovtp.server import cfg, SavedKey, func
 
 
 class OvtpServer:
     class Handler:
         def __init__(self, server, reader, writer):
             self.server = server
@@ -114,14 +115,16 @@
                         iv=rsa.decrypt(header_iv, self.cr.private_key)
                     )
                 else:
                     self.aes = ov_aes_cipher.AESCipher('pass')
 
                 if data_type == b'file' and os.path.isfile(filename):
                     os.remove(filename)
+                elif data_type == b'link' and os.path.isfile(filename):
+                    os.remove(filename)
 
                 if address in self.server.saved_keys:
                     ov_sign = ovcrypt.OvSign(self.server.saved_keys[address].key)
                 part_data = b''
                 msg_pad = b''
                 dc = oe_common.DinConsole()
                 sc = oe_common.SpeedChecker('bits / second', 4096)
@@ -346,14 +349,25 @@
                     self.server.temp_keys[remote_address] = SavedKey(
                         rsa.PublicKey.load_pkcs1(temp_key),
                         datetime.now() + timedelta(minutes=5)
                     )
                     send_data = json.dumps({'status': 'OK', 'description': 'Temp key added'}).encode()
                     await self.write_with_prefix(self.aes.encrypt(send_data))
                     print("Temp key added")
+                elif data_type == b'file':
+                    print(f'Received "{filename}"')
+                    if not os.path.isfile(filename):
+                        print(f'File not exist, creating: "{filename}"')
+                elif data_type == b'link':
+                    data = b''.join(data_parts)
+                    del data_parts
+                    print(f'Received link: "{filename}" to "{data.decode()}"')
+                    oe_common.check_create_dir(filename)
+                    os.symlink(data.decode(), filename)
+                    ov_sign.update_hash(data)
                 elif data_type == b'auth_resp':
                     data = b''.join(data_parts)
                     del data_parts
                     if self.server.debug:
                         print(f'auth resp is: {data}')
                     if data == self.server.saved_keys[address].verification_string:
                         status, response = func.check_key(self, self.server.saved_keys[address], address)
```

### Comparing `ovtp-1.0.5.0/ovtp.egg-info/PKG-INFO` & `ovtp-1.0.6.0/ovtp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovtp
-Version: 1.0.5.0
+Version: 1.0.6.0
 Summary: Over Transfer Protocol
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ovtp-1.0.5.0/ovtp.egg-info/SOURCES.txt` & `ovtp-1.0.6.0/ovtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

