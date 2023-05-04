# Comparing `tmp/hexicapi-1.0.732.tar.gz` & `tmp/hexicapi-1.0.733.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexicapi-1.0.732.tar", last modified: Tue May  2 21:46:28 2023, max compression
+gzip compressed data, was "hexicapi-1.0.733.tar", last modified: Thu May  4 14:56:15 2023, max compression
```

## Comparing `hexicapi-1.0.732.tar` & `hexicapi-1.0.733.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.079982 hexicapi-1.0.732/
--rw-rw-rw-   0        0        0      360 2023-05-02 21:46:28.070116 hexicapi-1.0.732/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.031237 hexicapi-1.0.732/hexicapi/
--rw-rw-rw-   0        0        0      133 2022-02-20 04:22:49.000000 hexicapi-1.0.732/hexicapi/__init__.py
--rw-rw-rw-   0        0        0    13098 2023-05-02 21:22:58.000000 hexicapi-1.0.732/hexicapi/client.py
--rw-rw-rw-   0        0        0     1815 2023-05-02 21:43:10.000000 hexicapi-1.0.732/hexicapi/connectors.py
--rw-rw-rw-   0        0        0      607 2022-11-12 19:37:47.000000 hexicapi-1.0.732/hexicapi/encryption.py
--rw-rw-rw-   0        0        0     4170 2022-11-01 11:41:18.000000 hexicapi-1.0.732/hexicapi/redlogger.py
--rw-rw-rw-   0        0        0     8305 2022-11-22 17:34:54.000000 hexicapi-1.0.732/hexicapi/registrator.py
--rw-rw-rw-   0        0        0      398 2022-07-22 07:54:05.000000 hexicapi-1.0.732/hexicapi/save.py
--rw-rw-rw-   0        0        0    24313 2023-05-02 20:16:09.000000 hexicapi-1.0.732/hexicapi/server.py
--rw-rw-rw-   0        0        0     4409 2023-05-02 21:15:42.000000 hexicapi-1.0.732/hexicapi/socketMessage.py
--rw-rw-rw-   0        0        0      145 2023-05-02 20:10:51.000000 hexicapi-1.0.732/hexicapi/verinfo.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:46:28.065615 hexicapi-1.0.732/hexicapi.egg-info/
--rw-rw-rw-   0        0        0      360 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 21:46:27.000000 hexicapi-1.0.732/hexicapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 21:46:28.081009 hexicapi-1.0.732/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-02 20:24:09.000000 hexicapi-1.0.732/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:56:15.918740 hexicapi-1.0.733/
+-rw-rw-rw-   0        0        0      360 2023-05-04 14:56:15.906733 hexicapi-1.0.733/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 14:56:15.874740 hexicapi-1.0.733/hexicapi/
+-rw-rw-rw-   0        0        0      133 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/__init__.py
+-rw-rw-rw-   0        0        0    13324 2023-05-03 13:38:33.000000 hexicapi-1.0.733/hexicapi/client.py
+-rw-rw-rw-   0        0        0     1982 2023-05-04 14:31:10.000000 hexicapi-1.0.733/hexicapi/connectors.py
+-rw-rw-rw-   0        0        0      607 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/encryption.py
+-rw-rw-rw-   0        0        0     4170 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/redlogger.py
+-rw-rw-rw-   0        0        0     8305 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/registrator.py
+-rw-rw-rw-   0        0        0      398 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/save.py
+-rw-rw-rw-   0        0        0    24313 2023-05-03 11:13:44.000000 hexicapi-1.0.733/hexicapi/server.py
+-rw-rw-rw-   0        0        0     4437 2023-05-03 14:09:40.000000 hexicapi-1.0.733/hexicapi/socketMessage.py
+-rw-rw-rw-   0        0        0      145 2023-05-04 14:00:32.000000 hexicapi-1.0.733/hexicapi/verinfo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:56:15.902738 hexicapi-1.0.733/hexicapi.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-05-04 14:56:15.000000 hexicapi-1.0.733/hexicapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-04 14:56:15.000000 hexicapi-1.0.733/hexicapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:56:15.000000 hexicapi-1.0.733/hexicapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-04 14:56:15.000000 hexicapi-1.0.733/hexicapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 14:56:15.000000 hexicapi-1.0.733/hexicapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:56:15.919736 hexicapi-1.0.733/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-03 13:33:48.000000 hexicapi-1.0.733/setup.py
```

### Comparing `hexicapi-1.0.732/hexicapi/client.py` & `hexicapi-1.0.733/hexicapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,16 +258,21 @@
         return None
 
     enc_public = enc_public.encode('utf-8')
     enc_public = serialization.load_pem_public_key(
         enc_public
     )
     enc_private, public_key = generate_keys()
