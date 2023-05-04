# Comparing `tmp/Sandra-0.0.16.tar.gz` & `tmp/Sandra-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sandra-0.0.16.tar", last modified: Thu Apr 27 19:59:36 2023, max compression
+gzip compressed data, was "Sandra-0.0.17.tar", last modified: Thu May  4 09:54:23 2023, max compression
```

## Comparing `Sandra-0.0.16.tar` & `Sandra-0.0.17.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 19:59:35.988211 Sandra-0.0.16/
--rw-rw-rw-   0        0        0     1080 2023-04-27 16:41:21.000000 Sandra-0.0.16/LICENSE
--rw-rw-rw-   0        0        0     5363 2023-04-27 19:59:35.984177 Sandra-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-04-27 19:12:42.000000 Sandra-0.0.16/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 19:59:35.962170 Sandra-0.0.16/Sandra/
--rw-rw-rw-   0        0        0      133 2023-04-27 19:59:29.000000 Sandra-0.0.16/Sandra/__init__.py
--rw-rw-rw-   0        0        0      765 2023-04-27 18:01:39.000000 Sandra-0.0.16/Sandra/helpers.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 19:43:53.000000 Sandra-0.0.16/Sandra/performance.py
--rw-rw-rw-   0        0        0     4909 2023-04-27 19:49:42.000000 Sandra-0.0.16/Sandra/sandra.py
--rw-rw-rw-   0        0        0     1332 2023-04-26 02:08:05.000000 Sandra-0.0.16/Sandra/troy.py
-drwxrwxrwx   0        0        0        0 2023-04-27 19:59:35.983184 Sandra-0.0.16/Sandra.egg-info/
--rw-rw-rw-   0        0        0     5363 2023-04-27 19:59:35.000000 Sandra-0.0.16/Sandra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-04-27 19:59:35.000000 Sandra-0.0.16/Sandra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 19:59:35.000000 Sandra-0.0.16/Sandra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-27 19:59:35.000000 Sandra-0.0.16/Sandra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 19:59:35.000000 Sandra-0.0.16/Sandra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 19:59:35.988211 Sandra-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-04-27 19:59:32.000000 Sandra-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:23.014542 Sandra-0.0.17/
+-rw-rw-rw-   0        0        0     1080 2023-04-27 16:41:21.000000 Sandra-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0     4427 2023-05-04 09:54:23.014542 Sandra-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     3684 2023-05-04 09:53:50.000000 Sandra-0.0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:22.623147 Sandra-0.0.17/Sandra/
+-rw-rw-rw-   0        0        0      133 2023-05-04 09:27:04.000000 Sandra-0.0.17/Sandra/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-04 08:39:19.000000 Sandra-0.0.17/Sandra/helpers.py
+-rw-rw-rw-   0        0        0     2702 2023-05-04 09:36:56.000000 Sandra-0.0.17/Sandra/performance.py
+-rw-rw-rw-   0        0        0     4954 2023-05-04 08:39:49.000000 Sandra-0.0.17/Sandra/sandra.py
+-rw-rw-rw-   0        0        0     2095 2023-05-04 09:06:12.000000 Sandra-0.0.17/Sandra/troy.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:54:23.013549 Sandra-0.0.17/Sandra.egg-info/
+-rw-rw-rw-   0        0        0     4427 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 09:54:22.000000 Sandra-0.0.17/Sandra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:54:23.015542 Sandra-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-05-04 09:26:57.000000 Sandra-0.0.17/setup.py
```

### Comparing `Sandra-0.0.16/LICENSE` & `Sandra-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `Sandra-0.0.16/PKG-INFO` & `Sandra-0.0.17/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: Sandra
-Version: 0.0.16
+Version: 0.0.17
 Summary: AES Stream Cipher with CFB and OpenPGP Modes
 Home-page: https://github.com/lopgogo/Sandra
 Author: George Assaad
 Author-email: <lopgogo@gmail.com>
+License: MIT
 Keywords: python,encryption,decryption,cipher,cryptography
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -34,19 +35,19 @@
     file_names, # name of files to be written
     file_data, # data to be written, must be the same length as file_names
     path='.' # path to write data to
 )
 ```
 
 ## Examples
