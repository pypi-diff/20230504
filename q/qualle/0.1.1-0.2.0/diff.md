# Comparing `tmp/qualle-0.1.1.tar.gz` & `tmp/qualle-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualle-0.1.1.tar", last modified: Thu Dec  8 11:24:31 2022, max compression
+gzip compressed data, was "qualle-0.2.0.tar", max compression
```

## Comparing `qualle-0.1.1.tar` & `qualle-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,33 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.314739 qualle-0.1.1/
--rw-rw-r--   0 bart      (1000) bart      (1000)    11358 2022-12-08 09:13:20.000000 qualle-0.1.1/LICENSE
--rw-rw-r--   0 bart      (1000) bart      (1000)     5255 2022-12-08 11:24:31.314739 qualle-0.1.1/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)     4654 2022-12-08 09:13:37.000000 qualle-0.1.1/README.md
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.306739 qualle-0.1.1/qualle/
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1742 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/evaluate.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.310739 qualle-0.1.1/qualle/features/
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      854 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/base.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1543 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/combined.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1205 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/confidence.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.310739 qualle-0.1.1/qualle/features/label_calibration/
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/label_calibration/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      971 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/label_calibration/base.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1978 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/label_calibration/simple_label_calibration.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7289 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/label_calibration/thesauri_label_calibration.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1140 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/features/text.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.314739 qualle-0.1.1/qualle/interface/
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/interface/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     9846 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/interface/cli.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1844 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/interface/config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5833 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/interface/internal.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2898 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/interface/rest.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.314739 qualle-0.1.1/qualle/label_calibration/
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/label_calibration/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2336 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/label_calibration/category.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1399 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/label_calibration/simple.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      726 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/main.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1162 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/models.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5234 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/pipeline.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1440 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/quality_estimation.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3038 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/train.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4263 2022-12-08 09:13:20.000000 qualle-0.1.1/qualle/utils.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-12-08 11:24:31.310739 qualle-0.1.1/qualle.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)     5255 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)      949 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       63 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/entry_points.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      135 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        7 2022-12-08 11:24:31.000000 qualle-0.1.1/qualle.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2022-12-08 11:24:31.314739 qualle-0.1.1/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)     6088 2022-12-08 11:24:12.000000 qualle-0.1.1/setup.py
+-rw-r--r--   0        0        0    11358 2023-05-04 10:19:34.216655 qualle-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7710 2023-05-04 10:19:34.216655 qualle-0.2.0/README.md
+-rw-r--r--   0        0        0      905 2023-05-04 10:19:49.204784 qualle-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      627 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/evaluate.py
+-rw-r--r--   0        0        0      627 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/__init__.py
+-rw-r--r--   0        0        0      853 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/base.py
+-rw-r--r--   0        0        0     1544 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/combined.py
+-rw-r--r--   0        0        0     1205 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/confidence.py
+-rw-r--r--   0        0        0      627 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/label_calibration/__init__.py
+-rw-r--r--   0        0        0      970 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/label_calibration/base.py
+-rw-r--r--   0        0        0     1976 2023-05-04 10:19:34.216655 qualle-0.2.0/qualle/features/label_calibration/simple_label_calibration.py
+-rw-r--r--   0        0        0     7127 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/features/label_calibration/thesauri_label_calibration.py
+-rw-r--r--   0        0        0     1677 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/features/text/__init__.py
+-rw-r--r--   0        0        0     2258 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/features/text/count.py
+-rw-r--r--   0        0        0      627 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/__init__.py
+-rw-r--r--   0        0        0    11330 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/cli.py
+-rw-r--r--   0        0        0     2522 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/config.py
+-rw-r--r--   0        0        0      636 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/data/__init__.py
+-rw-r--r--   0        0        0     4529 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/data/annif.py
+-rw-r--r--   0        0        0     2432 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/data/tsv.py
+-rw-r--r--   0        0        0     8197 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/internal.py
+-rw-r--r--   0        0        0     2868 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/interface/rest.py
+-rw-r--r--   0        0        0      627 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/label_calibration/__init__.py
+-rw-r--r--   0        0        0     2294 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/label_calibration/category.py
+-rw-r--r--   0        0        0     1388 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/label_calibration/simple.py
+-rw-r--r--   0        0        0      726 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/main.py
+-rw-r--r--   0        0        0     1962 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/models.py
+-rw-r--r--   0        0        0     5046 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/pipeline.py
+-rw-r--r--   0        0        0     1386 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/quality_estimation.py
+-rw-r--r--   0        0        0     2969 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/train.py
+-rw-r--r--   0        0        0     1366 2023-05-04 10:19:34.220655 qualle-0.2.0/qualle/utils.py
+-rw-r--r--   0        0        0     8677 1970-01-01 00:00:00.000000 qualle-0.2.0/PKG-INFO
```

### Comparing `qualle-0.1.1/LICENSE` & `qualle-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualle-0.1.1/PKG-INFO` & `qualle-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,163 @@
-Metadata-Version: 2.1
-Name: qualle
-Version: 0.1.1
-Summary: A framework to predict the quality of a multi-label classification result
-Home-page: https://github.com/zbw/qualle
-Author: AutoSE
-Author-email: autose@zbw.eu
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8,<3.10
-License-File: LICENSE
-
 # Qualle
