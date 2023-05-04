# Comparing `tmp/py_multiauth-2.0.0rc0.tar.gz` & `tmp/py_multiauth-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_multiauth-2.0.0rc0.tar", max compression
+gzip compressed data, was "py_multiauth-2.0.0rc1.tar", max compression
```

## Comparing `py_multiauth-2.0.0rc0.tar` & `py_multiauth-2.0.0rc1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1117 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/LICENSE
--rw-r--r--   0        0        0     2572 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/README.md
--rw-r--r--   0        0        0      152 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/__init__.py
--rw-r--r--   0        0        0       94 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/__main__.py
--rw-r--r--   0        0        0     2088 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/cli.py
--rw-r--r--   0        0        0       40 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/__init__.py
--rw-r--r--   0        0        0      598 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/errors.py
--rw-r--r--   0        0        0      474 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/http.py
--rw-r--r--   0        0        0     2250 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/interfaces.py
--rw-r--r--   0        0        0     3101 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/main.py
--rw-r--r--   0        0        0        0 2023-02-27 19:58:35.685070 py_multiauth-2.0.0rc0/multiauth/entities/providers/__init__.py
--rw-r--r--   0        0        0     1719 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/entities/providers/aws.py
--rw-r--r--   0        0        0      830 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/entities/providers/graphql.py
--rw-r--r--   0        0        0     1575 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/entities/providers/oauth.py
--rw-r--r--   0        0        0      632 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/entities/providers/rest.py
--rw-r--r--   0        0        0      511 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/entities/utils.py
--rw-r--r--   0        0        0     7876 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/generator.py
--rw-r--r--   0        0        0     3381 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/handlers.py
--rw-r--r--   0        0        0    13730 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/helpers.py
--rw-r--r--   0        0        0    10409 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/main.py
--rw-r--r--   0        0        0     6462 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/manager.py
--rw-r--r--   0        0        0      599 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/__init__.py
--rw-r--r--   0        0        0     3198 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/apikey.py
--rw-r--r--   0        0        0    15633 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/aws.py
--rw-r--r--   0        0        0     1590 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/basic.py
--rw-r--r--   0        0        0     9003 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/digest.py
--rw-r--r--   0        0        0    14465 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/graphql.py
--rw-r--r--   0        0        0     1067 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/manual.py
--rw-r--r--   0        0        0    15749 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/oauth.py
--rw-r--r--   0        0        0     9672 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/providers/rest.py
--rw-r--r--   0        0        0        0 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/py.typed
--rw-r--r--   0        0        0        0 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/static/__init__.py
--rw-r--r--   0        0        0    44688 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/static/auth_schema.json
--rw-r--r--   0        0        0     5361 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/multiauth/utils.py
--rw-r--r--   0        0        0     1692 2023-02-27 19:58:35.689070 py_multiauth-2.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc0/setup.py
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-04 10:03:08.722401 py_multiauth-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2572 2023-05-04 10:03:08.722401 py_multiauth-2.0.0rc1/README.md
+-rw-r--r--   0        0        0      152 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/__main__.py
+-rw-r--r--   0        0        0     2088 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/cli.py
+-rw-r--r--   0        0        0       40 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/__init__.py
+-rw-r--r--   0        0        0      598 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/errors.py
+-rw-r--r--   0        0        0      474 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/http.py
+-rw-r--r--   0        0        0     2250 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/interfaces.py
+-rw-r--r--   0        0        0     3101 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/main.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/__init__.py
+-rw-r--r--   0        0        0     1719 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/aws.py
+-rw-r--r--   0        0        0      830 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/graphql.py
+-rw-r--r--   0        0        0     1575 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/oauth.py
+-rw-r--r--   0        0        0      632 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/providers/rest.py
+-rw-r--r--   0        0        0      511 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/entities/utils.py
+-rw-r--r--   0        0        0     7876 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/generator.py
+-rw-r--r--   0        0        0     3381 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/handlers.py
+-rw-r--r--   0        0        0    13730 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/helpers.py
+-rw-r--r--   0        0        0    10409 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/main.py
+-rw-r--r--   0        0        0     6462 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/manager.py
+-rw-r--r--   0        0        0      599 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/__init__.py
+-rw-r--r--   0        0        0     3198 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/apikey.py
+-rw-r--r--   0        0        0    15633 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/aws.py
+-rw-r--r--   0        0        0     1590 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/basic.py
+-rw-r--r--   0        0        0     9003 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/digest.py
+-rw-r--r--   0        0        0    14577 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/graphql.py
+-rw-r--r--   0        0        0     1067 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/manual.py
+-rw-r--r--   0        0        0    15749 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/oauth.py
+-rw-r--r--   0        0        0     9672 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/providers/rest.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/py.typed
+-rw-r--r--   0        0        0        0 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/static/__init__.py
+-rw-r--r--   0        0        0    44688 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/static/auth_schema.json
+-rw-r--r--   0        0        0     5361 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/multiauth/utils.py
+-rw-r--r--   0        0        0     1496 2023-05-04 10:03:08.726401 py_multiauth-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 py_multiauth-2.0.0rc1/PKG-INFO
```

### Comparing `py_multiauth-2.0.0rc0/LICENSE` & `py_multiauth-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/README.md` & `py_multiauth-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/cli.py` & `py_multiauth-2.0.0rc1/multiauth/cli.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/errors.py` & `py_multiauth-2.0.0rc1/multiauth/entities/errors.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/interfaces.py` & `py_multiauth-2.0.0rc1/multiauth/entities/interfaces.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/main.py` & `py_multiauth-2.0.0rc1/multiauth/entities/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/providers/aws.py` & `py_multiauth-2.0.0rc1/multiauth/entities/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/providers/graphql.py` & `py_multiauth-2.0.0rc1/multiauth/entities/providers/graphql.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/providers/oauth.py` & `py_multiauth-2.0.0rc1/multiauth/entities/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/entities/providers/rest.py` & `py_multiauth-2.0.0rc1/multiauth/entities/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/generator.py` & `py_multiauth-2.0.0rc1/multiauth/generator.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/handlers.py` & `py_multiauth-2.0.0rc1/multiauth/handlers.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/helpers.py` & `py_multiauth-2.0.0rc1/multiauth/helpers.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/main.py` & `py_multiauth-2.0.0rc1/multiauth/main.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/manager.py` & `py_multiauth-2.0.0rc1/multiauth/manager.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/__init__.py` & `py_multiauth-2.0.0rc1/multiauth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/apikey.py` & `py_multiauth-2.0.0rc1/multiauth/providers/apikey.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/aws.py` & `py_multiauth-2.0.0rc1/multiauth/providers/aws.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/basic.py` & `py_multiauth-2.0.0rc1/multiauth/providers/basic.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/digest.py` & `py_multiauth-2.0.0rc1/multiauth/providers/digest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/graphql.py` & `py_multiauth-2.0.0rc1/multiauth/providers/graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
         raise AuthenticationError('Please provide with the authentication URL')
     if not schema.get('mutation_name'):
         raise AuthenticationError('Please provide the mutation name for the authentication')
     if not schema.get('mutation_field'):
         raise AuthenticationError('Please provide the mutation field in the authentication response')
 
     auth_config['url'] = schema['url']