-### RSA File Encryption using [PKCS#1 OAEP](https://datatracker.ietf.org/doc/html/rfc8017)
+### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(1024)
+enc_dec_rsa = Sandra.RSA(256)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
@@ -83,24 +84,31 @@
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
+> Padding here is unnecessary as this mode is a stream cipher
 ```python
 import Sandra
 iv   = bytes.fromhex('fffffe00000000000000000000000000')
 key  = bytes.fromhex('00000000000000000000000000000000')
-file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv, segment_size=16)
-ciphertext = enc_dec_pgp.encrypt(file_data[0])
+file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt')
+print(len(file_data[0]))
+file_data_padded = Sandra.pad(file_data, Sandra.AES_BLOCK_SIZE) 
+print(len(file_data_padded[0]))
+enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv)
+ciphertext = enc_dec_pgp.encrypt(file_data_padded[0])
 eiv, ciphertext = ciphertext[:18], ciphertext[18:]
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
+print(len(plaintext))
+plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
+print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
@@ -108,19 +116,8 @@
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
 Sandra.performance_test(file_names, file_data)
 ```
-
-|                    |   taylor_swift_1KB.txt |   taylor_swift_10KB.txt |   taylor_swift_100KB.txt |   taylor_swift_5KB.txt |
-|:-------------------|-----------------------:|------------------------:|-------------------------:|-----------------------:|
-| CFB_enc            |            3.20184e-05 |             0.000228404 |              0.0022509   |            0.000106322 |
-| CFB_dec            |            2.25229e-05 |             0.000222947 |              0.00330419  |            9.85432e-05 |
-| OPENPGP_enc        |            5.70565e-06 |             3.0201e-05  |              0.000280344 |            1.57004e-05 |
-| OPENPGP_dec        |            6.0602e-06  |             3.05637e-05 |              0.000297508 |            1.55763e-05 |
-| OPENPGP_SANDRA_enc |            0.000358904 |             0.00407359  |              0.0492199   |            0.00173748  |
-| OPENPGP_SANDRA_dec |            0.000388411 |             0.00396413  |              0.063188    |            0.00174934  |
-| RSA_TROY_enc       |            0.00453846  |             0.0412725   |              0.463819    |            0.0194584   |
-| RSA_TROY_dec       |            0.0323089   |             0.15982     |              1.38922     |            0.0765507   |
-
+![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
```

### Comparing `Sandra-0.0.16/README.md` & `Sandra-0.0.17/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     file_names, # name of files to be written
     file_data, # data to be written, must be the same length as file_names
     path='.' # path to write data to
 )
 ```
 
 ## Examples
-### RSA File Encryption using [PKCS#1 OAEP](https://datatracker.ietf.org/doc/html/rfc8017)
+### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(1024)
+enc_dec_rsa = Sandra.RSA(256)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
@@ -65,24 +65,31 @@
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
+> Padding here is unnecessary as this mode is a stream cipher
 ```python
 import Sandra
 iv   = bytes.fromhex('fffffe00000000000000000000000000')
 key  = bytes.fromhex('00000000000000000000000000000000')
