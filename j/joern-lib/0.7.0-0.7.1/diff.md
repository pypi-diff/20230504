# Comparing `tmp/joern_lib-0.7.0.tar.gz` & `tmp/joern_lib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.7.0.tar", max compression
+gzip compressed data, was "joern_lib-0.7.1.tar", max compression
```

## Comparing `joern_lib-0.7.0.tar` & `joern_lib-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-04-29 00:44:10.997535 joern_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0     3102 2023-04-29 00:44:10.997535 joern_lib-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/__init__.py
--rw-r--r--   0        0        0     6685 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/client.py
--rw-r--r--   0        0        0        0 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-04-29 00:44:11.017536 joern_lib-0.7.0/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     6184 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     3914 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/detectors/js.py
--rw-r--r--   0        0        0     2800 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/utils.py
--rw-r--r--   0        0        0     4535 2023-04-29 00:44:11.021535 joern_lib-0.7.0/joern_lib/workspace.py
--rw-r--r--   0        0        0     1185 2023-04-29 00:44:11.021535 joern_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 joern_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 20:10:33.342101 joern_lib-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3441 2023-05-04 20:10:33.342101 joern_lib-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/client.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     7124 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     2814 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3914 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0    10805 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1188 2023-05-04 20:10:33.354101 joern_lib-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 joern_lib-0.7.1/PKG-INFO
```

### Comparing `joern_lib-0.7.0/LICENSE` & `joern_lib-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.0/README.md` & `joern_lib-0.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```
 python -m asyncio
 ```
 
 Execute single query
 
 ```
-from joern_lib import client, workspace
+from joern_lib import client, workspace, utils
 from joern_lib.detectors import common as cpg
 
 connection = await client.get("http://localhost:9000", "http://localhost:7072", "admin", "admin")
 
 # connection = await client.get("http://localhost:9000")
 
 res = await client.q(connection, "val a=1");
@@ -103,14 +103,33 @@
 List files
 
 ```
 res = await cpg.list_files(connection)
 # list of files
 ```
 
+Print call tree
+
+```
+res = await cpg.get_call_tree(connection, "com.example.vulnspring.WebController.issue:java.lang.String(org.springframework.ui.Model,java.lang.String)")
+utils.print_tree(res)
+```
+
+### Java specific
+
+```
+from joern_lib.detectors import java
+```
+
+List http routes
+
+```
+await java.list_http_routes(connection)
+```
+
 ### JavaScript specific
 
 ```
 from joern_lib.detectors import js
 ```
 
 List http routes
```

### Comparing `joern_lib-0.7.0/joern_lib/client.py` & `joern_lib-0.7.1/joern_lib/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,18 +65,37 @@
 
 
 async def receive(connection):
     return await connection.websocket.recv()
 
 
 def fix_json(sout):
+    source_sink_mode = False
     try:
-        sout = sout.replace(r'"\"', '"').replace(r'\""', '"')
+        if "defined function source" in sout:
+            source_sink_mode = True
+            sout = sout.replace("defined function source\n", "")
+            sout = sout.replace("defined function sink\n", "")
+        else:
+            sout = sout.replace(r'"\"', '"').replace(r'\""', '"')
         if ': String = "[' in sout:
-            sout = sout.split(': String = "')[-1][-1]
+            if source_sink_mode:
+                sout = (
+                    sout.replace(r"\"", '"')
+                    .replace('}]}]"', "}]}]")
+                    .replace('\\"', '"')
+                )
+                sout = sout.split(': String = "')[-1]
+            else:
+                sout = sout.split(': String = "')[-1][-1]
+        elif "tree: ListBuffer" in sout:
+            sout = sout.split(": String = ")[-1]
+            if '"""' in sout:
+                sout = sout.replace('"""', "")
+            return sout
         elif 'String = """[' in sout:
             tmpA = sout.split("\n")[1:-2]
             sout = "[ " + "\n".join(tmpA) + "]"
         return orjson.loads(sout)
     except Exception:
         return {"response": sout}
 
@@ -190,14 +209,39 @@
         if isinstance(tmpres, dict) and tmpres.get("response"):
             tmpres = tmpres.get("response")
         tmpA = tmpres.split('"""')[1:-1]
         print_md("\n".join([n for n in tmpA if len(n.strip()) > 1]))
     return results
 
 
