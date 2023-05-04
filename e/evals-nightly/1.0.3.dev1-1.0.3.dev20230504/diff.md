# Comparing `tmp/evals-nightly-1.0.3.dev1.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev1.tar", last modified: Tue May  2 22:36:46 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230504.tar", last modified: Thu May  4 20:21:55 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev1.tar` & `evals-nightly-1.0.3.dev20230504.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.051692 evals-nightly-1.0.3.dev1/
--rw-r--r--   0 alvin      (502) staff       (20)     1063 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/LICENSE
--rw-r--r--   0 alvin      (502) staff       (20)      136 2023-05-02 22:36:33.000000 evals-nightly-1.0.3.dev1/MANIFEST.in
--rw-r--r--   0 alvin      (502) staff       (20)      107 2023-05-02 22:36:46.051391 evals-nightly-1.0.3.dev1/PKG-INFO
--rw-r--r--   0 alvin      (502) staff       (20)     5239 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/README.md
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.981558 evals-nightly-1.0.3.dev1/evals/
--rw-r--r--   0 alvin      (502) staff       (20)      316 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/__init__.py
--rw-r--r--   0 alvin      (502) staff       (20)     2964 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/api.py
--rw-r--r--   0 alvin      (502) staff       (20)     1900 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/base.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.982803 evals-nightly-1.0.3.dev1/evals/cli/
--rw-r--r--   0 alvin      (502) staff       (20)     5645 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/cli/oaieval.py
--rw-r--r--   0 alvin      (502) staff       (20)     3294 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/cli/oaievalset.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.992226 evals-nightly-1.0.3.dev1/evals/completion_fns/
--rw-r--r--   0 alvin      (502) staff       (20)        0 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/__init__.py
--rw-r--r--   0 alvin      (502) staff       (20)     2678 2023-04-11 18:52:38.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/cot.py
--rw-r--r--   0 alvin      (502) staff       (20)     1245 2023-04-11 18:52:38.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 alvin      (502) staff       (20)     1068 2023-04-11 18:52:38.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/langchain_math.py
--rw-r--r--   0 alvin      (502) staff       (20)     4941 2023-04-11 18:52:38.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/openai.py
--rw-r--r--   0 alvin      (502) staff       (20)     4422 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/completion_fns/retrieval.py
--rw-r--r--   0 alvin      (502) staff       (20)     5699 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/data.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.993235 evals-nightly-1.0.3.dev1/evals/elsuite/
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.995827 evals-nightly-1.0.3.dev1/evals/elsuite/basic/
--rw-r--r--   0 alvin      (502) staff       (20)     1755 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 alvin      (502) staff       (20)     1085 2023-04-24 18:44:58.000000 evals-nightly-1.0.3.dev1/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 alvin      (502) staff       (20)     1241 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/elsuite/basic/includes.py
--rw-r--r--   0 alvin      (502) staff       (20)     1185 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 alvin      (502) staff       (20)     1831 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/elsuite/basic/match.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.997287 evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/
--rw-r--r--   0 alvin      (502) staff       (20)      624 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 alvin      (502) staff       (20)     4832 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 alvin      (502) staff       (20)     7590 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 alvin      (502) staff       (20)     2682 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/elsuite/translate.py
--rw-r--r--   0 alvin      (502) staff       (20)     6436 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/elsuite/utils.py
--rw-r--r--   0 alvin      (502) staff       (20)     5534 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/eval.py
--rw-r--r--   0 alvin      (502) staff       (20)     1137 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/formatting.py
--rw-r--r--   0 alvin      (502) staff       (20)     2455 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/metrics.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.997801 evals-nightly-1.0.3.dev1/evals/prompt/
--rw-r--r--   0 alvin      (502) staff       (20)     4093 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/prompt/base.py
--rw-r--r--   0 alvin      (502) staff       (20)    17356 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/record.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.964031 evals-nightly-1.0.3.dev1/evals/registry/
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:45.999523 evals-nightly-1.0.3.dev1/evals/registry/completion_fns/
--rw-r--r--   0 alvin      (502) staff       (20)      391 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      103 2023-04-11 17:31:12.000000 evals-nightly-1.0.3.dev1/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      524 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.004306 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/
--rw-r--r--   0 alvin      (502) staff       (20)      141 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      119 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      560 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      454 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      113 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      312 2023-04-11 01:08:32.000000 evals-nightly-1.0.3.dev1/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.044859 evals-nightly-1.0.3.dev1/evals/registry/evals/
--rw-r--r--   0 alvin      (502) staff       (20)      215 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      297 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      457 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      229 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      196 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/banking77.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      310 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      159 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      246 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/born-first.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      288 2023-04-11 17:31:12.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      305 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      573 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      309 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/chess.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      308 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      250 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      160 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      335 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1719 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      151 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/crepe.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      167 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      175 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/determinant.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      202 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      377 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      306 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      269 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      387 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      195 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      314 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      254 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/finance.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      183 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      276 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      928 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      194 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      258 2023-04-11 18:41:58.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      250 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      170 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      265 2023-03-29 22:37:58.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      222 2023-03-28 19:03:05.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      347 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      262 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/invoices.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      292 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      382 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      754 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      327 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      198 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      242 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      153 2023-04-11 18:52:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      262 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      674 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      278 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      159 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      215 2023-03-27 23:41:39.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      211 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1193 2023-04-11 17:31:12.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      186 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      292 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      258 2023-03-27 23:41:39.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      221 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      287 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      188 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      320 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      282 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/qa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      175 2023-03-28 19:03:05.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      378 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      255 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/rot13.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      236 2023-04-11 00:58:32.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/rucola.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      364 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/russe.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      199 2023-03-27 23:41:39.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      254 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      190 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      274 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      364 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      374 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1053 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/sql.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     4472 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      272 2023-04-11 18:41:58.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      150 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/taxes.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      399 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1218 2023-04-15 00:45:06.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      400 2023-03-21 21:09:38.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1271 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      347 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     3040 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      323 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      174 2023-03-28 19:03:05.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      189 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      365 2023-03-27 23:41:39.000000 evals-nightly-1.0.3.dev1/evals/registry/evals/which-is-heavier.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.047820 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/
--rw-r--r--   0 alvin      (502) staff       (20)      492 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      263 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      831 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      246 2023-05-02 22:06:46.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1157 2023-03-27 20:17:04.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     2564 2023-04-11 01:08:32.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-04-11 17:31:12.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1152 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     9600 2023-04-11 17:31:12.000000 evals-nightly-1.0.3.dev1/evals/registry.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.049009 evals-nightly-1.0.3.dev1/evals/utils/
--rw-r--r--   0 alvin      (502) staff       (20)     1504 2023-04-11 01:12:50.000000 evals-nightly-1.0.3.dev1/evals/utils/api_utils.py
--rw-r--r--   0 alvin      (502) staff       (20)      713 2023-03-16 23:15:22.000000 evals-nightly-1.0.3.dev1/evals/utils/misc.py
--rw-r--r--   0 alvin      (502) staff       (20)     4076 2023-04-24 18:26:26.000000 evals-nightly-1.0.3.dev1/evals/utils/snowflake.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-02 22:36:46.051045 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/
--rw-r--r--   0 alvin      (502) staff       (20)      107 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 alvin      (502) staff       (20)     5858 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 alvin      (502) staff       (20)        1 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 alvin      (502) staff       (20)       90 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 alvin      (502) staff       (20)      207 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 alvin      (502) staff       (20)        6 2023-05-02 22:36:45.000000 evals-nightly-1.0.3.dev1/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 alvin      (502) staff       (20)      559 2023-05-02 22:36:35.000000 evals-nightly-1.0.3.dev1/pyproject.toml
--rw-r--r--   0 alvin      (502) staff       (20)       38 2023-05-02 22:36:46.051763 evals-nightly-1.0.3.dev1/setup.cfg
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.438223 evals-nightly-1.0.3.dev20230504/
+-rw-r--r--   0 alvin      (502) staff       (20)     1063 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/LICENSE
+-rw-r--r--   0 alvin      (502) staff       (20)      136 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/MANIFEST.in
+-rw-r--r--   0 alvin      (502) staff       (20)      114 2023-05-04 20:21:55.437795 evals-nightly-1.0.3.dev20230504/PKG-INFO
+-rw-r--r--   0 alvin      (502) staff       (20)     5239 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/README.md
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.217764 evals-nightly-1.0.3.dev20230504/evals/
+-rw-r--r--   0 alvin      (502) staff       (20)      316 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/__init__.py
+-rw-r--r--   0 alvin      (502) staff       (20)     2964 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/api.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1900 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/base.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.223085 evals-nightly-1.0.3.dev20230504/evals/cli/
+-rw-r--r--   0 alvin      (502) staff       (20)     5645 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/cli/oaieval.py
+-rw-r--r--   0 alvin      (502) staff       (20)     3294 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/cli/oaievalset.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.236097 evals-nightly-1.0.3.dev20230504/evals/completion_fns/
+-rw-r--r--   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/__init__.py
+-rw-r--r--   0 alvin      (502) staff       (20)     2678 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/cot.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1245 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1068 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 alvin      (502) staff       (20)     4941 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/openai.py
+-rw-r--r--   0 alvin      (502) staff       (20)     4422 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/completion_fns/retrieval.py
+-rw-r--r--   0 alvin      (502) staff       (20)     5699 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/data.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.241943 evals-nightly-1.0.3.dev20230504/evals/elsuite/
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.250361 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/
+-rw-r--r--   0 alvin      (502) staff       (20)     1755 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1085 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1241 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/includes.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1185 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1831 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/match.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.256274 evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/
+-rw-r--r--   0 alvin      (502) staff       (20)      624 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 alvin      (502) staff       (20)     4832 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 alvin      (502) staff       (20)     7590 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 alvin      (502) staff       (20)     2682 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/translate.py
+-rw-r--r--   0 alvin      (502) staff       (20)     6436 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/elsuite/utils.py
+-rw-r--r--   0 alvin      (502) staff       (20)     5534 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/eval.py
+-rw-r--r--   0 alvin      (502) staff       (20)     1137 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/formatting.py
+-rw-r--r--   0 alvin      (502) staff       (20)     2455 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/metrics.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.260209 evals-nightly-1.0.3.dev20230504/evals/prompt/
+-rw-r--r--   0 alvin      (502) staff       (20)     4093 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/prompt/base.py
+-rw-r--r--   0 alvin      (502) staff       (20)    17356 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/record.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.185873 evals-nightly-1.0.3.dev20230504/evals/registry/
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.264107 evals-nightly-1.0.3.dev20230504/evals/registry/completion_fns/
+-rw-r--r--   0 alvin      (502) staff       (20)      391 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      103 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      524 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.272683 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/
+-rw-r--r--   0 alvin      (502) staff       (20)      141 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      119 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      560 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      454 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      113 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      312 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.417358 evals-nightly-1.0.3.dev20230504/evals/registry/evals/
+-rw-r--r--   0 alvin      (502) staff       (20)      215 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      297 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      457 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      229 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      196 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      310 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      159 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      246 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      288 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      305 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      573 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      309 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/chess.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      308 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      250 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      160 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      335 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1719 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      151 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      167 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      175 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      202 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      377 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      306 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      269 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      387 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      195 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      314 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      254 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/finance.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      183 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      276 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      928 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      194 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      258 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      250 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      170 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      265 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      222 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      347 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      262 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      292 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      382 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      754 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      327 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      198 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      242 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/logic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      153 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      262 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      674 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      278 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      159 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      215 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      211 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1193 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      186 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      292 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      258 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      221 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      287 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      188 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      320 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      282 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/qa.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      175 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      378 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      255 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      236 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      364 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/russe.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      199 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      254 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      190 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      274 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      364 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      374 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1053 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/sql.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     4472 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      272 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      150 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      399 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1218 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      400 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1271 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      347 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     3040 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      323 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      174 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      189 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      365 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/evals/which-is-heavier.yaml
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.430998 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/
+-rw-r--r--   0 alvin      (502) staff       (20)      492 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      263 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      831 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      246 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1157 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     2564 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     1152 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 alvin      (502) staff       (20)     9600 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/registry.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.433926 evals-nightly-1.0.3.dev20230504/evals/utils/
+-rw-r--r--   0 alvin      (502) staff       (20)     1504 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/utils/api_utils.py
+-rw-r--r--   0 alvin      (502) staff       (20)      713 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/utils/misc.py
+-rw-r--r--   0 alvin      (502) staff       (20)     4076 2023-05-04 20:21:30.000000 evals-nightly-1.0.3.dev20230504/evals/utils/snowflake.py
+drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-04 20:21:55.437228 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/
+-rw-r--r--   0 alvin      (502) staff       (20)      114 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 alvin      (502) staff       (20)     5858 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin      (502) staff       (20)        1 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin      (502) staff       (20)       90 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 alvin      (502) staff       (20)      207 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 alvin      (502) staff       (20)        6 2023-05-04 20:21:55.000000 evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 alvin      (502) staff       (20)      566 2023-05-04 20:21:46.000000 evals-nightly-1.0.3.dev20230504/pyproject.toml
+-rw-r--r--   0 alvin      (502) staff       (20)       38 2023-05-04 20:21:55.438288 evals-nightly-1.0.3.dev20230504/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev1/LICENSE` & `evals-nightly-1.0.3.dev20230504/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/README.md` & `evals-nightly-1.0.3.dev20230504/README.md`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/api.py` & `evals-nightly-1.0.3.dev20230504/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/base.py` & `evals-nightly-1.0.3.dev20230504/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230504/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230504/evals/cli/oaievalset.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230504/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230504/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230504/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230504/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230504/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/data.py` & `evals-nightly-1.0.3.dev20230504/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/basic/fuzzy_match_test.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/fuzzy_match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/includes.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230504/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/eval.py` & `evals-nightly-1.0.3.dev20230504/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/formatting.py` & `evals-nightly-1.0.3.dev20230504/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/metrics.py` & `evals-nightly-1.0.3.dev20230504/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230504/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/record.py` & `evals-nightly-1.0.3.dev20230504/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry/modelgraded/sql.yaml` & `evals-nightly-1.0.3.dev20230504/evals/registry/modelgraded/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/registry.py` & `evals-nightly-1.0.3.dev20230504/evals/registry.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230504/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230504/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230504/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/evals_nightly.egg-info/SOURCES.txt` & `evals-nightly-1.0.3.dev20230504/evals_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev1/pyproject.toml` & `evals-nightly-1.0.3.dev20230504/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "evals-nightly"
-version = "1.0.3.dev1"
+version = "1.0.3.dev20230504"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
```

