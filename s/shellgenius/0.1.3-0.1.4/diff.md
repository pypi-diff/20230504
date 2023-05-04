# Comparing `tmp/shellgenius-0.1.3.tar.gz` & `tmp/shellgenius-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.3.tar", last modified: Thu May  4 18:30:53 2023, max compression
+gzip compressed data, was "shellgenius-0.1.4.tar", last modified: Thu May  4 18:34:41 2023, max compression
```

## Comparing `shellgenius-0.1.3.tar` & `shellgenius-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:30:53.824735 shellgenius-0.1.3/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.3/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:30:53.824735 shellgenius-0.1.3/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3235 2023-05-04 18:15:13.000000 shellgenius-0.1.3/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-04 18:30:53.824735 shellgenius-0.1.3/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-04 18:30:46.000000 shellgenius-0.1.3/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:30:53.824735 shellgenius-0.1.3/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.3/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3089 2023-05-04 18:30:05.000000 shellgenius-0.1.3/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5522 2023-05-04 18:04:38.000000 shellgenius-0.1.3/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:30:53.824735 shellgenius-0.1.3/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-04 18:30:53.000000 shellgenius-0.1.3/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.4/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:34:41.834706 shellgenius-0.1.4/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3235 2023-05-04 18:15:13.000000 shellgenius-0.1.4/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-04 18:34:41.834706 shellgenius-0.1.4/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-04 18:34:32.000000 shellgenius-0.1.4/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.4/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3076 2023-05-04 18:34:00.000000 shellgenius-0.1.4/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5522 2023-05-04 18:04:38.000000 shellgenius-0.1.4/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:34:41.834706 shellgenius-0.1.4/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-04 18:34:41.000000 shellgenius-0.1.4/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.3/LICENSE` & `shellgenius-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.3/PKG-INFO` & `shellgenius-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.3
+Version: 0.1.4
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
```

### Comparing `shellgenius-0.1.3/README.md` & `shellgenius-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.3/setup.py` & `shellgenius-0.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.3/shellgenius/cli.py` & `shellgenius-0.1.4/shellgenius/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,25 @@
 @click.argument("command_description", type=str, nargs=-1)
 @click.pass_context
 def shellgenius(ctx, command_description):
     """
     Generate and optionally execute a shell command based on the given command description.
 
     Example:
-        $ shellgenius create a new file called example.txt
-        Generated command: touch example.txt
+
+        shellgenius create a new file called example.txt
+
+        `touch example.txt`
+
         Explanation:
+
         - touch command is used to create a new file if it doesn't exist
+
         - example.txt is the name of the new file
+
         Do you want to execute this command? [Y/n]: y
     """
     if not command_description:
         click.echo(ctx.get_help())
         return
 
     command_description = " ".join(command_description)
```

### Comparing `shellgenius-0.1.3/shellgenius/gpt_integration.py` & `shellgenius-0.1.4/shellgenius/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.3/shellgenius.egg-info/PKG-INFO` & `shellgenius-0.1.4/shellgenius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.3
+Version: 0.1.4
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
```