+    if not auth_config['url'].startswith('http'):
+        auth_config['url'] = 'https://' + auth_config['url']
+
     auth_config['mutation_name'] = schema['mutation_name']
     auth_config['mutation_field'] = schema['mutation_field']
 
     # Options
     if 'options' in schema:
         auth_config['refresh_mutation_name'] = schema['options'].get('refresh_mutation_name')
         auth_config['refresh_field_name'] = schema['options'].get('refresh_field_name')
```

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/manual.py` & `py_multiauth-2.0.0rc1/multiauth/providers/manual.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/oauth.py` & `py_multiauth-2.0.0rc1/multiauth/providers/oauth.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/providers/rest.py` & `py_multiauth-2.0.0rc1/multiauth/providers/rest.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/static/auth_schema.json` & `py_multiauth-2.0.0rc1/multiauth/static/auth_schema.json`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/multiauth/utils.py` & `py_multiauth-2.0.0rc1/multiauth/utils.py`

 * *Files identical despite different names*

### Comparing `py_multiauth-2.0.0rc0/pyproject.toml` & `py_multiauth-2.0.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-multiauth"
-version = "2.0.0-rc.0"
+version = "2.0.0-rc.1"
 description = "Python package to interact with multiple authentication services"
 authors = ["Escape Technologies SAS <ping@escape.tech>"]
 maintainers = [
     "Antoine Carossio <antoine@escape.tech>",
     "Swan <swan@escape.tech>"
 ]
 license = "MIT"
