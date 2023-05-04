# Comparing `tmp/fastdev-py-0.3.0.tar.gz` & `tmp/fastdev-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-py-0.3.0.tar", last modified: Tue May  2 02:12:20 2023, max compression
+gzip compressed data, was "fastdev-py-0.4.0.tar", last modified: Thu May  4 00:28:59 2023, max compression
```

## Comparing `fastdev-py-0.3.0.tar` & `fastdev-py-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      677 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      748 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.github/workflows/pypitest-publish.yml
--rw-r--r--   0        0        0      856 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.gitignore
--rw-r--r--   0        0        0       51 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/license.md
--rw-r--r--   0        0        0     1231 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      302 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/readme.md
--rw-r--r--   0        0        0      154 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/__init__.py
--rw-r--r--   0        0        0      584 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/__main__.py
--rw-r--r--   0        0        0    11496 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/builders/deno_lts_esbuild.ts
--rw-r--r--   0        0        0     1015 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/config.py
--rw-r--r--   0        0        0     1701 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/fs_serving.py
--rw-r--r--   0        0        0     8133 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/preprocessor/temp.py.bak
--rw-r--r--   0        0        0     4405 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/router.py
--rw-r--r--   0        0        0     1410 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/ts_serving.py
--rw-r--r--   0        0        0     1463 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/utils.py
--rw-r--r--   0        0        0      313 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/tests/1/hello.ts
--rw-r--r--   0        0        0       40 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/tests/1/temp.ts
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      677 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      748 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/.github/workflows/pypitest-publish.yml
+-rw-r--r--   0        0        0      856 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/.gitignore
+-rw-r--r--   0        0        0       51 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/license.md
+-rw-r--r--   0        0        0     1231 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/readme.md
+-rw-r--r--   0        0        0      208 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/__main__.py
+-rw-r--r--   0        0        0     1015 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/config.py
+-rw-r--r--   0        0        0     4288 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/deno_ltbs/deps.ts
+-rw-r--r--   0        0        0     4098 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/deno_ltbs/esbuild_builder.ts
+-rw-r--r--   0        0        0     2267 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/deno_ltbs/html_builder.ts
+-rw-r--r--   0        0        0     5055 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/deno_ltbs/mod.ts
+-rw-r--r--   0        0        0     3091 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/fs_serving.py
+-rw-r--r--   0        0        0     8133 2023-05-04 00:28:48.349193 fastdev-py-0.4.0/src/fastdev/preprocessor/temp.py.bak
+-rw-r--r--   0        0        0     7409 2023-05-04 00:28:48.353193 fastdev-py-0.4.0/src/fastdev/router.py
+-rw-r--r--   0        0        0     1965 2023-05-04 00:28:48.353193 fastdev-py-0.4.0/src/fastdev/ts_serving.py
+-rw-r--r--   0        0        0     1463 2023-05-04 00:28:48.353193 fastdev-py-0.4.0/src/fastdev/utils.py
+-rw-r--r--   0        0        0      313 2023-05-04 00:28:48.353193 fastdev-py-0.4.0/tests/1/hello.ts
+-rw-r--r--   0        0        0       40 2023-05-04 00:28:48.353193 fastdev-py-0.4.0/tests/1/temp.ts
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.4.0/PKG-INFO
```

### Comparing `fastdev-py-0.3.0/.github/workflows/pypi-publish.yml` & `fastdev-py-0.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/.github/workflows/pypitest-publish.yml` & `fastdev-py-0.4.0/.github/workflows/pypitest-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/.gitignore` & `fastdev-py-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/pyproject.toml` & `fastdev-py-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fastdev-py"
-version = "0.3.0"
+version = "0.4.0"
 description = "FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files."
 readme = "readme.md"
 requires-python = ">=3.11"
 license = { file = "license.md" }
 authors = [{ name = "Omar Azmi" }]
 dependencies = ["fastapi"]
 keywords = [
```

### Comparing `fastdev-py-0.3.0/src/fastdev/__main__.py` & `fastdev-py-0.4.0/src/fastdev/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 def main(*, host: str = "localhost", port: int = config.Port, esbuild_config: Annotated[dict, "Partial", config.ESBuildConfig] = dict()):
 	if host.lower().rstrip("/").endswith("localhost"):
 		host = "0.0.0.0"
 	config.Port = port
 	config.ESBuildConfig.update(esbuild_config)
 	app = FastAPI()
-	from .__init__ import apply_route_path, apply_route_ts
+	from .__init__ import apply_route_fs, apply_route_html_ts, apply_route_ts
+	apply_route_html_ts(app)
 	apply_route_ts(app)
-	apply_route_path(app)
+	apply_route_fs(app)
 	uvicorn.run(app, host=host, port=config.Port, reload=False)
 
 
 if __name__ == "__main__":
 	main()
```

### Comparing `fastdev-py-0.3.0/src/fastdev/config.py` & `fastdev-py-0.4.0/src/fastdev/config.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/src/fastdev/preprocessor/temp.py.bak` & `fastdev-py-0.4.0/src/fastdev/preprocessor/temp.py.bak`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/src/fastdev/router.py` & `fastdev-py-0.4.0/src/fastdev/router.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from pathlib import Path
 from typing import Type, TypeVar
 from fastapi import APIRouter, FastAPI, Response
 from fastapi.responses import PlainTextResponse, RedirectResponse
 from .config import SWD
 from .fs_serving import serve_dir, serve_file
 from .ts_serving import (
-	build_server_callback_path, build_server_loaded_promise, serve_ts,
+	build_server_callback_path, build_server_loaded_promise, serve_html_ts,
+	serve_ts,
 )
 
 APP_OR_ROUTER = TypeVar("APP_OR_ROUTER", FastAPI, APIRouter)
 
 
 async def enable_ts_build_server():
 	if not build_server_loaded_promise.done():
@@ -19,15 +20,15 @@
 
 
 async def route_ts(
 	file_path: str,
 	base_dir: Path = SWD,
 	ext: str = ".ts"
 ) -> Response:
-	""" route a typescript file
+	""" route to a compiled version of a typescript file
 
 	:param file_path: path to typescript file. must exclude extension
 	:type file_path: str
 	:param base_dir: \
 		filesystem path to mount onto your `base_url`. \
 		the path MUST be absolute (use `base_dir.absolute()`) \
 		defaults to SWD (server's root working directory)
@@ -43,15 +44,15 @@
 	return await serve_ts(abspath)
 
 
 def apply_route_ts(
 	fastapi_app: Type[APP_OR_ROUTER],
 	base_url: str = "/",
 	base_dir: Path = SWD,
-	exts: list[str] = [".ts", ".tsx"]
+	exts: list[str] = [".ts", ".tsx", ".jsx"]
 ) -> APP_OR_ROUTER:
 	""" apply typescript routing to your provided FastAPI app. <br>
 	it's best if you apply this routing first, before applying any other routing <br>
 	so that it captures all typescript files first and foremost.
 
 	:param fastapi_app: your FastAPI app to apply the routing to
 	:type fastapi_app: FastAPI | APIRouter
@@ -62,15 +63,15 @@
 	:type base_url: str, optional
 	:param base_dir: \
 		filesystem path to mount onto your `base_url`. \
 		defaults to SWD (server's root working directory)
 	:type base_dir: Path, optional
 	:param exts: \
 		name the extensions that your typescript files end with. \
-		defaults to [".ts", ".tsx"]
+		defaults to [".ts", ".tsx", ".jsx"]
 	:type exts: list[str], optional
 	:return: the provided `fastapi_app` gets returned back
 	:rtype: FastAPI | APIRouter
 	"""
 	fastapi_app.add_api_route(
 		build_server_callback_path,
 		enable_ts_build_server,
@@ -81,37 +82,120 @@
 			base_url + "{file_path:path}" + ext,
 			partial(route_ts, base_dir=base_dir.absolute(), ext=ext),
 			methods=["GET"]
 		)
 	return fastapi_app
 
 
-async def route_path(path: str, base_dir: Path = SWD):
-	# TODO add docstring and include: base_dir must be absolute
+async def route_html_ts(
+	file_path: str,
+	base_dir: Path = SWD,
+	ext: str = ".html.js"
+) -> Response:
+	""" route to a javascript's code's default output string
+
+	:param file_path: path to javascript-like file (js, ts, etc...). must exclude extension
+	:type file_path: str
+	:param base_dir: \
+		filesystem path to mount onto your `base_url`. \
+		the path MUST be absolute (use `base_dir.absolute()`) \
+		defaults to SWD (server's root working directory)
+	:type base_dir: Path, optional
+	:param ext: \
+		javascript, or typescript file extension. \
+		defaults to ".html.js"
+	:type ext: str, optional
+	:return: executes javascript file and returns its `export default` string output as an html
+	:rtype: Response
+	"""
+	abspath = base_dir.joinpath(file_path + ext)
+	return await serve_html_ts(abspath)
+
+
+def apply_route_html_ts(
+	fastapi_app: Type[APP_OR_ROUTER],
+	base_url: str = "/",
+	base_dir: Path = SWD,
+	exts: list[str] = [".html.js", ".html.ts", ".html.tsx", ".html.jsx"]
+) -> APP_OR_ROUTER:
+	""" apply javascript generated html routing to your provided FastAPI app. <br>
+	it's best if you apply this routing before `apply_route_ts` <br>
+	so that it captures all ".html.(js|ts|tsx|jsx)" files first and foremost.
+
+	:param fastapi_app: your FastAPI app to apply the routing to
+	:type fastapi_app: FastAPI | APIRouter
+	:param base_url: \
+		base url of the path that will be mounted. \
+		must always begin with a slash "/" and also end with one. \
+		defaults to "/"
+	:type base_url: str, optional
+	:param base_dir: \
+		filesystem path to mount onto your `base_url`. \
+		defaults to SWD (server's root working directory)
+	:type base_dir: Path, optional
+	:param exts: \
+		javascript, or typescript file extension. \
+		defaults to [".html.js", ".html.ts", ".html.tsx", ".html.jsx"]
+	:type exts: list[str], optional
+	:return: the provided `fastapi_app` gets returned back
+	:rtype: FastAPI | APIRouter
+	"""
+	fastapi_app.add_api_route(
+		build_server_callback_path,
+		enable_ts_build_server,
+		methods=["GET", "POST"]
+	)
+	for ext in exts:
+		fastapi_app.add_api_route(
+			base_url + "{file_path:path}" + ext,
+			partial(route_html_ts, base_dir=base_dir.absolute(), ext=ext),
+			methods=["GET"]
+		)
+	return fastapi_app
+
+
+async def route_fs(path: str, base_dir: Path = SWD):
+	""" route across a filesystem `path`, relative to `base_dir`.
+	note that `base_dir` must be an absolute path.
+	if a directory path is requested, then a listing of the directory's contents will be seved.
+	if there's "index.html" in the requested directory, then you'll be redirected towards it.
+	else if a file's path is requested, then that file will be served.
+
+	:param path: path to serve, relative to `base_dir`
+	:type path: str
+	:param base_dir: \
+		root directory of this router. \
+		when `path == "/"` or `path == ""`, this filesystem directory will be served. \
+		note that it must be an absolute path. \
+		defaults to SWD (server's root working directory)
+	:type base_dir: Path, optional
+	:return: file or directory listing
+	:rtype: FileResponse | HTMLResponse | PlainTextResponse
+	"""
 	abspath = base_dir.joinpath(path)
 	if not abspath.exists():
 		return Response(status_code=404)
 	elif abspath.is_file():
 		return await serve_file(abspath)
 	elif abspath.is_dir():
 		if path.endswith("/") or base_dir.samefile(abspath):
 			# check if "./index.html" is available in the requested path directory, and redirect to it if it does exist
 			if abspath.joinpath("./index.html").is_file():
 				print("index.html found in requested directory. redirecting to it.")
-				RedirectResponse("./index.html")
+				return RedirectResponse("./index.html")
 			return await serve_dir(abspath, base_dir)
 		return RedirectResponse("./" + path.split("/")[-1] + "/")
 	else:
 		return PlainTextResponse(
 			f"the following request was uncaught by path router:\n\tpath:\t{path}\n\tbase_dir:\t{base_dir}",
 			status_code=500
 		)
 
 
-def apply_route_path(
+def apply_route_fs(
 	fastapi_app: Type[APP_OR_ROUTER],
 	base_url: str = "/",
 	base_dir: Path = SWD
 ) -> APP_OR_ROUTER:
 	""" apply filesystem path routing to your provided FastAPI app. <br>
 	you would probably want to apply this route lastly, since it captures all paths.
 
@@ -125,9 +209,9 @@
 	:param base_dir: \
 		filesystem path to mount onto your `base_url`. \
 		defaults to SWD (server's root working directory)
 	:type base_dir: Path, optional
 	:return: the provided `fastapi_app` gets returned back
 	:rtype: FastAPI | APIRouter
 	"""
-	fastapi_app.get(base_url + "{path:path}")(partial(route_path, base_dir=base_dir.absolute()))
+	fastapi_app.get(base_url + "{path:path}")(partial(route_fs, base_dir=base_dir.absolute()))
 	return fastapi_app
```

### Comparing `fastdev-py-0.3.0/src/fastdev/utils.py` & `fastdev-py-0.4.0/src/fastdev/utils.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.3.0/PKG-INFO` & `fastdev-py-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdev-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files.
 Keywords: devserver,dev-server,devtools,sever,liveserver,live-server
 Author: Omar Azmi
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Project-URL: Homepage, https://github.com/omar-azmi/fastdev_py
```

