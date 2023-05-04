# Comparing `tmp/plugnplai-0.0.4.tar.gz` & `tmp/plugnplai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugnplai-0.0.4.tar", max compression
+gzip compressed data, was "plugnplai-0.0.5.tar", max compression
```

## Comparing `plugnplai-0.0.4.tar` & `plugnplai-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-25 18:31:47.487043 plugnplai-0.0.4/LICENSE
--rw-r--r--   0        0        0     1413 2023-04-25 18:31:47.501043 plugnplai-0.0.4/README.md
--rw-r--r--   0        0        0      466 2023-04-25 18:31:47.503043 plugnplai-0.0.4/plugnplai/__init__.py
--rw-r--r--   0        0        0     4889 2023-04-25 18:31:47.504043 plugnplai-0.0.4/plugnplai/call_api.py
--rw-r--r--   0        0        0     5036 2023-04-25 18:31:47.506043 plugnplai-0.0.4/plugnplai/load.py
--rw-r--r--   0        0        0     5755 2023-04-25 18:31:47.510043 plugnplai-0.0.4/plugnplai/plugin.py
--rw-r--r--   0        0        0      400 2023-04-25 18:34:06.560053 plugnplai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 plugnplai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 18:31:47.487043 plugnplai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1935 2023-05-04 06:13:47.475045 plugnplai-0.0.5/README.md
+-rw-r--r--   0        0        0      466 2023-04-25 18:31:47.503043 plugnplai-0.0.5/plugnplai/__init__.py
+-rw-r--r--   0        0        0     4889 2023-04-25 18:31:47.504043 plugnplai-0.0.5/plugnplai/call_api.py
+-rw-r--r--   0        0        0     5599 2023-05-04 06:15:01.990050 plugnplai-0.0.5/plugnplai/load.py
+-rw-r--r--   0        0        0     5755 2023-04-25 18:31:47.510043 plugnplai-0.0.5/plugnplai/plugin.py
+-rw-r--r--   0        0        0      400 2023-05-04 06:17:03.779060 plugnplai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 plugnplai-0.0.5/PKG-INFO
```

### Comparing `plugnplai-0.0.4/LICENSE` & `plugnplai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.4/README.md` & `plugnplai-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,55 @@
-# 🎸 Plug and PLAI
+# 🎸 Plug and Plai
 
