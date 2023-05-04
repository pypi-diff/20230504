# Comparing `tmp/graphql_http_server-1.4.5.tar.gz` & `tmp/graphql_http_server-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.5.tar", last modified: Mon Apr 24 10:02:10 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.6.tar", last modified: Thu May  4 16:12:25 2023, max compression
```

## Comparing `graphql_http_server-1.4.5.tar` & `graphql_http_server-1.4.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 10:02:10.457164 graphql_http_server-1.4.5/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 10:02:10.457164 graphql_http_server-1.4.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 10:02:09.000000 graphql_http_server-1.4.5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 10:02:10.453163 graphql_http_server-1.4.5/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 10:02:10.455164 graphql_http_server-1.4.5/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9365 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 10:02:10.454163 graphql_http_server-1.4.5/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 10:02:10.000000 graphql_http_server-1.4.5/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-24 10:02:10.000000 graphql_http_server-1.4.5/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 10:02:10.000000 graphql_http_server-1.4.5/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-24 10:02:10.000000 graphql_http_server-1.4.5/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-24 10:02:10.000000 graphql_http_server-1.4.5/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 10:02:10.457164 graphql_http_server-1.4.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 10:02:10.456164 graphql_http_server-1.4.5/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     2246 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2770 2023-04-24 10:01:59.000000 graphql_http_server-1.4.5/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.774419 graphql_http_server-1.4.6/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.776419 graphql_http_server-1.4.6/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6574 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     8905 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.776419 graphql_http_server-1.4.6/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1319 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2211 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.5/LICENSE` & `graphql_http_server-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.5/PKG-INFO` & `graphql_http_server-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.4.5
+Version: 1.4.6
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.5.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.6.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.5/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.6/graphql_http_server/graphiql/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,16 @@
             query: query,
             onEdit: setQuery,
         });
         return React.createElement(GraphiQL, {
             fetcher: GraphiQL.createFetcher({
                 url: fetchURL,
             }),
-            defaultEditorToolsVisibility: true,
+            defaultEditorToolsVisibility: false,
+            headerEditorEnabled: true,
             plugins: [explorerPlugin],
             query: query,
             onEditQuery: setQuery,
             schemaDescription: "test"
         });
     }
```

### Comparing `graphql_http_server-1.4.5/graphql_http_server/helpers.py` & `graphql_http_server-1.4.6/graphql_http_server/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,66 +42,51 @@
     query_data: Optional[Dict] = None,
     batch_enabled: bool = False,
     catch: bool = False,
     allow_post_query: bool = True,
     **execute_options,
 ):
     if not isinstance(schema, GraphQLSchema):
-        raise TypeError(
-            f"Expected a GraphQL schema, but received {schema!r}."
-        )
+        raise TypeError(f"Expected a GraphQL schema, but received {schema!r}.")
     if request_method not in ("get", "post"):
         raise HttpQueryError(
             405,
             "GraphQL only supports GET and POST requests.",
             headers={"Allow": "GET, POST"},
         )
     if catch:
-        catch_exc: Union[Type[HttpQueryError], Type[SkipException]] = \
-            HttpQueryError
+        catch_exc: Union[Type[HttpQueryError], Type[SkipException]] = HttpQueryError
     else:
         catch_exc = SkipException
     is_batch = isinstance(data, list)
 
     is_get_request = request_method == "get"
     allow_only_query = is_get_request and not allow_post_query
 
     if not is_batch:
         if not isinstance(data, (dict, MutableMapping)):
             raise HttpQueryError(
                 400, f"GraphQL params should be a dict. Received {data!r}."
             )
         data = [data]
     elif not batch_enabled:
-        raise HttpQueryError(
-            400,
-            "Batch GraphQL requests are not enabled."
-        )
+        raise HttpQueryError(400, "Batch GraphQL requests are not enabled.")
 
     if not data:
