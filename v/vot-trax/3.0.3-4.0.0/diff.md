# Comparing `tmp/vot-trax-3.0.3.tar.gz` & `tmp/vot-trax-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vot-trax-3.0.3.tar", last modified: Thu Nov 12 15:08:22 2020, max compression
+gzip compressed data, was "vot-trax-4.0.0.tar", last modified: Thu May  4 21:27:08 2023, max compression
```

## Comparing `vot-trax-3.0.3.tar` & `vot-trax-4.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2020-11-12 15:08:22.643010 vot-trax-3.0.3/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1049 2020-11-12 15:08:22.643010 vot-trax-3.0.3/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        6 2020-11-12 15:07:02.746830 vot-trax-3.0.3/VERSION
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3127 2020-11-12 15:07:02.746830 vot-trax-3.0.3/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2020-11-12 15:08:22.643010 vot-trax-3.0.3/trax/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6685 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6953 2020-11-12 15:07:02.758830 vot-trax-3.0.3/trax/base64.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      335 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/base64.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4548 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/buffer.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8013 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/client.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1562 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/debug.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      971 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/debug.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7954 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/image.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    20976 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/internal.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23407 2020-11-12 15:07:02.758830 vot-trax-3.0.3/trax/message.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1810 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/message.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30473 2020-11-12 15:07:02.758830 vot-trax-3.0.3/trax/region.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3364 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/region.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8708 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/region.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5916 2020-11-12 15:07:02.754830 vot-trax-3.0.3/trax/server.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14754 2020-11-12 15:07:02.758830 vot-trax-3.0.3/trax/strmap.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12968 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/strmap.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    43846 2020-11-12 15:07:02.758830 vot-trax-3.0.3/trax/trax.c
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29722 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/trax.h
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    18170 2020-11-12 15:07:02.762830 vot-trax-3.0.3/trax/traxpp.cpp
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-04 21:27:08.575316 vot-trax-4.0.0/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1053 2023-05-04 21:27:08.575316 vot-trax-4.0.0/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      544 2023-05-04 21:26:46.047421 vot-trax-4.0.0/README.rst
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        6 2023-05-04 21:26:06.363611 vot-trax-4.0.0/VERSION
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3126 2023-05-04 21:26:06.363611 vot-trax-4.0.0/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-04 21:27:08.575316 vot-trax-4.0.0/trax/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-04 21:26:46.063421 vot-trax-4.0.0/trax/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    54378 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/_ctypes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6953 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/base64.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      335 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/base64.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4548 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/buffer.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7944 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/client.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1562 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/debug.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      971 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/debug.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8029 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/image.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23442 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/message.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1810 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/message.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30473 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/region.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3364 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/region.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8687 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/region.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5967 2023-05-04 21:26:46.067421 vot-trax-4.0.0/trax/server.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14754 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/strmap.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12968 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/strmap.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    58417 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/trax.c
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    36170 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/trax.h
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24834 2023-05-04 21:26:46.083421 vot-trax-4.0.0/trax/traxpp.cpp
```

### Comparing `vot-trax-3.0.3/PKG-INFO` & `vot-trax-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: vot-trax
-Version: 3.0.3
+Version: 4.0.0
 Summary: TraX protocol reference implementation wrapper for Python
 Home-page: https://github.com/votchallenge/trax/
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
-        [Visual Tracking eXchange protocol](http://prints.vicos.si/publications/311/) is a simple protocol that enables easier evaluation of computer vision tracking algorithms. The basic idea is that a tracker communicates with the evaluation software using a set of text commands over the (standard) input/output streams or TCP sockets. 
+        `Visual Tracking eXchange protocol <http://prints.vicos.si/publications/311/>`_ is a simple protocol that enables easier evaluation of computer vision tracking algorithms. The basic idea is that a tracker communicates with the evaluation software using a set of text commands over the (standard) input/output streams or TCP sockets. 
         
-        This package contains a Python wrapper to C library (using CTypes) available in the `support/python` directory. More information and source code available at [Github](https://github.com/votchallenge/trax/).
+        This package contains a Python wrapper to C library (using CTypes) available in the `support/python` directory. More information and source code available at `Github <https://github.com/votchallenge/trax/>`_.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `vot-trax-3.0.3/setup.py` & `vot-trax-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,24 @@
             python, abi, plat = _bdist_wheel.get_tag(self)
             # We don't contain any python source
             python, abi = 'py2.py3', 'none'
             return python, abi, plat
 
 except ImportError:
     bdist_wheel = None
-
 try:
     with open(os.path.join(root, "VERSION"), encoding='utf-8') as fp:
         VERSION = fp.readline().strip()
 
 except IOError:
     VERSION = os.getenv("TRAX_VERSION", "unknown")
 
 try:
-    with open(os.path.join(root, 'README.md'), encoding='utf-8') as f:
+    with open(os.path.join(root, 'README.rst'), encoding='utf-8') as f:
         long_description = f.read()
-
 except IOError:
     long_description = ""
 
 
 varargs = dict()
 
 if os.path.isfile(os.path.join("trax", library_prefix + "trax" + library_suffix)):
```

### Comparing `vot-trax-3.0.3/trax/__init__.py` & `vot-trax-4.0.0/trax/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 
 import sys, os
 import traceback
 import weakref
 from ctypes import py_object, c_void_p, cast, byref, POINTER
 
-from .internal import \
+from ._ctypes import \
     trax_properties_enumerate, trax_properties_create, trax_enumerator, \
-    trax_properties_get, trax_properties_set, trax_properties_p, \
-    trax_image_release, trax_region_release, \
+    trax_properties_get, trax_properties_set, trax_object_list, \
+    trax_image_release, trax_region_release, trax_object_list_release, \
     trax_cleanup, trax_properties_release, trax_image_list_release, \
     struct_trax_handle, struct_trax_image, struct_trax_image_list, \
-    struct_trax_metadata, struct_trax_properties, POINTER_T
+    struct_trax_properties, struct_trax_object_list, POINTER
 
+trax_image_p = POINTER(struct_trax_image)
+trax_image_list_p = POINTER(struct_trax_image_list)
+trax_region_p = c_void_p
+trax_object_list_p = POINTER(trax_object_list)
+trax_properties_p = POINTER(struct_trax_properties)
 class TraxException(Exception):
     pass
 
 class TraxStatus(object):
     """ The message type container class """
     ERROR = "error"
     OK = "ok"
@@ -142,52 +147,119 @@
         if not self.ref:
             return None
         return self.ref.item
 
     def __nonzero__(self):
         return not self.ref is None
 
+def _debug_wrapper(cb, message):
+    def wrapper(*args, **kwargs):
+        print(message, args, kwargs)
+        cb(*args, **kwargs)
+    return wrapper
 class ImageWrapper(Wrapper):
 
     def __init__(self, reference, owner=True):
-        super().__init__(POINTER_T(struct_trax_image), reference, lambda x: trax_image_release(byref(x)) if owner else None)
+        super().__init__(POINTER(struct_trax_image), reference, lambda x: trax_image_release(byref(x)) if owner else None)
 
 class ImageListWrapper(Wrapper):
 
     def __init__(self, reference, owner=True):
-        super().__init__(POINTER_T(struct_trax_image_list), reference, lambda x: trax_image_list_release(byref(x)) if owner else None)
+        super().__init__(POINTER(struct_trax_image_list), reference, lambda x: trax_image_list_release(byref(x)) if owner else None)
+
+class ObjectListWrapper(Wrapper):
+
+    def __init__(self, reference, owner=True):
+        super().__init__(POINTER(struct_trax_object_list), reference, lambda x: trax_object_list_release(byref(x)) if owner else None)
 
 class RegionWrapper(Wrapper):
 
     def __init__(self, reference, owner=True):
         super().__init__(c_void_p, reference, lambda x: trax_region_release(byref(cast(x, c_void_p))) if owner else None)
 
 class PropertiesWrapper(Wrapper):
 
     def __init__(self, reference, owner=True):
-        super().__init__(POINTER_T(struct_trax_properties), reference, lambda x: trax_properties_release(byref(x)) if owner else None)
+        super().__init__(POINTER(struct_trax_properties), reference, lambda x: trax_properties_release(byref(x)) if owner else None)
 
 class HandleWrapper(Wrapper):
 
     def __init__(self, reference, owner=True):
-        super().__init__(POINTER_T(struct_trax_handle), reference, lambda x: trax_cleanup(byref(x)) if owner else None)
+        super().__init__(POINTER(struct_trax_handle), reference, lambda x: trax_cleanup(byref(x)) if owner else None)
+
+def wrap_image_list(list):
+    from ._ctypes import trax_image_list_get
+
+    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
+    wrapped = {}
+
+    for channel in channels:
+        img = trax_image_list_get(list, ImageChannel.encode(channel))
+        if not img:
+            continue
+        wrapped[channel] = Image.wrap(img)
+
+    return wrapped
+
+def wrap_object_list(list):
+    from ._ctypes import trax_object_list_count, \
+        trax_object_list_get, trax_object_list_properties, \
+        trax_region_clone
+    import ctypes
+
+    objects = []
+    for i in range(trax_object_list_count(list)):
+        region = trax_object_list_get(list, i)
+        properties = Properties(trax_object_list_properties(list, i), False).dict()
+        r = trax_region_clone(region)
+        objects.append((Region.wrap(ctypes.cast(r, c_void_p)), properties))
+    return objects
 
 
+def wrap_images(images):
+    from ._ctypes import trax_image_list_create, trax_image_list_set
+
+    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
+    tlist = ImageListWrapper(trax_image_list_create())
+
+    for channel in channels:
+        if not channel in images:
+            continue
+
+        trax_image_list_set(tlist.reference, images[channel].reference, ImageChannel.encode(channel))
+
+    return tlist
+
+def wrap_objects(objects):
+    from ._ctypes import trax_properties_append, trax_object_list_set, \
+         trax_object_list_properties, trax_object_list_create
+    tlist = ObjectListWrapper(trax_object_list_create(len(objects)))
+
+    for i, (region, properties) in enumerate(objects):
+        properties =  Properties(properties, False)
+        trax_object_list_set(tlist.reference, i, region.reference)
+        trax_properties_append(trax_object_list_properties(tlist.reference, i), properties.reference, 0)
+
+    return tlist
 class Properties(object):
 
     def __init__(self, data=None, owner=True):
         if not data:
             self._ref = PropertiesWrapper(trax_properties_create())
         elif isinstance(data, trax_properties_p):
             self._ref = PropertiesWrapper(data, owner)
         elif isinstance(data, dict):
             self._ref = PropertiesWrapper(trax_properties_create())
             for key, value in data.items():
                 trax_properties_set(self._ref.reference, key.encode('utf8'), str(value).encode('utf8'))
 
+    def copy(self, source: "Properties"):
+        for k, v in source.dict().items():
+            self[k] = v
+
     @property
     def reference(self):
         return self._ref.reference
 
     def __getitem__(self, key):
         return trax_properties_get(self._ref.reference, key)
```

### Comparing `vot-trax-3.0.3/trax/base64.c` & `vot-trax-4.0.0/trax/base64.c`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/buffer.h` & `vot-trax-4.0.0/trax/buffer.h`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/client.py` & `vot-trax-4.0.0/trax/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,30 @@
 """
 Bindings for the TraX sever.
 """
 
-import os
 import time
-import collections
 
-from ctypes import byref, cast
+from ctypes import byref, c_int
 
-from . import TraxException, TraxStatus, Properties, HandleWrapper, ImageListWrapper, \
-    ConsoleLogger, FileLogger, ProxyLogger
+from . import TraxException, TraxStatus, Properties, HandleWrapper, \
+    ConsoleLogger, FileLogger, ProxyLogger, trax_object_list_p
     
-from .internal import \
-    trax_image_list_set, trax_client_initialize, \
-    trax_client_wait, trax_region_p, trax_properties_p, \
-    trax_image_create_path, trax_client_frame, \
+from . import wrap_images, wrap_objects, wrap_object_list, ObjectListWrapper
+
+from ._ctypes import \
+    trax_client_initialize, \
+    trax_client_wait, trax_client_frame, \
     trax_client_setup_file, trax_client_setup_socket, \
-    trax_image_list_create, trax_logger_setup, trax_logger, \
-    trax_properties_create, trax_terminate, trax_get_error, \
-    trax_is_alive
+    trax_logger_setup, trax_logger, trax_get_parameter, \
+    trax_terminate, trax_get_error, trax_is_alive, TRAX_PARAMETER_MULTIOBJECT
+
 from .image import ImageChannel, Image
 from .region import Region
 
-def wrap_images(images):
-
-    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
-    tlist = ImageListWrapper(trax_image_list_create())
-
-    for channel in channels:
-        if not channel in images:
-            continue
-
-        trax_image_list_set(tlist.reference, images[channel].reference, ImageChannel.encode(channel))
-
-    return tlist
-
-
 class Client(object):
 
     """ TraX client."""
 
     def __init__(self, stream=None, timeout=30, log=False):
 
         if isinstance(log, bool) and log:
@@ -100,14 +85,19 @@
         self._tracker_description = metadata.contents.tracker_description.decode("utf-8") \
             if not metadata.contents.tracker_description is None else ""
 
         custom = Properties(metadata.contents.custom, False)
 
         self._custom = custom.dict()
 
+        value = c_int(value=0)   
+        trax_get_parameter(handle, TRAX_PARAMETER_MULTIOBJECT, byref(value))
+
+        self._custom["multiobject"] = bool(value.value)
+
     @property
     def channels(self):
         return self._channels
 
     @property
     def image_formats(self):
         return self._format_image
@@ -129,39 +119,41 @@
         return self._tracker_description
 
     def get(self, key):
         if key in self._custom:
             return self._custom[key]
         return None
 
-    def initialize(self, images, region, properties):
+    def initialize(self, images, objects, properties):
 
         timage = wrap_images(images)
-        tregion = region.reference
+        tobjects = wrap_objects(objects)
         tproperties = Properties(properties)
 
-        status = TraxStatus.decode(trax_client_initialize(self._handle.reference, timage.reference, tregion, tproperties.reference))
+        status = TraxStatus.decode(trax_client_initialize(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
 
         if self._logger and self._logger.interrupted:
             raise KeyboardInterrupt("Interrupted by user in log callback")
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when initializing tracker: {}".format(message))
 
-        tregion = trax_region_p()
+        tobjects = trax_object_list_p()
         properties = Properties()
 
         start = time.time()
 
-        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tregion), properties.reference))
+        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
 
         elapsed = time.time() - start
 
+        tobjects = ObjectListWrapper(tobjects)
+
         if self._logger and self._logger.interrupted:
             raise KeyboardInterrupt("Interrupted by user in log callback")
 
         if status == TraxStatus.ERROR:
             raise TraxException("Exception when waiting for response")
         if status == TraxStatus.QUIT:
             reason = properties.get("trax.reason", None)
@@ -171,59 +163,58 @@
                 raise TraxException("Server terminated the session: {}".format(reason))
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when waiting for response: {}".format(message))
 
-        region = Region.wrap(tregion)
+        return wrap_object_list(tobjects.reference), elapsed
 
-        return region, properties, elapsed
-
-    def frame(self, images, properties = dict()):
+    def frame(self, images, properties = dict(), objects = None):
 
         timage = wrap_images(images)
+        tobjects = wrap_objects(objects)
         tproperties = Properties(properties)
 
-        status = TraxStatus.decode(trax_client_frame(self._handle.reference, timage.reference, tproperties.reference))
+        status = TraxStatus.decode(trax_client_frame(self._handle.reference, timage.reference, tobjects.reference, tproperties.reference))
 
         if self._logger and self._logger.interrupted:
             raise KeyboardInterrupt("Interrupted by user in log callback")
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when sending frame to tracker: {}".format(message))
 
-        tregion = trax_region_p()
+        tobjects = trax_object_list_p()
         properties = Properties()
 
         start = time.time()
 
-        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tregion), properties.reference))
+        status = TraxStatus.decode(trax_client_wait(self._handle.reference, byref(tobjects), properties.reference))
 
         elapsed = time.time() - start
 