-Plug and PlAI is an open source library that allows you to manage AI plugins. It provides utility functions to load available plugins, get plugin manifests, and extract OpenAPI specifications.
+Plug and Plai is an open source library aiming to simplify the integration of AI plugins into open-source language models (LLMs). 
+
+It provides utility functions to get a list of active plugins from [plugnplai.com](https://plugnplai.com/) directory, get plugin manifests, and extract OpenAPI specifications and load plugins.
 
 ## Installation
 
 You can install Plug and PlAI using pip:
 
-`pip install plugnplai`
+```python
+pip install plugnplai
+```
 
 ## Usage
 
 ### Utility Functions
 
 The following utility functions are available in the library:
 
 - `get_plugins(endpoint)`: Get a list of available plugins from a [plugins repository](https://www.plugplai.com/).
 - `get_plugin_manifest(url)`: Get the AI plugin manifest from the specified plugin URL.
 - `get_openapi_url(url, manifest)`: Get the OpenAPI URL from the plugin manifest.
 - `get_openapi_spec(openapi_url)`: Get the OpenAPI specification from the specified OpenAPI URL.
-- `from_url(url)`: Returns the Manifest and OpenAPI specification from the plugin URL.
+- `spec_from_url(url)`: Returns the Manifest and OpenAPI specification from the plugin URL.
 
 ### Example
 
 Here is an example of how to use the utility functions:
 
 ```python
 import plugnplai
 
-# Get a list of available plugins
-plugins = plugnplai.get_plugins()
+# Get all plugins from plugnplai.com
+urls = plugnplai.get_plugins()
+
+#  Get ChatGPT plugins - only ChatGPT verified plugins
+urls = plugnplai.get_plugins(filter = 'ChatGPT')
+
+#  Get working plugins - only tested plugins (in progress)
+urls = plugnplai.get_plugins(filter = 'working')
+
 
 # Get the Manifest and the OpenAPI specification from the plugin URL 
 manifest, openapi_spec = spec_from_url(plugins[0])
 ```
 
+## Contributing
+
+Plug and Plai is an open source library, and we welcome contributions from the entire community. If you're interested in contributing to the project, please feel free to fork, submit pull requests, report issues, or suggest new features.
+
 ## Links
 
-- GitHub Repository: [https://github.com/edreisMD/plugnplai](https://github.com/edreisMD/plugnplai)
-- Plugins database: [https://plugplai.com/](https://plugplai.com/)
-- Database API: [https://plugnplai.github.io/](https://plugnplai.github.io/)
+- Plugins directory: [https://plugplai.com/](https://plugplai.com/)
+- API reference: [https://plugnplai.github.io/](https://plugnplai.github.io/)
```

### Comparing `plugnplai-0.0.4/plugnplai/call_api.py` & `plugnplai-0.0.5/plugnplai/call_api.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.4/plugnplai/load.py` & `plugnplai-0.0.5/plugnplai/load.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,41 @@
 
 import jsonref
 import requests
 import yaml
 
 
 def get_plugins(
-    filter: str = None, base_url: str = "https://www.plugplai.com/_functions/getUrls"
+    filter: str = None, provider: str = "plugnplai"
 ):
-    # Construct the endpoint URL based on the filter argument
-    if filter in ["working", "ChatGPT"]:
-        url = f'{base_url.strip("/")}/{filter}'
-    else:
-        url = base_url
-    # Make the HTTP GET request
-    response = requests.get(url)
-    # Check if the response status code is successful (200 OK)
-    if response.status_code == 200:
-        # Parse the JSON response and return the result
-        return response.json()
-    else:
-        # Handle unsuccessful responses
-        return f"An error occurred: {response.status_code} {response.reason}"
-
+    if provider == "plugnplai":
+        base_url = "https://www.plugnplai.com/_functions/getUrls"
+        # Construct the endpoint URL based on the filter argument
+        if filter in ["working", "ChatGPT"]:
+            url = f'{base_url.strip("/")}/{filter}'
+        else:
+            url = base_url
+        # Make the HTTP GET request
+        response = requests.get(url)
+        # Check if the response status code is successful (200 OK)
+        if response.status_code == 200:
+            # Parse the JSON response and return the result
+            return response.json()
+        else:
+            # Handle unsuccessful responses
+            return f"An error occurred: {response.status_code} {response.reason}"
+    elif provider == "pluginso":
+        url = "https://plugin.so/api/plugins/list"
+        response = requests.get(url)
+        if response.status_code == 200:
+                # Parse the JSON response and return the result
+            return [f"https://{entry['domain']}" for entry in response.json()]
+        else:
+            # Handle unsuccessful responses
+            return f"An error occurred: {response.status_code} {response.reason}"
 
 # given a plugin url, get the ai-plugin.json manifest, in "/.well-known/ai-plugin.json"
 def get_plugin_manifest(url: str):
     urlJson = os.path.join(url, ".well-known/ai-plugin.json")
     response = requests.get(urlJson).json()
     return response
```

### Comparing `plugnplai-0.0.4/plugnplai/plugin.py` & `plugnplai-0.0.5/plugnplai/plugin.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.4/PKG-INFO` & `plugnplai-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,73 @@
 Metadata-Version: 2.1
 Name: plugnplai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Connect plugins to AI
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
-# 🎸 Plug and PLAI
+# 🎸 Plug and Plai
 
-Plug and PlAI is an open source library that allows you to manage AI plugins. It provides utility functions to load available plugins, get plugin manifests, and extract OpenAPI specifications.
+Plug and Plai is an open source library aiming to simplify the integration of AI plugins into open-source language models (LLMs). 
+
+It provides utility functions to get a list of active plugins from [plugnplai.com](https://plugnplai.com/) directory, get plugin manifests, and extract OpenAPI specifications and load plugins.
 
 ## Installation
 
 You can install Plug and PlAI using pip:
 
-`pip install plugnplai`
+```python
+pip install plugnplai
+```
 
 ## Usage
 
 ### Utility Functions
 
 The following utility functions are available in the library:
 
 - `get_plugins(endpoint)`: Get a list of available plugins from a [plugins repository](https://www.plugplai.com/).
 - `get_plugin_manifest(url)`: Get the AI plugin manifest from the specified plugin URL.
 - `get_openapi_url(url, manifest)`: Get the OpenAPI URL from the plugin manifest.
 - `get_openapi_spec(openapi_url)`: Get the OpenAPI specification from the specified OpenAPI URL.
-- `from_url(url)`: Returns the Manifest and OpenAPI specification from the plugin URL.
+- `spec_from_url(url)`: Returns the Manifest and OpenAPI specification from the plugin URL.
 
 ### Example
 
 Here is an example of how to use the utility functions:
 
 ```python
 import plugnplai
 
-# Get a list of available plugins
-plugins = plugnplai.get_plugins()
+# Get all plugins from plugnplai.com
+urls = plugnplai.get_plugins()
+
+#  Get ChatGPT plugins - only ChatGPT verified plugins
+urls = plugnplai.get_plugins(filter = 'ChatGPT')
+
+#  Get working plugins - only tested plugins (in progress)
+urls = plugnplai.get_plugins(filter = 'working')
+
 
 # Get the Manifest and the OpenAPI specification from the plugin URL 
 manifest, openapi_spec = spec_from_url(plugins[0])
 ```
 
+## Contributing
+
+Plug and Plai is an open source library, and we welcome contributions from the entire community. If you're interested in contributing to the project, please feel free to fork, submit pull requests, report issues, or suggest new features.
+
 ## Links
 
-- GitHub Repository: [https://github.com/edreisMD/plugnplai](https://github.com/edreisMD/plugnplai)
-- Plugins database: [https://plugplai.com/](https://plugplai.com/)
-- Database API: [https://plugnplai.github.io/](https://plugnplai.github.io/)
+- Plugins directory: [https://plugplai.com/](https://plugplai.com/)
+- API reference: [https://plugnplai.github.io/](https://plugnplai.github.io/)
```

