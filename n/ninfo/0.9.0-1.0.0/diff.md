# Comparing `tmp/ninfo-0.9.0.tar.gz` & `tmp/ninfo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninfo-0.9.0.tar", last modified: Tue Jan 31 15:26:56 2023, max compression
+gzip compressed data, was "ninfo-1.0.0.tar", last modified: Thu May  4 18:15:25 2023, max compression
```

## Comparing `ninfo-0.9.0.tar` & `ninfo-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:26:56.464517 ninfo-0.9.0/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1084 2023-01-31 15:07:15.000000 ninfo-0.9.0/LICENSE
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       32 2023-01-31 15:07:15.000000 ninfo-0.9.0/MANIFEST.in
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-01-31 15:26:56.464517 ninfo-0.9.0/PKG-INFO
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     4925 2023-01-31 15:07:15.000000 ninfo-0.9.0/README.md
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:26:56.464517 ninfo-0.9.0/ninfo/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)    13937 2023-01-31 15:22:07.000000 ninfo-0.9.0/ninfo/__init__.py
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:26:56.464517 ninfo-0.9.0/ninfo/helpers/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:07:15.000000 ninfo-0.9.0/ninfo/helpers/__init__.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1869 2023-01-31 15:07:15.000000 ninfo-0.9.0/ninfo/helpers/splunk.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     3686 2023-01-31 15:22:07.000000 ninfo-0.9.0/ninfo/util.py
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:26:56.464517 ninfo-0.9.0/ninfo.egg-info/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/PKG-INFO
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      339 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/SOURCES.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/dependency_links.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       37 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/entry_points.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-01-31 15:09:13.000000 ninfo-0.9.0/ninfo.egg-info/not-zip-safe
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      120 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/requires.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        6 2023-01-31 15:26:56.000000 ninfo-0.9.0/ninfo.egg-info/top_level.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1350 2023-01-31 15:22:07.000000 ninfo-0.9.0/pyproject.toml
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       38 2023-01-31 15:26:56.464517 ninfo-0.9.0/setup.cfg
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      523 2023-01-31 15:22:07.000000 ninfo-0.9.0/setup.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1084 2023-01-31 15:07:15.000000 ninfo-1.0.0/LICENSE
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       32 2023-01-31 15:07:15.000000 ninfo-1.0.0/MANIFEST.in
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:15:25.206552 ninfo-1.0.0/PKG-INFO
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     4925 2023-01-31 15:07:15.000000 ninfo-1.0.0/README.md
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.202552 ninfo-1.0.0/ninfo/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)    14652 2023-05-04 18:03:17.000000 ninfo-1.0.0/ninfo/__init__.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/ninfo/helpers/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:07:15.000000 ninfo-1.0.0/ninfo/helpers/__init__.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1869 2023-01-31 15:07:15.000000 ninfo-1.0.0/ninfo/helpers/splunk.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     3686 2023-01-31 15:22:07.000000 ninfo-1.0.0/ninfo/util.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/ninfo.egg-info/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/PKG-INFO
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      398 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       37 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/entry_points.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-01-31 15:09:13.000000 ninfo-1.0.0/ninfo.egg-info/not-zip-safe
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      120 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/requires.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        6 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/top_level.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1350 2023-05-04 18:03:17.000000 ninfo-1.0.0/pyproject.toml
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       38 2023-05-04 18:15:25.206552 ninfo-1.0.0/setup.cfg
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      523 2023-05-04 18:03:17.000000 ninfo-1.0.0/setup.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/tests/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      841 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_clone.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1515 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_ninfo.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     2724 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_util.py
```

### Comparing `ninfo-0.9.0/LICENSE` & `ninfo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninfo-0.9.0/PKG-INFO` & `ninfo-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfo
-Version: 0.9.0
+Version: 1.0.0
 Summary: Plugin based information gathering library
 Author-email: Justin Azoff <justin.azoff@gmail.com>, Ryan Goggin <support@ryangoggin.net>
 Project-URL: Homepage, https://github.com/ninfo-py/ninfo
 Keywords: ninfo,search
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ninfo-0.9.0/README.md` & `ninfo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ninfo-0.9.0/ninfo/__init__.py` & `ninfo-1.0.0/ninfo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pkg_resources import iter_entry_points
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 import memcache
-
 import logging
 
 logger = logging.getLogger("ninfo")
 
 import os
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
+import json
+
 from mako.template import Template
 
 try:
     from inspect import getargspec
 except ImportError:
     from inspect import getfullargspec as getargspec
 
@@ -39,15 +40,14 @@
 
 
 class PluginInitError(PluginError):
     pass
 
 
 class PluginBase(object):
-
     cache_timeout = 60 * 60
     local = True
     remote = True
     template = True
     options = {}
     converters = {}
 
@@ -57,14 +57,19 @@
             config = {}
         if plugin_config is None:
             plugin_config = {}
         self.config = config
         self.plugin_config = plugin_config
         self.initialized = False
         self._name = self.name
