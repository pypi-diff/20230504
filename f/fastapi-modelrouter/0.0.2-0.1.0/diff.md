# Comparing `tmp/fastapi-modelrouter-0.0.2.tar.gz` & `tmp/fastapi-modelrouter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-modelrouter-0.0.2.tar", last modified: Thu May  4 08:05:19 2023, max compression
+gzip compressed data, was "fastapi-modelrouter-0.1.0.tar", last modified: Thu May  4 18:37:10 2023, max compression
```

## Comparing `fastapi-modelrouter-0.0.2.tar` & `fastapi-modelrouter-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 08:05:19.817684 fastapi-modelrouter-0.0.2/
--rw-rw-r--   0 windt     (1000) windt     (1000)     1065 2023-05-02 16:43:49.000000 fastapi-modelrouter-0.0.2/LICENSE
--rw-rw-r--   0 windt     (1000) windt     (1000)      537 2023-05-04 08:05:19.817684 fastapi-modelrouter-0.0.2/PKG-INFO
--rw-rw-r--   0 windt     (1000) windt     (1000)      428 2023-05-03 14:42:46.000000 fastapi-modelrouter-0.0.2/README.md
--rw-rw-r--   0 windt     (1000) windt     (1000)      103 2023-05-04 08:05:19.817684 fastapi-modelrouter-0.0.2/setup.cfg
--rw-rw-r--   0 windt     (1000) windt     (1000)     1143 2023-05-04 08:05:12.000000 fastapi-modelrouter-0.0.2/setup.py
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 08:05:19.813684 fastapi-modelrouter-0.0.2/src/
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 08:05:19.813684 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/
--rw-rw-r--   0 windt     (1000) windt     (1000)      537 2023-05-04 08:05:19.000000 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/PKG-INFO
--rw-rw-r--   0 windt     (1000) windt     (1000)      366 2023-05-04 08:05:19.000000 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/SOURCES.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)        1 2023-05-04 08:05:19.000000 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/dependency_links.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)       11 2023-05-04 08:05:19.000000 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/requires.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)       12 2023-05-04 08:05:19.000000 fastapi-modelrouter-0.0.2/src/fastapi_modelrouter.egg-info/top_level.txt
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 08:05:19.813684 fastapi-modelrouter-0.0.2/src/modelrouter/
--rw-rw-r--   0 windt     (1000) windt     (1000)        0 2023-05-04 07:46:21.000000 fastapi-modelrouter-0.0.2/src/modelrouter/__init__.py
--rw-rw-r--   0 windt     (1000) windt     (1000)     2061 2023-05-04 07:45:26.000000 fastapi-modelrouter-0.0.2/src/modelrouter/model_to_pydantic.py
--rw-rw-r--   0 windt     (1000) windt     (1000)     9723 2023-05-04 07:45:26.000000 fastapi-modelrouter-0.0.2/src/modelrouter/modelrouter.py
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1065 2023-05-02 17:18:03.000000 fastapi-modelrouter-0.1.0/LICENSE
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2204 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/PKG-INFO
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1384 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/README.md
+-rw-rw-r--   0 windt     (1000) windt     (1000)      103 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/setup.cfg
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1497 2023-05-04 18:37:02.000000 fastapi-modelrouter-0.1.0/setup.py
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.056375 fastapi-modelrouter-0.1.0/src/
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.056375 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2204 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/PKG-INFO
+-rw-rw-r--   0 windt     (1000) windt     (1000)      366 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/SOURCES.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)        1 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/dependency_links.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)       19 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/requires.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)       12 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/top_level.txt
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/src/modelrouter/
+-rw-rw-r--   0 windt     (1000) windt     (1000)      141 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/__init__.py
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2061 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/model_to_pydantic.py
+-rw-rw-r--   0 windt     (1000) windt     (1000)     9725 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/modelrouter.py
```

### Comparing `fastapi-modelrouter-0.0.2/LICENSE` & `fastapi-modelrouter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-modelrouter-0.0.2/setup.py` & `fastapi-modelrouter-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapi-modelrouter',
-    version='0.0.2',
+    version='0.1.0',
     license='MIT',
-    description='CRUD Router for SqlAlchemy models',
+    description='FastAPI Router that creates CRUD routes for SqlAlchemy models',
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     author="Uwe Windt",
     author_email='uwe.windt@windisoft.de',
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    url='https://github.com/UweWindt/fastapi-modelrouter',
-    keywords='fastapi router sqlalchemy',
+    url="https://github.com/UweWindt/fastapi-modelrouter",
+    keywords='fastapi router sqlalchemy development',
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         'Development Status :: 3 - Alpha',
 
@@ -23,14 +25,19 @@
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
         'sqlalchemy',
+        'fastapi'
     ],
 
 )
```

### Comparing `fastapi-modelrouter-0.0.2/src/modelrouter/model_to_pydantic.py` & `fastapi-modelrouter-0.1.0/src/modelrouter/model_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `fastapi-modelrouter-0.0.2/src/modelrouter/modelrouter.py` & `fastapi-modelrouter-0.1.0/src/modelrouter/modelrouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.pk_schema: Type[BaseModel] = model_to_pydantic(db_model,
                                                             name=db_model.__name__ + 'Pk',
                                                             only_pk=True)
         self.nonpk_schema: Type[BaseModel] = model_to_pydantic(db_model,
                                                                name=db_model.__name__ + 'body',
                                                                exclude_pk=True)
 
-        prefix = prefix if prefix != "" else "/"+db_model.__name__.lower()
+        prefix = prefix if prefix != "" else "/" + db_model.__name__.lower()
         print(prefix)
         super().__init__(prefix=prefix, tags=tags, **kwargs)
 
         if get_all_route:
             self._add_api_route(
                 "",
                 self._get_all(),
```

