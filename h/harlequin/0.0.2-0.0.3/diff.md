# Comparing `tmp/harlequin-0.0.2.tar.gz` & `tmp/harlequin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.2.tar", max compression
+gzip compressed data, was "harlequin-0.0.3.tar", max compression
```

## Comparing `harlequin-0.0.2.tar` & `harlequin-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-05-02 20:18:52.433412 harlequin-0.0.2/LICENSE
--rw-r--r--   0        0        0      826 2023-05-02 20:18:52.433412 harlequin-0.0.2/README.md
--rw-r--r--   0        0        0      652 2023-05-02 20:18:52.433412 harlequin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/__init__.py
--rw-r--r--   0        0        0      388 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/cli.py
--rw-r--r--   0        0        0      204 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0      403 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/code_editor.py
--rw-r--r--   0        0        0       81 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/results_viewer.py
--rw-r--r--   0        0        0     1300 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/schema_viewer.py
--rw-r--r--   0        0        0      155 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/sql_client.css
--rw-r--r--   0        0        0     1399 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/sql_client.py
--rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 harlequin-0.0.2/setup.py
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 harlequin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 21:57:48.643889 harlequin-0.0.3/LICENSE
+-rw-r--r--   0        0        0      827 2023-05-04 21:57:48.643889 harlequin-0.0.3/README.md
+-rw-r--r--   0        0        0     1312 2023-05-04 21:57:48.643889 harlequin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/__init__.py
+-rw-r--r--   0        0        0      336 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/cli.py
+-rw-r--r--   0        0        0        0 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2254 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     5738 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      476 2023-05-04 21:57:48.643889 harlequin-0.0.3/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0     2083 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1034 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0      148 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3677 2023-05-04 21:57:48.647889 harlequin-0.0.3/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 harlequin-0.0.3/setup.py
+-rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 harlequin-0.0.3/PKG-INFO
```

### Comparing `harlequin-0.0.2/LICENSE` & `harlequin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.2/README.md` & `harlequin-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # harlequin
 A Text User Interface for DuckDB.
 
 (A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)
+
 ![harlequin](harlequin.jpg)
 
 ## Installing Harlequin
 
 Use `pip` or `pipx`:
 
 ```bash
```

### Comparing `harlequin-0.0.2/setup.py` & `harlequin-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['harlequin', 'harlequin.tui']
+['harlequin', 'harlequin.tui', 'harlequin.tui.components']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.1.3,<9.0.0', 'duckdb>=0.7.1,<0.8.0', 'textual>=0.22.3,<0.23.0']
+['click>=8.1.3,<9.0.0',
+ 'duckdb>=0.7.1,<0.8.0',
+ 'shandy-sqlfmt>=0.18.0,<0.19.0',
+ 'textual>=0.22.3,<0.23.0']
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'A Text User Interface for DuckDB',
-    'long_description': '# harlequin\nA Text User Interface for DuckDB.\n\n(A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n![harlequin](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main text input, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.',
+    'long_description': '# harlequin\nA Text User Interface for DuckDB.\n\n(A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main text input, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `harlequin-0.0.2/PKG-INFO` & `harlequin-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
+Requires-Dist: shandy-sqlfmt (>=0.18.0,<0.19.0)
 Requires-Dist: textual (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # harlequin
 A Text User Interface for DuckDB.
 
 (A Harlequin is a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)
+
 ![harlequin](harlequin.jpg)
 
 ## Installing Harlequin
 
 Use `pip` or `pipx`:
 
 ```bash
```

