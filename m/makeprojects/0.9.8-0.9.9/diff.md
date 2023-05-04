# Comparing `tmp/makeprojects-0.9.8.tar.gz` & `tmp/makeprojects-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\makeprojects-0.9.8.tar", last modified: Tue Jul  9 07:22:49 2019, max compression
+gzip compressed data, was "dist\makeprojects-0.9.9.tar", last modified: Sun Aug 11 22:54:20 2019, max compression
```

## Comparing `makeprojects-0.9.8.tar` & `makeprojects-0.9.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2019-07-09 07:22:49.000000 makeprojects-0.9.8/
--rw-rw-rw-   0        0        0     3494 2019-07-09 07:22:49.000000 makeprojects-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2019-04-28 07:34:54.000000 makeprojects-0.9.8/README.rst
-drwxrwxrwx   0        0        0        0 2019-07-09 07:22:49.000000 makeprojects-0.9.8/makeprojects/
--rw-rw-rw-   0        0        0     7313 2019-07-04 17:46:15.000000 makeprojects-0.9.8/makeprojects/__init__.py
--rw-rw-rw-   0        0        0    15026 2019-06-04 02:51:34.000000 makeprojects-0.9.8/makeprojects/__main__.py
--rw-rw-rw-   0        0        0      867 2019-06-13 06:43:09.000000 makeprojects-0.9.8/makeprojects/__pkginfo__.py
--rw-rw-rw-   0        0        0    10908 2019-07-03 05:55:01.000000 makeprojects-0.9.8/makeprojects/build_rules.py
--rw-rw-rw-   0        0        0    53119 2019-06-13 05:39:22.000000 makeprojects-0.9.8/makeprojects/buildme.py
--rw-rw-rw-   0        0        0     9489 2019-06-02 01:23:48.000000 makeprojects-0.9.8/makeprojects/cleanme.py
--rw-rw-rw-   0        0        0     8161 2019-06-26 07:08:11.000000 makeprojects-0.9.8/makeprojects/codeblocks.py
--rw-rw-rw-   0        0        0    38549 2019-07-03 05:50:51.000000 makeprojects-0.9.8/makeprojects/codewarrior.py
--rw-rw-rw-   0        0        0     4881 2019-06-02 01:23:46.000000 makeprojects-0.9.8/makeprojects/config.py
--rw-rw-rw-   0        0        0    38020 2019-07-06 20:15:38.000000 makeprojects-0.9.8/makeprojects/core.py
--rw-rw-rw-   0        0        0    11486 2019-06-25 07:29:14.000000 makeprojects-0.9.8/makeprojects/defaults.py
--rw-rw-rw-   0        0        0    41481 2019-07-08 07:07:12.000000 makeprojects-0.9.8/makeprojects/enums.py
--rw-rw-rw-   0        0        0     1414 2019-07-07 20:04:51.000000 makeprojects-0.9.8/makeprojects/glsl_support.py
--rw-rw-rw-   0        0        0     5169 2019-07-07 18:51:52.000000 makeprojects-0.9.8/makeprojects/hlsl_support.py
--rw-rw-rw-   0        0        0    20045 2019-07-03 05:50:17.000000 makeprojects-0.9.8/makeprojects/makefile.py
--rw-rw-rw-   0        0        0     4958 2019-06-02 01:23:49.000000 makeprojects-0.9.8/makeprojects/rebuildme.py
--rw-rw-rw-   0        0        0    16976 2019-07-07 18:52:47.000000 makeprojects-0.9.8/makeprojects/validators.py
--rw-rw-rw-   0        0        0   129086 2019-07-09 07:15:06.000000 makeprojects-0.9.8/makeprojects/visual_studio.py
--rw-rw-rw-   0        0        0    59817 2019-07-08 07:22:53.000000 makeprojects-0.9.8/makeprojects/visual_studio_2010.py
--rw-rw-rw-   0        0        0    22415 2019-07-03 05:50:17.000000 makeprojects-0.9.8/makeprojects/watcom.py
--rw-rw-rw-   0        0        0    50102 2019-06-26 07:44:20.000000 makeprojects-0.9.8/makeprojects/xcode.py
-drwxrwxrwx   0        0        0        0 2019-07-09 07:22:49.000000 makeprojects-0.9.8/makeprojects.egg-info/
--rw-rw-rw-   0        0        0     3494 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-07-09 07:22:42.000000 makeprojects-0.9.8/makeprojects.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2019-07-09 07:22:48.000000 makeprojects-0.9.8/makeprojects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-07-09 07:22:49.000000 makeprojects-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     5374 2019-06-30 23:46:54.000000 makeprojects-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-08-11 22:54:20.000000 makeprojects-0.9.9/
+-rw-rw-rw-   0        0        0     3494 2019-08-11 22:54:20.000000 makeprojects-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2019-04-28 07:34:54.000000 makeprojects-0.9.9/README.rst
+drwxrwxrwx   0        0        0        0 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects/
+-rw-rw-rw-   0        0        0     7313 2019-07-04 17:46:15.000000 makeprojects-0.9.9/makeprojects/__init__.py
+-rw-rw-rw-   0        0        0    15026 2019-06-04 02:51:34.000000 makeprojects-0.9.9/makeprojects/__main__.py
+-rw-rw-rw-   0        0        0      867 2019-08-11 22:16:16.000000 makeprojects-0.9.9/makeprojects/__pkginfo__.py
+-rw-rw-rw-   0        0        0    11314 2019-08-11 20:56:45.000000 makeprojects-0.9.9/makeprojects/build_rules.py
+-rw-rw-rw-   0        0        0    53119 2019-06-13 05:39:22.000000 makeprojects-0.9.9/makeprojects/buildme.py
+-rw-rw-rw-   0        0        0     9489 2019-06-02 01:23:48.000000 makeprojects-0.9.9/makeprojects/cleanme.py
+-rw-rw-rw-   0        0        0     8161 2019-06-26 07:08:11.000000 makeprojects-0.9.9/makeprojects/codeblocks.py
+-rw-rw-rw-   0        0        0    37983 2019-08-11 21:52:02.000000 makeprojects-0.9.9/makeprojects/codewarrior.py
+-rw-rw-rw-   0        0        0     4881 2019-06-02 01:23:46.000000 makeprojects-0.9.9/makeprojects/config.py
+-rw-rw-rw-   0        0        0    39851 2019-08-11 01:43:06.000000 makeprojects-0.9.9/makeprojects/core.py
+-rw-rw-rw-   0        0        0    11486 2019-06-25 07:29:14.000000 makeprojects-0.9.9/makeprojects/defaults.py
+-rw-rw-rw-   0        0        0    41481 2019-07-08 07:07:12.000000 makeprojects-0.9.9/makeprojects/enums.py
+-rw-rw-rw-   0        0        0     1414 2019-07-07 20:04:51.000000 makeprojects-0.9.9/makeprojects/glsl_support.py
+-rw-rw-rw-   0        0        0     5169 2019-07-07 18:51:52.000000 makeprojects-0.9.9/makeprojects/hlsl_support.py
+-rw-rw-rw-   0        0        0    20441 2019-07-14 05:50:52.000000 makeprojects-0.9.9/makeprojects/makefile.py
+-rw-rw-rw-   0        0        0     4958 2019-06-02 01:23:49.000000 makeprojects-0.9.9/makeprojects/rebuildme.py
+-rw-rw-rw-   0        0        0    16976 2019-07-07 18:52:47.000000 makeprojects-0.9.9/makeprojects/validators.py
+-rw-rw-rw-   0        0        0   128994 2019-07-15 02:28:39.000000 makeprojects-0.9.9/makeprojects/visual_studio.py
+-rw-rw-rw-   0        0        0    59505 2019-08-05 00:04:24.000000 makeprojects-0.9.9/makeprojects/visual_studio_2010.py
+-rw-rw-rw-   0        0        0    22908 2019-08-11 01:07:12.000000 makeprojects-0.9.9/makeprojects/watcom.py
+-rw-rw-rw-   0        0        0    51482 2019-07-14 01:22:45.000000 makeprojects-0.9.9/makeprojects/xcode.py
+drwxrwxrwx   0        0        0        0 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/
+-rw-rw-rw-   0        0        0     3494 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2019-08-11 22:54:12.000000 makeprojects-0.9.9/makeprojects.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2019-08-11 22:54:20.000000 makeprojects-0.9.9/makeprojects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2019-08-11 22:54:20.000000 makeprojects-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     5374 2019-08-11 22:08:14.000000 makeprojects-0.9.9/setup.py
```

### Comparing `makeprojects-0.9.8/PKG-INFO` & `makeprojects-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: makeprojects
-Version: 0.9.8
+Version: 0.9.9
 Summary: IDE project generator for Visual Studio, XCode, etc...
 Home-page: http://makeprojects.readthedocs.io
 Author: Rebecca Ann Heineman <becky@burgerbecky.com>
 Author-email: becky@burgerbecky.com
 License: MIT License
 Description: =======================
         Makeprojects for Python
