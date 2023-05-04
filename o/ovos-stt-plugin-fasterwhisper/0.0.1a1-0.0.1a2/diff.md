# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a1.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a1.tar", last modified: Thu May  4 03:07:55 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a2.tar", last modified: Thu May  4 14:16:10 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 03:07:50.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:07:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:07:55.313961 ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-04 03:07:48.000000 ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 14:16:03.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,29 @@
 
         if self.use_cuda:
             device = "cuda"
         else:
             device = "cpu"
         self.engine = WhisperModel(model, device=device, compute_type=self.compute_type)
 
+    @staticmethod
+    def audiochunk2array(audio_data):
+        # Convert buffer to float32 using NumPy
+        audio_as_np_int16 = numpy.frombuffer(audio_data, dtype=numpy.int16)
+        audio_as_np_float32 = audio_as_np_int16.astype(numpy.float32)
+
+        # Normalise float32 array so that values are between -1.0 and +1.0
+        max_int16 = 2 ** 15
+        data = audio_as_np_float32 / max_int16
+        return data
+
     # plugin api
     def transform(self, audio_data):
         # segments is an iterator, transcription is not done here
-        _, info = self.engine.transcribe(FasterWhisperSTT.audiodata2array(audio_data), beam_size=self.beam_size)
+        _, info = self.engine.transcribe(self.audiochunk2array(audio_data), beam_size=self.beam_size)
         LOG.info(f"Detected speech language '{info.language}' with probability {info.language_probability}")
         return audio_data, {"stt_lang": info.language, "lang_probability": info.language_probability}
 
 
 class FasterWhisperSTT(STT):
     MODELS = ("tiny.en", "tiny", "base.en", "base", "small.en", "small", "medium.en", "medium", "large", "large-v2")
     LANGUAGES = {
@@ -154,22 +165,15 @@
         else:
             device = "cpu"
         self.engine = WhisperModel(model, device=device, compute_type=self.compute_type)
 
     @staticmethod
     def audiodata2array(audio_data):
         assert isinstance(audio_data, AudioData)
-        # Convert buffer to float32 using NumPy
-        audio_as_np_int16 = numpy.frombuffer(audio_data.get_wav_data(), dtype=numpy.int16)
-        audio_as_np_float32 = audio_as_np_int16.astype(numpy.float32)
-
-        # Normalise float32 array so that values are between -1.0 and +1.0
-        max_int16 = 2 ** 15
-        data = audio_as_np_float32 / max_int16
-        return data
+        return FasterWhisperLangClassifier.audiochunk2array(audio_data.get_wav_data())
 
     def execute(self, audio, language=None):
         segments, _ = self.engine.transcribe(self.audiodata2array(audio), beam_size=self.beam_size)
         # segments is an iterator, transcription only happens here
         transcription = "".join(segment.text for segment in segments).strip()
         return transcription
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a1/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.py`

 * *Files identical despite different names*

