# Comparing `tmp/werpy-0.0.3.tar.gz` & `tmp/werpy-0.0.4.tar.gz`

## Comparing `werpy-0.0.3.tar` & `werpy-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 werpy-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
--rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/assets/images/werpy-logo-word-error-rate.png
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/workflows/codacy.yml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 werpy-0.0.3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSES/PANDAS_LICENSE
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/__init__.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/metrics.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/normalize.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/summary.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/wer.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/werp.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/werps.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 werpy-0.0.3/werpy/wers.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 werpy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.3/LICENSE
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 werpy-0.0.3/README.md
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 werpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 werpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 werpy-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 werpy-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 werpy-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 werpy-0.0.4/SECURITY.md
+-rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.4/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
+-rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.4/.github/assets/images/werpy-logo-word-error-rate.png
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 werpy-0.0.4/.github/workflows/codacy.yml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 werpy-0.0.4/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 werpy-0.0.4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.4/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.4/LICENSES/PANDAS_LICENSE
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/errorhandler.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/metrics.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/normalize.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/summary.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/wer.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/werp.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/werps.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 werpy-0.0.4/werpy/wers.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 werpy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 werpy-0.0.4/README.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 werpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 werpy-0.0.4/PKG-INFO
```

### Comparing `werpy-0.0.3/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png` & `werpy-0.0.4/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/.github/assets/images/werpy-logo-word-error-rate.png` & `werpy-0.0.4/.github/assets/images/werpy-logo-word-error-rate.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/.github/workflows/codacy.yml` & `werpy-0.0.4/.github/workflows/codacy.yml`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/.github/workflows/codeql.yml` & `werpy-0.0.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/LICENSES/NUMPY_LICENSE` & `werpy-0.0.4/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/LICENSES/PANDAS_LICENSE` & `werpy-0.0.4/LICENSES/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/werpy/metrics.py` & `werpy-0.0.4/werpy/metrics.py`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/werpy/normalize.py` & `werpy-0.0.4/werpy/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,18 @@
     TypeError
         if any input data is has an int, float or complex data type.
     AttributeError
         if input text is not a str, list or np.ndarray data type.
     """
     try:
         vectorize_instantiate_normalize_class = np.vectorize(instantiate_normalize_class)
-        return vectorize_instantiate_normalize_class(text).tolist()
     except TypeError as err:
         print("TypeError:", err,
               "\nAll text should be in a str(string) format. "
               "Please check your input does not include any Numeric Data Types such as int, float or complex.")
+        return None
     except AttributeError:
         print(
             "AttributeError: "
             "The normalization method cannot be executed if data input is not a String, List or Numpy Array")
+        return None
+    return vectorize_instantiate_normalize_class(text).tolist()
```

### Comparing `werpy-0.0.3/werpy/summary.py` & `werpy-0.0.4/werpy/summary.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DataFrame.
 
 This module defines the following function:
     - summary(reference, hypothesis)
 """
 
 import pandas as pd
-from .metrics import metrics
+from .errorhandler import error_handler
 
 
 def summary(reference, hypothesis):
     """
     This function provides a comprehensive breakdown of the calculated results including the WER, Levenshtein 
     Distance and all the insertion, deletion and substitution errors.
 
@@ -41,22 +41,19 @@
             substitutions - count of words needing to be transformed so the hypothesis matches the reference
             inserted_words - list of inserted words
             deleted_words - list of deleted words
             substituted_words - list of substitutions. Each substitution will be shown as a tuple with the reference
             word and the hypothesis word. For example: [(cited, sighted), (abnormally, normally)]
     """
     try:
-        word_error_rate_breakdown = metrics(reference, hypothesis)
-    except ValueError:
-        print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
-    except AttributeError:
-        print("AttributeError: All text should be in a string format. Please check your input does not include any "
-              "Numeric data types.")
+        word_error_rate_breakdown = error_handler(reference, hypothesis)
+    except (ValueError, AttributeError) as err:
+        print(f"{type(err).__name__}: {str(err)}")
+        return None
+    if word_error_rate_breakdown[0].size == 1:
+        word_error_rate_breakdown = [word_error_rate_breakdown.tolist()]
     else:
-        if word_error_rate_breakdown[0].size == 1:
-            word_error_rate_breakdown = [word_error_rate_breakdown.tolist()]
-        else:
-            word_error_rate_breakdown = word_error_rate_breakdown.tolist()
-        columns = ['wer', 'ld', 'm', 'insertions', 'deletions', 'substitutions', 'inserted_words', 'deleted_words',
+        word_error_rate_breakdown = word_error_rate_breakdown.tolist()
+    columns = ['wer', 'ld', 'm', 'insertions', 'deletions', 'substitutions', 'inserted_words', 'deleted_words',
                    'substituted_words']
-        df = pd.DataFrame(word_error_rate_breakdown, columns=columns)
-        return df
+    df = pd.DataFrame(word_error_rate_breakdown, columns=columns)
+    return df
```

### Comparing `werpy-0.0.3/werpy/wer.py` & `werpy-0.0.4/werpy/wer.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 the hypothesis text into the reference text, divided by the number of words in the reference text.
 
 This module defines the following function:
     - wer(reference, hypothesis): Calculate the WER between a reference text and a hypothesis text.
 """
 
 import numpy as np
-from .metrics import metrics
+from .errorhandler import error_handler
 
 
 def wer(reference, hypothesis) -> float:
     """
     This function will calculate the overall Word Error Rate for the entire reference and hypothesis texts.
 
     Parameters
@@ -44,21 +44,18 @@
     >>> ref = ['i love cold pizza','the sugar bear character was popular']
     >>> hyp = ['i love pizza','the sugar bare character was popular']
     >>> wer_example_2 = wer(ref, hyp)
     >>> print(wer_example_2)
     0.2
     """
     try:
-        word_error_rate_breakdown = metrics(reference, hypothesis)
-    except ValueError:
-        print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
-    except AttributeError:
-        print("AttributeError: All text should be in a string format. Please check your input does not include any "
-              "Numeric data types.")
-    else:
-        if isinstance(word_error_rate_breakdown[0], np.ndarray):
-            transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
-            wer_result = (np.sum(transform_word_error_rate_breakdown[1])) / (np.sum(transform_word_error_rate_breakdown[
+        word_error_rate_breakdown = error_handler(reference, hypothesis)
+    except (ValueError, AttributeError) as err:
+        print(f"{type(err).__name__}: {str(err)}")
+        return None
+    if isinstance(word_error_rate_breakdown[0], np.ndarray):
+        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        wer_result = (np.sum(transform_word_error_rate_breakdown[1])) / (np.sum(transform_word_error_rate_breakdown[
                                                                                      2]))
-        else:
-            wer_result = word_error_rate_breakdown[0]
-        return wer_result
+    else:
+        wer_result = word_error_rate_breakdown[0]
+    return wer_result
```

### Comparing `werpy-0.0.3/werpy/werp.py` & `werpy-0.0.4/werpy/werp.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
 
 This module defines the following function:
     - werp(reference, hypothesis)
 """
 
 import numpy as np
-from .metrics import metrics
+from .errorhandler import error_handler
 
 
 def werp(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a weighted Word Error Rate for the entire reference and hypothesis texts. It allows the
     insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
@@ -58,30 +58,25 @@
     0.25
 
     >>> werp_example_4 = werp(ref, hyp, 0.5, 0.5, 1)
     >>> print(werp_example_4)
     0.25
     """
     try:
-        word_error_rate_breakdown = metrics(reference, hypothesis)
-    except ValueError:
-        print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
-    except AttributeError:
-        print(
-            "AttributeError: All text should be in a string format. Please check your input does not include any "
-            "Numeric data types.")
+        word_error_rate_breakdown = error_handler(reference, hypothesis)
+    except (ValueError, AttributeError) as err:
+        print(f"{type(err).__name__}: {str(err)}")
+        return None
+    if isinstance(word_error_rate_breakdown[0], np.ndarray):
+        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
+        weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
+        weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
+        m = np.sum(transform_word_error_rate_breakdown[2])
     else:
-        if isinstance(word_error_rate_breakdown[0], np.ndarray):
-            transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
-            weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
-            weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
-            weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
-            m = np.sum(transform_word_error_rate_breakdown[2])
-        else:
-            weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
-            weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
-            weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
-            m = np.sum(word_error_rate_breakdown[2])
-
-        weighted_errors = np.sum([weighted_insertions, weighted_deletions, weighted_substitutions])
-        werp_result = weighted_errors / m
-        return werp_result
+        weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
+        weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
+        weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
+        m = np.sum(word_error_rate_breakdown[2])
+    weighted_errors = np.sum([weighted_insertions, weighted_deletions, weighted_substitutions])
+    werp_result = weighted_errors / m
+    return werp_result
```

### Comparing `werpy-0.0.3/werpy/werps.py` & `werpy-0.0.4/werpy/werps.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 hypothesis texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
 
 This module defines the following function:
     - werps(reference, hypothesis)
 """
 
 import numpy as np
-from .metrics import metrics
+from .errorhandler import error_handler
 
 
 def werps(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. It
     allows the insertion, deletion and substitution errors to be penalized or weighted at different rates.
 
@@ -52,34 +52,30 @@
     [0.2857142857142857, 0.3333333333333333]
 
     >>> werps_example_2 = werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
     >>> print(werps_example_2)
     [0.21428571428571427, 0.2777777777777778]
     """
     try:
-        word_error_rate_breakdown = metrics(reference, hypothesis)
-    except ValueError:
-        print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
-    except AttributeError:
-        print(
-            "AttributeError: All text should be in a string format. Please check your input does not include any "
-            "Numeric data types.")
+        word_error_rate_breakdown = error_handler(reference, hypothesis)
+    except (ValueError, AttributeError) as err:
+        print(f"{type(err).__name__}: {str(err)}")
+        return None
+    if isinstance(word_error_rate_breakdown[0], np.ndarray):
+        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
+        weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
+        weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
+        m = transform_word_error_rate_breakdown[2]
     else:
-        if isinstance(word_error_rate_breakdown[0], np.ndarray):
-            transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
-            weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
-            weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
-            weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
-            m = transform_word_error_rate_breakdown[2]
-        else:
-            weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
-            weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
-            weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
-            m = word_error_rate_breakdown[2]
-
-        weighted_errors = sum((weighted_insertions, weighted_deletions, weighted_substitutions))
-        werps_result = weighted_errors / m
-
-        if word_error_rate_breakdown[0].size == 1:
-            return werps_result
-        else:
-            return werps_result.tolist()
+        weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
+        weighted_deletions = word_error_rate_breakdown[4] * deletions_weight
+        weighted_substitutions = word_error_rate_breakdown[5] * substitutions_weight
+        m = word_error_rate_breakdown[2]
+
+    weighted_errors = sum((weighted_insertions, weighted_deletions, weighted_substitutions))
+    werps_result = weighted_errors / m
+
+    if word_error_rate_breakdown[0].size == 1:
+        return werps_result
+
+    return werps_result.tolist()
```

### Comparing `werpy-0.0.3/werpy/wers.py` & `werpy-0.0.4/werpy/wers.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 This module provides a function for calculating a list of the Word Error Rates for each of the reference and
 hypothesis texts.
 
 This module defines the following function:
     - wers(reference, hypothesis)
 """
 
-
 import numpy as np
-from .metrics import metrics
+from .errorhandler import error_handler
 
 
 def wers(reference, hypothesis):
     """
     This function calculates a list of the Word Error Rates for each of the reference and hypothesis texts.
 
     Parameters
@@ -39,22 +38,18 @@
     --------
     >>> ref = ['no one else could claim that','she cited multiple reasons why']
     >>> hyp = ['no one else could claim that','she sighted multiple reasons why']
     >>> wers_example_1 = wers(ref, hyp)
     >>> print(wers_example_1)
     [0.0, 0.2]
     """
-
     try:
-        word_error_rate_breakdown = metrics(reference, hypothesis)
-    except ValueError:
-        print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
-    except AttributeError:
-        print("AttributeError: All text should be in a string format. Please check your input does not include any "
-              "Numeric data types.")
+        word_error_rate_breakdown = error_handler(reference, hypothesis)
+    except (ValueError, AttributeError) as err:
+        print(f"{type(err).__name__}: {str(err)}")
+        return None
+    if isinstance(word_error_rate_breakdown[0], np.ndarray):
+        transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
+        wers_result = transform_word_error_rate_breakdown[0].tolist()
     else:
-        if isinstance(word_error_rate_breakdown[0], np.ndarray):
-            transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
-            wers_result = transform_word_error_rate_breakdown[0].tolist()
-        else:
-            wers_result = word_error_rate_breakdown[0].tolist()
-        return wers_result
+        wers_result = word_error_rate_breakdown[0].tolist()
+    return wers_result
```

### Comparing `werpy-0.0.3/.gitignore` & `werpy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/LICENSE` & `werpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.3/README.md` & `werpy-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
-# werpy (Word Error Rate for Python)
+# werpy - Word Error Rate for Python
 <!-- badges: start -->
 [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp;
 [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;
 ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;
 [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp;
 [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp;
+[![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp;
 <!-- badges: end -->
 
 ## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
 It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
```

### Comparing `werpy-0.0.3/pyproject.toml` & `werpy-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "werpy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ross Armstrong", email="ross.armstrong@analyticsinmotion.com" },
 ]
 description = "A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER)."
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
+    "Development Status :: 5 - Production/Stable"
 ]
 
 keywords = [
     "wer",
     "word error rate",
     "python",
     "python package",
     "stt",
-    "speech to text",
+    "speech-to-text",
     "levenshtein distance",
-    "nlp"
+    "nlp",
+    "metrics"
 ]
 
 dependencies = [
   "numpy>=1.21.6; python_version<'3.11'",
   "numpy>=1.23.2; python_version>='3.11'",
   "pandas>=1.3.0"
 ]
```

### Comparing `werpy-0.0.3/PKG-INFO` & `werpy-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: werpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER).
 Project-URL: Homepage, https://github.com/analyticsinmotion/werpy
 Project-URL: Bug Tracker, https://github.com/analyticsinmotion/werpy/issues
 Author-email: Ross Armstrong <ross.armstrong@analyticsinmotion.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
-Keywords: levenshtein distance,nlp,python,python package,speech to text,stt,wer,word error rate
+Keywords: levenshtein distance,metrics,nlp,python,python package,speech-to-text,stt,wer,word error rate
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.21.6; python_version < '3.11'
 Requires-Dist: numpy>=1.23.2; python_version >= '3.11'
 Requires-Dist: pandas>=1.3.0
 Description-Content-Type: text/markdown
 
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
-# werpy (Word Error Rate for Python)
+# werpy - Word Error Rate for Python
 <!-- badges: start -->
 [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp;
 [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;
 ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;
 [![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp;
 [![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp;
+[![Pylint](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/pylint.yml)&nbsp;&nbsp;
 <!-- badges: end -->
 
 ## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
 It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
```

