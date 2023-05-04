# Comparing `tmp/getpack-0.2.4.tar.gz` & `tmp/getpack-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpack-0.2.4.tar", last modified: Fri Apr 28 00:04:39 2023, max compression
+gzip compressed data, was "dist\getpack-0.2.5.tar", last modified: Thu May  4 17:50:30 2023, max compression
```

## Comparing `getpack-0.2.4.tar` & `getpack-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.436935 getpack-0.2.4/
--rw-rw-rw-   0        0        0       37 2023-02-16 21:01:44.000000 getpack-0.2.4/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.360936 getpack-0.2.4/.vscode/
--rw-rw-rw-   0        0        0      186 2022-11-26 18:28:38.000000 getpack-0.2.4/.vscode/cspell.json
--rw-rw-rw-   0        0        0      534 2023-04-27 21:31:59.000000 getpack-0.2.4/.vscode/launch.json
--rw-rw-rw-   0        0        0      500 2022-11-26 18:28:38.000000 getpack-0.2.4/.vscode/settings.json
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2504 2023-04-28 00:04:39.437935 getpack-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.4/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      967 2023-04-28 00:04:39.447938 getpack-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.339940 getpack-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.379936 getpack-0.2.4/src/getpack/
--rw-rw-rw-   0        0        0      403 2023-04-27 21:46:03.000000 getpack-0.2.4/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.4/src/getpack/executable.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.427935 getpack-0.2.4/src/getpack/library/
--rw-rw-rw-   0        0        0     2486 2023-04-03 00:18:28.000000 getpack-0.2.4/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0      449 2023-04-03 00:13:44.000000 getpack-0.2.4/src/getpack/library/ffmpeg.py
--rw-rw-rw-   0        0        0    11596 2023-04-27 23:46:55.000000 getpack-0.2.4/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.423936 getpack-0.2.4/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 00:04:39.000000 getpack-0.2.4/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 00:04:39.435937 getpack-0.2.4/tests/
--rw-rw-rw-   0        0        0     1219 2023-04-28 00:04:00.000000 getpack-0.2.4/tests/test_common.py
--rw-rw-rw-   0        0        0      954 2023-04-27 22:47:06.000000 getpack-0.2.4/tests/test_concurrency.py
--rw-rw-rw-   0        0        0      426 2023-03-31 19:43:17.000000 getpack-0.2.4/tests/test_executable.py
--rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.4/tests/test_unicode.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.390493 getpack-0.2.5/
+-rw-rw-rw-   0        0        0       37 2023-02-16 21:01:44.000000 getpack-0.2.5/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.317797 getpack-0.2.5/.vscode/
+-rw-rw-rw-   0        0        0      186 2022-11-26 18:28:38.000000 getpack-0.2.5/.vscode/cspell.json
+-rw-rw-rw-   0        0        0      534 2023-04-27 21:31:59.000000 getpack-0.2.5/.vscode/launch.json
+-rw-rw-rw-   0        0        0      500 2022-11-26 18:28:38.000000 getpack-0.2.5/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2504 2023-05-04 17:50:30.391494 getpack-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.5/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      967 2023-05-04 17:50:30.402489 getpack-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.280795 getpack-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.339798 getpack-0.2.5/src/getpack/
+-rw-rw-rw-   0        0        0      403 2023-05-04 08:53:10.000000 getpack-0.2.5/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.5/src/getpack/executable.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.379490 getpack-0.2.5/src/getpack/library/
+-rw-rw-rw-   0        0        0     3024 2023-05-04 17:14:18.000000 getpack-0.2.5/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0    12129 2023-05-04 17:46:45.000000 getpack-0.2.5/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.377487 getpack-0.2.5/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.389497 getpack-0.2.5/tests/
+-rw-rw-rw-   0        0        0     1452 2023-05-04 17:20:38.000000 getpack-0.2.5/tests/test_common.py
+-rw-rw-rw-   0        0        0     1071 2023-05-04 17:32:32.000000 getpack-0.2.5/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      426 2023-03-31 19:43:17.000000 getpack-0.2.5/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.5/tests/test_unicode.py
```

### Comparing `getpack-0.2.4/.vscode/launch.json` & `getpack-0.2.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `getpack-0.2.4/LICENSE` & `getpack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.2.4/PKG-INFO` & `getpack-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Description: ### Declarative external resources any with implicit deployment
```

### Comparing `getpack-0.2.4/README.md` & `getpack-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `getpack-0.2.4/setup.cfg` & `getpack-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `getpack-0.2.4/src/getpack/executable.py` & `getpack-0.2.5/src/getpack/executable.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.4/src/getpack/library/__init__.py` & `getpack-0.2.5/src/getpack/library/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import platform
 
 from ..resource import PyPiPackage, WebResource
 from ..executable import Executable
 
 
