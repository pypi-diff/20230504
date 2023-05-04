# Comparing `tmp/miditok-2.0.4.tar.gz` & `tmp/miditok-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.0.4.tar", last modified: Tue May  2 11:40:35 2023, max compression
+gzip compressed data, was "miditok-2.0.5.tar", last modified: Thu May  4 16:33:33 2023, max compression
```

## Comparing `miditok-2.0.4.tar` & `miditok-2.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 11:40:20.000000 miditok-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-02 11:40:35.005035 miditok-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-02 11:40:20.000000 miditok-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    83576 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-02 11:40:20.000000 miditok-2.0.4/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.001035 miditok-2.0.4/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 11:40:34.000000 miditok-2.0.4/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:40:35.005035 miditok-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 11:40:20.000000 miditok-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:40:35.005035 miditok-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_bpe_slow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 11:40:20.000000 miditok-2.0.4/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 16:33:14.000000 miditok-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-04 16:33:33.896236 miditok-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-04 16:33:14.000000 miditok-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86192 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:33:33.896236 miditok-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 16:33:14.000000 miditok-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_bpe_slow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/tests_utils.py
```

### Comparing `miditok-2.0.4/LICENSE` & `miditok-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/PKG-INFO` & `miditok-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.4
+Version: 2.0.5
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.0.4/README.md` & `miditok-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/classes.py` & `miditok-2.0.5/miditok/classes.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/constants.py` & `miditok-2.0.5/miditok/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.0.4"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.0.5"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
```

### Comparing `miditok-2.0.4/miditok/data_augmentation/data_augmentation.py` & `miditok-2.0.5/miditok/data_augmentation/data_augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,17 @@
                 Tuple[int, int, int], List[Union[int, List[int]]]
             ] = {}
             for track, (_, is_drum) in zip(ids, programs):
                 if is_drum:  # we dont augment drums
                     continue
                 corrected_offsets = deepcopy(offsets)
                 vel_dim = int(128 / len(tokenizer.velocities))
-                corrected_offsets[1] = [int(off / vel_dim) for off in corrected_offsets[1]]
+                corrected_offsets[1] = [
+                    int(off / vel_dim) for off in corrected_offsets[1]
+                ]
                 aug = data_augmentation_tokens(
                     np.array(track),
                     tokenizer,
                     *corrected_offsets,
                     all_offset_combinations=all_offset_combinations,
                 )
                 if len(aug) == 0:
```

### Comparing `miditok-2.0.4/miditok/midi_tokenizer.py` & `miditok-2.0.5/miditok/midi_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1000,26 +1000,77 @@
         :param vocab_size: size of the vocabulary to learn / build.
         :param iterator: an iterable object yielding the training data, as lists of string.
             It can be a list or a Generator. This iterator will be passed to the BPE model for
             training. If None is given, you must use the ``tokens_paths`` argument. (default: None)
         :param tokens_paths: paths of the token json files to load and use. (default: False)
         :param start_from_empty_voc: the training will start from an empty base vocabulary.
             The tokenizer will then have a base vocabulary only based on the unique bytes present