+async def df(connection, source, sink):
+    if not source.startswith("def"):
+        source = f"def source = {source}"
+    if not sink.startswith("def"):
+        sink = f"def sink = {sink}"
+    results = await query(
+        connection,
+        f"""
+        {source}
+        {sink}
+        sink.reachableByFlows(source).map(m => (m, m.elements.location.l)).toJson
+        """,
+    )
+    if len(results):
+        tmpres = results[-1]
+        if isinstance(tmpres, dict) and tmpres.get("response"):
+            tmpres = tmpres.get("response")
+        # print(tmpres)
+    return results
+
+
+async def reachableByFlows(connection, source, sink):
+    return await df(connection, source, sink)
+
+
 async def create_cpg(connection, src, out_dir, lang):
     client = connection.cpggenclient
     if not client:
         return {
             "error": "true",
             "message": "No active connection to cpggen server. Pass the cpggen url to the client.get method.",
         }, 500
```

### Comparing `joern_lib-0.7.0/joern_lib/detectors/c.py` & `joern_lib-0.7.1/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.0/joern_lib/detectors/common.py` & `joern_lib-0.7.1/joern_lib/detectors/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import os
-from tempfile import NamedTemporaryFile
-
 from joern_lib import client
 
 
 async def list_files(connection):
     return await client.q(connection, "cpg.file")
 
 
@@ -36,14 +33,21 @@
     return await client.q(connection, "cpg.dependency")
 
 
 async def list_identifiers(connection):
     return await client.q(connection, "cpg.identifier")
 
 
+async def list_declared_identifiers(connection):
+    return await client.q(
+        connection,
+        """({cpg.assignment.argument(1).isIdentifier.refsTo ++ cpg.parameter.filter(_.typeFullName != "ANY")})""",
+    )
+
+
 async def list_imports(connection):
     return await client.q(connection, "cpg.imports")
 
 
 async def list_if_blocks(connection):
     return await client.q(connection, "cpg.ifBlock")
 
@@ -61,15 +65,27 @@
 
 
 async def list_metadatas(connection):
     return await client.q(connection, "cpg.metaData")
 
 
 async def list_methods(connection):
-    return await client.q(connection, "cpg.method")
+    return await client.q(
+        connection, """cpg.method.whereNot(_.name(".*<operator>.*"))"""
+    )
+
+
+async def list_constructors(connection):
+    return await client.q(connection, """cpg.method.internal.name("<init>")""")
+
+
+async def list_external_methods(connection):
+    return await client.q(
+        connection, """cpg.method.isExternal(true).whereNot(_.name(".*<operator>.*"))"""
+    )
 
 
 async def list_method_refs(connection):
     return await client.q(connection, "cpg.methodRef")
 
 
 async def list_methodReturns(connection):
@@ -88,14 +104,21 @@
     return await client.q(connection, "cpg.tag")
 
 
 async def list_types(connection):
     return await client.q(connection, "cpg.typ")
 
 
+async def list_custom_types(connection):
+    return await client.q(
+        connection,
+        """cpg.typeDecl.filterNot(t => t.isExternal || t.name.matches("(:program|<module>|<init>|<meta>|<body>)"))""",
+    )
+
+
 async def get_calls(connection, pattern):
     return await client.q(connection, f"""cpg.call.code("(?i){pattern}")""")
 
 
 async def get_method_callIn(connection, pattern):
     return await client.q(
         connection, f"""cpg.method("(?i){pattern}").callIn.location"""
@@ -105,53 +128,77 @@
 async def get_identifiers_in_file(connection, filename):
     return await client.q(
         connection,
         f"""cpg.call.name(Operators.assignment).argument.order(1).map(t => (t, t.location.filename)).filter(_._2.equals("{filename}")).filter(_._1.isIdentifier).map(_._1.code).filterNot(_.contains("_tmp_")).dedup""",
     )
 
 
+async def get_methods_multiple_returns(connection):
+    return await get_functions_multiple_returns(connection)
+
+
 async def get_functions_multiple_returns(connection):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.ast.isReturn.l.size > 1).nameNot("<global>")}).location""",
     )
 
 
+async def get_complex_methods(connection, n=4):
+    return await get_complex_functions(connection, n)
+
+
 async def get_complex_functions(connection, n=4):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.controlStructure.size > %(n)d).nameNot("<global>")}).location"""
         % dict(n=n),
     )
 
 
