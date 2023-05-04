# Comparing `tmp/OWR-2.4.tar.gz` & `tmp/OWR-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.4.tar", last modified: Thu May  4 11:45:28 2023, max compression
+gzip compressed data, was "OWR-2.5.1.tar", last modified: Thu May  4 12:31:09 2023, max compression
```

## Comparing `OWR-2.4.tar` & `OWR-2.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 08:03:42.000000 OWR-2.4/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8228 2023-05-04 11:44:58.000000 OWR-2.4/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2718 2023-05-04 11:40:55.000000 OWR-2.4/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      304 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      304 2023-05-04 11:45:28.785057 OWR-2.4/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 11:40:55.000000 OWR-2.4/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 11:45:28.785057 OWR-2.4/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      745 2023-05-04 11:40:55.000000 OWR-2.4/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 12:31:09.638855 OWR-2.5.1/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.5.1/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 12:31:09.634855 OWR-2.5.1/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8231 2023-05-04 12:30:17.000000 OWR-2.5.1/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 12:31:09.634855 OWR-2.5.1/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2718 2023-05-04 12:30:17.000000 OWR-2.5.1/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 12:31:09.634855 OWR-2.5.1/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 12:31:09.000000 OWR-2.5.1/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 12:31:09.000000 OWR-2.5.1/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 12:31:09.000000 OWR-2.5.1/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 12:31:09.000000 OWR-2.5.1/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 12:31:09.000000 OWR-2.5.1/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 12:31:09.634855 OWR-2.5.1/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 12:29:59.000000 OWR-2.5.1/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 12:31:09.638855 OWR-2.5.1/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-04 12:30:59.000000 OWR-2.5.1/setup.py
```

### Comparing `OWR-2.4/LICENSE` & `OWR-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.4/OWR/__init__.py` & `OWR-2.5.1/OWR/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,16 @@
                     samples[i[0]:i[1]] = librosa.tone(600, length=i[1] - i[0], sr=16000)
                 else:
                     samples[i[0]:i[1]] = np.tile((librosa.tone(600, length=i[1] - i[0], sr=16000)),
                                                  (samples.ndim, 1)).transpose()
 
     def __init__(self):
         self.ASR = SpeechRecognitionModel("rmgaliullin/wav2vec2-based-obscenity-detector", letter_case='lowercase')
-        self.__phonetic_word_codes = self.__get_phonetic_for_words(
-            os.path.split(inspect.getfile(self.__class__))[0] + '/data/obscenity_words.json')
+        self.__phonetic_word_codes = self.__get_phonetic_for_words(os.path.join(
+            os.path.split(inspect.getfile(self.__class__))[0], 'data', 'obscenity_words.json'))
         logger.info("Initialization of the model has been completed")
 
     def mute_words(self, audio_path: str, mode: str):
         audio_file = sf.SoundFile(audio_path)
         origin_samples = audio_file.read()
         origin_sr = audio_file.samplerate
         logger.info(
@@ -148,43 +148,42 @@
                 end += 2 * letter_len
                 if start < 0:
                     start = 0
                 if end > end_timestamps[-1] * (sample_rate // 1000):
                     end = end_timestamps[-1] * (sample_rate // 1000)
                 ow_timestamps.append((start, end))
         # ows - all recognised words
-        if evaluation != None:
+        if evaluation is not None:
             evaluation.extend(ows)
         return ow_timestamps
 
-    def evaluate(self, audio_transcript_data):
+    def evaluate(self, audio_transcript_data) -> dict:
         data = []
-        cer_ow = 0
-        wer_ow = 0
         true_positive = 0
         total = 0
-        for audio_path, transcript_path in audio_transcript_data:
+        for test in audio_transcript_data:
             prediction_ow = []
-            text = open(transcript_path).read().strip()
-            data.append({'path': audio_path, 'transcription': text})
-            reference_ow = [i for i in self.__phonetic_word_codes.keys() if i in text]
-            self.__find_words(self.ASR.transcribe([audio_path])[0], 16000, prediction_ow)
+            text = open(test["transcript_path"]).read().strip()
+            data.append({'path': test["audio_path"], 'transcription': text})
+            reference_ow = [i for i in text.split() if i in self.__phonetic_word_codes.keys()]
+            reference_ow.sort()
+            self.__find_words(self.ASR.transcribe([test["audio_path"]])[0], 16000, prediction_ow)
+            prediction_ow.sort()
             true_positive += len(prediction_ow)
             total += len(reference_ow)
-            cer_ow = cer(prediction_ow, reference_ow)
-            wer_ow = wer(prediction_ow, reference_ow)
-
+        if total == 0:
+            total = 1
+            true_positive = 0
         return {"total cer": self.ASR.evaluate(data)["cer"],
                 "total wer": self.ASR.evaluate(data)["wer"],
-                "obscenity cer": cer_ow,
-                "obscenity wer": wer_ow,
-                "rate of word detection": true_positive / (1 if total == 0 else total)}
+                "rate of word detection": true_positive / total}
 
 
 if __name__ == "__main__":
     detector = ObscenityWordsRecognizer()
-    dir_path = os.path.join(os.getcwd(), "data")
-    file_name = "audio_03.wav"
-    playsound(os.path.join(dir_path, file_name))
-    a = detector.mute_words(os.path.join(dir_path, file_name), "b")
-    print(a)
-    playsound(os.path.join(dir_path, "result_" + file_name))
+    evaluation = detector.evaluate(
+        [{'audio_path': os.path.join("test", "audio", f'audio_{i}.wav'),
+          'transcript_path': os.path.join("test", "transcript", f'transcript_{i}.txt')}
+         for i in range(6)
+         ])
+    with open(os.path.join("test", 'result.json'), 'w') as outfile:
+        outfile.write(json.dumps(evaluation))
```

### Comparing `OWR-2.4/OWR/data/obscenity_words.json` & `OWR-2.5.1/OWR/data/obscenity_words.json`

 * *Files identical despite different names*

### Comparing `OWR-2.4/setup.py` & `OWR-2.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.4',
+    version='2.5.1',
     description='Obscene word recognition package',
     url='https://github.com/RuslanGaliullin/FFixTelegramBot/tree/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
```