-            in the training data. If you set this argument to True, you should probably then use the
-            tokenizer only with the training data, as new data might contain "unknown" tokens
-            missing from the vocabulary. (default: False)
+            in the training data. If you set this argument to True, you should use the tokenizer only
+            with the training data, as new data might contain "unknown" tokens missing from the vocabulary.
+            Comparing this to text, setting this argument to True would create a tokenizer that will only know
+            the characters present in the training data, and would not be compatible / know other characters.
+            This argument can allow to optimize the vocabulary size.
+            If you are unsure about this, leave it to False. (default: False)
         :param kwargs: any additional argument to pass to the trainer.
         """
+        if self.is_multi_voc:
+            print(
+                "This tokenizer is based on multiple vocabularies / embedding pooling. It is therefore not compatible"
+                "with Byte Pair Encoding (BPE). Skipping this function call (learn_bpe)."
+            )
+            return
         assert (
             not self.bpe_slow
         ), "This tokenizer has already been trained with slow BPE. You can't retrain it with fast BPE"
         assert (
             iterator is not None or tokens_paths is not None
         ), "You must give at an iterator or a path to to token "
 
+        if vocab_size <= len(self.vocab):
+            print(
+                f"vocab_size ({vocab_size}) need to be higher than the size of the current vocabulary "
+                f"({len(self.vocab)}). Skipping BPE training."
+            )
+            return
+
+        # If no iterator, loads tokens / samples to analyze
+        if iterator is None:
+            iterator = []  # list of lists of one string (bytes)
+            for file_path in tqdm(tokens_paths, desc="Loading token files"):
+                sample = self.load_tokens(file_path)
+                bytes_ = self._ids_to_bytes(
+                    sample["ids"], as_one_str=True
+                )  # list of str (bytes)
+                iterator += (
+                    [[byte_] for byte_ in bytes_]
+                    if not self.unique_track
+                    else [[bytes_]]
+                )
+
+            # This doesn't seem to work, the trainer pre-processes the sequences, but then no word remains
+            """def it_gen():
+                for file_path_ in tqdm(tokens_paths, desc="Loading token files"):
+                    sample_ = self.load_tokens(file_path_)
+                    yield self._ids_to_bytes(sample_["ids"], as_one_str=True)
+
+            iterator = it_gen()"""
+
+            # Make sure the target vocab size > nb of unique chars across all samples
+            unique_chars = set()
+            for seq in iterator:
+                unique_chars.update(*seq)
+
+            if len(unique_chars) >= vocab_size:
+                print(
+                    f"BPE TRAINING: the provided data comprises {len(unique_chars)} base tokens (character level), "
+                    f"whereas the target BPE vocaulary size is inferior ({vocab_size}). No new token can be learned, "
+                    f"skipping BPE training."
+                )
+                return
+
         # Create new tokenizer model
         if self._bpe_model is None or start_from_empty_voc:
             nb_bytes = (
                 len(self.special_tokens)
                 if start_from_empty_voc
                 else len(self._vocab_base)
             )
@@ -1031,33 +1082,14 @@
                     dropout=None,
                     continuing_subword_prefix="",
                     end_of_word_suffix="",
                     fuse_unk=False,
                 )
             )
 
-        # If no iterator, loads tokens / samples to analyze
-        if iterator is None:
-            samples = []  # list of lists of one string (bytes)
-            for file_path in tqdm(tokens_paths, desc="Loading token files"):
-                sample = self.load_tokens(file_path)
-                bytes_ = self._ids_to_bytes(
-                    sample["ids"], as_one_str=True
-                )  # list of str (bytes)
-                samples += [[byte_] for byte_ in bytes_]
-            iterator = samples  # List of Lists of just one str
-
-            # This doesn't seem to work, the trainer pre-processes the sequences, but then no word remains
-            """def it_gen():
-                for file_path_ in tqdm(tokens_paths, desc="Loading token files"):
-                    sample_ = self.load_tokens(file_path_)
-                    yield self._ids_to_bytes(sample_["ids"], as_one_str=True)
-
-            iterator = it_gen()"""
-
         # Trains the tokenizer
         special_tokens_bytes = self._ids_to_bytes(
             self._tokens_to_ids([f"{tok}_None" for tok in self.special_tokens])
         )
         trainer = BpeTrainer(
             vocab_size=vocab_size,
             special_tokens=special_tokens_bytes,
@@ -1145,15 +1177,16 @@
         tokens_path: Union[Path, str],
         vocab_size: int,
         out_dir: Union[Path, str] = None,
         files_lim: int = None,
         save_converted_samples: bool = False,
         print_seq_len_variation: bool = True,
     ) -> Tuple[List[float], List[int], List[float]]:
-        r"""Method to construct the vocabulary from BPE, 100% in Python and slower than
+        r"""**DEPRECIATED - WILL BE REMOVED IN FUTURE UPDATES**
+        Method to construct the vocabulary from BPE, 100% in Python and slower than
         :py:func:`miditok.MIDITokenizer.learn_bpe`.
         This method will build (modify) the vocabulary by analyzing an already tokenized dataset to find
         the most recurrent token successions.
         **Note that this implementation is in pure Python and will be slow if you use a large amount of
         tokens files.** It will also not be updated in the future. We advise to use the fast
         :py:func:`miditok.MIDITokenizer.learn_bpe` method.
 
@@ -1167,14 +1200,18 @@
                 and the variation in %. (default: True)
         :return: learning metrics, as lists of:
                 - the average number of token combinations covered by the newly created BPE tokens
                 - the maximum number of token combinations
                 - the average sequence length
                 Each index in the list correspond to a learning step.
         """
+        print(
+            "You are using the slow BPE method, which is depreciated and will be removed in future updates."
+            "We recommend to use the learn_bpe method for much faster (x30-50) learning, encoding and decoding."
+        )
         assert not self.is_multi_voc, (
             "You are using a multi-vocabulary tokenizer, "
             "it is not compatible with byte pair encoding"
         )
         assert (
             not self.has_bpe and not self.bpe_slow
         ), "This tokenizer has already been trained with fast BPE. You can't retrain it with slow BPE."
