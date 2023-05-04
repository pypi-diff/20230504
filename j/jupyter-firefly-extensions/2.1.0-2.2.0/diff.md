# Comparing `tmp/jupyter_firefly_extensions-2.1.0.tar.gz` & `tmp/jupyter_firefly_extensions-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyter_firefly_extensions-2.1.0.tar", last modified: Fri May  6 18:13:00 2022, max compression
+gzip compressed data, was "jupyter_firefly_extensions-2.2.0.tar", last modified: Thu May  4 21:00:51 2023, max compression
```

## Comparing `jupyter_firefly_extensions-2.1.0.tar` & `jupyter_firefly_extensions-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 roby       (555) staff       (20)        0 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/
--rw-rw-r--   0 roby       (555) staff       (20)      785 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/PKG-INFO
-drwxrwxr-x   0 roby       (555) staff       (20)        0 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/
--rw-rw-r--   0 roby       (555) staff       (20)      252 2022-05-06 17:37:08.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/_version.py
--rwxrwxr-x   0 roby       (555) staff       (20)     5213 2022-05-06 17:51:10.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/__init__.py
--rw-rw-r--   0 roby       (555) staff       (20)      312 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/chart.py
-drwxrwxr-x   0 roby       (555) staff       (20)        0 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/labextension/
--rw-rw-r--   0 roby       (555) staff       (20)    49379 2018-09-26 19:20:28.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/labextension/jupyter_firefly_extensions-0.1.0.tgz
--rw-rw-r--   0 roby       (555) staff       (20)     1443 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/utils.py
--rw-rw-r--   0 roby       (555) staff       (20)     1079 2019-02-14 23:06:57.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/slate_widget.py
--rw-rw-r--   0 roby       (555) staff       (20)      984 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/table.py
--rw-rw-r--   0 roby       (555) staff       (20)     1393 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/image.py
--rwxrwxr-x   0 roby       (555) staff       (20)       99 2018-09-25 16:52:48.000000 jupyter_firefly_extensions-2.1.0/MANIFEST.in
--rwxrwxr-x   0 roby       (555) staff       (20)     3791 2019-05-13 21:26:18.000000 jupyter_firefly_extensions-2.1.0/README.md
--rwxrwxr-x   0 roby       (555) staff       (20)     2912 2019-05-09 22:14:24.000000 jupyter_firefly_extensions-2.1.0/setup.py
-drwxrwxr-x   0 roby       (555) staff       (20)        0 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/
--rw-rw-r--   0 roby       (555) staff       (20)      785 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 roby       (555) staff       (20)      621 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 roby       (555) staff       (20)       73 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/requires.txt
--rw-rw-r--   0 roby       (555) staff       (20)       27 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/top_level.txt
--rw-rw-r--   0 roby       (555) staff       (20)        1 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 roby       (555) staff       (20)       38 2022-05-06 18:13:00.000000 jupyter_firefly_extensions-2.1.0/setup.cfg
+drwxrwxr-x   0 roby       (555) staff       (20)        0 2023-05-04 21:00:51.153379 jupyter_firefly_extensions-2.2.0/
+-rwxrwxr-x   0 roby       (555) staff       (20)       99 2018-09-25 16:52:48.000000 jupyter_firefly_extensions-2.2.0/MANIFEST.in
+-rw-rw-r--   0 roby       (555) staff       (20)      747 2023-05-04 21:00:51.153263 jupyter_firefly_extensions-2.2.0/PKG-INFO
+-rwxrwxr-x   0 roby       (555) staff       (20)     3061 2022-05-06 19:10:54.000000 jupyter_firefly_extensions-2.2.0/README.md
+drwxrwxr-x   0 roby       (555) staff       (20)        0 2023-05-04 21:00:51.151115 jupyter_firefly_extensions-2.2.0/jupyter-config/
+drwxrwxr-x   0 roby       (555) staff       (20)        0 2023-05-04 21:00:51.151763 jupyter_firefly_extensions-2.2.0/jupyter-config/jupyter_server_config.d/
+-rw-rw-r--   0 roby       (555) staff       (20)      120 2023-05-03 21:40:38.000000 jupyter_firefly_extensions-2.2.0/jupyter-config/jupyter_server_config.d/jupyter_firefly_extensions.json
+drwxrwxr-x   0 roby       (555) staff       (20)        0 2023-05-04 21:00:51.152551 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/
+-rwxrwxr-x   0 roby       (555) staff       (20)     5439 2023-05-04 20:28:13.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/__init__.py
+-rw-rw-r--   0 roby       (555) staff       (20)      252 2023-05-04 20:33:36.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/_version.py
+-rw-rw-r--   0 roby       (555) staff       (20)      312 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/chart.py
+-rw-rw-r--   0 roby       (555) staff       (20)     1393 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/image.py
+-rw-rw-r--   0 roby       (555) staff       (20)     1079 2019-02-14 23:06:57.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/slate_widget.py
+-rw-rw-r--   0 roby       (555) staff       (20)      984 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/table.py
+-rw-rw-r--   0 roby       (555) staff       (20)     1443 2018-12-11 20:24:45.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/utils.py
+drwxrwxr-x   0 roby       (555) staff       (20)        0 2023-05-04 21:00:51.153110 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/
+-rw-rw-r--   0 roby       (555) staff       (20)      747 2023-05-04 21:00:51.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 roby       (555) staff       (20)      615 2023-05-04 21:00:51.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 roby       (555) staff       (20)        1 2023-05-04 21:00:51.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 roby       (555) staff       (20)       73 2023-05-04 21:00:51.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/requires.txt
+-rw-rw-r--   0 roby       (555) staff       (20)       27 2023-05-04 21:00:51.000000 jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/top_level.txt
+-rw-rw-r--   0 roby       (555) staff       (20)       38 2023-05-04 21:00:51.153414 jupyter_firefly_extensions-2.2.0/setup.cfg
+-rwxrwxr-x   0 roby       (555) staff       (20)     3119 2023-05-04 16:43:52.000000 jupyter_firefly_extensions-2.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jupyter_firefly_extensions-2.1.0/PKG-INFO` & `jupyter_firefly_extensions-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: jupyter_firefly_extensions
-Version: 2.1.0
-Summary: UNKNOWN
+Version: 2.2.0
 Home-page: https://github.com/Caltech-IPAC/firefly
 Author: Trey Roby
 Author-email: roby@ipac.caltech.edu
 License: BSD
