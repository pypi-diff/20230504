# Comparing `tmp/loanpy-2.0.2.tar.gz` & `tmp/loanpy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loanpy-2.0.2.tar", last modified: Thu Jun  9 22:57:55 2022, max compression
+gzip compressed data, was "loanpy-3.0.0.tar", last modified: Thu May  4 19:32:41 2023, max compression
```

## Comparing `loanpy-2.0.2.tar` & `loanpy-3.0.0.tar`

### file list

```diff
@@ -1,66 +1,32 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.687636 loanpy-2.0.2/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3821 2022-06-09 22:57:55.687636 loanpy-2.0.2/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2245 2022-06-09 20:43:52.191887 loanpy-2.0.2/README.rst
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.683636 loanpy-2.0.2/loanpy/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2245 2022-06-09 20:43:52.191887 loanpy-2.0.2/loanpy/README.rst
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1023 2022-06-07 21:53:54.895886 loanpy-2.0.2/loanpy/__init__.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)    40831 2022-06-08 23:49:34.959893 loanpy-2.0.2/loanpy/adrc.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)   112693 2022-04-07 00:03:51.967904 loanpy-2.0.2/loanpy/cvfb.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1562 2022-06-07 23:30:44.815705 loanpy-2.0.2/loanpy/differences.csv
--rw-r--r--   0 viktor    (1000) viktor    (1000)    60048 2022-06-09 22:34:11.999680 loanpy-2.0.2/loanpy/helpers.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)   357103 2022-03-27 20:24:08.771990 loanpy-2.0.2/loanpy/ipa_all.csv
--rw-r--r--   0 viktor    (1000) viktor    (1000)    28060 2022-06-09 01:09:42.139743 loanpy-2.0.2/loanpy/loanfinder.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)    31143 2022-06-09 22:35:30.903678 loanpy-2.0.2/loanpy/qfysc.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      239 2022-06-04 16:00:57.179896 loanpy-2.0.2/loanpy/readme.md
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      608 2022-06-09 22:19:46.103707 loanpy-2.0.2/loanpy/requirements.txt
--rw-r--r--   0 viktor    (1000) viktor    (1000)    64450 2022-06-09 01:02:18.639757 loanpy-2.0.2/loanpy/sanity.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.683636 loanpy-2.0.2/loanpy/tests/
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.683636 loanpy-2.0.2/loanpy/tests/expected_files/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    11483 2022-06-03 21:29:12.019185 loanpy-2.0.2/loanpy/tests/expected_files/eval_all_exp.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      378 2022-06-01 00:38:14.566951 loanpy-2.0.2/loanpy/tests/expected_files/getnse4df_ad.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      426 2022-06-01 00:53:53.138921 loanpy-2.0.2/loanpy/tests/expected_files/getnse4df_rc.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    23469 2022-06-01 03:05:21.770675 loanpy-2.0.2/loanpy/tests/expected_files/mockplot.jpg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      823 2022-06-01 01:19:46.094873 loanpy-2.0.2/loanpy/tests/expected_files/postprocess_ad.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      929 2022-06-03 20:31:05.695295 loanpy-2.0.2/loanpy/tests/expected_files/postprocess_ad_workflow.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      901 2022-06-01 01:24:52.446863 loanpy-2.0.2/loanpy/tests/expected_files/postprocess_rc.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2249 2022-05-20 11:10:47.139774 loanpy-2.0.2/loanpy/tests/expected_files/test_noncrossval_sc_eval_all_integration.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     9259 2022-06-03 21:29:12.015185 loanpy-2.0.2/loanpy/tests/expected_files/workflow.csv
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.687636 loanpy-2.0.2/loanpy/tests/input_files/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       67 2022-05-10 19:12:17.779374 loanpy-2.0.2/loanpy/tests/input_files/ad_read_data.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      149 2022-05-05 21:30:41.515378 loanpy-2.0.2/loanpy/tests/input_files/forms.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     8740 2022-05-13 00:50:46.963561 loanpy-2.0.2/loanpy/tests/input_files/forms_27cogs.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1217 2022-05-07 10:47:12.187992 loanpy-2.0.2/loanpy/tests/input_files/forms_3cogs_wot.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       17 2022-05-10 01:49:21.831691 loanpy-2.0.2/loanpy/tests/input_files/got.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       17 2022-05-10 01:49:40.435691 loanpy-2.0.2/loanpy/tests/input_files/hun.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       55 2022-05-11 02:44:36.263877 loanpy-2.0.2/loanpy/tests/input_files/loans_got.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       68 2022-05-11 02:45:03.667877 loanpy-2.0.2/loanpy/tests/input_files/loans_hun.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       43 2022-05-10 21:53:16.599072 loanpy-2.0.2/loanpy/tests/input_files/loans_hun_NoPhonMatch.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       90 2022-06-07 17:39:02.039630 loanpy-2.0.2/loanpy/tests/input_files/rc_read_data.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      526 2022-05-21 21:28:24.747186 loanpy-2.0.2/loanpy/tests/input_files/sc_ad_3cogs.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      491 2022-05-10 00:29:09.375842 loanpy-2.0.2/loanpy/tests/input_files/sc_ad_handmade.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      233 2022-05-09 23:33:22.847946 loanpy-2.0.2/loanpy/tests/input_files/sc_ad_handmade2.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      155 2022-05-11 02:24:18.519916 loanpy-2.0.2/loanpy/tests/input_files/sc_ad_likeliest.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      593 2022-05-09 00:30:22.551295 loanpy-2.0.2/loanpy/tests/input_files/sc_rc_3cogs.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      162 2022-05-10 00:42:35.523817 loanpy-2.0.2/loanpy/tests/input_files/sc_rc_handmade.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      221 2022-05-10 20:19:58.619247 loanpy-2.0.2/loanpy/tests/input_files/sc_rc_likeliest.txt
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2022-06-09 22:57:55.687636 loanpy-2.0.2/loanpy/tests/output_files/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     5454 2022-06-09 00:21:22.415834 loanpy-2.0.2/loanpy/tests/output_files/eval_27cogs.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    22814 2022-06-09 00:21:22.399834 loanpy-2.0.2/loanpy/tests/output_files/eval_27cogs.jpg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    25089 2022-05-24 19:47:56.915781 loanpy-2.0.2/loanpy/tests/output_files/eval_all_plot.jpg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      755 2022-06-03 21:30:11.775184 loanpy-2.0.2/loanpy/tests/output_files/example_cache.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      205 2022-06-09 00:41:05.403797 loanpy-2.0.2/loanpy/tests/output_files/mock_cache.csv
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    23469 2022-06-09 22:49:01.651652 loanpy-2.0.2/loanpy/tests/output_files/mockplot.jpg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2249 2022-05-20 11:10:47.139774 loanpy-2.0.2/loanpy/tests/output_files/test_noncrossval_sc_eval_all_integration
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2249 2022-05-24 20:02:18.923754 loanpy-2.0.2/loanpy/tests/output_files/test_noncrossval_sc_eval_all_integration.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    29914 2022-06-09 22:35:56.687677 loanpy-2.0.2/loanpy/tests/test_adrc_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    54999 2022-06-09 22:36:05.459677 loanpy-2.0.2/loanpy/tests/test_adrc_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    28133 2022-06-09 00:04:29.755865 loanpy-2.0.2/loanpy/tests/test_helpers_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    53566 2022-06-09 22:48:35.971653 loanpy-2.0.2/loanpy/tests/test_helpers_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    14514 2022-06-09 00:07:58.555859 loanpy-2.0.2/loanpy/tests/test_loanfinder_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    39051 2022-06-09 22:36:16.519676 loanpy-2.0.2/loanpy/tests/test_loanfinder_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    10974 2022-06-09 22:36:46.731675 loanpy-2.0.2/loanpy/tests/test_qfysc_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    15937 2022-06-09 22:37:25.447674 loanpy-2.0.2/loanpy/tests/test_qfysc_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    29808 2022-06-09 22:38:03.003673 loanpy-2.0.2/loanpy/tests/test_sanity_integration.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    45259 2022-06-09 00:15:18.859845 loanpy-2.0.2/loanpy/tests/test_sanity_unit.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       91 2022-06-09 21:59:30.247745 loanpy-2.0.2/setup.cfg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1983 2022-06-09 22:57:32.551637 loanpy-2.0.2/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2023-04-16 19:03:02.000000 loanpy-3.0.0/LICENSE
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       20 2023-04-26 13:54:21.000000 loanpy-3.0.0/MANIFEST.in
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-04 19:32:41.701367 loanpy-3.0.0/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3222 2023-05-04 19:19:00.000000 loanpy-3.0.0/README.rst
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/loanpy/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-04-24 21:01:57.000000 loanpy-3.0.0/loanpy/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     8247 2023-04-27 23:30:23.000000 loanpy-3.0.0/loanpy/eval_sca.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)   435389 2023-04-25 21:27:41.000000 loanpy-3.0.0/loanpy/ipa_all.csv
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6845 2023-05-04 18:49:25.000000 loanpy-3.0.0/loanpy/loanfinder.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    37335 2023-05-03 17:44:27.000000 loanpy-3.0.0/loanpy/scapplier.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     9260 2023-04-27 23:29:00.000000 loanpy-3.0.0/loanpy/scminer.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    23190 2023-04-27 23:28:10.000000 loanpy-3.0.0/loanpy/utils.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/loanpy.egg-info/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4890 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      643 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       64 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-05-04 19:32:41.000000 loanpy-3.0.0/loanpy.egg-info/top_level.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      210 2023-05-04 19:32:41.701367 loanpy-3.0.0/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1956 2023-05-04 19:32:24.000000 loanpy-3.0.0/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-04 19:32:41.701367 loanpy-3.0.0/tests/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     5427 2023-04-25 17:53:13.000000 loanpy-3.0.0/tests/test_eval_sca_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3576 2023-04-25 23:59:23.000000 loanpy-3.0.0/tests/test_eval_sca_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      660 2023-04-23 22:13:44.000000 loanpy-3.0.0/tests/test_loanfinder_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1680 2023-04-23 22:13:26.000000 loanpy-3.0.0/tests/test_loanfinder_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    12621 2023-04-25 23:59:22.000000 loanpy-3.0.0/tests/test_scapplier_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    27616 2023-04-25 23:59:22.000000 loanpy-3.0.0/tests/test_scapplier_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1727 2023-04-16 19:03:02.000000 loanpy-3.0.0/tests/test_scminer_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6820 2023-04-25 23:59:23.000000 loanpy-3.0.0/tests/test_scminer_unit.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3482 2023-04-25 21:48:43.000000 loanpy-3.0.0/tests/test_utils_integration.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11626 2023-04-25 22:18:49.000000 loanpy-3.0.0/tests/test_utils_unit.py
```

### Comparing `loanpy-2.0.2/loanpy/adrc.py` & `loanpy-3.0.0/loanpy/scapplier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,317 +1,364 @@
-"""Adapt or reconstruct words, i.e. surf horizontally and vertically
-through the network of life"""
+# -*- coding: utf-8 -*-
+"""
+This module provides tools for predicting and analyzing changes in the
+horizontal or vertical transfer of words. It includes the
+Adrc class, which supports the adaptation and reconstruction of words based
+on sound and prosodic correspondences and inventories. The module also
+contains functions for repairing phonotactics.
+
+Horizontal transfer refers to the borrowing of words
+between languages in contact, while vertical transfer refers to the
+inheritance of words from a parent language to its descendants.
+"""
+
+import heapq
+import re
+from collections import OrderedDict
+from itertools import cycle, product
+from json import load
+from pathlib import Path
+from typing import Dict, Iterable, List, Tuple, Union
 
-from ast import literal_eval
-from collections import Counter, OrderedDict
-from itertools import count, cycle, product
-from math import prod
-from operator import itemgetter
-
-from tqdm import tqdm
-
-from loanpy.helpers import (
-    Etym,
-    apply_edit,
-    clusterise,
-    combine_ipalists,
-    editops,
-    flatten,
-    get_howmany,
-    list2regex,
-    pick_minmax,
-    tokenise)
-from loanpy.qfysc import Qfy
-
-
-def read_scdictlist(scdictlist):
-    """
-    Called by loanpy.adrc.Adrc.__init__. \
-Reads sound correspondence dictionary list generated by \
-loanpy.qfysc.Qfy.get_sound_corresp from a file.
-
-    :param scdictlist: The path to the sound correspondence dictionaries
-    :type scdictlist: pathlib.PosixPath | str | None
-
-    :returns: Only the first 4 of the 6 dicts because the last two are \
-not necessary for any computations. Returns 4 times None if \
-input is None.
-    :rtype: [None, None, None, None] | [dict, dict, dict, dict]
-
-    :Example:
-
-    >>> from loanpy.adrc import read_scdictlist, __file__
-    >>> from pathlib import Path
-    >>> read_scdictlist(None)
-    [None, None, None, None]
-    >>> path2sc = Path(__file__).parent / "tests" \
-/ "input_files" / "sc_ad_3cogs.txt"
-    >>> read_scdictlist(path2sc)
-    [{'a': ['a'], 'd': ['d'], 'j': ['j'], 'l': ['l'], 'n': ['n'], \
-'t͡ʃː': ['t͡ʃ'], 'ɣ': ['ɣ'], 'ɯ': ['i']}, {'a<a': 6, 'd<d': 1, 'i<ɯ': 1, \
-'j<j': 1, 'l<l': 1, 'n<n': 1, 't͡ʃ<t͡ʃː': 1, 'ɣ<ɣ': 2}, {'a<a': [1, 2, 3], \
-'d<d': [2], 'i<ɯ': [1], 'j<j': [3], 'l<l': [2], 'n<n': [3], 't͡ʃ<t͡ʃː': [1], \
-'ɣ<ɣ': [1, 2]}, \
-{'VCCVC': ['VCCVC'], 'VCVC': ['VCVC'], 'VCVCV': ['VCVCV']}]
-
-    """
-    if scdictlist is None:
-        return [None]*4
-    with open(scdictlist, "r", encoding="utf-8") as f:
-        return literal_eval(f.read())[:4]
-
-
-def move_sc(sclistlist, whichsound, out):
-    """
-    Called by loanpy.adrc.Adrc.read_sc. \
-    Moves sound correspondences. \
-A list of stacks where param <whichsound> indicates \
-which stack to pick. Append its second element to out and pop its first.
-
-    :param sclistlist: A word where every phoneme has been replaced with a \
-list of **all** possible sound correspondences ranked by likelihood, \
-i.e. how often \
-each sound correspondence occurred in the data. \
-(Heuristic correspondences have frequency 0.)
-    :type sclistlist: list of lists
+from loanpy.utils import prod
 
-    :param whichsound: The index of the phoneme to move from sclistlist to \
-the output
-    :type whichsound: int
+class Adrc():
+    """
+    Adapt or Reconstruct (ADRC) class.
 
-    :param out: The future output of loanpy.adrc.Adrc.adapt/reconstruct
-    :type out: list of lists
+    This class provides functionality for automatically
+    adapting or reconstructing words of a language,
+    based on sound and prosodic correspondences and inventories.
+    Inputs are generated by ``loanpy.scminer``.
+
+    :param sc: The path to the sound-correspondence json-file containing the
+               list of six dictionaries, outputted by
+               ``loanpy.scminer.get_correspondences``
+    :type sc: str or pathlike object, optional
+
+    :param prosodic_inventory: Path to the prosodic inventory json-file.
+    :type prosodic_inventory: str or pathlike object, optional
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=Zf-zKt4HHH8M&line=10&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import Adrc
+        >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+        >>> adrc.sc
+        [{'d': ['d', 't'], 'a': ['a', 'o']},
+         {'d d': 5, 'd t': 4, 'a a': 7, 'a o': 1},
+         {},
+         {'CVCV': ['CVC']}]
+        >>> adrc.prosodic_inventory
+        ['CV', 'CVV']
+    """
 
-    :returns: List with the selected stack popped, and the new out variable.
-    :rtype: tuple: (list of lists, list of lists)
+    def __init__(
+            self, sc: Union[str, Path] = "", prosodic_inventory: Union[str, Path] = ""
+            ) -> None:
+        """
+        Constructor for the ADRC class.
 
-    :Example:
+        :param sc: Path to the sound correspondence dictionary file.
+        :type sc: str, optional
 
-    >>> from loanpy.adrc import move_sc
-    >>>  # Transfer phoneme #1 of list #0 from sclistlist to out
-    >>> move_sc(sclistlist=[["x", "x"]], whichsound=0, out=[[]])
-    ([["x"]], [["x"]])
-    >>>  # Transfer phoneme #1 of list #0 from sclistlist to out
-    >>> move_sc(sclistlist=[["x", "x"], ["y", "y"], ["z"]], whichsound=0, \
-out=[["a"], ["b"], ["c"]])
-    ([["x"], ["y", "y"], ["z"]], [["a", "x"], ["b"], ["c"]])
-    >>>  # Transfer phoneme #1 of list #2 from sclistlist to out
-    >>> move_sc(sclistlist=[["", "$"], ["", "$"], ["Z", "2", "$"]], \
-whichsound=2, out=[["o"], ["r"], ["f"]])
-    [["", "$"], ["", "$"], ["2", "$"]], [["o"], ["r"], ["f", "2"]])
-    """
+        :param prosodic_inventory: Path to the CVCV and phoneme inventories file.
+        :type prosodic_inventory: str, optional
+        """
 
-    out[whichsound].append(sclistlist[whichsound][1])  # move sound #1 to out
-    sclistlist[whichsound].pop(0)  # move input by 1 (remove sound #0)
-    return sclistlist, out  # tuple
+        self.sc = None
+        self.prosodic_inventory = None
+        self.workflow = None  # will be filled by self.adapt()
+        if sc:
+            with open(sc, "r", encoding='utf-8') as f:
+                self.sc = load(f) #  sound correspondence dictionaries
+        if prosodic_inventory:
+            with open(prosodic_inventory, "r", encoding='utf-8') as f:
+                self.prosodic_inventory = load(f) # CVCV and phoneme inventories
 