```

### Comparing `makeprojects-0.9.8/README.rst` & `makeprojects-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/__init__.py` & `makeprojects-0.9.9/makeprojects/__init__.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/__main__.py` & `makeprojects-0.9.9/makeprojects/__main__.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/__pkginfo__.py` & `makeprojects-0.9.9/makeprojects/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 ## \package makeprojects.__pkginfo__
 
 from __future__ import unicode_literals
 
 ## Numeric version
-NUMVERSION = (0, 9, 8)
+NUMVERSION = (0, 9, 9)
 
 ## String version
 VERSION = '.'.join([str(num) for num in NUMVERSION])
 
 ## Author's name
 AUTHOR = 'Rebecca Ann Heineman <becky@burgerbecky.com>'
```

### Comparing `makeprojects-0.9.8/makeprojects/build_rules.py` & `makeprojects-0.9.9/makeprojects/build_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,39 @@
         configuration: Configuration record to update.
     """
 
     # Too many branches
     # Too many statements
     # pylint: disable=R0912,R0915
 
+    ide = configuration.project.ide
     define_list = []
     libraries_list = []
 
     # Debug/Release
     if configuration.debug:
         define_list.append('_DEBUG')
     else:
         define_list.append('NDEBUG')
 
     # Sanity check for missing platform
     platform = configuration.platform
     if platform is not None:
+
         # Windows specific defines
         if platform.is_windows():
+
+            if ide.is_codewarrior():
+                configuration.library_folders_list = [
+                    '$(CodeWarrior)/MSL', '$(CodeWarrior)/Win32-x86 Support']
+                if configuration.debug:
+                    libraries_list.append('MSL_All_x86_D.lib')
+                else:
+                    libraries_list.append('MSL_All_x86.lib')
+
             libraries_list.extend(
                 ['Kernel32.lib', 'Gdi32.lib', 'Shell32.lib', 'Ole32.lib',
                  'User32.lib', 'Advapi32.lib', 'version.lib', 'Ws2_32.lib',
                  'Comctl32.lib'])
 
             define_list.extend(['_WINDOWS', 'WIN32_LEAN_AND_MEAN'])
             if platform in (PlatformTypes.win64,
```

### Comparing `makeprojects-0.9.8/makeprojects/buildme.py` & `makeprojects-0.9.9/makeprojects/buildme.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/cleanme.py` & `makeprojects-0.9.9/makeprojects/cleanme.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/codeblocks.py` & `makeprojects-0.9.9/makeprojects/codeblocks.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/config.py` & `makeprojects-0.9.9/makeprojects/config.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/core.py` & `makeprojects-0.9.9/makeprojects/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from operator import attrgetter
 from copy import deepcopy
 from burger import get_windows_host_type, convert_to_windows_slashes, \
     convert_to_linux_slashes, is_string, translate_to_regex_match, \
     string_to_bool, StringListProperty, BooleanProperty, NoneProperty
 
 from .enums import FileTypes, ProjectTypes, IDETypes, PlatformTypes
+from .enums import platformtype_short_code
 from .build_rules import rules as default_rules
 
-
 ########################################
 
 
 def validate_enum_type(value, data_type):
     """
     Verify a value is a specific data type.
 
