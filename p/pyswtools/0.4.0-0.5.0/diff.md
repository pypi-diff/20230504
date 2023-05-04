# Comparing `tmp/pyswtools-0.4.0.tar.gz` & `tmp/pyswtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswtools-0.4.0.tar", max compression
+gzip compressed data, was "pyswtools-0.5.0.tar", max compression
```

## Comparing `pyswtools-0.4.0.tar` & `pyswtools-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     2687 2023-05-04 11:45:48.133287 pyswtools-0.4.0/README.md
--rw-r--r--   0        0        0      786 2023-05-04 11:48:13.765655 pyswtools-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.4.0/pyswtools/__init__.py
--rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.4.0/pyswtools/config.py
--rw-r--r--   0        0        0     1807 2023-05-04 11:45:48.133287 pyswtools-0.4.0/pyswtools/copy_full_assembly/main.py
--rw-r--r--   0        0        0      664 2023-05-04 11:50:26.339192 pyswtools-0.4.0/pyswtools/main.py
--rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.4.0/pyswtools/ready_dxf/__init__.py
--rw-r--r--   0        0        0     1326 2023-05-03 13:47:31.066860 pyswtools-0.4.0/pyswtools/ready_dxf/dxf_utilities.py
--rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.4.0/pyswtools/ready_dxf/file_utilities.py
--rw-r--r--   0        0        0      502 2023-05-03 13:47:31.058860 pyswtools-0.4.0/pyswtools/ready_dxf/main.py
--rw-r--r--   0        0        0      454 2023-05-04 08:29:48.610745 pyswtools-0.4.0/pyswtools/utils.py
--rw-r--r--   0        0        0     3526 1970-01-01 00:00:00.000000 pyswtools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3604 2023-05-04 20:45:17.566358 pyswtools-0.5.0/README.md
+-rw-r--r--   0        0        0      807 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.5.0/pyswtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/auto_exporter/__init__.py
+-rw-r--r--   0        0        0     5406 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/auto_exporter/main.py
+-rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.5.0/pyswtools/config.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/copy_full_assembly/__init__.py
+-rw-r--r--   0        0        0     1807 2023-05-04 15:28:13.720447 pyswtools-0.5.0/pyswtools/copy_full_assembly/main.py
+-rw-r--r--   0        0        0      737 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/main.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.5.0/pyswtools/ready_dxf/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-03 13:47:31.066860 pyswtools-0.5.0/pyswtools/ready_dxf/dxf_utilities.py
+-rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.5.0/pyswtools/ready_dxf/file_utilities.py
+-rw-r--r--   0        0        0      502 2023-05-03 13:47:31.058860 pyswtools-0.5.0/pyswtools/ready_dxf/main.py
+-rw-r--r--   0        0        0      454 2023-05-04 08:29:48.610745 pyswtools-0.5.0/pyswtools/utils.py
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 pyswtools-0.5.0/PKG-INFO
```

### Comparing `pyswtools-0.4.0/pyproject.toml` & `pyswtools-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyswtools"
-version = "0.4.0"
+version = "0.5.0"
 description = "Set of tools to improve Solidworks usage"
 authors = ["ldevillez <louis.devillez@gmail.com>"]
 license = "GNU General Public License"
 readme = "README.md"
 homepage = "https://github.com/ldevillez/pySwTools"
 repository = "https://github.com/ldevillez/pySwTools"
 
@@ -16,14 +16,15 @@
 python = "^3.10"
 ezdxf = "^1.0.3"
 click = "^8.1.3"
 pywin32 = { version = "^306", markers = "sys_platform == 'win32'" }
 rtoml = "^0.9.0"
 appdirs = "^1.4.4"
 pydantic = "^1.10.7"
+numpy-stl = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pylint= "^2.16.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyswtools-0.4.0/pyswtools/config.py` & `pyswtools-0.5.0/pyswtools/config.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.4.0/pyswtools/copy_full_assembly/main.py` & `pyswtools-0.5.0/pyswtools/copy_full_assembly/main.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.4.0/pyswtools/main.py` & `pyswtools-0.5.0/pyswtools/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 """
 
 import click
 
 from .config import config
 from .ready_dxf.main import ready_dxf
 from .copy_full_assembly.main import copy_full_assembly
