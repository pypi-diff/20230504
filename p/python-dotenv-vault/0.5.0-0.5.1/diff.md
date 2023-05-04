# Comparing `tmp/python-dotenv-vault-0.5.0.tar.gz` & `tmp/python-dotenv-vault-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.5.0.tar", last modified: Wed May  3 17:59:17 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.5.1.tar", last modified: Thu May  4 06:13:15 2023, max compression
```

## Comparing `python-dotenv-vault-0.5.0.tar` & `python-dotenv-vault-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.767441 python-dotenv-vault-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-03 17:58:58.000000 python-dotenv-vault-0.5.0/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:59:17.771441 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 17:59:17.000000 python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.292907 python-dotenv-vault-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.5.0/CHANGELOG.md` & `python-dotenv-vault-0.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.0/PKG-INFO` & `python-dotenv-vault-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.0
+Version: 0.5.1
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
```

### Comparing `python-dotenv-vault-0.5.0/README.md` & `python-dotenv-vault-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.0/setup.py` & `python-dotenv-vault-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.0/src/dotenv_vault/main.py` & `python-dotenv-vault-0.5.1/src/dotenv_vault/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     # https://www.dotenv.org/docs/security/dotenv-key).
     uri = urlparse(dotenv_key)
     
     # The 64-character encryption key is stored in the password field
     # of the URI, possibly with a prefix.
     key = uri.password
     if len(key) < KEY_LENGTH: 
-        raise DotEnvVault('INVALID_DOTENV_KEY: Key part must be 64 characters long (or more)')
+        raise DotEnvVaultError('INVALID_DOTENV_KEY: Key part must be 64 characters long (or more)')
         
     # The environment is provided in the URI's query parameters.
     params = dict(parse_qsl(uri.query))
     vault_environment = params.get('environment')
     if not vault_environment:
         raise DotEnvVaultError('INVALID_DOTENV_KEY: Missing environment part')
 
@@ -148,8 +148,7 @@
     """
     for k in keys:
         try:
             return _decrypt(ciphertext=k['ciphertext'], key=k['encrypted_key'])
         except InvalidTag:
             continue
     raise DotEnvVaultError('INVALID_DOTENV_KEY: Key must be valid.')
-
```

### Comparing `python-dotenv-vault-0.5.0/src/dotenv_vault/test_vault.py` & `python-dotenv-vault-0.5.1/src/dotenv_vault/test_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,21 @@
                 os.unsetenv("DOTENV_KEY")
                 if old_dotenv_key:
                     os.environ["DOTENV_KEY"] = old_dotenv_key
 
     PARSE_TEST_KEY = "dotenv://:key_0dec82bea24ada79a983dcc11b431e28838eae59a07a8f983247c7ca9027a925@dotenv.local/vault/.env.vault?environment=development"
 
     PARSE_TEST_VAULT = """# .env.vault (generated with npx dotenv-vault local build)
-DOTENV_VAULT_DEVELOPMENT="H2A2wOUZU+bjKH3kTpeua9iIhtK/q7/VpAn+LLVNnms+CtQ/cwXqiw=="
-"""
+                        DOTENV_VAULT_DEVELOPMENT="H2A2wOUZU+bjKH3kTpeua9iIhtK/q7/VpAn+LLVNnms+CtQ/cwXqiw=="
+                        """
                 
     def test_vault_parsing(self):
         old_dotenv_key = os.environ.get("DOTENV_KEY")
         os.environ["DOTENV_KEY"] = self.PARSE_TEST_KEY
         try:
             stream = vault.parse_vault(StringIO(self.PARSE_TEST_VAULT))
             dotenv = DotEnv(dotenv_path=".env.vault", stream=stream)
             self.assertEqual(dotenv.dict().get("HELLO"), "world")
         finally:
             os.unsetenv("DOTENV_KEY")
             if old_dotenv_key:
                 os.environ["DOTENV_KEY"] = old_dotenv_key
-
```

### Comparing `python-dotenv-vault-0.5.0/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.0
+Version: 0.5.1
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
```

