# Comparing `tmp/browsr-1.1.0.tar.gz` & `tmp/browsr-1.1.1.tar.gz`

## Comparing `browsr-1.1.0.tar` & `browsr-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.1.0/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.1.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.1.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/__main__.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/_base.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/_version.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/code_browser.css
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 browsr-1.1.0/browsr/code_browser.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.1.0/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.1.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.1.0/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.1.0/docs/index.md
--rw-r--r--   0        0        0    57970 2020-02-02 00:00:00.000000 browsr-1.1.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 browsr-1.1.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.1.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.1.0/README.md
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 browsr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.1.1/.releaserc.js
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.1.1/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.1.1/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/__main__.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/_base.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/_version.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/code_browser.css
+-rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 browsr-1.1.1/browsr/code_browser.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.1.1/docs/api_documentation.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.1.1/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.1.1/docs/contributing.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.1.1/docs/index.md
+-rw-r--r--   0        0        0   115582 2020-02-02 00:00:00.000000 browsr-1.1.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 browsr-1.1.1/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.1.1/README.md
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 browsr-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 browsr-1.1.1/PKG-INFO
```

### Comparing `browsr-1.1.0/.pre-commit-config.yaml` & `browsr-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.releaserc.js` & `browsr-1.1.1/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/mkdocs.yaml` & `browsr-1.1.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/semantic_release/package-lock.json` & `browsr-1.1.1/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/semantic_release/release_notes.hbs` & `browsr-1.1.1/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/workflows/lint.yaml` & `browsr-1.1.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/workflows/publish.yaml` & `browsr-1.1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/workflows/release.yaml` & `browsr-1.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/.github/workflows/tests.yaml` & `browsr-1.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/browsr/_base.py` & `browsr-1.1.1/browsr/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     debug: bool = False
 
     @property
     def path(self) -> pathlib.Path:
         """
         Resolve `file_path` to a upath.UPath object
         """
-
+        if str(self.file_path).endswith("/"):
+            self.file_path = str(self.file_path)[:-1]
         return (
             upath.UPath(self.file_path).resolve()
             if self.file_path
             else pathlib.Path.cwd().resolve()
         )
```

### Comparing `browsr-1.1.0/browsr/code_browser.py` & `browsr-1.1.1/browsr/code_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import upath
 from art import text2art  # type: ignore[import]
 from PIL import Image
 from rich import traceback
 from rich.markdown import Markdown
 from rich.syntax import Syntax
 from rich.traceback import Traceback
