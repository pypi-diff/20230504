# Comparing `tmp/whisper-cli-tool-1.0.2.tar.gz` & `tmp/whisper-cli-tool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-cli-tool-1.0.2.tar", last modified: Thu May  4 19:03:44 2023, max compression
+gzip compressed data, was "whisper-cli-tool-1.0.3.tar", last modified: Thu May  4 19:10:52 2023, max compression
```

## Comparing `whisper-cli-tool-1.0.2.tar` & `whisper-cli-tool-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:03:44.204005 whisper-cli-tool-1.0.2/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.2/LICENSE
--rw-r--r--   0 joaonogueira   (501) staff       (20)    14448 2023-05-04 19:03:44.203761 whisper-cli-tool-1.0.2/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1215 2023-05-04 19:03:41.000000 whisper-cli-tool-1.0.2/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 19:03:44.204057 whisper-cli-tool-1.0.2/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      662 2023-05-04 19:03:32.000000 whisper-cli-tool-1.0.2/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:03:44.203464 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    14448 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      288 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       17 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1419 2023-05-04 18:58:27.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:10:52.842527 whisper-cli-tool-1.0.3/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.3/LICENSE
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    14619 2023-05-04 19:10:52.842304 whisper-cli-tool-1.0.3/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1387 2023-05-04 19:10:38.000000 whisper-cli-tool-1.0.3/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 19:10:52.842577 whisper-cli-tool-1.0.3/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      662 2023-05-04 19:09:57.000000 whisper-cli-tool-1.0.3/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:10:52.842030 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    14619 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      288 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       17 2023-05-04 19:10:52.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1419 2023-05-04 18:58:27.000000 whisper-cli-tool-1.0.3/whisper_cli_tool.py
```

### Comparing `whisper-cli-tool-1.0.2/LICENSE` & `whisper-cli-tool-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-cli-tool-1.0.2/PKG-INFO` & `whisper-cli-tool-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -214,22 +214,26 @@
 ================
 CLI to translate an audiofile on the command-line
 
 ## Setup
 
 Before to install, make sure you have a OpenAI api key available on your computer PATH.
 
+Execute the command below to install the `whisper-cli-tool` python package, which offer the `whisper` command line utility to make transcriptions.
+
 ```bash
 $ pip install whisper-cli-tool
 ```
 
+After installation, just execute:
+
 ```bash
 $ whisper --help
 
-usage: whisper_cli_tool.py [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
+usage: whisper [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
 
 Do transcription of an audiofile
 
 positional arguments:
   infile                Input file name. Supported formats: m4a, mp3, webm, mp4, mpga, wav, mpeg.
 
 options:
```

### Comparing `whisper-cli-tool-1.0.2/README.md` & `whisper-cli-tool-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 ================
 CLI to translate an audiofile on the command-line
 
 ## Setup
 
 Before to install, make sure you have a OpenAI api key available on your computer PATH.
 
+Execute the command below to install the `whisper-cli-tool` python package, which offer the `whisper` command line utility to make transcriptions.
+
 ```bash
 $ pip install whisper-cli-tool
 ```
 
+After installation, just execute:
+
 ```bash
 $ whisper --help
 
-usage: whisper_cli_tool.py [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
+usage: whisper [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
 
 Do transcription of an audiofile
 
 positional arguments:
   infile                Input file name. Supported formats: m4a, mp3, webm, mp4, mpga, wav, mpeg.
 
 options:
@@ -35,8 +39,8 @@
 $ whisper my-audio.mp3
 ```
 where my-audio.mp3 is your audiofile. The transcribed text will be saved into transcription-output.txt 
 
 If you want to change arguments, let's say, change the response format from text to str, just do:
 ```
 $ whisper my-audio.mp3 --response-format str --language pt --outfile my-transcription.mp3
-```
+```
```

### Comparing `whisper-cli-tool-1.0.2/setup.py` & `whisper-cli-tool-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="whisper-cli-tool",
-    version="1.0.2",
+    version="1.0.3",
     description="Do transcriptions of audiofiles using the whisper-1 model from OpenAI.",
     long_description=readfile('README.md'),
     author="João Nogueira",
     author_email="joaopcnogueira@gmail.com",
     url="",
     py_modules=['whisper_cli_tool'],
     license=readfile('LICENSE'),
```

### Comparing `whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/PKG-INFO` & `whisper-cli-tool-1.0.3/whisper_cli_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -214,22 +214,26 @@
 ================
 CLI to translate an audiofile on the command-line
 
 ## Setup
 
 Before to install, make sure you have a OpenAI api key available on your computer PATH.
 
+Execute the command below to install the `whisper-cli-tool` python package, which offer the `whisper` command line utility to make transcriptions.
+
 ```bash
 $ pip install whisper-cli-tool
 ```
 
+After installation, just execute:
+
 ```bash
 $ whisper --help
 
-usage: whisper_cli_tool.py [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
+usage: whisper [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
 
 Do transcription of an audiofile
 
 positional arguments:
   infile                Input file name. Supported formats: m4a, mp3, webm, mp4, mpga, wav, mpeg.
 
 options:
```

### Comparing `whisper-cli-tool-1.0.2/whisper_cli_tool.py` & `whisper-cli-tool-1.0.3/whisper_cli_tool.py`

 * *Files identical despite different names*