-class cefpython3(PyPiPackage):
+class CefPython3(PyPiPackage):
     name = 'cefpython3'
     version = '66.1'
 
     if sys.version_info.major == 3 and sys.version_info.minor == 10:
         version = '88.0'
         archive_url = (
             'https://github.com/HonorarPlus/cefpython/releases/'
@@ -74,17 +74,34 @@
     @property
     def platform(self):
         if platform.system() == 'Darwin':
             return 'macos'
         return platform.system().lower()
 
 
-class rclone:
-    pass
+class Rclone:
+    version = '1.62.2'
+    platform = 'windows-amd64'
+    archive_url = (
+        'https://downloads.rclone.org/v{self.version}/'
+        'rclone-v{self.version}-{self.platform}.zip')
 
 
 class Python(Executable, WebResource):
     name = 'python'
     version = '3.7.9'
     archive_url = (
         'https://www.python.org/ftp/python/{self.version}/'
         'python-{self.version}-embed-amd64.zip')
+
+
+class Ffmpeg(Executable, WebResource):
+    name = 'ffmpeg'
+    version = '5.1.2'
+    archive_url = (
+        'https://github.com/GyanD/codexffmpeg/releases/download/'
+        '{self.version}/ffmpeg-{self.version}-essentials_build.zip')
+    archive_extraction = {
+        'ffmpeg-{self.version}-essentials_build/bin/': {
+            'path': '',
+        },
+    }
```

### Comparing `getpack-0.2.4/src/getpack/resource.py` & `getpack-0.2.5/src/getpack/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,24 +30,35 @@
 
 __FILE_LOCK_TIMEOUT__ = 15 * 60
 
 
 class HybridLock:
     def __init__(self, key):
         self.key = key.as_posix() + '.portalock'
+        self.folder = os.path.dirname(self.key)
         self.file_lock = portalocker.RLock(
                 self.key,
                 timeout=__FILE_LOCK_TIMEOUT__,
                 mode='w',
             )
         self.lock = threading.RLock()
 
     def __enter__(self):
         self.lock.acquire()
-        self.file_lock.acquire()
+        if not os.path.isdir(self.folder):
+            try:
+                os.makedirs(self.folder)
+            except FileExistsError:
+                pass  # may fail because of race
+        try:
+            self.file_lock.acquire()
+        except Exception:
+            # attempt to fix rare PermissionError in multiprocess races, maybe
+            # timeout? Have no info on effectiveness of following code
+            self.file_lock.acquire()
 
     def __exit__(self, *_):
         self.file_lock.release()
         self.lock.release()
         try:
             os.unlink(self.key)
         except Exception:
@@ -85,14 +96,18 @@
         Initialization is not heavy operation, feel free to construct a
         Resource and query available versions.
         """
         for k, v in kwargs.items():
             if v is not None:
                 setattr(self, k, v)
 
+    @property
+    def lock(self):
+        return lock(self.path)
+
     def get_available_versions(self):  # type: () -> typing.List[str]
         """Get list of available versions."""
         raise NotImplementedError()
 
     def deploy(self):
         """
         This will produce all the hard work to make resource available, but
@@ -104,15 +119,15 @@
 
     def provide(self):
         """Make resource available so it would be immediately used."""
         if self._available:
             return
         assert self.name, 'Resource should be named'
         assert self.version, 'Resource should be versioned'
-        with lock(self.path):
+        with self.lock:
             if self.version in self.get_available_versions():
                 self._available = True
                 return
             self.deploy()
             self._available = True
 
     def __call__(self):
@@ -169,15 +184,15 @@
             temp_path.rename(self.path)
         except Exception:
             if temp_path and temp_path.is_dir():
                 shutil.rmtree(str(temp_path))
             raise
 
     def cleanup(self):
-        with lock(self.path):
+        with self.lock:
             if self.path.is_dir():
                 info('Cleanup %s', self.path)
                 shutil.rmtree(str(self.path))
             self._available = False
 
 
 class ArchiveExtractor:
```

### Comparing `getpack-0.2.4/src/getpack.egg-info/PKG-INFO` & `getpack-0.2.5/src/getpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Description: ### Declarative external resources any with implicit deployment
```

### Comparing `getpack-0.2.4/tests/test_common.py` & `getpack-0.2.5/tests/test_common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from getpack import  library, resource
 
 
-def test_cefpython3():
+def test_cefpython3(temp_folder):
     cefpython3 = resource.WebPackage(
         name='cefpython3',
         archive_url=(
             'https://files.pythonhosted.org/packages/3b/d4/f313221a999e4d295'
             'cc8fcb15fc4ac9c98f6759e50735d6f6ce84fd3e98a/'
             'cefpython3-66.1-py2.py3-none-win_amd64.whl'),
         version='66.1',
+        local_base=temp_folder,
     )
     assert cefpython3().__version__ == cefpython3.version
     assert '66.1' in cefpython3.get_available_versions()
 
 
 def test_pyside2():
     PySide2 = library.PySide2()
     PySide2.cleanup()
     assert PySide2().__version__ == PySide2.version
 
 
-def test_cefpython3_pypi():
-    cefpython3 = library.cefpython3()
+def test_cefpython3_pypi(temp_folder):
+    cefpython3 = library.CefPython3(local_base=temp_folder)
     assert not cefpython3._activated
     cefpython3.cleanup()
     assert not cefpython3._activated
     assert cefpython3().__version__ == cefpython3.version
     assert cefpython3._activated
 
 
@@ -35,7 +36,12 @@
     assert not blender._available, (
         'Blender resource is not initialized and could not have _available '
         'flag set')
     blender.cleanup()
     blender.provide()
     output = blender('--version')
     assert version in output.decode()
+
+
+def test_parent_folders_exists(temp_folder):
+    python = library.Python(local_base=temp_folder)
+    assert python.version.encode() in python('--version')
```

