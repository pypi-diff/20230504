# Comparing `tmp/pf_fpga_tools-0.0.2.tar.gz` & `tmp/pf_fpga_tools-0.0.3.tar.gz`

## Comparing `pf_fpga_tools-0.0.2.tar` & `pf_fpga_tools-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/.flake8
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/__about__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/exceptions.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pffpgatools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/README.md
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/.flake8
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/exceptions.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/README.md
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/utils.py` & `pf_fpga_tools-0.0.3/pffpgatools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/pfBuildCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
                 print(self.packagedFilename())
                 sys.exit(0)
             elif print_bitstream_file is True:
                 print(self.bitstreamFile())
                 sys.exit(0)
 
             self.destination_folder: str = arguments[1]
+            self.core_folder = os.path.join(self.destination_folder, '_core')
 
             self.dependency_count = 0
 
         except getopt.GetoptError:
             print('Unknown option or argument. Maybe start with `pfBuildCore --help?')
             sys.exit(0)
 
@@ -224,24 +225,25 @@
         self.addDependency(dep_file, src_image_file)
 
     def outputFilename(self):
         return os.path.join(self.destination_folder, self.packagedFilename())
 
     def packageCore(self):
         deps = []
-        packaged_filename = self.packagedFilename()
+        packaged_filename = os.path.join('..', self.packagedFilename())
 
         arguments: List[str] = ['zip', '-r', packaged_filename]
-        for p in Path(self.destination_folder).rglob('*'):
-            extension = p.suffix
-            if not os.path.isdir(p) and not extension == '.zip' and not extension == '.d':
-                arguments.append(str(p.relative_to(self.destination_folder)))
-                deps.append(str(p))
+        for p in Path(self.core_folder).rglob('*'):
+            if os.path.isdir(p):
+                continue
 
-        Utils.shellCommand(arguments, from_dir=self.destination_folder)
+            arguments.append(str(p.relative_to(self.core_folder)))
+            deps.append(str(p))
+
+        Utils.shellCommand(arguments, from_dir=self.core_folder)
 
     def addDependency(self, dep_file, dep):
         if self.dependency_count == 0:
             output_filename = os.path.join(self.destination_folder, self.packagedFilename())
             dep_file.write('%s: %s' % (output_filename.replace(' ', '\\ '), self.config_filename))
 
         dep_file.write(' \\\n %s' % (dep))
@@ -254,27 +256,27 @@
     def packagedFilename(self) -> str:
         return '%s-%s-%s.zip' % (self.fullPlatformName(), self.getConfigParam('Build', 'version'), self.today)
 
     def bitstreamFile(self) -> str:
         return os.path.expandvars(self.getConfigParam('Bitstream', 'source'))
 
     def main(self) -> None:
-        os.makedirs(self.destination_folder, exist_ok=True)
+        os.makedirs(self.core_folder, exist_ok=True)
 
         full_platform_name = self.fullPlatformName()
-        cores_folder = os.path.join(self.destination_folder, 'Cores', full_platform_name)
+        cores_folder = os.path.join(self.core_folder, 'Cores', full_platform_name)
         os.makedirs(cores_folder, exist_ok=True)
 
-        platforms_folder = os.path.join(self.destination_folder, 'Platforms')
+        platforms_folder = os.path.join(self.core_folder, 'Platforms')
         os.makedirs(platforms_folder, exist_ok=True)
 
         platforms_image_folder = os.path.join(platforms_folder, '_images')
         os.makedirs(platforms_image_folder, exist_ok=True)
 
-        dependency_filename = os.path.join(self.destination_folder, 'deps.d')
+        dependency_filename = os.path.join(self.core_folder, 'deps.d')
         with open(dependency_filename, 'w') as dep_file:
             print('Building bitstream file...')
             bitstream_source = self.bitstreamFile()
             bitstream_dest = os.path.join(cores_folder, '%s.rbf_r' % (self.getConfigParam('Platform', 'short_name')))
             Utils.shellCommand(['pfReverseBitstream', bitstream_source, bitstream_dest])
 
             self.addDependency(dep_file, bitstream_source)
