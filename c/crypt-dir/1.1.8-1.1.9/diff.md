# Comparing `tmp/crypt-dir-1.1.8.tar.gz` & `tmp/crypt-dir-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypt-dir-1.1.8.tar", last modified: Fri Apr 21 09:10:19 2023, max compression
+gzip compressed data, was "crypt-dir-1.1.9.tar", last modified: Wed Apr 26 16:08:06 2023, max compression
```

## Comparing `crypt-dir-1.1.8.tar` & `crypt-dir-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.108338 crypt-dir-1.1.8/
--rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-03-31 12:34:48.000000 crypt-dir-1.1.8/LICENSE
--rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-21 09:10:19.108204 crypt-dir-1.1.8/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)     4158 2023-04-09 16:58:00.000000 crypt-dir-1.1.8/README.md
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.107249 crypt-dir-1.1.8/crypt_dir/
--rw-r--r--   0 khanh      (501) staff       (20)      181 2023-04-08 11:45:56.000000 crypt-dir-1.1.8/crypt_dir/__init__.py
--rw-r--r--   0 khanh      (501) staff       (20)     2748 2023-04-09 15:05:50.000000 crypt-dir-1.1.8/crypt_dir/crypt.py
--rw-r--r--   0 khanh      (501) staff       (20)     6101 2023-04-06 16:56:20.000000 crypt-dir-1.1.8/crypt_dir/crypt_dir.py
--rw-r--r--   0 khanh      (501) staff       (20)     4075 2023-04-07 17:36:26.000000 crypt-dir-1.1.8/crypt_dir/crypt_file.py
--rw-r--r--   0 khanh      (501) staff       (20)      257 2023-04-06 15:59:40.000000 crypt-dir-1.1.8/crypt_dir/serialize.py
--rw-r--r--   0 khanh      (501) staff       (20)      805 2023-04-06 16:03:15.000000 crypt-dir-1.1.8/crypt_dir/signature.py
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.108011 crypt-dir-1.1.8/crypt_dir.egg-info/
--rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      324 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/SOURCES.txt
--rw-r--r--   0 khanh      (501) staff       (20)        1 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/dependency_links.txt
--rw-r--r--   0 khanh      (501) staff       (20)       20 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/requires.txt
--rw-r--r--   0 khanh      (501) staff       (20)       10 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/top_level.txt
--rw-r--r--   0 khanh      (501) staff       (20)       38 2023-04-21 09:10:19.108383 crypt-dir-1.1.8/setup.cfg
--rw-r--r--   0 khanh      (501) staff       (20)      577 2023-04-21 09:09:52.000000 crypt-dir-1.1.8/setup.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-26 16:08:06.387272 crypt-dir-1.1.9/
+-rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-03-31 12:34:48.000000 crypt-dir-1.1.9/LICENSE
+-rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-26 16:08:06.387133 crypt-dir-1.1.9/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)     4158 2023-04-09 16:58:00.000000 crypt-dir-1.1.9/README.md
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-26 16:08:06.386152 crypt-dir-1.1.9/crypt_dir/
+-rw-r--r--   0 khanh      (501) staff       (20)      181 2023-04-08 11:45:56.000000 crypt-dir-1.1.9/crypt_dir/__init__.py
+-rw-r--r--   0 khanh      (501) staff       (20)     2690 2023-04-26 16:03:29.000000 crypt-dir-1.1.9/crypt_dir/crypt.py
+-rw-r--r--   0 khanh      (501) staff       (20)     6188 2023-04-26 16:03:59.000000 crypt-dir-1.1.9/crypt_dir/crypt_dir.py
+-rw-r--r--   0 khanh      (501) staff       (20)     4080 2023-04-26 15:59:05.000000 crypt-dir-1.1.9/crypt_dir/crypt_file.py
+-rw-r--r--   0 khanh      (501) staff       (20)      257 2023-04-06 15:59:40.000000 crypt-dir-1.1.9/crypt_dir/serialize.py
+-rw-r--r--   0 khanh      (501) staff       (20)      805 2023-04-06 16:03:15.000000 crypt-dir-1.1.9/crypt_dir/signature.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-26 16:08:06.386940 crypt-dir-1.1.9/crypt_dir.egg-info/
+-rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-26 16:08:06.000000 crypt-dir-1.1.9/crypt_dir.egg-info/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      324 2023-04-26 16:08:06.000000 crypt-dir-1.1.9/crypt_dir.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh      (501) staff       (20)        1 2023-04-26 16:08:06.000000 crypt-dir-1.1.9/crypt_dir.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       20 2023-04-26 16:08:06.000000 crypt-dir-1.1.9/crypt_dir.egg-info/requires.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       10 2023-04-26 16:08:06.000000 crypt-dir-1.1.9/crypt_dir.egg-info/top_level.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       38 2023-04-26 16:08:06.387321 crypt-dir-1.1.9/setup.cfg
+-rw-r--r--   0 khanh      (501) staff       (20)      577 2023-04-26 16:06:42.000000 crypt-dir-1.1.9/setup.py
```

### Comparing `crypt-dir-1.1.8/LICENSE` & `crypt-dir-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.8/PKG-INFO` & `crypt-dir-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt-dir
-Version: 1.1.8
+Version: 1.1.9
 Home-page: https://github.com/khanh101/crypt-dir
 Author: Nguyen Ngoc Khanh
 Author-email: khanh.nguyen.contact@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crypt-dir-1.1.8/README.md` & `crypt-dir-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.8/crypt_dir/crypt.py` & `crypt-dir-1.1.9/crypt_dir/crypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     assert len(init_vec) == BLOCK_SIZE
     assert len(key) == KEY_SIZE
 
     aes = AES.new(key, AES_MODE, init_vec)
     remaining_size = file_size
     while remaining_size > 0:
         chunk = encrypted_read_io.read(CHUNK_SIZE)
