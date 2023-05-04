# Comparing `tmp/OWR-2.3.tar.gz` & `tmp/OWR-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.3.tar", last modified: Wed May  3 18:01:39 2023, max compression
+gzip compressed data, was "OWR-2.4.tar", last modified: Thu May  4 11:45:28 2023, max compression
```

## Comparing `OWR-2.3.tar` & `OWR-2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.3/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6921 2023-05-03 16:39:31.000000 OWR-2.3/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2719 2023-05-03 17:59:31.000000 OWR-2.3/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 18:01:39.416102 OWR-2.3/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.3/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 18:01:39.416102 OWR-2.3/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 18:01:33.000000 OWR-2.3/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 08:03:42.000000 OWR-2.4/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8228 2023-05-04 11:44:58.000000 OWR-2.4/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2718 2023-05-04 11:40:55.000000 OWR-2.4/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 11:45:28.785057 OWR-2.4/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      304 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 11:45:28.000000 OWR-2.4/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      304 2023-05-04 11:45:28.785057 OWR-2.4/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 11:40:55.000000 OWR-2.4/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 11:45:28.785057 OWR-2.4/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      745 2023-05-04 11:40:55.000000 OWR-2.4/setup.py
```

### Comparing `OWR-2.3/LICENSE` & `OWR-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.3/OWR/__init__.py` & `OWR-2.4/OWR/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import soundfile as sf
 from fonetika.soundex import RussianSoundex
 import numpy as np
 from playsound import playsound
 import pylcs
 import logging
 import inspect
+from huggingsound.metrics import cer, wer
 
 # Setup logging
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(message)s",
     datefmt="%m/%d/%Y %H:%M:%S",
     handlers=[logging.StreamHandler(sys.stdout)],
@@ -22,36 +23,34 @@
 logger.setLevel(logging.INFO)
 
 
 class ObscenityWordsRecognizer:
     soundex = RussianSoundex(delete_first_letter=True, reduce_word=True)
 
     @staticmethod
-    def __get_phonetic_for_words(path_to_words: str) -> tuple[dict[str, str], dict[str, str]]:
+    def __get_phonetic_for_words(path_to_words: str) -> dict[str, str]:
         soundex = RussianSoundex(delete_first_letter=True)
         result_word_to_code = {}
-        result_code_to_word = {}
         with open(path_to_words, 'rb') as fp:
             words = json.load(fp)
         for i in words:
-            result_code_to_word[soundex.transform(i)] = i
             result_word_to_code[i] = soundex.transform(i)
-        return result_code_to_word, result_word_to_code
+        return result_word_to_code
 
     @staticmethod
     def __cover_by_sound(samples: np.ndarray[np.float32], words_to_delete: list[tuple], mode: str) -> None:
         if mode == 's':
             for i in words_to_delete:
-                if (samples.ndim == 1):
+                if samples.ndim == 1:
                     samples[i[0]:i[1]] = np.zeros(i[1] - i[0])
                 else:
                     samples[i[0]:i[1]] = np.zeros((i[1] - i[0], samples.ndim))
         if mode == 'b':
             for i in words_to_delete:
-                if (samples.ndim == 1):
+                if samples.ndim == 1:
                     samples[i[0]:i[1]] = librosa.tone(600, length=i[1] - i[0], sr=16000)
                 else:
                     samples[i[0]:i[1]] = np.tile((librosa.tone(600, length=i[1] - i[0], sr=16000)),
                                                  (samples.ndim, 1)).transpose()
 
     def __init__(self):
         self.ASR = SpeechRecognitionModel("rmgaliullin/wav2vec2-based-obscenity-detector", letter_case='lowercase')
@@ -65,15 +64,15 @@
         origin_sr = audio_file.samplerate
         logger.info(
             f"Audio is loaded with {origin_sr} sample rate, {audio_file.channels} channels, type {audio_file.subtype}")
         resampled_audio = self.resample_audio(audio_path, 16000)
 
         # y, sr = librosa.load(resampled_audio, mono=True, sr=16000)
 
