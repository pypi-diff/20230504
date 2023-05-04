# Comparing `tmp/autoplugin-0.1.3.tar.gz` & `tmp/autoplugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplugin-0.1.3.tar", last modified: Mon Apr 17 22:42:28 2023, max compression
+gzip compressed data, was "autoplugin-0.1.4.tar", last modified: Thu May  4 18:49:59 2023, max compression
```

## Comparing `autoplugin-0.1.3.tar` & `autoplugin-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.476311 autoplugin-0.1.3/
--rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.3/LICENSE
--rw-r--r--   0 suvansh    (501) staff       (20)     7334 2023-04-17 22:42:28.476128 autoplugin-0.1.3/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)     6481 2023-04-17 22:37:50.000000 autoplugin-0.1.3/README.md
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.474535 autoplugin-0.1.3/autoplugin/
--rw-r--r--   0 suvansh    (501) staff       (20)       81 2023-04-17 22:27:43.000000 autoplugin-0.1.3/autoplugin/__init__.py
--rw-r--r--   0 suvansh    (501) staff       (20)     9781 2023-04-17 22:30:01.000000 autoplugin-0.1.3/autoplugin/autoplugin.py
--rw-r--r--   0 suvansh    (501) staff       (20)      546 2023-04-17 22:27:27.000000 autoplugin-0.1.3/autoplugin/basic_app.py
--rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-04-14 20:36:12.000000 autoplugin-0.1.3/autoplugin/testing.py
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.475822 autoplugin-0.1.3/autoplugin.egg-info/
--rw-r--r--   0 suvansh    (501) staff       (20)     7334 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)      289 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/SOURCES.txt
--rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/dependency_links.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/requires.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/top_level.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-04-17 22:42:28.476367 autoplugin-0.1.3/setup.cfg
--rw-r--r--   0 suvansh    (501) staff       (20)     1200 2023-04-17 22:42:21.000000 autoplugin-0.1.3/setup.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.496769 autoplugin-0.1.4/
+-rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.4/LICENSE
+-rw-r--r--   0 suvansh    (501) staff       (20)     7506 2023-05-04 18:49:59.496641 autoplugin-0.1.4/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)     6595 2023-05-04 18:25:12.000000 autoplugin-0.1.4/README.md
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.495353 autoplugin-0.1.4/autoplugin/
+-rw-r--r--   0 suvansh    (501) staff       (20)       81 2023-04-20 13:10:34.000000 autoplugin-0.1.4/autoplugin/__init__.py
+-rw-r--r--   0 suvansh    (501) staff       (20)    10228 2023-05-04 18:23:19.000000 autoplugin-0.1.4/autoplugin/autoplugin.py
+-rw-r--r--   0 suvansh    (501) staff       (20)      546 2023-04-17 22:27:27.000000 autoplugin-0.1.4/autoplugin/basic_app.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-05-04 18:20:07.000000 autoplugin-0.1.4/autoplugin/testing.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.496403 autoplugin-0.1.4/autoplugin.egg-info/
+-rw-r--r--   0 suvansh    (501) staff       (20)     7506 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)      289 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/requires.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/top_level.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-05-04 18:49:59.496815 autoplugin-0.1.4/setup.cfg
+-rw-r--r--   0 suvansh    (501) staff       (20)     1258 2023-05-04 18:49:46.000000 autoplugin-0.1.4/setup.py
```

### Comparing `autoplugin-0.1.3/LICENSE` & `autoplugin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.3/PKG-INFO` & `autoplugin-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
+Project-URL: Blog, https://brilliantly.ai/blog/autoplugin
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -60,15 +61,16 @@
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
-Optionally, specify `out_dir` to change where they're saved to:
+Optionally, specify `out_dir` to change where they're saved to,
+or set `overwrite_openapi_spec=False` or `overwrite_plugin_spec=False` to avoid overwriting the respective files.
 ```python
 # generated files saved to `.well-known/` directory
 generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
```

### Comparing `autoplugin-0.1.3/README.md` & `autoplugin-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
-Optionally, specify `out_dir` to change where they're saved to:
+Optionally, specify `out_dir` to change where they're saved to,
+or set `overwrite_openapi_spec=False` or `overwrite_plugin_spec=False` to avoid overwriting the respective files.
 ```python
 # generated files saved to `.well-known/` directory
 generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
```

### Comparing `autoplugin-0.1.3/autoplugin/autoplugin.py` & `autoplugin-0.1.4/autoplugin/autoplugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,34 +23,20 @@
 _func_description_chain = None
 
 
 def launch(app: FastAPI, host="127.0.0.1", port=8000):
     uvicorn.run(app, host=host, port=port)
 
 
-def generate(app: FastAPI, out_dir=".well-known", **kwargs):
+def generate(app: FastAPI, version="v1", out_dir=".well-known",
+             overwrite_plugin_spec=True, overwrite_openapi_spec=True,
+             **kwargs):
     """ kwargs should be key-value pairs for the plugin_spec json """
     os.makedirs(out_dir, exist_ok=True)
 
-    """ OpenAPI spec """
-    openapi = get_openapi(
-        title="Custom ChatGPT Plugin",
-        version="1.0.0",
-        routes=app.routes,
-    )
-
-    with open(join(out_dir, "openapi.yaml"), "w") as openapi_yaml:
-        yaml.dump(openapi, openapi_yaml, sort_keys=False)
-    
-    @app.get("/openapi.yaml", response_class=PlainTextResponse)
-    async def get_openapi_yaml():
-        with open(join(out_dir, "openapi.yaml"), "r") as f:
-            content = f.read()
-        return content
-
     """ Plugin manifest file """
     plugin_spec = {
         "name_for_human": "Custom Plugin",
         "name_for_model": "Custom Plugin",
         "description_for_human": "Unspecified custom plugin. Add behavior here.",
         "description_for_model": "Unspecified custom plugin. Add behavior here.",
         "schema_version": "v1",
@@ -62,14 +48,15 @@
             "url": "http://localhost:8000/openapi.yaml",
             "is_user_authenticated": False
         },
         "logo_url": "http://example.com/logo.png",
         "contact_email": "support@example.com",
         "legal_info_url": "http://www.example.com/legal"
     }