-        assert len(chunk) == CHUNK_SIZE, "corrupted_file"
 
         b = aes.decrypt(chunk)
 
         if remaining_size < len(b):
             b = b[:remaining_size]
         remaining_size -= len(b)
```

### Comparing `crypt-dir-1.1.8/crypt_dir/crypt_dir.py` & `crypt-dir-1.1.9/crypt_dir/crypt_dir.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
     def make_dir_and_encrypt_file_if_needed(plain_path: str):
         encrypted_path = plain_path_to_encrypted_path(plain_dir, encrypted_dir, plain_path)
         try:
             os.makedirs(os.path.dirname(encrypted_path))
         except FileExistsError:
             pass
+        print(f"encrypting: {encrypted_path}", file=sys.stderr)
         encrypted = codec.encrypt_file_if_needed(plain_path=plain_path, encrypted_path=encrypted_path)
         return encrypted, encrypted_path
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         future_list = [executor.submit(make_dir_and_encrypt_file_if_needed, plain_path) for plain_path in
                        walk_file(plain_dir)]
         for future in concurrent.futures.as_completed(future_list):
@@ -149,17 +150,17 @@
 
     def decrypt_file(encrypted_path: str):
         decrypted_path = encrypted_path_to_plain_path(restored_dir, encrypted_dir, encrypted_path)
         try:
             os.makedirs(os.path.dirname(decrypted_path))
         except FileExistsError:
             pass
-        decrypted = codec.decrypt_file(encrypted_path=encrypted_path, decrypted_path=decrypted_path)
-        return decrypted, decrypted_path
+        print(f"decrypting ... {encrypted_path}", file=sys.stderr)
+        codec.decrypt_file(encrypted_path=encrypted_path, decrypted_path=decrypted_path)
+        return decrypted_path
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         future_list = [executor.submit(decrypt_file, encrypted_path) for encrypted_path in
                        walk_file(encrypted_dir) if is_encrypted_file(encrypted_path)]
         for future in concurrent.futures.as_completed(future_list):
-            decrypted, path = future.result()
-            if decrypted:
-                print(f"decrypted: {path}", file=sys.stderr)
+            decrypted_path = future.result()
+            print(f"decrypted: {decrypted_path}", file=sys.stderr)
```

### Comparing `crypt-dir-1.1.8/crypt_dir/crypt_file.py` & `crypt-dir-1.1.9/crypt_dir/crypt_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 def read_header(read_io: BinaryIO) -> Header:
     def read_exact(n: int) -> bytes:
         b = read_io.read(n)
         assert len(b) == n, "corrupted_file"
         return b
+
     file_sig = read_exact(FILE_SIG_SIZE)
     key_sig = read_exact(KEY_SIG_SIZE)
     file_size = bytes_to_uint64(read_exact(UINT64_SIZE))
     init_vec = read_exact(BLOCK_SIZE)
     return Header(file_sig=file_sig, key_sig=key_sig, file_size=file_size, init_vec=init_vec)
 
 
@@ -44,22 +45,23 @@
         key_sig: bytes | None = None,
 ) -> bool:
     if key_sig is None:
         key_sig = get_key_sig(key)
     file_sig = get_file_sig(plain_path)
     # check file updated
     if os.path.exists(encrypted_path):
-        try:
-            with open(encrypted_path, "rb") as f:
+        with open(encrypted_path, "rb") as f:
+            try:
                 header = read_header(f)
-            if key_sig == header.key_sig and file_sig == header.file_sig:
-                # only skip if both key_sig and file_sig are the same
-                return False
-        except AssertionError:
-            print(f"warning: corrupted encrypted file {encrypted_path}", file=sys.stderr)
+            except AssertionError:
+                print(f"warning: corrupted header encrypted file {encrypted_path}", file=sys.stderr)
+
+        if key_sig == header.key_sig and file_sig == header.file_sig:
+            # only skip if both key_sig and file_sig are the same
+            return False
 
     # encrypted file will be updated regardless its mtime is sooner or later
     # encrypt
     init_vec = os.urandom(BLOCK_SIZE)
     file_size = os.path.getsize(plain_path)
     with open(plain_path, "rb") as plain_f, open(encrypted_path, "wb") as encrypted_f:
         write_header(write_io=encrypted_f, header=Header(
```

### Comparing `crypt-dir-1.1.8/crypt_dir/signature.py` & `crypt-dir-1.1.9/crypt_dir/signature.py`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.8/crypt_dir.egg-info/PKG-INFO` & `crypt-dir-1.1.9/crypt_dir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt-dir
-Version: 1.1.8
+Version: 1.1.9
 Home-page: https://github.com/khanh101/crypt-dir
 Author: Nguyen Ngoc Khanh
 Author-email: khanh.nguyen.contact@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crypt-dir-1.1.8/setup.py` & `crypt-dir-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
     setuptools.setup(
         name="crypt-dir",
-        version="1.1.8",
+        version="1.1.9",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/khanh101/crypt-dir",
         packages=setuptools.find_packages(),
         license="MIT",
```