+        self._template = self.name
+
+        if "template_override" in plugin_config:
+            self._template = plugin_config["template_override"]
+
         if "disabled" in plugin_config:
             return
 
     def init(self):
         if self.initialized:
             return True
         try:
@@ -132,15 +137,15 @@
 
         out = self._do_render(filename, arg, result)
         return out
 
     def get_template(self, output_type):
         code = getsourcefile(self.__class__)
         path = os.path.dirname(code)
-        filename = "%s_template_%s.mako" % (self._name, output_type)
+        filename = "%s_template_%s.mako" % (self._template, output_type)
         template = os.path.join(path, filename)
         if os.path.exists(template):
             return template
 
     def get_converter(self, a, b):
         func = self.converters.get((a, b))
         if func:
@@ -348,17 +353,17 @@
                 continue
             try:
                 result = self.get_info(p.name, arg, options)
                 yield p, result
             except PluginError:
                 logger.exception("Error running plugin %s", p.name)
 
-    def get_info_dict(self, arg):
+    def get_info_dict(self, arg, plugins=None, options={}):
         res = {}
-        for p, result in self.get_info_iter(arg):
+        for p, result in self.get_info_iter(arg, plugins, options):
             res[p.name] = result
         return res
 
     def show_info(self, arg, plugins=None, options={}):
         for p, result in self.get_info_iter(arg, plugins, options):
             print("*** %s (%s) ***" % (p.title, p.description))
             print(p.render_template("text", arg, result))
@@ -379,15 +384,30 @@
     logging.basicConfig(level=logging.INFO)
     # requests logs stuff at level INFO
     logging.getLogger("requests.packages.urllib3").setLevel(logging.ERROR)
 
     from optparse import OptionParser
 
     parser = OptionParser(usage="usage: %prog [options] [addresses]")
-    parser.add_option("-p", "--plugin", dest="plugins", action="append", default=None)
+    parser.add_option(
+        "-p",
+        "--plugin",
+        dest="plugins",
+        action="append",
+        help="The plugin to run",
+        default=None,
+    )
+    parser.add_option(
+        "-j",
+        "--json",
+        dest="json",
+        action="store_true",
+        help="Output json instead of rendering",
+        default=False,
+    )
     parser.add_option("-l", "--list", dest="list", action="store_true", default=False)
     (options, complete_args) = parser.parse_args()
 
     p = Ninfo()
     if options.list:
         print("%-20s %-20s %s" % ("Name", "Title", "Description"))
         for pl in p.plugins:
@@ -400,15 +420,22 @@
         if "=" in arg:
             (ctxt_name, ctxt_value) = arg.split("=", 1)
             context_options[ctxt_name] = ctxt_value
         else:
             args.append(arg)
 
     plugins = options.plugins or None
+    json_output = []
     for arg in args:
         if len(args) != 1:
             print("=== %s === " % (arg,))
-        p.show_info(arg, plugins=plugins, options=context_options)
+        if options.json:
+            json_output.append({"arg": arg, "data": p.get_info_dict(arg, plugins=plugins, options=context_options)})
+        else:
+            p.show_info(arg, plugins=plugins, options=context_options)
+
+    if options.json:
+        print(json.dumps(json_output))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ninfo-0.9.0/ninfo/helpers/splunk.py` & `ninfo-1.0.0/ninfo/helpers/splunk.py`

 * *Files identical despite different names*

### Comparing `ninfo-0.9.0/ninfo/util.py` & `ninfo-1.0.0/ninfo/util.py`

 * *Files identical despite different names*

### Comparing `ninfo-0.9.0/ninfo.egg-info/PKG-INFO` & `ninfo-1.0.0/ninfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfo
-Version: 0.9.0
+Version: 1.0.0
 Summary: Plugin based information gathering library
 Author-email: Justin Azoff <justin.azoff@gmail.com>, Ryan Goggin <support@ryangoggin.net>
 Project-URL: Homepage, https://github.com/ninfo-py/ninfo
 Keywords: ninfo,search
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ninfo-0.9.0/pyproject.toml` & `ninfo-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninfo"
-version = "0.9.0"
+version = "1.0.0"
 description = "Plugin based information gathering library"
 readme = "README.md"
 authors = [{ name = "Justin Azoff", email = "justin.azoff@gmail.com" }, { name = "Ryan Goggin", email = "support@ryangoggin.net" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 [project.urls]
 Homepage = "https://github.com/ninfo-py/ninfo"
 
 [project.scripts]
 ninfo = "ninfo:main"
 
 [tool.bumpver]
-current_version = "0.9.0"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `ninfo-0.9.0/setup.py` & `ninfo-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='ninfo',
-    version='0.9.0',
+    version='1.0.0',
     zip_safe=False,
     description="Plugin based information gathering library",
     packages = find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "Mako",
         "python-memcached",
```

