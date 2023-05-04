# Comparing `tmp/ml_infrastructure-1.7.1.tar.gz` & `tmp/ml_infrastructure-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_infrastructure-1.7.1.tar", last modified: Thu May  4 03:37:32 2023, max compression
+gzip compressed data, was "ml_infrastructure-1.8.1.tar", last modified: Thu May  4 03:41:59 2023, max compression
```

## Comparing `ml_infrastructure-1.7.1.tar` & `ml_infrastructure-1.8.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.998443 ml_infrastructure-1.7.1/
--rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.7.1/LICENSE.rst
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-04 03:37:31.998443 ml_infrastructure-1.7.1/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.7.1/README.rst
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.994444 ml_infrastructure-1.7.1/ml_infrastructure/
--rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.7.1/ml_infrastructure/__init__.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     9631 2023-05-04 03:29:31.000000 ml_infrastructure-1.7.1/ml_infrastructure/app.py
--rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.7.1/ml_infrastructure/data_manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     4843 2023-05-04 03:00:15.000000 ml_infrastructure-1.7.1/ml_infrastructure/evaluator.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.7.1/ml_infrastructure/example.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.7.1/ml_infrastructure/manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3301 2023-04-30 18:13:06.000000 ml_infrastructure-1.7.1/ml_infrastructure/model.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.994444 ml_infrastructure-1.7.1/ml_infrastructure/static/
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.994444 ml_infrastructure-1.7.1/ml_infrastructure/static/js/
--rw-rw-r--   0 maple     (1000) maple     (1000)    86927 2023-05-03 22:18:49.000000 ml_infrastructure-1.7.1/ml_infrastructure/static/js/jquery.min.js
--rw-rw-r--   0 maple     (1000) maple     (1000)  3478174 2023-05-03 22:18:49.000000 ml_infrastructure-1.7.1/ml_infrastructure/static/js/plotly-latest.min.js
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.998443 ml_infrastructure-1.7.1/ml_infrastructure/static/styles/
--rw-rw-r--   0 maple     (1000) maple     (1000)    23409 2023-05-03 22:11:19.000000 ml_infrastructure-1.7.1/ml_infrastructure/static/styles/bootstrap-theme.min.css
--rw-rw-r--   0 maple     (1000) maple     (1000)   121200 2023-05-03 22:11:23.000000 ml_infrastructure-1.7.1/ml_infrastructure/static/styles/bootstrap.min.css
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.998443 ml_infrastructure-1.7.1/ml_infrastructure/templates/
--rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/control.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/eval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1340 2023-05-03 22:31:11.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/header.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/index.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/loss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/stopForm.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/trainingEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/trainingLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/validationEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.7.1/ml_infrastructure/templates/validationLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     2123 2023-04-30 18:36:27.000000 ml_infrastructure-1.7.1/ml_infrastructure/trainer.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:37:31.994444 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-04 03:37:31.000000 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)     1102 2023-05-04 03:37:31.000000 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/SOURCES.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-05-04 03:37:31.000000 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/dependency_links.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-05-04 03:37:31.000000 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/requires.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-05-04 03:37:31.000000 ml_infrastructure-1.7.1/ml_infrastructure.egg-info/top_level.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-05-04 03:37:31.998443 ml_infrastructure-1.7.1/setup.cfg
--rw-rw-r--   0 maple     (1000) maple     (1000)     1053 2023-05-03 22:44:38.000000 ml_infrastructure-1.7.1/setup.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.8.1/LICENSE.rst
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.8.1/README.rst
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.048582 ml_infrastructure-1.8.1/ml_infrastructure/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.8.1/ml_infrastructure/__init__.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     9430 2023-05-04 03:41:16.000000 ml_infrastructure-1.8.1/ml_infrastructure/app.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.8.1/ml_infrastructure/data_manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     4843 2023-05-04 03:00:15.000000 ml_infrastructure-1.8.1/ml_infrastructure/evaluator.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.8.1/ml_infrastructure/example.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.8.1/ml_infrastructure/manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3301 2023-04-30 18:13:06.000000 ml_infrastructure-1.8.1/ml_infrastructure/model.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.048582 ml_infrastructure-1.8.1/ml_infrastructure/static/
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/ml_infrastructure/static/js/
+-rw-rw-r--   0 maple     (1000) maple     (1000)    86927 2023-05-03 22:18:49.000000 ml_infrastructure-1.8.1/ml_infrastructure/static/js/jquery.min.js
+-rw-rw-r--   0 maple     (1000) maple     (1000)  3478174 2023-05-03 22:18:49.000000 ml_infrastructure-1.8.1/ml_infrastructure/static/js/plotly-latest.min.js
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/ml_infrastructure/static/styles/
+-rw-rw-r--   0 maple     (1000) maple     (1000)    23409 2023-05-03 22:11:19.000000 ml_infrastructure-1.8.1/ml_infrastructure/static/styles/bootstrap-theme.min.css
+-rw-rw-r--   0 maple     (1000) maple     (1000)   121200 2023-05-03 22:11:23.000000 ml_infrastructure-1.8.1/ml_infrastructure/static/styles/bootstrap.min.css
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/ml_infrastructure/templates/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/control.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/eval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1340 2023-05-03 22:31:11.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/header.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/index.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/loss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/stopForm.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/trainingEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/trainingLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/validationEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.8.1/ml_infrastructure/templates/validationLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     2123 2023-04-30 18:36:27.000000 ml_infrastructure-1.8.1/ml_infrastructure/trainer.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-04 03:41:59.048582 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-04 03:41:59.000000 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1102 2023-05-04 03:41:59.000000 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/SOURCES.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-05-04 03:41:59.000000 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/dependency_links.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-05-04 03:41:59.000000 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/requires.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-05-04 03:41:59.000000 ml_infrastructure-1.8.1/ml_infrastructure.egg-info/top_level.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-05-04 03:41:59.052582 ml_infrastructure-1.8.1/setup.cfg
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1053 2023-05-04 03:41:37.000000 ml_infrastructure-1.8.1/setup.py
```

### Comparing `ml_infrastructure-1.7.1/LICENSE.rst` & `ml_infrastructure-1.8.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/PKG-INFO` & `ml_infrastructure-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_infrastructure
-Version: 1.7.1
+Version: 1.8.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/app.py` & `ml_infrastructure-1.8.1/ml_infrastructure/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,20 +225,14 @@
     }
     return json.dumps(loss_graph, cls=plotly.utils.PlotlyJSONEncoder)
 
 
 def get_eval_table(mode):
     global performance
     global idx