-file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv, segment_size=16)
-ciphertext = enc_dec_pgp.encrypt(file_data[0])
+file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt')
+print(len(file_data[0]))
+file_data_padded = Sandra.pad(file_data, Sandra.AES_BLOCK_SIZE) 
+print(len(file_data_padded[0]))
+enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv)
+ciphertext = enc_dec_pgp.encrypt(file_data_padded[0])
 eiv, ciphertext = ciphertext[:18], ciphertext[18:]
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
+print(len(plaintext))
+plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
+print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
@@ -90,19 +97,8 @@
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
 Sandra.performance_test(file_names, file_data)
 ```
-
-|                    |   taylor_swift_1KB.txt |   taylor_swift_10KB.txt |   taylor_swift_100KB.txt |   taylor_swift_5KB.txt |
-|:-------------------|-----------------------:|------------------------:|-------------------------:|-----------------------:|
-| CFB_enc            |            3.20184e-05 |             0.000228404 |              0.0022509   |            0.000106322 |
-| CFB_dec            |            2.25229e-05 |             0.000222947 |              0.00330419  |            9.85432e-05 |
-| OPENPGP_enc        |            5.70565e-06 |             3.0201e-05  |              0.000280344 |            1.57004e-05 |
-| OPENPGP_dec        |            6.0602e-06  |             3.05637e-05 |              0.000297508 |            1.55763e-05 |
-| OPENPGP_SANDRA_enc |            0.000358904 |             0.00407359  |              0.0492199   |            0.00173748  |
-| OPENPGP_SANDRA_dec |            0.000388411 |             0.00396413  |              0.063188    |            0.00174934  |
-| RSA_TROY_enc       |            0.00453846  |             0.0412725   |              0.463819    |            0.0194584   |
-| RSA_TROY_dec       |            0.0323089   |             0.15982     |              1.38922     |            0.0765507   |
-
+![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
```

### Comparing `Sandra-0.0.16/Sandra/performance.py` & `Sandra-0.0.17/Sandra/performance.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
     def run_n_times(mode_name, encryptor, decryptor, OPENPGP=0, n=100):
         if mode_name + '_enc' not in stats:
             stats[mode_name + '_enc'] = dict()
             stats[mode_name + '_dec'] = dict()
         for filename, file in files.items():
             ct = encryptor.encrypt(file)
-            if OPENPGP == 1:
+            if OPENPGP == 1: # PyCrypto
                 eiv, ct = ct[:18], ct[18:]
                 decryptor = AES.new(key, AES.MODE_OPENPGP, eiv)
