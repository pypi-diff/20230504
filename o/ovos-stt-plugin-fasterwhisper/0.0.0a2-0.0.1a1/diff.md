# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.0a2.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.0a2.tar", last modified: Sat Apr 29 17:06:43 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a1.tar", last modified: Thu May  4 03:07:55 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 17:06:39.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:06:43.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:06:43.530910 ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3479 2023-04-29 17:06:36.000000 ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 03:07:50.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.0a2
+Version: 0.0.1a1
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,40 @@
 
 ## Configuration
 
 available models are `"tiny.en", "tiny", "base.en", "base", "small.en", "small", "medium.en", "medium", "large-v2"`
 
 eg, to use Large model with GPU
 
+To use Whisper as STT
+
 ```json
   "stt": {
     "module": "ovos-stt-plugin-fasterwhisper",
     "ovos-stt-plugin-fasterwhisper": {
         "model": "large-v2",
         "use_cuda": true,
         "compute_type": "float16",
         "beam_size": 5
     }
   }
  
 ```
 
+To use Whisper for lang detection  (ovos-dinkum-listener only)
+
+
+```json
+  "listener": {
+    "audio_transformers": {
+        "ovos-audio-transformer-plugin-fasterwhisper": {
+            "model": "small"
+        }
+    }
+  }
+
+```
+
 ## Models
 
 Models will be auto downloaded by faster whisper on plugin load
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ovos_utils.log import LOG
 from speech_recognition import AudioData
 
 
 class FasterWhisperLangClassifier(AudioTransformer):
     def __init__(self, config=None):
         config = config or {}
-        super().__init__("fasterwhisper_lang", 10, config)
+        super().__init__("ovos-audio-transformer-plugin-fasterwhisper", 10, config)
         model = self.config.get("model")
         if not model:
             model = "small.en"
         assert model in FasterWhisperSTT.MODELS  # TODO - better error handling
 
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.0a2
+Version: 0.0.1a1
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.0a2/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 
 PLUGIN_ENTRY_POINT = 'ovos-stt-plugin-fasterwhisper = ovos_stt_plugin_fasterwhisper:FasterWhisperSTT'
 CONFIG_ENTRY_POINT = 'ovos-stt-plugin-fasterwhisper.config = ovos_stt_plugin_fasterwhisper:FasterWhisperSTTConfig'
-LANG_PLUGIN_ENTRY_POINT = 'ovos-stt-plugin-fasterwhisper = ovos_stt_plugin_fasterwhisper:FasterWhisperLangClassifier'
+LANG_PLUGIN_ENTRY_POINT = 'ovos-audio-transformer-plugin-fasterwhisper = ovos_stt_plugin_fasterwhisper:FasterWhisperLangClassifier'
 
 
 setup(
     name='ovos-stt-plugin-fasterwhisper',
     version=get_version(),
     description='A fasterwhisper stt plugin for mycroft',
     url='https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper',
```