+from .auto_exporter.main import auto_export
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "Devillez Louis"
 __maintainer__ = "Deville Louis"
 __email__ = "louis.devillez@gmail.com"
 
 
 @click.group()
 @click.version_option(__version__, "-v", "--version")
@@ -23,10 +24,11 @@
     Combination of commands to help you work with solidworks
     """
 
 
 cli.add_command(config)
 cli.add_command(ready_dxf)
 cli.add_command(copy_full_assembly)
+cli.add_command(auto_export)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pyswtools-0.4.0/pyswtools/ready_dxf/dxf_utilities.py` & `pyswtools-0.5.0/pyswtools/ready_dxf/dxf_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.4.0/pyswtools/ready_dxf/file_utilities.py` & `pyswtools-0.5.0/pyswtools/ready_dxf/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.4.0/PKG-INFO` & `pyswtools-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pyswtools
-Version: 0.4.0
-Summary: Set of tools to improve Solidworks usage
-Home-page: https://github.com/ldevillez/pySwTools
-License: GNU General Public License
-Author: ldevillez
-Author-email: louis.devillez@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: ezdxf (>=1.0.3,<2.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pywin32 (>=306,<307) ; sys_platform == "win32"
-Requires-Dist: rtoml (>=0.9.0,<0.10.0)
-Project-URL: Repository, https://github.com/ldevillez/pySwTools
-Description-Content-Type: text/markdown
-
 # pySwTools
 
 pySwTools is a combination of tools that I made to help me with my workflow when working with Solidworks. Sometimes it is not directly link to SW but more to what I do with the CAD models.
 
 ## Installation
 
 You can directly install it from pypi:
@@ -37,15 +15,19 @@
 ```
 
 If you are on windows, maybe the directory where the script is installed will not be on the PATH but it can be added to directly be able to use the script from a command prompt.
 
 
 ## Contributing
 
-If you found a bug or if you have any idea for the project feel free to open a new issue on github ! And if you want to directly contribute, you are welcome
+If you found a bug or if you have any idea for the project feel free to open a new issue on github ! And if you want to directly contribute, you are welcome.
+
+List of ressources that can be helpful when starting with the solidworks API:
+- [https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1](Solidworks API)
+- [https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf](Python examples)
 
 ## List of modules
 
 ### CLI
 It is the main module of this project. It allows you to select the actions that you want to apply. To directly get help from the tool simply type:
 ```
 pyswtools
@@ -73,15 +55,15 @@
 ```
 Or the path to the current config:
 ```
 pyswtools config dump --path
 ```
 
 
-### Ready_DXF
+### Ready-dxf
 Prepare dxf files from solidworks to be laser cutted:
 - Remove the solidworks text from the output dxf file
 
 #### How to use
 You can use the following command:
 ```
 pyswtools ready-dxf /path/to/file.dxf
@@ -99,23 +81,39 @@
 
 #### Features to come
 - [ ] Combine Lines
 - [ ] Combine Files
 - [ ] Add auto coloring
 - [ ] Add tests
 
-### Copy_full_assembly
+### Copy-full-assembly
 This tool help you when copying multiple file or assembly. It will help you by updating path reference to new path reference:
 - In the equation manager
 #### How to use
 ```
 pyswtools copy-full-assembly PATH_TO_DIR SRC_REPLACE TARGET_REPLACE
 ```
 - `PATH_TO_DIR` is the path to directory with all the files to update
 - `SRC_REPLACE` is the string in the current path reference that you want to replace (probably the name of the old directory)
 - `TARGET_REPLACE` is the string in the current path reference that you want to replace (probably the name of the new directory)
 
-### Exports_to_STL
-- [ ] To migrate
-### Exports_to_dxf
-- [ ] To migrate
+### Auto-export
+
+This tool help you export a directory (or a part) to other file extensions. The current exrports are:
+- DXF
+- STL
+- Auto
+
+The Auto mode will use the name of the part and see if an extension is specified in it (e.g. `DXF_my_part.SLDPRT`)
+
+The DXF export will only work when there is only one body in the part. Also the face that will be exported is a planar one with the biggest surface.
+
+The STL export will consider the z axis as being the vertical dimension.
+
+#### How to use
+
+
+```
+pyswtools auto-export PATH/TO/DIR MODE
+```
 
+With `Mode` being `AUTO`, `DXF` or `STL`. It will create directory with the extension used  and the corresponding files in it.
```

