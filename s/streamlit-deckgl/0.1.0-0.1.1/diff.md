# Comparing `tmp/streamlit-deckgl-0.1.0.tar.gz` & `tmp/streamlit-deckgl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.1.0.tar", last modified: Wed May  3 03:42:09 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.1.1.tar", last modified: Thu May  4 01:05:33 2023, max compression
```

## Comparing `streamlit-deckgl-0.1.0.tar` & `streamlit-deckgl-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-03 03:42:09.787621 streamlit-deckgl-0.1.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-03 03:42:09.787621 streamlit-deckgl-0.1.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1274 2023-04-28 04:00:31.000000 streamlit-deckgl-0.1.0/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-03 03:42:09.787621 streamlit-deckgl-0.1.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-01 21:52:11.000000 streamlit-deckgl-0.1.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-03 03:42:09.775622 streamlit-deckgl-0.1.0/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-03 03:42:09.779621 streamlit-deckgl-0.1.0/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1930 2023-05-01 23:05:39.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-03 03:42:09.783621 streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-04-29 06:28:45.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-03 03:42:09.779621 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-03 03:42:09.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-03 03:42:09.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-03 03:42:09.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       29 2023-05-03 03:42:09.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-03 03:42:09.000000 streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1274 2023-04-28 04:00:31.000000 streamlit-deckgl-0.1.1/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-04 01:05:19.000000 streamlit-deckgl-0.1.1/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.843577 streamlit-deckgl-0.1.1/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.847577 streamlit-deckgl-0.1.1/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1919 2023-05-04 01:05:08.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-04-29 06:28:45.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.847577 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.1.0/LICENSE` & `streamlit-deckgl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.0/PKG-INFO` & `streamlit-deckgl-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-deckgl-0.1.0/README.md` & `streamlit-deckgl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.0/setup.py` & `streamlit-deckgl-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.1.0",
+    version="0.1.1",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
     include_package_data=True,
     python_requires=">=3.7",
     keywords=["streamlit", "pydeck", "deck.gl", "visualisation"],
-    install_requires=["streamlit>=1.2", "jinja2", "pydeck"],
+    install_requires=["streamlit>=1.2", "jinja2", "pydeck>=0.8"],
     entry_points={},
 )
```

### Comparing `streamlit-deckgl-0.1.0/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.1.1/src/streamlit_deckgl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Returns
     =======
     component_value : dict
         A dictionary containing the info dictionary of the event.
 
     """
     json = deck.to_json()
-    tooltip = deck.deck_widget.tooltip
+    tooltip = deck._tooltip
     customLibraries = pdk.settings.custom_libraries
     configuration = pdk.settings.configuration
 
     component_value = _component_func(
         key=key,
         width=width,
         height=height,
```

### Comparing `streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/main.js` & `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.0/src/streamlit_deckgl.egg-info/PKG-INFO` & `streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