-![CI](https://github.com/zbw/qualle/actions/workflows/main.yml/badge.svg)
+[![Extended Tests](https://github.com/zbw/qualle/actions/workflows/extended.yml/badge.svg)](https://github.com/zbw/qualle/actions/workflows/extended.yml)
 [![codecov](https://codecov.io/gh/zbw/qualle/branch/master/graph/badge.svg?token=ZE7OWKA83Q)](https://codecov.io/gh/zbw/qualle)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is an implementation of the Qualle framework as proposed in the paper
 [1] and accompanying source code.
 
 The framework allows to train a model which can be used to predict
-the quality of the result of applying a multi-label classification (MLC) 
+the quality of the result of applying a multi-label classification (MLC)
 method on a document. In this implementation, only the
-[recall](https://en.wikipedia.org/wiki/Precision_and_recall) 
+[recall](https://en.wikipedia.org/wiki/Precision_and_recall)
 is predicted for a document, but in principle
-any document-level quality estimation (such as the prediction of precision) 
+any document-level quality estimation (such as the prediction of precision)
 can be implemented analogously.
 
 Qualle provides a command-line interface to train
 and evaluate models. In addition, a REST webservice for predicting
 the recall of a MLC result is provided.
 
-### Command line interface (CLI)
-In order to run the CLI, you must install the packages from the Pipfile.
-The interface is then accessible from the module ``qualle.main``. To
-see the help message, run (inside the Qualle directory)
 
-``python -m qualle.main -h``
+## Requirements
 
+Python ``>= 3.8`` is required.
 
-### Train
-In order to train a model you have to provide a training data file.
-This file has to be a tabular-separated file (tsv) in the format (tabular is marked with ``\t``)
+## Installation
+
+Choose one of these installation methods:
+
+### With pip
+Qualle is available on [PyPI](https://pypi.org/) . You can install Qualle using pip:
+
+``pip install qualle``
+
+This will install a command line tool called `qualle` . You can call `qualle -h` to see the help message which will
+display the available modes and options.
+
+Note that it is generally recommended to use a [virtual environment](https://docs.python.org/3/tutorial/venv.html) to avoid
+ conflicting behaviour with the system package manager.
+
+### From source
+You also have the option to checkout the repository and install the packages from source. You need
+[poetry](https://python-poetry.org) to perform the task:
+
+```shell
+# call inside the project directory
+poetry install --without ci
+```
+
+### Docker
+You can also use a Docker Image from the [Container Registry of Github](https://github.com/zbw/qualle/pkgs/container/qualle):
+
+``docker pull ghcr.io/zbw/qualle``
+
+Alternatively, you can use the Dockerfile included in this project to build a Docker image yourself. E.g.:
+
+ ``docker build -t qualle .``
+
+By default, a container built from this image launches a REST interface listening on ``0.0.0.0:8000``
+
+You need to pass the model file (see below the section REST interface) per bind mount or volume to the docker container.
+Beyond that, you need to specify the location of the model file with an
+environment variable named `MODEL_FILE`:
+
+``docker run --rm -it --env MODEL_FILE=/model -v /path/to/model:/model -p 8000:8000 ghcr.io/zbw/qualle``
+
+[Gunicorn](https://gunicorn.org/) is used as HTTP Server. You can use the environment variable ``GUNICORN_CMD_ARGS`` to customize
+Gunicorn settings, such as the number of worker processes to use:
+
+``docker run --rm -it --env MODEL_FILE=/model --env GUNICORN_CMD_ARGS="--workers 4" -v /path/to/model:/model -p 8000:8000 ghcr.io/zbw/qualle``
+
+You can also use the Docker image to train or evaluate by using the Qualle command line tool:
+
+```shell
+docker run --rm -it -v \
+ /path/to/train_data_file:/train_data_file /path/to/model:/model ghcr.io/zbw/qualle \
+ qualle train /train_data_file /model
+ ```
+
+The Qualle command line tool is not available for the release 0.1.0 and 0.1.1. For these releases,
+you need to call the python module ``qualle.main`` instead:
+
+```shell
+docker run --rm -it -v \
+ /path/to/train_data_file:/train_data_file /path/to/model:/model ghcr.io/zbw/qualle:0.1.1 \
+ python -m qualle.main train /train_data_file /model
+```
+
+## Usage
+
+### Input data 
+In order to train a model, evaluate a model or predict the quality of an MLC result
+you have to provide data.
+
+This can be a tabular-separated file (tsv) in the format (tabular is marked with ``\t``)
 
 ```document-content\tpredicted_labels_with_scores\ttrue_labels```
 
 where
 - ``document-content`` is a string describing the content of the document
 (more precisely: the string on which the MLC method is trained), e.g. the title
 - ``predicted_labels_with_scores`` is a comma-separated list of pairs ``predicted_label:confidence-score``
 (this is basically the output of the MLC method)
 - ``true_labels`` is a comma-separated list of true labels (ground truth)
 
+Note that you can omit the ``true_labels`` section if you only want to predict the 
+quality of the MLC result.
+
 For example, a row in the data file could look like this:
 
 ``Optimal investment policy of the regulated firm\tConcept0:0.5,Concept1:1\tConcept0,Concept3``
 
-To train a model, use the ``main`` module inside ``qualle``, e.g.:
+For those who use an MLC method via the toolkit [Annif](https://github.com/NatLibFi/annif) for automated subject indexing:
+You can alternatively specify a
+[full-text document corpus](https://github.com/NatLibFi/Annif/wiki/Document-corpus-formats/70a8f079313e872ed513a4bff1747c604b5781a7)
+ combined with the result of the Annif index method (tested with Annif version 0.59) applied on the corpus.
+This is a  folder with three files per document:
+
+* ``doc.annif`` : result of Annif index method
+* ``doc.tsv`` : ground truth
+* ``doc.txt`` : document content
+
+As above, you may omit the ``doc.tsv`` if you just want to
+predict the quality of the MLC result.
 
-``python -m qualle.main train /path/to/train_data_file /path/to/output/model``
+### Train
+To train a model, use the ``train`` mode, e.g.:
+
+``qualle train /path/to/train_data_file /path/to/output/model``
 
-It is also possible to use label calibration using the subthesauri of a thesaurus (such as the [STW](http://zbw.eu/stw/version/latest/about))
+It is also possible to use label calibration (comparison of predicted vs actual labels) using the subthesauri of a thesaurus (such as the [STW](http://zbw.eu/stw/version/latest/about))
 as categories (please read the paper for more explanations). Consult the help (see above) for the required options.
 
 ### Evaluate
-You must provide a test data file and the path to a trained model in order to evaluate that model.
-The test data file has the same format as the training data file. Metrics
+You must provide test data and the path to a trained model in order to evaluate that model. Metrics
 such as the [explained variation](https://en.wikipedia.org/wiki/Explained_variation) are printed out, describing the quality
 of the recall prediction (please consult the paper for more information).
 
 ### REST interface
-To perform the prediction on a MLC result, a REST interface can be started. 
+To perform the prediction on a MLC result, a REST interface can be started.
 [uvicorn](https://www.uvicorn.org/) is used as HTTP server. You can also use any
 ASGI server implementation and create the ASGI app directly with the method
 ``qualle.interface.rest.create_app``. You need to provide the environment variable
 MODEL_FILE with the path to the model (see ``qualle.interface.config.RESTSettings``).
 
 The REST endpoint expects a HTTP POST with the result of a MLC for a list of documents
 as body. The format is JSON as specified in ``qualle/openapi.json``. You can also use
 the Swagger UI accessible at ``http://address_of_server/docs`` to play around a bit.
 
-### Deployment with Docker
-You can use the Dockerfile included in this project to build a Docker image. E.g.:
-
- ``docker build -t qualle .``
 
-Per default, gunicorn is used to run the REST interface on ``0.0.0.0:8000``
-You need to pass the required settings per environment variable. E.g.:
+## Contribute
 
-``docker run --rm -it --env model_file=/model -v /path/to/model:/model -p 8000:8000 qualle``
+Contributions via pull requests are welcome. Please create an issue beforehand
+to explain and discuss the reasons for the respective contribution.
 
-Of course you can also use the Docker image to train or evaluate by using a 
-different command as input to [docker run](https://docs.docker.com/engine/reference/run/#general-form).
+qualle code should follow the [Black style](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html).
+The Black tool is included as a development dependency; you can run `black .` in the project root to autoformat code.
 
 ## References
 [1] [Toepfer, Martin, and Christin Seifert. "Content-based quality estimation for automatic subject indexing of short texts under precision and recall constraints." International Conference on Theory and Practice of Digital Libraries. Springer, Cham, 2018., DOI 10.1007/978-3-030-00066-0_1](https://arxiv.org/abs/1806.02743)
 
 ## Context information
 This code was created as part of the subject indexing automatization effort at [ZBW - Leibniz Information Centre for Economics](https://www.zbw.eu/en/). See [our homepage](https://www.zbw.eu/en/about-us/key-activities/automated-subject-indexing) for more information, publications, and contact details.
```

### Comparing `qualle-0.1.1/qualle/__init__.py` & `qualle-0.2.0/qualle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/evaluate.py` & `qualle-0.2.0/qualle/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,32 +18,28 @@
 
 from qualle.models import TrainData
 from qualle.pipeline import QualityEstimationPipeline
 from qualle.utils import recall
 
 
 class Evaluator:
-
     def __init__(self, test_data: TrainData, qe_p: QualityEstimationPipeline):
         self._test_data = test_data
         self._qe_p = qe_p
 
     def evaluate(self) -> Dict:
         predict_data = self._test_data.predict_data
         pred_recall = self._qe_p.predict(predict_data)
-        true_recall = recall(self._test_data.true_labels,
-                             predict_data.predicted_labels)
+        true_recall = recall(self._test_data.true_labels, predict_data.predicted_labels)
 
         return scores(true_recall, pred_recall)
 
 
 def scores(true_recall: List[float], pred_recall: List[float]) -> Dict:
     scores = dict()
-    scores['explained_variance_score'] = explained_variance_score(
+    scores["explained_variance_score"] = explained_variance_score(
         true_recall, pred_recall
     )
-    scores['mean_squared_error'] = mean_squared_error(
-        true_recall, pred_recall)
+    scores["mean_squared_error"] = mean_squared_error(true_recall, pred_recall)
 
-    scores['correlation_coefficient'] = np.corrcoef(true_recall, pred_recall)[
-        0, 1]
+    scores["correlation_coefficient"] = np.corrcoef(true_recall, pred_recall)[0, 1]
     return scores
```

### Comparing `qualle-0.1.1/qualle/features/__init__.py` & `qualle-0.2.0/qualle/features/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/features/base.py` & `qualle-0.2.0/qualle/features/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,13 +12,12 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from sklearn.base import BaseEstimator, TransformerMixin
 
 
 class Features(BaseEstimator, TransformerMixin):
-
     def fit(self, X=None, y=None):
         return self
 
     def transform(self, X):
         pass  # pragma: no cover
```

### Comparing `qualle-0.1.1/qualle/features/combined.py` & `qualle-0.2.0/qualle/features/combined.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,24 +21,25 @@
 
 
 CombinedFeaturesData = Dict[Type[Features], Any]
 
 
 class CombinedFeatures(Features):
     """Combine n features by horizontal stacking"""
+
     def __init__(self, features: List[Features]):
         self.features = features
 
     def fit(self, X: CombinedFeaturesData, y=None):
         self.features_ = self.features
         for f in self.features_:
             f.fit(X[f.__class__])
         return self
 
     def transform(self, X: CombinedFeaturesData):
         check_is_fitted(self)
         combined = [f.transform(X[f.__class__]) for f in self.features_]
         issparse = any(map(sp.issparse, combined))
         if issparse:
-            return sp.hstack(combined, format='csr')
+            return sp.hstack(combined, format="csr")
         else:
             return np.hstack(combined)
```

### Comparing `qualle-0.1.1/qualle/features/confidence.py` & `qualle-0.2.0/qualle/features/confidence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/features/label_calibration/__init__.py` & `qualle-0.2.0/qualle/features/label_calibration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/features/label_calibration/base.py` & `qualle-0.2.0/qualle/features/label_calibration/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,13 +15,12 @@
 
 from sklearn.base import RegressorMixin, BaseEstimator
 
 from qualle.models import Documents, Labels
 
 
 class AbstractLabelCalibrator(BaseEstimator, RegressorMixin):
-
     def fit(self, X: Documents, y: List[Labels]):
         pass  # pragma: no cover
 
     def predict(self, X: Documents):
         pass  # pragma: no cover
```

### Comparing `qualle-0.1.1/qualle/features/label_calibration/simple_label_calibration.py` & `qualle-0.2.0/qualle/features/label_calibration/simple_label_calibration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,14 @@
 
 
 def transform_to_label_count(X: List[Labels]) -> np.array:
     return np.array(list(map(len, X)))
 
 
 class SimpleLabelCalibrator(AbstractLabelCalibrator):
-
     def __init__(self, regressor: RegressorMixin):
         self.regressor = regressor
 
     def fit(self, X: Documents, y: List[Labels]):
         self.calibrator_ = LabelCalibrator(self.regressor)
         y_transformed = transform_to_label_count(y)
         self.calibrator_.fit(X, y_transformed)
@@ -41,15 +40,14 @@
 
     def predict(self, X: Documents):
         check_is_fitted(self)
         return self.calibrator_.predict(X)
 
 
 class SimpleLabelCalibrationFeatures(Features):
-
     def transform(self, X: LabelCalibrationData):
         no_of_pred_labels = transform_to_label_count(X.predicted_labels)
         rows = len(X.predicted_no_of_labels)
         data = np.zeros((rows, 2))
         data[:, 0] = X.predicted_no_of_labels
         data[:, 1] = X.predicted_no_of_labels - no_of_pred_labels
         return data
```

### Comparing `qualle-0.1.1/qualle/features/label_calibration/thesauri_label_calibration.py` & `qualle-0.2.0/qualle/features/label_calibration/thesauri_label_calibration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,171 +16,173 @@
 from functools import lru_cache
 from typing import List, Set, Optional
 
 import numpy as np
 from rdflib import URIRef, Graph
 from rdflib.namespace import SKOS, RDF
 from scipy.sparse import coo_matrix
-from sklearn.base import TransformerMixin
 from sklearn.ensemble import ExtraTreesRegressor
 from sklearn.utils.validation import check_is_fitted
-from stwfsapy import thesaurus
 
 from qualle.features.base import Features
 from qualle.features.label_calibration.base import AbstractLabelCalibrator
 from qualle.label_calibration.category import MultiCategoryLabelCalibrator
 from qualle.models import Labels, Documents, LabelCalibrationData, Matrix
 from qualle.utils import get_logger
 
 
-class LabelCountForSubthesauriTransformer(TransformerMixin):
-    # Do not inherit from BaseEstimator to avoid refitting requirement when
-    # transformer gets cloned (e.g. in cross-val-predict)
-    """Compute count of labels per Subthesauri for a given RDF Graph."""
+class NotInitializedException(Exception):
+    pass
+
+
+class Thesaurus:
+    """Handle access to RDF Graph."""
+
     def __init__(
-            self,
-            graph: Graph,
-            subthesaurus_type_uri: URIRef,
-            concept_type_uri: URIRef,
-            concept_uri_prefix: str,
-            use_sparse_count_matrix: bool,
-            subthesauri: Optional[List[URIRef]] = None
+        self,
+        graph: Graph,
+        subthesaurus_type_uri: URIRef,
+        concept_type_uri: URIRef,
+        concept_uri_prefix: str,
     ):
         self.graph = graph
         self.subthesaurus_type_uri = subthesaurus_type_uri
         self.concept_type_uri = concept_type_uri
-        self.subthesauri = subthesauri
-        self.use_sparse_count_matrix = use_sparse_count_matrix
-        self.concept_uri_prefix = concept_uri_prefix
-
-    def fit(self, X=None, y=None):
-        self.mapping_ = dict()
-        self.logger_ = get_logger()
-        self.concept_uri_prefix_len_ = 1 + len(
-            self.concept_uri_prefix.rstrip('/')
-        )
-        if self.subthesauri:
-            self.subthesauri_ = self.subthesauri
-        else:
-            self.subthesauri_ = list(thesaurus.extract_by_type_uri(
-                self.graph,
-                self.subthesaurus_type_uri,
-            ))
-        subthesauri_len = len(self.subthesauri_)
+        self.concept_uri_prefix_len_ = 1 + len(concept_uri_prefix.rstrip("/"))
+
+    @lru_cache(maxsize=1000)
+    def get_concepts_for_subthesaurus(self, subthesaurus: URIRef) -> Set:
+        concepts = set()
+        for x in self.graph[subthesaurus : SKOS.narrower]:
+            if (x, RDF.type, self.subthesaurus_type_uri) in self.graph:
+                concepts_from_subthesaurus = self.get_concepts_for_subthesaurus(x)
+                concepts = concepts.union(concepts_from_subthesaurus)
+            elif (x, RDF.type, self.concept_type_uri) in self.graph:
+                concepts.add(self.extract_concept_id_from_uri_ref(x))
+            else:
+                logging.warning("unknown narrower type %s", str(x))
+        return concepts
+
+    def get_all_subthesauri(self) -> List[URIRef]:
+        return list(self.graph[: RDF.type : self.subthesaurus_type_uri])
+
+    def extract_concept_id_from_uri_ref(self, concept_uri: URIRef):
+        return concept_uri.toPython()[self.concept_uri_prefix_len_ :]
+
+
+class LabelCountForSubthesauriTransformer:
+    """Compute count of labels per Subthesauri for a given RDF Graph."""
+
+    def __init__(
+        self,
+        use_sparse_count_matrix: bool,
+    ):
+        self._use_sparse_count_matrix = use_sparse_count_matrix
+        self._mapping = None
+        self._logger = get_logger()
+        self._subthesauri_count = 0
+
+    def init(self, thesaurus: Thesaurus, subthesauri: Optional[List[URIRef]]):
+        self._mapping = dict()
+        self._subthesauri_count = len(subthesauri)
 
-        for idx, s in enumerate(self.subthesauri_):
-            concepts = self._get_concepts_for_thesaurus(s)
+        for idx, s in enumerate(subthesauri):
+            concepts = thesaurus.get_concepts_for_subthesaurus(s)
             for c in concepts:
-                if c not in self.mapping_:
-                    self.mapping_[c] = [False] * subthesauri_len
-                self.mapping_[c][idx] = True
+                if c not in self._mapping:
+                    self._mapping[c] = [False] * self._subthesauri_count
+                self._mapping[c][idx] = True
         return self
 
     def transform(self, X: List[Labels]) -> Matrix:
-        """Transform rows of concepts to 2-dimensional count array
+        """Transform rows of concepts to 2-dimensional count matrix
 
         Each row in the result matrix contains in each column the total
-        amount of labels per subthesauri. The subthesauri are given
-        in the same order as in the list passed to the constructor.
+        amount of labels per subthesaurus.
         """
-        check_is_fitted(self)
-        if self.use_sparse_count_matrix:
-            values = []
-            row_inds = []
-            col_inds = []
+        if not self._mapping:
+            raise NotInitializedException()
+
+        if self._use_sparse_count_matrix:
+            return self._transform_with_sparse_matrix(X)
         else:
-            count_matrix = np.zeros((len(X), len(self.subthesauri_)))
+            return self._transform_without_sparse_matrix(X)
+
+    def _transform_with_sparse_matrix(self, X: List[Labels]) -> Matrix:
+        values = []
+        row_inds = []
+        col_inds = []
         for row_idx, row in enumerate(X):
             subthesauri_counts = self._extract_subthesauri_counts(row)
-            if self.use_sparse_count_matrix:
-                for col_idx, count in enumerate(subthesauri_counts):
-                    if count:
-                        values.append(count)
-                        row_inds.append(row_idx)
-                        col_inds.append(col_idx)
-            else:
-                count_matrix[row_idx] = subthesauri_counts
+            for col_idx, count in enumerate(subthesauri_counts):
+                if count:
+                    values.append(count)
+                    row_inds.append(row_idx)
+                    col_inds.append(col_idx)
 
-        if self.use_sparse_count_matrix:
-            return coo_matrix(
-                (values, (row_inds, col_inds)),
-                shape=(len(X), len(self.subthesauri_))
-            )
-        else:
-            return count_matrix
+        return coo_matrix(
+            (values, (row_inds, col_inds)), shape=(len(X), self._subthesauri_count)
+        )
+
+    def _transform_without_sparse_matrix(self, X: List[Labels]) -> Matrix:
+        count_matrix = np.zeros((len(X), self._subthesauri_count))
+        for row_idx, row in enumerate(X):
+            subthesauri_counts = self._extract_subthesauri_counts(row)
+            count_matrix[row_idx] = subthesauri_counts
+
+        return count_matrix
 
     def _extract_subthesauri_counts(self, labels: Labels):
-        subthesauri_counts = [0] * len(self.subthesauri_)
+        subthesauri_counts = [0] * self._subthesauri_count
         for concept in labels:
-            subthesauri_membership = self.mapping_.get(concept)
+            subthesauri_membership = self._mapping.get(concept)
             if not subthesauri_membership:
-                self.logger_.warning(
+                self._logger.warning(
                     'Concept "%s" not found in concept map. '
-                    'Seems to be invalid for this thesaurus.',
-                    concept
+                    "Seems to be invalid for this thesaurus.",
+                    concept,
                 )
             else:
                 for j, is_in_subthesauri in enumerate(subthesauri_membership):
                     if is_in_subthesauri:
                         subthesauri_counts[j] = subthesauri_counts[j] + 1
         return subthesauri_counts
 
-    @lru_cache(maxsize=1000)
-    def _get_concepts_for_thesaurus(self, thesaurus: URIRef) -> Set:
-        concepts = set()
-        for x in self.graph[thesaurus:SKOS.narrower]:
-            if (x, RDF.type, self.subthesaurus_type_uri) in self.graph:
-                concepts_from_subthesaurus = self._get_concepts_for_thesaurus(
-                    x)
-                concepts = concepts.union(concepts_from_subthesaurus)
-            elif (x, RDF.type, self.concept_type_uri) in self.graph:
-                concepts.add(self._extract_concept_id_from_uri_ref(x))
-            else:
-                logging.warning('unknown narrower type %s', str(x))
-        return concepts
-
-    def _extract_concept_id_from_uri_ref(self,  concept_uri: URIRef):
-        return concept_uri.toPython()[self.concept_uri_prefix_len_:]
-
 
 class ThesauriLabelCalibrator(AbstractLabelCalibrator):
-
     def __init__(
-            self, transformer: LabelCountForSubthesauriTransformer,
-            regressor_class=ExtraTreesRegressor,
-            regressor_params=None
+        self,
+        transformer: LabelCountForSubthesauriTransformer,
+        regressor_class=ExtraTreesRegressor,
+        regressor_params=None,
     ):
         self.transformer = transformer
         self.regressor_class = regressor_class
         self.regressor_params = regressor_params
 
     def fit(self, X: Documents, y: List[Labels]):
         self.calibrator_ = MultiCategoryLabelCalibrator(
-            regressor_class=self.regressor_class,
-            regressor_params=self.regressor_params
+            regressor_class=self.regressor_class, regressor_params=self.regressor_params
         )
         y_transformed = self.transformer.transform(y)
         self.calibrator_.fit(X, y_transformed)
         return self
 
     def predict(self, X: Documents):
         check_is_fitted(self)
         return self.calibrator_.predict(X)
 
 
 class ThesauriLabelCalibrationFeatures(Features):
-
     def __init__(self, transformer: LabelCountForSubthesauriTransformer):
         self.transformer = transformer
 
     def transform(self, X: LabelCalibrationData):
         rows = len(X.predicted_no_of_labels)
-        no_of_predicted_labels = self.transformer.transform(
-            X.predicted_labels
-        )
-        subthesauri_len = len(self.transformer.subthesauri_)
-        data = np.zeros((rows, 2 * subthesauri_len))
-        data[:, :subthesauri_len] = X.predicted_no_of_labels
-        data[:, subthesauri_len:] = (
-                X.predicted_no_of_labels - no_of_predicted_labels
+        no_of_predicted_labels = self.transformer.transform(X.predicted_labels)
+        transformed_cols_len = no_of_predicted_labels.shape[1]
+        data = np.zeros((rows, 2 * transformed_cols_len))
+        data[:, :transformed_cols_len] = X.predicted_no_of_labels
+        data[:, transformed_cols_len:] = (
+            X.predicted_no_of_labels - no_of_predicted_labels
         )
         return data
```

### Comparing `qualle-0.1.1/qualle/features/text.py` & `qualle-0.2.0/qualle/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import logging
+from contextlib import contextmanager
+from time import perf_counter
 from typing import List
 
-from sklearn.utils.validation import check_is_fitted
-from stwfsapy.text_features import mk_text_features
+from qualle.models import Labels
 
-from qualle.features.base import Features
 
+def recall(true_labels: List[Labels], predicted_labels: List[Labels]) -> List:
+    return [
+        len(set(tc) & set(pc)) / len_tc if (len_tc := len(tc)) > 0 else 0
+        for tc, pc in zip(true_labels, predicted_labels)
+    ]
 
-class TextFeatures(Features):
-    """Features based on the text string of a document."""
 
-    def fit(self, X: List[str], y=None):
-        self.features_ = mk_text_features()
-        self.features_.fit(X)
-        return self
+def get_logger():
+    return logging.getLogger("qualle")
 
-    def transform(self, X: List[str]):
-        check_is_fitted(self)
-        return self.features_.transform(X)
+
+@contextmanager
+def timeit():
+    """Context manager to time the code block wrapped by the manager.
+
+    Yielded object is a lambda function which can be called to compute the
+    duration (in seconds) of the executed code block.
+    """
+    start = perf_counter()
+    yield lambda: perf_counter() - start
```

### Comparing `qualle-0.1.1/qualle/interface/__init__.py` & `qualle-0.2.0/qualle/interface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/interface/config.py` & `qualle-0.2.0/qualle/interface/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from enum import Enum
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
-from pydantic import BaseSettings
+from pydantic import BaseSettings, root_validator, FilePath, DirectoryPath
 from pydantic.networks import AnyUrl
 from qualle.features.confidence import ConfidenceFeatures
 from qualle.features.text import TextFeatures
 
 
+FileOrDirPath = Union[FilePath, DirectoryPath]
+
+
 class RegressorSettings(BaseSettings):
     regressor_class: str
     params: Dict
 
 
 class SubthesauriLabelCalibrationSettings(BaseSettings):
-    thesaurus_file: Path
+    thesaurus_file: FilePath
     subthesaurus_type: AnyUrl
     concept_type: AnyUrl
     concept_type_prefix: AnyUrl
     subthesauri: List[AnyUrl]
     use_sparse_count_matrix: bool = False
 
 
@@ -41,27 +44,43 @@
 
 
 class TrainSettings(BaseSettings):
 
     label_calibrator_regressor: RegressorSettings
     quality_estimator_regressor: RegressorSettings
 
-    train_data_path: Path
+    train_data_path: FileOrDirPath
     output_path: Path
 
     features: List[FeaturesEnum]
 
-    subthesauri_label_calibration: Optional[
-        SubthesauriLabelCalibrationSettings] = None
+    subthesauri_label_calibration: Optional[SubthesauriLabelCalibrationSettings] = None
 
     should_debug: bool = False
 
 
 class EvalSettings(BaseSettings):
-    test_data_path: Path
-    model_file: Path
+    test_data_path: FileOrDirPath
+    model_file: FilePath
+
+
+class PredictSettings(BaseSettings):
+    predict_data_path: FileOrDirPath
+    model_file: FilePath
+    output_path: Optional[Path]
+
+    @root_validator
+    def check_output_path_specified_for_input_file(cls, values):
+        predict_data_path = values.get("predict_data_path")
+        output_path = values.get("output_path")
+        if predict_data_path.is_file() and not output_path:
+            raise ValueError(
+                "output_path has to be specified if predict_data_path "
+                "refers to a file"
+            )
+        return values
 
 
 class RESTSettings(BaseSettings):
-    model_file: Path
+    model_file: FilePath
     port: int = 8000
-    host: str = '127.0.0.1'
+    host: str = "127.0.0.1"
```

### Comparing `qualle-0.1.1/qualle/interface/internal.py` & `qualle-0.2.0/qualle/interface/internal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,144 +11,217 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Internal interface to access Qualle functionality"""
 
 from importlib import import_module
-from typing import Type
+from pathlib import Path
+from typing import Type, Optional, List, Any, Union
 
 from joblib import dump, load
 from rdflib import Graph, URIRef
 
 from qualle.evaluate import Evaluator
-from qualle.features.label_calibration.simple_label_calibration import \
-    SimpleLabelCalibrator, SimpleLabelCalibrationFeatures
-from qualle.features.label_calibration.thesauri_label_calibration import \
-    ThesauriLabelCalibrator, ThesauriLabelCalibrationFeatures, \
-    LabelCountForSubthesauriTransformer
-from qualle.interface.config import TrainSettings, EvalSettings
+from qualle.features.label_calibration.simple_label_calibration import (
+    SimpleLabelCalibrator,
+    SimpleLabelCalibrationFeatures,
+)
+from qualle.features.label_calibration.thesauri_label_calibration import (
+    ThesauriLabelCalibrator,
+    ThesauriLabelCalibrationFeatures,
+    LabelCountForSubthesauriTransformer,
+    Thesaurus,
+)
+from qualle.interface.config import TrainSettings, EvalSettings, PredictSettings
+from qualle.models import TrainData, PredictData
 from qualle.train import Trainer
-from qualle.utils import get_logger, load_train_input, timeit
+from qualle.utils import get_logger, timeit
+from qualle.interface.data.annif import AnnifHandler
+from qualle.interface.data.tsv import (
+    load_train_input as load_tsv_train_input,
+    load_predict_input,
+)
 
 
 def train(settings: TrainSettings):
     logger = get_logger()
     path_to_train_data = settings.train_data_path
     path_to_model_output_file = settings.output_path
     slc_settings = settings.subthesauri_label_calibration
     features = list(map(lambda f: f.value(), settings.features))
 
     lc_regressor_cls = _get_class_from_str(
         settings.label_calibrator_regressor.regressor_class
     )
     lc_regressor_params = settings.label_calibrator_regressor.params
     logger.debug(
-        'Use (%s %s) as Regressor for Label Calibration',
+        "Use (%s %s) as Regressor for Label Calibration",
         settings.label_calibrator_regressor.regressor_class,
-        settings.label_calibrator_regressor.params
+        settings.label_calibrator_regressor.params,
     )
 
     quality_estimator_cls = _get_class_from_str(
         settings.quality_estimator_regressor.regressor_class
     )
     quality_estimator = quality_estimator_cls(
         **settings.quality_estimator_regressor.params
     )
     logger.debug(
-        'Use (%s %s) as Regressor for Quality Estimation',
+        "Use (%s %s) as Regressor for Quality Estimation",
         settings.quality_estimator_regressor.regressor_class,
-        settings.quality_estimator_regressor.params
+        settings.quality_estimator_regressor.params,
     )
 
     with timeit() as t:
-        train_data = load_train_input(str(path_to_train_data))
-    logger.debug('Loaded train data in %.4f seconds', t())
+        train_data = _load_train_input(path_to_train_data)
+
+    logger.debug("Loaded train data in %.4f seconds", t())
 
     if slc_settings:
-        logger.info('Run training with Subthesauri Label Calibration')
+        logger.info("Run training with Subthesauri Label Calibration")
         path_to_graph = slc_settings.thesaurus_file
         g = Graph()
         with timeit() as t:
-            g.parse(str(path_to_graph))
-        logger.debug('Parsed RDF Graph in %.4f seconds', t())
+            g.parse(path_to_graph)
+        logger.debug("Parsed RDF Graph in %.4f seconds", t())
 
-        if not slc_settings.subthesauri:
-            logger.info(
-                'No subthesauri passed, will extract subthesauri by type'
-            )
-        if slc_settings.use_sparse_count_matrix:
-            logger.info(
-                'Will use Sparse Count Matrix for '
-                'Subthesauri Label Calibration'
-            )
-        transformer = LabelCountForSubthesauriTransformer(
+        thesaurus = Thesaurus(
             graph=g,
             subthesaurus_type_uri=URIRef(slc_settings.subthesaurus_type),
             concept_type_uri=URIRef(slc_settings.concept_type),
-            subthesauri=list(map(
-                lambda s: URIRef(s), slc_settings.subthesauri
-            )),
             concept_uri_prefix=slc_settings.concept_type_prefix,
-            use_sparse_count_matrix=slc_settings.use_sparse_count_matrix
         )
-        with timeit() as t:
-            transformer.fit()
-        logger.debug(
-            'Ran Subthesauri Transformer fit in %.4f seconds', t()
+        subthesauri = list(map(lambda s: URIRef(s), slc_settings.subthesauri))
+        if not subthesauri:
+            logger.info("No subthesauri passed, will extract subthesauri by type")
+            subthesauri = thesaurus.get_all_subthesauri()
+            logger.debug("Extracted %d subthesauri", len(subthesauri))
+        if slc_settings.use_sparse_count_matrix:
+            logger.info(
+                "Will use Sparse Count Matrix for " "Subthesauri Label Calibration"
+            )
+        transformer = LabelCountForSubthesauriTransformer(
+            use_sparse_count_matrix=slc_settings.use_sparse_count_matrix
         )
+        transformer.init(thesaurus=thesaurus, subthesauri=subthesauri)
+
         label_calibration_features = ThesauriLabelCalibrationFeatures(
             transformer=transformer
         )
         features.append(label_calibration_features)
         t = Trainer(
             train_data=train_data,
             label_calibrator=ThesauriLabelCalibrator(
                 regressor_class=lc_regressor_cls,
                 regressor_params=lc_regressor_params,
-                transformer=transformer),
+                transformer=transformer,
+            ),
             quality_regressor=quality_estimator,
             features=features,
-            should_debug=settings.should_debug
+            should_debug=settings.should_debug,
         )
     else:
-        logger.info('Run training with Simple Label Calibration')
+        logger.info("Run training with Simple Label Calibration")
         label_calibration_features = SimpleLabelCalibrationFeatures()
         features.append(label_calibration_features)
         t = Trainer(
             train_data=train_data,
             label_calibrator=SimpleLabelCalibrator(
                 lc_regressor_cls(**lc_regressor_params)
             ),
             quality_regressor=quality_estimator,
             features=features,
-            should_debug=settings.should_debug
+            should_debug=settings.should_debug,
         )
 
     model = t.train()
-    logger.info('Store trained model in %s', path_to_model_output_file)
+    logger.info("Store trained model in %s", path_to_model_output_file)
     dump(model, path_to_model_output_file)
 
 
 def _get_class_from_str(fully_qualified_path: str) -> Type:
-    split = fully_qualified_path.split('.')
-    module = '.'.join(split[:-1])
+    split = fully_qualified_path.split(".")
+    module = ".".join(split[:-1])
     cls_name = split[-1]
     return getattr(import_module(module), cls_name)
 
 
 def evaluate(settings: EvalSettings):
     logger = get_logger()
     path_to_test_data = settings.test_data_path
     path_to_model_file = settings.model_file
-    model = load_model(path_to_model_file)
-    logger.info('Run evaluation with model:\n%s', model)
-    test_input = load_train_input(str(path_to_test_data))
+    model = load_model(str(path_to_model_file))
+    logger.info("Run evaluation with model:\n%s", model)
+    test_input = _load_train_input(path_to_test_data)
     ev = Evaluator(test_input, model)
     eval_data = ev.evaluate()
-    logger.info('\nScores:')
+    logger.info("\nScores:")
     for metric, score in eval_data.items():
-        logger.info(f'{metric}: {score}')
+        logger.info(f"{metric}: {score}")
+
+
+def predict(settings: PredictSettings):
+    logger = get_logger()
+    path_to_predict_data = settings.predict_data_path
+    path_to_model_file = settings.model_file
+    output_path = settings.output_path
+    model = load_model(str(path_to_model_file))
+    io_handler = _get_predict_io_handler(
+        predict_data_path=path_to_predict_data, output_path=output_path
+    )
+    predict_data = io_handler.load_predict_data()
+    logger.info("Run predict with model:\n%s", model)
+
+    scores = model.predict(predict_data)
+    io_handler.store(scores)
 
 
 def load_model(path_to_model_file: str):
     return load(path_to_model_file)
+
+
+def _load_train_input(p: Path) -> TrainData:
+    if p.is_dir():
+        train_input = AnnifHandler(dir=p).load_train_input().train_data
+    else:
+        train_input = load_tsv_train_input(p)
+    return train_input
+
+
+class PredictTSVIOHandler:
+    def __init__(self, predict_data_path: Path, output_path: Optional[Path] = None):
+        self._predict_data_path = predict_data_path
+        self._output_path = output_path
+
+    def load_predict_data(self):
+        return load_predict_input(self._predict_data_path)
+
+    def store(self, data: List[Any]):
+        with self._output_path.open("w") as f:
+            for d in data:
+                f.write(str(d) + "\n")
+
+
+class PredictAnnifIOHandler:
+    def __init__(self, predict_data_path: Path):
+        self._annif_handler = AnnifHandler(dir=predict_data_path)
+        self._doc_ids = []
+
+    def load_predict_data(self) -> PredictData:
+        data = self._annif_handler.load_predict_input()
+        self._doc_ids = data.document_ids
+        return data.predict_data
+
+    def store(self, data: List[Any]):
+        quality_ests = zip(data, self._doc_ids)
+        self._annif_handler.store_quality_estimations(quality_ests)
+
+
+def _get_predict_io_handler(
+    predict_data_path: Path, output_path: Optional[Path]
+) -> Union[PredictAnnifIOHandler, PredictTSVIOHandler]:
+    if predict_data_path.is_dir():
+        return PredictAnnifIOHandler(predict_data_path)
+    return PredictTSVIOHandler(
+        predict_data_path=predict_data_path, output_path=output_path
+    )
```

### Comparing `qualle-0.1.1/qualle/interface/rest.py` & `qualle-0.2.0/qualle/interface/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,29 +21,29 @@
 from pydantic.main import BaseModel
 
 from qualle.interface.config import RESTSettings
 from qualle.interface.internal import load_model as internal_load_model
 from qualle.models import PredictData
 from qualle.pipeline import QualityEstimationPipeline
 
-PREDICT_ENDPOINT = '/predict'
+PREDICT_ENDPOINT = "/predict"
 
 
 class Document(BaseModel):
     content: str
     predicted_labels: List[str]
     scores: List[float]
 
 
 class Documents(BaseModel):
     documents: List[Document]
 
 
 class Metric(Enum):
-    RECALL = 'recall'
+    RECALL = "recall"
 
 
 class QualityScores(BaseModel):
     name: Metric
     scores: List[float]
 
 
@@ -58,45 +58,41 @@
 @lru_cache
 def load_model() -> QualityEstimationPipeline:
     settings = RESTSettings()
     return internal_load_model(str(settings.model_file))
 
 
 @router.post(
-    PREDICT_ENDPOINT, status_code=status.HTTP_200_OK,
-    response_model=QualityEstimation
+    PREDICT_ENDPOINT, status_code=status.HTTP_200_OK, response_model=QualityEstimation
 )
 def predict(
-        documents: Documents,
-        qe_pipeline: QualityEstimationPipeline = Depends(load_model)
+    documents: Documents, qe_pipeline: QualityEstimationPipeline = Depends(load_model)
 ) -> QualityEstimation:
     predict_data = _map_documents_to_predict_data(documents)
     scores = qe_pipeline.predict(predict_data)
-    return QualityEstimation(scores=[QualityScores(
-        name=Metric.RECALL, scores=list(scores))
-    ])
+    return QualityEstimation(
+        scores=[QualityScores(name=Metric.RECALL, scores=list(scores))]
+    )
 
 
-@router.get('/_up')
+@router.get("/_up")
 def up():
     return True
 
 
 def _map_documents_to_predict_data(documents: Documents) -> PredictData:
     docs = []
     p_labels = []
     scores = []
 
     for idx, doc in enumerate(documents.documents):
         docs.append(doc.content)
         p_labels.append(doc.predicted_labels)
         scores.append(doc.scores)
-    return PredictData(
-        docs=docs, predicted_labels=p_labels, scores=scores
-    )
+    return PredictData(docs=docs, predicted_labels=p_labels, scores=scores)
 
 
 def create_app(settings: Optional[RESTSettings] = None):
     settings = settings or RESTSettings()
     app = FastAPI()
     app.include_router(router)
     m = internal_load_model(str(settings.model_file))
```

### Comparing `qualle-0.1.1/qualle/label_calibration/__init__.py` & `qualle-0.2.0/qualle/label_calibration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `qualle-0.1.1/qualle/label_calibration/category.py` & `qualle-0.2.0/qualle/label_calibration/category.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,33 +23,29 @@
 from qualle.models import Matrix
 
 
 class MultiCategoryLabelCalibrator(BaseEstimator, RegressorMixin):
     """Label calibrator for multiple distinct categories.
     E.g. to predict the no of labels for different thesauri."""
 
-    def __init__(
-            self,
-            regressor_class=ExtraTreesRegressor,
-            regressor_params=None
-    ):
+    def __init__(self, regressor_class=ExtraTreesRegressor, regressor_params=None):
         self.regressor_class = regressor_class
         self.regressor_params = regressor_params or {}
 
     def fit(self, X: List[str], y: Matrix):
         """
         :param X: list of content, e.g. doc titles
         :param y: matrix where each column corresponds to no of labels for
             respective category
         :return: self
         """
         try:
             no_categories = y.shape[1]
         except IndexError:
-            raise ValueError('Number of categories must be greater 0')
+            raise ValueError("Number of categories must be greater 0")
 
         self.calibrators_ = [
             LabelCalibrator(self.regressor_class(**self.regressor_params))
             for _ in range(no_categories)
         ]
 
         y_is_sparse = issparse(y)
```

### Comparing `qualle-0.1.1/qualle/label_calibration/simple.py` & `qualle-0.2.0/qualle/label_calibration/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,24 +14,23 @@
 from typing import List
 
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.ensemble import ExtraTreesRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.utils.validation import check_is_fitted
 
-from stwfsapy.text_features import mk_text_features
+from qualle.features.text import TextFeatures
 
 
 class LabelCalibrator(BaseEstimator, RegressorMixin):
-
     def __init__(self, regressor=ExtraTreesRegressor()):
         self.regressor = regressor
 
     def fit(self, X: List[str], y):
-        features = mk_text_features()
+        features = TextFeatures()
         self.pipeline_ = Pipeline(
             [("features", features), ("regressor", self.regressor)]
         )
         self.pipeline_.fit(X, y)
         return self
 
     def predict(self, X: List[str]):
```

### Comparing `qualle-0.1.1/qualle/main.py` & `qualle-0.2.0/qualle/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,9 +11,9 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from qualle.interface.cli import cli_entrypoint
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli_entrypoint()
```

### Comparing `qualle-0.1.1/qualle/pipeline.py` & `qualle-0.2.0/qualle/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,53 +19,46 @@
 from qualle.features.label_calibration.base import AbstractLabelCalibrator
 from qualle.models import TrainData, PredictData, LabelCalibrationData
 from qualle.quality_estimation import QualityEstimator
 from qualle.utils import recall, get_logger, timeit
 
 
 class QualityEstimationPipeline:
-
     def __init__(
-            self,
-            label_calibrator: AbstractLabelCalibrator,
-            recall_predictor: QualityEstimator,
-            features_data_mapper: Callable[
-                [PredictData, LabelCalibrationData], Any
-            ],
-            should_debug=False
+        self,
+        label_calibrator: AbstractLabelCalibrator,
+        recall_predictor: QualityEstimator,
+        features_data_mapper: Callable[[PredictData, LabelCalibrationData], Any],
+        should_debug=False,
     ):
         self._label_calibrator = label_calibrator
         self._recall_predictor = recall_predictor
         self._features_data_mapper = features_data_mapper
         self._should_debug = should_debug
         self._logger = get_logger()
 
     def train(self, data: TrainData):
         predict_data = data.predict_data
-        with self._debug('cross_val_predict with label calibrator'):
+        with self._debug("cross_val_predict with label calibrator"):
             predicted_no_of_labels = cross_val_predict(
                 self._label_calibrator, predict_data.docs, data.true_labels
             )
 
-        with self._debug('label calibrator fit'):
+        with self._debug("label calibrator fit"):
             self._label_calibrator.fit(predict_data.docs, data.true_labels)
 
         label_calibration_data = LabelCalibrationData(
             predicted_labels=predict_data.predicted_labels,
-            predicted_no_of_labels=predicted_no_of_labels
-        )
-        features_data = self._features_data_mapper(
-            predict_data, label_calibration_data
+            predicted_no_of_labels=predicted_no_of_labels,
         )
-        with self._debug('recall computation'):
-            true_recall = recall(
-                data.true_labels, predict_data.predicted_labels
-            )
+        features_data = self._features_data_mapper(predict_data, label_calibration_data)
+        with self._debug("recall computation"):
+            true_recall = recall(data.true_labels, predict_data.predicted_labels)
 
-        with self._debug('RecallPredictor fit'):
+        with self._debug("RecallPredictor fit"):
             self._recall_predictor.fit(features_data, true_recall)
 
     def predict(self, data: PredictData) -> List[float]:
         zero_idxs = self._get_pdata_idxs_with_zero_labels(data)
         data_with_labels = self._get_pdata_with_labels(data, zero_idxs)
         if data_with_labels.docs:
             predicted_no_of_labels = self._label_calibrator.predict(
@@ -74,67 +67,61 @@
             label_calibration_data = LabelCalibrationData(
                 predicted_labels=data_with_labels.predicted_labels,
                 predicted_no_of_labels=predicted_no_of_labels,
             )
             features_data = self._features_data_mapper(
                 data_with_labels, label_calibration_data
             )
-            predicted_recall = self._recall_predictor.predict(
-                features_data
-            )
+            predicted_recall = self._recall_predictor.predict(features_data)
             recall_scores = self._merge_zero_recall_with_predicted_recall(
                 predicted_recall=predicted_recall,
                 zero_labels_idx=zero_idxs,
             )
         else:
             recall_scores = [0] * len(data.predicted_labels)
         return recall_scores
 
     @staticmethod
     def _get_pdata_idxs_with_zero_labels(data: PredictData) -> Collection[int]:
         return [
-            i for i in range(len(data.predicted_labels))
-            if not data.predicted_labels[i]
+            i for i in range(len(data.predicted_labels)) if not data.predicted_labels[i]
         ]
 
     @staticmethod
     def _get_pdata_with_labels(
         data: PredictData, zero_labels_idxs: Collection[int]
     ) -> PredictData:
         non_zero_idxs = [
-            i for i in range(len(data.predicted_labels))
-            if i not in zero_labels_idxs
+            i for i in range(len(data.predicted_labels)) if i not in zero_labels_idxs
         ]
         return PredictData(
             docs=[data.docs[i] for i in non_zero_idxs],
             predicted_labels=[data.predicted_labels[i] for i in non_zero_idxs],
             scores=[data.scores[i] for i in non_zero_idxs],
         )
 
     @staticmethod
     def _merge_zero_recall_with_predicted_recall(
         predicted_recall: List[float],
         zero_labels_idx: Collection[int],
     ):
         recall_scores = []
         j = 0
-        for i in range(
-                len(zero_labels_idx) +
-                len(predicted_recall)):
+        for i in range(len(zero_labels_idx) + len(predicted_recall)):
             if i in zero_labels_idx:
                 recall_scores.append(0)
             else:
                 recall_scores.append(predicted_recall[j])
                 j += 1
         return recall_scores
 
     @contextmanager
     def _debug(self, method_name):
         if self._should_debug:
             with timeit() as t:
                 yield
-            self._logger.debug('Ran %s in %.4f seconds', method_name, t())
+            self._logger.debug("Ran %s in %.4f seconds", method_name, t())
         else:
             yield
 
     def __str__(self):
-        return f'{self._label_calibrator}\n{self._recall_predictor}'
+        return f"{self._label_calibrator}\n{self._recall_predictor}"
```

### Comparing `qualle-0.1.1/qualle/quality_estimation.py` & `qualle-0.2.0/qualle/quality_estimation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,26 +18,21 @@
 
 from qualle.features.base import Features
 
 
 class QualityEstimator(BaseEstimator, RegressorMixin):
     """Regressor which uses a pipeline with given features and regressor."""
 
-    def __init__(
-            self,
-            regressor: RegressorMixin,
-            features: Features
-    ):
+    def __init__(self, regressor: RegressorMixin, features: Features):
         self.regressor = regressor
         self.features = features
 
     def fit(self, X, y):
-        self.pipeline_ = Pipeline([
-            ("features", self.features),
-            ("regressor", self.regressor)
-        ])
+        self.pipeline_ = Pipeline(
+            [("features", self.features), ("regressor", self.regressor)]
+        )
         self.pipeline_.fit(X, y)
         return self
 
     def predict(self, X):
         check_is_fitted(self)
         return self.pipeline_.predict(X)
```

### Comparing `qualle-0.1.1/qualle/train.py` & `qualle-0.2.0/qualle/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021-2022 ZBW – Leibniz Information Centre for Economics
+#  Copyright 2021-2023 ZBW – Leibniz Information Centre for Economics
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,68 +15,65 @@
 
 from sklearn.base import RegressorMixin
 
 from qualle.features.base import Features
 from qualle.features.combined import CombinedFeaturesData, CombinedFeatures
 from qualle.features.confidence import ConfidenceFeatures
 from qualle.features.label_calibration.base import AbstractLabelCalibrator
-from qualle.features.label_calibration.simple_label_calibration import \
-    SimpleLabelCalibrationFeatures
-from qualle.features.label_calibration.thesauri_label_calibration import \
-    ThesauriLabelCalibrationFeatures
+from qualle.features.label_calibration.simple_label_calibration import (
+    SimpleLabelCalibrationFeatures,
+)
+from qualle.features.label_calibration.thesauri_label_calibration import (
+    ThesauriLabelCalibrationFeatures,
+)
 from qualle.features.text import TextFeatures
 from qualle.models import PredictData, LabelCalibrationData
 from qualle.pipeline import QualityEstimationPipeline
 from qualle.quality_estimation import QualityEstimator
 
 FeaturesTypes = Set[Type[Features]]
 
 
 class Trainer:
-
     def __init__(
-            self, train_data,
-            label_calibrator: AbstractLabelCalibrator,
-            quality_regressor: RegressorMixin,
-            features: List[Features],
-            should_debug=False
+        self,
+        train_data,
+        label_calibrator: AbstractLabelCalibrator,
+        quality_regressor: RegressorMixin,
+        features: List[Features],
+        should_debug=False,
     ):
         combined_features = CombinedFeatures(features)
-        rp = QualityEstimator(
-            regressor=quality_regressor, features=combined_features
-        )
+        rp = QualityEstimator(regressor=quality_regressor, features=combined_features)
         self._qe_p = QualityEstimationPipeline(
             recall_predictor=rp,
             label_calibrator=label_calibrator,
             should_debug=should_debug,
-            features_data_mapper=FeaturesDataMapper(
-                set(f.__class__ for f in features)
-            )
+            features_data_mapper=FeaturesDataMapper(set(f.__class__ for f in features)),
         )
         self._train_data = train_data
 
     def train(self) -> QualityEstimationPipeline:
         self._qe_p.train(self._train_data)
 
         return self._qe_p
 
 
 class FeaturesDataMapper:
-
     def __init__(self, features_types: FeaturesTypes):
         self._features_types = features_types
 
     def __call__(
-            self, p_data: PredictData, l_data: LabelCalibrationData
+        self, p_data: PredictData, l_data: LabelCalibrationData
     ) -> CombinedFeaturesData:
         features_data = dict()
         for ftype in self._features_types:
             if ftype == ConfidenceFeatures:
                 features_data[ConfidenceFeatures] = p_data.scores
             if ftype == TextFeatures:
                 features_data[TextFeatures] = p_data.docs
             if ftype in (
-                    SimpleLabelCalibrationFeatures,
-                    ThesauriLabelCalibrationFeatures
+                SimpleLabelCalibrationFeatures,
+                ThesauriLabelCalibrationFeatures,
             ):
                 features_data[ftype] = l_data
         return features_data
```

