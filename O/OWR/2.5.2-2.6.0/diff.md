# Comparing `tmp/OWR-2.5.2.tar.gz` & `tmp/OWR-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.5.2.tar", last modified: Thu May  4 13:05:34 2023, max compression
+gzip compressed data, was "OWR-2.6.0.tar", last modified: Thu May  4 14:10:43 2023, max compression
```

## Comparing `OWR-2.5.2.tar` & `OWR-2.6.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 13:05:34.195719 OWR-2.5.2/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.5.2/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 13:05:34.195719 OWR-2.5.2/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8299 2023-05-04 13:05:20.000000 OWR-2.5.2/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 13:05:34.195719 OWR-2.5.2/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2718 2023-05-04 12:54:04.000000 OWR-2.5.2/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 13:05:34.195719 OWR-2.5.2/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 13:05:34.000000 OWR-2.5.2/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 13:05:34.000000 OWR-2.5.2/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 13:05:34.000000 OWR-2.5.2/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 13:05:34.000000 OWR-2.5.2/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 13:05:34.000000 OWR-2.5.2/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 13:05:34.195719 OWR-2.5.2/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 12:54:04.000000 OWR-2.5.2/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 13:05:34.195719 OWR-2.5.2/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-04 12:54:31.000000 OWR-2.5.2/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.6.0/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8319 2023-05-04 14:04:42.000000 OWR-2.6.0/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:10:43.617809 OWR-2.6.0/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 14:01:03.000000 OWR-2.6.0/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 14:10:43.617809 OWR-2.6.0/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      693 2023-05-04 14:09:49.000000 OWR-2.6.0/setup.py
```

### Comparing `OWR-2.5.2/LICENSE` & `OWR-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.5.2/OWR/__init__.py` & `OWR-2.6.0/OWR/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,19 @@
         sf.write(os.path.join(directory, "RS_" + full_name), new_samples, target_rate, format='wav', subtype="PCM_16")
         return os.path.join(directory, "RS_" + full_name)
 
     def __ow_probability(self, word: str, probabilities: list[float]) -> (float, int):
         result = 0
         res_ow = ''
         word_t = ObscenityWordsRecognizer.soundex.transform(word)
-        s_len = (int(len(word_t) / 3) + 1) if (len(word_t) >= int(len(word_t) / 3) + 1) else len(word_t)
+        s_len = min(int((len(word_t) + 1) / 2), len(word_t))
         for ow in self.__phonetic_word_codes.keys():
-            if word_t[0:s_len] == ObscenityWordsRecognizer.soundex.transform(ow)[0:s_len]:
+            ow_t = ObscenityWordsRecognizer.soundex.transform(ow)
+            ow_s = min(len(ow_t), s_len)
+            if word_t[0:ow_s] == ow_t[0:ow_s]:
                 indexes = pylcs.lcs_sequence_idx(word, ow)
                 probability = 0
                 for index, value in enumerate(indexes):
                     if value != -1:
                         probability += probabilities[index]
                 dist = Levenshtein.distance(ow, word)
                 probability = probability / max(len(word), len(ow))
@@ -183,7 +185,8 @@
     evaluation = detector.evaluate(
         [{'audio_path': os.path.join("test", "audio", f'audio_{i}.wav'),
           'transcript_path': os.path.join("test", "transcript", f'transcript_{i}.txt')}
          for i in range(6)
          ])
     with open(os.path.join("test", 'result.json'), 'w') as outfile:
         outfile.write(json.dumps(evaluation))
+
```

### Comparing `OWR-2.5.2/setup.py` & `OWR-2.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.5.2',
+    version='2.6.0',
     description='Obscene word recognition package',
     url='https://github.com/RuslanGaliullin/FFixTelegramBot/tree/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
-    package_data={'': ['data/obscenity_words.json']},
     include_package_data=True,
     install_requires=['scikit-learn',
                       'huggingsound',
                       'librosa',
                       'levenshtein',
                       'soundfile',
                       'fonetika',
```