@@ -178,14 +178,17 @@
 
     ## List of file patterns to exclude from this configuration
     exclude_from_build_list = StringListProperty('_exclude_from_build_list')
 
     ## List of files to exclude from directory scanning
     exclude_list = StringListProperty('_exclude_list')
 
+    ## List of CodeWarrior environment variables
+    cw_environment_variables = StringListProperty('_cw_environment_variables')
+
     def __init__(self, **kargs):
         """
         Perform initialization that's common to all parts.
 
         Args:
             kargs: List of defaults.
         """
@@ -625,14 +628,15 @@
 
     ## Don't allow Visual Studio targets files
     vs_targets = NoneProperty('_vs_targets')
 
     ## Don't allow Visual Studio rules files
     vs_rules = NoneProperty('_vs_rules')
 
+
     def __init__(self, **kargs):
         """
         Init defaults.
 
         Args:
             kargs: List of defaults.
         """
@@ -645,14 +649,15 @@
 
         # Init the base class
         Attributes.__init__(self, **kargs)
 
         ## Project this Configuration is attached to.
         self.project = None
 
+
     ########################################
 
     # Attribute defined outside __init__
     # pylint: disable=W0201
 
     @property
     def ide(self):
@@ -819,14 +824,17 @@
 
         ## Used by scan_directory
         self.file_list = None
 
         ## Used by scan_directory
         self.include_list = None
 
+        ## Platform code for generation
+        self.platform_code = ''
+
     ########################################
 
     @property
     def ide(self):
         """
         Return the preferred IDE
         """
@@ -1139,14 +1147,20 @@
         # Set a default project type
         if self.project_type is None:
             self.project_type = ProjectTypes.default()
 
         ## Initial array of Project records for projects
         self.project_list = []
 
+        ## IDE code for generation
+        self.ide_code = ''
+
+        ## Platform code for generation
+        self.platform_code = ''
+
     ########################################
 
     @property
     def ide(self):
         """
         Return the ide type
         """
@@ -1190,49 +1204,92 @@
         """
         Generate a project file and write it out to disk.
         """
 
         # Work from a copy to ensure the original is not touched.
         solution = deepcopy(self)
 
+        # If an ide was passed, check it, otherwise assume
+        # solution.ide is valid
+        if ide is not None:
+            # Note, this will throw if IDE is not an IDE value
+            solution.ide = ide
+
+            # Grab the value back if there was conversion
+            ide = solution.ide
+
+        # Set the default IDE to whatever the system uses
+        if ide is None:
+            ide = IDETypes.default()
+            solution.ide = ide
+
+        # Determine which generator to use based on the selected IDE
+
+        import makeprojects.watcom
+        import makeprojects.makefile
+        import makeprojects.visual_studio
+        import makeprojects.visual_studio_2010
+        import makeprojects.codewarrior
+        import makeprojects.xcode
+
+        generator_list = (
+            makeprojects.visual_studio,
+            makeprojects.visual_studio_2010,
+            makeprojects.watcom,
+            makeprojects.makefile,
+            makeprojects.codewarrior,
+            makeprojects.xcode)
+        for generator in generator_list:
+            if ide in generator.SUPPORTED_IDES:
+                break
+        else:
+            print('IDE {} is not supported.'.format(ide))
+            return 10
+
+        # Convert keys that need to be regexes from *.cpp to regex
         solution.custom_rules = regex_dict(solution.custom_rules)
 
-        # Sort the configuration/platforms to ensure diffs are minimized
+        all_configurations_list = []
+
+        # Process all the projects and configurations
         for project in solution.project_list:
+
+            # Handle projects
             project.custom_rules = regex_dict(project.custom_rules)
 
