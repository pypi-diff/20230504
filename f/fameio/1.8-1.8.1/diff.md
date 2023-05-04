# Comparing `tmp/fameio-1.8.tar.gz` & `tmp/fameio-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fameio-1.8.tar", last modified: Fri Apr 14 14:12:01 2023, max compression
+gzip compressed data, was "fameio-1.8.1.tar", last modified: Thu May  4 07:30:23 2023, max compression
```

## Comparing `fameio-1.8.tar` & `fameio-1.8.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.419520 fameio-1.8/
--rw-rw-rw-   0        0        0    10391 2023-04-14 05:55:34.000000 fameio-1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    28055 2023-04-14 14:12:01.419520 fameio-1.8/PKG-INFO
--rw-rw-rw-   0        0        0    27385 2023-04-14 14:10:34.000000 fameio-1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 14:12:01.420533 fameio-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1760 2023-04-14 05:55:34.000000 fameio-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.293521 fameio-1.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.299522 fameio-1.8/src/fameio/
--rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.310521 fameio-1.8/src/fameio/scripts/
--rw-rw-rw-   0        0        0      746 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/__init__.py
--rw-rw-rw-   0        0        0     3296 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/convert_results.py
--rw-rw-rw-   0        0        0     1339 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/scripts/make_config.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.343526 fameio-1.8/src/fameio/source/
--rw-rw-rw-   0        0        0      278 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/__init__.py
--rw-rw-rw-   0        0        0     9376 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/source/cli.py
--rw-rw-rw-   0        0        0     7403 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/loader.py
--rw-rw-rw-   0        0        0     1929 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/logs.py
--rw-rw-rw-   0        0        0     1321 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/path_resolver.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.367521 fameio-1.8/src/fameio/source/results/
--rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/__init__.py
--rw-rw-rw-   0        0        0     4321 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/agent_type.py
--rw-rw-rw-   0        0        0     3793 2023-04-14 14:10:34.000000 fameio-1.8/src/fameio/source/results/conversion.py
--rw-rw-rw-   0        0        0     4216 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/csv_writer.py
--rw-rw-rw-   0        0        0     6222 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/data_transformer.py
--rw-rw-rw-   0        0        0     3960 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/output_dao.py
--rw-rw-rw-   0        0        0     4791 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/results/reader.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.398531 fameio-1.8/src/fameio/source/scenario/
--rw-rw-rw-   0        0        0      372 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/__init__.py
--rw-rw-rw-   0        0        0     3830 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/agent.py
--rw-rw-rw-   0        0        0     5002 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/attribute.py
--rw-rw-rw-   0        0        0     8853 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/contract.py
--rw-rw-rw-   0        0        0     1455 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/exception.py
--rw-rw-rw-   0        0        0     1376 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/fameiofactory.py
--rw-rw-rw-   0        0        0     4593 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/generalproperties.py
--rw-rw-rw-   0        0        0     3582 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/scenario/scenario.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.418530 fameio-1.8/src/fameio/source/schema/
--rw-rw-rw-   0        0        0      270 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/__init__.py
--rw-rw-rw-   0        0        0     3331 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/agenttype.py
--rw-rw-rw-   0        0        0     8214 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/attribute.py
--rw-rw-rw-   0        0        0      224 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/exception.py
--rw-rw-rw-   0        0        0     1715 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/schema/schema.py
--rw-rw-rw-   0        0        0     1924 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/series.py
--rw-rw-rw-   0        0        0     6943 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/time.py
--rw-rw-rw-   0        0        0      630 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/tools.py
--rw-rw-rw-   0        0        0    11409 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/validator.py
--rw-rw-rw-   0        0        0    11633 2023-04-14 05:55:34.000000 fameio-1.8/src/fameio/source/writer.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:12:01.309521 fameio-1.8/src/fameio.egg-info/
--rw-rw-rw-   0        0        0    28055 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1470 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 14:12:00.000000 fameio-1.8/src/fameio.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 14:12:01.000000 fameio-1.8/src/fameio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.384606 fameio-1.8.1/
+-rw-rw-rw-   0        0        0    10391 2023-04-14 05:55:34.000000 fameio-1.8.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    30105 2023-05-04 07:30:23.384606 fameio-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29433 2023-05-04 05:22:58.000000 fameio-1.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:30:23.385610 fameio-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1762 2023-05-04 07:29:08.000000 fameio-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.212571 fameio-1.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.219577 fameio-1.8.1/src/fameio/
+-rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.241608 fameio-1.8.1/src/fameio/scripts/
+-rw-rw-rw-   0        0        0      746 2023-04-14 14:10:34.000000 fameio-1.8.1/src/fameio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3296 2023-04-14 14:10:34.000000 fameio-1.8.1/src/fameio/scripts/convert_results.py
+-rw-rw-rw-   0        0        0     1339 2023-04-14 14:10:34.000000 fameio-1.8.1/src/fameio/scripts/make_config.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.285609 fameio-1.8.1/src/fameio/source/
+-rw-rw-rw-   0        0        0      278 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/__init__.py
+-rw-rw-rw-   0        0        0     9384 2023-05-04 07:29:08.000000 fameio-1.8.1/src/fameio/source/cli.py
+-rw-rw-rw-   0        0        0     7403 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/loader.py
+-rw-rw-rw-   0        0        0     1929 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/logs.py
+-rw-rw-rw-   0        0        0     1321 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/path_resolver.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.320687 fameio-1.8.1/src/fameio/source/results/
+-rw-rw-rw-   0        0        0      109 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/__init__.py
+-rw-rw-rw-   0        0        0     4321 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/agent_type.py
+-rw-rw-rw-   0        0        0     3793 2023-04-14 14:10:34.000000 fameio-1.8.1/src/fameio/source/results/conversion.py
+-rw-rw-rw-   0        0        0     4216 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/csv_writer.py
+-rw-rw-rw-   0        0        0     6222 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/data_transformer.py
+-rw-rw-rw-   0        0        0     3960 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/output_dao.py
+-rw-rw-rw-   0        0        0     4791 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/results/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.358605 fameio-1.8.1/src/fameio/source/scenario/
+-rw-rw-rw-   0        0        0      372 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/__init__.py
+-rw-rw-rw-   0        0        0     3830 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/agent.py
+-rw-rw-rw-   0        0        0     5002 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/attribute.py
+-rw-rw-rw-   0        0        0     8853 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/contract.py
+-rw-rw-rw-   0        0        0     1455 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/exception.py
+-rw-rw-rw-   0        0        0     1376 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/fameiofactory.py
+-rw-rw-rw-   0        0        0     4593 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/generalproperties.py
+-rw-rw-rw-   0        0        0     3582 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/scenario/scenario.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.383608 fameio-1.8.1/src/fameio/source/schema/
+-rw-rw-rw-   0        0        0      270 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/schema/__init__.py
+-rw-rw-rw-   0        0        0     3331 2023-05-04 05:22:58.000000 fameio-1.8.1/src/fameio/source/schema/agenttype.py
+-rw-rw-rw-   0        0        0     8214 2023-05-04 05:22:58.000000 fameio-1.8.1/src/fameio/source/schema/attribute.py
+-rw-rw-rw-   0        0        0      224 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/schema/exception.py
+-rw-rw-rw-   0        0        0     1715 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/schema/schema.py
+-rw-rw-rw-   0        0        0     1924 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/series.py
+-rw-rw-rw-   0        0        0     6943 2023-05-04 05:22:58.000000 fameio-1.8.1/src/fameio/source/time.py
+-rw-rw-rw-   0        0        0      630 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/tools.py
+-rw-rw-rw-   0        0        0    11409 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/validator.py
+-rw-rw-rw-   0        0        0    11633 2023-04-14 05:55:34.000000 fameio-1.8.1/src/fameio/source/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:30:23.229570 fameio-1.8.1/src/fameio.egg-info/
+-rw-rw-rw-   0        0        0    30105 2023-05-04 07:30:22.000000 fameio-1.8.1/src/fameio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1470 2023-05-04 07:30:23.000000 fameio-1.8.1/src/fameio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:30:22.000000 fameio-1.8.1/src/fameio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-05-04 07:30:22.000000 fameio-1.8.1/src/fameio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 14:12:00.000000 fameio-1.8.1/src/fameio.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-05-04 07:30:23.000000 fameio-1.8.1/src/fameio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 07:30:23.000000 fameio-1.8.1/src/fameio.egg-info/top_level.txt
```

### Comparing `fameio-1.8/LICENSE.txt` & `fameio-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fameio-1.8/PKG-INFO` & `fameio-1.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: fameio
-Version: 1.8
-Summary: Python scripts for operation of FAME models
-Home-page: https://gitlab.com/fame-framework/fame-io/
-Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
-Author-email: fame@dlr.de
-License: Apache License 2.0
-Keywords: FAME,agent-based modelling
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 <!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
 [![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
@@ -30,30 +12,36 @@
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
 
-    pip install fameio
+We recommend installing `fameio` using PyPI:
 
+    pip install fameio
 
 You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
 
     pipx install fameio
 
+`fameio` is currently developed and tested for Python 3.8 or higher. 
+See the `setup.py` for a complete listing of dependencies. 
 
 # Usage
-FAME-Io currently offers two main scripts "makeFameRunConfig" and "convertFameResults".
+
+FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
 Both are automatically installed with the package.
-The first one creates a protobuf file for FAME applications using YAML definition files and .csv files.
-The latter one reads output files from FAME applications in protobuf format and converts them to .csv files.
+The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
+The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
+
+You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
 
 ## Make a FAME run configuration
-Digests configuration files in YAML format, combines them with .csv data files and creates a single input file for FAME applications in protobuf format.
+Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
 Call structure:
 
     makeFameRunConfig -f <path/to/scenario.yaml>
 
 You may also specify any of the following arguments:
 
 | Command              | Action                                                                                                          |
@@ -85,15 +73,14 @@
               Options.OUTPUT: "output.pb",
               Options.LOG_FILE: "scenario.log",
               }
 
 make_config("path/to/scenario.yaml", run_config)
 ```
 
-
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
 The Schema is used to validate the inputs of the "scenario.yaml".
 Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
@@ -358,22 +345,22 @@
     ProductName: MyThirdProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 ```
 
 ### CSV files
 TIME_SERIES inputs are not directly fed into the Scenario YAML file.
-Instead, TIME_SERIES reference a .csv file that can be stored some place else.
-These .csv files follow a specific structure:
+Instead, TIME_SERIES reference a CSV file that can be stored some place else.
+These CSV files follow a specific structure:
 * They must contain exactly two columns.
 * The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
 * The second column must be a numerical value (either integer or floating-point)
 * The separator of the two columns is a semicolon
 
-Exemplary content of a valid .csv file:
+Exemplary content of a valid CSV file:
 
     2012-01-01_00:00:00;400
     2013-01-01_00:00:00;720.5
     2014-01-01_00:00:00;650
     2015-01-01_00:00:00;99.27772
     2016-01-01_00:00:00;42
     2017-01-01_00:00:00;0.1
@@ -523,15 +510,15 @@
 
 #### Ignoring files
 Files that have their name start with "IGNORE_" are not included with the !include command.
 You will see a debug output to notify you that the file was ignored.
 Use this to temporarily take files out ouf your configuration without deleting or moving them.
 
 ## Read FAME results
-Takes an output file in protobuf format of FAME-based applications and converts it into files in .csv format.
+Takes an output file in protobuf format of FAME-based applications and converts it into files in CSV format.
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
@@ -603,35 +590,48 @@
   title   = {FAME-Io: Configuration tools for complex agent-based simulations},
   journal = {Journal of Open Source Software},
   year    = {2023},
   doi     = {doi: https://doi.org/10.21105/joss.04958}
 }
 ```
 
-## Contribute
+## Available Support
+This is a purely scientific project by (at the moment) one research group. 
+Thus, there is no paid technical support available.
+However, we will give our best to answer your questions and provide support.
+
+If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](#Contribute)).
+For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working together on the code in common projects or towards common publications and thus further develop FAME-Io.
+
+# Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
-## Testing changes locally
+You will also find templates for [bug reports](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/bug_report.md),
+[feature requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/feature_request.md), and 
+[pull requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/pull_request.md).
+
+We kindly ask you to read the Contributors License Agreement `cla.md`, sign it, and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing. Please see our [conventions of contribution](https://gitlab.com/fame-framework/wiki/-/wikis/developers/contribute/Conventions) which are described in the Wiki.
+
+## Testing changes locally 
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters.
+The maximum line length is defined as 120 characters. 
 Therefore, before committing, run `black --line-length 120 .`
 
 ## Pre-Commit hooks
 
 FAME-Io uses several pre-commit hooks to ensure high code quality.
 To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
 
 ```
     pip install fameio[dev]
     pre-commit install -t pre-commit -t pre-push
-```
-
-
+```
```

### Comparing `fameio-1.8/README.md` & `fameio-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: fameio
+Version: 1.8.1
+Summary: Python scripts for operation of FAME models
+Home-page: https://gitlab.com/fame-framework/fame-io/
+Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
+Author-email: fame@dlr.de
+License: Apache License 2.0
+Keywords: FAME,agent-based modelling
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
 <!-- SPDX-FileCopyrightText: 2023 German Aerospace Center <fame@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 [![PyPI version](https://badge.fury.io/py/fameio.svg)](https://badge.fury.io/py/fameio)
 [![JOSS](https://joss.theoj.org/papers/10.21105/joss.04958/status.svg)](https://doi.org/10.21105/joss.04958)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4314337.svg)](https://doi.org/10.5281/zenodo.4314337)
 [![PyPI license](https://img.shields.io/pypi/l/fameio.svg)](https://badge.fury.io/py/fameio)
@@ -12,30 +30,36 @@
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
 
-    pip install fameio
+We recommend installing `fameio` using PyPI:
 
+    pip install fameio
 
 You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
 
     pipx install fameio
 
+`fameio` is currently developed and tested for Python 3.8 or higher. 
+See the `setup.py` for a complete listing of dependencies. 
 
 # Usage
-FAME-Io currently offers two main scripts "makeFameRunConfig" and "convertFameResults".
+
+FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
 Both are automatically installed with the package.
-The first one creates a protobuf file for FAME applications using YAML definition files and .csv files.
-The latter one reads output files from FAME applications in protobuf format and converts them to .csv files.
+The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
+The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
+
+You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
 
 ## Make a FAME run configuration
-Digests configuration files in YAML format, combines them with .csv data files and creates a single input file for FAME applications in protobuf format.
+Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
 Call structure:
 
     makeFameRunConfig -f <path/to/scenario.yaml>
 
 You may also specify any of the following arguments:
 
 | Command              | Action                                                                                                          |
@@ -67,15 +91,14 @@
               Options.OUTPUT: "output.pb",
               Options.LOG_FILE: "scenario.log",
               }
 
 make_config("path/to/scenario.yaml", run_config)
 ```
 
-
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
 The Schema is used to validate the inputs of the "scenario.yaml".
 Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
@@ -340,22 +363,22 @@
     ProductName: MyThirdProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 ```
 
 ### CSV files
 TIME_SERIES inputs are not directly fed into the Scenario YAML file.
-Instead, TIME_SERIES reference a .csv file that can be stored some place else.
-These .csv files follow a specific structure:
+Instead, TIME_SERIES reference a CSV file that can be stored some place else.
+These CSV files follow a specific structure:
 * They must contain exactly two columns.
 * The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
 * The second column must be a numerical value (either integer or floating-point)
 * The separator of the two columns is a semicolon
 
-Exemplary content of a valid .csv file:
+Exemplary content of a valid CSV file:
 
     2012-01-01_00:00:00;400
     2013-01-01_00:00:00;720.5
     2014-01-01_00:00:00;650
     2015-01-01_00:00:00;99.27772
     2016-01-01_00:00:00;42
     2017-01-01_00:00:00;0.1
@@ -505,15 +528,15 @@
 
 #### Ignoring files
 Files that have their name start with "IGNORE_" are not included with the !include command.
 You will see a debug output to notify you that the file was ignored.
 Use this to temporarily take files out ouf your configuration without deleting or moving them.
 
 ## Read FAME results
-Takes an output file in protobuf format of FAME-based applications and converts it into files in .csv format.
+Takes an output file in protobuf format of FAME-based applications and converts it into files in CSV format.
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
@@ -585,33 +608,49 @@
   title   = {FAME-Io: Configuration tools for complex agent-based simulations},
   journal = {Journal of Open Source Software},
   year    = {2023},
   doi     = {doi: https://doi.org/10.21105/joss.04958}
 }
 ```
 
-## Contribute
+## Available Support
+This is a purely scientific project by (at the moment) one research group. 
+Thus, there is no paid technical support available.
+However, we will give our best to answer your questions and provide support.
+
+If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](#Contribute)).
+For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working together on the code in common projects or towards common publications and thus further develop FAME-Io.
+
+# Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
-## Testing changes locally
+You will also find templates for [bug reports](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/bug_report.md),
+[feature requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/feature_request.md), and 
+[pull requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/pull_request.md).
+
+We kindly ask you to read the Contributors License Agreement `cla.md`, sign it, and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing. Please see our [conventions of contribution](https://gitlab.com/fame-framework/wiki/-/wikis/developers/contribute/Conventions) which are described in the Wiki.
+
+## Testing changes locally 
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters.
+The maximum line length is defined as 120 characters. 
 Therefore, before committing, run `black --line-length 120 .`
 
 ## Pre-Commit hooks
 
 FAME-Io uses several pre-commit hooks to ensure high code quality.
 To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
 
 ```
     pip install fameio[dev]
     pre-commit install -t pre-commit -t pre-push
 ```
+
```

### Comparing `fameio-1.8/setup.py` & `fameio-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="fameio",
-    version="1.8",
+    version="1.8.1",
     description="Python scripts for operation of FAME models",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["FAME", "agent-based modelling"],
     url="https://gitlab.com/fame-framework/fame-io/",
     author=", ".join(__author__),
     author_email=__email__,
```

### Comparing `fameio-1.8/src/fameio/scripts/__init__.py` & `fameio-1.8.1/src/fameio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/scripts/convert_results.py` & `fameio-1.8.1/src/fameio/scripts/convert_results.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/scripts/make_config.py` & `fameio-1.8.1/src/fameio/scripts/make_config.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/cli.py` & `fameio-1.8.1/src/fameio/source/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     help_text = "Range of TimeSteps after the `focal-point` they get merged to"
     parser.add_argument("-sa", "--steps-after", required=True, type=non_negative_int, help=help_text)
 
 
 def get_merging_args(args: argparse.Namespace) -> Dict[MergingOptions, int]:
     """Returns a dictionary of GroupingOptions with their values if `time_merging` entry exists"""
     merging_args = {}
-    if "time_merging" in args:
+    if vars(args).get("time_merging"):
         merging_args[MergingOptions.FOCAL_POINT] = args.focal_point
         merging_args[MergingOptions.STEPS_BEFORE] = args.steps_before
         merging_args[MergingOptions.STEPS_AFTER] = args.steps_after
     return merging_args
 
 
 def update_default_config(config: Optional[dict], default: dict) -> dict:
```

### Comparing `fameio-1.8/src/fameio/source/loader.py` & `fameio-1.8.1/src/fameio/source/loader.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/logs.py` & `fameio-1.8.1/src/fameio/source/logs.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/path_resolver.py` & `fameio-1.8.1/src/fameio/source/path_resolver.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/agent_type.py` & `fameio-1.8.1/src/fameio/source/results/agent_type.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/conversion.py` & `fameio-1.8.1/src/fameio/source/results/conversion.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/csv_writer.py` & `fameio-1.8.1/src/fameio/source/results/csv_writer.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/data_transformer.py` & `fameio-1.8.1/src/fameio/source/results/data_transformer.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/output_dao.py` & `fameio-1.8.1/src/fameio/source/results/output_dao.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/results/reader.py` & `fameio-1.8.1/src/fameio/source/results/reader.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/agent.py` & `fameio-1.8.1/src/fameio/source/scenario/agent.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/attribute.py` & `fameio-1.8.1/src/fameio/source/scenario/attribute.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/contract.py` & `fameio-1.8.1/src/fameio/source/scenario/contract.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/exception.py` & `fameio-1.8.1/src/fameio/source/scenario/exception.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/fameiofactory.py` & `fameio-1.8.1/src/fameio/source/scenario/fameiofactory.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/generalproperties.py` & `fameio-1.8.1/src/fameio/source/scenario/generalproperties.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/scenario/scenario.py` & `fameio-1.8.1/src/fameio/source/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/schema/agenttype.py` & `fameio-1.8.1/src/fameio/source/schema/agenttype.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/schema/attribute.py` & `fameio-1.8.1/src/fameio/source/schema/attribute.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/schema/schema.py` & `fameio-1.8.1/src/fameio/source/schema/schema.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/series.py` & `fameio-1.8.1/src/fameio/source/series.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/time.py` & `fameio-1.8.1/src/fameio/source/time.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/tools.py` & `fameio-1.8.1/src/fameio/source/tools.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/validator.py` & `fameio-1.8.1/src/fameio/source/validator.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio/source/writer.py` & `fameio-1.8.1/src/fameio/source/writer.py`

 * *Files identical despite different names*

### Comparing `fameio-1.8/src/fameio.egg-info/PKG-INFO` & `fameio-1.8.1/src/fameio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fameio
-Version: 1.8
+Version: 1.8.1
 Summary: Python scripts for operation of FAME models
 Home-page: https://gitlab.com/fame-framework/fame-io/
 Author: Felix Nitsch, Christoph Schimeczek, Ulrich Frey, Marc Deissenroth-Uhrig, Benjamin Fuchs, A. Achraf El Ghazi
 Author-email: fame@dlr.de
 License: Apache License 2.0
 Keywords: FAME,agent-based modelling
 Platform: UNKNOWN
@@ -30,30 +30,36 @@
 # FAME-Io
 Python scripts for FAME models, generation of protobuf input files and conversion of protobuf output files.
 Please visit the [FAME-Wiki](https://gitlab.com/fame-framework/wiki/-/wikis/home) to get an explanation of FAME and its components.
 The package is also formerly known as [FAME-Py](https://doi.org/10.5281/zenodo.4314338).
 
 # Installation
 
-    pip install fameio
+We recommend installing `fameio` using PyPI:
 
+    pip install fameio
 
 You may also use `pipx`. For detailed information please refer to the official `pipx` [documentation](https://github.com/pypa/pipx).
 
     pipx install fameio
 
+`fameio` is currently developed and tested for Python 3.8 or higher. 
+See the `setup.py` for a complete listing of dependencies. 
 
 # Usage
-FAME-Io currently offers two main scripts "makeFameRunConfig" and "convertFameResults".
+
+FAME-Io currently offers two main scripts `makeFameRunConfig` and `convertFameResults`.
 Both are automatically installed with the package.
-The first one creates a protobuf file for FAME applications using YAML definition files and .csv files.
-The latter one reads output files from FAME applications in protobuf format and converts them to .csv files.
+The first one creates a protobuf file for FAME applications using YAML definition files and CSV files.
+The latter one reads output files from FAME applications in protobuf format and converts them to CSV files.
+
+You may use the [example data](https://gitlab.com/dlr-ve/esy/amiris/examples) provided for the [AMIRIS](https://gitlab.com/dlr-ve/esy/amiris/amiris) model which can be used to simulate electricity markets in [Germany](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Germany2019), [Austria](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Austria2019), and a simple [proof-of-concept model](https://gitlab.com/dlr-ve/esy/amiris/examples/-/tree/main/Simple).
 
 ## Make a FAME run configuration
-Digests configuration files in YAML format, combines them with .csv data files and creates a single input file for FAME applications in protobuf format.
+Digests configuration files in YAML format, combines them with CSV data files and creates a single input file for FAME applications in protobuf format.
 Call structure:
 
     makeFameRunConfig -f <path/to/scenario.yaml>
 
 You may also specify any of the following arguments:
 
 | Command              | Action                                                                                                          |
@@ -85,15 +91,14 @@
               Options.OUTPUT: "output.pb",
               Options.LOG_FILE: "scenario.log",
               }
 
 make_config("path/to/scenario.yaml", run_config)
 ```
 
-
 ### Scenario YAML
 The "scenario.yaml" file contains all configuration options for a FAME-based simulation.
 It consists of the sections `Schema`, `GeneralProperties`, `Agents` and `Contracts`, all of them described below.
 
 #### Schema
 The Schema is used to validate the inputs of the "scenario.yaml".
 Since the Schema should be valid across multiple scenarios, it is recommended to defined it in a separate file and include the file here.
@@ -358,22 +363,22 @@
     ProductName: MyThirdProduct
     FirstDeliveryTime: 100
     DeliveryIntervalInSteps: 3600
 ```
 
 ### CSV files
 TIME_SERIES inputs are not directly fed into the Scenario YAML file.
-Instead, TIME_SERIES reference a .csv file that can be stored some place else.
-These .csv files follow a specific structure:
+Instead, TIME_SERIES reference a CSV file that can be stored some place else.
+These CSV files follow a specific structure:
 * They must contain exactly two columns.
 * The first column must be a time stamp in form `YYYY-MM-DD_hh:mm:ss`
 * The second column must be a numerical value (either integer or floating-point)
 * The separator of the two columns is a semicolon
 
-Exemplary content of a valid .csv file:
+Exemplary content of a valid CSV file:
 
     2012-01-01_00:00:00;400
     2013-01-01_00:00:00;720.5
     2014-01-01_00:00:00;650
     2015-01-01_00:00:00;99.27772
     2016-01-01_00:00:00;42
     2017-01-01_00:00:00;0.1
@@ -523,15 +528,15 @@
 
 #### Ignoring files
 Files that have their name start with "IGNORE_" are not included with the !include command.
 You will see a debug output to notify you that the file was ignored.
 Use this to temporarily take files out ouf your configuration without deleting or moving them.
 
 ## Read FAME results
-Takes an output file in protobuf format of FAME-based applications and converts it into files in .csv format.
+Takes an output file in protobuf format of FAME-based applications and converts it into files in CSV format.
 An individual file for each type of Agent is created in a folder named after the protobuf input file.
 Call structure:
 
     convertFameResults -f <./path/to/protobuf_file.pb>
 
 You may also specify any of the following arguments:
 
@@ -603,35 +608,49 @@
   title   = {FAME-Io: Configuration tools for complex agent-based simulations},
   journal = {Journal of Open Source Software},
   year    = {2023},
   doi     = {doi: https://doi.org/10.21105/joss.04958}
 }
 ```
 
-## Contribute
+## Available Support
+This is a purely scientific project by (at the moment) one research group. 
+Thus, there is no paid technical support available.
+However, we will give our best to answer your questions and provide support.
+
+If you experience any trouble with FAME-Io, you may contact the developers via [fame@dlr.de](mailto:fame@dlr.de).
+Please report bugs and make feature requests by filing issues following the provided templates (see also [Contribute](#Contribute)).
+For substantial enhancements, we recommend that you contact us via [fame@dlr.de](mailto:fame@dlr.de) for working together on the code in common projects or towards common publications and thus further develop FAME-Io.
+
+# Contribute
 Please read the Contributors License Agreement `cla.md`, sign it and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing.
 
-## Testing changes locally
+You will also find templates for [bug reports](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/bug_report.md),
+[feature requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/feature_request.md), and 
+[pull requests](https://gitlab.com/fame-framework/fame-io/-/blob/main/.gitlab/issue_templates/pull_request.md).
+
+We kindly ask you to read the Contributors License Agreement `cla.md`, sign it, and send it to [`fame@dlr.de`](mailto:fame@dlr.de) before contributing. Please see our [conventions of contribution](https://gitlab.com/fame-framework/wiki/-/wikis/developers/contribute/Conventions) which are described in the Wiki.
+
+## Testing changes locally 
 
 Once some changes have been performed on the local git clone, use the following command to override your local installation with your modified copy in order to test the result:
 
 ```bash
 python3 setup.py bdist_wheel && pip3 install --force-reinstall --no-dependencies ./dist/*.whl
 ```
 
 ## Code style
 
 We use the code formatting library [`black`](https://pypi.org/project/black/).
-The maximum line length is defined as 120 characters.
+The maximum line length is defined as 120 characters. 
 Therefore, before committing, run `black --line-length 120 .`
 
 ## Pre-Commit hooks
 
 FAME-Io uses several pre-commit hooks to ensure high code quality.
 To use them, install `dev` packages and then initialise pre-commit in FAME-Io's base folder:
 
 ```
     pip install fameio[dev]
     pre-commit install -t pre-commit -t pre-push
 ```
 
-
```

### Comparing `fameio-1.8/src/fameio.egg-info/SOURCES.txt` & `fameio-1.8.1/src/fameio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

