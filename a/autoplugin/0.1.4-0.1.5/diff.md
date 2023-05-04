# Comparing `tmp/autoplugin-0.1.4.tar.gz` & `tmp/autoplugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplugin-0.1.4.tar", last modified: Thu May  4 18:49:59 2023, max compression
+gzip compressed data, was "autoplugin-0.1.5.tar", last modified: Thu May  4 19:55:44 2023, max compression
```

## Comparing `autoplugin-0.1.4.tar` & `autoplugin-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.496769 autoplugin-0.1.4/
--rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.4/LICENSE
--rw-r--r--   0 suvansh    (501) staff       (20)     7506 2023-05-04 18:49:59.496641 autoplugin-0.1.4/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)     6595 2023-05-04 18:25:12.000000 autoplugin-0.1.4/README.md
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.495353 autoplugin-0.1.4/autoplugin/
--rw-r--r--   0 suvansh    (501) staff       (20)       81 2023-04-20 13:10:34.000000 autoplugin-0.1.4/autoplugin/__init__.py
--rw-r--r--   0 suvansh    (501) staff       (20)    10228 2023-05-04 18:23:19.000000 autoplugin-0.1.4/autoplugin/autoplugin.py
--rw-r--r--   0 suvansh    (501) staff       (20)      546 2023-04-17 22:27:27.000000 autoplugin-0.1.4/autoplugin/basic_app.py
--rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-05-04 18:20:07.000000 autoplugin-0.1.4/autoplugin/testing.py
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 18:49:59.496403 autoplugin-0.1.4/autoplugin.egg-info/
--rw-r--r--   0 suvansh    (501) staff       (20)     7506 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)      289 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/SOURCES.txt
--rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/dependency_links.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/requires.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-05-04 18:49:59.000000 autoplugin-0.1.4/autoplugin.egg-info/top_level.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-05-04 18:49:59.496815 autoplugin-0.1.4/setup.cfg
--rw-r--r--   0 suvansh    (501) staff       (20)     1258 2023-05-04 18:49:46.000000 autoplugin-0.1.4/setup.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 19:55:44.585160 autoplugin-0.1.5/
+-rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.5/LICENSE
+-rw-r--r--   0 suvansh    (501) staff       (20)     8480 2023-05-04 19:55:44.584991 autoplugin-0.1.5/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)     7569 2023-05-04 19:48:00.000000 autoplugin-0.1.5/README.md
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 19:55:44.584158 autoplugin-0.1.5/autoplugin/
+-rw-r--r--   0 suvansh    (501) staff       (20)       81 2023-04-20 13:10:34.000000 autoplugin-0.1.5/autoplugin/__init__.py
+-rw-r--r--   0 suvansh    (501) staff       (20)    10160 2023-05-04 19:52:07.000000 autoplugin-0.1.5/autoplugin/autoplugin.py
+-rw-r--r--   0 suvansh    (501) staff       (20)      546 2023-04-17 22:27:27.000000 autoplugin-0.1.5/autoplugin/basic_app.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-05-04 18:20:07.000000 autoplugin-0.1.5/autoplugin/testing.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-05-04 19:55:44.584775 autoplugin-0.1.5/autoplugin.egg-info/
+-rw-r--r--   0 suvansh    (501) staff       (20)     8480 2023-05-04 19:55:44.000000 autoplugin-0.1.5/autoplugin.egg-info/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)      289 2023-05-04 19:55:44.000000 autoplugin-0.1.5/autoplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-05-04 19:55:44.000000 autoplugin-0.1.5/autoplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-05-04 19:55:44.000000 autoplugin-0.1.5/autoplugin.egg-info/requires.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-05-04 19:55:44.000000 autoplugin-0.1.5/autoplugin.egg-info/top_level.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-05-04 19:55:44.585204 autoplugin-0.1.5/setup.cfg
+-rw-r--r--   0 suvansh    (501) staff       (20)     1258 2023-05-04 19:55:25.000000 autoplugin-0.1.5/setup.py
```

### Comparing `autoplugin-0.1.4/LICENSE` & `autoplugin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.4/PKG-INFO` & `autoplugin-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Blog, https://brilliantly.ai/blog/autoplugin
@@ -111,41 +111,75 @@
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
-## The `@register` Decorator
-The `@register` decorator is used as follows:
+
+## Docs 
+
+### The `@register` Decorator
+
+The `@register` decorator is used as follows:
+
 ```python
 @register(app: FastAPI,
             methods: List[str],                     # which HTTP methods to support
             description: Optional[str],             # if provided, used as is
             generate_description: Optional[bool])   # whether to autogenerate a description
 def my_func(...):
     ...
 ```
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
-Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
 
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few arguments to customize the behavior of this generation.
+
+- `app`: Your FastAPI application. AutoPlugin provides a `get_app` function that includes CORSMiddleware for testing convenience (allows all origins by default).
+- `methods`: A list of HTTP methods to be supported (e.g. ”GET”, POST”)
+- `description`: If provided, overrides everything else and is used directly as the endpoint description for the OpenAPI spec
+- `generate_description`: If set to `True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+
+By default (if neither `description` nor `generate_description` are provided), the description is fetched from the docstring. If there's no docstring, AutoPlugin falls back to generating one automatically.
+
+
+### The `generate` Function
 
-## The `generate` Function
 The `generate` function has the following signature:
+
+```python
+def generate(app: FastAPI, version="v1", out_dir=".well-known",
+             overwrite_plugin_spec=True, overwrite_openapi_spec=True,
+             name="", description="",
+             **kwargs)
+```
+
+- `app`: Your FastAPI application again.
+- `version="v1"`: What version number to pass to both the plugin and OpenAPI specs.
+- `out_dir=".well-known"`: The directory to save both files to.
+- `overwrite_plugin_spec=True`: If set to False, does not overwrite `ai-plugin.json` if it already exists.
+- `overwrite_openapi_spec=True`: If set to False, does not overwrite `openapi.yaml` if it already exists.
+- `name=""`: If specified, used for both `name_for_human` and `name_for_model`.
+- `description=""`: If specified, used for both `description_for_human` and `description_for_model`. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `**kwargs`: All other keyword arguments are passed on to `ai-plugin.json` directly. See the full list of possible options [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+
+
+### The `launch` Function
+
+The `launch` function has the following signature:
+
 ```python