+    
     if "name" in kwargs:
         plugin_name = kwargs.pop("name")
         plugin_spec["name_for_human"] = plugin_name
         plugin_spec["name_for_model"] = plugin_name
     if "description" in kwargs:
         plugin_description = kwargs.pop("description")
         plugin_spec["description_for_human"] = plugin_description
@@ -79,22 +66,40 @@
     # character limit checks
     _plugin_check_limit(plugin_spec, "name_for_human", 50)
     _plugin_check_limit(plugin_spec, "name_for_model", 50)
     _plugin_check_limit(plugin_spec, "description_for_human", 120)
     _plugin_check_limit(plugin_spec, "description_for_model",
                        8000)  # will decrease over time
 
-    with open(join(out_dir, "ai-plugin.json"), "w") as plugin_json:
-        json.dump(plugin_spec, plugin_json, indent=4)
+    if overwrite_plugin_spec or not os.path.exists(join(out_dir, "ai-plugin.json")):
+        with open(join(out_dir, "ai-plugin.json"), "w") as plugin_json:
+            json.dump(plugin_spec, plugin_json, indent=4)
 
     @app.get("/.well-known/ai-plugin.json", response_class=PlainTextResponse)
     async def get_plugin_json():
         with open(join(out_dir, "ai-plugin.json"), "r") as f:
             content = f.read()
         return content
+    
+    """ OpenAPI spec """
+    openapi = get_openapi(
+        title=plugin_spec["name_for_human"],
+        version=version,
+        routes=app.routes,
+    )
+
+    if overwrite_openapi_spec or not os.path.exists(join(out_dir, "openapi.yaml")):
+        with open(join(out_dir, "openapi.yaml"), "w") as openapi_yaml:
+            yaml.dump(openapi, openapi_yaml, sort_keys=False)
+    
+    @app.get("/openapi.yaml", response_class=PlainTextResponse)
+    async def get_openapi_yaml():
+        with open(join(out_dir, "openapi.yaml"), "r") as f:
+            content = f.read()
+        return content
 
 
 def register(app: FastAPI,
              func: Callable = None,
              *,
              methods: List[str] = None,
              description: Optional[str] = None,
@@ -130,14 +135,16 @@
         Model = create_model(func.__name__ + "Model", **fields)
 
         async def post_wrapper(payload: Model):
             result = await wrapper(**payload.dict())
             return {"result": result}
 
         return post_wrapper
+    
+    ResponseModel = create_model(f"{func.__name__}ResponseModel", result=(Any, ...))
 
     for method in methods:
         if method == "GET":
             # Create a Pydantic model for the GET request query parameters
             GetModel = create_model(
                 func.__name__ + "GetModel",
                 **{
@@ -153,19 +160,19 @@
                 },
             )
 
             async def get_wrapper(params: GetModel = Depends()):
                 result = await wrapper(**params.dict())
                 return {"result": result}
 
-            app.get(f"/{func.__name__}", description=description)(get_wrapper)
+            app.get(f"/{func.__name__}", description=description, response_model=ResponseModel)(get_wrapper)
         elif method == "POST":
             post_wrapper = get_post_wrapper(func)
             app.post(f"/{func.__name__}",
-                     description=description)(post_wrapper)
+                     description=description, response_model=ResponseModel)(post_wrapper)
 
     return wrapper
 
 
 def _plugin_check_limit(plugin_spec: Dict[str, Any], key: str, char_limit: int):
     assert len(plugin_spec[key]) <= char_limit, \
         f"Key \"{key}\" in plugin spec is too long. Expected: <={char_limit}, found: {len(plugin_spec[key])}."
```

### Comparing `autoplugin-0.1.3/autoplugin/basic_app.py` & `autoplugin-0.1.4/autoplugin/basic_app.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.3/autoplugin/testing.py` & `autoplugin-0.1.4/autoplugin/testing.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.3/autoplugin.egg-info/PKG-INFO` & `autoplugin-0.1.4/autoplugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
+Project-URL: Blog, https://brilliantly.ai/blog/autoplugin
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -60,15 +61,16 @@
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
-Optionally, specify `out_dir` to change where they're saved to:
+Optionally, specify `out_dir` to change where they're saved to,
+or set `overwrite_openapi_spec=False` or `overwrite_plugin_spec=False` to avoid overwriting the respective files.
 ```python
 # generated files saved to `.well-known/` directory
 generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
```

### Comparing `autoplugin-0.1.3/setup.py` & `autoplugin-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autoplugin",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         "fastapi",
         "pydantic",
         "uvicorn",
         "requests",
         "PyYAML",
@@ -19,14 +19,15 @@
     description="Create ChatGPT plugins from Python code",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/suvansh/autoplugin",
     project_urls={        
         'Tracker': 'https://github.com/suvansh/autoplugin/issues',
         'Source': 'https://github.com/suvansh/autoplugin/',
+        'Blog': 'https://brilliantly.ai/blog/autoplugin',
         'Documentation': 'https://github.com/suvansh/AutoPlugin/blob/main/README.md',
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

