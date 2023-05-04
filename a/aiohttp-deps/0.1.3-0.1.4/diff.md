# Comparing `tmp/aiohttp_deps-0.1.3.tar.gz` & `tmp/aiohttp_deps-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.1.3.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.1.4.tar", max compression
```

## Comparing `aiohttp_deps-0.1.3.tar` & `aiohttp_deps-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/LICENSE
--rw-r--r--   0        0        0     6819 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/README.md
--rw-r--r--   0        0        0      375 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3202 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     7447 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1317 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1766 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8126 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-04 00:28:39.646442 aiohttp_deps-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7669 2023-05-04 00:28:39.646442 aiohttp_deps-0.1.4/README.md
+-rw-r--r--   0        0        0      497 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3202 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0     9364 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0     9138 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1317 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1766 2023-05-04 00:28:39.650442 aiohttp_deps-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9076 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.4/PKG-INFO
```

### Comparing `aiohttp_deps-0.1.3/LICENSE` & `aiohttp_deps-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.3/README.md` & `aiohttp_deps-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,33 @@
 
 main_router = Router()
 
 main_router.add_routes(api_router, prefix="/api")
 main_router.add_routes(memes_router, prefix="/memes")
 ```
 
+## Swagger
+
+If you use dependencies in you handlers, we can easily generate swagger for you.
+We have some limitations:
+1. We don't support string type annotation for detecting required parameters in openapi. Like `a: "Optional[int]"`.
+2. We don't have support for 3.10 style Option annotations. E.G. `int | None`
+
+We will try to fix these limitations later.
+
+To enable swagger, just add it to your startup.
+
+```python
+from aiohttp_deps import init, setup_swagger
+
+app = web.Application()
+
+app.on_startup.extend([init, setup_swagger()])
+```
+
 
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
@@ -205,15 +224,15 @@
 And, of course, you can provide this dependency with default value if the value from user cannot be parsed for some reason.
 
 ```python
 def decode_token(meme_id: str = Depends(Header(default="not-a-secret"))) -> str:
 ```
 
 
-# Queries
+## Queries
 
 You can depend on `Query` to get and parse query parameters.
 
 ```python
 from aiohttp_deps import Router, Query, Depends
 from aiohttp import web
 
@@ -274,7 +293,24 @@
 @router.post("/")
 async def handler(my_form: MyForm = Depends(Form())):
     with open("my_file", "wb") as f:
         f.write(my_form.file.file.read())
     return web.json_response({"id": my_form.id})
 
 ```
+
+## Path
+
+If you have path variables, you can also inject them in your handler.
+
+```python
+from aiohttp_deps import Router, Path, Depends
+from aiohttp import web
+
+router = Router()
+
+
+@router.get("/view/{var}")
+async def my_handler(var: str = Depends(Path())):
+    return web.json_response({"var": var})
+
+```
```

### Comparing `aiohttp_deps-0.1.3/aiohttp_deps/initializer.py` & `aiohttp_deps-0.1.4/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.3/aiohttp_deps/router.py` & `aiohttp_deps-0.1.4/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.3/aiohttp_deps/router.pyi` & `aiohttp_deps-0.1.4/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.3/aiohttp_deps/utils.py` & `aiohttp_deps-0.1.4/aiohttp_deps/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 
     def __init__(
         self,
         default: Any = ...,
         *,
         alias: Optional[str] = None,
         multiple: bool = False,
+        description: str = "",
     ):
         self.default = default
         self.alias = alias
         self.multiple = multiple
