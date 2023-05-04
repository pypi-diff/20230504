# Comparing `tmp/darkmark-0.0.1.tar.gz` & `tmp/darkmark-0.1.0.tar.gz`

## Comparing `darkmark-0.0.1.tar` & `darkmark-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 darkmark-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/__main__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/console.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/darkmark.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/replacer.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/cli/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 darkmark-0.0.1/darkmark/cli/common.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 darkmark-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 darkmark-0.0.1/tests/test_me.py
--rw-r--r--   0        0        0    17320 2020-02-02 00:00:00.000000 darkmark-0.0.1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 darkmark-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 darkmark-0.0.1/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 darkmark-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 darkmark-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 darkmark-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 darkmark-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__about__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__main__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/console.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/darkmark.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/replacer.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/cli/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/cli/common.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 darkmark-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 darkmark-0.1.0/tests/test_me.py
+-rw-r--r--   0        0        0    17320 2020-02-02 00:00:00.000000 darkmark-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 darkmark-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 darkmark-0.1.0/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 darkmark-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 darkmark-0.1.0/PKG-INFO
```

### Comparing `darkmark-0.0.1/darkmark/darkmark.py` & `darkmark-0.1.0/darkmark/darkmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,11 +107,22 @@
             ][i]
             self.md = replacer.insert_text(self.md, capture[0].end_point[0] + 1, block)
 
     def write_text(self):
         self.md_file.write_text(self.md)
 
 
+# @register_line_magic
+# def darkmark(file):
+#     d = DarkMark(file)
+#     d.run_cells()
+#     return d
+
+
+# def load_ipython_extension(ipython):
+#     ipython.register_magic_function(darkmark, magic_kind="cell")
+
+
 if __name__ == "__main__":
     d = DarkMark("test.md")
     d.run_cells()
     print(d.md)
```

### Comparing `darkmark-0.0.1/darkmark/replacer.py` & `darkmark-0.1.0/darkmark/replacer.py`

 * *Files identical despite different names*

### Comparing `darkmark-0.0.1/darkmark/cli/__init__.py` & `darkmark-0.1.0/darkmark/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2023-present Waylon S. Walker <waylon@waylonwalker.com>
 #
 # SPDX-License-Identifier: MIT
 import hashlib
 from pathlib import Path
+import time
 
 from rich.console import Console
 import typer
 
 from darkmark.cli.common import verbose_callback
 from darkmark.console import console
 from darkmark.darkmark import DarkMark
@@ -22,14 +23,26 @@
 
 app = typer.Typer(
     name=name,
     help="run code blocks in markdown",
 )
 
 
+def get_hash(file, retries=5, sleep=1):
+    try:
+        new_hash = hashlib.md5(Path(file).read_text().encode()).hexdigest()
+    except FileNotFoundError:
+        if retries > 0:
+            time.sleep(sleep)
+            return get_hash(file, retries - 1, sleep)
+        raise typer.Exit(1)
+
+    return new_hash
+
+
 @app.callback(invoke_without_command=True)
 def main(
     file: Path = typer.Argument(...),
     version: bool = typer.Option(
         False,
         "--version",
         callback=version_callback,  # is_eager=True
@@ -44,20 +57,23 @@
         help="show the log messages",
     ),
     watch: bool = typer.Option(False, help="rerun when file changes"),
 ) -> None:
     if watch:
         old_hash = ""
         while True:
-            if old_hash != hashlib.md5(Path(file).read_text().encode()).hexdigest():
-                Console().log("running")
+            if get_hash(file) != old_hash:
+                console.log("running")
+                console.log(f"old_hash: {old_hash}")
+                console.log(f"new_hash: {get_hash(file)}")
                 d = DarkMark(file)
                 d.clear()
                 d.run_cells()
                 d.write_text()
+                time.sleep(1)
                 old_hash = hashlib.md5(Path(file).read_text().encode()).hexdigest()
 
     d = DarkMark(file)
     d.clear()
 
     if clear and dry_run:
         Console().print(d.md)
```

### Comparing `darkmark-0.0.1/.gitignore` & `darkmark-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `darkmark-0.0.1/LICENSE.txt` & `darkmark-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `darkmark-0.0.1/pyproject.toml` & `darkmark-0.1.0/pyproject.toml`

 * *Files identical despite different names*