@@ -41,24 +41,18 @@
 PyJWT = "^2.6.0"
 python = ">=3.8,<4.0"
 jsonschema = "^4.17.3"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^2.0.1"
 docformatter = "^1.5.1"
-isort = [
-    {version = "^5.10.1", python = ">=3.7,<3.7.2"},
-    {version = "^5.10.1", python = ">=3.7.2,<4.0"},
-]
+isort = "^5.10.1"
 mypy = "^1.0.1"
 poetryup = "^0.12.7"
-pylint = [
-    {version = "^2.13.0", python = ">=3.7,<3.7.2"},
-    {version = "^2.15.0", python = ">=3.7.2,<4.0"},
-]
+pylint = "^2.15.0"
 pylint-quotes = "^0.2.3"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 setuptools = "^67.3.2"
 types-boto3 = "^1.0.2"
```

### Comparing `py_multiauth-2.0.0rc0/setup.py` & `py_multiauth-2.0.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-multiauth
+Version: 2.0.0rc1
+Summary: Python package to interact with multiple authentication services
+Home-page: https://escape.tech/
+License: MIT
+Author: Escape Technologies SAS
+Author-email: ping@escape.tech
+Maintainer: Antoine Carossio
+Maintainer-email: antoine@escape.tech
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Authlib (>=1.2.0,<2.0.0)
+Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
+Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: pycognito (>=2022.12.0,<2023.0.0)
+Requires-Dist: pydash (>=6.0.0,<7.0.0)
+Project-URL: Bug Tracker, https://github.com/Escape-Technologies/py-multiauth/issues
+Project-URL: Repository, https://github.com/Escape-Technologies/py-multiauth
+Description-Content-Type: text/markdown
+
+# py-multiauth ![PyPI](https://img.shields.io/pypi/v/py-multiauth) [![CI](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml) [![CD](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml) [![codecov](https://codecov.io/gh/Escape-Technologies/py-multiauth/branch/main/graph/badge.svg?token=NL148MNKAE)](https://codecov.io/gh/Escape-Technologies/py-multiauth)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-multiauth)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/py-multiauth)
+
+## Installation
+
+```bash
+pip install py-multiauth
+```
+
+## Supported methods
+
+|Name     |Authenticate|Refresh|Extra    |
+|---------|:----------:|:-----:|---------|
+|`API_KEY`|✓           |       |         |
+|`AWS`    |✓           |✓      |Signature|
+|`BASIC`  |✓           |       |         |
+|`REST`   |✓           |✓      |         |
+|`DIGEST` |✓           |       |         |
+|`GRAPHQL`|✓           |       |         |
+|`HAWK`   |✓           |       |         |
+|`MANUAL` |✓           |       |         |
+|`OAUTH`  |✓           |✓      |         |
+
+## Usage
+
+### Loading a configuration file
+
+Currently, we support 4 way of loading a configuration file.
+
+```python
+
+# Using constructor argument
+MultiAuth(authrc_file='path.json')
+
+# Using environment variable
+os.environ['AUTHRC'] = 'path.json'
+
+# Using autodection
+os.paths.exists('.authrc')?
+
+# Using autodection from user home directory
+os.path.exists(os.path.expanduser('~/.multiauth/.authrc'))?
+```
+
+### Managing authentication flow
+
+**MultiAuth supports context singleton.
+From that, you can instanciate MultiAuth and re-use the same class in another package as far it is sharing the same context.**
+
+```python
+auth = MultiAuth(auths=.., users=.., authrc=.., logger=..)
+
+# Sending the requests to get the correct headers
+auth.authenticate_users()
+
+# Getting the header before sending a HTTP request
+auth_headers = auth.reauthenticate(username=.., additional_headers=.., public=..)
+r = requests.get('https://example.com', headers=auth_headers[0])
+```
+
+## Contributing
 
