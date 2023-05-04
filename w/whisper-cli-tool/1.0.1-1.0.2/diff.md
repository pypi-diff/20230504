# Comparing `tmp/whisper-cli-tool-1.0.1.tar.gz` & `tmp/whisper-cli-tool-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-cli-tool-1.0.1.tar", last modified: Thu May  4 18:51:21 2023, max compression
+gzip compressed data, was "whisper-cli-tool-1.0.2.tar", last modified: Thu May  4 19:03:44 2023, max compression
```

## Comparing `whisper-cli-tool-1.0.1.tar` & `whisper-cli-tool-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:51:21.982171 whisper-cli-tool-1.0.1/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.1/LICENSE
--rw-r--r--   0 joaonogueira   (501) staff       (20)    13410 2023-05-04 18:51:21.981952 whisper-cli-tool-1.0.1/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      217 2023-05-04 18:48:50.000000 whisper-cli-tool-1.0.1/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 18:51:21.982215 whisper-cli-tool-1.0.1/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      604 2023-05-04 18:51:12.000000 whisper-cli-tool-1.0.1/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 18:51:21.981692 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    13410 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      268 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       12 2023-05-04 18:51:21.000000 whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/top_level.txt
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:03:44.204005 whisper-cli-tool-1.0.2/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-05-04 18:25:43.000000 whisper-cli-tool-1.0.2/LICENSE
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    14448 2023-05-04 19:03:44.203761 whisper-cli-tool-1.0.2/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1215 2023-05-04 19:03:41.000000 whisper-cli-tool-1.0.2/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-05-04 19:03:44.204057 whisper-cli-tool-1.0.2/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      662 2023-05-04 19:03:32.000000 whisper-cli-tool-1.0.2/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-05-04 19:03:44.203464 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    14448 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      288 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       17 2023-05-04 19:03:44.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1419 2023-05-04 18:58:27.000000 whisper-cli-tool-1.0.2/whisper_cli_tool.py
```

### Comparing `whisper-cli-tool-1.0.1/LICENSE` & `whisper-cli-tool-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-cli-tool-1.0.1/PKG-INFO` & `whisper-cli-tool-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.1
+Version: 1.0.2
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -203,22 +203,52 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Whisper CLI
-
-CLI to translate audiofiles on the command-line
-
+Whisper CLI
+================
+CLI to translate an audiofile on the command-line
 
 ## Setup
 
-Before to install, make sure you have a open api key available on your computer PATH.
+Before to install, make sure you have a OpenAI api key available on your computer PATH.
 
-```
+```bash
 $ pip install whisper-cli-tool
+```
+
+```bash
 $ whisper --help
+
+usage: whisper_cli_tool.py [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
+
+Do transcription of an audiofile
+
+positional arguments:
+  infile                Input file name. Supported formats: m4a, mp3, webm, mp4, mpga, wav, mpeg.
+
+options:
+  -h, --help            show this help message and exit
+  --response-format RESPONSE_FORMAT
+                        Response format. Supported formats: text, srt.
+  --language LANGUAGE   Language the audio should be translated to
+  --outfile OUTFILE     Output file name
+```
+
+## Usage
+
+To transcribe an audio to portuguese in text format, just execute:
+```
+$ whisper my-audio.mp3
+```
+where my-audio.mp3 is your audiofile. The transcribed text will be saved into transcription-output.txt 
+
+If you want to change arguments, let's say, change the response format from text to str, just do:
+```
+$ whisper my-audio.mp3 --response-format str --language pt --outfile my-transcription.mp3
 ```
```

### Comparing `whisper-cli-tool-1.0.1/setup.py` & `whisper-cli-tool-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="whisper-cli-tool",
-    version="1.0.1",
+    version="1.0.2",
     description="Do transcriptions of audiofiles using the whisper-1 model from OpenAI.",
     long_description=readfile('README.md'),
     author="João Nogueira",
     author_email="joaopcnogueira@gmail.com",
     url="",
-    py_modules=['whisper_cli'],
+    py_modules=['whisper_cli_tool'],
     license=readfile('LICENSE'),
     install_requires=['openai'],
+    long_description_content_type = 'text/markdown',
     entry_points={
         'console_scripts': [
             'whisper = whisper_cli_tool:main'
         ]
     },
 )
```

### Comparing `whisper-cli-tool-1.0.1/whisper_cli_tool.egg-info/PKG-INFO` & `whisper-cli-tool-1.0.2/whisper_cli_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli-tool
-Version: 1.0.1
+Version: 1.0.2
 Summary: Do transcriptions of audiofiles using the whisper-1 model from OpenAI.
 Home-page: 
 Author: João Nogueira
 Author-email: joaopcnogueira@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -203,22 +203,52 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Whisper CLI
-
-CLI to translate audiofiles on the command-line
-
+Whisper CLI
+================
+CLI to translate an audiofile on the command-line
 
 ## Setup
 
-Before to install, make sure you have a open api key available on your computer PATH.
+Before to install, make sure you have a OpenAI api key available on your computer PATH.
 
-```
+```bash
 $ pip install whisper-cli-tool
+```
+
+```bash
 $ whisper --help
+
+usage: whisper_cli_tool.py [-h] [--response-format RESPONSE_FORMAT] [--language LANGUAGE] [--outfile OUTFILE] infile
+
+Do transcription of an audiofile
+
+positional arguments:
+  infile                Input file name. Supported formats: m4a, mp3, webm, mp4, mpga, wav, mpeg.
+
+options:
+  -h, --help            show this help message and exit
+  --response-format RESPONSE_FORMAT
+                        Response format. Supported formats: text, srt.
+  --language LANGUAGE   Language the audio should be translated to
+  --outfile OUTFILE     Output file name
+```
+
+## Usage
+
+To transcribe an audio to portuguese in text format, just execute:
+```
+$ whisper my-audio.mp3
+```
+where my-audio.mp3 is your audiofile. The transcribed text will be saved into transcription-output.txt 
+
+If you want to change arguments, let's say, change the response format from text to str, just do:
+```
+$ whisper my-audio.mp3 --response-format str --language pt --outfile my-transcription.mp3
 ```
```

