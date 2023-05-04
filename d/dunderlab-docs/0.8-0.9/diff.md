# Comparing `tmp/dunderlab-docs-0.8.tar.gz` & `tmp/dunderlab-docs-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunderlab-docs-0.8.tar", last modified: Sat Mar  4 18:56:01 2023, max compression
+gzip compressed data, was "dunderlab-docs-0.9.tar", last modified: Sun Mar  5 03:08:34 2023, max compression
```

## Comparing `dunderlab-docs-0.8.tar` & `dunderlab-docs-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-04 18:56:01.162105 dunderlab-docs-0.8/
--rw-r--r--   0 yeison    (1000) users      (984)     1319 2022-11-25 19:45:17.000000 dunderlab-docs-0.8/LICENSE
--rw-r--r--   0 yeison    (1000) users      (984)      206 2023-02-14 16:29:56.000000 dunderlab-docs-0.8/MANIFEST.in
--rw-r--r--   0 yeison    (1000) users      (984)     6630 2023-03-04 18:56:01.162105 dunderlab-docs-0.8/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)     5338 2023-03-04 18:53:54.000000 dunderlab-docs-0.8/README.md
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-04 18:56:01.158771 dunderlab-docs-0.8/dunderlab/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-04 18:56:01.158771 dunderlab-docs-0.8/dunderlab/docs/
--rw-r--r--   0 yeison    (1000) users      (984)     9325 2023-03-04 18:20:15.000000 dunderlab-docs-0.8/dunderlab/docs/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-04 18:56:01.158771 dunderlab-docs-0.8/dunderlab/docs/static/
--rw-r--r--   0 yeison    (1000) users      (984)     1941 2023-03-04 18:40:34.000000 dunderlab-docs-0.8/dunderlab/docs/static/dunderlab_custom.css
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-04 18:56:01.162105 dunderlab-docs-0.8/dunderlab_docs.egg-info/
--rw-r--r--   0 yeison    (1000) users      (984)     6630 2023-03-04 18:56:01.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)      334 2023-03-04 18:56:01.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-03-04 18:56:01.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-01-20 15:59:18.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/not-zip-safe
--rw-r--r--   0 yeison    (1000) users      (984)        9 2023-03-04 18:56:01.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) users      (984)       10 2023-03-04 18:56:01.000000 dunderlab-docs-0.8/dunderlab_docs.egg-info/top_level.txt
--rw-r--r--   0 yeison    (1000) users      (984)       38 2023-03-04 18:56:01.162105 dunderlab-docs-0.8/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (984)     1760 2023-03-04 18:49:50.000000 dunderlab-docs-0.8/setup.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/
+-rw-r--r--   0 yeison    (1000) users      (984)     1319 2022-11-25 19:45:17.000000 dunderlab-docs-0.9/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)      206 2023-02-14 16:29:56.000000 dunderlab-docs-0.9/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) users      (984)     6630 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)     5338 2023-03-05 02:59:02.000000 dunderlab-docs-0.9/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-05 03:08:34.687699 dunderlab-docs-0.9/dunderlab/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/dunderlab/docs/
+-rw-r--r--   0 yeison    (1000) users      (984)     9946 2023-03-05 02:56:49.000000 dunderlab-docs-0.9/dunderlab/docs/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/dunderlab/docs/static/
+-rw-r--r--   0 yeison    (1000) users      (984)     1941 2023-03-04 18:40:34.000000 dunderlab-docs-0.9/dunderlab/docs/static/dunderlab_custom.css
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/dunderlab_docs.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)     6630 2023-03-05 03:08:34.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)      334 2023-03-05 03:08:34.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-03-05 03:08:34.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-01-20 15:59:18.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/not-zip-safe
+-rw-r--r--   0 yeison    (1000) users      (984)        9 2023-03-05 03:08:34.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       10 2023-03-05 03:08:34.000000 dunderlab-docs-0.9/dunderlab_docs.egg-info/top_level.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-03-05 03:08:34.691033 dunderlab-docs-0.9/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     1760 2023-03-05 03:07:48.000000 dunderlab-docs-0.9/setup.py
```

### Comparing `dunderlab-docs-0.8/LICENSE` & `dunderlab-docs-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dunderlab-docs-0.8/PKG-INFO` & `dunderlab-docs-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-docs
-Version: 0.8
+Version: 0.9
 Download-URL: 
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: Simplified BSD License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dunderlab-docs-0.8/README.md` & `dunderlab-docs-0.9/README.md`

 * *Files identical despite different names*

### Comparing `dunderlab-docs-0.8/dunderlab/docs/__init__.py` & `dunderlab-docs-0.9/dunderlab/docs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,14 +140,23 @@
     * :ref:`genindex`
     * :ref:`modindex`
     * :ref:`search`
        """
     else:
         code_reference = ""
 
+    if os.path.exists(os.path.join(notebooks_path, "footer.ipynb")):
+        dunderlab_footer = f"""
+        .. container:: dunderlab-footer
+
+            .. include:: {notebooks_dir}/footer.rst
+        """
+    else:
+        dunderlab_footer = ''
+
     with open(os.path.join(app.srcdir, 'index.rst'), 'w') as file:
         file.write(
             f"""
 .. include:: {notebooks_dir}/readme.rst
 
 {navigation_title}
 