-packages = \
-['multiauth',
- 'multiauth.entities',
- 'multiauth.entities.providers',
- 'multiauth.providers',
- 'multiauth.static']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Authlib>=1.2.0,<2.0.0',
- 'PyJWT>=2.6.0,<3.0.0',
- 'graphql-core>=3.2.3,<4.0.0',
- 'jsonschema>=4.17.3,<5.0.0',
- 'pycognito>=2022.12.0,<2023.0.0',
- 'pydash>=6.0.0,<7.0.0']
-
-entry_points = \
-{'console_scripts': ['multiauth = multiauth:cli']}
-
-setup_kwargs = {
-    'name': 'py-multiauth',
-    'version': '2.0.0rc0',
-    'description': 'Python package to interact with multiple authentication services',
-    'long_description': "# py-multiauth ![PyPI](https://img.shields.io/pypi/v/py-multiauth) [![CI](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/ci.yaml) [![CD](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml/badge.svg)](https://github.com/Escape-Technologies/py-multiauth/actions/workflows/cd.yaml) [![codecov](https://codecov.io/gh/Escape-Technologies/py-multiauth/branch/main/graph/badge.svg?token=NL148MNKAE)](https://codecov.io/gh/Escape-Technologies/py-multiauth)\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-multiauth)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/py-multiauth)\n\n## Installation\n\n```bash\npip install py-multiauth\n```\n\n## Supported methods\n\n|Name     |Authenticate|Refresh|Extra    |\n|---------|:----------:|:-----:|---------|\n|`API_KEY`|✓           |       |         |\n|`AWS`    |✓           |✓      |Signature|\n|`BASIC`  |✓           |       |         |\n|`REST`   |✓           |✓      |         |\n|`DIGEST` |✓           |       |         |\n|`GRAPHQL`|✓           |       |         |\n|`HAWK`   |✓           |       |         |\n|`MANUAL` |✓           |       |         |\n|`OAUTH`  |✓           |✓      |         |\n\n## Usage\n\n### Loading a configuration file\n\nCurrently, we support 4 way of loading a configuration file.\n\n```python\n\n# Using constructor argument\nMultiAuth(authrc_file='path.json')\n\n# Using environment variable\nos.environ['AUTHRC'] = 'path.json'\n\n# Using autodection\nos.paths.exists('.authrc')?\n\n# Using autodection from user home directory\nos.path.exists(os.path.expanduser('~/.multiauth/.authrc'))?\n```\n\n### Managing authentication flow\n\n**MultiAuth supports context singleton.\nFrom that, you can instanciate MultiAuth and re-use the same class in another package as far it is sharing the same context.**\n\n```python\nauth = MultiAuth(auths=.., users=.., authrc=.., logger=..)\n\n# Sending the requests to get the correct headers\nauth.authenticate_users()\n\n# Getting the header before sending a HTTP request\nauth_headers = auth.reauthenticate(username=.., additional_headers=.., public=..)\nr = requests.get('https://example.com', headers=auth_headers[0])\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License ![PyPI - License](https://img.shields.io/pypi/l/py-multiauth)\n\n[MIT](https://choosealicense.com/licenses/mit/)\n",
-    'author': 'Escape Technologies SAS',
-    'author_email': 'ping@escape.tech',
-    'maintainer': 'Antoine Carossio',
-    'maintainer_email': 'antoine@escape.tech',
-    'url': 'https://escape.tech/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
+Please make sure to update tests as appropriate.
+
+## License ![PyPI - License](https://img.shields.io/pypi/l/py-multiauth)
+
+[MIT](https://choosealicense.com/licenses/mit/)
 
-setup(**setup_kwargs)
```