-    send_all(CLI(id, s), public_key, skip=True)
-    recv_all(CLI(id, s), enc=enc_private)
+    try:
+        send_all(CLI(id, s), public_key, skip=True)
+        recv_all(CLI(id, s), enc=enc_private)
+    except UnicodeDecodeError:
+        s.close()
+        if not silent: calf('connection_warning', "Encryption handshake failed.")
+        return run(app, username, password, autoauth, silent, connector)
     if not silent: calf('handshake', "Encryption handshake.")
 
     cli = Client(*s.getsockname(), s, id, enc_private, enc_public, username, app)
 
     if autoauth:
         if not silent: calf('authenticating',"Autoauth was enabled.")
         cli.auth(password=password, silent=silent)
```

### Comparing `hexicapi-1.0.732/hexicapi/connectors.py` & `hexicapi-1.0.733/hexicapi/connectors.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,35 +27,38 @@
 
     def connect(self, address: str):
         split = address.split(':')
         if len(split) != 2: raise AddressException("Address is missing port entirely")
         if not split[-1]: raise AddressException("Address is missing port after colon")
         if not split[0]: raise AddressException("Address is missing ip before colon")
         self.sockname = (split[0], int(split[1]))
-        print(self.sockname)
         try:
             self.s.connect(self.sockname)
         except ValueError:
             AddressException("Address port isn't a valid value")
 
-    def send(self, data: bytes | bytearray): return self.s.send(data)
+    def send(self, data: bytes): return self.s.send(data)
 
     def recv(self, buffer_size: int): return self.s.recv(buffer_size)
 
     def close(self): return self.s.close()
 
 class WebsocketConnector(Connector):
-
+    buffer = []
     def __init__(self):
         self.s = websocket.WebSocket()
 
     def connect(self, address: str):
         self.sockname = address.split(':')
         if len(self.sockname) < 2: self.sockname.append()
         self.sockname = tuple(self.sockname)
         self.s.connect(address)
 
-    def send(self, data: bytes | bytearray): return self.s.send_binary(data)
+    def send(self, data: bytes): return self.s.send_binary(data)
 
-    def recv(self, buffer_size: int): return self.s.recv()
+    def recv(self, buffer_size: int):
+        if len(self.buffer) < 1: self.buffer.extend(self.s.recv())
+        items = self.buffer[0:min(buffer_size, len(self.buffer))]
+        del self.buffer[0:min(buffer_size, len(self.buffer))]
+        return bytes(items)
 
     def close(self): return self.s.close()
```

### Comparing `hexicapi-1.0.732/hexicapi/encryption.py` & `hexicapi-1.0.733/hexicapi/encryption.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.732/hexicapi/redlogger.py` & `hexicapi-1.0.733/hexicapi/redlogger.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.732/hexicapi/registrator.py` & `hexicapi-1.0.733/hexicapi/registrator.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.732/hexicapi/server.py` & `hexicapi-1.0.733/hexicapi/server.py`

 * *Files identical despite different names*

### Comparing `hexicapi-1.0.732/hexicapi/socketMessage.py` & `hexicapi-1.0.733/hexicapi/socketMessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         #         label=None
         # ))
         if sock_msg_debug: print(f"RECV data size was wrong: >{data}<")
         return data.encode('utf-8')
 
     data = b''
     while len(data) < data_length:
-        data += the_socket.recv(packet_size)
+        data += the_socket.recv(min(packet_size, data_length-len(data)))
     rm_record(client_id)
     if menc and not skip:
         if sock_msg_debug: print(f"RECV decrypting the following data: >{data}<")
         try:
             data = menc.decrypt(data,
             padding.OAEP(
                 mgf=padding.MGF1(algorithm=hashes.SHA256()),
```

### Comparing `hexicapi-1.0.732/setup.py` & `hexicapi-1.0.733/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.732'
+VERSION = '1.0.733'
 short = 'Tool for making quick servers.'
 long = '''API for making servers and clients to connect to those servers. 
 
 Includes end to end encryption!
 
 github: https://github.com/JustRedTTG/hexicapi'''
```

