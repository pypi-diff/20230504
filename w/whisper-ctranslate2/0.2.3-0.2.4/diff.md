# Comparing `tmp/whisper-ctranslate2-0.2.3.tar.gz` & `tmp/whisper-ctranslate2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.3.tar", last modified: Sat Apr 29 09:55:50 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.4.tar", last modified: Thu May  4 05:18:32 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.3.tar` & `whisper-ctranslate2-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.3/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.3/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 15:43:27.000000 whisper-ctranslate2-0.2.3/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4888 2023-04-28 15:31:31.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-04-29 07:49:33.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-27 16:20:26.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16957 2023-04-29 09:50:29.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10108 2023-04-29 09:43:21.000000 whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-29 09:55:50.876417 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5643 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-29 09:55:50.000000 whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.4/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.4/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 15:43:27.000000 whisper-ctranslate2-0.2.4/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.935876 whisper-ctranslate2-0.2.4/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5154 2023-05-03 14:33:47.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-05-01 06:35:27.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-03 14:00:51.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    17511 2023-05-03 17:29:49.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10279 2023-05-03 17:29:49.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.3/LICENSE` & `whisper-ctranslate2-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.3/PKG-INFO` & `whisper-ctranslate2-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.3
+Version: 0.2.4
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -128,9 +127,7 @@
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
-
-
```

### Comparing `whisper-ctranslate2-0.2.3/README.md` & `whisper-ctranslate2-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.3/setup.py` & `whisper-ctranslate2-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/live.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,27 +30,29 @@
         language: str,
         threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
         verbose: bool,
         threshold: float,
+        input_device: int,
         options: TranscriptionOptions,
     ):
         self.model_path = model_path
         self.cache_directory = cache_directory
         self.local_files_only = local_files_only
         self.task = task
         self.language = language
         self.threads = threads
         self.device = device
         self.device_index = device_index
         self.compute_type = compute_type
         self.verbose = verbose
         self.threshold = threshold
+        self.input_device = input_device
         self.options = options
 
         self.running = True
         self.waiting = 0
         self.prevblock = self.buffer = np.zeros((0, 1))
         self.speaking = False
         self.blocks_speaking = 0
@@ -133,20 +135,24 @@
                 options=self.options,
             )
             print(f"\033[1A\033[2K\033[0G{result['text']}")
             if not self.verbose:
                 print("")
 
     def listen(self):
+        print(
+            f"\033[32mLive stream device: \033[37m{sd.query_devices(device=self.input_device or sd.default.device[1])['name']}\033[0m"
+        )
         print("\033[32mListening.. \033[37m(Ctrl+C to Quit)\033[0m")
         with sd.InputStream(
             channels=1,
             callback=self.callback,
             blocksize=int(SampleRate * BlockSize / 1000),
             samplerate=SampleRate,
+            device=self.input_device,
         ):
             while self.running:
                 self.process()
 
     def inference(self):
         try:
             self.listen()
```

### Comparing `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 
 def optional_int(string):
     return None if string == "None" else int(string)
 
 
 def str2bool(string):
-    str2val = {"True": True, "False": False}
-    if string in str2val:
-        return str2val[string]
+    str2val = {"true": True, "false": False}
+    if string and string.lower() in str2val:
+        return str2val[string.lower()]
     else:
         raise ValueError(f"Expected one of {set(str2val.keys())}, got {string}")
 
 
 def optional_float(string):
     return None if string == "None" else float(string)
 
@@ -97,14 +97,22 @@
         type=str,
         default="all",
         choices=["txt", "vtt", "srt", "tsv", "json", "all"],
         help="format of the output file; if not specified, all available formats will be produced",
     )
 
     outputs_args.add_argument(
+        "--pretty_json",
+        "-p",
+        type=str2bool,
+        default=False,
+        help="produce json in a human redable format",
+    )
+
+    outputs_args.add_argument(
         "--print_colors",
         type=str2bool,
         default=False,
         help="print the transcribed text using an experimental color coding strategy to highlight words with high or low confidence",
     )
 
     outputs_args.add_argument(
@@ -340,14 +348,21 @@
     live_args.add_argument(
         "--live_volume_threshold",
         type=float,
         default=0.2,
         help="minimum volume threshold to activate listening in live transcribe mode",
     )
 
+    live_args.add_argument(
+        "--live_input_device",
+        type=int,
+        default=None,
+        help="Set live stream input device (python -m sounddevice)",
+    )
+
     return parser.parse_args().__dict__
 
 
 def _does_old_cache_dir_has_files():
     default = os.path.join(os.path.expanduser("~"), ".cache")
     cache_dir = os.path.join(
         os.getenv("XDG_CACHE_HOME", default), "whisper-ctranslate2"
@@ -371,15 +386,17 @@
     cache_directory: str = args.pop("model_dir")
     device_index: Union[int, List[int]] = args.pop("device_index")
     suppress_tokens: str = args.pop("suppress_tokens")
     live_transcribe: bool = args.pop("live_transcribe")
     audio: str = args.pop("audio")
     local_files_only: bool = args.pop("local_files_only")
     live_volume_threshold: float = args.pop("live_volume_threshold")
+    live_input_device: int = args.pop("live_input_device")
     temperature = args.pop("temperature")
+
     if (increment := args.pop("temperature_increment_on_fallback")) is not None:
         temperature = tuple(np.arange(temperature, 1.0 + 1e-6, increment))
     else:
         temperature = [temperature]
 
     language = from_language_to_iso_code(language)
 
@@ -431,15 +448,17 @@
             if args[option]:
                 sys.stderr.write(f"--{option} requires --word_timestamps True\n")
                 return
 
     if args["max_line_count"] and not args["max_line_width"]:
         warnings.warn("--max_line_count has no effect without --max_line_width")
 
-    writer_args = {arg: args.pop(arg) for arg in word_options}
+    writer_options = list(word_options)
+    writer_options.append("pretty_json")
+    writer_args = {arg: args.pop(arg) for arg in writer_options}
 
     if verbose:
         cache_dir, exists = _does_old_cache_dir_has_files()
         if exists:
             print(
                 f"There are old cache files at `{cache_dir}` which are no longer used. Consider deleting them"
             )
@@ -484,14 +503,15 @@
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
             live_volume_threshold,
+            live_input_device,
             options,
         ).inference()
 
         return
 
     for audio_path in audio:
         result = Transcribe().inference(
```

### Comparing `whisper-ctranslate2-0.2.3/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,20 @@
             print(segment["text"].strip().replace("\t", " "), file=file, flush=True)
 
 
 class WriteJSON(ResultWriter):
     extension: str = "json"
 
     def write_result(self, result: dict, file: TextIO, options: dict):
-        json.dump(result, file)
+        pretty_json: bool = options.get("pretty_json", False)
+
+        if pretty_json:
+            json.dump(result, file, indent=4, ensure_ascii=False)
+        else:
+            json.dump(result, file)
 
 
 def get_writer(
     output_format: str, output_dir: str
 ) -> Callable[[dict, TextIO, dict], None]:
     writers = {
         "txt": WriteTXT,
```

### Comparing `whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.3
+Version: 0.2.4
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -128,9 +127,7 @@
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
-
-
```

### Comparing `whisper-ctranslate2-0.2.3/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