-            elif OPENPGP == 2:
+            elif OPENPGP == 2: # Sandra
                 eiv, ct = ct[:18], ct[18:]
             t = timeit.Timer(
                 lambda: encryptor.encrypt(file)
             )
             stats[mode_name + '_enc'][filename] = t.timeit(n) / n
             t = timeit.Timer(
                 lambda: decryptor.decrypt(ct)
@@ -46,24 +46,30 @@
     # PyCrypto OPENPGP
     encryptor = AES.new(key, AES.MODE_OPENPGP, iv)
     decryptor = None
     run_n_times('OPENPGP',encryptor, decryptor, OPENPGP=1, n=1000)
     if verbose:
         print(">> Finished running OPENPGP 1000 times")
 
+    # Sandra CFB
+    enc_dec_sandra = sandra.AES(key, sandra.MODE_CFB, iv)
+    run_n_times('CFB_SANDRA', enc_dec_sandra, enc_dec_sandra, OPENPGP=0, n=100)
+    if verbose:
+        print(">> Finished running CFB_SANDRA 100 times")
+
     # Sandra OPENPGP
     enc_dec_sandra = sandra.AES(key, sandra.MODE_OPENPGP, iv)
     run_n_times('OPENPGP_SANDRA', enc_dec_sandra, enc_dec_sandra, OPENPGP=2, n=100)
     if verbose:
         print(">> Finished running OPENPGP_SANDRA 100 times")
 
     # Troy RSA (a wrapper around PyCrypto)
-    enc_dec_rsa = troy.RSA(1024)
-    run_n_times('RSA_TROY', enc_dec_rsa, enc_dec_rsa, n=100)
+    enc_dec_rsa = troy.RSA(256)
+    run_n_times('RSA_TROY_256', enc_dec_rsa, enc_dec_rsa, n=100)
     if verbose:
-        print(">> Finished running RSA_TROY 100 times")
+        print(">> Finished running RSA_TROY_256 100 times")
 
-        print("======================== Results ==========================")
+        print("============================================= Results (seconds) ============================================")
         df = pd.DataFrame.from_dict(stats, orient='index')
         print(df.to_string())
         
     return stats
```

### Comparing `Sandra-0.0.16/Sandra/sandra.py` & `Sandra-0.0.17/Sandra/sandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from Crypto.Random import get_random_bytes
 import warnings
 
 
 MODE_CFB = 1
 MODE_OPENPGP_STANDALONE = 2 # Deprecated use MODE_OPENPGP
 MODE_OPENPGP = 3
+AES_BLOCK_SIZE = 16
 
 class AES:
-    def __init__(self, key, mode, iv, segment_size=8):
+    def __init__(self, key, mode, iv, segment_size=128):
         if segment_size %8 != 0:
             raise ValueError(f"Segment Size must be multiples of a byte(octet) for all Modes.")
         if len(key) != aes.block_size:
             raise ValueError(f"Length of Key must be {aes.block_size} bytes for all Modes.")
         if len(iv) != aes.block_size:
             raise ValueError(f"Length of IV must be {aes.block_size} bytes for all Modes.")
         if mode == MODE_OPENPGP_STANDALONE:
@@ -102,36 +103,36 @@
         return plaintext
     
     @staticmethod
     def _encrypt_CFB(plaintext, key, iv, s):
 
         cipher = aes.new(key, aes.MODE_ECB)
         x = iv
-        ciphertext = bytes()
+        ciphertext = bytearray()
         for i in range(len(plaintext) // s):
             m = plaintext[i*s : (i+1)*s]
             out = cipher.encrypt(x)
             c = strxor(m, out[:s])
             ciphertext += c
             x = x[s:] + c
         rem = len(plaintext) % s
         if rem != 0:
             out = cipher.encrypt(x)
             ciphertext += strxor(plaintext[-rem:], out[:rem])
-        return ciphertext
+        return bytes(ciphertext)
     
     @staticmethod
     def _decrypt_CFB(ciphertext, key, iv, s):
         cipher = aes.new(key, aes.MODE_ECB)
         x = iv
-        plaintext = bytes()
+        plaintext = bytearray()
         for i in range(len(ciphertext) // s):
             c = ciphertext[i*s : (i+1)*s]
             out = cipher.encrypt(x)
             m = strxor(c, out[:s])
             plaintext += m
             x = x[s:] + c
         rem = len(ciphertext) % s
         if rem != 0:
             out = cipher.encrypt(x)
             plaintext += strxor(ciphertext[-rem:], out[:rem])
-        return plaintext
+        return bytes(plaintext)
```

### Comparing `Sandra-0.0.16/Sandra.egg-info/PKG-INFO` & `Sandra-0.0.17/Sandra.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: Sandra
-Version: 0.0.16
+Version: 0.0.17
 Summary: AES Stream Cipher with CFB and OpenPGP Modes
 Home-page: https://github.com/lopgogo/Sandra
 Author: George Assaad
 Author-email: <lopgogo@gmail.com>
+License: MIT
 Keywords: python,encryption,decryption,cipher,cryptography
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -34,19 +35,19 @@
     file_names, # name of files to be written
     file_data, # data to be written, must be the same length as file_names
     path='.' # path to write data to
 )
 ```
 
 ## Examples
-### RSA File Encryption using [PKCS#1 OAEP](https://datatracker.ietf.org/doc/html/rfc8017)
+### RSA File Encryption 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_rsa = Sandra.RSA(1024)
+enc_dec_rsa = Sandra.RSA(256)
 ciphertext = enc_dec_rsa.encrypt(file_data[0])
 print(len(ciphertext))
 plaintext = enc_dec_rsa.decrypt(ciphertext)
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
@@ -83,24 +84,31 @@
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
 
 ### AES OpenPGP-CFB Mode File Encryption
 > In This mode, the first 18 bytes of cipher text contain the encrypted IV
+> Padding here is unnecessary as this mode is a stream cipher
 ```python
 import Sandra
 iv   = bytes.fromhex('fffffe00000000000000000000000000')
 key  = bytes.fromhex('00000000000000000000000000000000')
-file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt') 
-enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv, segment_size=16)
-ciphertext = enc_dec_pgp.encrypt(file_data[0])
+file_names, file_data = Sandra.load_data('./taylor_txt/taylor_swift_1KB.txt')
+print(len(file_data[0]))
+file_data_padded = Sandra.pad(file_data, Sandra.AES_BLOCK_SIZE) 
+print(len(file_data_padded[0]))
+enc_dec_pgp = Sandra.AES(key, Sandra.MODE_OPENPGP, iv)
+ciphertext = enc_dec_pgp.encrypt(file_data_padded[0])
 eiv, ciphertext = ciphertext[:18], ciphertext[18:]
 print(len(ciphertext))
 plaintext = enc_dec_pgp.decrypt(ciphertext)
+print(len(plaintext))
+plaintext = Sandra.unpad(plaintext,Sandra.AES_BLOCK_SIZE)
+print(len(plaintext))
 print(plaintext == file_data[0])
 Sandra.write_data(
     file_names, # name of file to be written
     [plaintext], # data to be written, must be same length as file_names
     path='./taylor_txt_ed' # path to write data to
 )
 ```
@@ -108,19 +116,8 @@
 ## Performance
 To obtain a table like this one, run 
 ```python
 import Sandra
 file_names, file_data = Sandra.load_data('path/to/data')
 Sandra.performance_test(file_names, file_data)
 ```
-
-|                    |   taylor_swift_1KB.txt |   taylor_swift_10KB.txt |   taylor_swift_100KB.txt |   taylor_swift_5KB.txt |
-|:-------------------|-----------------------:|------------------------:|-------------------------:|-----------------------:|
-| CFB_enc            |            3.20184e-05 |             0.000228404 |              0.0022509   |            0.000106322 |
-| CFB_dec            |            2.25229e-05 |             0.000222947 |              0.00330419  |            9.85432e-05 |
-| OPENPGP_enc        |            5.70565e-06 |             3.0201e-05  |              0.000280344 |            1.57004e-05 |
-| OPENPGP_dec        |            6.0602e-06  |             3.05637e-05 |              0.000297508 |            1.55763e-05 |
-| OPENPGP_SANDRA_enc |            0.000358904 |             0.00407359  |              0.0492199   |            0.00173748  |
-| OPENPGP_SANDRA_dec |            0.000388411 |             0.00396413  |              0.063188    |            0.00174934  |
-| RSA_TROY_enc       |            0.00453846  |             0.0412725   |              0.463819    |            0.0194584   |
-| RSA_TROY_dec       |            0.0323089   |             0.15982     |              1.38922     |            0.0765507   |
-
+![image](https://user-images.githubusercontent.com/26662104/236169065-8fb0448c-1d7f-4a7c-89c4-7678ca33c57a.png)
```

### Comparing `Sandra-0.0.16/setup.py` & `Sandra-0.0.17/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.16'
+VERSION = '0.0.17'
 DESCRIPTION = 'AES Stream Cipher with CFB and OpenPGP Modes'
 LONG_DESCRIPTION = 'A package that allows you to build encrypt variable sized files using AES as a stream cipher with CFB and OpenPGP modes'
 
 # Setting up
 setup(
     name="Sandra",
     version=VERSION,
+    license= 'MIT',
     author="George Assaad",
     author_email="<lopgogo@gmail.com>",
     url='https://github.com/lopgogo/Sandra',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(exclude=['tests']),
-    install_requires=['pycryptodome', 'pandas'],
+    install_requires=['pycryptodome', 'pandas', 'rsa'],
     keywords=['python', 'encryption', 'decryption', 'cipher', 'cryptography'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