@@ -157,21 +166,15 @@
 
    {notebooks}
 
 {dunderlab_custom_index}
 
 {code_reference}
 
-
-
-
-.. container:: dunderlab-footer
-
-    .. include:: {notebooks_dir}/footer.rst
-
+{dunderlab_footer}
         """
         )
 
     run_command(
         f'jupyter-nbconvert --to rst {os.path.join(notebooks_path, "readme.ipynb")}'
     )
 
@@ -188,14 +191,23 @@
             f'mv ../../../LICENSE.md ../../../LICENSE'
         )
 
     run_command(
         f'jupyter-nbconvert --to markdown {os.path.join(notebooks_path, "readme.ipynb")} --output ../../../README.md'
     )
 
+    if app.config.dunderlab_github_repository:
+
+        with open('../README.md', 'r') as file:
+            content = file.read()
+        content = content.replace(
+            '(_images/', f'({app.config.dunderlab_github_repository}/blob/master/docs/source/notebooks/_images/')
+        with open('../README.md', 'w') as file:
+            file.write(content)
+
 
 # ----------------------------------------------------------------------
 def build_features(app, *args, **kwargs) -> None:
     """"""
     target = os.path.abspath(os.path.join(app.srcdir, '_static', 'dunderlab_custom.css'))
     source = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static', 'dunderlab_custom.css')
     shutil.copyfile(source, target)
@@ -208,14 +220,15 @@
 
 # ----------------------------------------------------------------------
 def setup(app) -> dict:
     """"""
     app.add_config_value('dunderlab_custom_index', '', rebuild='env')
     app.add_config_value('dunderlab_color_links', '#00acc1', rebuild='html')
     app.add_config_value('dunderlab_code_reference', True, rebuild='html')
+    app.add_config_value('dunderlab_github_repository', '', rebuild='html')
 
     notebooks_dir = 'notebooks'
     notebooks_path = os.path.abspath(os.path.join(app.srcdir, notebooks_dir))
 
     if not os.path.exists(notebooks_path):
         os.makedirs(notebooks_path)
```

### Comparing `dunderlab-docs-0.8/dunderlab/docs/static/dunderlab_custom.css` & `dunderlab-docs-0.9/dunderlab/docs/static/dunderlab_custom.css`

 * *Files identical despite different names*

### Comparing `dunderlab-docs-0.8/dunderlab_docs.egg-info/PKG-INFO` & `dunderlab-docs-0.9/dunderlab_docs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-docs
-Version: 0.8
+Version: 0.9
 Download-URL: 
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: Simplified BSD License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dunderlab-docs-0.8/setup.py` & `dunderlab-docs-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='dunderlab-docs',
-    version='0.8',
+    version='0.9',
     packages=['dunderlab.docs', 'dunderlab.docs.static'],
     author='Yeison Cardona',
     author_email='yencardonaal@unal.edu.co',
     maintainer='Yeison Cardona',
     maintainer_email='yencardonaal@unal.edu.co',
     download_url='',
     install_requires=[
```