+    def set_sc(self, sc: List[dict]) -> None:
+        """
+        Method to set sound correspondences manually.
+        Called by ``loanpy.eval_sca.eval_one``.
 
-class Adrc(Qfy):
-    """
-    Read etymological data and information about it generated by loanpy.\
-qfysc.py and use it to predict loanword adaptations (lateral transfers) \
-and reconstructions (vertical transfers).
-
-    The first 9 parameters are passed on to loanpy.qfysc.Qfy to inherit \
-12 attributes (of which 8 are inherited from loanpy.helpers.Etym). The last \
-parameter is passed on to __init__ to create 5 own attributes, \
-so 17 attributes \
-in total.
-
-    Define own attributes:
-
-    :param scdictlist: Path to data generated with \
-loanpy.qfysc.Qfy.get_sound_corresp. (\
-Dicts 0, 1, 2 capture phonological \
-correspondences, dicts 3, 4, 5 phonotactic ones. dict0/dict3: the actual \
-correspondences, dict1/dict4: How often each correspondence \
-occurs in the data, \
-dict2/dict5: list of cognate sets in which each correspondence occurs.
-    :type scdictlist: pathlib.PosixPath | str | None, default=None
-
-    :Exmaple:
-
-    >>> from loanpy.adrc import Adrc, __file__
-    >>> from pathlib import Path
-    >>> path2folder = Path(__file__).parent / "tests" \
-/ "input_files"
-    >>> path2sc = path2folder / "sc_ad_3cogs.txt"
-    >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-    >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", target_language="EAH", \
-mode="reconstruct", \
-most_frequent_phonotactics=2)
-    >>> adrc_obj.scdict  # sound correspondence dictionary
-    {'a': ['a'], 'd': ['d'], 'j': ['j'], 'l': ['l'], 'n': ['n'], \
-'t͡ʃː': ['t͡ʃ'], 'ɣ': ['ɣ'], 'ɯ': ['i']}
-    >>> adrc_obj.sedict  # sum of examples dictionary
-    {'a<a': 6, 'd<d': 1, 'i<ɯ': 1, 'j<j': 1, 'l<l': 1, \
-'n<n': 1, 't͡ʃ<t͡ʃː': 1, 'ɣ<ɣ': 2}
-    >>> adrc_obj.edict  # examples dictionary
-    {'a<a': [1, 2, 3], 'd<d': [2], 'i<ɯ': [1], 'j<j': [3], \
-'l<l': [2], 'n<n': [3], 't͡ʃ<t͡ʃː': [1], 'ɣ<ɣ': [1, 2]}
-    >>> adrc_obj.scdict_phonotactics  # phonotactic correspondence dictionary
-    {'VCCVC': ['VCCVC'], 'VCVC': ['VCVC'], 'VCVCV': ['VCVCV']}
-    >>> adrc_obj.workflow
-    OrderedDict()
-    >>> len(adrc_obj.__dict__)  # 5 own + 11 attributes inherited \
-from loanpy.qfysc.Qfy
-    17
-
-    """
-    def __init__(self,  # 9 args for inheritance from from loanpy.qfysc.Qfy
-                 forms_csv=None,
-                 source_language=None,
-                 target_language=None,
-                 most_frequent_phonotactics=9999999,
-                 phonotactic_inventory=None,
-                 mode=None,
-                 connector=None,
-                 scdictbase=None,
-                 vfb=None,
-                 # only this will be read here.
-                 scdictlist=None):
-        # inherit from loanpy.qfysc.Qfy
-        super().__init__(forms_csv=forms_csv,
-                         source_language=source_language,
-                         target_language=target_language,
-                         most_frequent_phonotactics=most_frequent_phonotactics,
-                         phonotactic_inventory=phonotactic_inventory,
-                         mode=mode,
-                         connector=connector,
-                         scdictbase=scdictbase,
-                         vfb=vfb)
-        # read here - was extracted by loanpy.qfysc.Qfy and written to file
-        (self.scdict, self.sedict, self.edict,
-            self.scdict_phonotactics) = read_scdictlist(scdictlist)
-        # sound correspondence dictionaries
-
-        self.workflow = OrderedDict()  # will be filled by self.adapt()
-
-    def get_diff(self, sclistlist, ipa):
-        """Called by loanpy.adrc.Adrc.read_sc. \
-Tells how much it would cost to move each \
-sound correspondence \
-by looking up the number of occurences of the current \
-and the next phoneme \
-in the sum-of-example dictionary and subtracting the \
-latter from the former. \
-(They were sorted by decreasing frequency by \
-loanpy.qfysc.Qfy.get_sound_corresp) \
-The bigger the difference the greater the cost to move it. \
-Since the higher the sum \
-of examples for each phoneme in a word, the more \
-credible its etymology.
-
-    :param sclistlist: A word where every phoneme has been replaced with a \
-list of possible sound correspondences ranked by likelihood, i.e. how often \
-each sound correspondence occurred in the data.
-    :type sclistlist: list of lists
+        :param sc: The sound correspondence dictionary.
+        :type sc: list of 6 dicts
+
+        :return: Set the attribute ``.sc``
+        :rtype: None
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=5eUpM6vcLLtH&line=2&uniqifier=1>`__
+
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.set_sc("lol")
+            >>> adrc.sc
+            'lol'
+        """
+        self.sc = sc
+
+    def set_prosodic_inventory(self, prosodic_inventory: List[str]) -> None:
+        """
+        Method to set the phonotactic inventory manually.
+        Called by ``loanpy.eval_sca.eval_one``.
+
+        :param prosodic_inventory: The phonotactic inventory.
+        :type prosodic_inventory: list of strings
+
+        :return: Set the attribute ``.prosodic_inventory``
+        :rtype: None
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=R1mPz_1lLhfb&line=2&uniqifier=1>`__
+
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.set_prosodic_inventory("rofl")
+            >>> adrc.prosodic_inventory
+            'rofl'
+        """
+        self.prosodic_inventory = prosodic_inventory
+
+    def adapt(self,
+              ipastr: Union[str, List[str]],
+              howmany: int = 1,
+              prosody: str = ""
+              ) -> str:
+        """
+        Predict the adaptation of a loanword in a target recipient language.
+
+        :param ipastr: Space-separated tokenised input IPA string.
+        :type ipastr: str
+
+        :param howmany: Number of adapted words to return. Default is 1.
+        :type howmany: int
+
+        :param prosody: Prosodic structure of the adapted words (e.g. "CVCV").
+                        Default is an empty string. Providing this triggers
+                        phonotactic repair.
+        :type prosody: str of 'C' and 'V'
+
+        :return: A list containing possible loanword adaptations.
+        :rtype: list of str
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=rHoxeCkcMQhO&line=2&uniqifier=1>`__
+
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.adapt("d a d a")
+            ['dada']
+            >>> adrc.adapt("d a d a", 5)
+            ['dada', 'data', 'doda', 'dota', 'tada']
+            >>> adrc.adapt("d a d a", 5, "CVCV")  # sc2.json says CVCV to CVC
+            ['dad', 'dat', 'dod', 'dot', 'tad']
+            >>> adrc.adapt("d a d", 5, "CVC")   # no info on CVC in sc2.json
+            ['da', 'do', 'ta', 'to']
+            # closest in inventory is "CV"
+        """
+
+        ipalist = ipastr.split(" ") if isinstance(ipastr, str) else ipastr
+        if prosody:
+            ipalist = self.repair_phonotactics(ipalist, prosody)
+        out = self.read_sc(ipalist, howmany)
+        out = ["".join(word).replace("-", "") for word in product(*out)]
+        return out[:howmany]  # cut off leftover, turn to string
+
+    def reconstruct(self,
+                    ipastr: str,
+                    howmany: int = 1,
+                    ) -> str:
+        """
+        Reconstructs a phonological form from a given IPA string using
+        a sound correspondence dictionary.
+
+        :param ipastr: A string of space-separated IPA symbols representing
+                       the phonetic form from which to predict a
+                       reconstruction.
+        :type ipastr: str
+
+        :param howmany: The maximum number of predicted reconstructions to
+                        return. Default is 1.
+        :type howmany: int
+
+        :return: A regular expression of predicted reconstructions from the
+                 given IPA string, based on the sound correspondence
+                 dictionary. Or the phoneme plus "not old" if a phoneme is
+                 missing from the correspondence-dictionaries.
+        :rtype: str
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=LfwIkQCSR5_v&line=1&uniqifier=1>`__
+
+        .. code-block:: python
 
-    :param ipa: The tokenised/clusterised input string
-    :type ipa: list
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.reconstruct("d a d a")
+            '^(d)(a)(d)(a)$'
+            >>> adrc.reconstruct("d a d a", 1000)
+            '^(d|t)(a|o)(d|t)(a|o)$'
+            >>> adrc.reconstruct("l a l a")
+            'l not old'
 
-    :returns: A list of integers where the integers indicate the cost of \
-moving the phoneme that is at the same index in the sound correspondence list.
-    :rtype: list of int
-
-    :Example:
-
-    >>> from loanpy.adrc import Adrc, __file__
-    >>> from pathlib import Path
-    >>> path2folder = Path(__file__).parent / "tests" \
-/ "input_files"
-    >>> path2sc = path2folder / "sc_ad_3cogs.txt"
-    >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-    >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", target_language="EAH")
-    >>> adrc_obj.get_diff(sclistlist=[["d", "x", "$"], ["a", "x", "$"], \
-["d", "x", "$"], ["a", "x", "$"]], ipa=["d", "a", "d", "a"])
-    [1, 6, 1, 6]
         """
+
+        ipalist = ipastr.split(" ") if isinstance(ipastr, str) else ipastr
+
+        # if phonemes missing from sound correspondence dict, return which ones
+        if not all(phon in self.sc[0] for phon in ipalist):
+            missing = [i for i in ipalist if i not in self.sc[0]]
+            return ', '.join(set(missing)) + " not old"
+
+        # read the correct number of sound correspondences per phoneme
+        out = self.read_sc(ipalist, howmany)
+
+        out = ''.join([list2regex(i) for i in out if i != ['-']])
+        return "^" + out + "$"  # regex
+
+    def repair_phonotactics(self,
+                            ipalist: List[str],
+                            prosody: str
+                            ) -> List[str]:
+        """
+        Repairs the phonotactics (prosody) of an IPA string.
+
+        :param ipalist: A list of IPA symbols representing the input word.
+        :type ipalist: list of str
+
+        :param prosody: A string representing the prosodic structure of the
+                        input word.
+        :type prosody: str
+
+        :return: A list of repaired IPA strings.
+        :rtype: list of str
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=06_G8ywk8Vo3&line=1&uniqifier=1>`__
+
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.repair_phonotactics(["d", "a", "d", "a"], "CVCV")
+            ['d', 'a', 'd']
+        """
+
+        # check if there is data available data for this structure
+        try:
+            predicted_phonotactics = self.sc[3][prosody][0]
+        except KeyError:
+            predicted_phonotactics = self.get_closest_phonotactics(prosody)
+        #print("predicted phonotactics: ", predicted_phonotactics)
+        # Get edit operations between structures, apply them 2 input IPA string
+        matrix = get_mtx(prosody, predicted_phonotactics)
+        graph = mtx2graph(matrix)
+        end = (len(matrix)-1, len(matrix[0])-1)
+        path = dijkstra(graph=graph, start=(0, 0), end=end)
+        editops = tuples2editops(path, prosody, predicted_phonotactics)
+        return apply_edit(ipalist, editops)
+
+    def get_diff(
+            self, sclistlist: List[List[str]], ipa: List[str]
+            ) -> List[int]:
+        """
+        Computes the difference in the number of examples between the current
+        and the next sound correspondences for each phoneme or cluster in a
+        word.
+
+        :param sclistlist: A list of sound correspondence lists.
+        :type sclistlist: list
+
+        :param ipa: A list of IPA symbols representing the word.
+        :type ipa: list
+
+        :return: A list of differences between the number of examples for each
+                 sound correspondence in the input word.
+        :rtype: list
+
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=6D7dEK7iQIkg&line=4&uniqifier=1>`__
+
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc()
+            >>> adrc.set_sc([{}, {"k k": 2, "k c": 1, "i e": 2, "i o": 1}, {}, {}, {}, {}, {}])
+            >>> sclistlist = [["k", "c", "$"], ["e", "o", "$"], ["k", "c", "$"], ["e", "o", "$"]]
+            >>> adrc.get_diff(sclistlist, ["k", "i", "k", "i"])
+            [1, 1, 1, 1]
+        """
+
         # difference in nr of examples between current and next sound corresp
         # for each phoneme or cluster in a word
         difflist = []  # this will be returned
         # loop through phonemes/clusters of word
         for idx, sclist in enumerate(sclistlist):
             # get nr of occurences of current sound corresp (0 if not in dict)
-            firstsc = self.sedict.get(ipa[idx] + self.connector + sclist[0], 0)
+            firstsc = self.sc[1].get(ipa[idx] + " " + sclist[0], 0)
             # check for two exceptions:
             if len(sclist) == 2:  # exception 1: if list has reached the end...
                 # ... it can never be moved again. Bc nth bigger than inf.
                 difflist.append(float("inf"))  # = stop button
                 continue  # check next phoneme
             # exception 2: no data avail. ~ nr of occurences == 0 ~ heuristics
             # don't loop through heuristics before all data available used
             if firstsc == 0:
                 difflist.append(9999999)  # = pause/freeze button...
                 continue  # ... can be unfrozen by inf (= end of list)
 
             # get nr of occurences of next sound corresp (0 if no data avail.)
-            nextsc = self.sedict.get(ipa[idx] + self.connector + sclist[1], 0)
+
+            nextsc = self.sc[1].get(ipa[idx] + " " + sclist[1], 0)
             # append diffrnc between current & next sound corresp to outputlist
             difflist.append(firstsc - nextsc)
 
         return difflist
 
-    def read_sc(self, ipa, howmany=1):
+    def read_sc(self, ipa: List[str], howmany: int = 1) -> List[List[str]]:
         """
-        Called by loanpy.adrc.Adrc.adapt and loanpy.adrc.Adrc.reconstruct. \
-Replaces every phoneme of a word with a list of phonemes \
-that it can correspond \
-to, meeting following conditions: a. The product of the length of each list \
-is just minimally above the number indicated in \
-param <howmany> (leftover will \
-be sliced away later). b. Those phonemes are chosen that diminish the sum of \
-examples of the predicted word the least. (Sum of example means \
-adding together how many times \
-each phoneme of the predicted reconstruction corresponded \
-to the aligned phoneme of the source word in the etymological data.)
+        Replaces every phoneme of a word with a list of phonemes
+        that it can correspond to. The next phoneme it picks is
+        always the one that makes the least difference in terms
+        of absolute frequency.
 
-        :param ipa: a tokenised/clusterised word
+        :param ipa: a tokenized/clusterised word
         :type ipa: list
 
-        :param howmany: How many words would this be, if combinatorics were \
-applied. This is the false positive rate if the prediction is wrong but \
-the false positive rate -1 if the prediction is right. (Say \
-1 guess is made and it is correct, then there are 0 false positives, \
-i.e. howmany-1. \
-If 1 guess is made and it's wrong then there will be 1 false positive.)
+        :param howmany: The desired number of possible combinations.
+                        This is the false positive rate if the prediction
+                        is wrong but the false positive rate -1 if the
+                        prediction is right.
         :type howmany: int, default=1
 
-        :returns: The information to which sounds each input \
-sound can correspond.
+        :return: The information about which sounds each input sound can
+                 correspond to.
         :rtype: list of lists
 
-        :Example:
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=HHP3PLv6OUhY&line=1&uniqifier=1>`__
 
-        >>> from loanpy.adrc import Adrc, __file__
-        >>> from pathlib import Path
-        >>> path2folder = Path(__file__).parent / "tests" / \
-"input_files"
-        >>> path2sc = path2folder / "sc_ad_handmade.txt"
-        >>> adrc_obj = Adrc(scdictlist=path2sc)
-        >>> adrc_obj.read_sc(ipa="dade", howmany=1)  # 1*1*1*1 = 1
-        [["d"], ["a"], ["d"], ["y"]]
-        >>> adrc_obj.read_sc(ipa="dade", howmany=4)  # 2*2*1*1 = 4
-        [["d", "tʰ"], ["a", "e"], ["d"], ["y"]]
-        >>> adrc_obj.read_sc(ipa="dade", howmany=160)  # 4*5*4*2 = 160
-        [["d", "tʰ", "t", "tː"], \
-["a", "e", "i", "o", "u"], ["d", "tʰ", "t", "tː"], ["y", "u"]]
-        >>> adrc_obj.read_sc(ipa="dade", howmany=float("inf"))  # all possible
-        [["d", "tʰ", "t", "tː"], \
-["a", "e", "i", "o", "u"], ["d", "tʰ", "t", "tː"], ["y", "u", "e"]]
+        .. code-block:: python
+
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc()
+            >>> adrc.set_sc([{"k": ["k", "h"], "i": ["e", "o"]},
+            ...              {"k k": 5, "k c": 3, "i e": 2, "i o": 1},
+            ...              {}, {}, {}, {}, {}])
+            >>> sclistlist = [["k", "c", "$"], ["e", "o", "$"], ["k", "c", "$"], ["e", "o", "$"]]
+            >>> adrc.read_sc(["k", "i"], 2)
+            [['k'], ['e', 'o']]
+            # difference between i e and i o = 2 - 1 = 1
+            # and between k k and k c = 5 - 3 = 2
+            # so picking the "o" makes less of a difference than picking the "c"
         """
 
         # pick all sound correspondences from dictionary
-        sclistlist = [self.scdict[i] for i in ipa]
+        sclistlist = [self.sc[0][i] for i in ipa]
         # if howmany is bigger/equal than their product, return all of them.
         if howmany >= prod([len(scl) for scl in sclistlist]):
             return sclistlist
         # else add a stop sign to the end of each sound corresp list
         sclistlist = [sclist+["$"] for sclist in sclistlist]
         # pick only 1st (=most likely/frequent) sound corresp for each phoneme
         out = [[i[0]] for i in sclistlist]
@@ -334,605 +381,578 @@
                 sclistlist, out = move_sc(sclistlist, next(idxpool), out)
                 # check the differences all phonemes would make
                 difflist2 = self.get_diff(sclistlist, ipa)
                 # latest if a sound hits end of list: turns 2 inf, breaks loop
 
         return out
 
-    def reconstruct(self,
-                    ipastr,
-                    howmany=1,
-                    clusterised=True,
-                    phonotactics_filter=False,
-                    vowelharmony_filter=False,
-                    sort_by_nse=False,
-                    *args):  # so sanity.eval_one can pass on more args
-        """
-        Predicts past forms of a word based on data. Should \
-theoretically also work for forward reconstructions, but not tested yet. \
-Word initial and word final sounds/clusters are \
-tagged with a "#". In addition to \
-this, every word gets a "#-" and a "-#" added to the front \
-and back of its list of tokens, \
-to capture \
-prefixes and suffixes that may have appeared or disappeared. \
-If parameters <phonotactics_filter>, <vowelharmony_filter> and <sort_by_nse> \
-are all set to False or zero, \
-the output will be a regular expression of the type "^(a|b)(c|d)(e)$". If one \
-of those parameters is set to True or non-zero, \
-combinatorics will be applied and the \
-outputted regular expression will be of the type "(^ace$|^ade$|^bce$|^bde$)".
-
-        :param ipastr: The non-tokenised input word. \
-Should consist only of \
-valid IPA-characters, as defined in ipa_all.csv's column "ipa", even though \
-the tokeniser handles invalid characters quite well. Make sure this is not \
-an empty string.
-        :type ipastr: str
-
-        :param howmany: Indicate how many guesses should be made. If all \
-predictions are wrong, this is the same as the false positive rate. \
-If the right prediction is among the guesses, it is the false positive \
-rate plus one.
-        :type howmany: int, default=1
+    def get_closest_phonotactics(self, struc: str) -> str:
+        """
+        Get the closest prosodic structure (e.g. "CVCV") from the
+        prosodic inventory of a given language based on edit distance
+        with two operations.
 
-        :param clusterised: If set to True, this will slice up the input \
-word into consonant and vowel clusters to look for them as keys in the sound \
-change dictionary.
-        :type clusterised: bool, default=True
-
-        :param phonotactics_filter: Indicate whether words \
-should be filtered out \
-from the final result if their phonotactic profile does not occur in the \
-phonotactic inventory of target language.
-        :type phonotactics_filter: bool, default=False
-
-        :param vowelharmony_filter: Indicate whether words violating the \
-constraint front-back vowel harmony (a word can contain only \
-front or only \
-back vowels) should be filtered out.
-        :type vowelharmony_filter: bool, default=False
-
-        :param sort_by_nse: Indicate whether results \
-should be sorted by their \
-normalised sum of examples (likelihood measure for etymologies). \
-Can be costly to calculate but still cheaper and more elegant than \
-replacing itertool's product function, which does this (from its \
-documentation): "The leftmost iterators are in the \
-outermost for-loop, so the \
-output tuples cycle in a manner similar to an odometer \
-(with the rightmost element changing on every iteration)"
-        :type sort_by_nse: bool, default=False
-
-        :param args: This does nothing. The purpose of this is \
-for loanpy.sanity.eval_one to be able \
-to pass on a consistent list of args to both adapt and reconstruct.
-
-        :returns: A regular expression **approximating** \
-the indicated number of predicted reconstructions, if \
-params <phonotactics_filter>, <vowelharmony_filter> and <sort_by_nse> \
-were all set to False or zero and the output thus is a regular expression \
-of the type "^(a|b)(c|d)(e)$". A regular expression **exactly** \
-the indicated number of predicted reconstructions, if one \
-of those aforementioned 3 parameters is set to True or non-zero, \
-thus combinatorics is applied and the \
-outputted regular expression is of the type "(^ace$|^ade$|^bce$|^bde$)".
+        :param struc: The phonotactic structure to compare against.
+        :type struc: str
 
+        :return: The closest prosodic structure (e.g. "CVCV") in
+                 the prosodic inventory.
         :rtype: str
 
-        :Example:
+        `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=MQ2yQCILA-d-&line=1&uniqifier=1>`__
 
-        >>> from loanpy.adrc import Adrc, __file__
-        >>> from pathlib import Path
-        >>> path2folder = Path(__file__).parent / "tests" / \
-"input_files"
-        >>> path2sc = path2folder / "sc_rc_3cogs.txt"
-        >>> adrc_obj = Adrc(scdictlist=path2sc, mode="reconstruct")
-        >>> adrc_obj.reconstruct("kriekrie")  # clusterise, missing from data
-        '#kr, ie, kr, ie# not old'
-        >>> adrc_obj.reconstruct("kriekrie", clusterised=False)  # tokenise
-        '#k, i, e, k, i, e# not old'
-        >>> adrc_obj.reconstruct("aːruː")
-        '^(a)(n)(a)(at͡ʃi)$'
-        >>> adrc_obj.reconstruct("aːruː", howmany=2)
-        '^(a)(n)(a)(at͡ʃi|ɣ)$'
-        >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-        >>> # read etymological data to get phonotactic inventory for filter
-        >>> adrc_obj = Adrc(forms_csv=path2forms, source_language="H", \
-target_language="EAH", scdictlist=path2sc, mode="reconstruct")
-        >>> adrc_obj.reconstruct("aːruː", \
-howmany=2, phonotactics_filter=True)  \
-# only CVCV in inventory
-        '^anaɣ$'
-        >>> adrc_obj.reconstruct("aːruː", howmany=1, \
-phonotactics_filter=True)  \
-# low howmany -> empty filter
-        'wrong phonotactics'
-        >>> adrc_obj.vow2fb["i"] = "B"  # let's assume "i" was a back vowel
-        >>> adrc_obj.reconstruct("aːruː", howmany=4, vowelharmony_filter=True)
-        '^anaɣ$'
-        >>> # "anaat͡ʃi" got filtered out b/c it contains \
-a front and back vowel
-        >>> # violation of constraint "vowelharmony_filter" in \
-terms of optimality theory
-        >>> adrc_obj.reconstruct("aːruː", howmany=1, \
-vowelharmony_filter=True)  \
-# low howmany -> empty filter
-        'wrong vowel harmony'
-        >>> adrc_obj.vow2fb["i"] = "F"  # make "i" a front vowel again
-        >>> adrc_obj.reconstruct("aːruː", howmany=4, \
-vowelharmony_filter=True)  \
-# nothing gets filtered
-        "^anaat͡ʃi$|^anaɣ$"
-        >>> adrc_obj.reconstruct("aːruː", howmany=4, sort_by_nse=True)
-        >>> # examples per phoneme divided by word length is higher for "anaɣ"
-        "^anaɣ$|^anaat͡ʃi$"
-        """
-
-        # slice up the input the way it's indicated in param <clusterised>
-        ipalist = clusterise(ipastr) if clusterised else tokenise(ipastr)
-
-        # apply same tagging process as in loanpy.qfysc.Qfy.align_clusterwise
-        ipalist[0], ipalist[-1] = f"#{ipalist[0]}", f"{ipalist[-1]}#"
-        ipalist = ["#-"] + ipalist + ["-#"]
+        .. code-block:: python
 
-        # if phonemes missing from sound correspondence dict, return which ones
-        if not all(phon in self.scdict for phon in ipalist):
-            return ', '.join([i for i in ipalist
-                              if i not in self.scdict]) + " not old"
+            >>> from loanpy.scapplier import Adrc
+            >>> adrc = Adrc("examples/sc2.json", "examples/inv.json")
+            >>> adrc.get_closest_phonotactics("CVC")
+            'CV'
+            >>> adrc.get_closest_phonotactics("CVCV")
+            'CVV'
+        """
 
-        # read the correct number of sound correspondences per phoneme
-        out = self.read_sc(ipalist, howmany)
+        dist_and_strucs = [
+            (edit_distance_with2ops(struc, i), i) for i in self.prosodic_inventory
+            ]
 
-        # skip combinatorics, instead return result if these 3 params are False
-        if all(i is False or i == 0 for i in
-               [phonotactics_filter, vowelharmony_filter, sort_by_nse]):
-            return f"^{''.join([list2regex(i) for i in out])}$"
-
-        # if one of the 3 params is True however, apply combinatorics
-        out = ["".join(i).replace("-", "") for i in product(*out)]
-
-        # apply first filter if indicated (wrong phontactics out)
-        if phonotactics_filter is True:
-            out = [i for i in out if self.word2phonotactics(i) in
-                   self.phonotactic_inventory]
-            if out == []:
-                return "wrong phonotactics"
-
-        # apply 2nd filter if indicated (wrong vowelharmony_filter out)
-        if vowelharmony_filter is True:
-            out = [i for i in out if self.has_harmony(i)]
-            if out == []:
-                return "wrong vowel harmony"
-
-        # sort results by decreasing likelihood (normalised sum of examples)
-        if sort_by_nse:
-            out_nse = [(i, self.get_nse(ipastr, i)) for i in out]  # get nse
-            out_max = pick_minmax(out_nse, sort_by_nse, max)
-            out = list(dict.fromkeys(out_max + out))
-
-        # can't have float in slice, but howmany=float("inf") is possible now
-        if howmany != float("inf"):
-            out = out[:howmany]
-        return f"^{'$|^'.join(out)}$"  # turn list to regular expression
+        return min(dist_and_strucs)[1]
 
-    def repair_phonotactics(self,
-                            ipastr,
-                            max_repaired_phonotactics=2,
-                            max_paths2repaired_phonotactics=1,
-                            deletion_cost=100,
-                            insertion_cost=49,
-                            show_workflow=False):
-        """
-        Called by loanpy.adrc.Adrc.adapt. \
-Repairs the phonotactic structure of a word.
-
-        :param ipastr: The input word. Will be tokenised if string.
-        :type ipastr: list | str
-
-        :param max_repaired_phonotactics: The maximum number of target \
-phonotactic structures \
-into which to turn the source structure.
-        :type max_repaired_phonotactics: int, default=2
-
-        :param max_paths2repaired_phonotactics: The maximum number of \
-different cheapest ways to \
-turn the source structure into the target structure
-        :type max_paths2repaired_phonotactics: int, default=1
-
-        :param deletion_cost: The cost of deleting a segment
-        :type deletion_cost: int | float, default=100
-
-        :param insertion_cost: The cost of inserting a segment
-        :type insertion_cost: int | float, default=49
-
-        :param show_workflow: Indicate whether 2 steps from this process \
-should be added to the dictionary assigned to loanpy.adrc.Adrc.workflow \
-(useful for debugging): the calculated \
-phonotactic profile of the input-string and the predicted repaired structures.
-        :type show_workflow: bool, default=False
 
-        :returns: a list of phonotacticly repaired words
-        :rtype: list of str
+def move_sc(
+        sclistlist: List[List[str]], whichsound: int, out: List[List[str]]
+        ) -> Tuple[List[List[str]], List[List[str]]]:
+    """
+    Moves a sound correspondence from the input list to the output
+    list and updates both lists.
 
-        :Example:
+    :param sclistlist: A list of lists containing sound correspondences.
+    :type sclistlist: list of lists
 
-        >>> from loanpy.adrc import Adrc, __file__
-        >>> from pathlib import Path
-        >>> path2folder = Path(__file__).parent / "tests" / \
-"input_files"
-        >>> path2sc = path2folder / "sc_ad_handmade.txt"
-        >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-        >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", \
-target_language="EAH")
-        >>> adrc_obj.repair_phonotactics(ipastr="kiki", \
-max_repaired_phonotactics=1)
-        [['k', 'i', 'k']]
-        >>> adrc_obj.repair_phonotactics(ipastr="kiki", \
-max_repaired_phonotactics=2)
-        [['k', 'i', 'k'], ['k', 'i', 'C', 'k', 'i']]
-        >>> adrc_obj.repair_phonotactics(ipastr="kiki", \
-max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        >>> #C can get inserted before or after k
-        [['k', 'i', 'k'], ['k', 'i', 'C', 'k', 'i'], ['k', 'i', 'k', 'C', 'i']]
-        >>> adrc_obj.scdict_phonotactics = {}  # empty sound corresp \
-data triggers heuristics
-        >>> adrc_obj.repair_phonotactics(ipastr="kiki", \
-max_repaired_phonotactics=2, \
-show_workflow=True)
-        [['V', 'k', 'i', 'k', 'i'], ['i', 'k', 'i', 'C']]
-        >>> adrc_obj.workflow
-        OrderedDict([('donor_phonotactics', ['CVCV']), \
-('predicted_phonotactics', \
-[['VCVCV', 'VCVC']])])
+    :param whichsound: The index of the sound to be moved.
+    :type whichsound: int
 
-        """
+    :param out: The output list where the sound correspondence will be
+                moved to.
+    :type out: list of lists
 
-        # tokenise if input is string
-        if isinstance(ipastr, str):
-            ipastr = tokenise(ipastr)
-        # get phonotactic profile of input string
-        if max_repaired_phonotactics == 0:
-            return [ipastr]
-        donorstruc = self.word2phonotactics(ipastr)
-        # append to workflow if indicated, to check if this went correctly
-        if show_workflow:
-            self.workflow["donor_phonotactics"] = str(donorstruc)
-        # check if there is data available for this structure
-        try:
-            predicted_phonotactics = self.scdict_phonotactics[
-                donorstruc][:max_repaired_phonotactics]
-        # if not use heuristics: pick n most similar strucs from inventory
-        except KeyError:
-            predicted_phonotactics = self.rank_closest_phonotactics(
-                donorstruc, max_repaired_phonotactics).split(", ")
-        # append this step to workflow for debugging, if indicated
-        if show_workflow:
-            self.workflow[
-                "predicted_phonotactics"] = str(predicted_phonotactics)
-        # get edit operations between strucs and apply them to input IPA-string
-        return flatten([[apply_edit(ipastr, edop) for edop in
-                         editops(
-                                 donorstruc,
-                                 pred,
-                                 max_paths2repaired_phonotactics,
-                                 deletion_cost,
-                                 insertion_cost)]
-                        for pred in predicted_phonotactics])
+    :return: An updated tuple containing the modified sclistlist and out.
+    :rtype: tuple of (list of lists, list of lists)
 
-    def adapt(self,
-              ipastr,
-              howmany=1,
-              cluster_filter=False,
-              phonotactics_filter=False,
-              repair_vowelharmony=False,
-              sort_by_nse=False,
-              max_repaired_phonotactics=0,
-              max_paths2repaired_phonotactics=1,
-              deletion_cost=100,
-              insertion_cost=49,
-              show_workflow=False):
-        """
-        Takes a word as input and uses available data \
-together with heuristics to make predictions about its transformation \
-when entering a target language as a loan.
-
-        :param ipastr: The non-tokenised input word. Should consist only of \
-valid IPA-characters, as defined in ipa_all.csv's column "ipa", even though \
-the tokeniser handles invalid characters quite well. Make sure this is not \
-an empty string.
-        :type ipastr: str
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=uRPvWbJLSDTj&line=1&uniqifier=1>`__
 
-        :param howmany: Indicate how many guesses should be made. If all \
-predictions are wrong, this is the same as the false positive rate. \
-If the right prediction is among the guesses, it is the false positive \
-rate plus one.
-        :type howmany: int, default=1
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import move_sc
+        >>> move_sc([["x", "x"]], 0, [[]])
+        ([['x']], [['x']])
+        >>> move_sc([["x", "x"], ["y", "y"], ["z"]], 1, [["a"], ["b"], ["c"]])
+        ([['x', 'x'], ['y'], ['z']], [['a'], ['b', 'y'], ['c']])
+    """
 
-        :param cluster_filter: Throws out all words that \
-contain vowel or consonant clusters that are not documented in the target \
-language.
-        :type cluster_filter: bool, default=False
-
-        :param phonotactics_filter: Indicate whether words \
-should be filtered out \
-from the final result if their phonotactic profile does not occur in the \
-phonotactic inventory of target language.
-        :type phonotactics_filter: bool, default=False
-
-        :param repair_vowelharmony: Indicate whether violations of \
-constraint "front-back vowel harmony" should be repaired.
-        :type repair_vowelharmony: bool, default=False
-
-        :param sort_by_nse: Indicate whether results should \
-be sorted by their \
-likelihood. Can be costly to calculate. If bool is passed, all or no \
-words will be sorted. If int is passed, only that many words will be sorted \
-in the beginning of the list, the rest remains unsorted.
-        :type sort_by_nse: bool, int, default=False
-
-        :param max_repaired_phonotactics: Indicate how many of \
-the most similar \
-available profiles \
-from the phonotactic inventory should be taken into consideration.
-        :type max_repaired_phonotactics: int, default=0
-
-        :param max_paths2repaired_phonotactics: Indicate in maximum how many \
-different ways \
-each phonotactic profile should be repaired towards the same target. E.g. if \
-source is "CCV" and target "CV", the first or the second "C" can be \
-deleted.
-        :type max_paths2repaired_phonotactics: int, default=1
-
-        :param deletion_cost: The cost of deleting a phoneme
-        :type deletion_cost: int | float, default=100
-
-        :param insertion_cost: The cost of inserting a phoneme
-        :type insertion_cost: int | float, default=49
-
-        :param show_workflow: Indicate if the workflow should be \
-documented. Useful for debugging and makes it less black-boxy. \
-The single steps are added as keys to the dictionary assigned to \
-loanpy.adrc.Adrc.workflow. The \
-number of keys varies between 2-5, depending on the arguments \
-passed on to this function. \
-Keys "tokenised" and "adapted_phonotactics" are always there. \
-Keys "donor_phonotactics" \
-and "predicted_phonotactics" are only added if param \
-<max_repaired_phonotactics> was \
-set to greater than 0. Key "adapted_vowelharmony" is only added if \
-param <repair_vowelharmony> was set to True.
-        :type show_workflow: bool, default=False
+    out[whichsound].append(sclistlist[whichsound][1])  # move sound #1 to out
+    sclistlist[whichsound].pop(0)  # move input by 1 (remove sound #0)
+    return sclistlist, out  # tuple
 
-        :returns: As many predictions as indicated in param \
- <howmany>, separated by ", "
-        :rtype: str
+def edit_distance_with2ops(
+        string1: str,
+        string2: str,
+        w_del: Union[int, float] = 100,
+        w_ins: Union[int, float] = 49
+        ) -> Union[int, float]:
+    """
+    Called by ``loanpy.scapplier.Adrc.get_closest_phonotactics``.
+    Takes two strings and calculates their similarity by
+    only allowing two operations: insertion and deletion.
+    An algorithmic implementation of the "Threshold Principle"
+    `(Paradis and LaCharité 1997: 385) <http://www.jstor.com/stable/4176422>`_
+
+    :param string1: The first of two strings to be compared to each other
+    :type string1: str
+
+    :param string2: The second of two strings to be compared to each other
+    :type string2: str
+
+    :param w_del: weight (cost) for deleting a phoneme. Default should
+                  always stay 100, since only relative costs between inserting
+                  and deleting count.
+    :type w_del: int or float, default=100
+
+    :param w_ins: weight (cost) for inserting a phoneme. Default 49
+                  is in accordance with the "Threshold Principle":
+                  2 insertions (2*49=98) are cheaper than a deletion (100).
+    :type w_ins: int or float, default=49.
+
+    :returns: The distance between two input strings
+    :rtype: int or float
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=vTJ6TnehBOGv&line=2&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import edit_distance_with2ops
+        >>> edit_distance_with2ops("rajka", "ajka", w_del=100, w_ins=49)
+        100
+        >>> edit_distance_with2ops("ajka", "rajka", w_del=100, w_ins=49)
+        49
+        >>> edit_distance_with2ops("Bécs", "Pécs", w_del=100, w_ins=49)
+        149
+        >>> edit_distance_with2ops("Hegyeshalom", "Mosonmagyaróvár", w_del=100, w_ins=49)
+        1388
+
+    """
+
+    m = len(string1)     # Find longest common subsequence (LCS)
+    n = len(string2)
+    L = [[0 for x in range(n + 1)]
+         for y in range(m + 1)]
+    for i in range(m + 1):
+        for j in range(n + 1):
+            if (i == 0 or j == 0):
+                L[i][j] = 0
+            elif (string1[i - 1] == string2[j - 1]):
+                L[i][j] = L[i - 1][j - 1] + 1
+            else:
+                L[i][j] = max(L[i - 1][j],
+                              L[i][j - 1])
+
+    lcs = L[m][n]
+    # Edit distance is delete operations + insert operations*0.49.
+    # costs (=distance) are lower for insertions
+    return (m - lcs) * w_del + (n - lcs) * w_ins
+
+def apply_edit(word: Iterable[str], editops: List[str]) -> List[str]:
+    """
+    Called by ``loanpy.scapplier.Adrc.repair_phonotactics``.
+    Applies a list of human readable edit operations to a string.
+
+    :param word: The input word
+    :type word: an iterable (e.g. list of phonemes, or string)
+
+    :param editops: list of (human readable) edit operations
+    :type editops: list or tuple of strings
+
+    :returns: transformed input word
+    :rtype: list of str
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=-xzLp00EKoaw&line=10&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import apply_edit
+        >>> apply_edit(
+        ...       ['f', 'ɛ', 'r', 'i', 'h', 'ɛ', 'ɟ'],
+        ...       ('insert d',
+        ...        'insert u',
+        ...        'insert n',
+        ...        'insert ɒ',
+        ...        'insert p',
+        ...        'substitute f by ɒ',
+        ...        'delete ɛ',
+        ...        'keep r',
+        ...        'delete i',
+        ...        'delete h',
+        ...        'delete ɛ',
+        ...        'substitute ɟ by t')
+        ... )
+        ['d', 'u', 'n', 'ɒ', 'p', 'ɒ', 'r', 't']
+    """
+
+    out, letter = [], iter(word)
+    for i, op in enumerate(editops):
+        if i != len(editops):  # to avoid stopiteration
+            if "keep" in op:
+                out.append(next(letter))
+            elif "delete" in op:
+                next(letter)
+        if "substitute" in op:
+            out.append(op[op.index(" by ") + 4:])
+            if i != len(editops) - 1:
+                next(letter)
+        elif "insert" in op:
+            out.append(op[len("insert "):])
+    return out
+
+def list2regex(sclist: List[str]) -> str:
+    """
+    Called by ``loanpy.scapplier.Adrc.reconstruct``.
+    Turns a list of phonemes into a regular expression.
+
+    :param sclist: a list of phonemes
+    :type sclist: list of str
+
+    :returns: The phonemes from the input list separated by a pipe. "-" is
+              removed and replaced with a question mark at the end.
+    :rtype: str
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=_wHBHRPq96_t&line=3&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import list2regex
+        >>> list2regex(["b", "k", "-", "v"])
+        '(b|k|v)?'
+    """
+
+    s = ")?" if "-" in sclist else ")"
+    out = "|".join([i.replace(".", "") for i in sclist if i != "-"])
+    return "(" + out + s
+
+def tuples2editops(
+        op_list: List[Tuple[int, int]], s1: str, s2: str
+        ) -> List[str]:
+    """
+    Called by ``loanpy.scapplier.editops``.
+    The path through the graph by which ``string1`` is converted to
+    ``string2`` is given in form of tuples that contain the x and y
+    coordinates of every step through the matrix shaped graph.
+    This function converts those numerical instructions to human readable
+    ones. The x values stand for movement from left to right, y values for
+    movement downwards.
+    Movement downwards means deletion, movement to the right means insertion.
+    Diagonal movement means the value is kept.
+    Moving to the right and downards or downwards and to the right after each
+    other means substitution.
+
+    :param op_list: The numeric list of edit operations
+    :type op_list: list of tuples of 2 int
+
+    :param s1: The first of two strings to be compared to each other
+    :type s1: str
+
+    :param s2: The second of two strings to be compared to each other
+    :type s2: str
+
+    :returns: list of human readable edit operations
+    :rtype: list of strings
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=LtpRErY0JAeR&line=5&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import tuples2editops
+        >>> tuples2editops([(0, 0), (0, 1), (1, 1), (2, 2)], "ló", "hó")
+        ['substitute l by h', 'insert ó']
+        >>> tuples2editops([(0, 0), (1, 1), (2, 2), (2, 3)], "lóh", "ló")
+        ['keep l', 'keep ó', 'delete h']
+
+    """
+
+    s1, s2 = "#" + s1, "#" + s2
+    out = []
+    for i in range(1, len(op_list)):
+        # where does the arrow point?
+        direction = [op_list[i][0] - op_list[i - 1][0],
+                     op_list[i][1] - op_list[i - 1][1]]
+        if direction == [1, 1]:  # if diagonal
+            out.append(f"keep {s1[op_list[i][1]]}")
+        elif direction == [0, 1]:  # if horizontal
+            out.append(f"delete {s1[op_list[i][1]]}")
+        elif direction == [1, 0]:  # if vertical
+            out.append(f"insert {s2[op_list[i][0]]}")
+
+    return substitute_operations(out)
+
+def substitute_operations(operations: List[str]) -> List[str]:
+    """
+    Replaces subsequent "delete, insert" / "insert, delete" operations with
+    "substitute". Called by ``loanpy.apply.tuples2editops``.
+
+    :param operations: A list of human readable edit operations
+    :type operations: List of strings, e.g. ['insert l', 'delete h', 'keep ó']
+
+    :returns: Updated operations
+    :rtype: List of strings, e.g. ['substitute l by h', 'keep ó']
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=8wTRsBg9K4JQ&line=7&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import substitute_operations
+        >>> substitute_operations(['insert A', 'delete B', 'insert C'])
+        ['substitute B by A', 'insert C']
+        >>> substitute_operations(['delete A', 'insert B', 'delete C', 'insert D'])
+        ['substitute A by B', 'substitute C by D']
+
+    """
+
+    i = 0
+    while i < len(operations) - 1:
+        if (operations[i].startswith('delete ') and
+                operations[i+1].startswith('insert ')):
+            x = operations[i][7:]
+            y = operations[i+1][7:]
+            operations[i:i+2] = [f'substitute {x} by {y}']
+        elif (operations[i].startswith('insert ') and
+                operations[i+1].startswith('delete ')):
+            x = operations[i][7:]
+            y = operations[i+1][7:]
+            operations[i:i+2] = [f'substitute {y} by {x}']
+        else:
+            i += 1
+    return operations
+
+def get_mtx(target: Iterable, source: Iterable) -> List[List[int]]:
+    """
+    Called by ``loanpy.scapplier.Adrc.repair_phonotactics``. Similar to
+    ``loanpy.scapplier.edit_distance_with2ops`` but without
+    weights (i.e. deletion and insertion both always cost one) and the matrix
+    is returned. Draws a matrix of minimum edit distances between every
+    substring of two input strings.
+
+    :param target: The target word
+    :type target: iterable, e.g. str or list
+
+    :param source: The source word
+    :type source: iterable, e.g. str or list
+
+    :returns: A matrix where every cell tells the cost of turning one
+              substring into the other (only delete and insert with cost 1 for
+              each)
+    :rtype: list of lists
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=rGHqIDXcDoab&line=3&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import get_mtx
+        >>> get_mtx("Bécs", "Pécs")
+        [[0, 1, 2, 3, 4],
+         [1, 2, 3, 4, 5],
+         [2, 3, 2, 3, 4],
+         [3, 4, 3, 2, 3],
+         [4, 5, 4, 3, 2]]
+        # What happens under the hood:
+        # deletion costs 1, insertion costs 1, so the distances are:
+        # B C D E  # hashtag stands for empty string
+        # 0 1 2 3 4  # distance B-#=1, BC-#=2, BCD-#=3, BCDE-#=4
+        # D 1 2 3 2 3  # distance D-#=1, D-B=2, D-BC=3, D-BCD=2, D-BCDE=3
+        # E 2 3 4 3 2  # distance DE-#=2, DE-B=3, DE-BC=4, DE-BCD=3, DE-BCDE=2
+        # the min. edit distance from BCDE-DE=2: delete B, delete C
+
+    .. seealso::
+        `YouTube tutorial by Rylan Fowers
+        <https://www.youtube.com/watch?v=AY2DZ4a9gyk>`_
+    """
+
+    # build matrix of correct size
+    target = ['#'] + [k for k in target]  # add hashtag as starting value
+    source = ['#'] + [k for k in source]  # starting value is always zero
+
+    # matrix consists of zeros at first. sol stands for solution.
+    sol = [[0 for _ in range(len(target))] for _ in range(len(source))]
+
+    # first row of matrix is 1,2,3,4,5,... as long as the target word is
+    sol[0] = [j for j in range(len(target))]
+
+    # first column is also 1,2,3,4,5....  as long as the source word is
+    for j in range(len(source)):
+        sol[j][0] = j
+
+    # Add anchor value
+    if target[1] != source[1]:  # if first letters of the 2 words r different
+        sol[1][1] = 2  # set the first value (upper left corner) to 2
+    # else it just stays zero
+
+    # loop through the indexes of the two words with a nested loop
+    for c in range(1, len(target)):
+        for r in range(1, len(source)):
+            if target[c] != source[r]:  # when the two letters are different
+                # pick minimum of the 2 boxes to the left and above and add 1
+                sol[r][c] = min(sol[r - 1][c], sol[r][c - 1]) + 1
+            else:  # but if the letters are different
+                # pick the letter diagonally up left
+                sol[r][c] = sol[r - 1][c - 1]
+
+    # returns the entire matrix. min edit distance in bottom right corner jff.
+    return sol
+
+def add_edge(
+        graph: Dict[Tuple[int, int], List[Tuple[int, int, int]]],
+        u: Tuple[int, int],
+        v: Tuple[int, int],
+        weight: int
+        ) -> None:
+    """
+    Add an edge to a graph. Called by ``loanpy.scapplier.mtx2graph``.
+
+    :param graph: The graph to be populated
+    :type graph: dict
+
+    :param u: Position of the starting node
+    :type u: Tuple of two integers, e.g. (0, 0)
+
+    :param v: Position of the ending node
+    :type v: Tuple of two integers, e.g. (0, 1)
+
+    :param weight: The weigt of the edge connecting the two nodes
+    :type weight: int
+
+    :return: Updates the graph in-place
+    :rtype: None
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=2MmHpBB9U2FM&line=3&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import add_edge
+        >>> graph = {'A': {'B': 3}}
+        >>> add_edge(graph, 'A', 'C', 7)
+        >>> graph
+        {'A': {'B': 3, 'C': 7}}
+
+    """
+
+    if u not in graph:
+        graph[u] = {}
+    graph[u][v] = weight
+
+def mtx2graph(
+        matrix: List[List[int]],
+        w_del: int = 100,
+        w_ins: int = 49
+        ) -> Dict[Tuple[int, int], Dict[Tuple[int, int], int]]:
+    """
+    Converts a distance-matrix to a weighted directed graph
+
+    :param matrix: The distance matrix, generated by ``loanpy.apply.get_mtx``.
+    :type matrix: A list of list of integers
+
+    :w_del: Weight of deletions. According to the Threshold Principle of the
+            Theory of Constraints and Repair Strategies (TCRS,
+            `Paradis and LaCharité 1997: 385
+            <http://www.jstor.com/stable/4176422>`__),
+            two insertions are cheaper than one deletion. Therefore,
+            the weight of deletions, i.e. moving to the right through the
+            matrix, is set to 49 by default.
+    :w_ins: Weight of insertions, i.e. moving downwards through the matrix.
+            Set to 100 by default, so that two insertions
+            (2*49=98) are just cheaper than one deletion.
+
+    :returns: A directed graph with weighted edges
+    :rtype: dictionary with tuples as keys and dictionaries as values.
+            The value-dictionaries contain tuples as keys and weights
+            (integers) as values.
+            All tuples contain two integers that represent the position
+            of a node in the matrix/graph, e.g. (0, 0).
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=HbEz8rWFEzGi&line=3&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import mtx2graph
+        >>> mtx2graph([[0, 1, 2], [1, 2, 3], [2, 3, 2]])
+        {(0, 0): {(0, 1): 100, (1, 0): 49},
+         (0, 1): {(0, 2): 100, (1, 1): 49},
+         (0, 2): {(1, 2): 49},
+         (1, 0): {(1, 1): 100, (2, 0): 49},
+         (1, 1): {(1, 2): 100, (2, 1): 49, (2, 2): 0},
+         (1, 2): {(2, 2): 49},
+         (2, 0): {(2, 1): 100},
+         (2, 1): {(2, 2): 100},
+         (2, 2): {}}
+
+    """
+
+    graph = {}
+    rows, cols = len(matrix), len(matrix[0])
+
+    for i in range(rows):
+        for j in range(cols):
+            current_node = (i, j)
+            graph[current_node] = {}
+
+            if j < cols - 1:  # Right neighbor
+                weight = w_del if matrix[i][j + 1] != matrix[i][j] else 0
+                graph[current_node][(i, j + 1)] = weight
+
+            if i < rows - 1:  # Down neighbor
+                weight = w_ins if matrix[i + 1][j] != matrix[i][j] else 0
+                graph[current_node][(i + 1, j)] = weight
+
+            if i < rows - 1 and j < cols - 1:  # Diagonal down-right neighbor
+                weight = 0 if matrix[i + 1][j + 1] == matrix[i][j] else None
+                if weight is not None:
+                    graph[current_node][(i + 1, j + 1)] = weight
+
+    return graph
+
+def dijkstra(
+        graph: Dict[Tuple[int, int], Dict[Tuple[int, int], int]],
+        start: Tuple[int, int],
+        end: Tuple[int, int]
+        ) -> Union[List[Tuple[int, int]], None]:
+    """
+    Find the shortest path between two nodes in a weighted graph
+    using Dijkstra's algorithm.
+
+    Dijkstra's algorithm is an algorithm for finding the shortest path
+    between two nodes in a weighted graph. It
+    maintains a priority queue of nodes to be expanded and their tentative
+    distances from the start node. The
+    algorithm iteratively extracts the node with the minimum tentative
+    distance from the priority queue and updates
+    the tentative distances of its neighbors if a shorter path is found.
+
+    :param graph: A dictionary representing the weighted graph, where each
+                  key is a node and each value is a
+                  dictionary representing its neighbors and edge weights.
+    :type graph: dict
+    :param start: The starting node.
+    :type start: A tuple of two integers representing the node's position on
+                 the x and y axis.
+    :param end: The ending node.
+    :type end: A tuple of two integers representing the node's position on
+                 the x and y axis.
+    :return: The shortest path between the start and end nodes,
+             represented as a list of nodes in the order they are
+             visited, or None if no path exists.
+    :rtype: list or None
+    :raises KeyError: If the start or end node is not in the graph.
+
+    `Run in Google Colab >> <https://colab.research.google.com/drive/1JlHKfdff_yjCO8yvxiKV9xoRAiEPgarM#scrollTo=WRYiNDPmHr5V&line=5&uniqifier=1>`__
+
+    .. code-block:: python
+
+        >>> from loanpy.scapplier import dijkstra
+        >>> graph1 = {
+        ...         'A': {'B': 1, 'C': 4},
+        ...         'B': {'C': 2, 'D': 6},
+        ...         'C': {'D': 3},
+        ...         'D': {}
+        ...     }
+        >>> dijkstra(graph1, 'A', 'D')
+        ['A', 'B', 'C', 'D']
+
+    .. seealso::
+        `Dijkstra's algorithm on Wikipedia
+        <https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm>`_
+    """
 
-        :Example:
+    dist = {node: float('inf') for node in graph}
+    dist[start] = 0
+    queue = [(0, start)]
+    path = {}
+
+    while queue:
+        current_dist, current_node = heapq.heappop(queue)
+
+        if current_dist > dist[current_node]:
+            continue
+
+        for neighbor, weight in graph[current_node].items():
+            new_dist = current_dist + weight
+
+            if new_dist < dist[neighbor]:
+                dist[neighbor] = new_dist
+                path[neighbor] = current_node
+                heapq.heappush(queue, (new_dist, neighbor))
+
+    if end not in path:
+        return None
+
+    # Reconstruct the shortest path
+    shortest_path = [end]
+    while shortest_path[-1] != start:
+        shortest_path.append(path[shortest_path[-1]])
+    shortest_path.reverse()
 
-        >>> from loanpy.adrc import Adrc, __file__
-        >>> from pathlib import Path
-        >>> path2folder = Path(__file__).parent / "tests" / \
-"input_files"
-        >>> path2sc = path2folder / "sc_ad_handmade.txt"
-        >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-        >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", \
-target_language="EAH")
-        >>> adrc_obj.adapt(ipastr="dade", howmany=5)
-        "dady, datʰy, dedy, detʰy, tʰady"
-        >>> # repair phonotactics with data hard-coded in "sc_ad_handmade.txt"
-        >>> # Usually this is the same as data extracted from forms.csv
-        >>> # But now due to illustrative purposes they are different.
-        >>> adrc_obj.adapt(ipastr="dade", howmany=6, \
-max_repaired_phonotactics=2)
-        "dad, ded, tʰad, tʰed, dajdy, dejdy"
-        >>> # max_paths2repaired_phonotactics=2 causes j to be \
-inserted before AND after d
-        >>> adrc_obj.adapt(ipastr="dade", howmany=6, \
-max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        "dad, tʰad, dajdy, tʰajdy, dadjy, tʰadjy"
-        >>> adrc_obj.vow2fb["e"] = "B"  # let's assume "e" was a backvowel.
-        >>> # repair repair_vowelharmony before substituting: dade->dadF
-        >>> adrc_obj.adapt(repair_vowelharmony=True, ipastr="dade", \
-howmany=6, \
-max_repaired_phonotactics=2, max_paths2repaired_phonotactics=2)
-        "dad, tʰad, dajdæ, tʰajdæ, dujdy, tʰujdy"
-        >>> # phonotactic inventory for phonotactics_filter is calculated \
-from forms.csv!
-        >>> # contains only structures of the 3 words occurring in \
-the target lg EAH
-        >>> adrc_obj.phonotactic_inventory  # this will filter out all results
-        {'VCVC', 'VCVCV', 'VCCVC'}
-        >>> adrc_obj.adapt(phonotactics_filter=True, \
-repair_vowelharmony=True, \
-ipastr="dade", howmany=6, max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        'wrong phonotactics'
-        >>> adrc_obj.phonotactic_inventory.add('CVCCV')  \
-# so let's assume CVCCV \
-was in the inventory
-        >>> adrc_obj.adapt(phonotactics_filter=True, \
-repair_vowelharmony=True, \
-ipastr="dade", howmany=6, max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        "dajdæ, tʰajdæ, dujdy, tʰujdy, dadjæ, tʰadjæ"
-        >>> # now let's filter out all clusters undocumented in forms.csv
-        >>> adrc_obj.cluster_inventory  # only these clusters are allowed
-        {'ld', 't͡ʃ', 'j', 'ɣ', 'a', 'n', 'ia'}
-        >>> adrc_obj.adapt(cluster_filter=True, phonotactics_filter=True, \
-repair_vowelharmony=True, ipastr="dade", howmany=6, \
-max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        "wrong clusters"
-        >>>  # let's use a different sound correspondence file
-        >>> path2sc = path2folder / "sc_ad_handmade2.txt"
-        >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", \
-target_language="EAH")
-        >>> adrc_obj.phonotactic_inventory.add('CVCCV')
-        >>> # let's ramp up the combinatorics
-        >>> adrc_obj.adapt(howmany=1000, cluster_filter=True, \
-phonotactics_filter=True, \
-repair_vowelharmony=True, ipastr="dade", max_repaired_phonotactics=2, \
-max_paths2repaired_phonotactics=2)
-        't͡ʃalda'
-        >>> adrc_obj.cluster_inventory.add("d")  \
-# let's assume d was an allowed cluster
-        >>> adrc_obj.adapt(howmany=1000, cluster_filter=True, \
-phonotactics_filter=True, repair_vowelharmony=True, ipastr="dade", \
-max_repaired_phonotactics=2, max_paths2repaired_phonotactics=2)
-        'dalda, t͡ʃalda'
-        >>> # now sort results by likelihood (nse) and document workflow
-        >>> adrc_obj.adapt(sort_by_nse=True, show_workflow=True, \
-howmany=1000, cluster_filter=True, \
-phonotactics_filter=True, repair_vowelharmony=True, ipastr="dade", \
-max_repaired_phonotactics=2, max_paths2repaired_phonotactics=2)
-        't͡ʃalda, dalda'
-        >>> adrc_obj.workflow
-        OrderedDict([('tokenised', \
-[['d', 'a', 'd', 'e']]), ('donor_phonotactics', ['CVCV']), \
-('predicted_phonotactics', \
-[['CVC', 'CVCCV']]), ('adapted_phonotactics', [[['d', 'a', 'd'], \
-['d', 'a', 'C', 'd', 'e'], ['d', 'a', 'd', 'C', 'e']]]), \
-('adapted_vowelharmony', \
-[[['d', 'a', 'd'], ['d', 'a', 'C', 'd', 'e'], \
-  ['d', 'a', 'd', 'C', 'e']]]), \
-('before_combinatorics', \
-[[[['d', 't͡ʃ'], ['a', 'e'], ['d', 't͡ʃ']], \
-[['d', 't͡ʃ'], ['a', 'e'], ['l'], ['d', 't͡ʃ'], ['e', 'a']], \
-  [['d', 't͡ʃ'], ['a', 'e'], ['d', 't͡ʃ'], ['l'], ['e', 'a']]]])])
-
-        """
-        # distribute howmany so that the product of these three approximates it
-        (max_phon, max_repaired_phonotactics,
-         max_paths2repaired_phonotactics
-         ) = get_howmany(howmany, max_repaired_phonotactics,
-                         max_paths2repaired_phonotactics)
-        # reset workflow variable, tokenise input (must be untokenised ipa str)
-        self.workflow, out = OrderedDict(), tokenise(ipastr)
-        # document the tokenisation if indicated
-        if show_workflow:
-            self.workflow["tokenised"] = str(out)
-
-        # repair the phonotactic structure if indicated
-        out = self.repair_phonotactics(
-                                      out,
-                                      max_repaired_phonotactics,
-                                      max_paths2repaired_phonotactics,
-                                      deletion_cost,
-                                      insertion_cost,
-                                      show_workflow)
-        # document how structure was repaired if indicated
-        if show_workflow:
-            self.workflow["adapted_phonotactics"] = str(out)
-
-        if repair_vowelharmony:  # repair vowel harmony if indicated
-            out = flatten(map(self.repair_harmony, out))
-            # document how repair_vowelharmony was repaired if indicated
-            if show_workflow:
-                self.workflow["adapted_vowelharmony"] = str(out)
-
-        # read possible sound correspondences for each phoneme
-        out = [self.read_sc(ipalist, max_phon) for ipalist in out]
-
-        # document which sound corresp were read, if indicated
-        if show_workflow:
-            self.workflow["before_combinatorics"] = str(out)
-
-        # combine the sound correspondences to create a list of words (str)
-        out = combine_ipalists(out)
-
-        # phonotactics repaired, still: 1 phoneme can correspond to +-1 phoneme
-        # structure not in target lg's phonotactic inventory
-        if phonotactics_filter:
-            out = [i for i in out if self.word2phonotactics(i)
-                   in self.phonotactic_inventory]
-            #  indicate empty filter and return if necessary
-            if out == []:
-                return "wrong phonotactics"
-
-        # filter clusters not in target lg's cluster inventory
-        if cluster_filter:
-            out = [wrd for wrd in out
-                   if all(cl in self.cluster_inventory for cl
-                          in clusterise(wrd))]
-            # indicate empty filter and return if necessary
-            if out == []:
-                return "wrong clusters"
-
-        if sort_by_nse:  # sort resutls by likelyhood (nse) if indicated
-            out_nse = [(i, self.get_nse(ipastr, i)) for i in out]  # get nse
-            out = pick_minmax(out_nse, sort_by_nse, max, True)
-
-        return ", ".join(out[:howmany])  # cut off leftover, turn to string
-
-    def get_nse(self, left, right):
-        """
-        Called by loanpy.adrc.Adrc.adapt, loanpy.adrc.Adrc.reconstruct, \
-loanpy.loanfinder.Search, loanpy.loanfinder.likeliestphonmatch. \
-Aligns two words (alignment type depends \
-on the mode defined when initiating \
-loanpy.adrc.Adrc), check in the sound correspondence \
-dictionary how often each aligned sound correspondence \
-occurred (0 if not in dict), sum up their number, and \
-divide it by the number of phoneme (clusters) in the word.
-
-        :param left: The string on the left side of the etymology to align.
-        :type left: str
-
-        :param right: The string on the right side of the etymology to align.
-        :type right: str
-
-        :returns: A tuple of four elements: First is the sum of examples \
-        divided by the number of phoneme \
-        (clusters) in the word, second is the sum \
-        of examples, i.e. how many other words in the etymological data go \
-        through the same sound substitution/ sound change as this word. \
-        Third is the distribution of sound correspondences, i.e. how many \
-        examples in other words are found for each phoneme in the data. \
-        Fourth is how the source and target word were aligned. Elements \
-        three and four need to be strings, since if they were lists, it would \
-        be difficult to build a data frame from them in sanity.py.
-        :rtype: (float, int, str, str)
-
-        :Example:
-
-        >>> from loanpy.adrc import Adrc, __file__
-        >>> from pathlib import Path
-        >>> path2folder = Path(__file__).parent / "tests" / \
-"input_files"
-        >>> path2sc = path2folder / "sc_ad_handmade.txt"
-        >>> path2forms = path2folder / "forms_3cogs_wot.csv"
-        >>> adrc_obj = Adrc(\
-scdictlist=path2sc, \
-forms_csv=path2forms, \
-source_language="WOT", \
-target_language="EAH")
-        >>> adrc_obj.get_nse("dade", "dady")
-        (33.25, 133, '[1, 6, 1, 125]', "['d<d', 'a<a', 'd<d', 'e<y']")
-        """
-        # self.align can't handle empty strings as input!
-        if not left or not right:
-            return (0, 0, [0], [])
-        # align the two input strings
-        dfsc = self.align(left, right)
-        # turn alignment-df into one pandas Series of sound correspondences
-        sc = dfsc["vals"] + self.connector + dfsc["keys"] if self.mode == "\
-adapt" else (dfsc["keys"] + self.connector + dfsc["vals"])
-        # read nr of examples for each sound corresp in sum-of-examples-dict
-        outlist = [self.sedict.get(i, 0) for i in sc]
-        # add up the nr of examples for each corresp in the word
-        outsum = sum(outlist)
-        # divide the sum through the length of the word, round on 2 decimals
-        normalised_outsum = round(outsum / len(dfsc), 2)
-        # add the in-between-steps if indicated so (useful for debugging)
-        return normalised_outsum, outsum, str(outlist), str(list(sc))
+    return shortest_path
```

### Comparing `loanpy-2.0.2/loanpy/tests/test_helpers_integration.py` & `loanpy-3.0.0/tests/test_scapplier_unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,701 +1,741 @@
-"""integration tests for loanpy.helpers.py (2.0 BETA) for pytest 7.1.1"""
+# -*- coding: utf-8 -*-
+"""unit tests for loanpy.scapplier with pytest 7.1.2"""
 
-from ast import literal_eval
-from inspect import ismethod
+import pytest
+from loanpy.scapplier import (Adrc, move_sc, edit_distance_with2ops, apply_edit,
+                          list2regex, tuples2editops, get_mtx,
+                          mtx2graph, dijkstra, add_edge, substitute_operations)
+from unittest.mock import patch, call
+from tempfile import TemporaryDirectory
+from collections import OrderedDict
 from os import remove
 from pathlib import Path
+import json
 
-from networkx import DiGraph
-from numpy import array
-from numpy.testing import assert_array_equal
-from pandas import DataFrame, Index, read_csv
-from pandas.testing import assert_frame_equal
-from pytest import raises
-
-from loanpy.helpers import (
-    Etym,
-    InventoryMissingError,
-    cldf2pd,
-    editops,
-    gensim_multiword,
-    get_mtx,
-    combine_ipalists,
-    clusterise,
-    mtx2graph,
-    read_cvfb,
-    read_dst,
-    read_forms,
-    tuples2editops)
-
-PATH2FORMS = Path(__file__).parent / "input_files" / "forms.csv"
-
-
-def test_plug_in_model():
-    pass  # unittest = integration test
-
-
-def test_read_cvfb():
-    """reading in cvfb.txt which is always in the same place"""
-    cvfb = read_cvfb()
-    assert isinstance(cvfb, tuple)
-    assert len(cvfb) == 2
-    # extremely long dictionary, so just type is checked
-    assert isinstance(cvfb[0], dict)
-    assert isinstance(cvfb[1], dict)
-    # extremely long dictionary, here's how long
-    assert len(cvfb[0]) == 6358
-    assert len(cvfb[1]) == 1240
-    assert all(cvfb[0][val] in ["C", "V"] for val in cvfb[0])
-    assert all(cvfb[1][val] in ["F", "B", "V"] for val in cvfb[1])
-
-    # verify that the dict is actually based on ipa_all.csv
-    # and that "C" corresponds to "+" and "V" "-" in col "ipa".
-    dfipa = read_csv(Path(__file__).parent.parent / "ipa_all.csv")
-    for i, c in zip(dfipa.ipa, dfipa.cons):
-        if c == "+":
-            assert cvfb[0][i] == "C"
-        elif c == "-":
-            assert cvfb[0][i] == "V"
-        else:
-            assert cvfb[0].get(i, "notindict") == "notindict"
-
-    del dfipa, cvfb
-
-
-def test_read_forms():
-    """test if CLDF's forms.csv is read in correctly"""
-    # test first break
-    assert read_forms(None) is None
-
-    # set up
-    dfexp = DataFrame({"Language_ID": [1, 2],
-                       "Segments": ["abc", "xyz"],  # pulled together segments
-                       "Cognacy": [1, 1]})
-
-    assert read_forms(None) is None
-    assert_frame_equal(read_forms(PATH2FORMS), dfexp)
-
-    # tear down
-    del dfexp
-
-
-def test_cldf2pd():
-    """test if the CLDF format is correctly tranformed to a pandas dataframe"""
-
-    # set up
-    dfin = read_csv(PATH2FORMS)
-    dfexp = DataFrame({"Target_Form": ["x y z"],
-                       "Source_Form": ["a b c"],
-                       "Cognacy": [1]})
-
+def test_init_with_files(tmp_path):
+    # Create temporary files for sound correspondence dictionary and inventories
+    sc_path = tmp_path / "sound_correspondences.json"
+    sc_path.write_text('{"a": {"b": "c"}}')
+    prosodic_inventory_path = tmp_path / "inventories.json"
+    prosodic_inventory_path.write_text('["CVCV"]')
+
+    # Initialize Adrc object with temporary file paths
+    obj = Adrc(sc=str(sc_path), prosodic_inventory=str(prosodic_inventory_path))
+
+    # Assert that sound correspondence dictionary and inventories were loaded properly
+    assert obj.sc == {"a": {"b": "c"}}
+    assert obj.prosodic_inventory == ["CVCV"]
+
+def test_init_without_files():
+    # Initialize Adrc object without files
+    obj = Adrc()
+
+    # Assert that sound correspondence dictionary and inventories are None
+    assert obj.sc is None
+    assert obj.prosodic_inventory is None
+
+def test_set_sc():
+    """
+    Test if sound correspondences are plugged in correctly into  attribute
+    """
+    obj = Adrc()
+    obj.set_sc("lol")
+    assert obj.sc == "lol"
+
+def test_set_prosodic_inventory():
+    """
+    Test if inventories are plugged in correctly into attribute
+    """
+    obj = Adrc()
+    obj.set_prosodic_inventory("rofl")
+    assert obj.prosodic_inventory == "rofl"
+
+class AdrcMonkey:
+    def __init__(self):
+        self.sc = [{},{},{},{},{},{}]
+        self.prosodic_inventory = []
+
+def test_move_sc():
+    """test if sound correspondences are moved correctly"""
+    # no setup, teardown, or patch needed here
+    assert move_sc(sclistlist=[["x", "x"]], whichsound=0,
+                   out=[[]]) == ([["x"]], [["x"]])
+
+    assert move_sc(sclistlist=[["x", "x"], ["y", "y"], ["z"]], whichsound=0,
+                   out=[["a"], ["b"], ["c"]]) == ([["x"], ["y", "y"], ["z"]],
+                                                  [["a", "x"], ["b"], ["c"]])
+
+    assert move_sc(sclistlist=[["x", "x"], ["y", "y"], ["z"]], whichsound=1,
+                   out=[["a"], ["b"], ["c"]]) == ([["x", "x"], ["y"], ["z"]],
+                                                  [["a"], ["b", "y"], ["c"]])
+
+    assert move_sc(sclistlist=[["", "x", "$"], ["", "y", "$"], ["", "$"]],
+                   whichsound=1, out=[["a"], ["b"], ["c"]]) == (
+        [["", "x", "$"], ["y", "$"], ["", "$"]], [["a"], ["b", "y"], ["c"]])
+
+    assert move_sc(sclistlist=[["", "$"], ["", "$"], ["Z", "2", "$"]],
+                   whichsound=2, out=[["o"], ["r"], ["f"]]) == (
+        [["", "$"], ["", "$"], ["2", "$"]], [["o"], ["r"], ["f", "2"]])
+
+
+def test_get_diff():
+    """test if the difference is calculated correctly
+    between the first two sound of a sound correspondence list"""
+
+    # test without exception
+    # set up: mock class, 2 attributes, 1 var for input-param
+    monkey_adrc = AdrcMonkey()
+    monkey_adrc.sc[1] = {"k k": 2, "k c": 1, "i e": 2, "i o": 1}
+    sclistlist = [["k", "c", "$"], ["e", "o", "$"],
+                  ["k", "c", "$"], ["e", "o", "$"]]
     # assert
-    assert cldf2pd(None, source_language="whatever",
-                   target_language="wtvr2") is None
-    assert_frame_equal(cldf2pd(dfin, source_language=1,
-                               target_language=2), dfexp)
-
-    # tear down
-    del dfexp, dfin
-
-
-def test_read_dst():
-    """test if input-string is correctly mapped to
-    method of panphon.distance.Distance"""
-    out = read_dst("weighted_feature_edit_distance")
-    assert ismethod(out)
-
-
-def test_flatten():
-    pass  # unittest == integration test
-
-
-def test_combine_ipalists():
-    """test if combinatorics is correctly applied to phonemes (#odometer)"""
-    inlist = [[["k", "g"], ["i", "e"]], [["b", "p"], ["u", "o"]]]
-    out = ["ki", "ke", "gi", "ge", "bu", "bo", "pu", "po"]
-    assert combine_ipalists(inlist) == out
-    del inlist, out
-
-
-def test_form2list():
-    pass  # unit == integration test
-
-
-def test_init():
-    """test if class Etym is initiated correctly"""
-    # set up: initiate without args
-    mocketym = Etym()
-
-    # assert that the right number of class attributes were instanciated
-    assert len(mocketym.__dict__) == 8
-
-    # assert phon2cv was read correctly
-    assert isinstance(mocketym.phon2cv, dict)
-    assert len(mocketym.phon2cv) == 6358
-    assert mocketym.phon2cv["k"] == "C"
-    assert mocketym.phon2cv["p"] == "C"
-    assert mocketym.phon2cv["l"] == "C"
-    assert mocketym.phon2cv["w"] == "C"
-    assert mocketym.phon2cv["C"] == "C"
-    assert mocketym.phon2cv["a"] == "V"
-    assert mocketym.phon2cv["e"] == "V"
-    assert mocketym.phon2cv["i"] == "V"
-    assert mocketym.phon2cv["o"] == "V"
-    assert mocketym.phon2cv["u"] == "V"
-
-    # assert vow2fb was read correctly
-    assert isinstance(mocketym.vow2fb, dict)
-    assert len(mocketym.vow2fb) == 1240
-    assert mocketym.vow2fb["e"] == "F"
-    assert mocketym.vow2fb["i"] == "F"
-    assert mocketym.vow2fb["o"] == "B"
-    assert mocketym.vow2fb["u"] == "B"
-
-    # assert the other 5 attributes were read correctly
-    assert mocketym.dfety is None
-    assert mocketym.phoneme_inventory is None
-    assert mocketym.cluster_inventory is None
-    assert mocketym.phonotactic_inventory is None
-    ismethod(mocketym.distance_measure)
-
-    # tear down
-    del mocketym
-
-    # set up2: run with advanced parameters
-    # input vars for init params
-    mocketym = Etym(forms_csv=PATH2FORMS, source_language=1, target_language=2)
-
-    # assert right number of attributes was initiated (7)
-    assert len(mocketym.__dict__) == 8
-
-    # (1) assert phon2cv was read correctly
-    assert isinstance(mocketym.phon2cv, dict)
-    assert len(mocketym.phon2cv) == 6358
-    assert mocketym.phon2cv["k"] == "C"
-    assert mocketym.phon2cv["p"] == "C"
-    assert mocketym.phon2cv["l"] == "C"
-    assert mocketym.phon2cv["w"] == "C"
-    assert mocketym.phon2cv["C"] == "C"
-    assert mocketym.phon2cv["a"] == "V"
-    assert mocketym.phon2cv["e"] == "V"
-    assert mocketym.phon2cv["i"] == "V"
-    assert mocketym.phon2cv["o"] == "V"
-    assert mocketym.phon2cv["u"] == "V"
-
-    # (2) assert vow2fb was read correctly
-    assert isinstance(mocketym.vow2fb, dict)
-    assert len(mocketym.vow2fb) == 1240
-    assert mocketym.vow2fb["e"] == "F"
-    assert mocketym.vow2fb["i"] == "F"
-    assert mocketym.vow2fb["o"] == "B"
-    assert mocketym.vow2fb["u"] == "B"
-
-    # (3) assert dfety was read correctly
-    assert_frame_equal(mocketym.dfety, DataFrame(
-        {"Target_Form": ["xyz"], "Source_Form": ["abc"], "Cognacy": [1]}))
-
-    # assert the other 4 attributes were read correctly
-    assert mocketym.phoneme_inventory == {'x', 'y', 'z'}
-    assert mocketym.cluster_inventory == {'x', 'y', 'z'}
-    assert mocketym.phonotactic_inventory == {"CVC"}
-    ismethod(mocketym.distance_measure)
-
-    # tear down
-    del mocketym
-
-
-def test_read_inventory():
-    """test if phoneme/cluster inventory is read in correctly"""
-    # assert first two exceptions: inv is not None and inv and forms are None
-    etym = Etym()
-    etym.forms_target_language = "some_inv"
-    assert etym.read_inventory("some_formscsv") == "some_formscsv"
-    assert etym.read_inventory(None) == set("someinv")  # tokeniser drops "_"
-    etym.forms_target_language = None
-    assert etym.read_inventory(None, None) is None
-
-    # assert calculations
-    etym.forms_target_language = ["a", "aab", "bc"]
-    assert etym.read_inventory(None) == set(['a', 'b', 'c'])
-    etym.forms_target_language = ["a", "ab", "baac"]
-    assert etym.read_inventory(None, clusterise
-                               ) == set(['aa', 'bb', 'c'])
-
-
-def test_get_inventories():
-    """test if phoneme/cluster/phonotactic inventories are read in well"""
-    # set up instancce
-    etym = Etym()
-    # run func, assert output
-    etym.get_inventories() == (None, None, None)
-
-    # rerun with non-default args
-    # create instancce
-    etym = Etym()
-    # run func, assert output
-    etym.get_inventories("param1", "param2", "param3", 4) == (
-        "param1", "param2", "param3")
-
-    # rerun with real etym instnace
-    etym = Etym(PATH2FORMS, source_language=1, target_language=2)
-    # run func
-    etym.get_inventories()
-    # assert assigned attributes
-    assert etym.phoneme_inventory == {'x', 'y', 'z'}
-    assert etym.cluster_inventory == {'x', 'y', 'z'}
-    assert etym.phonotactic_inventory == {'CVC'}
-
-    # tear down
-    del etym
-
+    assert Adrc.get_diff(
+        self=monkey_adrc,
+        sclistlist=sclistlist,
+        ipa=["k", "i", "k", "i"]) == [1, 1, 1, 1]
+    # there were no mock calls, so no calls to assert
+
+    # test first exception
+    # set up: mock class, 2 attributes, 1 var for input-param
+    monkey_adrc = AdrcMonkey()
+    monkey_adrc.sc[1] = {"k k": 2, "k c": 1, "i e": 2, "i o": 1}
+    sclistlist = [["k", "c", "x"], ["x", "$"]]
+    # assert
+    assert Adrc.get_diff(
+        self=monkey_adrc,
+        sclistlist=sclistlist,
+        ipa=["k", "i"]) == [1, float("inf")]
+    # no calls made so no calls to assert
+
+    # test second exception
+    # set up: mock class, 2 attributes, 1 var for input-param
+    monkey_adrc = AdrcMonkey()
+    monkey_adrc.sc[1] = {"k k": 0, "k c": 0, "i e": 7, "i o": 1}
+    sclistlist = [["k", "c", "x"], ["e", "o", "x"]]
+
+    # assert 1
+    assert Adrc.get_diff(
+        self=monkey_adrc,
+        sclistlist=sclistlist,
+        ipa=["k", "i"]) == [9999999, 6]
+
+    # teardown/setup: overwrite attribute nsedict
+    monkey_adrc.sc[1] = {"k k": 0, "k c": 0, "i e": 7, "i o": 7}
+
+    # assert 2
+    assert Adrc.get_diff(
+        self=monkey_adrc,
+        sclistlist=sclistlist,
+        ipa=["k", "i"]) == [9999999, 0]
+
+    # teardown/setup: overwrite attribute nsedict
+    monkey_adrc.sc[1] = {"k k": 0, "k c": 0, "i e": 0, "i o": 0}
+
+    # assert 3
+    assert Adrc.get_diff(
+        self=monkey_adrc,
+        sclistlist=sclistlist,
+        ipa=["k", "i"]) == [9999999, 9999999]
 
-def test_read_phonotactic_inv():
-    """test if phonotactic inventory is read in correctly"""
-    # set up rest
-    etym = Etym()
-    # from forms.csv in CLDF
-    etym.forms_target_language = ["ab", "ab", "aa", "bb", "bb", "bb"]
-    # assert with different parameter combinations
-    assert etym.read_phonotactic_inv(phonotactic_inventory=["a", "b", "c"],
-                                     ) == ["a", "b", "c"]
-    etym.forms_target_language = None
-    assert etym.read_phonotactic_inv(phonotactic_inventory=None,
-                                     ) is None
-    etym.forms_target_language = ["ab", "ab", "aa", "bb", "bb", "bb"]
-    # now just read the most frquent 2 structures. VV is the 3rd frquent. so
-    # not in the output.
-    assert etym.read_phonotactic_inv(phonotactic_inventory=None,
-                                     howmany=2) == {"CC", "VC"}
+    # no calls made so no calls to assert
 
     # tear down
-    del etym
+    del monkey_adrc, sclistlist
 
 
-def test_word2phonotactics():
-    """test if the phonotactic profile of a word is correctly concluded"""
+def test_read_sc():
+    """test if sound correspondences are read correctly"""
 
-    etym = Etym()
-    assert etym.word2phonotactics("t͡ʃɒlːoːkøz") == "CVCVCVC"
-    assert etym.word2phonotactics("hortobaːɟ") == "CVCCVCVC"
-    # hashtag is ignored
-    assert etym.word2phonotactics("lɒk#sɒkaːlːɒʃ") == "CVCCVCVCVC"
-    assert etym.word2phonotactics("boɟ!ɒ") == "CVCV"  # exclam. mark is ignored
-    assert etym.word2phonotactics("ɡɛlːeːr") == "CVCVC"
+    # set up mock class
+    class AdrcMonkeyread_sc:
+        def __init__(self, get_diff=""):
+            self.get_diff_returns = iter(get_diff)
+            self.get_diff_called_with = []
+            self.sc = [{},{},{},{},{},{}]
+
+        def get_diff(self, sclistlist, ipa):
+            self.get_diff_called_with.append((sclistlist, ipa))
+            return next(self.get_diff_returns)
+
+    # test if first break works (max)
+
+    # set up mock class, plug in mock sc[0], mock tokenise, mock math.prod
+    monkey_adrc = AdrcMonkeyread_sc()
+    monkey_adrc.sc[0] = {"k": ["k", "h"], "i": ["e", "o"]}
+    with patch("loanpy.scapplier.prod") as prod_mock:
+        prod_mock.return_value = 16
+
+        # assert
+        assert Adrc.read_sc(self=monkey_adrc, ipa=["k", "i", "k", "i"],
+                            howmany=1000) == [
+            ["k", "h"], ["e", "o"], ["k", "h"], ["e", "o"]]
+
+    # assert 3 calls: get_diff, prod_mock, tokenise
+    assert monkey_adrc.get_diff_called_with == []  # not called!
+    prod_mock.assert_called_with([2, 2, 2, 2])
+
+    # test if second break works (min)
+
+    # set up mock class, plug in mock sc[0], mock math.prod
+    monkey_adrc = AdrcMonkeyread_sc()
+    monkey_adrc.sc[0] = {"k": ["k", "h"], "i": ["e", "o"]}
+    with patch("loanpy.scapplier.prod", side_effect=[16, 1]) as prod_mock:
+
+        # assert read_sc works with tokenised list as input
+        assert Adrc.read_sc(
+            self=monkey_adrc,
+            ipa=["k", "i", "k", "i"],
+            howmany=1) == [["k"], ["e"], ["k"], ["e"]]
+
+    # assert 2 calls: get_diff, prod_mock
+    assert monkey_adrc.get_diff_called_with == []  # not called!
+    assert prod_mock.call_args_list == [
+        call([2, 2, 2, 2]), call([1, 1, 1, 1])]
+
+    # test while loop with 1 minimum
+
+    # set up mock class, plug in mock sc[0], mock move_sc, mock math.prod
+    monkey_adrc = AdrcMonkeyread_sc(get_diff=[[4, 5]])
+    monkey_adrc.sc[0] = {"k": ["k", "h"], "i": ["e", "o"]}
+    with patch("loanpy.scapplier.move_sc") as move_sc_mock:
+        move_sc_mock.return_value = ([["$"], ["o", "$"]], [["k", "h"], ["e"]])
+        with patch("loanpy.scapplier.prod", side_effect=[4, 1, 2]) as prod_mock:
+
+            # assert sound correspondences are read in correctly
+            assert Adrc.read_sc(self=monkey_adrc, ipa=["k", "i"],
+                                howmany=2) == [
+                ["k", "h"], ["e"]]
+
+    # assert 3 calls: prod_mock, get_diff, move_sc
+    assert prod_mock.call_args_list == [
+        call([2, 2]), call([1, 1]), call([2, 1])]
+    assert monkey_adrc.get_diff_called_with == [
+        ([["k", "h", "$"], ["e", "o", "$"]], ["k", "i"])]
+    move_sc_mock.assert_called_with(
+        [["k", "h", "$"], ["e", "o", "$"]], 0, [["k"], ["e"]])
+
+    # test while loop with 2 minima (🚲)
+
+    # set up mock class, plug in mock sc[0],
+    # def var for side_effect of move_sc, mock move_sc, mock math.prod
+    monkey_adrc = AdrcMonkeyread_sc(get_diff=[[2, 2, 5], [2, 2, 5], [3, 2, 5]])
+    monkey_adrc.sc[0] = {"k": ["k", "h", "s"], "i": ["e", "o"],
+                          "p": ["b", "v"]}
+    se_move_sc = [
+        ([["s", "$"], ["o", "$"], ["v", "$"]], [["k", "h"], ["e"], ["b"]]),
+        ([["s", "$"], ["$"], ["v", "$"]], [["k", "h"], ["e", "o"], ["b"]])
+    ]
+    with patch("loanpy.scapplier.move_sc", side_effect=se_move_sc) as move_sc_mock:
+        with patch("loanpy.scapplier.prod", side_effect=[
+                12, 1, 1, 2, 4]) as prod_mock:
+            # prod "3" gets only called once, bc difflist1!=difflist2, so 2nd
+            # while loop doesnt call prod
+
+            # assert read_sc works
+            assert Adrc.read_sc(self=monkey_adrc, ipa=["k", "i", "p"],
+                                howmany=3) == [["k", "h"], ["e", "o"], ["b"]]
+
+    # assert calls: prod_mock, get_diff, move_sc
+    assert prod_mock.call_args_list == [call([3, 2, 2]), call(
+        [1, 1, 1]), call([1, 1, 1]), call([2, 1, 1]), call([2, 2, 1])]
+    assert monkey_adrc.get_diff_called_with == [
+        ([["k", "h", "s", "$"], ["e", "o", "$"], ["b", "v", "$"]],
+         ["k", "i", "p"]),
+        ([["s", "$"], ["o", "$"], ["v", "$"]], ["k", "i", "p"]),
+        ([["s", "$"], ["$"], ["v", "$"]], ["k", "i", "p"])]
+    assert move_sc_mock.call_args_list == [
+        call([["k", "h", "s", "$"], ["e", "o", "$"], ["b", "v", "$"]],
+             0, [["k"], ["e"], ["b"]]),
+        call([["s", "$"], ["o", "$"], ["v", "$"]],
+             1, [["k", "h"], ["e"], ["b"]])]
 
     # tear down
-    del etym
-
+    del AdrcMonkeyread_sc, monkey_adrc, se_move_sc
 
-def test_word2phonotactics_keepcv():
-    """Not used in loanpy. Test if C and V is kept
-    during phonotactic profiling"""
-    etym = Etym()
-    assert etym.word2phonotactics(
-        ['C', 'V', 'C', 'V', 'k', 'ø', 'z']) == "CVCVCVC"
-    assert etym.word2phonotactics(
-        ['h', 'o', 'r', 'C', 'V', 'C', 'V', 'ɟ']) == "CVCCVCVC"
-    assert etym.word2phonotactics(
-        ['l', 'V', 'k', 's', 'ɒ', 'k', 'V', 'C', 'V', 'ʃ']) == "CVCCVCVCVC"
-    assert etym.word2phonotactics(['C', 'o', '!', 'ɟ', 'V']) == "CVCV"
-    assert etym.word2phonotactics(["C", "V", "lː", "eː", "r"]) == "CVCVC"
-    del etym
-
-
-def test_harmony():
-    """Test if it is detected correctly whether a word does or does not
-    have front-back vowel harmony"""
-    etym = Etym()
-    assert etym.has_harmony(
-        ['b', 'o', 't͡s', 'i', 'b', 'o', 't͡s', 'i']) is False
-    assert etym.has_harmony("bot͡sibot͡si") is False
-    assert etym.has_harmony("tɒrkɒ") is True
-    assert etym.has_harmony("ʃɛfylɛʃɛ") is True
-    del etym
-
-
-def test_repair_harmony():
-    """test if words without front-back vowel harmony are repaired correctly"""
-    etym = Etym()
-    assert etym.repair_harmony(ipalist='kɛsthɛj') == [
-        ['k', 'ɛ', 's', 't', 'h', 'ɛ', 'j']]
-    assert etym.repair_harmony(ipalist='ɒlʃoːørʃ') == [
-        ['ɒ', 'l', 'ʃ', 'oː', 'B', 'r', 'ʃ']]
-    assert etym.repair_harmony(ipalist=[
-        'b', 'eː', 'l', 'ɒ', 't', 'ɛ', 'l', 'ɛ', 'p']) == [
-        ['b', 'eː', 'l', 'F', 't', 'ɛ', 'l', 'ɛ', 'p']]
-    assert etym.repair_harmony(ipalist='bɒlɒtonkɛnɛʃɛ') == [
-        ['b', 'F', 'l', 'F', 't', 'F', 'n', 'k', 'ɛ', 'n', 'ɛ', 'ʃ', 'ɛ'],
-        ['b', 'ɒ', 'l', 'ɒ', 't', 'o', 'n', 'k', 'B', 'n', 'B', 'ʃ', 'B']]
-    del etym
-
-
-def test_get_fb():
-    """test if front and back vowels are fetched correctly"""
-    etym = Etym()
-    assert etym.get_fb(ipalist=['k', 'ɛ', 's', 't', 'h', 'ɛ', 'j']) == [
-        'k', 'ɛ', 's', 't', 'h', 'ɛ', 'j']
-    assert etym.get_fb(ipalist=[
-        'ɒ', 'l', 'ʃ', 'oː', 'ø', 'r', 'ʃ'], turnto="B") == [
-        'ɒ', 'l', 'ʃ', 'oː', 'B', 'r', 'ʃ']
-    assert etym.get_fb(['b', 'ɒ', 'l', 'ɒ', 't', 'o', 'n',
-                        'k', 'ɛ', 'n', 'ɛ', 'ʃ', 'ɛ'], "B") == [
-        'b', 'ɒ', 'l', 'ɒ', 't', 'o', 'n', 'k', 'B', 'n', 'B', 'ʃ', 'B']
-    assert etym.get_fb(['b', 'ɒ', 'l', 'ɒ', 't', 'o', 'n',
-                        'k', 'ɛ', 'n', 'ɛ', 'ʃ', 'ɛ'], "F") == [
-        'b', 'F', 'l', 'F', 't', 'F', 'n', 'k', 'ɛ', 'n', 'ɛ', 'ʃ', 'ɛ']
-    del etym
-
-
-def test_get_scdictbase():
-    """test if heuristic sound correspondence dictionary
-    is calculated correctly"""
-    # test with phoneme_inventory manually plugged in
-    etym = Etym(phoneme_inventory=["a", "b", "c"])
-    scdictbase = etym.get_scdictbase(write_to=False)
-    assert isinstance(scdictbase, dict)
-    assert len(scdictbase) == 6371
-    assert scdictbase["p"] == ["b", "c", "a"]  # b is obv most similar to p
-    assert scdictbase["h"] == ["c", "b", "a"]
-    assert scdictbase["e"] == ["a", "b", "c"]
-    assert scdictbase["C"] == ["b", "c"]
-    assert scdictbase["V"] == ["a"]
-    assert scdictbase["F"] == ["a"]
-    assert scdictbase["B"] == []
-    del etym, scdictbase
-
-    # test with invetory extracted from forms.csv
-    etym = Etym(PATH2FORMS, source_language=1, target_language=2)
-    scdictbase = etym.get_scdictbase(write_to=False)
-    assert isinstance(scdictbase, dict)
-    assert len(scdictbase) == 6371
-    assert scdictbase["p"] == ["z", "x", "y"]  # IPA z is most similar to IPA p
-    assert scdictbase["h"] == ["x", "z", "y"]
-    assert scdictbase["e"] == ["y", "z", "x"]
-    assert scdictbase["C"] == ["x", "z"]
-    assert scdictbase["V"] == ["y"]
-    assert scdictbase["F"] == ["y"]
-    assert scdictbase["B"] == []
-    del etym, scdictbase
-
-    # test if written correctly and if param most_common works
+@patch("loanpy.scapplier.list2regex", side_effect=["(k)", "(i)", "(h)", "(e)"])
+def test_reconstruct1(list2regex_mock):
+    """test first break: some sounds are not in sc[0]"""
+
+    # set up mock class, plug in mock sc[0], mock clusterise
+    monkey_adrc = AdrcMonkey()
+    monkey_adrc.sc[0] = {"#-": ["-"], "#k": ["k", "h"], "k": ["h"],
+                          "-#": ["-"]}
+
+    # assert reconstruct works
+    assert Adrc.reconstruct(
+        self=monkey_adrc,
+        ipastr="k i k i") == "i not old"
+
+# set up mock class, will be used multiple times throughout this test
+class AdrcMonkeyReconstruct:
+    def __init__(
+        self,
+        read_sc_returns):
+        self.read_sc_called_with = []
+        self.read_sc_returns = read_sc_returns
+        self.prosodic_inventory = []
+        self.sc = [{},{},{},{},{},{}]
+
+    def read_sc(self, ipalist, howmany):
+        self.read_sc_called_with.append((ipalist, howmany))
+        return self.read_sc_returns
+
+@patch("loanpy.scapplier.list2regex", side_effect=["(k)", "(i)", "(h)", "(e)"])
+def test_reconstruct2(list2regex_mock):
+    """Test if reconstructions with howmany=1 work fine"""
+
+    # set up: create instance of mock class
+    monkey_adrc = AdrcMonkeyReconstruct(
+        read_sc_returns=[["-"], ["k"], ["i"], ["h"], ["e"], ["-"]])
+
+    # set up: plug in sound correspondence dictionary into mock class
+    monkey_adrc.sc[0] = {
+        "#-": ["-"], "#k": ["k", "h"], "i": ["i", "e"],
+        "k": ["h"], "i#": ["e", "o"], "-#": ["-"]
+    }
+    # assert reconstruct works
+    assert Adrc.reconstruct(
+        self=monkey_adrc,
+        ipastr="k i k i",
+        ) == "^(k)(i)(h)(e)$"
+
+    # assert 3 calls: tokenise, read_sc, list2regex
+    assert monkey_adrc.read_sc_called_with == [
+        (['k', 'i', 'k', 'i',], 1)]
+    assert list2regex_mock.call_args_list == [
+        call(["k"]), call(["i"]),
+        call(["h"]), call(["e"])]
+
+@patch("loanpy.scapplier.list2regex", side_effect=["(k|h)", "(i)", "(h)", "(e)"])
+def test_reconstruct3(list2regex_mock):
+    """Test if reconstructions with howmany=2 work fine"""
 
     # set up
-    etym = Etym(phoneme_inventory=["a", "b", "c"])
-    path2scdict_integr_test = Path(__file__).parent / "integr_test_scdict.txt"
-    etym.get_scdictbase(write_to=path2scdict_integr_test, most_common=2)
-    with open(path2scdict_integr_test, "r", encoding="utf-8") as f:
-        scdictbase = literal_eval(f.read())
-
-    # assert
-    assert isinstance(scdictbase, dict)
-    assert len(scdictbase) == 6371
-    assert scdictbase["p"] == ["b", "c"]  # b is obv most similar to p
-    assert scdictbase["h"] == ["c", "b"]
-    assert scdictbase["e"] == ["a", "b"]
-    assert scdictbase["C"] == ["b", "c"]
-    assert scdictbase["V"] == ["a"]
-    assert scdictbase["F"] == ["a"]
-    assert scdictbase["B"] == []
-
-    # tear down
-    remove(path2scdict_integr_test)
-    del etym, scdictbase, path2scdict_integr_test
-
-
-def test_rankclosest():
-    """test if closest phonemes from inventory are ranked correctly"""
-    # assert error is being raised correctly
-    etym = Etym()
-    with raises(InventoryMissingError) as inventorymissingerror_mock:
-        etym.rank_closest(ph="d", howmany=3, inv=None)
-    assert str(inventorymissingerror_mock.value
-               ) == "define phoneme inventory or forms.csv"
-    del etym
-
-    # assert phonemes are ranked correctly
-    etym = Etym(phoneme_inventory=["a", "b", "c"])
-    assert etym.rank_closest(ph="d") == "b, c, a"
-    assert etym.rank_closest(ph="d", howmany=2) == "b, c"
-    assert etym.rank_closest(ph="d", inv=["r", "t", "l"], howmany=1) == "t"
-    del etym
-
-
-def test_rankclosest_phonotactics():
-    """test if most similar phonotactic profiles from inventory
-    are ranked up correctly"""
-    # assert error is raised correctly if phoneme_inventory is missing
-    etym = Etym()
-    with raises(InventoryMissingError) as inventorymissingerror_mock:
-        # assert error is raised
-        etym.rank_closest_phonotactics(struc="CV", howmany=float("inf"))
-        assert str(inventorymissingerror_mock.value
-                   ) == "define phonotactic phoneme_inventory or forms.csv"
-    del etym
-
-    # assert structures are ranked correctly
-    etym = Etym(PATH2FORMS, source_language=1, target_language=2)
-    # phonotactic_inventory is only lg2 aka "xyz"
-    assert etym.rank_closest_phonotactics(struc="CVCV") == "CVC"
-    assert etym.rank_closest_phonotactics(
-        struc="CVCV", howmany=3, inv=[
-            "CVC", "CVCVV", "CCCC", "VVVVVV"]) == "CVCVV, CVC, CCCC"
-    del etym
-
-
-def test_gensim_multiword():
-    pass  # checked in detail and unit == integration test (!)
-
-
-def test_list2regex():
-    pass  # no patches in unittest
+    monkey_adrc = AdrcMonkeyReconstruct(
+        read_sc_returns=[["-"], ["k", "h"], ["i"], ["h"], ["e"], ["-"]])
+    monkey_adrc.sc[0] = {
+        "#-": ["-"], "#k": ["k", "h"], "i": ["i", "e"],
+        "k": ["h"], "i#": ["e", "o"], "-#": ["-"]
+    }
+
+    # assert reconstruct works
+    assert Adrc.reconstruct(
+        self=monkey_adrc,
+        ipastr="k i k i",
+        howmany=2) == "^(k|h)(i)(h)(e)$"
+
+    # assert 3 calls: clusterise, read_sc, list2regex
+    assert monkey_adrc.read_sc_called_with == [
+        (['k', 'i', 'k', 'i',], 2)]
+    assert list2regex_mock.call_args_list == [
+        call(["k", "h"]), call(["i"]),
+        call(["h"]), call(["e"])]
+
+@patch("loanpy.scapplier.get_mtx")
+@patch("loanpy.scapplier.mtx2graph")
+@patch("loanpy.scapplier.dijkstra")
+@patch("loanpy.scapplier.tuples2editops")
+@patch("loanpy.scapplier.apply_edit")
+def test_repair_phonotactics1(apply_edit_mock, tuples2editops_mock,
+    dijkstra_mock, mtx2graph_mock, get_mtx_mock):
+    """
+    test if phonotactic structures are adapted correctly
+    when no data available
+    """
+
+    # test all in dict
+    # set up mock class, used multiple times throughout this test
+    class AdrcMonkeyrepair_phonotactics:
+        def __init__(self):
+            self.get_closest_phonotactics_returns = "V"
+            self.get_closest_phonotactics_called_with = []
+            self.sc = [{}, {}, {}, {}, {}, {}]
+
+        def get_closest_phonotactics(self, *args):
+            self.get_closest_phonotactics_called_with.append([*args])
+            return self.get_closest_phonotactics_returns
+    # teardown/setup: overwrite mock class, plug in sc[3],
+    monkey_adrc = AdrcMonkeyrepair_phonotactics()
+
+    get_mtx_mock.return_value = [[0, 0], [0, 1]]
+    mtx2graph_mock.return_value = {
+        (0, 0): {(0, 1): 100, (1, 0): 49},
+        (0, 1): {(1, 1): 49},
+        (1, 0): {(1, 1): 100},
+        (1, 1): {}
+        }
+    dijkstra_mock.return_value = [(0, 0), (1, 0), (1, 1)]
+    tuples2editops_mock.return_value = ['substitute C by V']
+    apply_edit_mock.return_value = "V"
+
+    # assert repair_phonotactics is working
+    assert Adrc.repair_phonotactics(
+        self=monkey_adrc,
+        ipalist="k",
+        prosody="C") == 'V'
+
+    # dijkstra, apply_edit
+    assert monkey_adrc.get_closest_phonotactics_called_with == [['C']]
+    get_mtx_mock.assert_called_with("C", "V")
+    mtx2graph_mock.assert_called_with(get_mtx_mock.return_value)
+    dijkstra_mock.assert_called_with(graph=mtx2graph_mock.return_value,
+                                     start=(0, 0), end=(1, 1)
+                                     )
+    tuples2editops_mock.assert_called_with(dijkstra_mock.return_value,
+                                           "C", "V")
+    apply_edit_mock.assert_called_with("k", tuples2editops_mock.return_value)
+
+@patch("loanpy.scapplier.get_mtx")
+@patch("loanpy.scapplier.mtx2graph")
+@patch("loanpy.scapplier.dijkstra")
+@patch("loanpy.scapplier.tuples2editops")
+@patch("loanpy.scapplier.apply_edit")
+def test_repair_phonotactics2(apply_edit_mock, tuples2editops_mock,
+    dijkstra_mock, mtx2graph_mock, get_mtx_mock):
+    """
+    test if phonotactic structures are adapted correctly
+    when data is available
+    """
+
+    # test all in dict
+    # set up mock class, used multiple times throughout this test
+    class AdrcMonkeyrepair_phonotactics:
+        def __init__(self):
+            self.sc = [{}, {}, {}, {}, {}, {}]
+            self.prosodic_inventory =[]
+
+    # teardown/setup: overwrite mock class, plug in sc[3],
+    monkey_adrc = AdrcMonkeyrepair_phonotactics()
+    monkey_adrc.sc[3] = {"C": ["V", "CV"]}
+
+    get_mtx_mock.return_value = [[0, 0], [0, 1]]
+    mtx2graph_mock.return_value = {
+        (0, 0): {(0, 1): 100, (1, 0): 49},
+        (0, 1): {(1, 1): 49},
+        (1, 0): {(1, 1): 100},
+        (1, 1): {}
+        }
+    dijkstra_mock.return_value = [(0, 0), (1, 0), (1, 1)]
+    tuples2editops_mock.return_value = ['substitute C by V']
+    apply_edit_mock.return_value = "V"
+
+    # assert repair_phonotactics is working
+    assert Adrc.repair_phonotactics(
+        self=monkey_adrc,
+        ipalist="k",
+        prosody="C") == 'V'
+
+    # dijkstra, apply_edit
+    get_mtx_mock.assert_called_with("C", "V")
+    mtx2graph_mock.assert_called_with(get_mtx_mock.return_value)
+    dijkstra_mock.assert_called_with(graph=mtx2graph_mock.return_value,
+                                     start=(0, 0), end=(1, 1)
+                                     )
+    tuples2editops_mock.assert_called_with(dijkstra_mock.return_value,
+                                           "C", "V")
+    apply_edit_mock.assert_called_with("k", tuples2editops_mock.return_value)
+
+# set up mock class, used multiple times throughout this test.
+class AdrcMonkeyAdapt:
+    def __init__(self, read_screturns=[
+            [["k", "h"], ["e", "o"], ["k"], ["e"]]],
+            combineipalistsreturns=[
+            "kek", "kok", "hek", "hok",
+            "ketke", "kotke", "hetke", "hotke"]):
+        self.repair_phonotactics_called_with = None
+        self.read_sc_returns = iter(read_screturns)
+        self.read_sc_called_with = []
+        self.prosodic_inventory = ["CVCCV"]
+
+    def repair_phonotactics(self, *args):
+        self.repair_phonotactics_called_with = [*args]
+        return 'k i C k i'
+
+    def read_sc(self, *args):
+        self.read_sc_called_with.append([*args])
+        return next(self.read_sc_returns)
+
+    # create instance of mock class
+
+@patch("loanpy.scapplier.product")
+def test_adapt1(product_mock):
+    """test if words are adapted correctly without prosody, howmany=4"""
+
+    adrc_monkey = AdrcMonkeyAdapt()
+    product_mock.return_value = [
+        ("k", "e", "t", "e"), ("k", "o", "t", "e"),
+        ("h", "e", "t", "e"), ("h", "o", "t", "e")
+                                         ]
+    # assert adapt is working
+    assert Adrc.adapt(
+        self=adrc_monkey,
+        ipastr="k i k i",
+        howmany=4
+        ) == ["kete", "kote", "hete", "hote"]
+
+    assert not adrc_monkey.repair_phonotactics_called_with
+    assert adrc_monkey.read_sc_called_with == [[["k", "i", "k", "i"], 4]]
+    product_mock.assert_called_with(
+            ["k", "h"], ["e", "o"], ["k"], ["e"]
+                                   )
+
+@patch("loanpy.scapplier.product")
+def test_adapt2(product_mock):
+    """test if words are adapted correctly with prosody, howmany=8"""
+
+    adrc_monkey = AdrcMonkeyAdapt()
+    product_mock.return_value = [
+        ("k", "e", "k"), ("k", "o", "k"), ("h", "e", "k"), ("h", "o", "k"),
+        ("k", "e", "t", "k", "e"), ("k", "o", "t", "k", "e"),
+        ("h", "e", "t", "k", "e"), ("h", "o", "t", "k", "e")]
+
+    # assert adapt is working
+    assert Adrc.adapt(
+        self=adrc_monkey,
+        ipastr="k i k i",
+        prosody="CVCV",
+        howmany=8
+        ) == ["kek", "kok", "hek", "hok", "ketke", "kotke", "hetke", "hotke"]
+
+class TestRankClosestPhonotactics:
+    @pytest.fixture
+    def adrc_instance(self):
+        with TemporaryDirectory() as temp_dir:
+            temp_path = Path(temp_dir) / "prosodic_inventory.json"
+            with open(temp_path, "w+", encoding='utf-8') as f:
+                f.write(json.dumps(["CVCV", "CVVC", "VCVC",
+                "CCVV", "CVC", "CVV", "VCV", "CV"]))
+            yield Adrc(prosodic_inventory=temp_path)
+
+    @patch('loanpy.scapplier.edit_distance_with2ops')
+    @patch('loanpy.scapplier.min')
+    def test_get_closest_phonotactics_all(self,
+            mock_min, mock_edit_distance, adrc_instance):
+        mock_edit_distance.side_effect = [0, 1, 1, 2, 2, 2, 2, 2]
+        mock_min.return_value = (0, "CVCV")
+        result = adrc_instance.get_closest_phonotactics("CVCV")
+        assert result == "CVCV"
+
+        calls = [call("CVCV", i) for i in adrc_instance.prosodic_inventory]
+        mock_edit_distance.assert_has_calls(calls)
+        mock_min.assert_called_once_with([(0, 'CVCV'),
+        (1, 'CVVC'), (1, 'VCVC'), (2, 'CCVV'), (2, 'CVC'), (2, 'CVV'),
+        (2, 'VCV'), (2, 'CV')])
 
 
 def test_edit_distance_with2ops():
-    pass  # no patches in unittest
-
-
-def test_get_mtx():
-    """Dynamic programming. Test if matrix of edit operations is
-    calculated correctly"""
-    # assert error is raised if one of the input strings is empty
-    with raises(IndexError) as indexerror_mock:
-        get_mtx("a", "")
-    assert str(indexerror_mock.value == "list index out of range")
-
-    with raises(IndexError) as indexerror_mock:
-        get_mtx("", "bla")
-    assert str(indexerror_mock.value == "list index out of range")
-
-    with raises(IndexError) as indexerror_mock:
-        get_mtx("", "")
-    assert str(indexerror_mock.value == "list index out of range")
-
-    # illustration with small examples
-    # anchor is 0 if first chars are same
-    assert_array_equal(get_mtx("a", "a"), array([[0., 1.], [1., 0.]]))
-
-    # anchor is 2 if first chars are different
-    assert_array_equal(get_mtx("b", "a"), array([[0., 1.], [1., 2.]]))
-
-    assert_array_equal(get_mtx("xy", "y"),
-                       array([[0., 1., 2.],
-                              [1., 2., 1.]]))  # 1 insertion
-
-    assert_array_equal(get_mtx("y", "xy"),
-                       array([[0., 1.],
-                              [1., 2.],
-                              [2., 1.]]))  # 1 deletion
-
-    assert_array_equal(get_mtx("z", "xy"),
-                       array([[0., 1.],
-                              [1., 2.],
-                              [2., 3.]]))  # 1 del + 2 ins = 3 esit ops
-
-    assert_array_equal(get_mtx("Bécs", "Pécs"),
-                       # delete B insert P: 2 editops
-                       array([[0., 1., 2., 3., 4.],
-                              [1., 2., 3., 4., 5.],
-                              [2., 3., 2., 3., 4.],
-                              [3., 4., 3., 2., 3.],
-                              [4., 5., 4., 3., 2.]]))
-
-    assert_array_equal(get_mtx("Komárom", "Révkomárom"),
-                       array([[0., 1., 2., 3., 4., 5., 6., 7.],
-                              [1., 2., 3., 4., 5., 6., 7., 8.],
-                              [2., 3., 4., 5., 6., 7., 8., 9.],
-                              [3., 4., 5., 6., 7., 8., 9., 10.],
-                              [4., 5., 6., 7., 8., 9., 10., 11.],
-                              [5., 6., 5., 6., 7., 8., 9., 10.],
-                              [6., 7., 6., 5., 6., 7., 8., 9.],
-                              [7., 8., 7., 6., 5., 6., 7., 8.],
-                              [8., 9., 8., 7., 6., 5., 6., 7.],
-                              [9., 10., 9., 8., 7., 6., 5., 6.],
-                              [10., 11., 10., 9., 8., 7., 6., 5.]]))
-
-    assert_array_equal(get_mtx("Révkomárom", "Komárom"),
-                       array([[0., 1., 2., 3., 4., 5., 6., 7., 8., 9., 10.],
-                              [1., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11.],
-                              [2., 3., 4., 5., 6., 5., 6., 7., 8., 9., 10.],
-                              [3., 4., 5., 6., 7., 6., 5., 6., 7., 8., 9.],
-                              [4., 5., 6., 7., 8., 7., 6., 5., 6., 7., 8.],
-                              [5., 6., 7., 8., 9., 8., 7., 6., 5., 6., 7.],
-                              [6., 7., 8., 9., 10., 9., 8., 7., 6., 5., 6.],
-                              [7., 8., 9., 10., 11., 10., 9., 8., 7., 6., 5.]
-                              ]))
-
-    assert_array_equal(get_mtx("Tata", "Tatbánya"),
-                       array([[0., 1., 2., 3., 4.],
-                              [1., 0., 1., 2., 3.],
-                              [2., 1., 0., 1., 2.],
-                              [3., 2., 1., 0., 1.],
-                              [4., 3., 2., 1., 2.],
-                              [5., 4., 3., 2., 3.],
-                              [6., 5., 4., 3., 4.],
-                              [7., 6., 5., 4., 5.],
-                              [8., 7., 6., 5., 4.]]))
-
-    assert_array_equal(get_mtx("Budapest", "Debrecen"),
-                       array([[0., 1., 2., 3., 4., 5., 6., 7., 8.],
-                              [1., 2., 3., 4., 5., 6., 7., 8., 9.],
-                              [2., 3., 4., 5., 6., 7., 6., 7., 8.],
-                              [3., 4., 5., 6., 7., 8., 7., 8., 9.],
-                              [4., 5., 6., 7., 8., 9., 8., 9., 10.],
-                              [5., 6., 7., 8., 9., 10., 9., 10., 11.],
-                              [6., 7., 8., 9., 10., 11., 10., 11., 12.],
-                              [7., 8., 9., 10., 11., 12., 11., 12., 13.],
-                              [8., 9., 10., 11., 12., 13., 12., 13., 14.]]))
-
-    assert_array_equal(get_mtx("Debrecen", "Beregszász"),
-                       array([[0., 1., 2., 3., 4., 5., 6., 7., 8.],
-                              [1., 2., 3., 4., 5., 6., 7., 8., 9.],
-                              [2., 3., 2., 3., 4., 5., 6., 7., 8.],
-                              [3., 4., 3., 4., 3., 4., 5., 6., 7.],
-                              [4., 5., 4., 5., 4., 3., 4., 5., 6.],
-                              [5., 6., 5., 6., 5., 4., 5., 6., 7.],
-                              [6., 7., 6., 7., 6., 5., 6., 7., 8.],
-                              [7., 8., 7., 8., 7., 6., 7., 8., 9.],
-                              [8., 9., 8., 9., 8., 7., 8., 9., 10.],
-                              [9., 10., 9., 10., 9., 8., 9., 10., 11.],
-                              [10., 11., 10., 11., 10., 9., 10., 11., 12.]]))
-
-    assert_array_equal(
-        get_mtx("Szentpétervár", "Vlagyivosztok"),
- array([[0., 1., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11., 12., 13.],
-        [1., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11., 12., 13., 14.],
-        [2., 3., 4., 5., 6., 7., 8., 9., 10., 11., 12., 13., 14., 15.],
-        [3., 4., 5., 6., 7., 8., 9., 10., 11., 12., 13., 14., 15., 16.],
-        [4., 5., 6., 7., 8., 9., 10., 11., 12., 13., 14., 15., 16., 17.],
-        [5., 6., 7., 8., 9., 10., 11., 12., 13., 14., 15., 16., 17., 18.],
-        [6., 7., 8., 9., 10., 11., 12., 13., 14., 15., 16., 17., 18., 19.],
-        [7., 8., 9., 10., 11., 12., 13., 14., 15., 16., 17., 16., 17., 18.],
-        [8., 9., 10., 11., 12., 13., 14., 15., 16., 17., 18., 17., 18., 19.],
-        [9., 10., 11., 12., 13., 14., 15., 16., 17., 18., 19., 18., 19., 20.],
-        [10., 11., 10., 11., 12., 13., 14., 15., 16., 17., 18., 19., 20., 21.],
-        [11., 12., 11., 12., 13., 12., 13., 14., 15., 16., 17., 18., 19., 20.],
-        [12., 13., 12., 13., 14., 13., 14., 15., 16., 17., 18., 19., 20., 21.],
-        [13., 14., 13., 14., 15., 14., 15., 16., 17., 18., 19., 20., 21., 22.]
-        ]))
-
-    assert_array_equal(
-        get_mtx("Vlagyivosztok", "az óperenciás tengeren túl"),
-array([[0., 1., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11., 12., 13.],
-      [1., 2., 3., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11., 12.],
-      [2., 3., 4., 3., 4., 5., 6., 7., 8., 9., 8., 9., 10., 11.],
-      [3., 4., 5., 4., 5., 6., 7., 8., 9., 10., 9., 10., 11., 12.],
-      [4., 5., 6., 5., 6., 7., 8., 9., 10., 11., 10., 11., 12., 13.],
-      [5., 6., 7., 6., 7., 8., 9., 10., 11., 12., 11., 12., 13., 14.],
-      [6., 7., 8., 7., 8., 9., 10., 11., 12., 13., 12., 13., 14., 15.],
-      [7., 8., 9., 8., 9., 10., 11., 12., 13., 14., 13., 14., 15., 16.],
-      [8., 9., 10., 9., 10., 11., 12., 13., 14., 15., 14., 15., 16., 17.],
-      [9., 10., 11., 10., 11., 12., 13., 14., 15., 16., 15., 16., 17., 18.],
-      [10., 11., 12., 11., 12., 13., 14., 15., 16., 17., 16., 17., 18., 19.],
-      [11., 12., 13., 12., 13., 14., 13., 14., 15., 16., 17., 18., 19., 20.],
-      [12., 13., 14., 13., 14., 15., 14., 15., 16., 17., 18., 19., 20., 21.],
-      [13., 14., 15., 14., 15., 16., 15., 16., 17., 16., 17., 18., 19., 20.],
-      [14., 15., 16., 15., 16., 17., 16., 17., 18., 17., 18., 19., 20., 21.],
-      [15., 16., 17., 16., 17., 18., 17., 18., 19., 18., 19., 18., 19., 20.],
-      [16., 17., 18., 17., 18., 19., 18., 19., 20., 19., 20., 19., 20., 21.],
-      [17., 18., 19., 18., 19., 20., 19., 20., 21., 20., 21., 20., 21., 22.],
-      [18., 19., 20., 19., 18., 19., 20., 21., 22., 21., 22., 21., 22., 23.],
-      [19., 20., 21., 20., 19., 20., 21., 22., 23., 22., 23., 22., 23., 24.],
-      [20., 21., 22., 21., 20., 21., 22., 23., 24., 23., 24., 23., 24., 25.],
-      [21., 22., 23., 22., 21., 22., 23., 24., 25., 24., 25., 24., 25., 26.],
-      [22., 23., 24., 23., 22., 23., 24., 25., 26., 25., 26., 25., 26., 27.],
-      [23., 24., 25., 24., 23., 24., 25., 26., 27., 26., 27., 26., 27., 28.],
-      [24., 25., 26., 25., 24., 25., 26., 27., 28., 27., 28., 27., 28., 29.],
-      [25., 26., 27., 26., 25., 26., 27., 28., 29., 28., 29., 28., 29., 30.],
-      [26., 27., 26., 27., 26., 27., 28., 29., 30., 29., 30., 29., 30., 31.]]))
+    """test if editdistances are calculated correctly"""
 
+    # default weight is 100 per deletion and 49 per insertion
+    # in 80 tests around the world
+    assert edit_distance_with2ops("ajka", "Rajka") == 49
+    assert edit_distance_with2ops("Rajka", "ajka") == 100
+    assert edit_distance_with2ops("Debrecen", "Mosonmagyaróvár") == 1386
+    assert edit_distance_with2ops("Bécs", "Hegyeshalom") == 790
+    assert edit_distance_with2ops("Hegyeshalom", "Mosonmagyaróvár") == 1388
+    assert edit_distance_with2ops("Mosonmagyaróvár", "Győr") == 1398
+    # 4 del + 4 ins = 4*49+4*100
+    assert edit_distance_with2ops("Győr", "Tata") == 596
+    assert edit_distance_with2ops("Tata", "Tatabánya") == 245  # 5 ins: 5*49
+    assert edit_distance_with2ops("Tatabánya", "Budapest") == 994
+    assert edit_distance_with2ops("Budapest", "Komárom") == 1143
+    # 4 ins + 1 del: 4*49+100
+    assert edit_distance_with2ops("Komárom", "Révkomárom") == 296
+    # 4 del + 1 ins: 4*100+49
+    assert edit_distance_with2ops("Révkomárom", "Komárom") == 449
+    assert edit_distance_with2ops("Komárom", "Budapest") == 1092
+    assert edit_distance_with2ops("Budapest", "Debrecen") == 1043
+    assert edit_distance_with2ops("Debrecen", "Beregszász") == 843
+    assert edit_distance_with2ops("Beregszász", "Kiiv") == 1196
+    assert edit_distance_with2ops("Kiiv", "Moszkva") == 594
+    assert edit_distance_with2ops("Moszkva", "Szenpétervár") == 990
+    assert edit_distance_with2ops("Szentpétervár", "Vlagyivosztok") == 1639
+    assert edit_distance_with2ops("Vlagyivosztok", "Tokió") == 1247
+    assert edit_distance_with2ops("Tokió", "New York") == 594
+    assert edit_distance_with2ops("New York", "Bécs") == 996
+
+    # check if custom weights for insertion work. deletion always costs 1.
+    assert edit_distance_with2ops("ajka", "Rajka", w_ins=90) == 90
+    assert edit_distance_with2ops("Rajka", "ajka", w_ins=90) == 100
+    assert edit_distance_with2ops(
+        "Debrecen", "Mosonmagyaróvár", w_ins=90) == 1960
 
-def test_mtx2graph():
-    """Test if matrix of edit distances is correctly transformed to a
-    directed graph object"""
-    # similar to unittest, but 1 patch missing
-    expG = DiGraph()
-    expG.add_weighted_edges_from([((2, 2), (2, 1), 100),
-                                  ((2, 2), (1, 2), 49),
-                                  ((2, 2), (1, 1), 0),
-                                  ((2, 1), (2, 0), 100),
-                                  ((2, 1), (1, 1), 49),
-                                  ((2, 0), (1, 0), 49),
-                                  ((1, 2), (1, 1), 100),
-                                  ((1, 2), (0, 2), 49),
-                                  ((1, 1), (1, 0), 100),
-                                  ((1, 1), (0, 1), 49),
-                                  ((1, 0), (0, 0), 49),
-                                  ((0, 2), (0, 1), 100),
-                                  ((0, 1), (0, 0), 100)])
-    exp = [(e, datadict["weight"]) for e, datadict in expG.edges.items()]
-
-    outtuple = mtx2graph("ló", "hó")
-    out = [(e, datadict["weight"])
-           for e, datadict in outtuple[0].edges.items()]
-
-    # assert expected and actual output is the same
-    assert len(outtuple) == 3
-    assert isinstance(outtuple, tuple)
-    assert set(out) == set(exp)
-    # the height. always 1 longer than the word bc + "#" (#ló)
-    assert outtuple[1] == 3
-    assert outtuple[2] == 3  # the width.
-
-    # set up2: assert weights are passed on correctly
-    expG = DiGraph()
-    expG.add_weighted_edges_from([((2, 2), (2, 1), 11),
-                                  ((2, 2), (1, 2), 7),
-                                  ((2, 2), (1, 1), 0),
-                                  ((2, 1), (2, 0), 11),
-                                  ((2, 1), (1, 1), 7),
-                                  ((2, 0), (1, 0), 7),
-                                  ((1, 2), (1, 1), 11),
-                                  ((1, 2), (0, 2), 7),
-                                  ((1, 1), (1, 0), 11),
-                                  ((1, 1), (0, 1), 7),
-                                  ((1, 0), (0, 0), 7),
-                                  ((0, 2), (0, 1), 11),
-                                  ((0, 1), (0, 0), 11)])
-    exp = [(e, datadict["weight"]) for e, datadict in expG.edges.items()]
-
-    outtuple = mtx2graph("ló", "hó", w_del=11, w_ins=7)
-    out = [(e, datadict["weight"])
-           for e, datadict in outtuple[0].edges.items()]
-
-    # assert expected and actual output is the same
-    assert len(outtuple) == 3
-    assert isinstance(outtuple, tuple)
-    assert set(out) == set(exp)
-    # the height. always 1 longer than the word bc + "#" (#ló)
-    assert outtuple[1] == 3
-    assert outtuple[2] == 3  # the width.
+def test_apply_edit():
+    """test if editoperations are correctly applied to words"""
+    assert apply_edit("ló", ('substitute l by h', 'keep ó')) == ['h', 'ó']
+    assert apply_edit(["l", "ó"],
+                      ('substitute l by h', 'keep ó')) == ['h', 'ó']
+    assert apply_edit(['f', 'ɛ', 'r', 'i', 'h', 'ɛ', 'ɟ'],
+                      ('insert d',
+                       'insert u',
+                       'insert n',
+                       'insert ɒ',
+                       'insert p',
+                       'substitute f by ɒ',
+                       'delete ɛ',
+                       'keep r',
+                       'delete i',
+                       'delete h',
+                       'delete ɛ',
+                       'substitute ɟ by t')
+                      ) == ['d', 'u', 'n', 'ɒ', 'p', 'ɒ', 'r', 't']
+    assert apply_edit(['t͡ʃ',
+                       'ø',
+                       't͡ʃ'],
+                      ("substitute t͡ʃ by f",
+                       "insert r",
+                       "keep ø",
+                       "substitute t͡ʃ by t͡ʃː")) == ['f', 'r', 'ø', 't͡ʃː']
 
+def test_list2regex():
+    """test if list of phonemes is correctly converted to regular expression"""
+    assert list2regex(["b", "k", "v"]) == "(b|k|v)"
+    assert list2regex(["b", "k", "-", "v"]) == "(b|k|v)?"
+    assert list2regex(["b", "k", "-", "v", "mp"]) == "(b|k|v|mp)?"
+    assert list2regex(["b", "k", "-", "v", "mp", "mk"]) == "(b|k|v|mp|mk)?"
+    assert list2regex(["o"]) == '(o)'
+    assert list2regex(["ʃʲk"]) == '(ʃʲk)'
 
 def test_tuples2editops():
-    """Tuples correspond to points in the matrix (directed graph).
-    The list of tuples encodes the edit operations necessary
-    to get from string A to string B. Test if this list of tuples
-    is correctly converted to a human readable format."""
-    assert tuples2editops([(0, 0), (0, 1), (1, 1), (2, 2)],
-                          "ló", "hó") == ['substitute l by h', 'keep ó']
-
+    """assert that edit operations coded as tuples
+    are converted to natural language correctly"""
 
-def test_editops():
-    """test if human-readable edit operations are concluded
-    correctly from two strings"""
-    assert editops("ló", "hó") == [('substitute l by h', 'keep ó')]
-    assert editops("CCV", "CV", howmany_paths=2) == [
-        ('delete C', 'keep C', 'keep V'),
-        ('keep C', 'delete C', 'keep V')]
 
+    # assert list of tuples is correctly converted to list of strings
+    assert tuples2editops([(0, 0), (0, 1), (1, 1), (2, 2)],
+        "ló", "hó") == ['substitute l by h', 'keep ó']
+    assert tuples2editops([(0, 0), (1, 1), (2, 2), (2, 3)],
+        "lóh", "ló") == ['keep l', 'keep ó', 'delete h']
+    assert tuples2editops([(0, 0), (1, 1), (2, 2), (3, 3)],
+        "foo", "foo") == ['keep f', 'keep o', 'keep o']
 
-def test_apply_edit():
-    pass  # unit == integration tests (no patches)
-
+def test_get_mtx():
+    """test if distance matrix between two words is set up correctly"""
 
-def test_get_howmany():
-    pass  # unit == integration tests (no patches)
+    exp = [[0, 1, 2, 3, 4],
+           [1, 2, 3, 4, 5],
+           [2, 3, 2, 3, 4],
+           [3, 4, 3, 2, 3],
+           [4, 5, 4, 3, 2]
+          ]
 
+        # assert
+    assert get_mtx("Bécs", "Pécs") == exp
 
-def test_pick_minmax():
-    pass  # unit == integration tests (no patches)
+    # tear down
+    del exp
 
-    #
+def test_mtx2graph():
+    expected = {(0, 0): {(0, 1): 100, (1, 0): 49},
+                (0, 1): {(0, 2): 100, (1, 1): 49},
+                (0, 2): {(1, 2): 49},
+                (1, 0): {(1, 1): 100, (2, 0): 49},
+                (1, 1): {(1, 2): 100, (2, 1): 49, (2, 2): 0},
+                (1, 2): {(2, 2): 49},
+                (2, 0): {(2, 1): 100},
+                (2, 1): {(2, 2): 100},
+                (2, 2): {}}
+
+    # "ló", "hó"
+    assert mtx2graph([[0, 1, 2], [1, 2, 3], [2, 3, 2]]) == expected
+
+def test_dijkstra():
+    # Test 1: Basic graph with a simple shortest path
+    graph1 = {
+        'A': {'B': 1, 'C': 4},
+        'B': {'C': 2, 'D': 6},
+        'C': {'D': 3},
+        'D': {}
+    }
+    assert dijkstra(graph1, 'A', 'D') == ['A', 'B', 'C', 'D']
+
+    # Test 3: Graph with multiple paths to the destination
+    graph3 = {
+        'A': {'B': 5, 'C': 1},
+        'B': {'D': 2},
+        'C': {'D': 6},
+        'D': {}
+    }
+    assert dijkstra(graph3, 'A', 'D') == ['A', 'C', 'D']
+
+    # Test 6: Graph with disconnected components
+    graph6 = {
+        'A': {'B': 1},
+        'B': {'C': 2},
+        'C': {},
+        'D': {'E': 3},
+        'E': {'F': 4},
+        'F': {}
+    }
+    assert dijkstra(graph6, 'A', 'F') == (None)
+
+def test_add_edge_new_node():
+    graph = {}
+    add_edge(graph, 'A', 'B', 5)
+    assert graph == {'A': {'B': 5}}
+
+
+def test_add_edge_existing_node():
+    graph = {'A': {'B': 3}}
+    add_edge(graph, 'A', 'C', 7)
+    assert graph == {'A': {'B': 3, 'C': 7}}
+
+
+def test_add_edge_overwrite_edge():
+    graph = {'A': {'B': 3}}
+    add_edge(graph, 'A', 'B', 5)
+    assert graph == {'A': {'B': 5}}
+
+
+def test_add_edge_self_loop():
+    graph = {'A': {}}
+    add_edge(graph, 'A', 'A', 4)
+    assert graph == {'A': {'A': 4}}
+
+
+def test_add_edge_negative_weight():
+    graph = {'A': {}}
+    add_edge(graph, 'A', 'B', -2)
+    assert graph == {'A': {'B': -2}}
+
+
+@pytest.mark.parametrize("graph, u, v, weight, expected", [
+    ({}, 'A', 'B', 5, {'A': {'B': 5}}),
+    ({'A': {'B': 3}}, 'A', 'C', 7, {'A': {'B': 3, 'C': 7}}),
+    ({'A': {'B': 3}}, 'A', 'B', 5, {'A': {'B': 5}}),
+    ({'A': {}}, 'A', 'A', 4, {'A': {'A': 4}}),
+    ({'A': {}}, 'A', 'B', -2, {'A': {'B': -2}}),
+])
+def test_add_edge_parametrized(graph, u, v, weight, expected):
+    add_edge(graph, u, v, weight)
+    assert graph == expected
+
+
+def test_substitute_operations_empty():
+    operations = []
+    result = substitute_operations(operations)
+    assert result == []
+
+
+def test_substitute_operations_no_substitution():
+    operations = ['insert A', 'delete B', 'insert C']
+    result = substitute_operations(operations)
+    assert result == ['substitute B by A', 'insert C']
+
+
+def test_substitute_operations_single_substitution():
+    operations = ['delete A', 'insert B']
+    result = substitute_operations(operations)
+    assert result == ['substitute A by B']
+
+
+def test_substitute_operations_multiple_substitutions():
+    operations = ['delete A', 'insert B', 'delete C', 'insert D']
+    result = substitute_operations(operations)
+    assert result == ['substitute A by B', 'substitute C by D']
+
+
+def test_substitute_operations_mixed_operations():
+    operations = ['insert A', 'delete B', 'insert C', 'delete D', 'insert E']
+    result = substitute_operations(operations)
+    assert result == ['substitute B by A', 'substitute D by C', 'insert E']
```