```

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/pfConvertImage.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfInstallCore/pfInstallCore.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/pfInstallCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/pffpgatools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/LICENSE` & `pf_fpga_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.2/README.md` & `pf_fpga_tools-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,34 +10,45 @@
 
 -----
 
 ### Installation
 
 **pf-fpga-tools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
-You will also need following dependencies via [brew](https://brew.sh):
+You can then install **pf-fpga-tools** by typing the following in a terminal window:
 ```console
-brew install imagemagick
+pip install pf-fpga-tools
 ```
 
-You can then install **pf-fpga-tools** by typing the following in a terminal window:
+### Installation (macOS)
+
+Also install the following tool dependencies via [brew](https://brew.sh):
 ```console
-pip install pf-fpga-tools
+brew install imagemagick
+```
+
+### Installation (Ubuntu Linux)
+
+Also install the following tool dependencies:
+```
+sudo apt install imagemagick
 ```
 
 ### Usage
 
 **pf-fpga-tools** provides the follow commands commands, sometimes with one or two extra arguments:
 
 - `pfBuildCore` - Build a core according to a `toml` config file.
 
 - `pfInstallCore` - Install a zipped up core file onto a given volume.
 
 - `pfConvertImage` - Convert an image for to the binary format used by the **Analog Pocket** for its cores and platform lists.
 
-- `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbd_r` reversed bitstream.
+- `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbf_r` reversed bitstream.
+
+- `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
 You can use the `--help` argument to get some usage info for each command.
 
 ### License
 
 **pf-fpga-tools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

### Comparing `pf_fpga_tools-0.0.2/pyproject.toml` & `pf_fpga_tools-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -50,7 +50,8 @@
 ]
 
 [project.scripts]
 pfBuildCore = "pffpgatools.pfBuildCore.__main__:main"
 pfConvertImage = "pffpgatools.pfConvertImage.__main__:main"
 pfInstallCore = "pffpgatools.pfInstallCore.__main__:main"
 pfReverseBitstream = "pffpgatools.pfReverseBitstream.__main__:main"
+pfCloneCoreTemplate = "pffpgatools.pfCloneCoreTemplate.__main__:main"
```

### Comparing `pf_fpga_tools-0.0.2/PKG-INFO` & `pf_fpga_tools-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pf-fpga-tools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pf-fpga-tools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pf-fpga-tools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -35,34 +35,45 @@
 
 -----
 
 ### Installation
 
 **pf-fpga-tools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
-You will also need following dependencies via [brew](https://brew.sh):
+You can then install **pf-fpga-tools** by typing the following in a terminal window:
 ```console
-brew install imagemagick
+pip install pf-fpga-tools
 ```
 
-You can then install **pf-fpga-tools** by typing the following in a terminal window:
+### Installation (macOS)
+
+Also install the following tool dependencies via [brew](https://brew.sh):
 ```console
-pip install pf-fpga-tools
+brew install imagemagick
+```
+
+### Installation (Ubuntu Linux)
+
+Also install the following tool dependencies:
+```
+sudo apt install imagemagick
 ```
 
 ### Usage
 
 **pf-fpga-tools** provides the follow commands commands, sometimes with one or two extra arguments:
 
 - `pfBuildCore` - Build a core according to a `toml` config file.
 
 - `pfInstallCore` - Install a zipped up core file onto a given volume.
 
 - `pfConvertImage` - Convert an image for to the binary format used by the **Analog Pocket** for its cores and platform lists.
 
-- `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbd_r` reversed bitstream.
+- `pfReverseBitstream` - Converts an `rbf` bitstream file into an `rbf_r` reversed bitstream.
+
+- `pfCloneCoreTemplate` - Clone the core dev template from Github.
 
 You can use the `--help` argument to get some usage info for each command.
 
 ### License
 
 **pf-fpga-tools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