-def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+def launch(app: FastAPI, host="127.0.0.1", port=8000):
 ```
-The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
 
-All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
-The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `app`: Still your FastAPI application.
+- `host="127.0.0.1"`: the host to launch the server on
+- `port=8000`: the port to launch the server on
 
 
-## Testing
+### Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
 
 def test_api():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoplugin-0.1.4/README.md` & `autoplugin-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -89,41 +89,75 @@
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
-## The `@register` Decorator
-The `@register` decorator is used as follows:
+
+## Docs 
+
+### The `@register` Decorator
+
+The `@register` decorator is used as follows:
+
 ```python
 @register(app: FastAPI,
             methods: List[str],                     # which HTTP methods to support
             description: Optional[str],             # if provided, used as is
             generate_description: Optional[bool])   # whether to autogenerate a description
 def my_func(...):
     ...
 ```
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
-Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
 
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few arguments to customize the behavior of this generation.
+
+- `app`: Your FastAPI application. AutoPlugin provides a `get_app` function that includes CORSMiddleware for testing convenience (allows all origins by default).
+- `methods`: A list of HTTP methods to be supported (e.g. ”GET”, POST”)
+- `description`: If provided, overrides everything else and is used directly as the endpoint description for the OpenAPI spec
+- `generate_description`: If set to `True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+
+By default (if neither `description` nor `generate_description` are provided), the description is fetched from the docstring. If there's no docstring, AutoPlugin falls back to generating one automatically.
+
+
+### The `generate` Function
 