-from textual.containers import Container, Vertical
+from textual.containers import Container, VerticalScroll
 from textual.reactive import var
 from textual.widget import Widget
 from textual.widgets import DataTable, DirectoryTree, Footer, Header, Static
 from upath.implementations.cloud import CloudPath
 
 from browsr._base import (
     BrowsrClickContext,
@@ -114,17 +114,17 @@
             if TYPE_CHECKING:
                 assert isinstance(file_path, pathlib.Path)
             self.selected_file_path = file_path.joinpath("README.md")
             self.force_show_tree = True
         self.header = Header()
         yield self.header
         self.directory_tree = UniversalDirectoryTree(str(file_path), id="tree-view")
-        self.code_view = Vertical(Static(id="code", expand=True), id="code-view")
+        self.code_view = VerticalScroll(Static(id="code", expand=True), id="code-view")
         self.table_view: DataTable[str] = DataTable(
-            zebra_stripes=True, show_header=True, show_cursor=True
+            zebra_stripes=True, show_header=True, show_cursor=True, id="table-view"
         )
         self.table_view.display = False
         self.container = Container(self.directory_tree, self.code_view, self.table_view)
         yield self.container
         self.footer = Footer()
         yield self.footer
```

### Comparing `browsr-1.1.0/docs/contributing.md` & `browsr-1.1.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/docs/index.md` & `browsr-1.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/requirements/requirements-dev.txt` & `browsr-1.1.1/requirements/requirements-prod.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,238 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --generate-hashes --output-file=requirements/requirements-dev.txt --resolver=backtracking requirements.in
+#    pip-compile --generate-hashes --output-file=requirements/requirements-prod.txt --resolver=backtracking requirements.in
 #
+adal==1.2.7 \
+    --hash=sha256:2a7451ed7441ddbc57703042204a3e30ef747478eea022c70f789fc7f084bc3d \
+    --hash=sha256:d74f45b81317454d96e982fd1c50e6fb5c99ac2223728aea8764433a39f566f1
+    # via azure-datalake-store
+adlfs==2023.1.0 \
+    --hash=sha256:ccbdd6d33d5b7bce99a4a07c884c82fb135745d39b2d9b7b672f8e9d4d04407f \
+    --hash=sha256:eca53f53d88fc8e2e7a2f1d8f5a40b8a1c56aa3b541e4aa2e7eaf55a6a789262
+    # via -r requirements.in
+aiobotocore==2.4.2 \
+    --hash=sha256:0603b74a582dffa7511ce7548d07dc9b10ec87bc5fb657eb0b34f9bd490958bf \
+    --hash=sha256:4acd1ebe2e44be4b100aa553910bda899f6dc090b3da2bc1cf3d5de2146ed208
+    # via s3fs
+aiohttp==3.8.4 \
+    --hash=sha256:03543dcf98a6619254b409be2d22b51f21ec66272be4ebda7b04e6412e4b2e14 \
+    --hash=sha256:03baa76b730e4e15a45f81dfe29a8d910314143414e528737f8589ec60cf7391 \
+    --hash=sha256:0a63f03189a6fa7c900226e3ef5ba4d3bd047e18f445e69adbd65af433add5a2 \
+    --hash=sha256:10c8cefcff98fd9168cdd86c4da8b84baaa90bf2da2269c6161984e6737bf23e \
+    --hash=sha256:147ae376f14b55f4f3c2b118b95be50a369b89b38a971e80a17c3fd623f280c9 \
+    --hash=sha256:176a64b24c0935869d5bbc4c96e82f89f643bcdf08ec947701b9dbb3c956b7dd \
+    --hash=sha256:17b79c2963db82086229012cff93ea55196ed31f6493bb1ccd2c62f1724324e4 \
+    --hash=sha256:1a45865451439eb320784918617ba54b7a377e3501fb70402ab84d38c2cd891b \
+    --hash=sha256:1b3ea7edd2d24538959c1c1abf97c744d879d4e541d38305f9bd7d9b10c9ec41 \
+    --hash=sha256:22f6eab15b6db242499a16de87939a342f5a950ad0abaf1532038e2ce7d31567 \
+    --hash=sha256:3032dcb1c35bc330134a5b8a5d4f68c1a87252dfc6e1262c65a7e30e62298275 \
+    --hash=sha256:33587f26dcee66efb2fff3c177547bd0449ab7edf1b73a7f5dea1e38609a0c54 \
+    --hash=sha256:34ce9f93a4a68d1272d26030655dd1b58ff727b3ed2a33d80ec433561b03d67a \
+    --hash=sha256:3a80464982d41b1fbfe3154e440ba4904b71c1a53e9cd584098cd41efdb188ef \
+    --hash=sha256:3b90467ebc3d9fa5b0f9b6489dfb2c304a1db7b9946fa92aa76a831b9d587e99 \
+    --hash=sha256:3d89efa095ca7d442a6d0cbc755f9e08190ba40069b235c9886a8763b03785da \
+    --hash=sha256:3d8ef1a630519a26d6760bc695842579cb09e373c5f227a21b67dc3eb16cfea4 \
+    --hash=sha256:3f43255086fe25e36fd5ed8f2ee47477408a73ef00e804cb2b5cba4bf2ac7f5e \
+    --hash=sha256:40653609b3bf50611356e6b6554e3a331f6879fa7116f3959b20e3528783e699 \
+    --hash=sha256:41a86a69bb63bb2fc3dc9ad5ea9f10f1c9c8e282b471931be0268ddd09430b04 \
+    --hash=sha256:493f5bc2f8307286b7799c6d899d388bbaa7dfa6c4caf4f97ef7521b9cb13719 \
+    --hash=sha256:4a6cadebe132e90cefa77e45f2d2f1a4b2ce5c6b1bfc1656c1ddafcfe4ba8131 \
+    --hash=sha256:4c745b109057e7e5f1848c689ee4fb3a016c8d4d92da52b312f8a509f83aa05e \
+    --hash=sha256:4d347a172f866cd1d93126d9b239fcbe682acb39b48ee0873c73c933dd23bd0f \
+    --hash=sha256:4dac314662f4e2aa5009977b652d9b8db7121b46c38f2073bfeed9f4049732cd \
+    --hash=sha256:4ddaae3f3d32fc2cb4c53fab020b69a05c8ab1f02e0e59665c6f7a0d3a5be54f \
+    --hash=sha256:5393fb786a9e23e4799fec788e7e735de18052f83682ce2dfcabaf1c00c2c08e \
+    --hash=sha256:59f029a5f6e2d679296db7bee982bb3d20c088e52a2977e3175faf31d6fb75d1 \
+    --hash=sha256:5a7bdf9e57126dc345b683c3632e8ba317c31d2a41acd5800c10640387d193ed \
+    --hash=sha256:5b3f2e06a512e94722886c0827bee9807c86a9f698fac6b3aee841fab49bbfb4 \
+    --hash=sha256:5ce45967538fb747370308d3145aa68a074bdecb4f3a300869590f725ced69c1 \
+    --hash=sha256:5e14f25765a578a0a634d5f0cd1e2c3f53964553a00347998dfdf96b8137f777 \
+    --hash=sha256:618c901dd3aad4ace71dfa0f5e82e88b46ef57e3239fc7027773cb6d4ed53531 \
+    --hash=sha256:652b1bff4f15f6287550b4670546a2947f2a4575b6c6dff7760eafb22eacbf0b \
+    --hash=sha256:6c08e8ed6fa3d477e501ec9db169bfac8140e830aa372d77e4a43084d8dd91ab \
+    --hash=sha256:6ddb2a2026c3f6a68c3998a6c47ab6795e4127315d2e35a09997da21865757f8 \
+    --hash=sha256:6e601588f2b502c93c30cd5a45bfc665faaf37bbe835b7cfd461753068232074 \
+    --hash=sha256:6e74dd54f7239fcffe07913ff8b964e28b712f09846e20de78676ce2a3dc0bfc \
+    --hash=sha256:7235604476a76ef249bd64cb8274ed24ccf6995c4a8b51a237005ee7a57e8643 \
+    --hash=sha256:7ab43061a0c81198d88f39aaf90dae9a7744620978f7ef3e3708339b8ed2ef01 \
+    --hash=sha256:7c7837fe8037e96b6dd5cfcf47263c1620a9d332a87ec06a6ca4564e56bd0f36 \
+    --hash=sha256:80575ba9377c5171407a06d0196b2310b679dc752d02a1fcaa2bc20b235dbf24 \
+    --hash=sha256:80a37fe8f7c1e6ce8f2d9c411676e4bc633a8462844e38f46156d07a7d401654 \
+    --hash=sha256:8189c56eb0ddbb95bfadb8f60ea1b22fcfa659396ea36f6adcc521213cd7b44d \
+    --hash=sha256:854f422ac44af92bfe172d8e73229c270dc09b96535e8a548f99c84f82dde241 \
+    --hash=sha256:880e15bb6dad90549b43f796b391cfffd7af373f4646784795e20d92606b7a51 \
+    --hash=sha256:8b631e26df63e52f7cce0cce6507b7a7f1bc9b0c501fcde69742130b32e8782f \
+    --hash=sha256:8c29c77cc57e40f84acef9bfb904373a4e89a4e8b74e71aa8075c021ec9078c2 \
+    --hash=sha256:91f6d540163f90bbaef9387e65f18f73ffd7c79f5225ac3d3f61df7b0d01ad15 \
+    --hash=sha256:92c0cea74a2a81c4c76b62ea1cac163ecb20fb3ba3a75c909b9fa71b4ad493cf \
+    --hash=sha256:9bcb89336efa095ea21b30f9e686763f2be4478f1b0a616969551982c4ee4c3b \
+    --hash=sha256:a1f4689c9a1462f3df0a1f7e797791cd6b124ddbee2b570d34e7f38ade0e2c71 \
+    --hash=sha256:a3fec6a4cb5551721cdd70473eb009d90935b4063acc5f40905d40ecfea23e05 \
+    --hash=sha256:a5d794d1ae64e7753e405ba58e08fcfa73e3fad93ef9b7e31112ef3c9a0efb52 \
+    --hash=sha256:a86d42d7cba1cec432d47ab13b6637bee393a10f664c425ea7b305d1301ca1a3 \
+    --hash=sha256:adfbc22e87365a6e564c804c58fc44ff7727deea782d175c33602737b7feadb6 \
+    --hash=sha256:aeb29c84bb53a84b1a81c6c09d24cf33bb8432cc5c39979021cc0f98c1292a1a \
+    --hash=sha256:aede4df4eeb926c8fa70de46c340a1bc2c6079e1c40ccf7b0eae1313ffd33519 \
+    --hash=sha256:b744c33b6f14ca26b7544e8d8aadff6b765a80ad6164fb1a430bbadd593dfb1a \
+    --hash=sha256:b7a00a9ed8d6e725b55ef98b1b35c88013245f35f68b1b12c5cd4100dddac333 \
+    --hash=sha256:bb96fa6b56bb536c42d6a4a87dfca570ff8e52de2d63cabebfd6fb67049c34b6 \
+    --hash=sha256:bbcf1a76cf6f6dacf2c7f4d2ebd411438c275faa1dc0c68e46eb84eebd05dd7d \
+    --hash=sha256:bca5f24726e2919de94f047739d0a4fc01372801a3672708260546aa2601bf57 \
+    --hash=sha256:bf2e1a9162c1e441bf805a1fd166e249d574ca04e03b34f97e2928769e91ab5c \
+    --hash=sha256:c4eb3b82ca349cf6fadcdc7abcc8b3a50ab74a62e9113ab7a8ebc268aad35bb9 \
+    --hash=sha256:c6cc15d58053c76eacac5fa9152d7d84b8d67b3fde92709195cb984cfb3475ea \
+    --hash=sha256:c6cd05ea06daca6ad6a4ca3ba7fe7dc5b5de063ff4daec6170ec0f9979f6c332 \
+    --hash=sha256:c844fd628851c0bc309f3c801b3a3d58ce430b2ce5b359cd918a5a76d0b20cb5 \
+    --hash=sha256:c9cb1565a7ad52e096a6988e2ee0397f72fe056dadf75d17fa6b5aebaea05622 \
+    --hash=sha256:cab9401de3ea52b4b4c6971db5fb5c999bd4260898af972bf23de1c6b5dd9d71 \
+    --hash=sha256:cd468460eefef601ece4428d3cf4562459157c0f6523db89365202c31b6daebb \
+    --hash=sha256:d1e6a862b76f34395a985b3cd39a0d949ca80a70b6ebdea37d3ab39ceea6698a \
+    --hash=sha256:d1f9282c5f2b5e241034a009779e7b2a1aa045f667ff521e7948ea9b56e0c5ff \
+    --hash=sha256:d265f09a75a79a788237d7f9054f929ced2e69eb0bb79de3798c468d8a90f945 \
+    --hash=sha256:db3fc6120bce9f446d13b1b834ea5b15341ca9ff3f335e4a951a6ead31105480 \
+    --hash=sha256:dbf3a08a06b3f433013c143ebd72c15cac33d2914b8ea4bea7ac2c23578815d6 \
+    --hash=sha256:de04b491d0e5007ee1b63a309956eaed959a49f5bb4e84b26c8f5d49de140fa9 \
+    --hash=sha256:e4b09863aae0dc965c3ef36500d891a3ff495a2ea9ae9171e4519963c12ceefd \
+    --hash=sha256:e595432ac259af2d4630008bf638873d69346372d38255774c0e286951e8b79f \
+    --hash=sha256:e75b89ac3bd27d2d043b234aa7b734c38ba1b0e43f07787130a0ecac1e12228a \
+    --hash=sha256:ea9eb976ffdd79d0e893869cfe179a8f60f152d42cb64622fca418cd9b18dc2a \
+    --hash=sha256:eafb3e874816ebe2a92f5e155f17260034c8c341dad1df25672fb710627c6949 \
+    --hash=sha256:ee3c36df21b5714d49fc4580247947aa64bcbe2939d1b77b4c8dcb8f6c9faecc \
+    --hash=sha256:f352b62b45dff37b55ddd7b9c0c8672c4dd2eb9c0f9c11d395075a84e2c40f75 \
+    --hash=sha256:fabb87dd8850ef0f7fe2b366d44b77d7e6fa2ea87861ab3844da99291e81e60f \
+    --hash=sha256:fe11310ae1e4cd560035598c3f29d86cef39a83d244c7466f95c27ae04850f10 \
+    --hash=sha256:fe7ba4a51f33ab275515f66b0a236bcde4fb5561498fe8f898d4e549b2e4509f
+    # via
+    #   -r requirements.in
+    #   adlfs
+    #   aiobotocore
+    #   gcsfs
+    #   s3fs
+aioitertools==0.11.0 \
+    --hash=sha256:04b95e3dab25b449def24d7df809411c10e62aab0cbe31a50ca4e68748c43394 \
+    --hash=sha256:42c68b8dd3a69c2bf7f2233bf7df4bb58b557bca5252ac02ed5187bbc67d6831
+    # via aiobotocore
+aiosignal==1.3.1 \
+    --hash=sha256:54cd96e15e1649b75d6c87526a6ff0b6c1b0dd3459f43d9ca11d48c339b68cfc \
+    --hash=sha256:f8376fb07dd1e86a584e4fcdec80b36b7f81aac666ebc724e2c090300dd83b17
+    # via aiohttp
 art==5.9 \
     --hash=sha256:6a311ec0a227c6554c6789e91e74c3f2c86453a2a8e76947788695b7a91ccff0 \
     --hash=sha256:9b02463468fc51c77200dadee970cf02c9576008c4f3b99d7ed02371ec037bd1
     # via -r requirements.in
-black==23.3.0 \
-    --hash=sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5 \
-    --hash=sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915 \
-    --hash=sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326 \
-    --hash=sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940 \
-    --hash=sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b \
-    --hash=sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30 \
-    --hash=sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c \
-    --hash=sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c \
-    --hash=sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab \
-    --hash=sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27 \
-    --hash=sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2 \
-    --hash=sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961 \
-    --hash=sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9 \
-    --hash=sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb \
-    --hash=sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70 \
-    --hash=sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331 \
-    --hash=sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2 \
-    --hash=sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266 \
-    --hash=sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d \
-    --hash=sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6 \
-    --hash=sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b \
-    --hash=sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925 \
-    --hash=sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8 \
-    --hash=sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4 \
-    --hash=sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3
-    # via -r requirements.in
-build==0.10.0 \
-    --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
-    --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
-    # via pip-tools
+async-timeout==4.0.2 \
+    --hash=sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15 \
+    --hash=sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c
+    # via aiohttp
+attrs==23.1.0 \
+    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
+    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
+    # via aiohttp
+azure-core==1.26.4 \
+    --hash=sha256:075fe06b74c3007950dd93d49440c2f3430fd9b4a5a2756ec8c79454afc989c6 \
+    --hash=sha256:d9664b4bc2675d72fba461a285ac43ae33abb2967014a955bf136d9703a2ab3c
+    # via
+    #   adlfs
+    #   azure-identity
+    #   azure-storage-blob
+azure-datalake-store==0.0.52 \
+    --hash=sha256:4198ddb32614d16d4502b43d5c9739f81432b7e0e4d75d30e05149fe6007fea2 \
+    --hash=sha256:aaed72b9c856824aeab554f4dbe0ef2c6d0ff36700bdd8b93d8298793117c48e
+    # via adlfs
+azure-identity==1.12.0 \
+    --hash=sha256:2a58ce4a209a013e37eaccfd5937570ab99e9118b3e1acf875eed3a85d541b92 \
+    --hash=sha256:7f9b1ae7d97ea7af3f38dd09305e19ab81a1e16ab66ea186b6579d85c1ca2347
+    # via adlfs
+azure-storage-blob==12.16.0 \
+    --hash=sha256:43b45f19a518a5c6895632f263b3825ebc23574f25cc84b66e1630a6160e466f \
+    --hash=sha256:91bb192b2a97939c4259c72373bac0f41e30810bbc853d5184f0f45904eacafd
+    # via adlfs
+botocore==1.27.59 \
+    --hash=sha256:69d756791fc024bda54f6c53f71ae34e695ee41bbbc1743d9179c4837a4929da \
+    --hash=sha256:eda4aed6ee719a745d1288eaf1beb12f6f6448ad1fa12f159405db14ba9c92cf
+    # via aiobotocore
+cachetools==5.3.0 \
+    --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
+    --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
+    # via google-auth
 certifi==2022.12.7 \
     --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
     --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
     # via requests
+cffi==1.15.1 \
+    --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
+    --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
+    --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
+    --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
+    --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
+    --hash=sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375 \
+    --hash=sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a \
+    --hash=sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e \
+    --hash=sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc \
+    --hash=sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf \
+    --hash=sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185 \
+    --hash=sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497 \
+    --hash=sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3 \
+    --hash=sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35 \
+    --hash=sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c \
+    --hash=sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83 \
+    --hash=sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21 \
+    --hash=sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca \
+    --hash=sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984 \
+    --hash=sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac \
+    --hash=sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd \
+    --hash=sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee \
+    --hash=sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a \
+    --hash=sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2 \
+    --hash=sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192 \
+    --hash=sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7 \
+    --hash=sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585 \
+    --hash=sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f \
+    --hash=sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e \
+    --hash=sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27 \
+    --hash=sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b \
+    --hash=sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e \
+    --hash=sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e \
+    --hash=sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d \
+    --hash=sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c \
+    --hash=sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415 \
+    --hash=sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82 \
+    --hash=sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02 \
+    --hash=sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314 \
+    --hash=sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325 \
+    --hash=sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c \
+    --hash=sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3 \
+    --hash=sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914 \
+    --hash=sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045 \
+    --hash=sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d \
+    --hash=sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9 \
+    --hash=sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5 \
+    --hash=sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2 \
+    --hash=sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c \
+    --hash=sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3 \
+    --hash=sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2 \
+    --hash=sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8 \
+    --hash=sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d \
+    --hash=sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d \
+    --hash=sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9 \
+    --hash=sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162 \
+    --hash=sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76 \
+    --hash=sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4 \
+    --hash=sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e \
+    --hash=sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9 \
+    --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
+    --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
+    --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
+    --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
+    # via
+    #   azure-datalake-store
+    #   cryptography
 charset-normalizer==3.1.0 \
     --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
     --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
     --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
     --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
     --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
     --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
@@ -115,279 +301,374 @@
     --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
     --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
     --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
     --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
     --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
     --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
     --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
-    # via requests
+    # via
+    #   aiohttp
+    #   requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
     #   -r requirements.in
-    #   black
-    #   mkdocs
-    #   mkdocs-click
-    #   pip-tools
     #   rich-click
-colorama==0.4.6 \
-    --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
-    --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-    # via
-    #   griffe
-    #   mkdocs-material
-coverage[toml]==7.2.5 \
-    --hash=sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3 \
-    --hash=sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a \
-    --hash=sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813 \
-    --hash=sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0 \
-    --hash=sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a \
-    --hash=sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd \
-    --hash=sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139 \
-    --hash=sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b \
-    --hash=sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252 \
-    --hash=sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790 \
-    --hash=sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045 \
-    --hash=sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce \
-    --hash=sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200 \
-    --hash=sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718 \
-    --hash=sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b \
-    --hash=sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f \
-    --hash=sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5 \
-    --hash=sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade \
-    --hash=sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5 \
-    --hash=sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a \
-    --hash=sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8 \
-    --hash=sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33 \
-    --hash=sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e \
-    --hash=sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c \
-    --hash=sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3 \
-    --hash=sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969 \
-    --hash=sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068 \
-    --hash=sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2 \
-    --hash=sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771 \
-    --hash=sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed \
-    --hash=sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212 \
-    --hash=sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614 \
-    --hash=sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88 \
-    --hash=sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3 \
-    --hash=sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c \
-    --hash=sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84 \
-    --hash=sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11 \
-    --hash=sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1 \
-    --hash=sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1 \
-    --hash=sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e \
-    --hash=sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1 \
-    --hash=sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd \
-    --hash=sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47 \
-    --hash=sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a \
-    --hash=sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c \
-    --hash=sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31 \
-    --hash=sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5 \
-    --hash=sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6 \
-    --hash=sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303 \
-    --hash=sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5 \
-    --hash=sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47
-    # via pytest-cov
-exceptiongroup==1.1.1 \
-    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
-    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
-    # via pytest
+cryptography==40.0.2 \
+    --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
+    --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
+    --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
+    --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
+    --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
+    --hash=sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d \
+    --hash=sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a \
+    --hash=sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404 \
+    --hash=sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b \
+    --hash=sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e \
+    --hash=sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2 \
+    --hash=sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c \
+    --hash=sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b \
+    --hash=sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9 \
+    --hash=sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b \
+    --hash=sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636 \
+    --hash=sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99 \
+    --hash=sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e \
+    --hash=sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9
+    # via
+    #   adal
+    #   azure-identity
+    #   azure-storage-blob
+    #   msal
+    #   pyjwt
+decorator==5.1.1 \
+    --hash=sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330 \
+    --hash=sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186
+    # via gcsfs
+frozenlist==1.3.3 \
+    --hash=sha256:008a054b75d77c995ea26629ab3a0c0d7281341f2fa7e1e85fa6153ae29ae99c \
+    --hash=sha256:02c9ac843e3390826a265e331105efeab489ffaf4dd86384595ee8ce6d35ae7f \
+    --hash=sha256:034a5c08d36649591be1cbb10e09da9f531034acfe29275fc5454a3b101ce41a \
+    --hash=sha256:05cdb16d09a0832eedf770cb7bd1fe57d8cf4eaf5aced29c4e41e3f20b30a784 \
+    --hash=sha256:0693c609e9742c66ba4870bcee1ad5ff35462d5ffec18710b4ac89337ff16e27 \
+    --hash=sha256:0771aed7f596c7d73444c847a1c16288937ef988dc04fb9f7be4b2aa91db609d \
+    --hash=sha256:0af2e7c87d35b38732e810befb9d797a99279cbb85374d42ea61c1e9d23094b3 \
+    --hash=sha256:14143ae966a6229350021384870458e4777d1eae4c28d1a7aa47f24d030e6678 \
+    --hash=sha256:180c00c66bde6146a860cbb81b54ee0df350d2daf13ca85b275123bbf85de18a \
+    --hash=sha256:1841e200fdafc3d51f974d9d377c079a0694a8f06de2e67b48150328d66d5483 \
+    --hash=sha256:23d16d9f477bb55b6154654e0e74557040575d9d19fe78a161bd33d7d76808e8 \
+    --hash=sha256:2b07ae0c1edaa0a36339ec6cce700f51b14a3fc6545fdd32930d2c83917332cf \
+    --hash=sha256:2c926450857408e42f0bbc295e84395722ce74bae69a3b2aa2a65fe22cb14b99 \
+    --hash=sha256:2e24900aa13212e75e5b366cb9065e78bbf3893d4baab6052d1aca10d46d944c \
+    --hash=sha256:303e04d422e9b911a09ad499b0368dc551e8c3cd15293c99160c7f1f07b59a48 \
+    --hash=sha256:352bd4c8c72d508778cf05ab491f6ef36149f4d0cb3c56b1b4302852255d05d5 \
+    --hash=sha256:3843f84a6c465a36559161e6c59dce2f2ac10943040c2fd021cfb70d58c4ad56 \
+    --hash=sha256:394c9c242113bfb4b9aa36e2b80a05ffa163a30691c7b5a29eba82e937895d5e \
+    --hash=sha256:3bbdf44855ed8f0fbcd102ef05ec3012d6a4fd7c7562403f76ce6a52aeffb2b1 \
+    --hash=sha256:40de71985e9042ca00b7953c4f41eabc3dc514a2d1ff534027f091bc74416401 \
+    --hash=sha256:41fe21dc74ad3a779c3d73a2786bdf622ea81234bdd4faf90b8b03cad0c2c0b4 \
+    --hash=sha256:47df36a9fe24054b950bbc2db630d508cca3aa27ed0566c0baf661225e52c18e \
+    --hash=sha256:4ea42116ceb6bb16dbb7d526e242cb6747b08b7710d9782aa3d6732bd8d27649 \
+    --hash=sha256:58bcc55721e8a90b88332d6cd441261ebb22342e238296bb330968952fbb3a6a \
+    --hash=sha256:5c11e43016b9024240212d2a65043b70ed8dfd3b52678a1271972702d990ac6d \
+    --hash=sha256:5cf820485f1b4c91e0417ea0afd41ce5cf5965011b3c22c400f6d144296ccbc0 \
+    --hash=sha256:5d8860749e813a6f65bad8285a0520607c9500caa23fea6ee407e63debcdbef6 \
+    --hash=sha256:6327eb8e419f7d9c38f333cde41b9ae348bec26d840927332f17e887a8dcb70d \
+    --hash=sha256:65a5e4d3aa679610ac6e3569e865425b23b372277f89b5ef06cf2cdaf1ebf22b \
+    --hash=sha256:66080ec69883597e4d026f2f71a231a1ee9887835902dbe6b6467d5a89216cf6 \
+    --hash=sha256:783263a4eaad7c49983fe4b2e7b53fa9770c136c270d2d4bbb6d2192bf4d9caf \
+    --hash=sha256:7f44e24fa70f6fbc74aeec3e971f60a14dde85da364aa87f15d1be94ae75aeef \
+    --hash=sha256:7fdfc24dcfce5b48109867c13b4cb15e4660e7bd7661741a391f821f23dfdca7 \
+    --hash=sha256:810860bb4bdce7557bc0febb84bbd88198b9dbc2022d8eebe5b3590b2ad6c842 \
+    --hash=sha256:841ea19b43d438a80b4de62ac6ab21cfe6827bb8a9dc62b896acc88eaf9cecba \
+    --hash=sha256:84610c1502b2461255b4c9b7d5e9c48052601a8957cd0aea6ec7a7a1e1fb9420 \
+    --hash=sha256:899c5e1928eec13fd6f6d8dc51be23f0d09c5281e40d9cf4273d188d9feeaf9b \
+    --hash=sha256:8bae29d60768bfa8fb92244b74502b18fae55a80eac13c88eb0b496d4268fd2d \
+    --hash=sha256:8df3de3a9ab8325f94f646609a66cbeeede263910c5c0de0101079ad541af332 \
+    --hash=sha256:8fa3c6e3305aa1146b59a09b32b2e04074945ffcfb2f0931836d103a2c38f936 \
+    --hash=sha256:924620eef691990dfb56dc4709f280f40baee568c794b5c1885800c3ecc69816 \
+    --hash=sha256:9309869032abb23d196cb4e4db574232abe8b8be1339026f489eeb34a4acfd91 \
+    --hash=sha256:9545a33965d0d377b0bc823dcabf26980e77f1b6a7caa368a365a9497fb09420 \
+    --hash=sha256:9ac5995f2b408017b0be26d4a1d7c61bce106ff3d9e3324374d66b5964325448 \
+    --hash=sha256:9bbbcedd75acdfecf2159663b87f1bb5cfc80e7cd99f7ddd9d66eb98b14a8411 \
+    --hash=sha256:a4ae8135b11652b08a8baf07631d3ebfe65a4c87909dbef5fa0cdde440444ee4 \
+    --hash=sha256:a6394d7dadd3cfe3f4b3b186e54d5d8504d44f2d58dcc89d693698e8b7132b32 \
+    --hash=sha256:a97b4fe50b5890d36300820abd305694cb865ddb7885049587a5678215782a6b \
+    --hash=sha256:ae4dc05c465a08a866b7a1baf360747078b362e6a6dbeb0c57f234db0ef88ae0 \
+    --hash=sha256:b1c63e8d377d039ac769cd0926558bb7068a1f7abb0f003e3717ee003ad85530 \
+    --hash=sha256:b1e2c1185858d7e10ff045c496bbf90ae752c28b365fef2c09cf0fa309291669 \
+    --hash=sha256:b4395e2f8d83fbe0c627b2b696acce67868793d7d9750e90e39592b3626691b7 \
+    --hash=sha256:b756072364347cb6aa5b60f9bc18e94b2f79632de3b0190253ad770c5df17db1 \
+    --hash=sha256:ba64dc2b3b7b158c6660d49cdb1d872d1d0bf4e42043ad8d5006099479a194e5 \
+    --hash=sha256:bed331fe18f58d844d39ceb398b77d6ac0b010d571cba8267c2e7165806b00ce \
+    --hash=sha256:c188512b43542b1e91cadc3c6c915a82a5eb95929134faf7fd109f14f9892ce4 \
+    --hash=sha256:c21b9aa40e08e4f63a2f92ff3748e6b6c84d717d033c7b3438dd3123ee18f70e \
+    --hash=sha256:ca713d4af15bae6e5d79b15c10c8522859a9a89d3b361a50b817c98c2fb402a2 \
+    --hash=sha256:cd4210baef299717db0a600d7a3cac81d46ef0e007f88c9335db79f8979c0d3d \
+    --hash=sha256:cfe33efc9cb900a4c46f91a5ceba26d6df370ffddd9ca386eb1d4f0ad97b9ea9 \
+    --hash=sha256:d5cd3ab21acbdb414bb6c31958d7b06b85eeb40f66463c264a9b343a4e238642 \
+    --hash=sha256:dfbac4c2dfcc082fcf8d942d1e49b6aa0766c19d3358bd86e2000bf0fa4a9cf0 \
+    --hash=sha256:e235688f42b36be2b6b06fc37ac2126a73b75fb8d6bc66dd632aa35286238703 \
+    --hash=sha256:eb82dbba47a8318e75f679690190c10a5e1f447fbf9df41cbc4c3afd726d88cb \
+    --hash=sha256:ebb86518203e12e96af765ee89034a1dbb0c3c65052d1b0c19bbbd6af8a145e1 \
+    --hash=sha256:ee78feb9d293c323b59a6f2dd441b63339a30edf35abcb51187d2fc26e696d13 \
+    --hash=sha256:eedab4c310c0299961ac285591acd53dc6723a1ebd90a57207c71f6e0c2153ab \
+    --hash=sha256:efa568b885bca461f7c7b9e032655c0c143d305bf01c30caf6db2854a4532b38 \
+    --hash=sha256:efce6ae830831ab6a22b9b4091d411698145cb9b8fc869e1397ccf4b4b6455cb \
+    --hash=sha256:f163d2fd041c630fed01bc48d28c3ed4a3b003c00acd396900e11ee5316b56bb \
+    --hash=sha256:f20380df709d91525e4bee04746ba612a4df0972c1b8f8e1e8af997e678c7b81 \
+    --hash=sha256:f30f1928162e189091cf4d9da2eac617bfe78ef907a761614ff577ef4edfb3c8 \
+    --hash=sha256:f470c92737afa7d4c3aacc001e335062d582053d4dbe73cda126f2d7031068dd \
+    --hash=sha256:ff8bf625fe85e119553b5383ba0fb6aa3d0ec2ae980295aaefa552374926b3f4
+    # via
+    #   aiohttp
+    #   aiosignal
 fsspec==2023.1.0 \
     --hash=sha256:b833e2e541e9e8cde0ab549414187871243177feb3d344f9d27b25a93f5d8139 \
     --hash=sha256:fbae7f20ff801eb5f7d0bedf81f25c787c0dfac5e982d98fa3884a9cde2b5411
     # via
     #   -r requirements.in
+    #   adlfs
+    #   gcsfs
+    #   s3fs
     #   universal-pathlib
-ghp-import==2.1.0 \
-    --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
-    --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
-    # via mkdocs
-griffe==0.27.2 \
-    --hash=sha256:833990074c8c0b323a55f37f72265fdd841cb0a756122303505bf4bc80800e82 \
-    --hash=sha256:8d6bc40e7bede3fb5879598c1f71b8902d245804ab59ae55516f864b2bdc25c6
-    # via mkdocstrings-python
+gcsfs==2023.1.0 \
+    --hash=sha256:0a7b7ca8c1affa126a14ba35d7b7dff81c49e2aaceedda9732c7f159a4837a26 \
+    --hash=sha256:62c491b9e2a8e9e58b8a899eec2ce111f827718a65539019ff3cadf447e48f41
+    # via -r requirements.in
+google-api-core==2.11.0 \
+    --hash=sha256:4b9bb5d5a380a0befa0573b302651b8a9a89262c1730e37bf423cec511804c22 \
+    --hash=sha256:ce222e27b0de0d7bc63eb043b956996d6dccab14cc3b690aaea91c9cc99dc16e
+    # via
+    #   google-cloud-core
+    #   google-cloud-storage
+google-auth==2.17.3 \
+    --hash=sha256:ce311e2bc58b130fddf316df57c9b3943c2a7b4f6ec31de9663a9333e4064efc \
+    --hash=sha256:f586b274d3eb7bd932ea424b1c702a30e0393a2e2bc4ca3eae8263ffd8be229f
+    # via
+    #   gcsfs
+    #   google-api-core
+    #   google-auth-oauthlib
+    #   google-cloud-core
+    #   google-cloud-storage
+google-auth-oauthlib==1.0.0 \
+    --hash=sha256:95880ca704928c300f48194d1770cf5b1462835b6e49db61445a520f793fd5fb \
+    --hash=sha256:e375064964820b47221a7e1b7ee1fd77051b6323c3f9e3e19785f78ab67ecfc5
+    # via gcsfs
+google-cloud-core==2.3.2 \
+    --hash=sha256:8417acf6466be2fa85123441696c4badda48db314c607cf1e5d543fa8bdc22fe \
+    --hash=sha256:b9529ee7047fd8d4bf4a2182de619154240df17fbe60ead399078c1ae152af9a
+    # via google-cloud-storage
+google-cloud-storage==2.8.0 \
+    --hash=sha256:248e210c13bc109909160248af546a91cb2dabaf3d7ebbf04def9dd49f02dbb6 \
+    --hash=sha256:4388da1ff5bda6d729f26dbcaf1bfa020a2a52a7b91f0a8123edbda51660802c
+    # via gcsfs
+google-crc32c==1.5.0 \
+    --hash=sha256:024894d9d3cfbc5943f8f230e23950cd4906b2fe004c72e29b209420a1e6b05a \
+    --hash=sha256:02c65b9817512edc6a4ae7c7e987fea799d2e0ee40c53ec573a692bee24de876 \
+    --hash=sha256:02ebb8bf46c13e36998aeaad1de9b48f4caf545e91d14041270d9dca767b780c \
+    --hash=sha256:07eb3c611ce363c51a933bf6bd7f8e3878a51d124acfc89452a75120bc436289 \
+    --hash=sha256:1034d91442ead5a95b5aaef90dbfaca8633b0247d1e41621d1e9f9db88c36298 \
+    --hash=sha256:116a7c3c616dd14a3de8c64a965828b197e5f2d121fedd2f8c5585c547e87b02 \
+    --hash=sha256:19e0a019d2c4dcc5e598cd4a4bc7b008546b0358bd322537c74ad47a5386884f \
+    --hash=sha256:1c7abdac90433b09bad6c43a43af253e688c9cfc1c86d332aed13f9a7c7f65e2 \
+    --hash=sha256:1e986b206dae4476f41bcec1faa057851f3889503a70e1bdb2378d406223994a \
+    --hash=sha256:272d3892a1e1a2dbc39cc5cde96834c236d5327e2122d3aaa19f6614531bb6eb \
+    --hash=sha256:278d2ed7c16cfc075c91378c4f47924c0625f5fc84b2d50d921b18b7975bd210 \
+    --hash=sha256:2ad40e31093a4af319dadf503b2467ccdc8f67c72e4bcba97f8c10cb078207b5 \
+    --hash=sha256:2e920d506ec85eb4ba50cd4228c2bec05642894d4c73c59b3a2fe20346bd00ee \
+    --hash=sha256:3359fc442a743e870f4588fcf5dcbc1bf929df1fad8fb9905cd94e5edb02e84c \
+    --hash=sha256:37933ec6e693e51a5b07505bd05de57eee12f3e8c32b07da7e73669398e6630a \
+    --hash=sha256:398af5e3ba9cf768787eef45c803ff9614cc3e22a5b2f7d7ae116df8b11e3314 \
+    --hash=sha256:3b747a674c20a67343cb61d43fdd9207ce5da6a99f629c6e2541aa0e89215bcd \
+    --hash=sha256:461665ff58895f508e2866824a47bdee72497b091c730071f2b7575d5762ab65 \
+    --hash=sha256:4c6fdd4fccbec90cc8a01fc00773fcd5fa28db683c116ee3cb35cd5da9ef6c37 \
+    --hash=sha256:5829b792bf5822fd0a6f6eb34c5f81dd074f01d570ed7f36aa101d6fc7a0a6e4 \
+    --hash=sha256:596d1f98fc70232fcb6590c439f43b350cb762fb5d61ce7b0e9db4539654cc13 \
+    --hash=sha256:5ae44e10a8e3407dbe138984f21e536583f2bba1be9491239f942c2464ac0894 \
+    --hash=sha256:635f5d4dd18758a1fbd1049a8e8d2fee4ffed124462d837d1a02a0e009c3ab31 \
+    --hash=sha256:64e52e2b3970bd891309c113b54cf0e4384762c934d5ae56e283f9a0afcd953e \
+    --hash=sha256:66741ef4ee08ea0b2cc3c86916ab66b6aef03768525627fd6a1b34968b4e3709 \
+    --hash=sha256:67b741654b851abafb7bc625b6d1cdd520a379074e64b6a128e3b688c3c04740 \
+    --hash=sha256:6ac08d24c1f16bd2bf5eca8eaf8304812f44af5cfe5062006ec676e7e1d50afc \
+    --hash=sha256:6f998db4e71b645350b9ac28a2167e6632c239963ca9da411523bb439c5c514d \
+    --hash=sha256:72218785ce41b9cfd2fc1d6a017dc1ff7acfc4c17d01053265c41a2c0cc39b8c \
+    --hash=sha256:74dea7751d98034887dbd821b7aae3e1d36eda111d6ca36c206c44478035709c \
+    --hash=sha256:759ce4851a4bb15ecabae28f4d2e18983c244eddd767f560165563bf9aefbc8d \
+    --hash=sha256:77e2fd3057c9d78e225fa0a2160f96b64a824de17840351b26825b0848022906 \
+    --hash=sha256:7c074fece789b5034b9b1404a1f8208fc2d4c6ce9decdd16e8220c5a793e6f61 \
+    --hash=sha256:7c42c70cd1d362284289c6273adda4c6af8039a8ae12dc451dcd61cdabb8ab57 \
+    --hash=sha256:7f57f14606cd1dd0f0de396e1e53824c371e9544a822648cd76c034d209b559c \
+    --hash=sha256:83c681c526a3439b5cf94f7420471705bbf96262f49a6fe546a6db5f687a3d4a \
+    --hash=sha256:8485b340a6a9e76c62a7dce3c98e5f102c9219f4cfbf896a00cf48caf078d438 \
+    --hash=sha256:84e6e8cd997930fc66d5bb4fde61e2b62ba19d62b7abd7a69920406f9ecca946 \
+    --hash=sha256:89284716bc6a5a415d4eaa11b1726d2d60a0cd12aadf5439828353662ede9dd7 \
+    --hash=sha256:8b87e1a59c38f275c0e3676fc2ab6d59eccecfd460be267ac360cc31f7bcde96 \
+    --hash=sha256:8f24ed114432de109aa9fd317278518a5af2d31ac2ea6b952b2f7782b43da091 \
+    --hash=sha256:98cb4d057f285bd80d8778ebc4fde6b4d509ac3f331758fb1528b733215443ae \
+    --hash=sha256:998679bf62b7fb599d2878aa3ed06b9ce688b8974893e7223c60db155f26bd8d \
+    --hash=sha256:9ba053c5f50430a3fcfd36f75aff9caeba0440b2d076afdb79a318d6ca245f88 \
+    --hash=sha256:9c99616c853bb585301df6de07ca2cadad344fd1ada6d62bb30aec05219c45d2 \
+    --hash=sha256:a1fd716e7a01f8e717490fbe2e431d2905ab8aa598b9b12f8d10abebb36b04dd \
+    --hash=sha256:a2355cba1f4ad8b6988a4ca3feed5bff33f6af2d7f134852cf279c2aebfde541 \
+    --hash=sha256:b1f8133c9a275df5613a451e73f36c2aea4fe13c5c8997e22cf355ebd7bd0728 \
+    --hash=sha256:b8667b48e7a7ef66afba2c81e1094ef526388d35b873966d8a9a447974ed9178 \
+    --hash=sha256:ba1eb1843304b1e5537e1fca632fa894d6f6deca8d6389636ee5b4797affb968 \
+    --hash=sha256:be82c3c8cfb15b30f36768797a640e800513793d6ae1724aaaafe5bf86f8f346 \
+    --hash=sha256:c02ec1c5856179f171e032a31d6f8bf84e5a75c45c33b2e20a3de353b266ebd8 \
+    --hash=sha256:c672d99a345849301784604bfeaeba4db0c7aae50b95be04dd651fd2a7310b93 \
+    --hash=sha256:c6c777a480337ac14f38564ac88ae82d4cd238bf293f0a22295b66eb89ffced7 \
+    --hash=sha256:cae0274952c079886567f3f4f685bcaf5708f0a23a5f5216fdab71f81a6c0273 \
+    --hash=sha256:cd67cf24a553339d5062eff51013780a00d6f97a39ca062781d06b3a73b15462 \
+    --hash=sha256:d3515f198eaa2f0ed49f8819d5732d70698c3fa37384146079b3799b97667a94 \
+    --hash=sha256:d5280312b9af0976231f9e317c20e4a61cd2f9629b7bfea6a693d1878a264ebd \
+    --hash=sha256:de06adc872bcd8c2a4e0dc51250e9e65ef2ca91be023b9d13ebd67c2ba552e1e \
+    --hash=sha256:e1674e4307fa3024fc897ca774e9c7562c957af85df55efe2988ed9056dc4e57 \
+    --hash=sha256:e2096eddb4e7c7bdae4bd69ad364e55e07b8316653234a56552d9c988bd2d61b \
+    --hash=sha256:e560628513ed34759456a416bf86b54b2476c59144a9138165c9a1575801d0d9 \
+    --hash=sha256:edfedb64740750e1a3b16152620220f51d58ff1b4abceb339ca92e934775c27a \
+    --hash=sha256:f13cae8cc389a440def0c8c52057f37359014ccbc9dc1f0827936bcd367c6100 \
+    --hash=sha256:f314013e7dcd5cf45ab1945d92e713eec788166262ae8deb2cfacd53def27325 \
+    --hash=sha256:f583edb943cf2e09c60441b910d6a20b4d9d626c75a36c8fcac01a6c96c01183 \
+    --hash=sha256:fd8536e902db7e365f49e7d9029283403974ccf29b13fc7028b97e2295b33556 \
+    --hash=sha256:fe70e325aa68fa4b5edf7d1a4b6f691eb04bbccac0ace68e34820d283b5f80d4
+    # via google-resumable-media
+google-resumable-media==2.5.0 \
+    --hash=sha256:218931e8e2b2a73a58eb354a288e03a0fd5fb1c4583261ac6e4c078666468c93 \
+    --hash=sha256:da1bd943e2e114a56d85d6848497ebf9be6a14d3db23e9fc57581e7c3e8170ec
+    # via google-cloud-storage
+googleapis-common-protos==1.59.0 \
+    --hash=sha256:4168fcb568a826a52f23510412da405abd93f4d23ba544bb68d943b14ba3cb44 \
+    --hash=sha256:b287dc48449d1d41af0c69f4ea26242b5ae4c3d7249a38b0984c86a4caffff1f
+    # via google-api-core
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
-    # via requests
+    # via
+    #   requests
+    #   yarl
 importlib-metadata==6.6.0 \
     --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
     --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
-    # via
-    #   markdown
-    #   mkdocs
-    #   textual
-iniconfig==2.0.0 \
-    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
-    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-    # via pytest
-jinja2==3.1.2 \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-    # via
-    #   mkdocs
-    #   mkdocs-material
-    #   mkdocstrings
+    # via textual
+isodate==0.6.1 \
+    --hash=sha256:0751eece944162659049d35f4f549ed815792b38793f07cf73381c1c87cbed96 \
+    --hash=sha256:48c5881de7e8b0a0d648cb024c8062dc84e7b840ed81e864c7614fd3c127bde9
+    # via azure-storage-blob
+jmespath==1.0.1 \
+    --hash=sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980 \
+    --hash=sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe
+    # via botocore
 linkify-it-py==2.0.2 \
     --hash=sha256:19f3060727842c254c808e99d465c80c49d2c7306788140987a1a7a29b0d6ad2 \
     --hash=sha256:a3a24428f6c96f27370d7fe61d2ac0be09017be5190d68d8658233171f1b6541
     # via markdown-it-py
-markdown==3.3.7 \
-    --hash=sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874 \
-    --hash=sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621
-    # via
-    #   mkdocs
-    #   mkdocs-autorefs
-    #   mkdocs-click
-    #   mkdocs-material
-    #   mkdocstrings
-    #   pymdown-extensions
 markdown-it-py[linkify,plugins]==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
-markupsafe==2.1.2 \
-    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
-    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
-    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
-    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
-    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
-    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
-    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
-    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
-    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
-    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
-    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
-    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
-    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
-    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
-    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
-    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
-    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
-    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
-    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
-    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
-    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
-    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
-    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
-    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
-    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
-    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
-    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
-    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
-    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
-    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
-    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
-    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
-    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
-    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
-    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
-    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
-    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
-    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
-    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
-    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
-    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
-    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
-    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
-    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
-    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
-    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
-    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
-    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
-    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
-    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
-    # via
-    #   jinja2
-    #   mkdocstrings
 mdit-py-plugins==0.3.5 \
     --hash=sha256:ca9a0714ea59a24b2b044a1831f48d817dd0c817e84339f20e7889f392d77c4e \
     --hash=sha256:eee0adc7195e5827e17e02d2a258a2ba159944a0748f59c5099a4a27f78fcf6a
     # via markdown-it-py
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-mergedeep==1.3.4 \
-    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
-    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-    # via mkdocs
-mkdocs==1.4.3 \
-    --hash=sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57 \
-    --hash=sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd
-    # via
-    #   -r requirements.in
-    #   mkdocs-autorefs
-    #   mkdocs-material
-    #   mkdocstrings
-mkdocs-autorefs==0.4.1 \
-    --hash=sha256:70748a7bd025f9ecd6d6feeba8ba63f8e891a1af55f48e366d6d6e78493aba84 \
-    --hash=sha256:a2248a9501b29dc0cc8ba4c09f4f47ff121945f6ce33d760f145d6f89d313f5b
-    # via mkdocstrings
-mkdocs-click==0.8.0 \
-    --hash=sha256:965f38231eb04d8c980406c5ab4becf7303ef3ffc68fdb29be91927eff1adfbe \
-    --hash=sha256:f9c26d4abd505bca4113d1529d03d1ae709a68a82fc364db289634788d029353
-    # via -r requirements.in
-mkdocs-material==9.1.9 \
-    --hash=sha256:74d8da1371ab3a326868fe47bae3cbc4aa22e93c048b4ca5117e6817b88bd734 \
-    --hash=sha256:7db24261cb17400e132c46d17eea712bfe71056d892a9beba32cf68210297141
-    # via -r requirements.in
-mkdocs-material-extensions==1.1.1 \
-    --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
-    --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
-    # via mkdocs-material
-mkdocstrings[python]==0.21.2 \
-    --hash=sha256:304e56a2e90595708a38a13a278e538a67ad82052dd5c8b71f77a604a4f3d911 \
-    --hash=sha256:949ef8da92df9d692ca07be50616459a6b536083a25520fd54b00e8814ce019b
+msal==1.22.0 \
+    --hash=sha256:8a82f5375642c1625c89058018430294c109440dce42ea667d466c2cab520acd \
+    --hash=sha256:9120b7eafdf061c92f7b3d744e5f325fca35873445fa8ffebb40b1086a13dd58
     # via
-    #   -r requirements.in
-    #   mkdocstrings-python
-mkdocstrings-python==0.9.0 \
-    --hash=sha256:00e02b5d3d444f9abdec2398f9ba0c73e15deab78685f793f5801fd4d62a5b6f \
-    --hash=sha256:da0a54d7d46523a25a5227f0ecc74b491291bd9d36fc71445bfb0ea64283e287
-    # via mkdocstrings
-mypy==1.2.0 \
-    --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
-    --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
-    --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
-    --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
-    --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
-    --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
-    --hash=sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41 \
-    --hash=sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f \
-    --hash=sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e \
-    --hash=sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8 \
-    --hash=sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238 \
-    --hash=sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119 \
-    --hash=sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb \
-    --hash=sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d \
-    --hash=sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed \
-    --hash=sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9 \
-    --hash=sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e \
-    --hash=sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a \
-    --hash=sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5 \
-    --hash=sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950 \
-    --hash=sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937 \
-    --hash=sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394 \
-    --hash=sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6 \
-    --hash=sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602 \
-    --hash=sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1 \
-    --hash=sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba
-    # via -r requirements.in
-mypy-extensions==1.0.0 \
-    --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
-    --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
+    #   azure-identity
+    #   msal-extensions
+msal-extensions==1.0.0 \
+    --hash=sha256:91e3db9620b822d0ed2b4d1850056a0f133cba04455e62f11612e40f5502f2ee \
+    --hash=sha256:c676aba56b0cce3783de1b5c5ecfe828db998167875126ca4b47dc6436451354
+    # via azure-identity
+multidict==6.0.4 \
+    --hash=sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9 \
+    --hash=sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8 \
+    --hash=sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03 \
+    --hash=sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710 \
+    --hash=sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161 \
+    --hash=sha256:16ab77bbeb596e14212e7bab8429f24c1579234a3a462105cda4a66904998664 \
+    --hash=sha256:16d232d4e5396c2efbbf4f6d4df89bfa905eb0d4dc5b3549d872ab898451f569 \
+    --hash=sha256:21a12c4eb6ddc9952c415f24eef97e3e55ba3af61f67c7bc388dcdec1404a067 \
+    --hash=sha256:27c523fbfbdfd19c6867af7346332b62b586eed663887392cff78d614f9ec313 \
+    --hash=sha256:281af09f488903fde97923c7744bb001a9b23b039a909460d0f14edc7bf59706 \
+    --hash=sha256:33029f5734336aa0d4c0384525da0387ef89148dc7191aae00ca5fb23d7aafc2 \
+    --hash=sha256:3601a3cece3819534b11d4efc1eb76047488fddd0c85a3948099d5da4d504636 \
+    --hash=sha256:3666906492efb76453c0e7b97f2cf459b0682e7402c0489a95484965dbc1da49 \
+    --hash=sha256:36c63aaa167f6c6b04ef2c85704e93af16c11d20de1d133e39de6a0e84582a93 \
+    --hash=sha256:39ff62e7d0f26c248b15e364517a72932a611a9b75f35b45be078d81bdb86603 \
+    --hash=sha256:43644e38f42e3af682690876cff722d301ac585c5b9e1eacc013b7a3f7b696a0 \
+    --hash=sha256:4372381634485bec7e46718edc71528024fcdc6f835baefe517b34a33c731d60 \
+    --hash=sha256:458f37be2d9e4c95e2d8866a851663cbc76e865b78395090786f6cd9b3bbf4f4 \
+    --hash=sha256:45e1ecb0379bfaab5eef059f50115b54571acfbe422a14f668fc8c27ba410e7e \
+    --hash=sha256:4b9d9e4e2b37daddb5c23ea33a3417901fa7c7b3dee2d855f63ee67a0b21e5b1 \
+    --hash=sha256:4ceef517eca3e03c1cceb22030a3e39cb399ac86bff4e426d4fc6ae49052cc60 \
+    --hash=sha256:4d1a3d7ef5e96b1c9e92f973e43aa5e5b96c659c9bc3124acbbd81b0b9c8a951 \
+    --hash=sha256:4dcbb0906e38440fa3e325df2359ac6cb043df8e58c965bb45f4e406ecb162cc \
+    --hash=sha256:509eac6cf09c794aa27bcacfd4d62c885cce62bef7b2c3e8b2e49d365b5003fe \
+    --hash=sha256:52509b5be062d9eafc8170e53026fbc54cf3b32759a23d07fd935fb04fc22d95 \
+    --hash=sha256:52f2dffc8acaba9a2f27174c41c9e57f60b907bb9f096b36b1a1f3be71c6284d \
+    --hash=sha256:574b7eae1ab267e5f8285f0fe881f17efe4b98c39a40858247720935b893bba8 \
+    --hash=sha256:5979b5632c3e3534e42ca6ff856bb24b2e3071b37861c2c727ce220d80eee9ed \
+    --hash=sha256:59d43b61c59d82f2effb39a93c48b845efe23a3852d201ed2d24ba830d0b4cf2 \
+    --hash=sha256:5a4dcf02b908c3b8b17a45fb0f15b695bf117a67b76b7ad18b73cf8e92608775 \
+    --hash=sha256:5cad9430ab3e2e4fa4a2ef4450f548768400a2ac635841bc2a56a2052cdbeb87 \
+    --hash=sha256:5fc1b16f586f049820c5c5b17bb4ee7583092fa0d1c4e28b5239181ff9532e0c \
+    --hash=sha256:62501642008a8b9871ddfccbf83e4222cf8ac0d5aeedf73da36153ef2ec222d2 \
+    --hash=sha256:64bdf1086b6043bf519869678f5f2757f473dee970d7abf6da91ec00acb9cb98 \
+    --hash=sha256:64da238a09d6039e3bd39bb3aee9c21a5e34f28bfa5aa22518581f910ff94af3 \
+    --hash=sha256:666daae833559deb2d609afa4490b85830ab0dfca811a98b70a205621a6109fe \
+    --hash=sha256:67040058f37a2a51ed8ea8f6b0e6ee5bd78ca67f169ce6122f3e2ec80dfe9b78 \
+    --hash=sha256:6748717bb10339c4760c1e63da040f5f29f5ed6e59d76daee30305894069a660 \
+    --hash=sha256:6b181d8c23da913d4ff585afd1155a0e1194c0b50c54fcfe286f70cdaf2b7176 \
+    --hash=sha256:6ed5f161328b7df384d71b07317f4d8656434e34591f20552c7bcef27b0ab88e \
+    --hash=sha256:7582a1d1030e15422262de9f58711774e02fa80df0d1578995c76214f6954988 \
+    --hash=sha256:7d18748f2d30f94f498e852c67d61261c643b349b9d2a581131725595c45ec6c \
+    --hash=sha256:7d6ae9d593ef8641544d6263c7fa6408cc90370c8cb2bbb65f8d43e5b0351d9c \
+    --hash=sha256:81a4f0b34bd92df3da93315c6a59034df95866014ac08535fc819f043bfd51f0 \
+    --hash=sha256:8316a77808c501004802f9beebde51c9f857054a0c871bd6da8280e718444449 \
+    --hash=sha256:853888594621e6604c978ce2a0444a1e6e70c8d253ab65ba11657659dcc9100f \
+    --hash=sha256:99b76c052e9f1bc0721f7541e5e8c05db3941eb9ebe7b8553c625ef88d6eefde \
+    --hash=sha256:a2e4369eb3d47d2034032a26c7a80fcb21a2cb22e1173d761a162f11e562caa5 \
+    --hash=sha256:ab55edc2e84460694295f401215f4a58597f8f7c9466faec545093045476327d \
+    --hash=sha256:af048912e045a2dc732847d33821a9d84ba553f5c5f028adbd364dd4765092ac \
+    --hash=sha256:b1a2eeedcead3a41694130495593a559a668f382eee0727352b9a41e1c45759a \
+    --hash=sha256:b1e8b901e607795ec06c9e42530788c45ac21ef3aaa11dbd0c69de543bfb79a9 \
+    --hash=sha256:b41156839806aecb3641f3208c0dafd3ac7775b9c4c422d82ee2a45c34ba81ca \
+    --hash=sha256:b692f419760c0e65d060959df05f2a531945af31fda0c8a3b3195d4efd06de11 \
+    --hash=sha256:bc779e9e6f7fda81b3f9aa58e3a6091d49ad528b11ed19f6621408806204ad35 \
+    --hash=sha256:bf6774e60d67a9efe02b3616fee22441d86fab4c6d335f9d2051d19d90a40063 \
+    --hash=sha256:c048099e4c9e9d615545e2001d3d8a4380bd403e1a0578734e0d31703d1b0c0b \
+    --hash=sha256:c5cb09abb18c1ea940fb99360ea0396f34d46566f157122c92dfa069d3e0e982 \
+    --hash=sha256:cc8e1d0c705233c5dd0c5e6460fbad7827d5d36f310a0fadfd45cc3029762258 \
+    --hash=sha256:d5e3fc56f88cc98ef8139255cf8cd63eb2c586531e43310ff859d6bb3a6b51f1 \
+    --hash=sha256:d6aa0418fcc838522256761b3415822626f866758ee0bc6632c9486b179d0b52 \
+    --hash=sha256:d6c254ba6e45d8e72739281ebc46ea5eb5f101234f3ce171f0e9f5cc86991480 \
+    --hash=sha256:d6d635d5209b82a3492508cf5b365f3446afb65ae7ebd755e70e18f287b0adf7 \
+    --hash=sha256:dcfe792765fab89c365123c81046ad4103fcabbc4f56d1c1997e6715e8015461 \
+    --hash=sha256:ddd3915998d93fbcd2566ddf9cf62cdb35c9e093075f862935573d265cf8f65d \
+    --hash=sha256:ddff9c4e225a63a5afab9dd15590432c22e8057e1a9a13d28ed128ecf047bbdc \
+    --hash=sha256:e41b7e2b59679edfa309e8db64fdf22399eec4b0b24694e1b2104fb789207779 \
+    --hash=sha256:e69924bfcdda39b722ef4d9aa762b2dd38e4632b3641b1d9a57ca9cd18f2f83a \
+    --hash=sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547 \
+    --hash=sha256:ee2a1ece51b9b9e7752e742cfb661d2a29e7bcdba2d27e66e28a99f1890e4fa0 \
+    --hash=sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171 \
+    --hash=sha256:f70b98cd94886b49d91170ef23ec5c0e8ebb6f242d734ed7ed677b24d50c82cf \
+    --hash=sha256:fc35cb4676846ef752816d5be2193a1e8367b4c1397b74a565a9d0389c433a1d \
+    --hash=sha256:ff959bee35038c4624250473988b24f846cbeb2c6639de3602c073f10410ceba
     # via
-    #   black
-    #   mypy
+    #   aiohttp
+    #   yarl
 numpy==1.24.3 \
     --hash=sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187 \
     --hash=sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812 \
     --hash=sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7 \
     --hash=sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4 \
     --hash=sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6 \
     --hash=sha256:352ee00c7f8387b44d19f4cada524586f07379c0d49270f87233983bc5087ca0 \
@@ -409,23 +690,21 @@
     --hash=sha256:c91c4afd8abc3908e00a44b2672718905b8611503f7ff87390cc0ac3423fb096 \
     --hash=sha256:d5036197ecae68d7f491fcdb4df90082b0d4960ca6599ba2659957aafced7c17 \
     --hash=sha256:d6cc757de514c00b24ae8cf5c876af2a7c3df189028d68c0cb4eaa9cd5afc2bf \
     --hash=sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4 \
     --hash=sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02 \
     --hash=sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c \
     --hash=sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b
-    # via pandas
-packaging==23.1 \
-    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
-    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
-    # via
-    #   black
-    #   build
-    #   mkdocs
-    #   pytest
+    # via
+    #   pandas
+    #   pyarrow
+oauthlib==3.2.2 \
+    --hash=sha256:8139f29aac13e25d502680e9e19963e83f16838d48a0d71c287fe40e7067fbca \
+    --hash=sha256:9859c40929662bec5d64f34d01c99e093149682a3f38915dc0655d5a633dd918
+    # via requests-oauthlib
 pandas==1.5.3 \
     --hash=sha256:14e45300521902689a81f3f41386dc86f19b8ba8dd5ac5a3c7010ef8d2932813 \
     --hash=sha256:26d9c71772c7afb9d5046e6e9cf42d83dd147b5cf5bcb9d97252077118543792 \
     --hash=sha256:3749077d86e3a2f0ed51367f30bf5b82e131cc0f14260c4d3e499186fccc4406 \
     --hash=sha256:41179ce559943d83a9b4bbacb736b04c928b095b5f25dd2b7389eda08f46f373 \
     --hash=sha256:478ff646ca42b20376e4ed3fa2e8d7341e8a63105586efe54fa2508ee087f328 \
     --hash=sha256:50869a35cbb0f2e0cd5ec04b191e7b12ed688874bd05dd777c19b28cbea90996 \
@@ -447,22 +726,14 @@
     --hash=sha256:c4c00e0b0597c8e4f59e8d461f797e5d70b4d025880516a8261b2817c47759ee \
     --hash=sha256:c74a62747864ed568f5a82a49a23a8d7fe171d0c69038b38cedf0976831296fa \
     --hash=sha256:dd05f7783b3274aa206a1af06f0ceed3f9b412cf665b7247eacd83be41cf7bf0 \
     --hash=sha256:dfd681c5dc216037e0b0a2c821f5ed99ba9f03ebcf119c7dac0e9a7b960b9ec9 \
     --hash=sha256:e474390e60ed609cec869b0da796ad94f420bb057d86784191eefc62b65819ae \
     --hash=sha256:f76d097d12c82a535fda9dfe5e8dd4127952b45fea9b0276cb30cca5ea313fbc
     # via -r requirements.in
-pandas-stubs==2.0.0.230412 \
-    --hash=sha256:016f567cb9947edd0067ea2665ab00b77fa47e73a65ce1a097de4f499b3485c0 \
-    --hash=sha256:311ab8b42ee574d9fea5061d1f63aeca297e472de6073ba84bf2a017c6cb1b6b
-    # via -r requirements.in
-pathspec==0.11.1 \
-    --hash=sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687 \
-    --hash=sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293
-    # via black
 pillow==9.5.0 \
     --hash=sha256:07999f5834bdc404c442146942a2ecadd1cb6292f5229f4ed3b31e0a108746b1 \
     --hash=sha256:0852ddb76d85f127c135b6dd1f0bb88dbb9ee990d2cd9aa9e28526c93e794fba \
     --hash=sha256:1781a624c229cb35a2ac31cc4a77e28cafc8900733a864870c49bfeedacd106a \
     --hash=sha256:1e7723bd90ef94eda669a3c2c19d549874dd5badaeefabefd26053304abe5799 \
     --hash=sha256:229e2c79c00e85989a34b5981a2b67aa079fd08c903f0aaead522a1d68d79e51 \
     --hash=sha256:22baf0c3cf0c7f26e82d6e1adf118027afb325e703922c8dfc1d5d0156bb2eeb \
@@ -523,210 +794,114 @@
     --hash=sha256:e49eb4e95ff6fd7c0c402508894b1ef0e01b99a44320ba7d8ecbabefddcc5569 \
     --hash=sha256:f8286396b351785801a976b1e85ea88e937712ee2c3ac653710a4a57a8da5d9c \
     --hash=sha256:f8fc330c3370a81bbf3f88557097d1ea26cd8b019d6433aa59f71195f5ddebbf \
     --hash=sha256:fbd359831c1657d69bb81f0db962905ee05e5e9451913b18b831febfe0519082 \
     --hash=sha256:fe7e1c262d3392afcf5071df9afa574544f28eac825284596ac6db56e6d11062 \
     --hash=sha256:fed1e1cf6a42577953abbe8e6cf2fe2f566daebde7c34724ec8803c4c0cda579
     # via rich-pixels
-pip-tools==6.13.0 \
-    --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
-    --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
+portalocker==2.7.0 \
+    --hash=sha256:032e81d534a88ec1736d03f780ba073f047a06c478b06e2937486f334e955c51 \
+    --hash=sha256:a07c5b4f3985c3cf4798369631fb7011adb498e2a46d8440efc75a8f29a0f983
+    # via msal-extensions
+protobuf==4.22.3 \
+    --hash=sha256:13233ee2b9d3bd9a5f216c1fa2c321cd564b93d8f2e4f521a85b585447747997 \
+    --hash=sha256:23452f2fdea754a8251d0fc88c0317735ae47217e0d27bf330a30eec2848811a \
+    --hash=sha256:52f0a78141078077cfe15fe333ac3e3a077420b9a3f5d1bf9b5fe9d286b4d881 \
+    --hash=sha256:70659847ee57a5262a65954538088a1d72dfc3e9882695cab9f0c54ffe71663b \
+    --hash=sha256:7760730063329d42a9d4c4573b804289b738d4931e363ffbe684716b796bde51 \
+    --hash=sha256:7cf56e31907c532e460bb62010a513408e6cdf5b03fb2611e4b67ed398ad046d \
+    --hash=sha256:8b54f56d13ae4a3ec140076c9d937221f887c8f64954673d46f63751209e839a \
+    --hash=sha256:d14fc1a41d1a1909998e8aff7e80d2a7ae14772c4a70e4bf7db8a36690b54425 \
+    --hash=sha256:d4b66266965598ff4c291416be429cef7989d8fae88b55b62095a2331511b3fa \
+    --hash=sha256:e0e630d8e6a79f48c557cd1835865b593d0547dce221c66ed1b827de59c66c97 \
+    --hash=sha256:ecae944c6c2ce50dda6bf76ef5496196aeb1b85acb95df5843cd812615ec4b61 \
+    --hash=sha256:f08aa300b67f1c012100d8eb62d47129e53d1150f4469fd78a29fa3cb68c66f2 \
+    --hash=sha256:f2f4710543abec186aee332d6852ef5ae7ce2e9e807a3da570f36de5a732d88e
+    # via
+    #   google-api-core
+    #   googleapis-common-protos
+pyarrow==10.0.1 \
+    --hash=sha256:0ec7587d759153f452d5263dbc8b1af318c4609b607be2bd5127dcda6708cdb1 \
+    --hash=sha256:1765a18205eb1e02ccdedb66049b0ec148c2a0cb52ed1fb3aac322dfc086a6ee \
+    --hash=sha256:1a14f57a5f472ce8234f2964cd5184cccaa8df7e04568c64edc33b23eb285dd5 \
+    --hash=sha256:254017ca43c45c5098b7f2a00e995e1f8346b0fb0be225f042838323bb55283c \
+    --hash=sha256:42ba7c5347ce665338f2bc64685d74855900200dac81a972d49fe127e8132f75 \
+    --hash=sha256:443eb9409b0cf78df10ced326490e1a300205a458fbeb0767b6b31ab3ebae6b2 \
+    --hash=sha256:61f4c37d82fe00d855d0ab522c685262bdeafd3fbcb5fe596fe15025fbc7341b \
+    --hash=sha256:668e00e3b19f183394388a687d29c443eb000fb3fe25599c9b4762a0afd37775 \
+    --hash=sha256:6f7a7dbe2f7f65ac1d0bd3163f756deb478a9e9afc2269557ed75b1b25ab3610 \
+    --hash=sha256:70acca1ece4322705652f48db65145b5028f2c01c7e426c5d16a30ba5d739c24 \
+    --hash=sha256:7b4ede715c004b6fc535de63ef79fa29740b4080639a5ff1ea9ca84e9282f349 \
+    --hash=sha256:94fb4a0c12a2ac1ed8e7e2aa52aade833772cf2d3de9dde685401b22cec30002 \
+    --hash=sha256:abb57334f2c57979a49b7be2792c31c23430ca02d24becd0b511cbe7b6b08649 \
+    --hash=sha256:b069602eb1fc09f1adec0a7bdd7897f4d25575611dfa43543c8b8a75d99d6874 \
+    --hash=sha256:b1fc226d28c7783b52a84d03a66573d5a22e63f8a24b841d5fc68caeed6784d4 \
+    --hash=sha256:ba71e6fc348c92477586424566110d332f60d9a35cb85278f42e3473bc1373da \
+    --hash=sha256:bf26f809926a9d74e02d76593026f0aaeac48a65b64f1bb17eed9964bfe7ae1a \
+    --hash=sha256:cb627673cb98708ef00864e2e243f51ba7b4c1b9f07a1d821f98043eccd3f585 \
+    --hash=sha256:d1bc6e4d5d6f69e0861d5d7f6cf4d061cf1069cb9d490040129877acf16d4c2a \
+    --hash=sha256:db0c5986bf0808927f49640582d2032a07aa49828f14e51f362075f03747d198 \
+    --hash=sha256:e00174764a8b4e9d8d5909b6d19ee0c217a6cf0232c5682e31fdfbd5a9f0ae52 \
+    --hash=sha256:e141a65705ac98fa52a9113fe574fdaf87fe0316cde2dffe6b94841d3c61544c \
+    --hash=sha256:e3fe5049d2e9ca661d8e43fab6ad5a4c571af12d20a57dffc392a014caebef65 \
+    --hash=sha256:efa59933b20183c1c13efc34bd91efc6b2997377c4c6ad9272da92d224e3beb1 \
+    --hash=sha256:f2d00aa481becf57098e85d99e34a25dba5a9ade2f44eb0b7d80c80f2984fc03
     # via -r requirements.in
-platformdirs==3.5.0 \
-    --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
-    --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
-    # via black
-pluggy==1.0.0 \
-    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
-    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
-    # via pytest
+pyasn1==0.5.0 \
+    --hash=sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57 \
+    --hash=sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde
+    # via
+    #   pyasn1-modules
+    #   rsa
+pyasn1-modules==0.3.0 \
+    --hash=sha256:5bd01446b736eb9d31512a30d46c1ac3395d676c6f3cafa4c03eb54b9925631c \
+    --hash=sha256:d3ccd6ed470d9ffbc716be08bd90efbd44d0734bc9303818f7336070984a162d
+    # via google-auth
+pycparser==2.21 \
+    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
+    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
+    # via cffi
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
+    # via rich
+pyjwt[crypto]==2.6.0 \
+    --hash=sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd \
+    --hash=sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14
     # via
-    #   mkdocs-material
-    #   rich
-pymdown-extensions==9.11 \
-    --hash=sha256:a499191d8d869f30339de86fcf072a787e86c42b6f16f280f5c2cf174182b7f3 \
-    --hash=sha256:f7e86c1d3981f23d9dc43294488ecb54abadd05b0be4bf8f0e15efc90f7853ff
-    # via
-    #   mkdocs-material
-    #   mkdocstrings
-pyproject-hooks==1.0.0 \
-    --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
-    --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
-    # via build
-pytest==7.3.1 \
-    --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
-    --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
-    # via
-    #   -r requirements.in
-    #   pytest-cov
-    #   pytest-mock
-pytest-cov==4.0.0 \
-    --hash=sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b \
-    --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
-    # via -r requirements.in
-pytest-mock==3.10.0 \
-    --hash=sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b \
-    --hash=sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f
-    # via -r requirements.in
+    #   adal
+    #   msal
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via
-    #   ghp-import
+    #   adal
+    #   botocore
     #   pandas
 pytz==2023.3 \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
     # via pandas
-pyyaml==6.0 \
-    --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
-    --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
-    --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
-    --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
-    --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
-    --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
-    --hash=sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07 \
-    --hash=sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba \
-    --hash=sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9 \
-    --hash=sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287 \
-    --hash=sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513 \
-    --hash=sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0 \
-    --hash=sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1 \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7 \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358 \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
-    # via
-    #   mkdocs
-    #   pymdown-extensions
-    #   pyyaml-env-tag
-pyyaml-env-tag==0.1 \
-    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
-    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
-    # via mkdocs
-regex==2023.5.4 \
-    --hash=sha256:00f6f26e748c797a041ab6957f4cacc66a7fbd5dc5f627760985f5c5b7de2af6 \
-    --hash=sha256:0130a2fdd6f033c3e3710d0b950cc6abd3133c5af88c40c78e77641cb6f6cf8a \
-    --hash=sha256:027d4962340dbd84979fd1c40bfd7ca8362030abfbbff25f1327bbf4867f047c \
-    --hash=sha256:037f4be6a240a11a6d3397e932ef5d3ec5855858910792a0ab7d351bd0333533 \
-    --hash=sha256:04a825fd9f5931263eccd0cbdbf171a9792fa1bf2642ca62800b57689ca1b660 \
-    --hash=sha256:06fe9870165d4975a8a3e27a83919b9014b35dd2ee7061a5f2be8e579294cedc \
-    --hash=sha256:0a664857dd9b1076942c4d73c54a031066ee0ae88a438e7a1e0e79c1c5ddf47a \
-    --hash=sha256:0c731522eaf74166066fcf91fe7fe3c3617cc5e8df0c150132282d0dd5225afc \
-    --hash=sha256:0d5a0edefdf800aeef6cf559af75e614fb2eb2d0388f0b132af805fdefcf8ec6 \
-    --hash=sha256:0eee66c4ce6ced2e9d5d4497a569bab6257a6d118eb43dd57cceb61ba00b62d8 \
-    --hash=sha256:12be293d718e05f7304f715980b1a25b16e34a1ff2121740592559d066f91e67 \
-    --hash=sha256:1ad00c9aae6090d052c0ee16a2737a7154031793e6c7b58a629eed8d8aa77e31 \
-    --hash=sha256:1d98e4748a60c9902ad504e862756c43cc707404fc3025f82ef5bbe50bee3b9e \
-    --hash=sha256:1dc5e9a847613679ac8bd0386a0e54f2958441a0fcc123778637e433041aa763 \
-    --hash=sha256:1ef51012493837263236781ac9598f059dc4e5a4d72627bd3ac85cbd5d1b0ee1 \
-    --hash=sha256:2095acff95df0bf6ec3dee672a03d3d78606b4ca419d53fbd606c559cebedf45 \
-    --hash=sha256:21b653c1538cbbc1c58f6d6f3ccb4a5ce56491f0ab370ec057c1c64a152eb48c \
-    --hash=sha256:24db1c0fc20850db47977824a99fdae81d6764adaf8192dd874185d9e7166dbb \
-    --hash=sha256:2762750332f57820c0f38ade87ce4ebe671b178892faed0112f574f0b42801cf \
-    --hash=sha256:336fb3f585e239362d4f26dd6f904b15d91febfc980f47ed706858f5cee20ce6 \
-    --hash=sha256:3633a07ffeabc14f3cd531f11794bb603267d86e4109cb811a34aee020622d3f \
-    --hash=sha256:376fa2ef6a02a004b6fe4ebaa5ba370e7532ec6915efd12e33aa434517f8bbee \
-    --hash=sha256:3965a9ab13f1bf3e4af021c7dbe9678dd9f8dc5cc9097b3d3cbbf3ad00574b5d \
-    --hash=sha256:3d8cc797f87c07372e7d300198e1423c2b7bd35b68f375cc6700e26158940c9a \
-    --hash=sha256:460672c6ec94997755bd37b00302853b9d85a5a433121c198359958e8c10ced5 \
-    --hash=sha256:49a77f0b62a4122cf578d1194658973c435e6d2a9611013be11b6750056a5930 \
-    --hash=sha256:4c2ae89c92a04b057b412f88a3359e77600ce966a740e2da212667ce795e1bdc \
-    --hash=sha256:50e00ab84396bfbeb1bede61eff6641f957b6532e74e02be480d71914e20e2ac \
-    --hash=sha256:5a7ab3440f0c653dee8b42af858da6e07615c64ba86a6b3509a0ecf44eabdb11 \
-    --hash=sha256:5a98814d42282153c30d674ee34ea114a03ea8d32fd5d9b924d46fbeb2c7eb15 \
-    --hash=sha256:5cc67b3562aada6682ae45f2ea40819baa6bffe38155883100f8779c22c8c087 \
-    --hash=sha256:5d321dd059fd00482537aaba919e29189ea4ab6a03528881267982bb7707f610 \
-    --hash=sha256:5f82d4e0725788787216c9ae53116e6e477b2d97f29ec1e5086f5afbab5716b0 \
-    --hash=sha256:5fda1fc36dd923aee070d7aab3a85b448c8b62930900c615bb67db829281103b \
-    --hash=sha256:63a92f28a3f285dae06aae83227cb66cc87256db040aaf26c1c48ae5221eccde \
-    --hash=sha256:6469c2baf450fd1e648752b113a1fc1d67dfbad359f6171be954bacf7b09d126 \
-    --hash=sha256:6686256d1d435ed782ff12ef11e074705911a40d3907b986e53ca9a996e88489 \
-    --hash=sha256:6ccd0d7557c4e76303a6429ec9de55cd87334809cda66c0f101831e2ce9073c1 \
-    --hash=sha256:6f02105d4a511f550dcd63f750937d1607a1f6dc253c798c4adf36aba89215a3 \
-    --hash=sha256:70bd0c121b3c4e641e5c4e633c4581059acad774a1a62bcb15fea3470c2a61cc \
-    --hash=sha256:770f825c7751ce43aae2088fee94f2e60f95e181223642a0bb35cbaeea92001c \
-    --hash=sha256:77b3333a6cd1161b81bcf018a9bdb3cc567074a913aa69b98b9c8c79be28565c \
-    --hash=sha256:797bab57e1317c940030f3c15d48c01e1f16d12ba0f6a807ee0bebdc1cfe3f2d \
-    --hash=sha256:8418b0ee315555ca9786daab00ec8aaf47dfb2698a5be689676e83e88b949f22 \
-    --hash=sha256:861ed1249302664f96b2e968216486a02af0a143e0f3cc6fd92b78f11aa18579 \
-    --hash=sha256:89f54d4bbd452a5ee01dc31ec918f7b1f32483f13d3598af1acf5ea82ad82ad3 \
-    --hash=sha256:8c704e7062c59d2f7e2eebda2c0c0b69bd807ca6579c3a21fc4b1d8505cfc090 \
-    --hash=sha256:8d5bc5035989852a4ae7dacf8dc99db7c4f21c852486777a98b8efe37af4d8d7 \
-    --hash=sha256:91f47522688955cb33190f8354ccaa1cc058d05e73f99afe9ace40db36c159e8 \
-    --hash=sha256:9322797fddd51ec0312a8b649d9a3ebfabf4826a204ef8e1cc11801013005323 \
-    --hash=sha256:953ba37dd83c424c2cf699c64a8477645fc7c7403ffd2eb1417189eddbbfb4a7 \
-    --hash=sha256:97fd2885df308edcdf96baa632192a4291f3ed5b072c0bc3f29dc1e6de40ffa4 \
-    --hash=sha256:99780a0880d3dab2bb6f863492d38ab90ffdc9daf4fbefb505524f6f3a1c9dbe \
-    --hash=sha256:9b887d87188489859411d0c7e741f7dfe8a3ca5946b0db8b3c9e5daecc089b62 \
-    --hash=sha256:9e1b4b0b4baff934ef3c0ac56578a6b773f7f90ad1db3ff843ee40d83bdae09f \
-    --hash=sha256:a419384c6c80d58532016c3cf6a3aca009bfb7661f33e119ba7f77ec0e28222a \
-    --hash=sha256:aa92f9ad481108a7e4c5a5234608f7c718f8b67003ce4719a4d2735d82b54167 \
-    --hash=sha256:ac402ac165f42f41b3aef9e8a9c6fb204dac31faad65b3b0ae6bff4bc9d0dad2 \
-    --hash=sha256:ad84e1d4be3504e7dcd6370b3e847eaf05d5d35cb0818d0bd2d1a26b58c0abd2 \
-    --hash=sha256:b132e4507c6404faece005329de7b2b97653ddfeeaf84f058fe820791160dcda \
-    --hash=sha256:b365b8fa0d5fd0208db5b0e94582edb796dde07d1f99c5a9c1ff6be172c374ee \
-    --hash=sha256:b48820071a49b68ca8734e8b2bd1f26632512154816b261b614e62cc724d9f8a \
-    --hash=sha256:b7eb07d60c385aec906b82d48447907a2bbf454d0e9ead62168de111accabaf8 \
-    --hash=sha256:b87d38717ed855583ae1693f6095fc9c06b7dde4ddec782b41aa92931dd60e7c \
-    --hash=sha256:bda905e040e6c2875a7dde9652a9e0c426aaac6058568cc064f8128b061439ee \
-    --hash=sha256:c10b1388106447db0cdb8e340d06fa2d49b822368a049c36928d3c24296c2e37 \
-    --hash=sha256:c1155571edd498b6274f969517db6781500fbb24fc91ff740ea5a37c4735b3ba \
-    --hash=sha256:c1fa9651141caaafa0d6048695a4a04bc4bf39c75f250a36b1a05c9588a403a9 \
-    --hash=sha256:c300461ed8159f61d979971ba51f1acd1e6f9907d86888e9275165e06ea90f06 \
-    --hash=sha256:c40f7e8c02b287550166a3e36dbb89f9387db86a71101f6242668e3ef979cd2a \
-    --hash=sha256:c455d886838dd5a248e7f06e5573275fc854febd206eb937cf632082a06a939f \
-    --hash=sha256:cb22580ce5e2eee138a78df40444151ff51c91acd11be546216a046677c75593 \
-    --hash=sha256:ccd0c918971f79bd9a883f13f91343dd2eaefbafd4344aadfe5134a65fb821c3 \
-    --hash=sha256:d0ac14c36d91b191d1cb073fb5ac49937d88a5c8b051ced3875321a525202c34 \
-    --hash=sha256:d28933aa1242814ed737b569b2baf96e4d236c52be454b5dc17afd36bf893c12 \
-    --hash=sha256:db5d5c9c7bbcf9cbc541f8adba8c92a7a7abd0de4f0343da4e96fb78ffe9d1a1 \
-    --hash=sha256:dbc47670e0424a566084e15af9a253b85f90fa26e60fa07e1b10c90df4c8fd07 \
-    --hash=sha256:dbcb49036a6a6065035ac2acc1ad6a918f9e09ef2d0f9392dc90b8756f789f95 \
-    --hash=sha256:e708e69c4d3bc41df29efb94aadc5578c841b2cd02f8cbb1bcfbf280f2801238 \
-    --hash=sha256:e87450db3c444f41e3ac6a09b7a10ddfe54fa1e98bf60ee299fe6d11097540cd \
-    --hash=sha256:ea2d66c1fd898d81b8ce0f95afab9ba0ab522cf08810f11fa28ad958706cd2b2 \
-    --hash=sha256:eaff21326bc5d9be0c2f400931d39274105bd5d06650f0b0215392d1b050d404 \
-    --hash=sha256:ebf0776fdc7a5e0ac11b6db2d69ac77479411b627a96119ffa4427ba32f3bb66 \
-    --hash=sha256:f2bc7249840faacfff6196e5b5ffeb3fdaf078986521a1cda34e9be5607e773b \
-    --hash=sha256:f3e20cf2575b1330687d3dd6242f82278b3bdc09a9f36cc7ac4d45b7dd63c1f5 \
-    --hash=sha256:f576b8dec95456ba0157943a57f5f88c076cf96cc363ef1bf5027c2976fd487a \
-    --hash=sha256:fbc5b23b569d96b8c831574c93098b68c6d7ff2509f31268c968152ca4f2ecd0 \
-    --hash=sha256:ff8fef88029d0420315935041db517855ea022889fa8d54959943e39fffebf59
-    # via mkdocs-material
-requests==2.29.0 \
-    --hash=sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b \
-    --hash=sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059
-    # via mkdocs-material
+requests==2.28.2 \
+    --hash=sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa \
+    --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
+    # via
+    #   -r requirements.in
+    #   adal
+    #   azure-core
+    #   azure-datalake-store
+    #   gcsfs
+    #   google-api-core
+    #   google-cloud-storage
+    #   msal
+    #   requests-oauthlib
+requests-oauthlib==1.3.1 \
+    --hash=sha256:2577c501a2fb8d05a304c09d090d6e47c306fef15809d102b327cf8364bddab5 \
+    --hash=sha256:75beac4a47881eeb94d5ea5d6ad31ef88856affe2332b9aafb52c6452ccf0d7a
+    # via google-auth-oauthlib
 rich==13.3.5 \
     --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
     --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
     # via
     #   -r requirements.in
     #   rich-click
     #   rich-pixels
@@ -735,110 +910,207 @@
     --hash=sha256:131a94bed597eab9f1eda7eb41fb7275b6b60ae9e6defc3769277b70b104285d \
     --hash=sha256:a57ca70242cb8b372a670eaa0b0be48f2440b66656deb4a56e6aadc1bbb79670
     # via -r requirements.in
 rich-pixels==2.1.1 \
     --hash=sha256:170e6d3ef84825967f451f40f7c7deee324af630141c701cf054575f2fd34abb \
     --hash=sha256:24eccb904fcb6d2cf0727d7767ec81d3faaee8c64631a8bc6cf6d95bed2c34d6
     # via -r requirements.in
-ruff==0.0.264 \
-    --hash=sha256:04ec5d75e4bca754cedd20d53e2ba4920d6259e7579abfb2e8e30c3c80e41b17 \
-    --hash=sha256:05ee163a046fc593d150179d23f4af447fb82f3e59cd34e031ea0868c65bb8e8 \
-    --hash=sha256:068a82a29d80848a56e3d9d4308e6e0ca8b2ecdaf5ac342a292545a59b7f2c21 \
-    --hash=sha256:18a29ed37bf8cfe6dce8a2db56c313a64c0804095108753621f3c3321e0c9c5f \
-    --hash=sha256:323ae6c1702b26c96d0fbf939c5959c37e79021f86b70f63634df918bc77f36e \
-    --hash=sha256:3e2c38449548e122f2612843a7c04e22b4fd491656955c57b8cb05df11639ad6 \
-    --hash=sha256:4564e0f245eb515c6ed63988c21e9c40bcfd485cd1ec63bdd790f9a81d301f15 \
-    --hash=sha256:484e395d1984ab9e1e66bd42e7a5192decfee86998d07d36ee50b2fadccc8734 \
-    --hash=sha256:5a8658ebcc37d62f72840cbdf564171c1a2b6831db482b4d917962541a2f4a44 \
-    --hash=sha256:67326fdc9ac0a1b13e229c6e24e8d115863c52cd710faaaaa588851535281d6c \
-    --hash=sha256:71fd865ebacc1083259b3fb7e3eb45235a86e62e21830b8a6b067be0ec54aa2e \
-    --hash=sha256:8fcd4b693ca1374eb7a5796581c90689f884f98f388740d94f0702fd30f8f78f \
-    --hash=sha256:91c6eb4f979b661a2dd850d9ac803842bb7b66d4926de84f09c787af82590f73 \
-    --hash=sha256:cd4f60ffc3eb15802c554a9c8581bf2117c4d3d06fbc57e0ba58f04cb1aaa47f \
-    --hash=sha256:d628de91e2be7a83128526636097d2dd890669a06143f826f6c591d79aeefbc4 \
-    --hash=sha256:d97ba8db0fb601ffe9ee996ebb97c698e427a2fd4514fefbe7b803111354f783 \
-    --hash=sha256:ec2fa192c035b8b68cc2b91049c561cd69543e2b8c4d157d9aa7727320bedcca
+rsa==4.9 \
+    --hash=sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7 \
+    --hash=sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21
+    # via google-auth
+s3fs==2023.1.0 \
+    --hash=sha256:8b2e28372423e93f26312208a9272e22a962ddd0a79d63f9a68693b6af5ff187 \
+    --hash=sha256:a549ae518fff4388bd6fca5248575c29f521e7e39efcd2bfab476651701fd114
     # via -r requirements.in
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-    # via python-dateutil
+    # via
+    #   azure-core
+    #   azure-identity
+    #   google-auth
+    #   isodate
+    #   python-dateutil
 textual==0.22.3 \
     --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
     --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
     # via -r requirements.in
-tomli==2.0.1 \
-    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
-    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-    # via
-    #   black
-    #   build
-    #   coverage
-    #   mypy
-    #   pyproject-hooks
-    #   pytest
-types-pytz==2023.3.0.0 \
-    --hash=sha256:4fc2a7fbbc315f0b6630e0b899fd6c743705abe1094d007b0e612d10da15e0f3 \
-    --hash=sha256:ecdc70d543aaf3616a7e48631543a884f74205f284cefd6649ddf44c6a820aac
-    # via pandas-stubs
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
-    #   black
-    #   mkdocstrings
-    #   mypy
+    #   aioitertools
+    #   azure-core
+    #   azure-storage-blob
     #   textual
 uc-micro-py==1.0.2 \
     --hash=sha256:30ae2ac9c49f39ac6dce743bd187fcd2b574b16ca095fa74cd9396795c954c54 \
     --hash=sha256:8c9110c309db9d9e87302e2f4ad2c3152770930d88ab385cd544e7a7e75f3de0
     # via linkify-it-py
 universal-pathlib==0.0.23 \
     --hash=sha256:76cbc91d66ddb2c0c0c939d147bcd8fa2c79882b5451d2a59009811fc4f80bd3 \
     --hash=sha256:bd7ed0ad5c6a31b3bf0835b9e7526ed0974ec3a49e4a6a02b1f4058ce63ec79c
     # via -r requirements.in
 urllib3==1.26.15 \
     --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
     --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
-    # via requests
-watchdog==3.0.0 \
-    --hash=sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a \
-    --hash=sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100 \
-    --hash=sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8 \
-    --hash=sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc \
-    --hash=sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae \
-    --hash=sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41 \
-    --hash=sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0 \
-    --hash=sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f \
-    --hash=sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c \
-    --hash=sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9 \
-    --hash=sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3 \
-    --hash=sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709 \
-    --hash=sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83 \
-    --hash=sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759 \
-    --hash=sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9 \
-    --hash=sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3 \
-    --hash=sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7 \
-    --hash=sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f \
-    --hash=sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346 \
-    --hash=sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674 \
-    --hash=sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397 \
-    --hash=sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96 \
-    --hash=sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d \
-    --hash=sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a \
-    --hash=sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64 \
-    --hash=sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44 \
-    --hash=sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33
-    # via mkdocs
-wheel==0.40.0 \
-    --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
-    --hash=sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247
-    # via pip-tools
+    # via
+    #   botocore
+    #   requests
+wrapt==1.15.0 \
+    --hash=sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0 \
+    --hash=sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420 \
+    --hash=sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a \
+    --hash=sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c \
+    --hash=sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079 \
+    --hash=sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923 \
+    --hash=sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f \
+    --hash=sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1 \
+    --hash=sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8 \
+    --hash=sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86 \
+    --hash=sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0 \
+    --hash=sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364 \
+    --hash=sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e \
+    --hash=sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c \
+    --hash=sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e \
+    --hash=sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c \
+    --hash=sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727 \
+    --hash=sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff \
+    --hash=sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e \
+    --hash=sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29 \
+    --hash=sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7 \
+    --hash=sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72 \
+    --hash=sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475 \
+    --hash=sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a \
+    --hash=sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317 \
+    --hash=sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2 \
+    --hash=sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd \
+    --hash=sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640 \
+    --hash=sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98 \
+    --hash=sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248 \
+    --hash=sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e \
+    --hash=sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d \
+    --hash=sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec \
+    --hash=sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1 \
+    --hash=sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e \
+    --hash=sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9 \
+    --hash=sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92 \
+    --hash=sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb \
+    --hash=sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094 \
+    --hash=sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46 \
+    --hash=sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29 \
+    --hash=sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd \
+    --hash=sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705 \
+    --hash=sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8 \
+    --hash=sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975 \
+    --hash=sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb \
+    --hash=sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e \
+    --hash=sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b \
+    --hash=sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418 \
+    --hash=sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019 \
+    --hash=sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1 \
+    --hash=sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba \
+    --hash=sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6 \
+    --hash=sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2 \
+    --hash=sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3 \
+    --hash=sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7 \
+    --hash=sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752 \
+    --hash=sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416 \
+    --hash=sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f \
+    --hash=sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1 \
+    --hash=sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc \
+    --hash=sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145 \
+    --hash=sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee \
+    --hash=sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a \
+    --hash=sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7 \
+    --hash=sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b \
+    --hash=sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653 \
+    --hash=sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0 \
+    --hash=sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90 \
+    --hash=sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29 \
+    --hash=sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6 \
+    --hash=sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034 \
+    --hash=sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09 \
+    --hash=sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559 \
+    --hash=sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639
+    # via aiobotocore
+yarl==1.9.2 \
+    --hash=sha256:04ab9d4b9f587c06d801c2abfe9317b77cdf996c65a90d5e84ecc45010823571 \
+    --hash=sha256:066c163aec9d3d073dc9ffe5dd3ad05069bcb03fcaab8d221290ba99f9f69ee3 \
+    --hash=sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3 \
+    --hash=sha256:149ddea5abf329752ea5051b61bd6c1d979e13fbf122d3a1f9f0c8be6cb6f63c \
+    --hash=sha256:159d81f22d7a43e6eabc36d7194cb53f2f15f498dbbfa8edc8a3239350f59fe7 \
+    --hash=sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04 \
+    --hash=sha256:22a94666751778629f1ec4280b08eb11815783c63f52092a5953faf73be24191 \
+    --hash=sha256:2a96c19c52ff442a808c105901d0bdfd2e28575b3d5f82e2f5fd67e20dc5f4ea \
+    --hash=sha256:2b0738fb871812722a0ac2154be1f049c6223b9f6f22eec352996b69775b36d4 \
+    --hash=sha256:2c315df3293cd521033533d242d15eab26583360b58f7ee5d9565f15fee1bef4 \
+    --hash=sha256:32f1d071b3f362c80f1a7d322bfd7b2d11e33d2adf395cc1dd4df36c9c243095 \
+    --hash=sha256:3458a24e4ea3fd8930e934c129b676c27452e4ebda80fbe47b56d8c6c7a63a9e \
+    --hash=sha256:38a3928ae37558bc1b559f67410df446d1fbfa87318b124bf5032c31e3447b74 \
+    --hash=sha256:3da8a678ca8b96c8606bbb8bfacd99a12ad5dd288bc6f7979baddd62f71c63ef \
+    --hash=sha256:494053246b119b041960ddcd20fd76224149cfea8ed8777b687358727911dd33 \
+    --hash=sha256:50f33040f3836e912ed16d212f6cc1efb3231a8a60526a407aeb66c1c1956dde \
+    --hash=sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45 \
+    --hash=sha256:53338749febd28935d55b41bf0bcc79d634881195a39f6b2f767870b72514caf \
+    --hash=sha256:5415d5a4b080dc9612b1b63cba008db84e908b95848369aa1da3686ae27b6d2b \
+    --hash=sha256:5610f80cf43b6202e2c33ba3ec2ee0a2884f8f423c8f4f62906731d876ef4fac \
+    --hash=sha256:566185e8ebc0898b11f8026447eacd02e46226716229cea8db37496c8cdd26e0 \
+    --hash=sha256:56ff08ab5df8429901ebdc5d15941b59f6253393cb5da07b4170beefcf1b2528 \
+    --hash=sha256:59723a029760079b7d991a401386390c4be5bfec1e7dd83e25a6a0881859e716 \
+    --hash=sha256:5fcd436ea16fee7d4207c045b1e340020e58a2597301cfbcfdbe5abd2356c2fb \
+    --hash=sha256:61016e7d582bc46a5378ffdd02cd0314fb8ba52f40f9cf4d9a5e7dbef88dee18 \
+    --hash=sha256:63c48f6cef34e6319a74c727376e95626f84ea091f92c0250a98e53e62c77c72 \
+    --hash=sha256:646d663eb2232d7909e6601f1a9107e66f9791f290a1b3dc7057818fe44fc2b6 \
+    --hash=sha256:662e6016409828ee910f5d9602a2729a8a57d74b163c89a837de3fea050c7582 \
+    --hash=sha256:674ca19cbee4a82c9f54e0d1eee28116e63bc6fd1e96c43031d11cbab8b2afd5 \
+    --hash=sha256:6a5883464143ab3ae9ba68daae8e7c5c95b969462bbe42e2464d60e7e2698368 \
+    --hash=sha256:6e7221580dc1db478464cfeef9b03b95c5852cc22894e418562997df0d074ccc \
+    --hash=sha256:75df5ef94c3fdc393c6b19d80e6ef1ecc9ae2f4263c09cacb178d871c02a5ba9 \
+    --hash=sha256:783185c75c12a017cc345015ea359cc801c3b29a2966c2655cd12b233bf5a2be \
+    --hash=sha256:822b30a0f22e588b32d3120f6d41e4ed021806418b4c9f0bc3048b8c8cb3f92a \
+    --hash=sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80 \
+    --hash=sha256:82aa6264b36c50acfb2424ad5ca537a2060ab6de158a5bd2a72a032cc75b9eb8 \
+    --hash=sha256:832b7e711027c114d79dffb92576acd1bd2decc467dec60e1cac96912602d0e6 \
+    --hash=sha256:838162460b3a08987546e881a2bfa573960bb559dfa739e7800ceeec92e64417 \
+    --hash=sha256:83fcc480d7549ccebe9415d96d9263e2d4226798c37ebd18c930fce43dfb9574 \
+    --hash=sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59 \
+    --hash=sha256:891c0e3ec5ec881541f6c5113d8df0315ce5440e244a716b95f2525b7b9f3608 \
+    --hash=sha256:8c2ad583743d16ddbdf6bb14b5cd76bf43b0d0006e918809d5d4ddf7bde8dd82 \
+    --hash=sha256:8c56986609b057b4839968ba901944af91b8e92f1725d1a2d77cbac6972b9ed1 \
+    --hash=sha256:8ea48e0a2f931064469bdabca50c2f578b565fc446f302a79ba6cc0ee7f384d3 \
+    --hash=sha256:8ec53a0ea2a80c5cd1ab397925f94bff59222aa3cf9c6da938ce05c9ec20428d \
+    --hash=sha256:95d2ecefbcf4e744ea952d073c6922e72ee650ffc79028eb1e320e732898d7e8 \
+    --hash=sha256:9b3152f2f5677b997ae6c804b73da05a39daa6a9e85a512e0e6823d81cdad7cc \
+    --hash=sha256:9bf345c3a4f5ba7f766430f97f9cc1320786f19584acc7086491f45524a551ac \
+    --hash=sha256:a60347f234c2212a9f0361955007fcf4033a75bf600a33c88a0a8e91af77c0e8 \
+    --hash=sha256:a74dcbfe780e62f4b5a062714576f16c2f3493a0394e555ab141bf0d746bb955 \
+    --hash=sha256:a83503934c6273806aed765035716216cc9ab4e0364f7f066227e1aaea90b8d0 \
+    --hash=sha256:ac9bb4c5ce3975aeac288cfcb5061ce60e0d14d92209e780c93954076c7c4367 \
+    --hash=sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb \
+    --hash=sha256:b03917871bf859a81ccb180c9a2e6c1e04d2f6a51d953e6a5cdd70c93d4e5a2a \
+    --hash=sha256:b124e2a6d223b65ba8768d5706d103280914d61f5cae3afbc50fc3dfcc016623 \
+    --hash=sha256:b25322201585c69abc7b0e89e72790469f7dad90d26754717f3310bfe30331c2 \
+    --hash=sha256:b7232f8dfbd225d57340e441d8caf8652a6acd06b389ea2d3222b8bc89cbfca6 \
+    --hash=sha256:b8cc1863402472f16c600e3e93d542b7e7542a540f95c30afd472e8e549fc3f7 \
+    --hash=sha256:b9a4e67ad7b646cd6f0938c7ebfd60e481b7410f574c560e455e938d2da8e0f4 \
+    --hash=sha256:be6b3fdec5c62f2a67cb3f8c6dbf56bbf3f61c0f046f84645cd1ca73532ea051 \
+    --hash=sha256:bf74d08542c3a9ea97bb8f343d4fcbd4d8f91bba5ec9d5d7f792dbe727f88938 \
+    --hash=sha256:c027a6e96ef77d401d8d5a5c8d6bc478e8042f1e448272e8d9752cb0aff8b5c8 \
+    --hash=sha256:c0c77533b5ed4bcc38e943178ccae29b9bcf48ffd1063f5821192f23a1bd27b9 \
+    --hash=sha256:c1012fa63eb6c032f3ce5d2171c267992ae0c00b9e164efe4d73db818465fac3 \
+    --hash=sha256:c3a53ba34a636a256d767c086ceb111358876e1fb6b50dfc4d3f4951d40133d5 \
+    --hash=sha256:d4e2c6d555e77b37288eaf45b8f60f0737c9efa3452c6c44626a5455aeb250b9 \
+    --hash=sha256:de119f56f3c5f0e2fb4dee508531a32b069a5f2c6e827b272d1e0ff5ac040333 \
+    --hash=sha256:e65610c5792870d45d7b68c677681376fcf9cc1c289f23e8e8b39c1485384185 \
+    --hash=sha256:e9fdc7ac0d42bc3ea78818557fab03af6181e076a2944f43c38684b4b6bed8e3 \
+    --hash=sha256:ee4afac41415d52d53a9833ebae7e32b344be72835bbb589018c9e938045a560 \
+    --hash=sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b \
+    --hash=sha256:f3b078dbe227f79be488ffcfc7a9edb3409d018e0952cf13f15fd6512847f3f7 \
+    --hash=sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78 \
+    --hash=sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7
+    # via aiohttp
 zipp==3.15.0 \
     --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
     --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
     # via importlib-metadata
-
-# WARNING: The following packages were not pinned, but pip requires them to be
-# pinned when the requirements file includes hashes. Consider using the --allow-unsafe flag.
-# pip
-# setuptools
```

### Comparing `browsr-1.1.0/.gitignore` & `browsr-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/LICENSE.txt` & `browsr-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/README.md` & `browsr-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.1.0/pyproject.toml` & `browsr-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -79,31 +79,32 @@
   "mkdocstrings[python]~=0.21.2",
   "black~=23.3.0",
   "ruff~=0.0.261",
   "mypy~=1.2.0",
   "pandas-stubs~=2.0.0.230412",
   "pip-tools~=6.13.0"
 ]