-            project.configuration_list = sorted(
-                project.configuration_list, key=lambda x: (
+            # Purge unsupported configurations
+            configuration_list = []
+            for configuration in project.configuration_list:
+                if generator.test(ide, configuration.platform):
+                    configuration_list.append(configuration)
+
+            # Sort the configurations to ensure consistency
+            configuration_list = sorted(
+                configuration_list, key=lambda x: (
                     x.name, x.platform))
+            project.configuration_list = configuration_list
+            all_configurations_list.extend(configuration_list)
+            project.platform_code = platformtype_short_code(configuration_list)
 
-            for configuration in project.configuration_list:
+            # Handle regexes for configurations that will be used
+            for configuration in configuration_list:
                 configuration.custom_rules = regex_dict(
                     configuration.custom_rules)
                 configuration.exclude_list_regex = translate_to_regex_match(
                     configuration.exclude_list)
 
-        # If ide was passed, check it, otherwise assume
-        # solution.ide is valid
-        if ide is not None:
-            if not isinstance(ide, IDETypes):
-                raise TypeError("parameter 'ide' must be of type IDETypes")
-            solution.ide = ide
+        # Get the platform code
+        solution.platform_code = platformtype_short_code(
+            all_configurations_list)
+
+        # Set the IDE code
+        solution.ide_code = ide.get_short_code()
 
-        # Create Visual Studio files
-        if ide.is_visual_studio():
-            if ide < IDETypes.vs2010:
-                from .visual_studio import generate as vs_generate
-                return vs_generate(solution)
-            from .visual_studio_2010 import generate as vs_generate2010
-            return vs_generate2010(solution)
-        # Create Codewarrior files
-        if ide.is_codewarrior():
-            from .codewarrior import generate as cw_generate
-            return cw_generate(solution)
-        return 10
+        # Create project files
+        return generator.generate(solution)
 
     def __repr__(self):
         """
         Convert the solultion record into a human readable description
 
         Returns:
             Human readable string or None if the solution is invalid
```

### Comparing `makeprojects-0.9.8/makeprojects/defaults.py` & `makeprojects-0.9.9/makeprojects/defaults.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/enums.py` & `makeprojects-0.9.9/makeprojects/enums.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/glsl_support.py` & `makeprojects-0.9.9/makeprojects/glsl_support.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/hlsl_support.py` & `makeprojects-0.9.9/makeprojects/hlsl_support.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/makefile.py` & `makeprojects-0.9.9/makeprojects/makefile.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,37 @@
 # project files intended for use by make
 #
 
 from __future__ import absolute_import, print_function, unicode_literals
 import os
 from io import StringIO
 import burger
-from makeprojects import FileTypes, ProjectTypes, PlatformTypes
+from makeprojects import FileTypes, ProjectTypes, PlatformTypes, IDETypes
 
 # pylint: disable=C0302
 
+SUPPORTED_IDES = (IDETypes.make,)
+
+########################################
+
+
+def test(ide, platform_type):
+    """ Filter for supported platforms
+
+    Args:
+        ide: IDETypes
+        platform_type: PlatformTypes
+    Returns:
+        True if supported, False if not
+    """
+
+    # pylint: disable=unused-argument
+
+    return platform_type is PlatformTypes.linux
+
 #
 ## \package makeprojects.makefile
 # This module contains classes needed to generate
 # project files intended for use by GNU make
 #
 
 ## Array of targets that Watcom can build
```

### Comparing `makeprojects-0.9.8/makeprojects/rebuildme.py` & `makeprojects-0.9.9/makeprojects/rebuildme.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/validators.py` & `makeprojects-0.9.9/makeprojects/validators.py`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/makeprojects/visual_studio.py` & `makeprojects-0.9.9/makeprojects/visual_studio.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,46 @@
 from uuid import NAMESPACE_DNS, UUID
 from hashlib import md5
 from burger import save_text_file_if_newer, convert_to_windows_slashes, \
     escape_xml_cdata, escape_xml_attribute, is_string
 
 from .validators import BooleanProperty, StringProperty, EnumProperty, \
     StringListProperty, IntegerProperty
-from .enums import platformtype_short_code
 from .enums import FileTypes, ProjectTypes, IDETypes, PlatformTypes
 from .hlsl_support import HLSL_ENUMS, make_hlsl_command
 from .glsl_support import make_glsl_command
 
 # pylint: disable=invalid-name
 
+SUPPORTED_IDES = (IDETypes.vs2003, IDETypes.vs2005, IDETypes.vs2008)
+
+########################################
+
+
+def test(ide, platform_type):
+    """ Filter for supported platforms
+
+    Args:
+        ide: IDETypes
+        platform_type: PlatformTypes
+    Returns:
+        True if supported, False if not
+    """
+
+    # Windows 32 is always supported
+    if platform_type is PlatformTypes.win32:
+        return True
+
+    # Only vs 2003 supports xbox classic
+    if ide is IDETypes.vs2003:
+        return platform_type is PlatformTypes.xbox
+
+    # Only vs 2005 and 2008 support Windows 64
+    return platform_type is PlatformTypes.win64
+
 ########################################
 
 
 def convert_file_name_vs2010(item):
     """ Convert macros from to Visual Studio 2003-2008
     Args:
         item: Filename string
@@ -1401,14 +1426,20 @@
         # Windows doesn't support fat files, so deploy to different
         # folders for tools
         if project_type is ProjectTypes.tool:
             if platform is PlatformTypes.win32:
                 deploy_folder = deploy_folder + 'x86\\'
             elif platform is PlatformTypes.win64:
                 deploy_folder = deploy_folder + 'x64\\'
+            elif platform is PlatformTypes.winarm32:
+                deploy_folder = deploy_folder + 'arm\\'
+            elif platform is PlatformTypes.winarm64:
+                deploy_folder = deploy_folder + 'arm64\\'
+            elif platform is PlatformTypes.winitanium:
+                deploy_folder = deploy_folder + 'ia64\\'
 
     # Create the batch file
     # Make sure the destination directory is present
     command_list = ['mkdir "{}" 2>nul'.format(deploy_folder)]
 
     # Copy the executable
     command_list.extend(
@@ -4042,53 +4073,26 @@
     """
 
     # Too many branches
     # Too many locals
     # pylint: disable=R0912,R0914
 
     # Failsafe
-    if solution.ide not in (IDETypes.vs2003, IDETypes.vs2005, IDETypes.vs2008):
+    if solution.ide not in SUPPORTED_IDES:
         return 10
 
-    # Since Visual Studio 2003 and earlier doesn't support
-    # x64 build targets, remove them before invoking the
-    # XML generators
-
-    temp_list = [PlatformTypes.win32]
-    if solution.ide > IDETypes.vs2003:
-        temp_list.append(PlatformTypes.win64)
-
-    # Remove any targets that are not supported
-    # by Visual Studio 2003-2008
-    for project in solution.project_list:
-        configuration_list = []
-        for configuration in project.configuration_list:
-            if configuration.platform in temp_list:
-                configuration_list.append(configuration)
-        project.configuration_list = configuration_list
-
-    # Get the IDE name code
-    idecode = solution.ide.get_short_code()
-
-    # Get the platform code by scanning all project configurations
-    temp_list = []
-    for project in solution.project_list:
-        temp_list.extend(project.configuration_list)
-    platformcode = platformtype_short_code(temp_list)
-
     # For starters, generate the UUID and filenames for the solution file
     # for visual studio, since each solution and project file generate
     # seperately
 
     # Iterate over the project files and create the filenames
     for project in solution.project_list:
 
-        platformcode = platformtype_short_code(project.configuration_list)
         project.vs_output_filename = '{}{}{}.vcproj'.format(
-            project.name, idecode, platformcode)
+            project.name, solution.ide_code, project.platform_code)
         project.vs_uuid = get_uuid(project.vs_output_filename)
 
         for configuration in project.configuration_list:
             vs_platform = configuration.platform.get_vs_platform()[0]
             configuration.vs_platform = vs_platform
             configuration.vs_configuration_name = '{}|{}'.format(
                 configuration.name, vs_platform)
@@ -4100,15 +4104,15 @@
 
     # Get the output flags
     perforce = solution.perforce
     verbose = solution.verbose
 
     # Create the final filename for the Visual Studio Solution file
     solution_filename = '{}{}{}.sln'.format(
-        solution.name, idecode, platformcode)
+        solution.name, solution.ide_code, solution.platform_code)
 
     save_text_file_if_newer(
         os.path.join(solution.working_directory, solution_filename),
         solution_lines,
         bom=solution.ide != IDETypes.vs2003,
         perforce=perforce,
         verbose=verbose)
```

### Comparing `makeprojects-0.9.8/makeprojects/visual_studio_2010.py` & `makeprojects-0.9.9/makeprojects/visual_studio_2010.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,79 @@
 from __future__ import absolute_import, print_function, unicode_literals
 
 import os
 from burger import save_text_file_if_newer, convert_to_windows_slashes, \
     delete_file, escape_xml_cdata, escape_xml_attribute, \
     packed_paths, truefalse
 
-from .enums import platformtype_short_code
 from .enums import FileTypes, ProjectTypes, IDETypes, PlatformTypes
 from .core import source_file_filter
 from .visual_studio import get_uuid, create_deploy_script
 
+SUPPORTED_IDES = (
+    IDETypes.vs2010,
+    IDETypes.vs2012,
+    IDETypes.vs2013,
+    IDETypes.vs2015,
+    IDETypes.vs2017,
+    IDETypes.vs2019)
+
+########################################
+
+
+def test(ide, platform_type):
+    """ Filter for supported platforms
+
+    Args:
+        ide: IDETypes
+        platform_type: PlatformTypes
+    Returns:
+        True if supported, False if not
+    """
+
+    # pylint: disable=too-many-branches
+    # pylint: disable=too-many-return-statements
+
+    if platform_type in (PlatformTypes.win32, PlatformTypes.win64):
+        return True
+
+    if ide is IDETypes.vs2010:
+        if platform_type is PlatformTypes.xbox360:
+            return True
+
+    if ide >= IDETypes.vs2015:
+        if platform_type is PlatformTypes.xboxone:
+            return True
+
+    if ide < IDETypes.vs2017:
+        if platform_type in (PlatformTypes.ps3, PlatformTypes.vita):
+            return True
+
+    if ide >= IDETypes.vs2012:
+        if platform_type in (PlatformTypes.ps4, PlatformTypes.wiiu):
+            return True
+
+    if ide >= IDETypes.vs2013:
+        if platform_type in (PlatformTypes.tegra,
+                             PlatformTypes.androidarm32,
+                             PlatformTypes.androidarm64,
+                             PlatformTypes.androidintel32,
+                             PlatformTypes.androidintel64):
+            return True
+
+    if ide >= IDETypes.vs2015:
+        if platform_type is PlatformTypes.switch:
+            return True
+
+    if ide >= IDETypes.vs2017:
+        if platform_type in (PlatformTypes.winarm32, PlatformTypes.winarm64):
+            return True
+
+    return False
+
 
 ########################################
 
 
 def generate_solution_file(solution_lines, solution):
     """
     Serialize the solution file into a string array.
@@ -593,15 +653,15 @@
         self.project = project
         VS2010XML.__init__(self, 'PropertyGroup', {'Label': 'Globals'})
 
         ide = project.ide
 
         platform_version = None
         if ide >= IDETypes.vs2015:
-            platform_version = '10.0.17763.0'
+            platform_version = '10.0.18362.0'
 
         self.add_tags((
             ('ProjectName', project.name),
             ('ProjectGuid', '{{{}}}'.format(project.vs_uuid)),
             ('WindowsTargetPlatformVersion', platform_version)
         ))
 
@@ -1658,76 +1718,26 @@
     """
 
     # Too many branches
     # Too many locals
     # pylint: disable=R0912,R0914
 
     # Failsafe
-    if solution.ide not in (
-            IDETypes.vs2010, IDETypes.vs2012, IDETypes.vs2013, IDETypes.vs2015,
-            IDETypes.vs2017, IDETypes.vs2019):
+    if solution.ide not in SUPPORTED_IDES:
         return 10
 
-    # Since not all version of Visual Studio have plug ins for specific SDKS
-    # and build tools, filter out the ones know to not be compatible.
-
-    temp_list = [PlatformTypes.win32, PlatformTypes.win64]
-    if solution.ide is IDETypes.vs2010:
-        temp_list.append(PlatformTypes.xbox360)
-
-    if solution.ide >= IDETypes.vs2015:
-        temp_list.append(PlatformTypes.xboxone)
-
-    if solution.ide < IDETypes.vs2017:
-        temp_list.extend([PlatformTypes.ps3, PlatformTypes.vita])
-
-    if solution.ide >= IDETypes.vs2012:
-        temp_list.extend([PlatformTypes.ps4, PlatformTypes.wiiu])
-
-    if solution.ide >= IDETypes.vs2013:
-        temp_list.extend([PlatformTypes.tegra,
-                          PlatformTypes.androidarm32,
-                          PlatformTypes.androidarm64,
-                          PlatformTypes.androidintel32,
-                          PlatformTypes.androidintel64])
-
-    if solution.ide >= IDETypes.vs2015:
-        temp_list.append(PlatformTypes.switch)
-
-    if solution.ide >= IDETypes.vs2017:
-        temp_list.extend([PlatformTypes.winarm32, PlatformTypes.winarm64])
-
-    # Remove any targets that are not supported
-    # by Visual Studio 2010-2019
-    for project in solution.project_list:
-        configuration_list = []
-        for configuration in project.configuration_list:
-            if configuration.platform in temp_list:
-                configuration_list.append(configuration)
-        project.configuration_list = configuration_list
-
-    # Get the IDE name code
-    idecode = solution.ide.get_short_code()
-
-    # Get the platform code
-    temp_list = []
-    for project in solution.project_list:
-        temp_list.extend(project.configuration_list)
-    platformcode = platformtype_short_code(temp_list)
-
     # For starters, generate the UUID and filenames for the solution file
     # for visual studio, since each solution and project file generate
     # seperately
 
     # Iterate over the project files and create the filenames
     for project in solution.project_list:
 
-        platformcode = platformtype_short_code(project.configuration_list)
         project.vs_output_filename = '{}{}{}.vcxproj'.format(
-            project.name, idecode, platformcode)
+            project.name, solution.ide_code, project.platform_code)
         project.vs_uuid = get_uuid(project.vs_output_filename)
 
         for configuration in project.configuration_list:
             vs_platform = configuration.platform.get_vs_platform()[0]
             configuration.vs_platform = vs_platform
             configuration.vs_configuration_name = '{}|{}'.format(
                 configuration.name, vs_platform)
@@ -1740,15 +1750,15 @@
 
     # Get the output flags
     perforce = solution.perforce
     verbose = solution.verbose
 
     # Create the final filename for the Visual Studio Solution file
     solution_filename = '{}{}{}.sln'.format(
-        solution.name, idecode, platformcode)
+        solution.name, solution.ide_code, solution.platform_code)
 
     save_text_file_if_newer(
         os.path.join(solution.working_directory, solution_filename),
         solution_lines,
         bom=True,
         perforce=perforce,
         verbose=verbose)
```

### Comparing `makeprojects-0.9.8/makeprojects/xcode.py` & `makeprojects-0.9.9/makeprojects/xcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,53 @@
 
 from __future__ import absolute_import, print_function, unicode_literals
 import hashlib
 import os
 import operator
 import burger
 from burger import StringIO
-from .enums import FileTypes, ProjectTypes, PlatformTypes
+from .enums import FileTypes, ProjectTypes, PlatformTypes, IDETypes
 from .core import SourceFile
 
 # pylint: disable=C0302
 
+SUPPORTED_IDES = (
+    IDETypes.xcode3,
+    IDETypes.xcode4,
+    IDETypes.xcode5,
+    IDETypes.xcode6,
+    IDETypes.xcode7,
+    IDETypes.xcode8,
+    IDETypes.xcode9,
+    IDETypes.xcode10)
+
+########################################
+
+
+def test(ide, platform_type):
+    """ Filter for supported platforms
+
+    Args:
+        ide: IDETypes
+        platform_type: PlatformTypes
+    Returns:
+        True if supported, False if not
+    """
+
+    return platform_type in (
+        PlatformTypes.macosxintel32, PlatformTypes.macosxintel64, PlatformTypes.
+        macosxppc32, PlatformTypes.macosxppc64)
+
+
 #
 ## \package makeprojects.xcode
 # This module contains classes needed to generate
 # project files intended for use by Apple's XCode
 # IDE
 #
-
 IOS_MINIMUM_FRAMEWORKS = [
     'AVFoundation.framework',
     'CoreGraphics.framework',
     'CoreLocation.framework',
     'Foundation.framework',
     'QuartzCore.framework',
     'UIKit.framework'
@@ -55,16 +82,16 @@
 
 
 def calcuuid(input_str):
     """
     Given a string, create a 96 bit unique hash for XCode
     """
 
-    temphash = hashlib.md5(
-        burger.convert_to_windows_slashes(input_str).encode('utf-8')).hexdigest()
+    temphash = hashlib.md5(burger.convert_to_windows_slashes(
+        input_str).encode('utf-8')).hexdigest()
 
     # Take the hash string and only use the top 96 bits
 
     return temphash[0:24].upper()
 
 
 def writelist(selfarray, filep):
@@ -189,17 +216,26 @@
         if self.filereference.type == FileTypes.frameworks:
             ref_type = 'Frameworks'
         else:
             # It's a source file
             ref_type = 'Sources'
 
         basename = os.path.basename(self.filereference.filename)
-        filep.write('\t\t' + self.uuid + ' /* ' + basename + ' in ' + ref_type
-                    + ' */ = {isa = PBXBuildFile; fileRef = ' + self.filereference.uuid
-                    + ' /* ' + basename + ' */; };\n')
+        filep.write(
+            '\t\t' +
+            self.uuid +
+            ' /* ' +
+            basename +
+            ' in ' +
+            ref_type +
+            ' */ = {isa = PBXBuildFile; fileRef = ' +
+            self.filereference.uuid +
+            ' /* ' +
+            basename +
+            ' */; };\n')
 
 
 class PBXFileReference(object):
     """
     Each PBXFileReference entry
     Get the filename path and XCode type
     """
@@ -232,48 +268,76 @@
                 self.type != FileTypes.exe and \
                 self.type != FileTypes.frameworks:
             filep.write(' fileEncoding = 4;')
 
         # Each file type is handled differently
 
         if self.type == FileTypes.library:
-            filep.write(' explicitFileType = archive.ar; includeInIndex = 0; '
-                        'path = ' + basename + '; sourceTree = BUILT_PRODUCTS_DIR;')
+            filep.write(
+                ' explicitFileType = archive.ar; includeInIndex = 0; '
+                'path = ' + basename + '; sourceTree = BUILT_PRODUCTS_DIR;')
         elif self.type == FileTypes.exe:
             if basename.endswith('.app'):
                 filep.write(' explicitFileType = wrapper.application; '
                             'includeInIndex = 0; path = ' + basename
                             + '; sourceTree = BUILT_PRODUCTS_DIR;')
             else:
                 filep.write(' explicitFileType = "compiled.mach-o.executable"; '
                             'includeInIndex = 0; path = ' + basename
                             + '; sourceTree = BUILT_PRODUCTS_DIR;')
         elif self.type == FileTypes.frameworks:
-            filep.write(' lastKnownFileType = wrapper.framework; name = ' + basename
-                        + '; path = System/Library/Frameworks/' + basename
-                        + '; sourceTree = SDKROOT;')
+            filep.write(
+                ' lastKnownFileType = wrapper.framework; name = ' +
+                basename +
+                '; path = System/Library/Frameworks/' +
+                basename +
+                '; sourceTree = SDKROOT;')
         elif self.type == FileTypes.glsl:
-            filep.write(' lastKnownFileType = sourcecode.glsl; name = ' + basename +
-                        '; path = ' + self.filename + '; sourceTree = SOURCE_ROOT;')
+            filep.write(
+                ' lastKnownFileType = sourcecode.glsl; name = ' +
+                basename +
+                '; path = ' +
+                self.filename +
+                '; sourceTree = SOURCE_ROOT;')
         elif self.type == FileTypes.xml:
             if basename.endswith('.plist'):
-                filep.write(' lastKnownFileType = text.plist.xml; name = ' + basename +
-                            '; path = ' + self.filename + '; sourceTree = SOURCE_ROOT;')
+                filep.write(
+                    ' lastKnownFileType = text.plist.xml; name = ' +
+                    basename +
+                    '; path = ' +
+                    self.filename +
+                    '; sourceTree = SOURCE_ROOT;')
             else:
-                filep.write(' lastKnownFileType = text.xml; name = ' + basename +
-                            '; path = ' + self.filename + '; sourceTree = SOURCE_ROOT;')
+                filep.write(
+                    ' lastKnownFileType = text.xml; name = ' +
+                    basename +
+                    '; path = ' +
+                    self.filename +
+                    '; sourceTree = SOURCE_ROOT;')
         elif self.type == FileTypes.xcconfig:
-            filep.write(' lastKnownFileType = text.xcconfig; name = ' + basename +
-                        '; path = xcode/' + basename + '; sourceTree = BURGER_SDKS;')
+            filep.write(
+                ' lastKnownFileType = text.xcconfig; name = ' +
+                basename +
+                '; path = xcode/' +
+                basename +
+                '; sourceTree = BURGER_SDKS;')
         elif self.type == FileTypes.cpp:
-            filep.write(' lastKnownFileType = sourcecode.cpp.cpp; name = ' +
-                        basename + '; path = ' + self.filename + '; sourceTree = SOURCE_ROOT;')
+            filep.write(
+                ' lastKnownFileType = sourcecode.cpp.cpp; name = ' +
+                basename +
+                '; path = ' +
+                self.filename +
+                '; sourceTree = SOURCE_ROOT;')
         else:
-            filep.write(' lastKnownFileType = sourcecode.c.h; name = ' + basename +
-                        '; path = ' + self.filename + '; sourceTree = SOURCE_ROOT;')
+            filep.write(
+                ' lastKnownFileType = sourcecode.c.h; name = ' +
+                basename +
+                '; path = ' +
+                self.filename +
+                '; sourceTree = SOURCE_ROOT;')
 
         # Close out the line
 
         filep.write(' };\n')
 
 
 class PBXBuildRule(object):
@@ -294,17 +358,18 @@
         filep.write('\t\t\tcompilerSpec = com.apple.compilers.proxy.script;\n')
         filep.write('\t\t\tfilePatterns = "*.glsl";\n')
         filep.write('\t\t\tfileType = pattern.proxy;\n')
         filep.write('\t\t\tisEditable = 1;\n')
         filep.write('\t\t\toutputFiles = (\n')
         filep.write('\t\t\t\t"${INPUT_FILE_DIR}/${INPUT_FILE_BASE}.h",\n')
         filep.write('\t\t\t);\n')
-        filep.write('\t\t\tscript = "${BURGER_SDKS}/macosx/bin/stripcomments '
-                    '${INPUT_FILE_PATH}'
-                    ' -c -l g_${INPUT_FILE_BASE} ${INPUT_FILE_DIR}/${INPUT_FILE_BASE}.h";\n')
+        filep.write(
+            '\t\t\tscript = "${BURGER_SDKS}/macosx/bin/stripcomments '
+            '${INPUT_FILE_PATH}'
+            ' -c -l g_${INPUT_FILE_BASE} ${INPUT_FILE_DIR}/${INPUT_FILE_BASE}.h";\n')
         filep.write('\t\t};\n')
 
 
 class PBXGroup(object):
     """
     Each PBXGroup entry
     """
@@ -500,17 +565,20 @@
         filep.write('\t\t\tisa = PBXProject;\n')
         filep.write('\t\t\tattributes = {\n')
         filep.write('\t\t\t\tBuildIndependentTargetsInParallel = YES;\n')
         if self.project.idecode == 'xc5':
             filep.write('\t\t\t\tLastUpgradeCheck = 0510;\n')
         filep.write('\t\t\t};\n')
         if self.configlistref is not None:
-            filep.write('\t\t\tbuildConfigurationList = ' + self.configlistref.uuid
-                        + ' /* Build configuration list for PBXProject "'
-                        + self.project.projectnamecode + '" */;\n')
+            filep.write(
+                '\t\t\tbuildConfigurationList = ' +
+                self.configlistref.uuid +
+                ' /* Build configuration list for PBXProject "' +
+                self.project.projectnamecode +
+                '" */;\n')
 
         if self.project.idecode != 'xc3':
             filep.write('\t\t\tcompatibilityVersion = "Xcode 3.2";\n')
             filep.write('\t\t\tdevelopmentRegion = English;\n')
         else:
             filep.write('\t\t\tcompatibilityVersion = "Xcode 3.1";\n')
 
@@ -539,15 +607,16 @@
 
 
 class PBXNativeTarget(object):
     """
     Each PBXNative entry
     """
 
-    def __init__(self, parent, name, productreference, productname, producttype):
+    def __init__(self, parent, name, productreference,
+                 productname, producttype):
         self.parent = parent
         self.name = name
         self.productreference = productreference
         self.productname = productname
         self.producttype = producttype
         self.uuid = calcuuid('PBXNativeTarget' + name)
         self.configlistref = None
@@ -558,17 +627,20 @@
         """
         Write this record to output
         """
 
         filep.write('\t\t' + self.uuid + ' /* ' + self.name + ' */ = {\n')
         filep.write('\t\t\tisa = PBXNativeTarget;\n')
         if self.configlistref is not None:
-            filep.write('\t\t\tbuildConfigurationList = ' + self.configlistref.uuid
-                        + ' /* Build configuration list for PBXNativeTarget "'
-                        + self.name + '" */;\n')
+            filep.write(
+                '\t\t\tbuildConfigurationList = ' +
+                self.configlistref.uuid +
+                ' /* Build configuration list for PBXNativeTarget "' +
+                self.name +
+                '" */;\n')
         filep.write('\t\t\tbuildPhases = (\n')
         for item in self.phases:
             filep.write('\t\t\t\t' + item[0] + ' /* ' + item[1] + ' */,\n')
         filep.write('\t\t\t);\n')
         filep.write('\t\t\tbuildRules = (\n')
         for item in self.parent.pbxbuildrules:
             filep.write('\t\t\t\t' + item.uuid + ' /* PBXBuildRule */,\n')
@@ -616,17 +688,21 @@
         Write this record to output
         """
 
         filep.write('\t\t' + self.uuid + ' /* ' +
                     str(self.configname) + ' */ = {\n')
         filep.write('\t\t\tisa = XCBuildConfiguration;\n')
         if self.configfilereference is not None:
-            filep.write('\t\t\tbaseConfigurationReference = '
-                        + self.configfilereference.uuid
-                        + ' /* ' + os.path.basename(self.configfilereference.filename) + ' */;\n')
+            filep.write(
+                '\t\t\tbaseConfigurationReference = ' +
+                self.configfilereference.uuid +
+                ' /* ' +
+                os.path.basename(
+                    self.configfilereference.filename) +
+                ' */;\n')
         filep.write('\t\t\tbuildSettings = {\n')
         if self.sdkroot is not None:
             filep.write('\t\t\t\tSDKROOT = ' + self.sdkroot + ';\n')
         if self.installpath is True:
             filep.write('\t\t\t\tINSTALL_PATH = "$(HOME)/Applications";\n')
         filep.write('\t\t\t};\n')
         filep.write('\t\t\tname = ' + str(self.configname) + ';\n')
@@ -779,15 +855,16 @@
         Add a new source build phase list
         """
 
         entry = PBXSourcesBuildPhase(owner)
         self.sourcesbuildphases.append(entry)
         return entry
 
-    def addnativeproject(self, name, productreference, productname, producttype):
+    def addnativeproject(self, name, productreference,
+                         productname, producttype):
         """
         Add a new native target list
         """
 
         entry = PBXNativeTarget(
             self, name, productreference, productname, producttype)
         self.pbxnativetargets.append(entry)
@@ -937,22 +1014,25 @@
     rootproject = xcodeprojectfile.pbxprojects[0]
 
     #
     # Ensure the slashes are correct for XCode
     #
 
     for item in codefiles:
-        item.relative_pathname = burger.convert_to_linux_slashes(item.relative_pathname)
+        item.relative_pathname = burger.convert_to_linux_slashes(
+            item.relative_pathname)
 
     #
     # Let's create the solution file!
     #
 
     solutionfoldername = os.path.join(
-        solution.working_directory, xcodeprojectfile.projectnamecode + '.xcodeproj')
+        solution.working_directory,
+        xcodeprojectfile.projectnamecode +
+        '.xcodeproj')
     burger.create_folder_if_needed(solutionfoldername)
     projectfilename = os.path.join(solutionfoldername, 'project.pbxproj')
 
     #
     # Add the configuration file reference (or not)
     #
```

### Comparing `makeprojects-0.9.8/makeprojects.egg-info/PKG-INFO` & `makeprojects-0.9.9/makeprojects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: makeprojects
-Version: 0.9.8
+Version: 0.9.9
 Summary: IDE project generator for Visual Studio, XCode, etc...
 Home-page: http://makeprojects.readthedocs.io
 Author: Rebecca Ann Heineman <becky@burgerbecky.com>
 Author-email: becky@burgerbecky.com
 License: MIT License
 Description: =======================
         Makeprojects for Python
```

### Comparing `makeprojects-0.9.8/makeprojects.egg-info/SOURCES.txt` & `makeprojects-0.9.9/makeprojects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `makeprojects-0.9.8/setup.py` & `makeprojects-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 with io.open(os.path.join(CWD, 'README.rst'), encoding='utf-8') as filep:
     LONG_DESCRIPTION = filep.read()
 
 # Create the dependency list
 INSTALL_REQUIRES = [
     'setuptools >= 17.1',
     'enum34 >= 1.0.0',
-    'burger >= 1.1.28',
+    'burger >= 1.1.31',
     'argparse >= 1.0',
     'glob2 >= 0.6',
     'funcsigs >= 1.0'
 ]
 
 # Project classifiers
 CLASSIFIERS = [
```