-        raise HttpQueryError(
-            400,
-            "Received an empty list in the batch request."
-        )
+        raise HttpQueryError(400, "Received an empty list in the batch request.")
 
     extra_data: Dict[str, Any] = {}
     # If is a batch request, we don't consume the data from the query
     if not is_batch:
         extra_data = query_data or {}
 
     all_params = [get_graphql_params(entry, extra_data) for entry in data]
 
     responses = [
-        get_response(
-            schema,
-            params,
-            catch_exc,
-            allow_only_query,
-            **execute_options
-        )
+        get_response(schema, params, catch_exc, allow_only_query, **execute_options)
         for params in all_params
     ]
 
     return responses, all_params
 
 
 def json_encode(data: Union[Dict, List], pretty: bool = False) -> str:
@@ -113,17 +98,17 @@
 
 def encode_execution_results(
     execution_results: List[Optional[ExecutionResult]],
     format_error: Callable[[Exception], Dict] = None,
     is_batch: bool = False,
     encode: Callable[[Dict], Any] = json_encode,
 ) -> Tuple[Any, int]:
-
     if not format_error:
         from graphql_http_server import GraphQLHTTPServer
+
         format_error = GraphQLHTTPServer.format_error
 
     responses = [
         format_execution_result(execution_result, format_error)
         for execution_result in execution_results
     ]
     result, status_codes = zip(*responses)
@@ -131,30 +116,27 @@
 
     if not is_batch:
         result = result[0]
 
     return encode(result), status_code
 
 
-def load_json_variables(
-    variables: Optional[Union[str, Dict]]
-) -> Optional[Dict]:
+def load_json_variables(variables: Optional[Union[str, Dict]]) -> Optional[Dict]:
     if variables and isinstance(variables, str):
         try:
             return json.loads(variables)
         except Exception:
             raise HttpQueryError(400, "Variables are invalid JSON.")
     return variables  # type: ignore
 
 
 def get_graphql_params(data: Dict, query_data: Dict) -> GraphQLParams:
     query = data.get("query") or query_data.get("query")
     variables = data.get("variables") or query_data.get("variables")
-    operation_name = data.get("operationName") or \
-        query_data.get("operationName")
+    operation_name = data.get("operationName") or query_data.get("operationName")
 
     return GraphQLParams(query, load_json_variables(variables), operation_name)
 
 
 def get_response(
     schema: GraphQLSchema,
     params: GraphQLParams,
@@ -174,22 +156,21 @@
 
 def format_execution_result(
     execution_result: Optional[ExecutionResult],
     format_error: Optional[Callable[[Exception], Dict]] = None,
 ) -> GraphQLResponse:
     if not format_error:
         from graphql_http_server import GraphQLHTTPServer
+
         format_error = GraphQLHTTPServer.format_error
 
     if execution_result:
         response = {}
         if execution_result.errors:
-            response["errors"] = [
-                format_error(e) for e in execution_result.errors
-            ]
+            response["errors"] = [format_error(e) for e in execution_result.errors]
         if execution_result.data:
             response["data"] = execution_result.data
         status_code = 200
 
     else:
         response = None
         status_code = 200
@@ -242,8 +223,8 @@
     )
 
 
 def load_json_body(data: str) -> Union[Dict, List]:
     try:
         return json.loads(data)
     except Exception:
-        raise HttpQueryError(400, "POST body sent invalid JSON.")
+        raise HttpQueryError(400, f"POST body sent invalid JSON. {data}")
```

### Comparing `graphql_http_server-1.4.5/graphql_http_server/server.py` & `graphql_http_server-1.4.6/graphql_http_server/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,68 +13,58 @@
 from graphql.execution.execute import ExecutionContext
 
 from graphql_http_server.helpers import (
     HttpQueryError,
     encode_execution_results,
     json_encode,
     load_json_body,
-    run_http_query
+    run_http_query,
 )
 
 
 def run_simple(
-        schema,
-        root_value: Any = None,
-        middleware: List[Callable[[Callable, Any], Any]] = None,
-        hostname: str = None,
-        port: int = None,
-        **kwargs
+    schema,
+    root_value: Any = None,
+    middleware: List[Callable[[Callable, Any], Any]] = None,
+    hostname: str = None,
+    port: int = None,
+    **kwargs
 ):
     return GraphQLHTTPServer.from_api(
-        schema=schema,
-        root_value=root_value,
-        middleware=middleware,
-        **kwargs
-    ).run(
-        hostname=hostname,
-        port=port,
-        **kwargs
-    )
+        schema=schema, root_value=root_value, middleware=middleware, **kwargs
+    ).run(hostname=hostname, port=port, **kwargs)
 
 
-graphiql_dir = os.path.join(os.path.dirname(__file__), 'graphiql')
+graphiql_dir = os.path.join(os.path.dirname(__file__), "graphiql")
 
 
 class GraphQLHTTPServer:
-
     @classmethod
     def from_api(
-            cls,
-            api,
-            root_value: Any = None,
-            middleware: List[Callable[[Callable, Any], Any]] = None,
-            middleware_on_introspection: bool = False,
-            **kwargs
-    ) -> 'GraphQLHTTPServer':
+        cls,
+        api,
+        root_value: Any = None,
+        middleware: List[Callable[[Callable, Any], Any]] = None,
+        middleware_on_introspection: bool = False,
+        **kwargs
+    ) -> "GraphQLHTTPServer":
         try:
             from graphql_api import GraphQLAPI, GraphQLExecutor
             from graphql_api.context import GraphQLContext
 
         except ImportError:
-            raise ImportError(
-                'GraphQLAPI is not installed.'
-            )
+            raise ImportError("GraphQLAPI is not installed.")
 
         api: GraphQLAPI = api
 
         executor = api.executor(
             root_value=root_value,
             middleware=middleware,
             middleware_on_introspection=middleware_on_introspection,
-            error_protection=api.error_protection
+            error_protection=api.error_protection,
         )
 
         schema: GraphQLSchema = executor.schema
         meta = executor.meta
         root_value = executor.root_value
 
         middleware = GraphQLExecutor.adapt_middleware(executor.middleware)
@@ -86,27 +76,26 @@
             middleware=middleware,
             context=context,
             execution_context_class=executor.execution_context_class,
             **kwargs
         )
 
     def __init__(
-            self,
-            schema: GraphQLSchema,
-            root_value: Any = None,
-            middleware: List[Callable[[Callable, Any], Any]] = None,
-            context: Any = None,
-            serve_graphiql: bool = True,
-            graphiql_default_query: str = None,
-            graphiql_default_variables: str = None,
-            allow_cors: bool = False,
-            health_path: str = None,
-            execution_context_class: Optional[Type[ExecutionContext]] = None
+        self,
+        schema: GraphQLSchema,
+        root_value: Any = None,
+        middleware: List[Callable[[Callable, Any], Any]] = None,
+        context: Any = None,
+        serve_graphiql: bool = True,
+        graphiql_default_query: str = None,
+        graphiql_default_variables: str = None,
+        allow_cors: bool = False,
+        health_path: str = None,
+        execution_context_class: Optional[Type[ExecutionContext]] = None,
     ):
-
         if middleware is None:
             middleware = []
 
         self.schema = schema
         self.root_value = root_value
         self.middleware = middleware
         self.context = context
@@ -123,18 +112,18 @@
     @staticmethod
     def format_error(error: GraphQLError) -> {}:
         return error.formatted
 
     encode = staticmethod(json_encode)
 
     def dispatch(
-            self,
-            request: Request,
-            context=None,
-            execution_context_class: ExecutionContext = None
+        self,
+        request: Request,
+        context=None,
+        execution_context_class: ExecutionContext = None,
     ) -> Response:
         headers = {}
 
         if execution_context_class is None:
             execution_context_class = self.execution_context_class
 
         try:
@@ -143,167 +132,151 @@
 
             if self.health_path and request.path == self.health_path:
                 return Response("OK")
 
             if context is None:
                 context = self.create_context()
 
-            is_get = request_method == 'get'
+            is_get = request_method == "get"
             should_serve = self.should_serve_graphiql(request=request)
 
             show_graphiql = is_get and should_serve
             if show_graphiql:
-                graphiql_path = os.path.join(
-                    graphiql_dir,
-                    'index.html'
-                )
+                graphiql_path = os.path.join(graphiql_dir, "index.html")
                 if self.graphiql_default_query:
                     default_query = json.dumps(self.graphiql_default_query)
                 else:
                     default_query = '""'
 
                 if self.graphiql_default_variables:
-                    default_variables = json.dumps(
-                        self.graphiql_default_variables
-                    )
+                    default_variables = json.dumps(self.graphiql_default_variables)
                 else:
                     default_variables = '""'
 
-                html = open(graphiql_path, 'r').read()
-                html = html.replace('DEFAULT_QUERY', default_query)
-                html = html.replace('DEFAULT_VARIABLES', default_variables)
+                html = open(graphiql_path, "r").read()
+                html = html.replace("DEFAULT_QUERY", default_query)
+                html = html.replace("DEFAULT_VARIABLES", default_variables)
 
-                return Response(html, content_type='text/html')
+                return Response(html, content_type="text/html")
 
             if self.allow_cors:
                 headers = {
                     "Access-Control-Allow-Credentials": "true",
                     "Access-Control-Allow-Headers": "Content-Type",
-                    "Access-Control-Allow-Methods": "GET, POST"
+                    "Access-Control-Allow-Methods": "GET, POST",
                 }
-                origin = request.headers.get('ORIGIN')
+                origin = request.headers.get("ORIGIN")
                 if origin:
                     headers["Access-Control-Allow-Origin"] = origin
 
                 if request_method == "options":
                     return Response(response="OK", headers=headers)
 
             execution_results, all_params = run_http_query(
                 self.schema,
                 request_method,
                 data,
                 query_data=request.args,
                 root_value=self.root_value,
                 middleware=self.middleware,
                 context_value=context,
-                execution_context_class=execution_context_class
+                execution_context_class=execution_context_class,
             )
             result, status_code = encode_execution_results(
-                execution_results,
-                is_batch=isinstance(data, list),
-                encode=self.encode
+                execution_results, is_batch=isinstance(data, list), encode=self.encode
             )
 
             return Response(
                 result,
                 status=status_code,
-                content_type='application/json',
-                headers=headers
+                content_type="application/json",
+                headers=headers,
             )
 
         except HttpQueryError as e:
             return self.error_response(e, headers)
 
     def error_response(self, e, headers=None):
         if headers is None:
             headers = {}
         return Response(
-            self.encode({
-                'errors': [str(e)]
-            }),
+            self.encode({"errors": [str(e)]}),
             status=getattr(e, "status_code", 200),
             headers={**(getattr(e, "headers", {}) or {}), **headers},
-            content_type='application/json'
+            content_type="application/json",
         )
 
     # noinspection PyMethodMayBeStatic
     def parse_body(self, request):
         content_type = request.mimetype
-        if content_type == 'application/graphql':
-            return {'query': request.data.decode('utf8')}
+        if content_type == "application/graphql":
+            return {"query": request.data.decode("utf8")}
 
-        elif content_type == 'application/json':
-            return load_json_body(request.data.decode('utf8'))
+        elif content_type == "application/json":
+            return load_json_body(request.data.decode("utf8"))
 
         elif content_type in (
-                'application/x-www-form-urlencoded',
-                'multipart/form-data'
+            "application/x-www-form-urlencoded",
+            "multipart/form-data",
         ):
             return request.form
 
         if request.data:
             try:
-                body = request.data.decode('utf8')
+                body = request.data.decode("utf8")
                 return load_json_body(body)
             except Exception:
-                return {'query': request.data.decode('utf8')}
+                return {"query": request.data.decode("utf8")}
 
         return {}
 
     def should_serve_graphiql(self, request):
-        if not self.serve_graphiql or 'raw' in request.args:
+        if not self.serve_graphiql or "raw" in request.args:
             return False
 
         return self.request_wants_html(request=request)
 
     # noinspection PyMethodMayBeStatic
     def request_wants_html(self, request):
-        best = request.accept_mimetypes \
-            .best_match(['application/json', 'text/html'])
+        best = request.accept_mimetypes.best_match(["application/json", "text/html"])
 
-        if best == 'text/html':
+        if best == "text/html":
             accept_best = request.accept_mimetypes[best]
-            accept_json = request.accept_mimetypes['application/json']
+            accept_json = request.accept_mimetypes["application/json"]
             return accept_best > accept_json
 
         return False
 