+        self.description = description
 
     def __call__(  # noqa: C901, WPS210
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
@@ -52,15 +54,15 @@
 
         if self.multiple:
             value = request.headers.getall(header_name, default_value)
         else:
             value = request.headers.getone(header_name, default_value)
 
         definition = None
-        if (  # noqa: WPS337
+        if (
             param_info.definition
             and param_info.definition.annotation != inspect.Parameter.empty
         ):
             definition = param_info.definition.annotation
 
         if definition is None:
             return value
@@ -104,15 +106,15 @@
         """
         try:
             body = await request.json()
         except ValueError:
             body = None
 
         definition = None
-        if (  # noqa: WPS337
+        if (
             param_info.definition
             and param_info.definition.annotation != inspect.Parameter.empty
         ):
             definition = param_info.definition.annotation
 
         if definition is None:
             return body
@@ -144,18 +146,20 @@
 
     def __init__(
         self,
         default: Any = ...,
         *,
         alias: Optional[str] = None,
         multiple: bool = False,
+        description: str = "",
     ):
         self.default = default
         self.alias = alias
         self.multiple = multiple
+        self.description = description
 
     def __call__(  # noqa: C901, WPS210
         self,
         param_info: ParamInfo = Depends(),
         request: web.Request = Depends(),
     ) -> Any:
         """
@@ -174,15 +178,15 @@
 
         if self.multiple:
             value = request.query.getall(param_name, default_value)
         else:
             value = request.query.getone(param_name, default_value)
 
         definition = None
-        if (  # noqa: WPS337
+        if (
             param_info.definition
             and param_info.definition.annotation != inspect.Parameter.empty
         ):
             definition = param_info.definition.annotation
 
         if definition is None:
             return value
@@ -224,15 +228,15 @@
             was defined with name and type.
         :param request: current request.
         :raises HTTPBadRequest: if incorrect data was found.
         :return: parsed data.
         """
         form_data = await request.post()
         definition = None
-        if (  # noqa: WPS337
+        if (
             param_info.definition
             and param_info.definition.annotation != inspect.Parameter.empty
         ):
             definition = param_info.definition.annotation
 
         if definition is None:
             return form_data
@@ -243,7 +247,64 @@
             errors = err.errors()
             for error in errors:
                 error["loc"] = ("form",) + error["loc"]
             raise web.HTTPBadRequest(
                 headers={"Content-Type": "application/json"},
                 text=json.dumps(errors),
             )
+
+
+class Path:
+    """
+    Get path parameter.
+
+    This class takes a path parameter
+    from request and tries to parse it
+    in target type.
+    """
+
+    def __init__(
+        self,
+        default: Any = ...,
+        *,
+        alias: Optional[str] = None,
+        description: str = "",
+    ) -> None:
+        self.default = default
+        self.alias = alias
+        self.description = description
+
+    def __call__(
+        self,
+        param_info: ParamInfo = Depends(),
+        request: web.Request = Depends(),
+    ) -> Any:
+        """
+        Performs actual logic, described above.
+
+        :param param_info: information about how the dependency
+            was defined with name and type.
+        :param request: current request.
+        :raises HTTPBadRequest: if incorrect data was found.
+        :return: parsed data.
+        """
+        matched_data = request.match_info.get(self.alias or param_info.name)
+        definition = None
+        if (
+            param_info.definition
+            and param_info.definition.annotation != inspect.Parameter.empty
+        ):
+            definition = param_info.definition.annotation
+
+        if definition is None:
+            return matched_data
+
+        try:
+            return pydantic.parse_obj_as(definition, matched_data)
+        except pydantic.ValidationError as err:
+            errors = err.errors()
+            for error in errors:
+                error["loc"] = ("path",) + error["loc"]
+            raise web.HTTPBadRequest(
+                headers={"Content-Type": "application/json"},
+                text=json.dumps(errors),
+            )
```

### Comparing `aiohttp_deps-0.1.3/aiohttp_deps/view.py` & `aiohttp_deps-0.1.4/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.3/pyproject.toml` & `aiohttp_deps-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -20,15 +20,15 @@
     "Topic :: System :: Networking",
     "Development Status :: 3 - Alpha",
 ]
 keywords = ["aiohttp", "taskiq-dependencies"]
 homepage = "https://github.com/taskiq-python/aiohttp-deps"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.7"
 aiohttp = "^3"
 taskiq-dependencies = "^1"
 pydantic = "^1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
```

### Comparing `aiohttp_deps-0.1.3/PKG-INFO` & `aiohttp_deps-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
@@ -95,14 +97,33 @@
 
 main_router = Router()
 
 main_router.add_routes(api_router, prefix="/api")
 main_router.add_routes(memes_router, prefix="/memes")
 ```
 
+## Swagger
+
+If you use dependencies in you handlers, we can easily generate swagger for you.
+We have some limitations:
+1. We don't support string type annotation for detecting required parameters in openapi. Like `a: "Optional[int]"`.
+2. We don't have support for 3.10 style Option annotations. E.G. `int | None`
+
+We will try to fix these limitations later.
+
+To enable swagger, just add it to your startup.
+
+```python
+from aiohttp_deps import init, setup_swagger
+
+app = web.Application()
+
+app.on_startup.extend([init, setup_swagger()])
+```
+
 
 ## Default dependencies
 
 By default this library provides only two injectables. `web.Request` and `web.Application`.
 
 ```python
 
@@ -239,15 +260,15 @@
 And, of course, you can provide this dependency with default value if the value from user cannot be parsed for some reason.
 
 ```python
 def decode_token(meme_id: str = Depends(Header(default="not-a-secret"))) -> str:
 ```
 
 
-# Queries
+## Queries
 
 You can depend on `Query` to get and parse query parameters.
 
 ```python
 from aiohttp_deps import Router, Query, Depends
 from aiohttp import web
 
@@ -309,7 +330,24 @@
 async def handler(my_form: MyForm = Depends(Form())):
     with open("my_file", "wb") as f:
         f.write(my_form.file.file.read())
     return web.json_response({"id": my_form.id})
 
 ```
 
+## Path
+
+If you have path variables, you can also inject them in your handler.
+
+```python
+from aiohttp_deps import Router, Path, Depends
+from aiohttp import web
+
+router = Router()
+
+
+@router.get("/view/{var}")
+async def my_handler(var: str = Depends(Path())):
+    return web.json_response({"var": var})
+
+```
+
```