+        tobjects = ObjectListWrapper(tobjects)
+
         if self._logger and self._logger.interrupted:
             raise KeyboardInterrupt("Interrupted by user in log callback")
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when waiting for response: {}".format(message))
         if status == TraxStatus.QUIT:
             reason = properties.get("trax.reason", None)
             if reason is None:
                 raise TraxException("Server terminated the session")
             else:
                 raise TraxException("Server terminated the session: {}".format(reason))
             
-        region = Region.wrap(tregion)
-
-        return region, properties, elapsed
+        return wrap_object_list(tobjects.reference), elapsed
 
     def quit(self, reason=None):
         """ Sends quit message and end terminates communication. """
         if not reason is None:
             trax_terminate(self._handle.reference, reason.encode('utf-8'))
         else:
             trax_terminate(self._handle.reference, None)
```

### Comparing `vot-trax-3.0.3/trax/debug.c` & `vot-trax-4.0.0/trax/debug.c`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/debug.h` & `vot-trax-4.0.0/trax/debug.h`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/image.py` & `vot-trax-4.0.0/trax/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 Image description classes.
 """
 
 #from __future__ import absolute
 
-import sys
-import traceback
-import weakref
 from abc import abstractmethod
 from ctypes import memmove, byref, c_int, string_at
 
-from .internal import \
+from ._ctypes import \
         trax_image_create_path, trax_image_create_memory, \
         trax_image_get_memory_header, trax_image_get_type, \
         trax_image_get_path, trax_image_get_url, \
         trax_image_create_url, trax_image_get_memory_row, \
         trax_image_write_memory_row, trax_image_get_buffer, \
         trax_image_create_buffer
 from trax import TraxException, ImageWrapper
@@ -182,15 +179,19 @@
     _image_memory_map_string = {IMAGE_MEMORY_RGB : "rgb", IMAGE_MEMORY_GRAY8: "gray8", IMAGE_MEMORY_GRAY16: "gray16" }
     _image_memory_map_dtype = {IMAGE_MEMORY_RGB : np.uint8, IMAGE_MEMORY_GRAY8: np.uint8, IMAGE_MEMORY_GRAY16: np.uint16 }
     _image_memory_map_ch = {IMAGE_MEMORY_RGB : 3, IMAGE_MEMORY_GRAY8: 1, IMAGE_MEMORY_GRAY16: 1}
 
     class MemoryImage(Image):
 
         @staticmethod
-        def create(image):
+        def create(image: np.ndarray):
+
+            assert(isinstance(image, np.ndarray))
+
+            image = np.ascontiguousarray(image)
 
             width = image.shape[1]
             height = image.shape[0]
             format = 0
             if len(image.shape) == 3 and image.shape[2] == 3:
                 if image.itemsize == 1:
                     format = IMAGE_MEMORY_RGB
@@ -202,15 +203,16 @@
 
             if format == 0:
                 raise TraxException("Image format not supported")
 
             timage = trax_image_create_memory(width, height, format)
 
             data = trax_image_write_memory_row(timage, 0)
-            memmove(data, image.ctypes.data, image.nbytes)
+            
+            memmove(data, image.ctypes, image.nbytes)
             return MemoryImage(timage)
 
         def __str__(self):
             """ Get description """
             width = c_int()
             height = c_int()
             format = c_int()
@@ -222,30 +224,30 @@
             return Image.MEMORY
 
         def array(self):
             width = c_int()
             height = c_int()
             format = c_int()
             trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
-            mat = np.empty((height.value, width.value, _image_memory_map_ch[format.value]), dtype=_image_memory_map_dtype[format.value])
+            mat = np.ones((height.value, width.value, _image_memory_map_ch[format.value]), dtype=_image_memory_map_dtype[format.value])
 
             data = trax_image_get_memory_row(self.reference, 0)
+
             memmove(mat.ctypes.data, data, mat.nbytes)
 
             return mat
 except ImportError:
 
     class MemoryImage(Image):
         def __str__(self):
             """ Get description """
             width = c_int()
             height = c_int()
             format = c_int()
             trax_image_get_memory_header(self.reference, byref(width), byref(height), byref(format))
-
             return "Raw image of size {}x{}, format {}".format(width.value, height.value, _image_memory_map_string[format.value])
 
         def type(self):
             return Image.MEMORY
 
 IMAGE_BUFFER_JPEG = 1
```

### Comparing `vot-trax-3.0.3/trax/message.c` & `vot-trax-4.0.0/trax/message.c`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,15 @@
 
 }
 
 void write_message(message_stream* stream, trax_logging* log, int type, const string_list* arguments, trax_properties* properties) {
 
     int i;
 
-    assert(type >= TRAX_HELLO && type <= TRAX_STATE);
+    assert(type >= TRAX_HELLO);
 
     VALIDATE_MESSAGE_STREAM(stream);
 
     switch (type) {
         case TRAX_HELLO:
             OUTPUT_STRING(TRAX_PREFIX);
             OUTPUT_STRING("hello");
@@ -749,31 +749,31 @@
         default: {
             return;
         }
     }
 
     OUTPUT_STRING(" ");
 
-    for (i = 0; i < list_size(arguments); i++) {
-        char* arg = arguments->buffer[i];
-        OUTPUT_STRING("\"");
-        OUTPUT_ESCAPED(arg);
-        OUTPUT_STRING("\" ");
+    if (arguments) {
+        for (i = 0; i < list_size(arguments); i++) {
+            char* arg = arguments->buffer[i];
+            OUTPUT_STRING("\"");
+            OUTPUT_ESCAPED(arg);
+            OUTPUT_STRING("\" ");
+        }
     }
 
-    {
+    if (properties) {
 
         file_pair pair;
         pair.stream = stream;
         pair.log = log;
 
         trax_properties_enumerate(properties, __output_properties, &pair);
 
-        OUTPUT_STRING("\n");
-
-        LOG_BUFFER(log, NULL, 0); // Flush the log stream
-
     }
 
+    OUTPUT_STRING("\n");
+    LOG_BUFFER(log, NULL, 0); // Flush the log stream
 
 }
```

### Comparing `vot-trax-3.0.3/trax/message.h` & `vot-trax-4.0.0/trax/message.h`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/region.c` & `vot-trax-4.0.0/trax/region.c`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/region.h` & `vot-trax-4.0.0/trax/region.h`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/region.py` & `vot-trax-4.0.0/trax/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from abc import abstractmethod
 from ctypes import memmove, byref, c_int, c_float, cast, c_void_p
 from functools import reduce
 import numpy as np
 import six
 
-from .internal import trax_region_bounds, trax_region_create_polygon, \
+from ._ctypes import trax_region_create_polygon, \
     trax_region_create_rectangle, trax_region_get_polygon_count, trax_region_get_polygon_point, \
     trax_region_get_special, trax_region_get_type, trax_region_get_rectangle, \
     trax_region_set_polygon_point, trax_region_create_special, trax_region_create_mask, \
     trax_region_get_mask_header, trax_region_get_mask_row, trax_region_write_mask_row
 from trax import RegionWrapper
 
 class Region(object):
```

### Comparing `vot-trax-3.0.3/trax/server.py` & `vot-trax-4.0.0/trax/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,73 +4,68 @@
 
 import traceback
 import collections
 
 from ctypes import byref, cast, py_object
 
 from . import TraxException, TraxStatus, Properties, HandleWrapper, ConsoleLogger, FileLogger
-from .internal import \
-        trax_metadata_create, trax_server_setup, \
-        trax_logger_setup, trax_image_list_p, \
-        trax_image_list_get, trax_metadata_release, \
+from . import trax_image_list_p, trax_object_list_p, wrap_image_list, wrap_object_list, wrap_objects
+
+from ._ctypes import \
+        trax_metadata_create, trax_server_setup_v, \
+        trax_logger_setup, trax_metadata_release, \
         trax_server_wait, trax_server_reply, \
-        trax_image_list_release, trax_region_p, \
-        trax_properties_p, trax_logger, trax_terminate, \
-        trax_is_alive, trax_get_error
+        trax_image_list_release,  \
+        trax_logger, trax_terminate, \
+        trax_is_alive, trax_get_error, trax_object_list_release
 from .image import ImageChannel, Image
 from .region import Region
 
-def wrap_image_list(list):
-
-    channels = [ImageChannel.COLOR, ImageChannel.DEPTH, ImageChannel.IR]
-    wrapped = {}
-
-    for channel in channels:
-        img = trax_image_list_get(list, ImageChannel.encode(channel))
-        if not img:
-            continue
-        wrapped[channel] = Image.wrap(img)
-
-    return wrapped
+class Request(collections.namedtuple('Request', ['type', 'image', 'objects', 'properties'])):
 
-class Request(collections.namedtuple('Request', ['type', 'image', 'region', 'properties'])):
-
-    """ A container class for client requests. Contains fileds type, image, region and parameters. """
+    """ A container class for client requests. Contains fileds type, image, objects and parameters. """
 
 def _logger(buf, len, obj):
 
     self = cast(obj, py_object)
 
     #self._log(string)
 
 class Server(object):
 
     """ TraX server."""
 
-    def __init__(self, region_formats, image_formats, image_channels=["color"], trackerName="", trackerDescription="", trackerFamily="", customMetadata=None, log=False):
+    def __init__(self, region_formats, image_formats, image_channels=["color"], tracker_name="", tracker_description="", tracker_family="", metadata=None, log=False, multiobject=False):
+
+        from ._ctypes import TRAX_METADATA_MULTI_OBJECT
 
         if isinstance(log, bool) and log:
             self._logger = trax_logger(ConsoleLogger())
         elif isinstance(log, str):
             self._logger = trax_logger(FileLogger(log))
         else:
-            self._logger = None
+            self._logger = trax_logger()
+
+        flags = 0
+
+        if multiobject:
+            flags |= TRAX_METADATA_MULTI_OBJECT
 
         mdata = trax_metadata_create(Region.encode_list(region_formats),
             Image.encode_list(image_formats), ImageChannel.encode_list(image_channels),
-            trackerName.encode('utf-8'), trackerDescription.encode('utf-8'), trackerFamily.encode('utf-8'))
+            tracker_name.encode('utf-8'), tracker_description.encode('utf-8'), tracker_family.encode('utf-8'), flags)
 
-        if isinstance(customMetadata, dict):
+        if isinstance(metadata, dict):
             custom = Properties(mdata.contents.custom, False)
-            for key, value in customMetadata.items():
+            for key, value in metadata.items():
                 custom.set(key, value)
 
         logger = trax_logger_setup(self._logger, None, 0)
 
-        handle = trax_server_setup(mdata, logger)
+        handle = trax_server_setup_v(mdata, logger, 0)
 
         trax_metadata_release(byref(mdata))
 
         if not handle:
             raise TraxException("Exception when setting up.")
 
         if trax_is_alive(handle) == 0:
@@ -84,51 +79,55 @@
         """ Wait for client message request. Recognize it and parse them when received .
 
             :returns: A request structure
             :rtype: trax.server.Request
         """
 
         timage = trax_image_list_p()
-        tregion = trax_region_p()
-        tproperties = trax_properties_p()
+        tobjects = trax_object_list_p()
+        properties = Properties()
 
-        status = TraxStatus.decode(trax_server_wait(self._handle.reference, byref(timage), byref(tregion), tproperties))
+        status = TraxStatus.decode(trax_server_wait(self._handle.reference, byref(timage), byref(tobjects), properties.reference))
 
         if status == TraxStatus.QUIT:
-            properties = Properties(tproperties)
             return Request(status, None, None, properties)
 
         if status == TraxStatus.INITIALIZE:
             image = wrap_image_list(timage)
+            objects = wrap_object_list(tobjects)
             trax_image_list_release(byref(timage))
-            region = Region.wrap(tregion)
-            properties = Properties(tproperties)
-            return Request(status, image, region, properties)
+            trax_object_list_release(byref(tobjects))
+            return Request(status, image, objects, properties)
 
         if status == TraxStatus.FRAME:
             image = wrap_image_list(timage)
             trax_image_list_release(byref(timage))
-            properties = Properties(tproperties)
-            return Request(status, image, None, properties)
+            if tobjects:
+                objects = wrap_object_list(tobjects)
+                trax_object_list_release(byref(tobjects))
+            else:
+                objects = None
+            return Request(status, image, objects, properties)
 
         else:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when waiting for command: {}".format(message))
 
-    def status(self, region, properties=None):
+    def status(self, objects, properties=None):
         """ Reply to client with a status region and optional properties.
 
 