-    def app(
-            self,
-            main: Callable[[Request], Response] = None
-    ):
+    def app(self, main: Callable[[Request], Response] = None):
         @Request.application
         def app(request):
             if main is not None:
                 return main(request)
             return self.dispatch(request=request)
 
         return app
 
     def client(self, main=None):
         return Client(self.app(main=main), Response)
 
     def run(
-            self,
-            main: Callable[[Request], Response] = None,
-            hostname: str = None,
-            port: int = None,
-            **kwargs
+        self,
+        main: Callable[[Request], Response] = None,
+        hostname: str = None,
+        port: int = None,
+        **kwargs
     ):
         if hostname is None:
-            hostname = 'localhost'
+            hostname = "localhost"
 
         if port is None:
             port = 5000
 
         from werkzeug.serving import run_simple
 
         valid_arg_names = list(signature(run_simple).parameters)
 
         kwargs = {k: v for k, v in kwargs.items() if k in valid_arg_names}
 
         run_simple(
-            hostname=hostname,
-            port=port,
-            application=self.app(main=main),
-            **kwargs
+            hostname=hostname, port=port, application=self.app(main=main), **kwargs
         )
```

### Comparing `graphql_http_server-1.4.5/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.6/graphql_http_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.4.5
+Version: 1.4.6
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.5.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.6.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.5/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.6/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.5/setup.py` & `graphql_http_server-1.4.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import io
 
 from setuptools import setup, find_packages
 
-with io.open('README.md', 'rt', encoding='utf8') as f:
+with io.open("README.md", "rt", encoding="utf8") as f:
     readme = f.read()
 
-with io.open('VERSION') as version_file:
+with io.open("VERSION") as version_file:
     version = version_file.read().strip().lower()
     if version.startswith("v"):
         version = version[1:]
 
 setup(
-    name='graphql_http_server',
+    name="graphql_http_server",
     version=version,
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
     include_package_data=True,
-    author='Robert Parker',
-    author_email='rob@parob.com',
-    url='https://gitlab.com/parob/graphql-http-server',
-    download_url=f'https://gitlab.com/parob/graphql-http-server/-/'
-                 f'archive/master/graphql-http-server-v{version}.zip',
-    keywords=['GraphQL', 'HTTPServer', 'werkzeug'],
-    description='HTTPServer for GraphQL.',
+    author="Robert Parker",
+    author_email="rob@parob.com",
+    url="https://gitlab.com/parob/graphql-http-server",
+    download_url=f"https://gitlab.com/parob/graphql-http-server/-/"
+    f"archive/master/graphql-http-server-v{version}.zip",
+    keywords=["GraphQL", "HTTPServer", "werkzeug"],
+    description="HTTPServer for GraphQL.",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     install_requires=[
         "graphql-core>=3.2.0",
         "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
-        "graphql-schema-diff>=1.2.4"
+        "graphql-schema-diff>=1.2.4",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ]
+    ],
 )
```

### Comparing `graphql_http_server-1.4.5/tests/test_app.py` & `graphql_http_server-1.4.6/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,68 +6,64 @@
 from werkzeug.test import EnvironBuilder
 from werkzeug.wrappers import Request
 
 from graphql_http_server import GraphQLHTTPServer
 
 
 class TestApp:
-
     def test_dispatch(self, schema):
         server = GraphQLHTTPServer(schema=schema)
 
-        builder = EnvironBuilder(method='GET', query_string="query={hello}")
+        builder = EnvironBuilder(method="GET", query_string="query={hello}")
 
         request = Request(builder.get_environ())
         response = server.dispatch(request=request)
 
         assert response.status_code == 200
         assert response.data == b'{"data":{"hello":"world"}}'
 
     def test_app(self, schema):
         server = GraphQLHTTPServer(schema=schema)
-        response = server.client().get('/?query={hello}')
+        response = server.client().get("/?query={hello}")
 
         assert response.status_code == 200
         assert response.data == b'{"data":{"hello":"world"}}'
 
     def test_app_post(self, schema):
         server = GraphQLHTTPServer(schema=schema)
         response = server.client().post(data='{"query":"{hello}"}')
 
         assert response.status_code == 200
         assert response.data == b'{"data":{"hello":"world"}}'
 
     def test_health_endpoint(self, schema):
         server = GraphQLHTTPServer(schema=schema, health_path="/health")