-        words_to_delete = self.__find_words(self.ASR.transcribe([resampled_audio]), origin_sr)
+        words_to_delete = self.__find_words(self.ASR.transcribe([resampled_audio])[0], origin_sr)
         self.__cover_by_sound(origin_samples, words_to_delete, mode)
 
         directory = os.path.dirname(audio_path)
         full_name = os.path.basename(audio_path)
 
         sf.write(os.path.join(directory, "result_" + full_name), origin_samples, origin_sr, format='wav',
                  subtype=audio_file.subtype)
@@ -87,73 +86,105 @@
         full_name = os.path.basename(audio_path)
         y, sr = librosa.load(audio_path)
         y = librosa.to_mono(y)
         new_samples = librosa.resample(y, orig_sr=sr, target_sr=target_rate)
         sf.write(os.path.join(directory, "RS_" + full_name), new_samples, target_rate, format='wav', subtype="PCM_16")
         return os.path.join(directory, "RS_" + full_name)
 
-    def __ow_probability(self, word: str, probabilities: list[float]) -> float:
+    def __ow_probability(self, word: str, probabilities: list[float]) -> (float, int):
         result = 0
+        res_ow = ''
         word_t = ObscenityWordsRecognizer.soundex.transform(word)
         s_len = int(len(word_t) / 3)
-        for ow in self.__phonetic_word_codes[1].keys():
+        for ow in self.__phonetic_word_codes.keys():
             if word_t[0:s_len] == ObscenityWordsRecognizer.soundex.transform(ow)[0:s_len]:
                 indexes = pylcs.lcs_sequence_idx(word, ow)
                 probability = 0
                 for index, value in enumerate(indexes):
                     if value != -1:
                         probability += probabilities[index]
                 dist = Levenshtein.distance(ow, word)
                 probability = probability / max(len(word), len(ow))
-                result = max((probability / (dist + 1) ** 0.25) ** dist, result)
-        return int(result * 10) / 10
+                if (probability / (dist + 1) ** 0.25) ** dist >= result:
+                    result = (probability / (dist + 1) ** 0.25) ** dist
+                    res_ow = ow
+        return int(result * 10) / 10, res_ow
 
-    def __find_words(self, transcribe_result: list[dir], sample_rate: int) -> list[tuple]:
+    def __find_words(self, transcribe_result: dir, sample_rate: int, evaluation: list[str] = None) -> list[tuple]:
         o_words = []
-        sentence = transcribe_result[0]['transcription']
+        sentence = transcribe_result['transcription']
         logger.info(f"Transcription: {sentence}")
-        probabilities = transcribe_result[0]['probabilities']
-        start_timestamps = transcribe_result[0]["start_timestamps"]
-        end_timestamps = transcribe_result[0]["end_timestamps"]
+        probabilities = transcribe_result['probabilities']
+        start_timestamps = transcribe_result["start_timestamps"]
+        end_timestamps = transcribe_result["end_timestamps"]
 
         for length in range(2, 8):
             for i in range(0, len(sentence) - length + 1):
                 probability = self.__ow_probability(sentence[i:(i + length)], probabilities[i:(i + length)])
-                if probability >= 0.5:
-                    o_words.append((probability, length, i))
+                if probability[0] > 0.5:
+                    o_words.append((probability[0], length, i, probability[1]))
         o_words.sort()
         ow_timestamps = []
         recognized_ow_indexes = []
+        ows = []
         while len(o_words) != 0:
             word = o_words.pop()
             p = word[0]
-            word = (word[2], word[2] + word[1] - 1)
+            word = (word[2], word[2] + word[1] - 1, word[3])
             is_valid = True
             for w in recognized_ow_indexes:
                 if not ((word[0] < w[0] and word[1] < w[0]) or (w[0] < word[0] and w[1] < word[0])):
                     is_valid = False