+features = ["all"]
 pre-install-commands = ["pip install -U --no-deps -r requirements/requirements-dev.txt"]
 
 [tool.hatch.envs.default.scripts]
 _pip_compile = "pip-compile --resolver=backtracking --generate-hashes requirements.in"
 all = ["format", "lint", "check", "test"]
 check = [
   "mypy --install-types --strict-optional --non-interactive {args:browsr/ tests/}"
 ]
 docs-build = ["mkdocs build --clean --strict"]
 docs-deploy = ["mkdocs gh-deploy {args:}"]
 docs-serve = ["mkdocs serve --dev-addr localhost:8000"]
 format = ["ruff --fix {args:.}", "black {args:.}"]
 lint = ["ruff {args:.}", "black --check {args:.}"]
 requirements = [
-  "hatch dep show requirements --project-only > requirements.in",
+  "hatch dep show requirements --project-only --all > requirements.in",
   "_pip_compile --output-file requirements/requirements-prod.txt",
-  "hatch dep show requirements > requirements.in",
+  "hatch dep show requirements --all > requirements.in",
   "_pip_compile --output-file requirements/requirements-dev.txt",
   "rm requirements.in"
 ]
 requirements-upgrade = [
   "hatch dep show requirements --project-only --all > requirements.in",
   "_pip_compile --output-file requirements/requirements-prod.txt --upgrade",
   "hatch dep show requirements --all > requirements.in",
```

### Comparing `browsr-1.1.0/PKG-INFO` & `browsr-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.1.0
+Version: 1.1.1
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.1.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.1.1 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

