# Comparing `tmp/django_channels_graphql_ws-1.0.0rc3.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_channels_graphql_ws-1.0.0rc3.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc4.tar", max compression
```

## Comparing `django_channels_graphql_ws-1.0.0rc3.tar` & `django_channels_graphql_ws-1.0.0rc4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10111 2023-05-02 12:50:55.309876 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/client.py
--rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/dict_as_object.py
--rw-r--r--   0        0        0    56638 2023-05-02 20:35:56.015983 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    16451 2023-05-02 12:50:55.311452 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4816 2023-05-02 12:50:55.311701 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     8478 2023-05-02 20:43:08.691294 django_channels_graphql_ws-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10111 2023-05-02 12:50:55.309876 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    53350 2023-05-04 09:11:03.427948 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16451 2023-05-02 12:50:55.311452 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4816 2023-05-02 12:50:55.311701 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8478 2023-05-04 09:11:03.428885 django_channels_graphql_ws-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc4/PKG-INFO
```

### Comparing `django_channels_graphql_ws-1.0.0rc3/LICENSE` & `django_channels_graphql_ws-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/client.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/dict_as_object.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/dict_as_object.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,41 +115,41 @@
     # to the original protocol and the client must be tuned accordingly.
     confirm_subscriptions: bool = False
 
     # The message sent to the client when subscription activation
     # confirmation is enabled.
     subscription_confirmation_message: Dict[str, Any] = {"data": None, "errors": None}
 
-    # Issue a warning to the log when operation/resolver takes longer
-    # than specified number in seconds. None disables the warning.
+    # Issue a warning to the log when operation takes longer than
+    # specified number in seconds. None disables the warning.
     warn_operation_timeout: Optional[float] = 1
-    warn_resolver_timeout: Optional[float] = 1
 
     # The size of the subscription notification queue. If there are more
     # notifications (for a single subscription) than the given number,
     # then an oldest notification is dropped and a warning is logged.
     subscription_notification_queue_limit: int = 1024
 
     # GraphQL middleware.
-    # List of functions (callables) like the following:
+    # Instance of `graphql.MiddlewareManager` or the list of functions
+    # (callables) like the following:
     # ```python
     # async def my_middleware(next_middleware, root, info, *args, **kwds):
     #     result = next_middleware(root, info, *args, **kwds)
     #     if graphql.pyutils.is_awaitable(result):
     #        result = await result
     #     return result
     # ```
     # The first middleware in the middlewares list will be the closest
     # to the resolver in the middlewares call stack.
     # For more information read docs:
     # - https://docs.graphene-python.org/en/latest/execution/middleware/#middleware
     # - https://graphql-core-3.readthedocs.io/en/latest/diffs.html#custom-middleware
     # Docs about async middlewares are still missing - read the
     # GraphQL-core sources to know more.