-    with open("data.json", "w") as fout:
-        json.dump(performance, fout)
-
-    with open("data_metrics.json", "w") as fout:
-        json.dump(get_evaluation_metrics(performance, mode, idx), fout)
-
     keys = ['Name', 'Accuracy', 'Classification Error', 'Precision', 'Recall', 'Specificity', 'F1-Score', 'TP', 'FP',
             'TN', 'FN']
     table = Figure([Table(
         header=dict(
             values=keys,
             font=dict(size=12),
             align="left"
```

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/evaluator.py` & `ml_infrastructure-1.8.1/ml_infrastructure/evaluator.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/example.py` & `ml_infrastructure-1.8.1/ml_infrastructure/example.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/manager.py` & `ml_infrastructure-1.8.1/ml_infrastructure/manager.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/model.py` & `ml_infrastructure-1.8.1/ml_infrastructure/model.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/static/js/jquery.min.js` & `ml_infrastructure-1.8.1/ml_infrastructure/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/static/js/plotly-latest.min.js` & `ml_infrastructure-1.8.1/ml_infrastructure/static/js/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/static/styles/bootstrap-theme.min.css` & `ml_infrastructure-1.8.1/ml_infrastructure/static/styles/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/static/styles/bootstrap.min.css` & `ml_infrastructure-1.8.1/ml_infrastructure/static/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/templates/header.html` & `ml_infrastructure-1.8.1/ml_infrastructure/templates/header.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/templates/stopForm.html` & `ml_infrastructure-1.8.1/ml_infrastructure/templates/stopForm.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure/trainer.py` & `ml_infrastructure-1.8.1/ml_infrastructure/trainer.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure.egg-info/PKG-INFO` & `ml_infrastructure-1.8.1/ml_infrastructure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-infrastructure
-Version: 1.7.1
+Version: 1.8.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.7.1/ml_infrastructure.egg-info/SOURCES.txt` & `ml_infrastructure-1.8.1/ml_infrastructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.7.1/setup.py` & `ml_infrastructure-1.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '1.7.1'
+VERSION = '1.8.1'
 DESCRIPTION = 'Software infrastructure to for machine learning'
 LONG_DESCRIPTION = 'Software infrastructure for machine learning projects that makes it easier to manage experiments and log progress'
 
 setup(
     name="ml_infrastructure",
     version=VERSION,
     description=DESCRIPTION,
```

