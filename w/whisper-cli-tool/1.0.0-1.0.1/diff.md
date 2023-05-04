# Comparing `tmp/whisper-cli-tool-1.0.0.tar.gz` & `tmp/whisper-cli-tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-cli-tool-1.0.0.tar", last modified: Thu May  4 18:30:32 2023, max compression
+gzip compressed data, was "whisper-cli-tool-1.0.1.tar", last modified: Thu May  4 18:51:21 2023, max compression
```

## Comparing `whisper-cli-tool-1.0.0.tar` & `whisper-cli-tool-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:30:32.479658 whisper-cli-tool-1.0.0/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.0/LICENSE
--rw-r--r--   0 joaonogueira   (501) staff       (20)    13255 2023-05-04 18:30:32.479444 whisper-cli-tool-1.0.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)       63 2023-05-04 18:24:29.000000 whisper-cli-tool-1.0.0/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 18:30:32.479703 whisper-cli-tool-1.0.0/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      599 2023-05-04 18:28:10.000000 whisper-cli-tool-1.0.0/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:30:32.479167 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    13255 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      268 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       45 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       12 2023-05-04 18:30:32.000000 whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/top_level.txt
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:51:21.982171 whisper-cli-tool-1.0.1/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.1/LICENSE
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    13410 2023-05-04 18:51:21.981952 whisper-cli-tool-1.0.1/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      217 2023-05-04 18:48:50.000000 whisper-cli-tool-1.0.1/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 18:51:21.982215 whisper-cli-tool-1.0.1/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      604 2023-05-04 18:51:12.000000 whisper-cli-tool-1.0.1/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:51:21.981692 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    13410 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      268 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       12 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/top_level.txt
```

### Comparing `whisper-cli-tool-1.0.0/LICENSE` & `whisper-cli-tool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-cli-tool-1.0.0/PKG-INFO` & `whisper-cli-tool-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -208,7 +208,17 @@
            limitations under the License.
         
 License-File: LICENSE
 
 # Whisper CLI
 
 CLI to translate audiofiles on the command-line
+
+
+## Setup
+
+Before to install, make sure you have a open api key available on your computer PATH.
+
+```
+$ pip install whisper-cli-tool
+$ whisper --help
+```
```

### Comparing `whisper-cli-tool-1.0.0/setup.py` & `whisper-cli-tool-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="whisper-cli-tool",
-    version="1.0.0",
+    version="1.0.1",
     description="Do transcriptions of audiofiles using the whisper-1 model from OpenAI.",
     long_description=readfile('README.md'),
     author="João Nogueira",
     author_email="joaopcnogueira@gmail.com",
     url="",
     py_modules=['whisper_cli'],
     license=readfile('LICENSE'),
     install_requires=['openai'],
     entry_points={
         'console_scripts': [
-            'whisper = whisper_cli:main'
+            'whisper = whisper_cli_tool:main'
         ]
     },
 )
```

### Comparing `whisper-cli-tool-1.0.0/whisper_cli_tool.egg-info/PKG-INFO` & `whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -208,7 +208,17 @@
            limitations under the License.
         
 License-File: LICENSE
 
 # Whisper CLI
 
 CLI to translate audiofiles on the command-line
+
+
+## Setup
+
+Before to install, make sure you have a open api key available on your computer PATH.
+
+```
+$ pip install whisper-cli-tool
+$ whisper --help
+```
```