@@ -1493,15 +1530,15 @@
         If save_programs is True, the shape will be [(T, *), (T, 2)], first dim is tokens and programs instead,
         for programs the first value is the program, second a bool indicating if the track is drums.
         The config of the tokenizer will be saved as a "config.txt" file by default.
 
         :param midi_paths: paths of the MIDI files.
         :param out_dir: output directory to save the converted files.
         :param validation_fn: a function checking if the MIDI is valid on your requirements
-                            (e.g. time signature, minimum/maximum length, instruments ...).
+            (e.g. time signature, minimum/maximum length, instruments ...).
         :param data_augment_offsets: data augmentation arguments, to be passed to the
             miditok.data_augmentation.data_augmentation_dataset method. Has to be given as a list / tuple
             of offsets pitch octaves, velocities, durations, and finally their directions (up/down). (default: None)
         :param apply_bpe: will apply BPE on the dataset to save, if the vocabulary was learned with.
         :param save_programs: will also save the programs of the tracks of the MIDI. (default: True)
         :param logging: logs progress bar.
         """
@@ -1838,23 +1875,34 @@
         return (
             f'{len(self.len)} tokens {"(multi-voc) " if self.is_multi_voc else ""}'
             f'{"with BPE" if self.has_bpe else "without BPE"}'
         )
 
     def __getitem__(
         self, item: Union[int, str, Tuple[int, Union[int, str]]]
-    ) -> Union[str, int]:
+    ) -> Union[str, int, List[int]]:
         r"""Convert a token (int) to an event (str), or vice-versa.
 
-        :param item: a token (int) or an event (str). For embedding pooling, you must
-                provide a tuple where the first element in the index of the vocabulary.
+        :param item: a token (int) or an event (str). For tokenizers with embedding pooling / multiple vocabularies
+            ( `tokenizer.is_multi_voc` ), you must either provide a string (token) that is within all vocabularies (e.g.
+            special tokens), or a tuple where the first element in the index of the vocabulary and the second the
+            element to index.
         :return: the converted object.
         """
         if isinstance(item, tuple) and self.is_multi_voc:
             return self.__get_from_voc(item[1], item[0])
+        elif self.is_multi_voc and isinstance(item, str):
+            if all(item in voc for voc in self.vocab):
+                return [voc[item] for voc in self.vocab]
+            else:
+                raise ValueError(
+                    "This tokenizer uses multiple vocabularies / embedding pooling. To index it you must"
+                    "either provide a token (string) that is within all vocabularies (e.g. special tokens), or a tuple"
+                    "where the first element in the index of the vocabulary and the second the element to index."
+                )
         else:
             return self.__get_from_voc(item)
 
     def __get_from_voc(
         self, item: Union[int, str], vocab_id: int = None
     ) -> Union[int, str]:
         r"""Get element from the vocabulary.
```

### Comparing `miditok-2.0.4/miditok/tokenizations/cp_word.py` & `miditok-2.0.5/miditok/tokenizations/cp_word.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/midi_like.py` & `miditok-2.0.5/miditok/tokenizations/midi_like.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/mumidi.py` & `miditok-2.0.5/miditok/tokenizations/mumidi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/octuple.py` & `miditok-2.0.5/miditok/tokenizations/octuple.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/octuple_mono.py` & `miditok-2.0.5/miditok/tokenizations/octuple_mono.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/remi.py` & `miditok-2.0.5/miditok/tokenizations/remi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/remi_plus.py` & `miditok-2.0.5/miditok/tokenizations/remi_plus.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/structured.py` & `miditok-2.0.5/miditok/tokenizations/structured.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/tokenizations/tsd.py` & `miditok-2.0.5/miditok/tokenizations/tsd.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok/utils/utils.py` & `miditok-2.0.5/miditok/utils/utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/miditok.egg-info/PKG-INFO` & `miditok-2.0.5/miditok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.4
+Version: 2.0.5
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `miditok-2.0.4/miditok.egg-info/SOURCES.txt` & `miditok-2.0.5/miditok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/setup.py` & `miditok-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='miditok',
     author='Nathan Fradet',
     url='https://github.com/Natooz/MidiTok',
     packages=find_packages(exclude=("tests",)),
-    version='2.0.4',
+    version='2.0.5',
     license='MIT',
     description='A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         'artificial intelligence',
         'deep learning',
```