-## The `generate` Function
 The `generate` function has the following signature:
+
+```python
+def generate(app: FastAPI, version="v1", out_dir=".well-known",
+             overwrite_plugin_spec=True, overwrite_openapi_spec=True,
+             name="", description="",
+             **kwargs)
+```
+
+- `app`: Your FastAPI application again.
+- `version="v1"`: What version number to pass to both the plugin and OpenAPI specs.
+- `out_dir=".well-known"`: The directory to save both files to.
+- `overwrite_plugin_spec=True`: If set to False, does not overwrite `ai-plugin.json` if it already exists.
+- `overwrite_openapi_spec=True`: If set to False, does not overwrite `openapi.yaml` if it already exists.
+- `name=""`: If specified, used for both `name_for_human` and `name_for_model`.
+- `description=""`: If specified, used for both `description_for_human` and `description_for_model`. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `**kwargs`: All other keyword arguments are passed on to `ai-plugin.json` directly. See the full list of possible options [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+
+
+### The `launch` Function
+
+The `launch` function has the following signature:
+
 ```python
-def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+def launch(app: FastAPI, host="127.0.0.1", port=8000):
 ```
-The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
 
-All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
-The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `app`: Still your FastAPI application.
+- `host="127.0.0.1"`: the host to launch the server on
+- `port=8000`: the port to launch the server on
 
 
-## Testing
+### Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
 
 def test_api():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoplugin-0.1.4/autoplugin/autoplugin.py` & `autoplugin-0.1.5/autoplugin/autoplugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,46 +25,45 @@
 
 def launch(app: FastAPI, host="127.0.0.1", port=8000):
     uvicorn.run(app, host=host, port=port)
 
 
 def generate(app: FastAPI, version="v1", out_dir=".well-known",
              overwrite_plugin_spec=True, overwrite_openapi_spec=True,
+             name="", description="",
              **kwargs):
     """ kwargs should be key-value pairs for the plugin_spec json """
     os.makedirs(out_dir, exist_ok=True)
 
     """ Plugin manifest file """
     plugin_spec = {
         "name_for_human": "Custom Plugin",
         "name_for_model": "Custom Plugin",
         "description_for_human": "Unspecified custom plugin. Add behavior here.",
         "description_for_model": "Unspecified custom plugin. Add behavior here.",
-        "schema_version": "v1",
+        "schema_version": version,
         "auth": {
             "type": "none"
         },
         "api": {
             "type": "openapi",
             "url": "http://localhost:8000/openapi.yaml",
             "is_user_authenticated": False
         },
         "logo_url": "http://example.com/logo.png",
         "contact_email": "support@example.com",
         "legal_info_url": "http://www.example.com/legal"
     }
     
-    if "name" in kwargs:
-        plugin_name = kwargs.pop("name")
-        plugin_spec["name_for_human"] = plugin_name
-        plugin_spec["name_for_model"] = plugin_name
-    if "description" in kwargs:
-        plugin_description = kwargs.pop("description")
-        plugin_spec["description_for_human"] = plugin_description
-        plugin_spec["description_for_model"] = plugin_description
+    if name:
+        plugin_spec["name_for_human"] = name
+        plugin_spec["name_for_model"] = name
+    if description:
+        plugin_spec["description_for_human"] = description
+        plugin_spec["description_for_model"] = description
     plugin_spec.update(kwargs)
 
     # character limit checks
     _plugin_check_limit(plugin_spec, "name_for_human", 50)
     _plugin_check_limit(plugin_spec, "name_for_model", 50)
     _plugin_check_limit(plugin_spec, "description_for_human", 120)
     _plugin_check_limit(plugin_spec, "description_for_model",
@@ -184,15 +183,15 @@
         if _func_description_chain is not None:
             return _func_description_chain.run(func_str=func_str)
         try:
             from langchain.llms import OpenAI
             from langchain.prompts import PromptTemplate
             from langchain.chains import LLMChain
         except ImportError:
-            raise ImportError("Please install LangChain to generate function descriptions. Otherwise, set `generate_description=False` when registering your function.")
+            raise ImportError("Please install dependencies with `pip install 'autoplugin[gen]` to generate function descriptions. Otherwise, set `generate_description=False` when registering your function.")
         llm = OpenAI(temperature=0, max_tokens=100)
         # prompt = PromptTemplate(
         #     input_variables=["func_str"],
         #     template="""
         #         Come up with a concise description for this function for the OpenAPI spec that would serve as a useful description for a ChatGPT plugin to know when to call it.
         #         It should be at most one or two sentences, and must be less than 50 words.
         #         Function:
```

### Comparing `autoplugin-0.1.4/autoplugin/basic_app.py` & `autoplugin-0.1.5/autoplugin/basic_app.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.4/autoplugin/testing.py` & `autoplugin-0.1.5/autoplugin/testing.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.4/autoplugin.egg-info/PKG-INFO` & `autoplugin-0.1.5/autoplugin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Blog, https://brilliantly.ai/blog/autoplugin
@@ -111,41 +111,75 @@
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
-## The `@register` Decorator
-The `@register` decorator is used as follows:
+
+## Docs 
+
+### The `@register` Decorator
+
+The `@register` decorator is used as follows:
+
 ```python
 @register(app: FastAPI,
             methods: List[str],                     # which HTTP methods to support
             description: Optional[str],             # if provided, used as is
             generate_description: Optional[bool])   # whether to autogenerate a description
 def my_func(...):
     ...
 ```
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
-Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
 
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few arguments to customize the behavior of this generation.
+
+- `app`: Your FastAPI application. AutoPlugin provides a `get_app` function that includes CORSMiddleware for testing convenience (allows all origins by default).
+- `methods`: A list of HTTP methods to be supported (e.g. ”GET”, POST”)
+- `description`: If provided, overrides everything else and is used directly as the endpoint description for the OpenAPI spec
+- `generate_description`: If set to `True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+
+By default (if neither `description` nor `generate_description` are provided), the description is fetched from the docstring. If there's no docstring, AutoPlugin falls back to generating one automatically.
+
+
+### The `generate` Function
 
-## The `generate` Function
 The `generate` function has the following signature:
+
+```python
+def generate(app: FastAPI, version="v1", out_dir=".well-known",
+             overwrite_plugin_spec=True, overwrite_openapi_spec=True,
+             name="", description="",
+             **kwargs)
+```
+
+- `app`: Your FastAPI application again.
+- `version="v1"`: What version number to pass to both the plugin and OpenAPI specs.
+- `out_dir=".well-known"`: The directory to save both files to.
+- `overwrite_plugin_spec=True`: If set to False, does not overwrite `ai-plugin.json` if it already exists.
+- `overwrite_openapi_spec=True`: If set to False, does not overwrite `openapi.yaml` if it already exists.
+- `name=""`: If specified, used for both `name_for_human` and `name_for_model`.
+- `description=""`: If specified, used for both `description_for_human` and `description_for_model`. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `**kwargs`: All other keyword arguments are passed on to `ai-plugin.json` directly. See the full list of possible options [here](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+
+
+### The `launch` Function
+
+The `launch` function has the following signature:
+
 ```python
-def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+def launch(app: FastAPI, host="127.0.0.1", port=8000):
 ```
-The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
 
-All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
-The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+- `app`: Still your FastAPI application.
+- `host="127.0.0.1"`: the host to launch the server on
+- `port=8000`: the port to launch the server on
 
 
-## Testing
+### Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
 
 def test_api():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoplugin-0.1.4/setup.py` & `autoplugin-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autoplugin",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "fastapi",
         "pydantic",
         "uvicorn",
         "requests",
         "PyYAML",
```