-    middleware: Sequence = []
+    middleware: Optional[graphql.Middleware] = None
 
     # Subscription implementation shall return this to tell consumer
     # to suppress subscription notification.
     SKIP = object()
 
     async def on_connect(self, payload):
         """Client connection handler.
@@ -274,14 +274,23 @@
         # `asyncio.Lock` used to serialize processing of start & stop
         # requests. Since the collection is weak, it automatically
         # throws away items when locks are garbage collected.
         self._operation_locks: weakref.WeakValueDictionary = (
             weakref.WeakValueDictionary()
         )
 
+        # MiddlewareManager maintains internal cache for resolvers
+        # wrapped with middlewares. Using the same manager for all
+        # operations improves performance.
+        self._middleware = None
+        if self.middleware:
+            self._middleware = self.middleware
+            if not isinstance(self._middleware, graphql.MiddlewareManager):
+                self._middleware = graphql.MiddlewareManager(*self._middleware)
+
         super().__init__(*args, **kwargs)
 
     # ---------------------------------------------------------- CONSUMER EVENT HANDLERS
 
     async def connect(self):
         """Handle new WebSocket connection."""
 
@@ -591,35 +600,14 @@
                 await self._send_gql_data(op_id, None, errors)
                 await self._send_gql_complete(op_id)
                 return
             # Assert values are not None to suppress MyPy complains.
             assert doc_ast is not None
             assert op_ast is not None
 
-            async def unbound_root_middleware(*args, **kwds):
-                """Unbound function for root middleware.
-
-                `graphql.MiddlewareManager` accepts only unbound
-                functions as middleware.
-                """
-                return await self._on_gql_start__root_middleware(
-                    op_id, op_name, *args, **kwds
-                )
-
-            # NOTE: Middlewares order is important, root middleware
-            # should always be the farest from the real resolver (last
-            # in the middleware list). Because we want to calculate
-            # resolver execution time with middlewares included.
-            middlewares = list(self.middleware)
-            if self.warn_resolver_timeout is not None:
-                middlewares.append(unbound_root_middleware)
-            middleware_manager: Optional[graphql.MiddlewareManager] = None
-            if middlewares:
-                middleware_manager = graphql.MiddlewareManager(*middlewares)
-
             # If the operation is subscription.
             if op_ast.operation == graphql.language.ast.OperationType.SUBSCRIPTION:
                 LOG.debug(
                     "Subscription request. Operation ID: %s, operation name: %s.)",
                     op_id,
                     op_name,
                 )
@@ -633,15 +621,15 @@
                     variable_values=variables,
                     context_value=context,
                     subscribe_field_resolver=functools.partial(
                         self._on_gql_start__initialize_subscription_stream,
                         op_id,
                         op_name,
                     ),
-                    middleware=middleware_manager,
+                    middleware=self._middleware,
                     execution_context_class=self._SubscriptionExecutionContext,
                 )
 
                 # When subscr_result is an AsyncGenerator, consume
                 # stream of notifications and send them to clients.
                 if not isinstance(subscr_result, graphql.ExecutionResult):
                     stream = cast(AsyncIterator[graphql.ExecutionResult], subscr_result)
@@ -711,14 +699,15 @@
 
                 # Standard name for "IntrospectionQuery". We might also
                 # check that
                 # `doc_ast.definitions[0].selection_set.selections[0].name.value`
                 # equals to `__schema`. This is a more robust way. But
                 # it will eat up more CPU pre each query. For now lets
                 # check only a query name.
+                middleware_manager = self._middleware
                 if op_name == "IntrospectionQuery":
                     # No need to call middlewares for the
                     # IntrospectionQuery. There no real resolvers. Only
                     # the type information.
                     middleware_manager = None
                 exec_result = graphql.execution.execute(
                     self.schema.graphql_schema,
@@ -897,90 +886,14 @@
             )  # type: ignore
             result = await result if inspect.isawaitable(result) else result
             return cast(graphql.ExecutionResult, result)
 
         # Map every source value to a ExecutionResult value.
         return graphql.MapAsyncIterator(result_or_stream, map_source_to_response)
 
-    async def _on_gql_start__root_middleware(
-        self,
-        operation_id: int,
-        operation_name: str,
-        next_middleware,
-        root,
-        info: graphql.GraphQLResolveInfo,
-        *args,
-        **kwds,
-    ):
-        """Root middleware injected right before resolver invocation.
-
-        This middleware issues a warning if resolver execution time
-        exceeds a limit.
-
-        Since this middleware always comes first in the list of
-        middlewares, it always receives resolver as the first
-        argument instead of another middleware.
-
-        This is a part of START message processing routine so the name
-        prefixed with `_on_gql_start__` to make this explicit.
-
-        Args:
-            resolver: Resolver to "wrap" into this middleware
-            root: Anything. Eventually passed to the resolver.
-            info: Passed to the resolver.
-
-        Returns:
-            Any value: result returned by the resolver.
-            AsyncGenerator: when subscription starts.
-        """
-
-        # Unwrap resolver from functools.partial or other wrappers.
-        real_resolver = self._on_gql_start__unwrap(next_middleware)
-
-        # Start measuring resolver execution time.
-        if self.warn_resolver_timeout is not None:
-            start_time = time.perf_counter()
-
-        # Execute resolver.
-        result = next_middleware(root, info, *args, **kwds)
-        if inspect.isawaitable(result):
-            result = await result
-
-        # Warn about long resolver execution if the time limit exceeds.
-        if self.warn_resolver_timeout is not None:
-            duration = time.perf_counter() - start_time
-            if duration >= self.warn_resolver_timeout:
-                pretty_name = f"{real_resolver.__qualname__}"
-                if hasattr(real_resolver, "__self__"):
-                    pretty_name = f"{real_resolver.__self__.__qualname__}.{pretty_name}"
-                LOG.warning(
-                    "Resolver %s took %.3f seconds (>%.3f)!"
-                    " Operation %s(%s), path: %s.",
-                    pretty_name,
-                    duration,
-                    self.warn_resolver_timeout,
-                    operation_name,
-                    operation_id,
-                    info.path,
-                )
-
-        return result
-
-    def _on_gql_start__unwrap(self, fn: Callable) -> Callable:
-        """Auxiliary method which unwraps given function.
-
-        This is a part of START message processing routine so the name
-        prefixed with `_on_gql_start__` to make this explicit.
-        """
-        if isinstance(fn, functools.partial):
-            fn = self._on_gql_start__unwrap(fn.func)
-        elif hasattr(fn, "__wrapped__"):
-            fn = self._on_gql_start__unwrap(fn.__wrapped__)
-        return fn
-
     async def _on_gql_start__initialize_subscription_stream(
         self,
         operation_id: int,
         operation_name: str,
         root: Any,
         info: graphql.GraphQLResolveInfo,
         *args,
```

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/serializer.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/subscription.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/testing.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/transport.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc3/pyproject.toml` & `django_channels_graphql_ws-1.0.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # --------------------------------------------------------------- POETRY
 # Python packaging and dependency management.
 # Docs: https://python-poetry.org/docs/
 [tool.poetry]
 name = "django-channels-graphql-ws"
-version = "v1.0.0rc3"
+version = "v1.0.0rc4"
 description = """Django Channels based WebSocket GraphQL server with Graphene-like subscriptions"""
 authors = ["Alexander A. Prokhorov <alexander.prokhorov@datadvance.net>"]
 homepage = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 repository = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 license = "MIT"
 packages = [
     { include = "channels_graphql_ws/" },
```

### Comparing `django_channels_graphql_ws-1.0.0rc3/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