+async def get_long_methods(connection, n=1000):
+    return await get_long_functions(connection, n)
+
+
 async def get_long_functions(connection, n=1000):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.numberOfLines > %(n)d).nameNot("<global>")}).location"""
         % dict(n=n),
     )
 
 
+async def get_too_many_loops_methods(connection, n=4):
+    return await get_too_many_loops_functions(connection, n)
+
+
 async def get_too_many_loops_functions(connection, n=4):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.ast.isControlStructure.controlStructureType("(FOR|DO|WHILE)").size > %(n)d).nameNot("<global>")}).location"""
         % dict(n=n),
     )
 
 
+async def get_too_many_params_methods(connection, n=4):
+    return await get_too_many_params_functions(connection, n)
+
+
 async def get_too_many_params_functions(connection, n=4):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.parameter.size > %(n)d).nameNot("<global>")}).location"""
         % dict(n=n),
     )
 
 
+async def get_too_nested_methods(connection, n=4):
+    return await get_too_nested_functions(connection, n)
+
+
 async def get_too_nested_functions(connection, n=4):
     return await client.q(
         connection,
         """({cpg.method.internal.filter(_.depth(_.isControlStructure) > %(n)d).nameNot("<global>")}).location"""
         % dict(n=n),
     )
 
@@ -192,29 +239,16 @@
             }
         }
     }
     findCallee(lastCallerMethod, tree)
 }
 """,
     )
-    with NamedTemporaryFile(prefix="call-tree-", suffix=".txt", delete=False) as tp:
-        try:
-            os.chmod(tp.name, 0o777)
-        except Exception:
-            # ignore errors
-            pass
-        await client.q(
-            connection,
-            """
-            var tree = new ListBuffer[String]()
-            printCallTree("%(method_name)s", tree, %(n)d)
-            tree.toList |> "%(temp_file)s"
-            """
-            % dict(method_name=method_name, n=n, temp_file=tp.name),
-        )
-        content = open(tp.name).read()
-        try:
-            os.remove(tp.name)
-        except Exception:
-            # ignore errors
-            pass
-        return content.replace("\\n", "\n")
+    return await client.q(
+        connection,
+        """
+        var tree = new ListBuffer[String]()
+        printCallTree("%(method_name)s", tree, %(n)d)
+        tree.toList.mkString("\\n")
+        """
+        % dict(method_name=method_name, n=n),
+    )
```

### Comparing `joern_lib-0.7.0/joern_lib/detectors/js.py` & `joern_lib-0.7.1/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.0/joern_lib/workspace.py` & `joern_lib-0.7.1/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.0/pyproject.toml` & `joern_lib-0.7.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.7.0"
+version = "0.7.1"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
@@ -20,19 +20,19 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 exclude = ["contrib", "tests"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
-httpx = "^0.23.3"
-websockets = "^10.4"
+httpx = "^0.24.0"
+websockets = "^11.0.2"
 uvloop = "^0.17.0"
-orjson = "^3.8.7"
-rich = "^13.3.1"
+orjson = "^3.8.11"
+rich = "^13.3.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
 pyinstaller = "^5.0.1"
```

### Comparing `joern_lib-0.7.0/PKG-INFO` & `joern_lib-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.7,<3.11
@@ -19,19 +19,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: orjson (>=3.8.7,<4.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: orjson (>=3.8.11,<4.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
-Requires-Dist: websockets (>=10.4,<11.0)
+Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Project-URL: Repository, https://github.com/AppThreat/joern-lib
 Description-Content-Type: text/markdown
 
 # Introduction
 
 High level python library to interact with a Joern [server](https://docs.joern.io/server).
 
@@ -68,15 +68,15 @@
 ```
 python -m asyncio
 ```
 
 Execute single query
 
 ```
-from joern_lib import client, workspace
+from joern_lib import client, workspace, utils
 from joern_lib.detectors import common as cpg
 
 connection = await client.get("http://localhost:9000", "http://localhost:7072", "admin", "admin")
 
 # connection = await client.get("http://localhost:9000")
 
 res = await client.q(connection, "val a=1");
@@ -136,14 +136,33 @@
 List files
 
 ```
 res = await cpg.list_files(connection)
 # list of files
 ```
 
+Print call tree
+
+```
+res = await cpg.get_call_tree(connection, "com.example.vulnspring.WebController.issue:java.lang.String(org.springframework.ui.Model,java.lang.String)")
+utils.print_tree(res)
+```
+
+### Java specific
+
+```
+from joern_lib.detectors import java
+```
+
+List http routes
+
+```
+await java.list_http_routes(connection)
+```
+
 ### JavaScript specific
 
 ```
 from joern_lib.detectors import js
 ```
 
 List http routes
```