-Description: UNKNOWN
 Keywords: jupyter,firefly,caltech,ipac,astronomy,visualization
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/__init__.py` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -148,20 +148,26 @@
 
     hostname = platform.node()
     timestamp = time.time()
     channel = 'ffChan-{}-{}-{}'.format(hostname, int(timestamp), random.randint(1, 100))
     page_config['fireflyChannel'] = channel
     logger.info('firefly URL: {}'.format(url))
     logger.info('firefly Channel: {}'.format(channel))
+    # added next two lines because logger does not seem to work JL 3.5
+    print('firefly URL: {}'.format(url))
+    print('firefly Channel: {}'.format(channel))
     os.environ['fireflyChannelLab'] = channel
     os.environ['fireflyURLLab'] = url
     os.environ['fireflyLabExtension'] = 'true'
     firefly_config = dict(page_config)
 
     # setup server endpoint: sendToFirefly: http://127.0.0.1:8888/lab/sendToFirefly?path=x.fits
     host_pattern = '.*$'
     send_pattern = url_path_join(web_app.settings['base_url'], 'lab/sendToFirefly')
     get_ff_data_pattern = url_path_join(web_app.settings['base_url'], 'lab/fireflyLocation')
     web_app.add_handlers(host_pattern, [
         (send_pattern, SendToFireflyHandler, {'notebook_dir': nb_server_app.notebook_dir, 'firefly_url': url}),
         (get_ff_data_pattern, GetFireflyUrlData, {})
     ])
+
+
+_load_jupyter_server_extension = load_jupyter_server_extension
```

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/utils.py` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/slate_widget.py` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/slate_widget.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/table.py` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/table.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions/image.py` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions/image.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-2.1.0/README.md` & `jupyter_firefly_extensions-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,25 @@
 
 This extension adds the following features to JupyterLab:
 
   - Double click or right-click on a FITS file and see it in a tab
   - Start the full Firefly viewer in a tab.
   - Use `FireflyClient` in a Python notebook to start Firefly in a tab and send data
   (tables, images, charts) to it using the `FireflyClient` API
-  - There are several widgets (images, tables, charts) that can be used in a notebook
   - The `SlateWidget` is a full Firefly viewer widget that provides a `FireflyClient` instance to embed a full Firefly in a notebook as a widget
 
 
 
 ## Prerequisites
 
 * JupyterLab ^0.35.1
 * nodejs
-* ipywidgets ^7.0.0
 * astropy ^3.0.0
 * firefly_client ^2.1.1
 
-The first four prerequisites can be installed with `conda install jupyterlab nodejs ipywidgets astropy`.
 The `firefly_client` package can be installed with `pip install firefly_client`.
 
 ### _Very Important_: first setup the Firefly URL - 3 ways
 
  * Add the following line to your `~/.jupyter/jupyter_notebook_config.py`
 
    ```python
@@ -58,19 +55,16 @@
 
 **where the URL points to a Firefly server.**
 
 
 
 ### Install
 
-To use any of the widgets in this package you must install the jupyter widget manager (`@jupyter-widgets/jupyterlab-manager`)
-
 ```bash
 pip install firefly_client
