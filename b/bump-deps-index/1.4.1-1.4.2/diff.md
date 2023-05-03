# Comparing `tmp/bump_deps_index-1.4.1.tar.gz` & `tmp/bump_deps_index-1.4.2.tar.gz`

## Comparing `bump_deps_index-1.4.1.tar` & `bump_deps_index-1.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tox.ini
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/whitelist.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/changelog.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/cli.rst
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/conf.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/index.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/py_api.rst
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/__main__.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_cli.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_run.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/version.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_cli.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_main.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_run.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_spec.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/LICENSE
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/README.md
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tox.ini
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/whitelist.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/workflows/check.yml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/changelog.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/cli.rst
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/conf.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/index.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/py_api.rst
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/__main__.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_cli.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_run.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/version.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_main.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_run.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_spec.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/LICENSE
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/README.md
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/PKG-INFO
```

### Comparing `bump_deps_index-1.4.1/.pre-commit-config.yaml` & `bump_deps_index-1.4.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     hooks:
       - id: rst-backticks
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: "0.11.1"
+    hooks:
+      - id: pyproject-fmt
+        additional_dependencies: [tox>=4.5.1]
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-bugbear==23.3.23
           - flake8-comprehensions==3.12
@@ -55,11 +60,7 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v2.7.1"
     hooks:
       - id: prettier
         additional_dependencies:
           - "prettier@2.7.1"
           - "@prettier/plugin-xml@2.2"
-  - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "0.11.1"
-    hooks:
-      - id: pyproject-fmt
```

### Comparing `bump_deps_index-1.4.1/tox.ini` & `bump_deps_index-1.4.2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
 
 [testenv:fix]
 description = run static analysis and style check using flake8
 skip_install = true
 deps =
-    pre-commit>=3.2.2
+    pre-commit>=3.3.1
 pass_env =
     HOMEPATH
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
```

### Comparing `bump_deps_index-1.4.1/.github/workflows/check.yml` & `bump_deps_index-1.4.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/.github/workflows/release.yml` & `bump_deps_index-1.4.2/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         run: python -m pip install build
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Build package
         run: pyproject-build -s -w . -o dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
```

### Comparing `bump_deps_index-1.4.1/docs/changelog.rst` & `bump_deps_index-1.4.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/docs/conf.py` & `bump_deps_index-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/src/bump_deps_index/_cli.py` & `bump_deps_index-1.4.2/src/bump_deps_index/_cli.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/src/bump_deps_index/_run.py` & `bump_deps_index-1.4.2/src/bump_deps_index/_run.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/src/bump_deps_index/_spec.py` & `bump_deps_index-1.4.2/src/bump_deps_index/_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import json
+from collections import deque
 from enum import Enum, auto
 from functools import cache
-from io import StringIO
+from html.parser import HTMLParser
 from threading import Lock
 from urllib.request import urlopen
-from xml.etree.ElementTree import parse
 
 from packaging.requirements import Requirement
 from packaging.version import Version
 
 
 class PkgType(Enum):
     PYTHON = auto()
@@ -85,44 +85,64 @@
         new_req = str(Requirement(new_ver))
     else:
         op = "==" if eq else ">="
         new_req = str(req).replace(f"{op}{c_ver}", f"{op}{ver}")
     return new_req
 
 
+class IndexParser(HTMLParser):
+    def __init__(self) -> None:
+        super().__init__()
+        self._at_tag: deque[str] = deque()
+        self._files: list[str] = []
+
+    @property
+    def files(self) -> frozenset[str]:
+        return frozenset(self._files)
+
+    def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]) -> None:  # noqa: U100
+        self._at_tag.append(tag)
+
+    def handle_endtag(self, tag: str) -> None:
+        if self._at_tag and self._at_tag[-1] == tag:  # pragma: no branch
+            self._at_tag.pop()
+
+    def handle_data(self, data: str) -> None:
+        if self._at_tag and self._at_tag[-1] == "a" and data.strip():
+            self._files.append(data.strip())
+
+
 def get_pkgs(index_url: str, package: str, pre_release: bool) -> list[Version]:
     with urlopen(f"{index_url}/{package}") as handler:
         text = handler.read().decode("utf-8")
 
-    root = parse(StringIO(text))
-
     versions: set[Version] = set()
-    for element in root.iter("a"):
-        if element.text:
-            file = element.text
-            if file.endswith(".tar.bz2"):
-                file = file[:-8]
-            if file.endswith(".tar.gz"):
-                file = file[:-7]
-            if file.endswith(".whl"):
-                file = file[:-4]
-            if file.endswith(".zip"):
-                file = file[:-4]
-            parts = file.split("-")
-            for part in parts[1:]:
-                if part.split(".")[0].isnumeric():
-                    break
-            else:
-                continue
-            try:
-                version = Version(part)
-            except ValueError:
-                pass
-            else:
-                versions.add(version)
+    parser = IndexParser()
+    parser.feed(text)
+    for file in parser.files:
+        if file.endswith(".tar.bz2"):
+            file = file[:-8]
+        if file.endswith(".tar.gz"):
+            file = file[:-7]
+        if file.endswith(".whl"):
+            file = file[:-4]
+        if file.endswith(".zip"):
+            file = file[:-4]
+        parts = file.split("-")
+        for part in parts[1:]:
+            if part.split(".")[0].isnumeric():
+                break
+        else:
+            continue
+        try:
+            version = Version(part)
+        except ValueError:
+            pass
+        else:
+            versions.add(version)
     return sorted((v for v in versions if (True if pre_release else not v.is_prerelease)), reverse=True)
 
 
 __all__ = [
     "update",
     "PkgType",
 ]
```

### Comparing `bump_deps_index-1.4.1/tests/test_cli.py` & `bump_deps_index-1.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/tests/test_main.py` & `bump_deps_index-1.4.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/tests/test_run.py` & `bump_deps_index-1.4.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/tests/test_spec.py` & `bump_deps_index-1.4.2/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/LICENSE` & `bump_deps_index-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/README.md` & `bump_deps_index-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/pyproject.toml` & `bump_deps_index-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.1/PKG-INFO` & `bump_deps_index-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-deps-index
-Version: 1.4.1
+Version: 1.4.2
 Summary: Bump your dependencies to latest available from index.
 Project-URL: Documentation, https://bump-deps-index.readthedocs.io
 Project-URL: Homepage, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Source, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Tracker, https://github.com/gaborbernat/bump-deps-index/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License: MIT License
```