### Comparing `miditok-2.0.4/tests/test_bpe.py` & `miditok-2.0.5/tests/test_bpe.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,18 @@
         tokenizer: miditok.MIDITokenizer = getattr(miditok, tokenization)(
             beat_res=BEAT_RES_TEST, additional_tokens=add_tokens
         )
         tokenizer.tokenize_midi_dataset(
             files, Path("tests", "test_results", tokenization)
         )
         tokenizer.learn_bpe(
-            vocab_size=400,
-            tokens_paths=list(Path("tests", "test_results", tokenization).glob("**/*.json")),
+            vocab_size=len(tokenizer) + 400,
+            tokens_paths=list(
+                Path("tests", "test_results", tokenization).glob("**/*.json")
+            ),
             start_from_empty_voc=True,
         )
         tokenizer.save_params(
             Path("tests", "test_results", f"{tokenization}_bpe", "config.txt")
         )
         first_tokenizers.append(tokenizer)
 
@@ -138,21 +140,17 @@
     tok_times = []
     for tokenization, tokenizer in zip(tokenizations, tokenizers):
         samples_no_bpe = []
         for i, file_path in enumerate(tqdm(files, desc="Testing BPE batched")):
             # Reads the midi
             midi = MidiFile(file_path)
             if not tokenizer.unique_track:
-                samples_no_bpe.append(
-                    tokenizer(midi, apply_bpe_if_possible=False)[0]
-                )
+                samples_no_bpe.append(tokenizer(midi, apply_bpe_if_possible=False)[0])
             else:
-                samples_no_bpe.append(
-                    tokenizer(midi, apply_bpe_if_possible=False)
-                )
+                samples_no_bpe.append(tokenizer(midi, apply_bpe_if_possible=False))
 
         t0 = time()
         samples_bpe = deepcopy(samples_no_bpe)
         tokenizer.apply_bpe(samples_bpe)
         tok_times.append((time() - t0) / len(files))
 
         samples_bpe_decoded = deepcopy(samples_bpe)
```

### Comparing `miditok-2.0.4/tests/test_bpe_slow.py` & `miditok-2.0.5/tests/test_bpe_slow.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,17 @@
                 Path(
                     "tests",
                     "test_results",
                     f"{tokenization}_bpe",
                     f"{file_path.stem}.json",
                 )
             ) as json_file:
-                saved_tokens = json.load(json_file)["ids"]  # with BPE, saved after creating vocab
+                saved_tokens = json.load(json_file)[
+                    "ids"
+                ]  # with BPE, saved after creating vocab
             if not tokenizer.unique_track:
                 saved_tokens = saved_tokens[0]
             saved_tokens = miditok.TokSequence(ids=saved_tokens, ids_bpe_encoded=True)
             saved_tokens_decomposed = deepcopy(saved_tokens)
             tokenizer.decode_bpe(saved_tokens_decomposed)
             no_error_bpe = tokens == saved_tokens
             no_error = tokens_no_bpe == tokens_bpe_decomposed == saved_tokens_decomposed
```

### Comparing `miditok-2.0.4/tests/test_methods.py` & `miditok-2.0.5/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/tests/test_multitrack.py` & `miditok-2.0.5/tests/test_multitrack.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/tests/test_one_track.py` & `miditok-2.0.5/tests/test_one_track.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/tests/test_saving_loading_config.py` & `miditok-2.0.5/tests/test_saving_loading_config.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.4/tests/test_utils.py` & `miditok-2.0.5/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 from pathlib import Path
 from copy import deepcopy
 
 from miditoolkit import MidiFile
 
 from miditok import REMI
-from miditok.utils import merge_tracks, merge_tracks_per_class, merge_same_program_tracks, nb_bar_pos
+from miditok.utils import (
+    merge_tracks,
+    merge_tracks_per_class,
+    merge_same_program_tracks,
+    nb_bar_pos,
+)
 from miditok.constants import CLASS_OF_INST
 
 
 def test_merge_tracks():
     midi = MidiFile(Path("tests", "Maestro_MIDIs", "Maestro_1.mid"))
     original_track = deepcopy(midi.instruments[0])
     midi.instruments.append(deepcopy(midi.instruments[0]))
@@ -51,15 +56,15 @@
 
 
 def test_nb_pos():
     tokenizer = REMI()
     _ = nb_bar_pos(
         tokenizer(Path("tests", "Maestro_MIDIs", "Maestro_1.mid"))[0].ids,
         tokenizer["Bar_None"],
-        tokenizer.token_ids_of_type("Position")
+        tokenizer.token_ids_of_type("Position"),
     )
 
 
 if __name__ == "__main__":
     test_merge_tracks()
     test_merge_same_program_tracks_and_by_class()
     test_nb_pos()
```

### Comparing `miditok-2.0.4/tests/tests_utils.py` & `miditok-2.0.5/tests/tests_utils.py`

 * *Files identical despite different names*