-jupyter labextension install @jupyter-widgets/jupyterlab-manager
 jupyter labextension install jupyter_firefly_extensions
 pip install jupyter_firefly_extensions
 jupyter serverextension enable --py jupyter_firefly_extensions
 ```
 
 ### Install for development
 
@@ -78,15 +72,14 @@
 
 If developing `firefly_client`, be sure to clone the `firefly_client` repository
 (https://github.com/Caltech-IPAC/firefly_client)
 and then do `pip install -e .` from inside its directory.
 
 _Then:_
 ```bash
-jupyter labextension install @jupyter-widgets/jupyterlab-manager --no-build
 git clone https://github.com/Caltech-IPAC/jupyter_firefly_extensions
 cd jupyter_firefly_extensions
 jupyter labextension install . --no-build
 jupyter lab build
 pip install -e .
 jupyter serverextension enable --py jupyter_firefly_extensions
 ```
@@ -99,25 +92,19 @@
  - `jupyter labextension list` - show a list of lab extensions
  - `jupyter lab` - run jupyter lab
  - `jupyter lab build` - rebuild after modifying the javascript:
 
 
 ### To remove extensions:
 ```bash
-jupyter labextension uninstall @jupyter-widgets/jupyterlab-manager --no-build
 jupyter labextension uninstall jupyter_firefly_extensions
 jupyter serverextension disable --py jupyter_firefly_extensions
 pip uninstall jupyter_firefly_extensions
 ```
 
 
 ### Examples
 The `examples` directory has several example notebooks to demonstrate the extension features. When using the examples you should copy the directory and contents to another place or jupyter lab will and to keep rebuilding
 
  - `slate-demo-explicit.ipynb`, `slate-demo-explicit2.ipynb` - demonstrates
     opening a Firefly tab and sending data to it with the `FireflyClient` python API
  - `slate-widget-demo.ipnb` - simple demo of the Firefly slate widget
- - Three example demoing the images, tables, and charts widgets
-     - `Image Colorbar Test.ipynb`
-     - `Image Zoom and Pan Test.ipynb`
-     - `Images and Tables.ipynb`
-`
```

### Comparing `jupyter_firefly_extensions-2.1.0/setup.py` & `jupyter_firefly_extensions-2.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,17 +49,23 @@
 package_data = {
     name: [
         'nbextension/*.*js*',
         'labextension/*.tgz'
     ]
 }
 
+name = "jupyter_firefly_extensions"
+include_package_data = True
 data_files = expand_data_files([
     ('share/jupyter/nbextensions/jupyter_firefly_extensions', [pjoin(nbextension, '*.js*')]),
-    ('share/jupyter/lab/extensions', [pjoin(labextension, '*.tgz')])
+    ('share/jupyter/lab/extensions', [pjoin(labextension, '*.tgz')]),
+    (
+        "etc/jupyter/jupyter_server_config.d",
+        ["jupyter-config/jupyter_server_config.d/jupyter_firefly_extensions.json"]
+    )
 ])
 
 
 setup_args = dict(
     name            = name,
     version         = version_ns['__version__'],
     scripts         = glob(pjoin('scripts', '*')),
```

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/PKG-INFO` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: jupyter-firefly-extensions
-Version: 2.1.0
-Summary: UNKNOWN
+Version: 2.2.0
 Home-page: https://github.com/Caltech-IPAC/firefly
 Author: Trey Roby
 Author-email: roby@ipac.caltech.edu
 License: BSD
-Description: UNKNOWN
 Keywords: jupyter,firefly,caltech,ipac,astronomy,visualization
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jupyter_firefly_extensions-2.1.0/jupyter_firefly_extensions.egg-info/SOURCES.txt` & `jupyter_firefly_extensions-2.2.0/jupyter_firefly_extensions.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MANIFEST.in
 README.md
 setup.py
+jupyter-config/jupyter_server_config.d/jupyter_firefly_extensions.json
 jupyter_firefly_extensions/__init__.py
 jupyter_firefly_extensions/_version.py
 jupyter_firefly_extensions/chart.py
 jupyter_firefly_extensions/image.py
 jupyter_firefly_extensions/slate_widget.py
 jupyter_firefly_extensions/table.py
 jupyter_firefly_extensions/utils.py
 jupyter_firefly_extensions.egg-info/PKG-INFO
 jupyter_firefly_extensions.egg-info/SOURCES.txt
 jupyter_firefly_extensions.egg-info/dependency_links.txt
 jupyter_firefly_extensions.egg-info/requires.txt
-jupyter_firefly_extensions.egg-info/top_level.txt
-jupyter_firefly_extensions/labextension/jupyter_firefly_extensions-0.1.0.tgz
+jupyter_firefly_extensions.egg-info/top_level.txt
```