-        response = server.client().get('/health')
+        response = server.client().get("/health")
 
         assert response.status_code == 200
-        assert response.data == b'OK'
+        assert response.data == b"OK"
 
     def test_graphiql(self, schema):
         server = GraphQLHTTPServer(schema=schema)
-        response = server.client().get('/', headers={"Accept": "text/html"})
+        response = server.client().get("/", headers={"Accept": "text/html"})
 
         assert response.status_code == 200
-        assert b'GraphiQL' in response.data
+        assert b"GraphiQL" in response.data
 
     def test_no_graphiql(self, schema):
         server = GraphQLHTTPServer(schema=schema, serve_graphiql=False)
-        response = server.client().get('/', headers={"Accept": "text/html"})
+        response = server.client().get("/", headers={"Accept": "text/html"})
 
         assert response.status_code == 400
 
     def test_run_app_graphiql(self, schema):
         server = GraphQLHTTPServer(schema=schema)
 
         thread = threading.Thread(target=server.run, daemon=True)
         thread.start()
 
         time.sleep(0.5)
 
-        req = request.Request(
-            "http://localhost:5000",
-            headers={"Accept": "text/html"}
-        )
+        req = request.Request("http://localhost:5000", headers={"Accept": "text/html"})
         response = request.urlopen(req).read()
 
-        assert b'GraphiQL' in response
+        assert b"GraphiQL" in response
```

### Comparing `graphql_http_server-1.4.5/tests/test_graphql_api.py` & `graphql_http_server-1.4.6/tests/test_graphql_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,47 @@
 from requests import request, ConnectTimeout, ReadTimeout
 from graphql_http_server import GraphQLHTTPServer
 
 
 def is_graphql_api_installed():
     try:
         import graphql_api
+
         assert graphql_api
     except ImportError:
         return False
 
     return True
 
 
 def available(url, method="GET"):
     try:
         response = request(
-            method,
-            url,
-            headers={"Accept": "text/html"},
-            timeout=5,
-            verify=False
+            method, url, headers={"Accept": "text/html"}, timeout=5, verify=False
         )
     except (ConnectionError, ConnectTimeout, ReadTimeout):
         return False
 
     if response.status_code == 400 or response.status_code == 200:
         return True
 
     return False
 
 
 @pytest.mark.skipif(
-    not is_graphql_api_installed(),
-    reason="GraphQL-API is not installed"
+    not is_graphql_api_installed(), reason="GraphQL-API is not installed"
 )
 class TestGraphQLAPI:
-
     def test_graphql_api(self):
         from graphql_api import GraphQLAPI
 
         api = GraphQLAPI()
 
         @api.type(root=True)
         class RootQueryType:
-
             @api.field
             def hello(self, name: str) -> str:
                 return f"hey {name}"
 
         server = GraphQLHTTPServer.from_api(api=api)
 
         response = server.client().get('/?query={hello(name:"rob")}')
@@ -63,15 +57,14 @@
     def test_graphql_api_error(self):
         from graphql_api import GraphQLAPI
 
         api = GraphQLAPI()
 
         @api.type(root=True)
         class RootQueryType:
-
             @api.field
             def hello(self, error: bool = True) -> str:
                 if error:
                     raise Exception("hello error")
                 return ""
 
             @api.field
@@ -82,27 +75,23 @@
 
             @api.field({GraphQLMetaKey.error_protection: False})
             def raise_hello(self) -> str:
                 raise Exception("optional hello error")
 
         server = GraphQLHTTPServer.from_api(api=api)
 
-        response = server.client().get('/?query={hello}')
+        response = server.client().get("/?query={hello}")
 
         assert response.status_code == 200
         assert response.json
         assert "data" not in response.json
         assert "errors" in response.json
 
-        response = server.client().get(
-            '/?query={hello(error: false) optionalHello}'
-        )
+        response = server.client().get("/?query={hello(error: false) optionalHello}")
 
         assert response.status_code == 200
         assert response.json
         assert "data" in response.json
         assert "errors" in response.json
 
         with pytest.raises(Exception):
-            server.client().get(
-                '/?query={raiseHello}'
-            )
+            server.client().get("/?query={raiseHello}")
```