+                    break
             if is_valid:
-                logger.info(f"Detected word: {sentence[word[0]:(word[1] + 1)]};  Probability: {p}")
+                logger.info(
+                    f"Detected word: {sentence[word[0]:(word[1] + 1)]};  Probability: {p}; Real word: {word[2]}")
+                ows.append(word[2])
                 recognized_ow_indexes.append(word)
                 length = word[1] - word[0] + 1
                 start = start_timestamps[word[0]] * (sample_rate // 1000)
                 end = end_timestamps[word[1]] * (sample_rate // 1000)
                 letter_len = (end - start) // length
                 start -= 2 * letter_len
-                end += 2 * letter_len 
+                end += 2 * letter_len
                 if start < 0:
                     start = 0
                 if end > end_timestamps[-1] * (sample_rate // 1000):
                     end = end_timestamps[-1] * (sample_rate // 1000)
                 ow_timestamps.append((start, end))
+        # ows - all recognised words
+        if evaluation != None:
+            evaluation.extend(ows)
         return ow_timestamps
 
+    def evaluate(self, audio_transcript_data):
+        data = []
+        cer_ow = 0
+        wer_ow = 0
+        true_positive = 0
+        total = 0
+        for audio_path, transcript_path in audio_transcript_data:
+            prediction_ow = []
+            text = open(transcript_path).read().strip()
+            data.append({'path': audio_path, 'transcription': text})
+            reference_ow = [i for i in self.__phonetic_word_codes.keys() if i in text]
+            self.__find_words(self.ASR.transcribe([audio_path])[0], 16000, prediction_ow)
+            true_positive += len(prediction_ow)
+            total += len(reference_ow)
+            cer_ow = cer(prediction_ow, reference_ow)
+            wer_ow = wer(prediction_ow, reference_ow)
+
+        return {"total cer": self.ASR.evaluate(data)["cer"],
+                "total wer": self.ASR.evaluate(data)["wer"],
+                "obscenity cer": cer_ow,
+                "obscenity wer": wer_ow,
+                "rate of word detection": true_positive / (1 if total == 0 else total)}
+
 
 if __name__ == "__main__":
     detector = ObscenityWordsRecognizer()
     dir_path = os.path.join(os.getcwd(), "data")
-    file_name = "AgADuykAAiQEkUoSL96illlSfCB5zPvoice.wav"
+    file_name = "audio_03.wav"
     playsound(os.path.join(dir_path, file_name))
     a = detector.mute_words(os.path.join(dir_path, file_name), "b")
     print(a)
     playsound(os.path.join(dir_path, "result_" + file_name))
-
```

### Comparing `OWR-2.3/OWR/data/obscenity_words.json` & `OWR-2.4/OWR/data/obscenity_words.json`

 * *Files 1% similar despite different names*

```diff
@@ -163,8 +163,8 @@
 00000a20: d0bd d0bd d18b d0b5 222c 0a20 2022 d0be  ........",.  "..
 00000a30: d185 d183 d0b5 d0bd d0bd d18b d185 222c  ..............",
 00000a40: 0a20 2022 d0be d185 d183 d0b5 d0bd d0bd  .  "............
 00000a50: d18b d0bc 222c 0a20 2022 d0be d185 d183  ....",.  "......
 00000a60: d0b5 d0bd d0bd d18b d0bc d0b8 222c 0a20  ............",. 
 00000a70: 2022 d187 d191 d180 d182 222c 0a20 2022   "........",.  "
 00000a80: d0ba d0b0 d0bf d0b5 d186 222c 0a20 2022  ..........",.  "
-00000a90: d0b6 d0b5 d181 d182 d18c 222c 0a5d 0a    ..........",.].
+00000a90: d0b6 d0b5 d181 d182 d18c 220a 5d0a       ..........".].
```