-            :param trax.region.Region region: Resulting region object.
+            :param List[Region, Mapping] objects: Resulting status of tracked objects.
             :param dict properties: Optional arguments as a dictionary.
         """
-        assert(isinstance(region, Region))
+        assert(isinstance(objects, list))
         tproperties = Properties(properties)
-        status = TraxStatus.decode(trax_server_reply(self._handle.reference, cast(region.reference, trax_region_p), tproperties.reference))
+        tobjects = wrap_objects(objects)
+        status = TraxStatus.decode(trax_server_reply(self._handle.reference, tobjects.reference, tproperties.reference))
 
         if status == TraxStatus.ERROR:
             message = trax_get_error(self._handle.reference)
             message = message.decode('utf-8') if not message is None else "Unknown"
             raise TraxException("Exception when sending status: {}".format(message))
 
         return True
```

### Comparing `vot-trax-3.0.3/trax/strmap.c` & `vot-trax-4.0.0/trax/strmap.c`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/strmap.h` & `vot-trax-4.0.0/trax/strmap.h`

 * *Files identical despite different names*

### Comparing `vot-trax-3.0.3/trax/trax.c` & `vot-trax-4.0.0/trax/trax.c`

 * *Files 21% similar despite different names*

```diff
@@ -15,23 +15,30 @@
 #include "base64.h"
 #include "debug.h"
 
 #define VALIDATE_HANDLE(H) assert(((H)->flags & TRAX_FLAG_VALID))
 #define VALIDATE_SERVER_HANDLE(H) assert(((H)->flags & TRAX_FLAG_VALID) && ((H)->flags & TRAX_FLAG_SERVER))
 #define VALIDATE_CLIENT_HANDLE(H) assert(((H)->flags & TRAX_FLAG_VALID) && !((H)->flags & TRAX_FLAG_SERVER))
 
+#define IS_MULTI_OBJECT(H) (((H)->metadata->flags & TRAX_METADATA_MULTI_OBJECT))
+
+#define IS_VERSION_2(H) (((H)->version >= 2))
+#define IS_VERSION_3(H) (((H)->version >= 3))
+#define IS_VERSION_4(H) (((H)->version >= 4))
+
 #define HANDLE_ALIVE(H) (((H)->flags & TRAX_FLAG_VALID) && !((H)->flags & TRAX_FLAG_TERMINATED))
 
 #define LOGGER(H) (((H)->logging))
 
 #define BUFFER_LENGTH 64
 #define MAX_URI_SCHEME 16
 
 #define COPY_ALL 1
 #define COPY_EXTERNAL 0
+#define COPY_OVERWRITE 2
 
 #define REGION(VP) ((region_container*) (VP))
 
 #define REGION_TYPE(VP) ( \
     (((region_container*) (VP))->type == RECTANGLE) ? TRAX_REGION_RECTANGLE : \
     (((region_container*) (VP))->type == POLYGON) ? TRAX_REGION_POLYGON : \
     (((region_container*) (VP))->type == MASK) ? TRAX_REGION_MASK : \
@@ -206,31 +213,38 @@
 
     }
 
     return NULL;
 
 }
 
-void copy_property_all(const char *key, const char *value, const void *obj) {
-
+void copy_property_overwrite(const char *key, const char *value, const void *obj) {
     trax_properties* dest = (trax_properties*) obj;
     trax_properties_set(dest, key, value);
-
 }
 
-void copy_property_external(const char *key, const char *value, const void *obj) {
-
+void copy_property_safe(const char *key, const char *value, const void *obj) {
     trax_properties* dest = (trax_properties*) obj;
+    if (trax_properties_has(dest, key)) return;
+    trax_properties_set(dest, key, value);
+}
 
+void copy_property_external_overwrite(const char *key, const char *value, const void *obj) {
+    trax_properties* dest = (trax_properties*) obj;
     if (strncmp(key, "trax.", 5) == 0) return;
-
     trax_properties_set(dest, key, value);
+}
 
+void copy_property_external_safe(const char *key, const char *value, const void *obj) {
+    trax_properties* dest = (trax_properties*) obj;
+    if (trax_properties_has(dest, key) || strncmp(key, "trax.", 5) == 0) return;
+    trax_properties_set(dest, key, value);
 }
 
+
 char* image_encode(trax_image* image) {
 
     char* result = NULL;
 
     switch (image->type) {
     case TRAX_IMAGE_PATH: {
         int length = strlen(image->data);
@@ -441,14 +455,29 @@
     }
     if (TRAX_SUPPORTS(formats, TRAX_REGION_MASK)) {
         pch += sprintf(pch, "mask;");
     }
 
 }
 
+trax_region* region_autoconvert(trax_region* region, int supported) {
+
+    trax_region* converted = NULL;
+
+    if TRAX_SUPPORTS(supported, TRAX_REGION_MASK)
+        converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_MASK));
+    else if TRAX_SUPPORTS(supported, TRAX_REGION_POLYGON)
+        converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_POLYGON));
+    else if TRAX_SUPPORTS(supported, TRAX_REGION_RECTANGLE)
+        converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_RECTANGLE));
+
+    return converted;
+
+}
+
 int channels_decode(char *str) {
 
     int channels = 0;
 
     char *pch;
     pch = strtok (str, " ;");
     while (pch != NULL) {
@@ -484,17 +513,21 @@
     }
     if (TRAX_SUPPORTS(channels, TRAX_CHANNEL_IR)) {
         pch += sprintf(pch, "ir;");
     }
 
 }
 
-void copy_properties(const trax_properties* source, trax_properties* dest, int internal) {
+void copy_properties(const trax_properties* source, trax_properties* dest, int flags) {
 
-    trax_properties_enumerate(source, (internal) ? copy_property_all : copy_property_external, dest);
+    trax_enumerator f = (flags & COPY_ALL) ?
+     ((flags && COPY_OVERWRITE) ? copy_property_overwrite : copy_property_safe) :
+     ((flags && COPY_OVERWRITE) ? copy_property_external_overwrite : copy_property_external_safe);
+    
+    trax_properties_enumerate(source, f, dest);
 
 }
 
 void clear_error(trax_handle* handle) {
 
     if (handle->error) {
         free(handle->error);
@@ -525,25 +558,25 @@
 }
 
 
 trax_handle* client_setup(message_stream* stream, const trax_logging log) {
 
     trax_properties* tmp_properties;
     string_list* arguments;
-    int version = 1;
     char *tmp, *tracker_name, *tracker_description, *tracker_family;
-    int region_formats, image_formats, channels;
+    int region_formats, image_formats, channels, flags;
 
     trax_handle* client = (trax_handle*) malloc(sizeof(trax_handle));
 
     client->flags = (0 & ~TRAX_FLAG_SERVER) | TRAX_FLAG_VALID;
 
     client->logging = log;
     client->stream = stream;
     client->error = NULL;
+    client->objects = 0;
 
     tmp_properties = trax_properties_create();
     arguments = list_create(8);
 
     if (read_message((message_stream*)client->stream, &LOGGER(client), arguments, tmp_properties) != TRAX_HELLO) {
         DEBUGMSG("Unable to parse hello message.");
         goto failure;
@@ -560,38 +593,44 @@
     region_formats = region_formats_decode(tmp);
     free(tmp);
 
     tmp = trax_properties_get(tmp_properties, "trax.image");
     image_formats = image_formats_decode(tmp);
     free(tmp);
 
-    // Multiple channels are only supported in TraX version 2
+    // Multiple channels are only supported in TraX protocol version 2
     if (client->version < 2) {
         channels = TRAX_CHANNEL_COLOR;
     } else {
         tmp = trax_properties_get(tmp_properties, "trax.channels");
         channels = channels_decode(tmp);
         free(tmp);
         if (channels == 0)
             channels = TRAX_CHANNEL_COLOR;
     }
 
     tracker_name = trax_properties_get(tmp_properties, "trax.name");
     tracker_description = trax_properties_get(tmp_properties, "trax.description");
     tracker_family = trax_properties_get(tmp_properties, "trax.family");
 
-    client->metadata = trax_metadata_create(region_formats, image_formats, channels,
-                                            tracker_name, tracker_description, tracker_family);
+    flags = 0;
+    if (client->version > 3) {
+        if (trax_properties_get_int(tmp_properties, "trax.multiobject", 0)) {
+            flags |= TRAX_METADATA_MULTI_OBJECT;
+        }
+    }
 
+    client->metadata = trax_metadata_create(region_formats, image_formats, channels,
+                                            tracker_name, tracker_description, tracker_family, flags);
 
     if (tracker_name) free(tracker_name);
     if (tracker_description) free(tracker_description);
     if (tracker_family) free(tracker_family);
 
-    copy_properties(tmp_properties, client->metadata->custom, COPY_EXTERNAL);
+    copy_properties(tmp_properties, client->metadata->custom, COPY_EXTERNAL | COPY_OVERWRITE);
 
     trax_properties_release(&tmp_properties);
     list_destroy(&arguments);
 
     return client;
 
 failure:
@@ -599,34 +638,39 @@
     list_destroy(&arguments);
     trax_properties_release(&tmp_properties);
     free(client);
     return NULL;
 
 }
 
-trax_handle* server_setup(trax_metadata *metadata, message_stream* stream, const trax_logging log) {
+trax_handle* server_setup(trax_metadata *metadata, message_stream* stream, const trax_logging log, int version) {
 
     trax_properties* properties;
     trax_handle* server = (trax_handle*) malloc(sizeof(trax_handle));
     string_list* arguments;
+    int flags;
     char tmp[BUFFER_LENGTH];
 
     server->flags = (TRAX_FLAG_SERVER) | TRAX_FLAG_VALID;
     server->logging = log;
     server->error = NULL;
     server->stream = stream;
+    server->objects = 0;
 
     if (metadata->custom) {
         properties = trax_properties_copy(metadata->custom);
     } else {
         properties = trax_properties_create();
     }
     
-    server->version = TRAX_VERSION;
-    trax_properties_set_int(properties, "trax.version", TRAX_VERSION);
+    assert(version <= TRAX_VERSION);
+    if (version < 1) version = TRAX_VERSION;
+
+    server->version = version;
+    trax_properties_set_int(properties, "trax.version", server->version);
 
     region_formats_encode(metadata->format_region, tmp);
     trax_properties_set(properties, "trax.region", tmp);
 
     image_formats_encode(metadata->format_image, tmp);
     trax_properties_set(properties, "trax.image", tmp);
 
@@ -638,32 +682,39 @@
 
     if (metadata->tracker_description)
         trax_properties_set(properties, "trax.description", metadata->tracker_description);
 
     if (metadata->tracker_family)
         trax_properties_set(properties, "trax.family", metadata->tracker_family);
 
+    if (IS_VERSION_4(server)) {
+        flags = 0;
+        if (metadata->flags & TRAX_METADATA_MULTI_OBJECT) {
+            flags |= TRAX_METADATA_MULTI_OBJECT;
+            trax_properties_set_int(properties, "trax.multiobject", 1);
+        }
+    }
 
     server->metadata = trax_metadata_create(metadata->format_region, metadata->format_image, metadata->channels,
-                                            metadata->tracker_name, metadata->tracker_description, metadata->tracker_family);
+                                            metadata->tracker_name, metadata->tracker_description, metadata->tracker_family, flags);
 
     arguments = list_create(1);
 
     write_message((message_stream*)server->stream, &LOGGER(server), TRAX_HELLO, arguments, properties);
 
     trax_properties_release(&properties);
 
     list_destroy(&arguments);
 
     return server;
 
 }
 
 trax_metadata* trax_metadata_create(int region_formats, int image_formats, int channels,
-                                    const char* tracker_name, const char* tracker_description, const char* tracker_family) {
+                                    const char* tracker_name, const char* tracker_description, const char* tracker_family, int flags) {
 
     assert(channels != 0);
 
     trax_metadata* metadata = (trax_metadata*) malloc(sizeof(trax_metadata));
 
     metadata->format_region = region_formats;
     metadata->format_image = image_formats;
@@ -671,14 +722,16 @@
 
     metadata->tracker_name = (tracker_name) ? strdup(tracker_name) : NULL;
     metadata->tracker_description = (tracker_description) ? strdup(tracker_description) : NULL;
     metadata->tracker_family = (tracker_family) ? strdup(tracker_family) : NULL;
 
     metadata->custom = trax_properties_create();
 
+    metadata->flags = flags;
+
     return metadata;
 
 }
 
 void trax_metadata_release(trax_metadata** metadata) {
 
     if (!*metadata) return;
@@ -710,97 +763,141 @@
 
     if (!stream) return NULL;
 
     return client_setup(stream, log);
 
 }
 
-int trax_client_wait(trax_handle* client, trax_region** region, trax_properties* properties) {
+int trax_client_wait(trax_handle* client, trax_object_list** objects, trax_properties* properties) {
 
     trax_properties* tmp_properties;
     string_list* arguments;
     int result = TRAX_ERROR;
 
-    (*region) = NULL;
+    (*objects) = NULL;
 
     VALIDATE_CLIENT_HANDLE(client);
 
-    if (!HANDLE_ALIVE(client))
+    if (!HANDLE_ALIVE(client)) {
+        set_error(client, "Tracker not alive");
         return TRAX_ERROR;
+    }
 
-    tmp_properties = trax_properties_create();
-    arguments = list_create(8);
-
-    result = read_message((message_stream*)client->stream, &LOGGER(client), arguments, tmp_properties);
-
-    if (result == TRAX_STATE) {
+    (*objects) = trax_object_list_create(client->objects);
 
-        region_container *_region = NULL;
+    for (int i = 0; i < client->objects; i++) {
 
-        if (list_size(arguments) != 1)
-            goto failure;
+        tmp_properties = trax_properties_create();
+        arguments = list_create(8);
+        result = read_message((message_stream*)client->stream, &LOGGER(client), arguments, tmp_properties);
 
-        result = TRAX_STATE;
+        if (result == TRAX_STATE) {
 
-        if (!region_parse(arguments->buffer[0], &_region)) {
-            goto failure;
-        }
+            region_container *_region = NULL;
 
-        (*region) = _region;
+            if (list_size(arguments) != 1) {
+                list_destroy(&arguments);
+                trax_properties_release(&tmp_properties);
+                trax_object_list_release(objects);
+                result = TRAX_ERROR;
+                break;
+            }
+            
+            if (!region_parse(arguments->buffer[0], &_region)) {
+                list_destroy(&arguments);
+                trax_properties_release(&tmp_properties);
+                trax_object_list_release(objects);
+                result = TRAX_ERROR;
+                break;
+            }
 
-        copy_properties(tmp_properties, properties, 1);
+            trax_object_list_set((*objects), i, _region);
+            copy_properties(tmp_properties, trax_object_list_properties((*objects), i), COPY_ALL | COPY_OVERWRITE);
 
-        goto end;
+        } else if (result == TRAX_QUIT) {
 
-    } else if (result == TRAX_QUIT) {
+            if (list_size(arguments) != 0) {
+                list_destroy(&arguments);
+                trax_properties_release(&tmp_properties);
+                trax_object_list_release(objects);
+                result = TRAX_ERROR;
+                break;
+            }
+    
+            if (properties)
+                copy_properties(tmp_properties, properties, COPY_ALL | COPY_OVERWRITE);
 
-        if (list_size(arguments) != 0)
-            goto failure;
+            client->flags |= TRAX_FLAG_TERMINATED;
 
-        if (properties)
-            copy_properties(tmp_properties, properties, 1);
+            list_destroy(&arguments);
+            trax_properties_release(&tmp_properties);
+            trax_object_list_release(objects);
+            break;
+        } else if (result == TRAX_ERROR) {
+            list_destroy(&arguments);
+            trax_properties_release(&tmp_properties);
+            trax_object_list_release(objects);
+            break;
+        }
 
-        client->flags |= TRAX_FLAG_TERMINATED;
+        list_destroy(&arguments);
+        trax_properties_release(&tmp_properties);
 
-        goto end;
     }
 
-failure:
-    result = TRAX_ERROR;
-
-end:
-
-    list_destroy(&arguments);
-    trax_properties_release(&tmp_properties);
-
     return result;
 
 }
 
-int trax_client_initialize(trax_handle* client, trax_image_list* images, trax_region* region, trax_properties* properties) {
+int trax_client_initialize(trax_handle* client, trax_image_list* images, trax_object_list* objects, trax_properties* properties) {
 
     char* data = NULL;
-    region_container* _region;
+    trax_region* region;
     string_list* arguments;
-    int i;
+    int i, n;
 
     VALIDATE_CLIENT_HANDLE(client);
 
     clear_error(client);
 
     if (!HANDLE_ALIVE(client)) {
         set_error(client, "Client not alive");
         return TRAX_ERROR;
     }
 
-    assert(images && region);
+    assert(images && objects);
 
-    _region = REGION(region);
+    n = trax_object_list_count(objects);
 
-    assert(_region->type != SPECIAL);
+    if (n < 1) {
+        set_error(client, "At least one object required");
+        return TRAX_ERROR;
+    }
+
+    if (!IS_MULTI_OBJECT(client) && n > 1) {
+        set_error(client, "Too many objects given");
+        return TRAX_ERROR;
+    }
+
+    if (IS_VERSION_4(client)) {
+        if (client->objects > 0) {
+            // Reset object count with an empty initialize message
+            write_message((message_stream*)client->stream, &LOGGER(client), TRAX_INITIALIZE, NULL, NULL);
+            client->objects = 0;
+        }
+        return trax_client_frame(client, images, objects, properties);
+    }
+
+    // Legacy single target mode from now on.
+
+    region = trax_object_list_get(objects, 0);
+
+    assert(REGION_TYPE(region) != SPECIAL);
+
+    // TODO: verify server version?
 
     arguments = list_create(1);
 
     for (i = 0; i < TRAX_CHANNELS; i++) {
         if (TRAX_SUPPORTS(client->metadata->channels, TRAX_CHANNEL_ID(i))) {
 
             if (!images->images[i]) {
@@ -811,22 +908,15 @@
             list_append_direct(arguments, buffer);
 
         }
     }
 
     if (!TRAX_SUPPORTS(client->metadata->format_region, REGION_TYPE(region))) {
 
-        trax_region* converted = NULL;
-
-        if TRAX_SUPPORTS(client->metadata->format_region, TRAX_REGION_MASK)
-            converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_MASK));
-        else if TRAX_SUPPORTS(client->metadata->format_region, TRAX_REGION_POLYGON)
-            converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_POLYGON));
-        else if TRAX_SUPPORTS(client->metadata->format_region, TRAX_REGION_RECTANGLE)
-            converted = region_convert((region_container *)region, REGION_TYPE_BACK(TRAX_REGION_RECTANGLE));
+        trax_region* converted = region_autoconvert(region, client->metadata->format_region);
 
         assert(converted);
 
         data = region_string((region_container *)converted);
 
         trax_region_release(&converted);
 
@@ -837,65 +927,112 @@
         free(data);
     }
 
     write_message((message_stream*)client->stream, &LOGGER(client), TRAX_INITIALIZE, arguments, properties);
 
     list_destroy(&arguments);
 
+    client->objects = 1;
+
     return TRAX_OK;
 
 failure:
 
     list_destroy(&arguments);
 
     return TRAX_ERROR;
 
 }
 
-int trax_client_frame(trax_handle* client, trax_image_list* images, trax_properties* properties) {
+int trax_client_frame(trax_handle* client, trax_image_list* images, trax_object_list* objects, trax_properties* properties) {
 
     int i;
-    string_list* arguments;
     VALIDATE_CLIENT_HANDLE(client);
 
     clear_error(client);
 
     if (!HANDLE_ALIVE(client)) {
         set_error(client, "Client not alive");
         return TRAX_ERROR;
     }
 
-    arguments = list_create(1);
+    if (IS_VERSION_4(client)) {
 
-    for (i = 0; i < TRAX_CHANNELS; i++) {
-        if (TRAX_SUPPORTS(client->metadata->channels, TRAX_CHANNEL_ID(i))) {
-            if (!images->images[i]) {
-                set_error(client, "Required image channel not provided (ID: %d)", TRAX_CHANNEL_ID(i));
-                goto failure;
+        int n = (objects) ? trax_object_list_count(objects) : 0;
+
+        if (client->objects + n > 1 && !IS_MULTI_OBJECT(client)) {
+            set_error(client, "Invalid mode");
+            return TRAX_ERROR;
+        }
+
+        for (i = 0; i < n; i++) {
+            char* data = NULL;
+            string_list* arguments;
+            trax_region* region = trax_object_list_get(objects, i);
+
+            arguments = list_create(1);
+
+            if (!TRAX_SUPPORTS(client->metadata->format_region, REGION_TYPE(region))) {
+
+                    trax_region* converted = region_autoconvert(region, client->metadata->format_region);
+                    assert(converted);
+                    data = region_string((region_container *)converted);
+                    trax_region_release(&converted);
+
+            } else data = region_string((region_container *)region);
+
+            if (data) {
+                list_append(arguments, data);
+                free(data);
             }
-            char* buffer = image_encode(images->images[i]);
-            list_append_direct(arguments, buffer);
-        } 
-    }
 
-    write_message((message_stream*)client->stream, &LOGGER(client), TRAX_FRAME, arguments, properties);
+            write_message((message_stream*)client->stream, &LOGGER(client), TRAX_INITIALIZE, arguments, trax_object_list_properties(objects, i));
 
-    list_destroy(&arguments);
+            list_destroy(&arguments);
 
-    return TRAX_OK;
+        }
+        
+        client->objects += n;
+        
+    } else {
 
-failure:
+        int n = (objects) ? trax_object_list_count(objects) : 0;
 
-    list_destroy(&arguments);
+        if (n > 0) {
+            set_error(client, "Unable to add new objects");
+            return TRAX_ERROR;
+        }
 
-    return TRAX_ERROR;
+    }
+
+    {
+        string_list* arguments;
+        arguments = list_create(1);
+
+        for (i = 0; i < TRAX_CHANNELS; i++) {
+            if (TRAX_SUPPORTS(client->metadata->channels, TRAX_CHANNEL_ID(i))) {
+                if (!images->images[i]) {
+                    set_error(client, "Required image channel not provided (ID: %d)", TRAX_CHANNEL_ID(i));
+                    list_destroy(&arguments);
+                    return TRAX_ERROR;
+                }
+                char* buffer = image_encode(images->images[i]);
+                list_append_direct(arguments, buffer);
+            } 
+        }
+
+        write_message((message_stream*)client->stream, &LOGGER(client), TRAX_FRAME, arguments, properties);
+        list_destroy(&arguments);
+
+        return TRAX_OK;
+    }
 
 }
 
-trax_handle* trax_server_setup(trax_metadata *metadata, const trax_logging log) {
+trax_handle* trax_server_setup_v(trax_metadata *metadata, const trax_logging log, int version) {
 
     message_stream* stream;
 
     char* env_socket = getenv("TRAX_SOCKET");
 
     if (env_socket) {
 
@@ -917,26 +1054,26 @@
         if (env_out) fout = get_shared_fd(atoi(env_out), 0);
 #endif
 
         stream = create_message_stream_file(fin, fout);
 
     }
 
-    return server_setup(metadata, stream, log);
+    return server_setup(metadata, stream, log, version);
 
 }
 
-trax_handle* trax_server_setup_file(trax_metadata *metadata, int input, int output, const trax_logging log) {
+trax_handle* trax_server_setup_file_v(trax_metadata *metadata, int input, int output, const trax_logging log, int version) {
 
     message_stream* stream = create_message_stream_file(input, output);
 
-    return server_setup(metadata, stream, log);
+    return server_setup(metadata, stream, log, version);
 }
 
-int trax_server_wait(trax_handle* server, trax_image_list** images, trax_region** region, trax_properties* properties) {
+int trax_server_wait_sot(trax_handle* server, trax_image_list** images, trax_region** region, trax_properties* properties) {
 
     int result = TRAX_ERROR;
     int i, j = 0;
     string_list* arguments;
     trax_properties* tmp_properties;
 
     VALIDATE_SERVER_HANDLE(server);
@@ -944,14 +1081,19 @@
     clear_error(server);
 
     if (!HANDLE_ALIVE(server)) {
         set_error(server, "Server not alive");
         return TRAX_ERROR;
     }
 
+    if (IS_VERSION_4(server)) {
+        set_error(server, "Invalid mode");
+        return TRAX_ERROR;
+    }
+
     int argument_count = trax_image_list_count(server->metadata->channels);
 
     tmp_properties = trax_properties_create();
     arguments = list_create(8);
 
     result = read_message((message_stream*)server->stream, &LOGGER(server), arguments, tmp_properties);
 
@@ -974,26 +1116,26 @@
                 j++;
 
             }
 
         }
 
         if (properties)
-            copy_properties(tmp_properties, properties, COPY_ALL);
+            copy_properties(tmp_properties, properties, COPY_ALL | COPY_OVERWRITE);
         goto end;
 
     } else if (result == TRAX_QUIT) {
 
         if (list_size(arguments) != 0){
             set_error(server, "Protocol error, illegal argument number %d != %d", list_size(arguments), 0);
             goto failure;
         }   
 
         if (properties)
-            copy_properties(tmp_properties, properties, COPY_ALL);
+            copy_properties(tmp_properties, properties, COPY_ALL | COPY_OVERWRITE);
 
         server->flags |= TRAX_FLAG_TERMINATED;
 
         goto end;
 
     } else if (result == TRAX_INITIALIZE) {
 
@@ -1018,15 +1160,17 @@
         }
 
         if (!region_parse(arguments->buffer[j], (region_container**)region)) {
             goto failure;
         }
 
         if (properties)
-            copy_properties(tmp_properties, properties, COPY_ALL);
+            copy_properties(tmp_properties, properties, COPY_ALL | COPY_OVERWRITE);
+
+        server->objects = 1;
 
         goto end;
     }
 
 failure:
 
     result = TRAX_ERROR;
@@ -1045,28 +1189,192 @@
 
     list_destroy(&arguments);
     trax_properties_release(&tmp_properties);
 
     return result;
 }
 
-int trax_server_reply(trax_handle* server, trax_region* region, trax_properties* properties) {
+int trax_server_wait_mot(trax_handle* server, trax_image_list** images, trax_object_list** objects, trax_properties* properties) {
+
+    int result = TRAX_ERROR;
+    int i, j = 0;
+    string_list* arguments;
+    trax_properties* tmp_properties;
+    int object_capacity = 1;
+    int object_count = 0;
+    trax_region** object_regions = (trax_region**) malloc(sizeof(trax_region*) * object_capacity);
+    trax_properties** object_properties = (trax_properties**) malloc(sizeof(trax_properties*) * object_capacity);
+
+    VALIDATE_SERVER_HANDLE(server);
+
+    clear_error(server);
+
+    *objects = NULL;
+
+    if (!HANDLE_ALIVE(server)) {
+        set_error(server, "Server not alive");
+        return TRAX_ERROR;
+    }
+
+    int argument_count = trax_image_list_count(server->metadata->channels);
+
+    while (1) {
+        tmp_properties = trax_properties_create();
+        arguments = list_create(8);
+
+        int code = read_message((message_stream*)server->stream, &LOGGER(server), arguments, tmp_properties);
+
+        if (code == TRAX_ERROR) {
+            goto failure;
+        }
+
+        if (code == TRAX_QUIT) {
+
+            if (list_size(arguments) != 0){
+                set_error(server, "Protocol error, illegal argument number %d != %d", list_size(arguments), 0);
+                goto failure;
+            }   
+
+            if (properties)
+                copy_properties(tmp_properties, properties, COPY_EXTERNAL | COPY_OVERWRITE);
+
+            result = TRAX_QUIT;
+            server->flags |= TRAX_FLAG_TERMINATED;
+            goto end;
+        }
+
+        if (code == TRAX_FRAME) {
+
+            if (result == TRAX_INITIALIZE && object_count == 0) {
+                set_error(server, "No object was given to track");
+                goto failure;
+            }
+
+            if (result != TRAX_INITIALIZE || server->objects > 0) result = TRAX_FRAME;
+
+            if (list_size(arguments) != argument_count) {
+                set_error(server, "Protocol error, illegal argument number %d != %d", list_size(arguments), argument_count);
+                goto failure;
+            }   
+                
+            *images = trax_image_list_create();
+
+            for (i = 0; i < TRAX_CHANNELS; i++) {
+
+                if (TRAX_SUPPORTS(server->metadata->channels, TRAX_CHANNEL_ID(i))) {
+
+                    (*images)->images[i] = image_decode(arguments->buffer[j]);
+                    if (!(*images)->images[i] || !TRAX_SUPPORTS(server->metadata->format_image, (*images)->images[i]->type))
+                        goto failure;
+                    j++;
+
+                }
+
+            }
+
+            if (properties)
+                copy_properties(tmp_properties, properties, COPY_ALL | COPY_OVERWRITE);
+            goto end;
+        }
+
+        if (code == TRAX_INITIALIZE) {
+
+            if (list_size(arguments) == 0) {
+                result = TRAX_INITIALIZE;
+                server->objects = 0;
+                continue;
+            }
+
+            if (list_size(arguments) != 1) { // There's also the region info
+                set_error(server, "Protocol error, illegal argument number %d != %d", list_size(arguments), 1);
+                goto failure;
+            }
+
+            object_count++;
+
+            if (object_count > object_capacity) {
+                object_capacity += 10;
+                object_regions = (trax_region**) realloc(object_regions, sizeof(trax_region*) * object_capacity);
+                object_properties = (trax_properties**) realloc(object_properties, sizeof(trax_properties*) * object_capacity);
+            }
+
+            if (!region_parse(arguments->buffer[0], (region_container**)(&object_regions[object_count-1]))) {
+                object_count--;
+                goto failure;
+            }
+
+            object_properties[object_count-1] = trax_properties_create();
+            copy_properties(tmp_properties, object_properties[object_count-1], COPY_ALL | COPY_OVERWRITE);
+
+            result = TRAX_INITIALIZE;
+        }
+
+        list_destroy(&arguments);
+        trax_properties_release(&tmp_properties);
+
+    }
+
+failure:
+
+    result = TRAX_ERROR;
+
+    if (*images) {
+        for (i = 0; i < TRAX_CHANNELS; i++) {
+            if ((*images)->images[i]) trax_image_release(&(*images)->images[i]);
+        }
+        trax_image_list_release(images);
+    }
+
+    for (i = 0; i < object_count; i++) {
+        trax_region_release(&(object_regions[i]));
+        trax_properties_release(&(object_properties[i]));
+    }
+    object_count = 0;
+
+end:
+
+    if (object_count) {
+        *objects = trax_object_list_create(object_count);
+        for (i = 0; i < object_count; i++) {
+            trax_object_list_set(*objects, i, object_regions[i]);
+            copy_properties(object_properties[i], trax_object_list_properties(*objects, i), COPY_ALL | COPY_OVERWRITE);
+            trax_region_release(&(object_regions[i]));
+            trax_properties_release(&(object_properties[i]));
+        }
+        server->objects += object_count;
+    } 
+
+    if (arguments) list_destroy(&arguments);
+    if (tmp_properties) trax_properties_release(&tmp_properties);
+
+    free(object_regions);
+    free(object_properties);
+
+    return result;
+}
+
+int trax_server_reply_sot(trax_handle* server, trax_region* region, trax_properties* properties) {
 
     char* data;
     string_list* arguments;
 
     VALIDATE_SERVER_HANDLE(server);
 
     clear_error(server);
 
     if (!HANDLE_ALIVE(server)) {
         set_error(server, "Server not alive");
         return TRAX_ERROR;
     }
 
+    if (IS_VERSION_4(server)) {
+        set_error(server, "Invalid mode");
+        return TRAX_ERROR;
+    }
+
     data = region_string(REGION(region));
 
     if (!data) return TRAX_ERROR;
 
     arguments = list_create(1);
 
     list_append_direct(arguments, data);
@@ -1075,14 +1383,56 @@
 
     list_destroy(&arguments);
 
     return TRAX_OK;
 
 }
 
+int trax_server_reply_mot(trax_handle* server, trax_object_list* objects) {
+
+    int n, i;
+    char* data;
+    string_list* arguments;
+
+    VALIDATE_SERVER_HANDLE(server);
+
+    clear_error(server);
+
+    if (!HANDLE_ALIVE(server)) {
+        set_error(server, "Server not alive");
+        return TRAX_ERROR;
+    }
+
+    assert(objects);
+
+    n = trax_object_list_count(objects);
+
+    if (!IS_MULTI_OBJECT(server) && n != 1) {
+        set_error(server, "Invalid mode");
+        return TRAX_ERROR;
+    }
+
+    if (n != server->objects) {
+        set_error(server, "Invalid object count");
+        return TRAX_ERROR;
+    }
+
+    for (i = 0; i < n; i++) {
+        data = region_string(REGION(trax_object_list_get(objects, i)));
+        if (!data) return TRAX_ERROR;
+        arguments = list_create(1);
+        list_append_direct(arguments, data);
+        write_message((message_stream*)server->stream, &LOGGER(server), TRAX_STATE, arguments, trax_object_list_properties(objects, i));
+        list_destroy(&arguments);
+    }
+
+    return TRAX_OK;
+}
+
+
 const char* trax_get_error(trax_handle* handle) {
 
     VALIDATE_HANDLE(handle);
 
     return handle->error;
 
 }
@@ -1160,18 +1510,21 @@
         return TRAX_ERROR;
 
     switch (id) {
     case TRAX_PARAMETER_VERSION:
         *value = handle->version;
         return 1;
     case TRAX_PARAMETER_CLIENT:
-        *value = !(handle->flags & TRAX_FLAG_SERVER);
+        *value = (!(handle->flags & TRAX_FLAG_SERVER)) ? 1 : 0;
         return 1;
     case TRAX_PARAMETER_SOCKET:
-        *value = (((message_stream*)handle->stream)->flags & TRAX_STREAM_SOCKET);
+        *value = ((((message_stream*)handle->stream)->flags & TRAX_STREAM_SOCKET)) ? 1 : 0;
+        return 1;
+    case TRAX_PARAMETER_MULTIOBJECT:
+        *value = ((handle->metadata->flags) & TRAX_METADATA_MULTI_OBJECT) ? 1 : 0;
         return 1;
     }
 
     return 0;
 }
 
 void trax_image_release(trax_image** image) {
@@ -1587,14 +1940,23 @@
 
     copy_properties(original, prop, COPY_ALL);
 
     return prop;
 
 }
 
+void trax_properties_append(const trax_properties* source, trax_properties* drain, int overwrite) {
+
+    int flags = COPY_ALL;
+    if (overwrite) flags |= COPY_OVERWRITE;
+
+    copy_properties(source, drain, flags);
+
+}
+
 void trax_properties_set(trax_properties* properties, const char* key, const char* value) {
 
     sm_put(properties->map, key, value);
 
 }
 
 void trax_properties_set_int(trax_properties* properties, const char* key, int value) {
@@ -1623,14 +1985,19 @@
     value = (char *) malloc(sizeof(trax_properties) * size);
 
     sm_get(properties->map, key, value, size);
 
     return value;
 }
 
+int trax_properties_has(const trax_properties* properties, const char* key) {
+    int size = sm_get(properties->map, key, NULL, 0);
+    return (size < 1)? 0 : 1;
+}
+
 int trax_properties_get_int(const trax_properties* properties, const char* key, int def) {
 
     char* end;
     long ret;
     char* value = trax_properties_get(properties, key);
 
     if (value == NULL) return def;
@@ -1673,14 +2040,100 @@
 void trax_properties_enumerate(const trax_properties* properties, trax_enumerator enumerator, const void* object) {
     if (properties && enumerator) {
 
         sm_enum(properties->map, enumerator, object);
     }
 }
 
+
+trax_object_list* trax_object_list_create(int count) {
+
+    int i;
+
+    trax_object_list* list = (trax_object_list*)malloc(sizeof(trax_object_list));
+
+    list->size = count;
+
+    list->regions = (trax_region**) malloc(sizeof(trax_region*) * count);
+    list->properties = (trax_properties**) malloc(sizeof(trax_properties*) * count);
+
+    for (i = 0; i < count; i++) {
+        list->regions[i] = trax_region_create_special(0);
+        list->properties[i] = trax_properties_create();
+    }
+
+    return list;
+}
+
+
+void trax_object_list_release(trax_object_list** list) {
+
+    if (list && *list) {
+        int i;
+        for (i = 0; i < (*list)->size; i++) {
+            trax_region_release(&((*list)->regions[i]));
+            trax_properties_release(&((*list)->properties[i]));
+        }
+        free((*list)->regions);
+        free((*list)->properties);
+        free((*list));
+        *list = 0;
+    }
+}
+
+
+void trax_object_list_set(trax_object_list* list, int index, trax_region* region) {
+
+    if (index < 0 || index >= list->size) return;
+
+    trax_region_release(&(list->regions[index]));
+
+    list->regions[index] = trax_region_clone(region);
+
+}
+
+
+trax_region* trax_object_list_get(trax_object_list* list, int index) {
+
+    if (index < 0 || index >= list->size) return 0;
+    return list->regions[index];
+
+}
+
+trax_properties* trax_object_list_properties(trax_object_list* list, int index) {
+    if (index < 0 || index >= list->size) return 0;
+    return list->properties[index];
+}
+
+int trax_object_list_count(const trax_object_list* list) {
+    return list->size;
+}
+
+int trax_object_list_append(trax_object_list* list, const trax_object_list* src) {
+
+    int i, o;
+
+    assert(list && src);
+
+    o = list->size;
+    list->size += src->size;
+
+    list->regions = (trax_region**) realloc(list->regions, sizeof(trax_region*) * list->size);
+    list->properties = (trax_properties**) realloc(list->properties, sizeof(trax_properties*) * list->size);
+
+    for (i = 0; i < src->size; i++) {
+        list->regions[i + o] = trax_region_clone(src->regions[i]);
+        list->properties[i + o] = trax_properties_create();
+        copy_properties(src->properties[i], list->properties[i + o], COPY_ALL | COPY_OVERWRITE);
+    }
+
+    return list->size;
+
+}
+
 trax_image_list* trax_image_list_create() {
 
     int i;
 
     trax_image_list* list = (trax_image_list*)malloc(sizeof(trax_image_list));
 
     for (i = 0; i < TRAX_CHANNELS; i++)
```

### Comparing `vot-trax-3.0.3/trax/trax.h` & `vot-trax-4.0.0/trax/trax.h`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #if defined(_MSC_VER)
 #pragma comment(lib, "ws2_32.lib")
 #endif
 #else
 #define TRAX_NO_LOG -1
 #endif
 
-#define TRAX_VERSION 3
+#define TRAX_VERSION 4
 
 #define TRAX_ERROR -1
 #define TRAX_OK 0
 #define TRAX_HELLO 1
 #define TRAX_INITIALIZE 2
 #define TRAX_FRAME 3
 #define TRAX_QUIT 4
@@ -68,25 +68,26 @@
 
 #define TRAX_REGION_EMPTY 0
 #define TRAX_REGION_SPECIAL 1
 #define TRAX_REGION_RECTANGLE 2
 #define TRAX_REGION_POLYGON 4
 #define TRAX_REGION_MASK 8
 
-#define TRAX_REGION_ANY (TRAX_REGION_RECTANGLE | TRAX_REGION_POLYGON)
+#define TRAX_REGION_ANY (TRAX_REGION_RECTANGLE | TRAX_REGION_POLYGON | TRAX_REGION_MASK)
 
 #define TRAX_FLAG_VALID 1
 #define TRAX_FLAG_SERVER 2
 #define TRAX_FLAG_TERMINATED 4
 
 #define TRAX_PARAMETER_VERSION 0
 #define TRAX_PARAMETER_CLIENT 1
 #define TRAX_PARAMETER_SOCKET 2
 #define TRAX_PARAMETER_REGION 3
 #define TRAX_PARAMETER_IMAGE 4
+#define TRAX_PARAMETER_MULTIOBJECT 5
 
 #define TRAX_CHANNELS 3
 #define TRAX_CHANNEL_COLOR 1
 #define TRAX_CHANNEL_DEPTH 2
 #define TRAX_CHANNEL_IR 4
 
 #define TRAX_CHANNEL_INDEX(I) ( \
@@ -97,14 +98,29 @@
 #define TRAX_CHANNEL_ID(I) ( \
     (I) == 0 ? TRAX_CHANNEL_COLOR : ( \
     (I) == 1 ? TRAX_CHANNEL_DEPTH : ( \
     (I) == 2 ? TRAX_CHANNEL_IR : -1)))
 
 #define TRAX_LOCALHOST "127.0.0.1"
 
+// Metadata flags
+#define TRAX_METADATA_MULTI_OBJECT 1
+
+#ifdef TRAX_LEGACY_SINGLE
+#define trax_server_wait trax_server_wait_sot
+#define trax_server_reply trax_server_reply_sot
+#define trax_server_setup(M, L) trax_server_setup_v(M, L, 3)
+#define trax_server_setup_file(M, I, O, L) trax_server_setup_file_v(M, I, O, L, 3)
+#else
+#define trax_server_wait trax_server_wait_mot
+#define trax_server_reply trax_server_reply_mot
+#define trax_server_setup(M, L) trax_server_setup_v(M, L, 0)
+#define trax_server_setup_file(M, I, O, L) trax_server_setup_file_v(M, I, O, L, 0)
+#endif
+
 #define TRAX_SUPPORTS(F, M) (((F) & (M)) != 0)
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /**
@@ -126,14 +142,24 @@
 
 /**
  * A placeholder for properties structure. Use the trax_properties_* functions to manipulate
  * the data.
 **/
 typedef struct trax_properties trax_properties;
 
+/**
+ * A placeholder for object list structure. Use the trax_object_list_* functions to manipulate
+ * the data.
+**/
+typedef struct trax_object_list {
+    int size;
+    trax_region** regions;
+    trax_properties** properties; 
+} trax_object_list;
+
 typedef struct trax_bounds {
 
     float top;
     float bottom;
     float left;
     float right;
 
@@ -155,14 +181,15 @@
 /**
  * Metadata used to specify tracker metadata and taxonomy.
 **/
 typedef struct trax_metadata {
     int format_region;
     int format_image;
     int channels; // Encodes the number of channels (RGB, RGB+D, RGB+IR)
+    int flags;
     char* tracker_name;
     char* tracker_description;
     char* tracker_family;
     trax_properties* custom;
 } trax_metadata;
 
 typedef trax_metadata trax_configuration;
@@ -173,37 +200,38 @@
 typedef struct trax_handle {
     int flags;
     int version;
     void* stream;
     trax_logging logging;
     trax_metadata* metadata;
     char* error;
+    int objects;
 } trax_handle;
 
 /**
  * Array for keeping images (RGB, Depth, IR)
 **/
 typedef struct trax_image_list {
-    trax_image* images[3];
+    trax_image* images[TRAX_CHANNELS];
 } trax_image_list;
 
 __TRAX_EXPORT extern const trax_logging trax_no_log;
 
 __TRAX_EXPORT extern const trax_bounds trax_no_bounds;
 
 /**
  * Returns library version.
 **/
 __TRAX_EXPORT const char* trax_version();
 
 /**
- * Create a tracker metadata structure.
+ * Create a tracker metadata structure. The last argument contains metadata flags that influence communication modes.
 **/
 __TRAX_EXPORT trax_metadata* trax_metadata_create(int region_formats, int image_formats, int channels,
-    const char* tracker_name, const char* tracker_description, const char* tracker_family);
+    const char* tracker_name, const char* tracker_description, const char* tracker_family, int flags);
 
 /**
  * Correctly releases a metadata structure.
 **/
 __TRAX_EXPORT void trax_metadata_release(trax_metadata** metadata);
 
 /**
@@ -225,45 +253,55 @@
  * Setups the protocol state object for the client and returns a handle object.
 **/
 __TRAX_EXPORT trax_handle* trax_client_setup_socket(int server, int timeout, const trax_logging log);
 
 /**
  * Waits for a valid protocol message from the server.
 **/
-__TRAX_EXPORT int trax_client_wait(trax_handle* client, trax_region** region, trax_properties* properties);
+__TRAX_EXPORT int trax_client_wait(trax_handle* client, trax_object_list** objects, trax_properties* properties);
 
 /**
- * Sends an initialize message.
+ * Sends an initialize message, tracking state should be reset.
 **/
-__TRAX_EXPORT int trax_client_initialize(trax_handle* client, trax_image_list* image, trax_region* region, trax_properties* properties);
+__TRAX_EXPORT int trax_client_initialize(trax_handle* client, trax_image_list* image, trax_object_list* objects, trax_properties* properties);
 
 /**
  * Sends a frame message.
 **/
-__TRAX_EXPORT int trax_client_frame(trax_handle* client, trax_image_list* images, trax_properties* properties);
+__TRAX_EXPORT int trax_client_frame(trax_handle* client, trax_image_list* images, trax_object_list* objects, trax_properties* properties);
 
 /**
  * Setups the protocol for the server side and returns a handle object.
 **/
-__TRAX_EXPORT trax_handle* trax_server_setup(trax_metadata *metadata, const trax_logging log);
+__TRAX_EXPORT trax_handle* trax_server_setup_v(trax_metadata *metadata, const trax_logging log, int version);
 
 /**
  * Setups the protocol for the server side and returns a handle object.
 **/
-__TRAX_EXPORT trax_handle* trax_server_setup_file(trax_metadata *metadata, int input, int output, const trax_logging log);
+__TRAX_EXPORT trax_handle* trax_server_setup_file_v(trax_metadata *metadata, int input, int output, const trax_logging log, int version);
 
 /**
- * Waits for a valid protocol message from the client.
+ * Waits for a valid protocol message from the client. This method can only be used in single-object tracking mode.
 **/
-__TRAX_EXPORT int trax_server_wait(trax_handle* server, trax_image_list** images, trax_region** region, trax_properties* properties);
+__TRAX_EXPORT int trax_server_wait_sot(trax_handle* server, trax_image_list** images, trax_region** region, trax_properties* properties);
 
 /**
- * Sends a status reply to the client.
+ * Sends a status reply to the client. This method can only be used in single-object tracking mode.
 **/
-__TRAX_EXPORT int trax_server_reply(trax_handle* server, trax_region* region, trax_properties* properties);
+__TRAX_EXPORT int trax_server_reply_sot(trax_handle* server, trax_region* region, trax_properties* properties);
+
+/**
+ * Waits for a valid protocol message from the client. This method can only be used in multi-object tracking mode.
+**/
+__TRAX_EXPORT int trax_server_wait_mot(trax_handle* server, trax_image_list** images, trax_object_list** objects, trax_properties* properties);
+
+/**
+ * Sends a status reply to the client. This method can only be used in single-object tracking mode.
+**/
+__TRAX_EXPORT int trax_server_reply_mot(trax_handle* server, trax_object_list* objects);
 
 /**
  * Used in client and server. Closes communication, sends quit message if needed.
 **/
 __TRAX_EXPORT int trax_terminate(trax_handle* handle, const char* reason);
 
 /**
@@ -469,14 +507,49 @@
 
 /**
  * Decodes string representation of a region to an object.
  **/
 __TRAX_EXPORT trax_region* trax_region_decode(const char* data);
 
 /**
+* Allocate memory for storing multi object data.
+**/
+__TRAX_EXPORT trax_object_list* trax_object_list_create(int count);
+
+/**
+ * Destroy a object list object and clean up the memory, this also releases all objects.
+ **/
+__TRAX_EXPORT void trax_object_list_release(trax_object_list** list);
+
+/**
+ * Set a region of an object in a list. 
+ **/
+__TRAX_EXPORT void trax_object_list_set(trax_object_list* list, int index, trax_region* region);
+
+/**
+ * Set a region of an object in a list.
+ **/
+__TRAX_EXPORT trax_region* trax_object_list_get(trax_object_list* list, int index);
+
+/**
+ * Retrieve pointer to properties of a specific object in list.
+ **/
+__TRAX_EXPORT trax_properties* trax_object_list_properties(trax_object_list* list, int index);
+
+/**
+ * Get a number of objects in a list.
+ **/
+__TRAX_EXPORT int trax_object_list_count(const trax_object_list* list);
+
+/**
+ * Append one object list to another.
+ **/
+__TRAX_EXPORT int trax_object_list_append(trax_object_list* list, const trax_object_list* src);
+
+/**
  * Destroy a properties object and clean up the memory.
  **/
 __TRAX_EXPORT void trax_properties_release(trax_properties** properties);
 
 /**
  * Clear a properties object.
  **/
@@ -489,14 +562,19 @@
 
 /**
  * Create a property object using values from extisting property object.
  **/
 __TRAX_EXPORT trax_properties* trax_properties_copy(const trax_properties* original);
 
 /**
+ * Returns non-zero value if the entry exits and zero otherwise.
+ **/
+__TRAX_EXPORT int trax_properties_has(const trax_properties* properties, const char* key);
+
+/**
  * Set a string property (the value string is cloned).
  **/
 __TRAX_EXPORT void trax_properties_set(trax_properties* properties, const char* key, const char* value);
 
 /**
  * Set an integer property. The value will be encoded as a string.
  **/
@@ -533,14 +611,19 @@
 /**
  * Iterate over the property set using a callback function. An optional pointer can be given and is forwarded
  * to the callback.
  **/
 __TRAX_EXPORT void trax_properties_enumerate(const trax_properties* properties, trax_enumerator enumerator, const void* object);
 
 /**
+ * Append all properties from source to drain, optionally overwriting existing properties with same keys.
+ **/
+__TRAX_EXPORT void trax_properties_append(const trax_properties* source, trax_properties* drain, int overwrite);
+
+/**
 * Allocate memory for storing the input images
 **/
 __TRAX_EXPORT trax_image_list* trax_image_list_create();
 
 /**
 * Release image list structure, does not release any channel images
 **/
@@ -558,15 +641,15 @@
 
 /**
 * Set image at a specific channel
 **/
 __TRAX_EXPORT void trax_image_list_set(trax_image_list* list, trax_image* image, int channel);
 
 /**
-* Count the channels in descriptor bit-set
+* Size of the image list
 **/
 __TRAX_EXPORT int trax_image_list_count(int channels);
 
 #ifdef __cplusplus
 }
 
 #include <string>
@@ -575,14 +658,15 @@
 #include <algorithm>
 #include <iostream>
 
 namespace trax {
 
 class Image;
 class ImageList;
+class ObjectList;
 class Region;
 class Properties;
 
 typedef trax_enumerator Enumerator;
 
 class __TRAX_EXPORT Logging : public ::trax_logging {
 public:
@@ -608,16 +692,20 @@
     }
 
 protected:
     Wrapper();
 
     Wrapper(const Wrapper& count);
 
+    Wrapper(Wrapper&& count);
+
     void swap(Wrapper& lhs);
 
+    void acquire(const Wrapper& lhs);
+
     long claims() const;
 
     /**
      * Call after the wrapped pointer has been created or copied to increase
      * reference count;
     **/
     void acquire();
@@ -634,29 +722,33 @@
 
     long* pn;
 
 };
 
 class Handle;
 class Client;
-class Server;
+class ServerSOT;
+class ServerMOT;
 
 class __TRAX_EXPORT Metadata : public Wrapper {
 friend class Handle;
 friend class Client;
-friend class Server;
+friend class ServerSOT;
+friend class ServerMOT;
 public:
 
     Metadata();
 
     Metadata(const Metadata& original);
 
+    Metadata(Metadata&& original);
+
     Metadata(int region_formats, int image_formats, int channels = TRAX_CHANNEL_COLOR,
         std::string tracker_name = std::string(), std::string tracker_description = std::string(),
-        std::string tracker_family = std::string());
+        std::string tracker_family = std::string(), int flags = 0);
 
     virtual ~Metadata();
 
     int image_formats() const;
 
     int region_formats() const;
 
@@ -668,15 +760,17 @@
 
     std::string tracker_family() const;
 
     std::string get_custom(const std::string key) const;
 
     void set_custom(const std::string key, const std::string value);
 
-    Metadata& operator=(Metadata p) throw();
+    Metadata& operator=(const Metadata& p) throw();
+
+    Metadata& operator=(Metadata&& p) throw();
 
 protected:
 
     Metadata(trax_metadata* metadata);
 
     virtual void cleanup();
 
@@ -730,91 +824,147 @@
 
     void wrap(trax_handle* obj);
 
     Handle();
 
     Handle(const Handle& original);
 
+    Handle(Handle&& original);
+
     trax_handle* handle;
 };
 
 class __TRAX_EXPORT Client: public Handle {
 public:
     /**
      * Sets up the protocol for the client side and returns a handle object.
     **/
     Client(int input, int output, Logging logger);
 
     /**
      * Sets up the protocol for the client side and returns a handle object.
     **/
-    Client(int server, Logging logger,  int timeout = -1);
+    Client(int server, Logging logger, int timeout = -1);
 
     virtual ~Client();
 
     /**
-    * Waits for a valid protocol message from the server.
+    * Waits for a valid protocol message from the server. Only works in single-object mode
     **/
     int wait(Region& region, Properties& properties);
 
     /**
+    * Waits for a valid protocol message from the server. Returns the state of one or more objects.
+    **/
+    int wait(ObjectList& objects, Properties& properties);
+
+    /**
     * Sends an initialize message.
     **/
     int initialize(const ImageList& image, const Region& region, const Properties& properties);
 
     /**
+    * Sends an initialize message with one or more objects.
+    **/
+    int initialize(const ImageList& image, const ObjectList& objects, const Properties& properties);
+
+    /**
     * Sends a frame message.
     **/
     int frame(const ImageList& image, const Properties& properties);
 
+    /**
+    * Sends a frame message that adds new objects (in multi-object mode).
+    **/
+    int frame(const ImageList& image, const ObjectList& objects, const Properties& properties);
+
 protected:
 
     using Handle::cleanup;
 
 private:
 
     Client& operator=(Client p) throw();
 
 };
 
-class __TRAX_EXPORT Server: public Handle {
+class __TRAX_EXPORT ServerMOT: public Handle {
+public:
+
+    /**
+     * Sets up the protocol for the server side and returns a handle object.
+    **/
+    ServerMOT(Metadata metadata, Logging log);
+
+    virtual ~ServerMOT();
+
+    /**
+     * Waits for a valid protocol message from the client.
+    **/
+    int wait(ImageList& image, Region& region, Properties& properties);
+
+    /**
+     * Sends a status reply to the client.
+    **/
+    int reply(const Region& region, const Properties& properties);
+
+    /**
+     * Waits for a valid protocol message from the client.
+    **/
+    int wait(ImageList& image, ObjectList& objects, Properties& properties);
+
+    /**
+     * Sends a status reply to the client.
+    **/
+    int reply(const ObjectList& objects);
+
+private:
+    ServerMOT& operator=(ServerMOT p) throw();
+
+};
+
+class __TRAX_EXPORT ServerSOT: public Handle {
 public:
 
     /**
      * Sets up the protocol for the server side and returns a handle object.
     **/
-    Server(Metadata metadata, Logging log);
+    ServerSOT(Metadata metadata, Logging log);
 
-    virtual ~Server();
+    virtual ~ServerSOT();
 
     /**
      * Waits for a valid protocol message from the client.
     **/
     int wait(ImageList& image, Region& region, Properties& properties);
 
     /**
      * Sends a status reply to the client.
     **/
     int reply(const Region& region, const Properties& properties);
 
 private:
-    Server& operator=(Server p) throw();
+    ServerSOT& operator=(ServerSOT p) throw();
 
 };
 
 class __TRAX_EXPORT Image : public Wrapper {
 friend class Client;
-friend class Server;
+friend class ServerSOT;
+friend class ServerMOT;
 friend class ImageList;
+friend class ObjectList;
 public:
 
     Image();
 
     Image(const Image& original);
 
+    Image(Image&& original);
+
     /**
      * Creates a file-system path image description.
     **/
     static Image create_path(const std::string& path);
 
     /**
      * Creates a URL path image description.
@@ -875,15 +1025,18 @@
 
     /**
      * Returns a file buffer and its length. This function
      * returns a pointer to the internal data which should not be modified.
     **/
     const char* get_buffer(int* length, int* format) const;
 
-    Image& operator=(Image lhs) throw();
+    Image& operator=(const Image& lhs) throw();
+
+    Image& operator=(Image&& lhs) throw();
+
 
 protected:
 
     virtual void cleanup();
 
     void wrap(trax_image* obj);
 
@@ -891,21 +1044,24 @@
 
     trax_image* image;
 
 };
 
 class __TRAX_EXPORT ImageList : public Wrapper {
 friend class Client;
-friend class Server;
+friend class ServerSOT;
+friend class ServerMOT;
 public:
 
     ImageList();
 
     ImageList(const ImageList& original);
 
+    ImageList(ImageList&& original);
+
     /**
      * Releases image list structure, frees allocated memory.
     **/
     virtual ~ImageList();
 
     /**
     * Get image at a specific channel
@@ -918,43 +1074,102 @@
     bool has(int channel_num) const;
 
     /**
     * Set image at a specific channel
     **/
     void set(Image image, int channel_num);
 
-    ImageList& operator=(ImageList lhs) throw();
-
     int size() const;
 
+    ImageList& operator=(const ImageList& lhs) throw();
+
+    ImageList& operator=(ImageList&& lhs) throw();
+
 protected:
 
     virtual void cleanup();
 
     void wrap(trax_image_list* obj);
 
 private:
 
     std::vector<Image> images;
 
     trax_image_list* list;
 
 };
 
+class __TRAX_EXPORT ObjectList : public Wrapper {
+friend class Client;
+friend class ServerSOT;
+friend class ServerMOT;
+public:
+    ObjectList();
+
+    ObjectList(int count);
+
+    ObjectList(const ObjectList& original);
+
+    ObjectList(ObjectList&& original);
+
+    /**
+     * Releases object list and frees allocated memory.
+    **/
+    virtual ~ObjectList();
+
+    /**
+    * Get object region at a specific index
+    **/
+    Region get(int index) const;
+
+    /**
+    * Set object region at a specific index
+    **/
+    void set(int index, Region region);
+
+    /**
+    * Get object properties at a specific index
+    **/
+    Properties properties(int index) const;
+
+    int size() const;
+
+    ObjectList& operator=(const ObjectList& lhs) throw();
+
+    ObjectList& operator=(ObjectList&& lhs) throw();
+
+protected:
+
+    virtual void cleanup();
+
+    void wrap(trax_object_list* obj);
+
+private:
+
+    std::vector<Region> _regions;
+    std::vector<Properties> _properties;
 
+    trax_object_list* list;
+
+};
 
 class __TRAX_EXPORT Region : public Wrapper {
 friend class Client;
-friend class Server;
+friend class ServerSOT;
+friend class ServerMOT;
+friend class ObjectList;
 public:
 
     Region();
 
     Region(const Region& original);
 
+    Region(Region&& original);
+
+
     /**
      * Creates a special region object. Only one paramter (region code) required.
     **/
     static Region create_special(int code);
 
     /**
      * Creates a rectangle region.
@@ -1044,49 +1259,58 @@
 
     bool contains(float x, float y) const;
 
     Region convert(int type) const;
 
     float overlap(const Region& region, const Bounds& bounds = Bounds()) const;
 
-    Region& operator=(Region lhs) throw();
-
     operator std::string () const;
 
     friend __TRAX_EXPORT std::ostream& operator<< (std::ostream& output, const Region& region);
 
     friend __TRAX_EXPORT std::istream& operator>> (std::istream& input, Region &D);
 
+    Region& operator=(const Region& lhs) throw();
+
+    Region& operator=(Region&& lhs) throw();
+
 protected:
 
     virtual void cleanup();
 
     void wrap(trax_region* obj);
 
 private:
 
     trax_region* region;
 };
 
 class __TRAX_EXPORT Properties : public Wrapper {
 friend class Client;
-friend class Server;
+friend class ServerSOT;
+friend class ServerMOT;
+friend class ObjectList;
 public:
 
     /**
      * Create a property object.
      **/
     Properties();
 
     /**
      * A copy constructor.
      **/
     Properties(const Properties& original);
 
     /**
+     * A move constructor.
+     **/
+    Properties(Properties&& original);
+
+    /**
      * Destroy a properties object and clean up the memory.
      **/
     virtual ~Properties();
 
     /**
      * Return number of property pairs.
      **/
@@ -1147,31 +1371,38 @@
 
     void from_map(const std::map<std::string, std::string>& m);
 
     void to_map(std::map<std::string, std::string>& m) const;
 
     void to_vector(std::vector<std::string>& v) const;
 
-    Properties& operator=(Properties lhs) throw();
-
     friend __TRAX_EXPORT std::ostream& operator<< (std::ostream& output, const Properties& properties);
 
+    Properties& operator=(const Properties& lhs) throw();
+
+    Properties& operator=(Properties&& lhs) throw();
+
 protected:
 
     virtual void cleanup();
 
     void wrap(trax_properties* obj);
 
 private:
 
     void ensure_unique();
 
     trax_properties* properties;
 
 };
 
+#ifdef TRAX_LEGACY_SINGLE
+typedef ServerSOT Server;
+#else
+typedef ServerMOT Server;
+#endif
 
 }
 
 #endif
 
 #endif
```

### Comparing `vot-trax-3.0.3/trax/traxpp.cpp` & `vot-trax-4.0.0/trax/traxpp.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -55,21 +55,32 @@
 }
 
 Wrapper::Wrapper() : pn(NULL) {
 
 }
 
 Wrapper::Wrapper(const Wrapper& count) : pn(count.pn) {
+	acquire();
+}
 
+
+Wrapper::Wrapper(Wrapper&& count) : pn(count.pn) {
+	count.pn = NULL;
 }
 
 Wrapper::~Wrapper() {
 
 }
 
+void Wrapper::acquire(const Wrapper& lhs) {
+	release();
+	pn = lhs.pn;
+	acquire();
+}
+
 void Wrapper::swap(Wrapper& lhs) {
 	std::swap(pn, lhs.pn);
 }
 
 long Wrapper::claims() const {
 	long count = 0;
 	if (NULL != pn)
@@ -94,39 +105,41 @@
 			delete pn;
 		}
 		pn = NULL;
 	}
 }
 
 Metadata::Metadata() {
+    wrap(trax_metadata_create(0, 0, TRAX_CHANNEL_COLOR, NULL, NULL, NULL, 0));
+}
 
-    wrap(trax_metadata_create(0, 0, TRAX_CHANNEL_COLOR, NULL, NULL, NULL));
+Metadata::Metadata(Metadata&& original) : Wrapper(std::move(original)) {
+	metadata = original.metadata;
 }
 
 Metadata::Metadata(const Metadata& original) : Wrapper(original) {
-	if (original.metadata) acquire();
 	metadata = original.metadata;
 }
 
 Metadata::Metadata(int region_formats, int image_formats, int channels,
                    std::string tracker_name, std::string tracker_description,
-                   std::string tracker_family) {
+                   std::string tracker_family, int flags) {
 
     wrap(trax_metadata_create(region_formats, image_formats, channels,
 		(tracker_name.empty()) ? NULL : tracker_name.c_str(),
 		(tracker_description.empty()) ? NULL : tracker_description.c_str(),
-		(tracker_family.empty()) ? NULL : tracker_family.c_str()
+		(tracker_family.empty()) ? NULL : tracker_family.c_str(), flags
 		));
 
 }
 
 Metadata::Metadata(trax_metadata* metadata) {
 
     wrap(trax_metadata_create(metadata->format_region, metadata->format_image, metadata->channels,
-		metadata->tracker_name, metadata->tracker_description, metadata->tracker_family));
+		metadata->tracker_name, metadata->tracker_description, metadata->tracker_family, metadata->flags));
 
 }
 
 Metadata::~Metadata() {
 	release();
 }
 
@@ -174,20 +187,24 @@
 void Metadata::wrap(trax_metadata* obj) {
 	if (!obj) return;
 	release();
 	if (obj) acquire();
 	metadata = obj;
 }
 
-Metadata& Metadata::operator=(Metadata lhs) throw() {
+Metadata& Metadata::operator=(const Metadata& lhs) throw() {
+	acquire(lhs);
+	metadata = lhs.metadata;
+	return *this;
+}
 
-	std::swap(metadata, lhs.metadata);
+Metadata& Metadata::operator=(Metadata&& lhs) throw() {
 	swap(lhs);
+	std::swap(metadata, lhs.metadata);
 	return *this;
-
 }
 
 std::string Metadata::get_custom(const std::string key) const {
 
 	char* cval = trax_properties_get(metadata->custom, key.c_str());
 
 	if (!cval) return std::string();
@@ -205,15 +222,18 @@
 }
 
 Handle::Handle() {
 	handle = NULL;
 }
 
 Handle::Handle(const Handle& original) : Wrapper(original) {
-	if (original.handle) acquire();
+	handle = original.handle;
+}
+
+Handle::Handle(Handle&& original) : Wrapper(original) {
 	handle = original.handle;
 }
 
 Handle::~Handle() {
 	release();
 }
 
@@ -278,91 +298,246 @@
 	// Cleanup done in Handle
 }
 
 int Client::wait(Region& region, Properties& properties) {
 
 	if (!claims()) return -1;
 
+	trax_object_list* tobjects = NULL;
 	trax_region* tregion = NULL;
 
 	properties.ensure_unique();
 
-	int result = trax_client_wait(handle, &tregion, properties.properties);
+	int result = trax_client_wait(handle, &tobjects, properties.properties);
 
-	if (tregion)
-		region.wrap(tregion);
+	if (tobjects) {
+		if (trax_object_list_count(tobjects) > 1) {
+			trax_object_list_release(&tobjects);
+			return TRAX_ERROR;
+		}
+
+		if (trax_object_list_count(tobjects) == 1) {
+			tregion = trax_region_clone(trax_object_list_get(tobjects, 0));
+			region.wrap(tregion);
+			trax_properties_append(trax_object_list_properties(tobjects, 0), properties.properties, 0);
+		}
+		trax_object_list_release(&tobjects);
+	}
+	
+	return result;
+
+}
+
+int Client::wait(ObjectList& objects, Properties& properties) {
+
+	if (!claims()) return -1;
+
+	trax_object_list* tobjects = NULL;
+
+	properties.ensure_unique();
+
+	int result = trax_client_wait(handle, &tobjects, properties.properties);
+
+	if (tobjects) {
+		objects.wrap(tobjects);
+	}
 
 	return result;
 
 }
 
 int Client::initialize(const ImageList& image, const Region& region, const Properties& properties) {
 	if (!claims()) return -1;
 
-	return trax_client_initialize(handle, image.list, region.region, properties.properties);
+	trax_object_list* objects = trax_object_list_create(1);
+	trax_object_list_set(objects, 0, region.region);
+
+	int result = trax_client_initialize(handle, image.list, objects, properties.properties);
+
+	trax_object_list_release(&objects);
+
+	return result;
+
+}
+
+int Client::initialize(const ImageList& image, const ObjectList& objects, const Properties& properties) {
+	if (!claims()) return -1;
+
+	return trax_client_initialize(handle, image.list, objects.list, properties.properties);
 
 }
 
 int Client::frame(const ImageList& image, const Properties& properties) {
 	if (!claims()) return -1;
 
-	return trax_client_frame(handle, image.list, properties.properties);
+	return trax_client_frame(handle, image.list, NULL, properties.properties);
+
+}
+
+int Client::frame(const ImageList& image, const ObjectList& objects, const Properties& properties) {
+
+	if (!claims()) return -1;
+
+	return trax_client_frame(handle, image.list, objects.list, properties.properties);
 
 }
 
-Server::Server(Metadata metadata, Logging log) {
+ServerSOT::ServerSOT(Metadata metadata, Logging log) {
 
-	wrap(trax_server_setup(metadata.metadata, log));
+	wrap(trax_server_setup_v(metadata.metadata, log, 3));
 
 }
 
-Server::~Server() {
+ServerSOT::~ServerSOT() {
 	// Cleanup done in Handle
 }
 
-int Server::wait(ImageList& image, Region& region, Properties& properties) {
+int ServerSOT::wait(ImageList& image, Region& region, Properties& properties) {
 
 	if (!claims()) return -1;
 
 	trax_region* tregion = NULL;
 
     trax_image_list* timagelist = NULL;
 
 	properties.ensure_unique();
 
-    int result = trax_server_wait(handle, &timagelist, &tregion, properties.properties);
+    int result = trax_server_wait_sot(handle, &timagelist, &tregion, properties.properties);
 
 	if (tregion)
 		region.wrap(tregion);
 
 	if (timagelist) {
 		image.wrap(timagelist);		
 	}
 
 	return result;
 
 }
 
-int Server::reply(const Region& region, const Properties& properties) {
+int ServerSOT::reply(const Region& region, const Properties& properties) {
 
 	if (!claims()) return -1;
 
-	return trax_server_reply(handle, region.region, properties.properties);
+	return trax_server_reply_sot(handle, region.region, properties.properties);
+
+}
+
+ServerMOT::ServerMOT(Metadata metadata, Logging log) {
+
+	wrap(trax_server_setup_v(metadata.metadata, log, 0));
+
+}
+
+ServerMOT::~ServerMOT() {
+	// Cleanup done in Handle
+}
+
+int ServerMOT::wait(ImageList& image, Region& region, Properties& properties) {
+
+	if (!claims()) return -1;
+
+	trax_object_list* tobjects = NULL;
+    trax_image_list* timagelist = NULL;
+	trax_region* tregion = NULL;
+
+	properties.ensure_unique();
+
+    int result = trax_server_wait_mot(handle, &timagelist, &tobjects, properties.properties);
+
+	if (timagelist) {
+		image.wrap(timagelist);		
+	}
+
+	if (tobjects) {
+		if (trax_object_list_count(tobjects) > 1) {
+			trax_object_list_release(&tobjects);
+			return TRAX_ERROR;
+		}
+		if (trax_object_list_count(tobjects) == 1) {
+			tregion = trax_region_clone(trax_object_list_get(tobjects, 0));
+			region.wrap(tregion);
+			trax_properties_append(trax_object_list_properties(tobjects, 0), properties.properties, 0);
+		}
+	}
+
+	return result;
+
+}
+
+int ServerMOT::reply(const Region& region, const Properties& properties) {
+
+	if (!claims()) return -1;
+
+	trax_object_list* objects = trax_object_list_create(1);
+	trax_object_list_set(objects, 0, region.region);
+	trax_properties_append(trax_object_list_properties(objects, 0), properties.properties, 0);
+
+	int result = trax_server_reply_mot(handle, objects);
+
+	trax_object_list_release(&objects);
+
+	return result;
+
+}
+
+int ServerMOT::wait(ImageList& image, ObjectList& objects, Properties& properties) {
+
+	trax_object_list* tobjects = NULL;
+    trax_image_list* timagelist = NULL;
+
+	properties.ensure_unique();
+
+	int result = trax_server_wait_mot(handle, &timagelist, &tobjects, properties.properties);
+
+	if (timagelist) {
+		image.wrap(timagelist);		
+	}
+
+	if (tobjects) {
+		objects.wrap(tobjects);
+	}
+
+	return result;
+
+}
+
+
+int ServerMOT::reply(const ObjectList& objects) {
+
+	if (!claims()) return -1;
+
+	return trax_server_reply_mot(handle, objects.list);
 
 }
 
 Image::Image() {
 	image = NULL;
 }
 
 Image::Image(const Image& original) : Wrapper(original) {
-	if (original.image) acquire();
 	image = original.image;
 }
 
+Image::Image(Image&& original) : Wrapper(std::move(original)) {
+	image = original.image;
+}
+
+Image& Image::operator=(const Image& lhs) throw() {
+	acquire(lhs);
+	image = lhs.image;
+	return *this;
+}
+
+Image& Image::operator=(Image&& lhs) throw() {
+	swap(lhs);
+	std::swap(image, lhs.image);
+	return *this;
+}
+
 Image Image::create_path(const std::string& path) {
 	Image image;
 	image.wrap(trax_image_create_path(path.c_str()));
 	return image;
 }
 
 Image Image::create_url(const std::string& url) {
@@ -416,41 +591,145 @@
 }
 
 const char* Image::get_buffer(int* length, int* format) const {
 	return trax_image_get_buffer(image, length, format);
 }
 
 void Image::cleanup() {
+	if (!image) return;
 	trax_image_release(&image);
 }
 
 void Image::wrap(trax_image* obj) {
 	if (!obj) return;
 	release();
 	image = obj;
 	if (image) acquire();
 }
 
-Image& Image::operator=(Image lhs) throw() {
-	std::swap(image, lhs.image);
-	swap(lhs);
+ObjectList::ObjectList() {
+	list = NULL;
+}
+
+ObjectList::ObjectList(int count) {
+	list = trax_object_list_create(count);
+	_regions.resize(count);
+	_properties.resize(count);
+}
+
+ObjectList::ObjectList(const ObjectList& original) : Wrapper(original) {
+	list = original.list;
+	_regions = original._regions;
+	_properties = original._properties;
+}
+
+ObjectList::ObjectList(ObjectList&& original) : Wrapper(std::move(original)) {
+	std::swap(list, original.list);
+	std::swap(_regions, original._regions);
+	std::swap(_properties, original._properties);
+}
+
+
+ObjectList& ObjectList::operator=(const ObjectList& original) throw() {
+	acquire(original);
+	list = original.list;
+	_regions = original._regions;
+	_properties = original._properties;
+	return *this;
+}
+
+ObjectList& ObjectList::operator=(ObjectList&& original) throw() {
+	swap(original);
+	std::swap(list, original.list);
+	std::swap(_regions, original._regions);
+	std::swap(_properties, original._properties);
 	return *this;
 }
 
+ObjectList::~ObjectList() {
+	release();
+}
+
+Region ObjectList::get(int index) const {
+	return _regions[index];
+}
+
+void ObjectList::set(int index, Region region) {
+	_regions[index] = region;
+	list->regions[index] = region.region;
+	// Do not use C function as it will try to free old region
+	// trax_object_list_set(list, index, region.region);
+}
+
+Properties ObjectList::properties(int index) const {
+	return _properties[index];
+}
+
+int ObjectList::size() const {
+	if (!list) return 0;
+	return trax_object_list_count(list);
+}
+
+
+void ObjectList::cleanup() {
+	if (!list) return;
+	// Only free the structure, regions and properties will be 
+	// released by proxies
+	free(list->regions);
+	free(list->properties);
+	free(list);
+	_regions.clear();
+	_properties.clear();
+}
+
+void ObjectList::wrap(trax_object_list* obj) {
+	if (!obj) return;
+	release();
+	list = obj;
+	if (list) acquire();
+
+	_regions.resize(trax_object_list_count(obj));
+	_properties.resize(trax_object_list_count(obj));
+
+	for (int i = 0; i < trax_object_list_count(obj); i++) {
+		_regions[i].wrap(obj->regions[i]);
+		_properties[i].wrap(obj->properties[i]);
+	}
+}
+
+
 ImageList::ImageList()  {
 	list = trax_image_list_create();
 	images.resize(TRAX_CHANNELS);
 }
 
 ImageList::ImageList(const ImageList& original)  : Wrapper(original) {
-	if (original.list) acquire();
 	list = original.list;
 	images = original.images;
 }
 
+ImageList::ImageList(ImageList&& original)  : Wrapper(std::move(original)) {
+	std::swap(list, original.list);
+	std::swap(images, original.images);
+}
+
+ImageList& ImageList::operator=(const ImageList& original) throw() {
+	acquire(original);
+	list = original.list;
+	images = original.images;
+	return *this;
+}
+
+ImageList& ImageList::operator=(ImageList&& original) throw() {
+	swap(original);
+	std::swap(list, original.list);
+	std::swap(images, original.images);
+	return *this;
+}
+
 ImageList::~ImageList() {
 	release();
 }
 
 Image ImageList::get(int channel) const {
 
 	return images[TRAX_CHANNEL_INDEX(channel)];
@@ -480,23 +759,16 @@
 			count++;
 
 	}
 
 	return count;
 }
 
-ImageList& ImageList::operator=(ImageList lhs) throw() {
-	std::swap(list, lhs.list);
-	std::swap(images, lhs.images);
-	swap(lhs);
-	return *this;
-}
-
 void ImageList::cleanup() {
-
+	if (!list) return;
 	trax_image_list_release(&list);
 
 }
 
 void ImageList::wrap(trax_image_list* obj) {
 
 	if (!obj) return;
@@ -511,18 +783,33 @@
 
 
 Region::Region() {
 	region = NULL;
 }
 
 Region::Region(const Region& original) : Wrapper(original) {
-	if (original.region) acquire();
 	region = original.region;
 }
 
+Region::Region(Region&& original) : Wrapper(std::move(original)) {
+	std::swap(region, original.region);
+}
+
+Region& Region::operator=(const Region& original) throw() {
+	acquire(original);
+	region = original.region;
+	return *this;
+}
+
+Region& Region::operator=(Region&& original) throw() {
+	swap(original);
+	std::swap(region, original.region);
+	return *this;
+}
+
 Region Region::create_special(int code) {
 
 	Region region;
 	region.wrap(trax_region_create_special(code));
 	return region;
 
 }
@@ -639,14 +926,15 @@
 bool Region::contains(float x, float y) const {
 	if (empty()) return false;
 
 	return trax_region_contains(region, x, y) != 0;
 }
 
 void Region::cleanup() {
+	if (!region) return;
 	trax_region_release(&region);
 }
 
 float Region::overlap(const Region& region, const Bounds& bounds) const {
 
 	if (empty() || region.empty()) return 0;
 
@@ -656,20 +944,14 @@
 void Region::wrap(trax_region* obj) {
 	if (!obj) return;
 	release();
 	if (obj) acquire();
 	region = obj;
 }
 
-Region& Region::operator=(Region lhs) throw() {
-	std::swap(region, lhs.region);
-	swap(lhs);
-	return *this;
-}
-
 Region::operator std::string () const {
 
 	std::string result;
 
 	if (!empty()) {
 		char* str = trax_region_encode(region);
 
@@ -747,18 +1029,27 @@
 
 
 Properties::Properties() {
 	properties = NULL;
 }
 
 Properties::Properties(const Properties& original) : Wrapper(original) {
-	if (original.properties) acquire();
 	properties = original.properties;
 }
 
+Properties::Properties(Properties&& original) : Wrapper(std::move(original)) {
+	std::swap(properties, original.properties);
+}
+
+Properties& Properties::operator=(const Properties& original) throw() {
+	acquire(original);
+	properties = original.properties;
+	return *this;
+}
+
 Properties::~Properties() {
 	release();
 }
 
 int Properties::size() const {
 	if (!properties) return 0;
 	return trax_properties_count(properties);
@@ -824,31 +1115,25 @@
 
 void Properties::enumerate(Enumerator enumerator, void* object)  {
 	if (!properties) return;
 	trax_properties_enumerate(properties, enumerator, object);
 }
 
 void Properties::cleanup() {
-	if (properties)
-		trax_properties_release(&properties);
+	if (!properties) return;
+	trax_properties_release(&properties);
 }
 
 void Properties::wrap(trax_properties* obj) {
 	if (!obj) return;
 	release();
 	properties = obj;
 	acquire();
 }
 
-Properties& Properties::operator=(Properties lhs) throw() {
-	std::swap(properties, lhs.properties);
-	swap(lhs);
-	return *this;
-}
-
 void copy_enumerator(const char *key, const char *value, const void *obj) {
 
 	trax_properties_set((trax_properties*) obj, key, value);
 
 }
 
 void print_enumerator(const char *key, const char *value, const void *obj) {
```

