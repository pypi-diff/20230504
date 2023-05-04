# Comparing `tmp/querynator-0.2.2.tar.gz` & `tmp/querynator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querynator-0.2.2.tar", last modified: Mon Mar 20 09:22:19 2023, max compression
+gzip compressed data, was "querynator-0.3.0.tar", last modified: Thu May  4 14:42:13 2023, max compression
```

## Comparing `querynator-0.2.2.tar` & `querynator-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.830348 querynator-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-20 09:21:49.000000 querynator-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-03-20 09:21:49.000000 querynator-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-20 09:21:49.000000 querynator-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-20 09:21:49.000000 querynator-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-20 09:22:19.830348 querynator-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-20 09:21:49.000000 querynator-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.826348 querynator-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-20 09:21:49.000000 querynator-0.2.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-20 09:21:49.000000 querynator-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.826348 querynator-0.2.2/querynator/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.830348 querynator-0.2.2/querynator/query_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/query_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/query_api/cancertypes.js
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/query_api/cgi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-03-20 09:21:49.000000 querynator-0.2.2/querynator/query_api/civic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.830348 querynator-0.2.2/querynator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 09:21:53.000000 querynator-0.2.2/querynator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-20 09:22:19.000000 querynator-0.2.2/querynator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-20 09:21:49.000000 querynator-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 09:22:19.834348 querynator-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-20 09:21:49.000000 querynator-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:22:19.830348 querynator-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-20 09:21:49.000000 querynator-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-20 09:21:49.000000 querynator-0.2.2/tests/test_querynator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.742014 querynator-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-04 14:41:24.000000 querynator-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-04 14:41:24.000000 querynator-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 14:41:24.000000 querynator-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 14:41:24.000000 querynator-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-04 14:42:13.742014 querynator-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-04 14:41:24.000000 querynator-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-04 14:41:24.000000 querynator-0.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 14:41:24.000000 querynator-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/querynator/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/querynator/helper_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/helper_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/helper_functions/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/querynator/query_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/query_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/query_api/cancertypes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/query_api/cgi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/query_api/civic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/querynator/report_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/combine_cgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/combine_cgi_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/combine_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/create_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-04 14:41:24.000000 querynator-0.3.0/querynator/report_scripts/sort_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/querynator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:41:33.000000 querynator-0.3.0/querynator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 14:42:13.000000 querynator-0.3.0/querynator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 14:41:24.000000 querynator-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:42:13.742014 querynator-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 14:41:24.000000 querynator-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.738014 querynator-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 14:41:24.000000 querynator-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-04 14:41:24.000000 querynator-0.3.0/tests/test_querynator.py
```

### Comparing `querynator-0.2.2/CHANGELOG.rst` & `querynator-0.3.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 ============
 
+0.3.0 - Iron Mercury  (2023-05-04)
+---------------------------------------------
+
+**Added**
+
+* Added functionality to combine the results of the Knowledgebases in an HTML report
+* Added possibility to have non-numerical chromosome columns in the input vcf
+* Added deletion of CGI jobs from CGI Server after completion
+
+**Fixed**
+
+**Dependencies**
+
+**Deprecated**
+
 0.2.2 - Sour Venus  (2023-03-16)
 ---------------------------------------------
 
 **Added**
 
 * Optional VEP annotation based filtering
 * Additional metadata
```

### Comparing `querynator-0.2.2/CONTRIBUTING.rst` & `querynator-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/LICENSE` & `querynator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/PKG-INFO` & `querynator-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,29 @@
 
 
 
 
 Changelog
 ============
 
+0.3.0 - Iron Mercury  (2023-05-04)
+---------------------------------------------
+
+**Added**
+
+* Added functionality to combine the results of the Knowledgebases in an HTML report
+* Added possibility to have non-numerical chromosome columns in the input vcf
+* Added deletion of CGI jobs from CGI Server after completion
+
+**Fixed**
+
+**Dependencies**
+
+**Deprecated**
+
 0.2.2 - Sour Venus  (2023-03-16)
 ---------------------------------------------
 
 **Added**
 
 * Optional VEP annotation based filtering
 * Additional metadata
```

### Comparing `querynator-0.2.2/README.rst` & `querynator-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/docs/Makefile` & `querynator-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/docs/conf.py` & `querynator-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/docs/installation.rst` & `querynator-0.3.0/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 Installation
 ============
 
 
 Stable release
 --------------
 
-To install querynator, run this command in your terminal:
+To install the querynator, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install querynator
 
 This is the preferred method to install querynator, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
+You can also install the querynator using `conda`_:
+
+.. _conda: https://www.anaconda.com/
+
+
+.. code-block:: console
+
+    $ conda install querynator
 
 From sources
 ------------
 
 The sources for querynator can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
```

### Comparing `querynator-0.2.2/docs/make.bat` & `querynator-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/docs/usage.rst` & `querynator-0.3.0/docs/usage.rst`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,37 @@
 
 .. code-block:: bash
 
     querynator --help
     querynator query-api-cgi --help
     querynator query-api-civic --help
 
+VCF Normalization
+**************************************
+We recommend to normalize the input vcf's using `bcftools norm <https://samtools.github.io/bcftools/bcftools.html>`_ before
+running the querynator to unify the input:
+
+The vcf file must be indexed to run ``bcftools norm``, e.g. using `tabix <http://www.htslib.org/doc/tabix.html>`_:
+
+.. code-block:: bash
+
+    tabix /path/to/vcf_file.vcf
+
+Then run ``bcftools norm`` in the following way:
+
+.. code-block:: bash
+
+    bcftools norm \
+        -a \
+        --atom-overlaps . \
+        -f /path/to/reference_file \
+        /path/to/vcf
+
+
+
 
 Query the cancergenomeinterpeter - CGI
 **************************************
 
 A typical command to query the `cancergenomeinterpeter - CGI <https://www.cancergenomeinterpreter.org/home>`_:
 
 .. code-block:: bash
@@ -215,7 +238,56 @@
     |   ├── sample_name.removed_variants.vcf
     ├── sample_name.civic_results.tsv
     └── metadata.txt
 
 .. note::
     When the ``filter_vep`` flag is set a unique Querynator ID is added to the INFO column of each variant in the vcf file.
     The same ID is added to the ``sample_name.civic_results.tsv`` if CIViC is queried.
+
+
+Create an HTML Report
+**************************************
+
+After querying the knowledgebases included in the querynator, it is possible to combine the results into one table
+and to create an HTML report summarizing the most important features of each variant.
+
+
+.. note::
+    This functionality was specifically created to be included into the ``variantMTB`` nextflow pipeline
+    which can be found `here`_. (Currently under development)
+
+.. _here: https://github.com/qbic-pipelines/variantmtb
+
+
+A typical command to create such a report:
+
+.. code-block:: bash
+
+    querynator create-report \
+        --cgi_path path/to/cgi_results \
+        --civic_path path/to/civic_results \
+        --outdir path/to/save/results
+
+The command above generates the following result directory:
+
+.. code-block:: bash
+
+    outdir
+    ├── combined_files
+    |   ├── alterations_vep.tsv
+    |   ├── biomarkers_linked.tsv
+    |   ├── civic_cgi_vep.tsv
+    |   └── civic_vep.tsv
+    ├── report
+    |   |   ├── overall_report.html
+    |   |   ├── variant_reports
+    |   |   |    ├── chr1-1234-A-T.html
+    |   |   |    ├── chr1-1245-C-G.html
+    |   |   |    └── ...
+    |   |   ├── plots
+    |   |   |    ├── kb_upsetplot.png
+    └── └── └──  └── tier_upsetplot.png
+
+
+
+The command creates one overall report which includes some statistics and shows an overview of the most important variants in the project.
+The ``Details`` column in the overall report links directly to a more detailed report on the variant in question.
```

### Comparing `querynator-0.2.2/querynator/__main__.py` & `querynator-0.3.0/querynator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 import click
 import vcf
 from vcf.parser import _Info as VcfInfo
 from vcf.parser import field_counts as vcf_field_counts
 
 import querynator
-from querynator.query_api import (
-    gunzip_compressed_files,
-    gzipped,
-    query_cgi,
-    query_civic,
-    vcf_file,
+from querynator.helper_functions import gunzip_compressed_files, gzipped
+from querynator.query_api import query_cgi, query_civic, vcf_file
+from querynator.report_scripts import (
+    add_tiers_and_scores_to_df,
+    combine_cgi,
+    combine_cgi_civic,
+    combine_civic,
+    create_report_htmls,
 )
 
 # Create logger
 logger = logging.getLogger("Querynator")
 # Create console handler
 ch = logging.StreamHandler()
 # Create formatter
@@ -114,15 +116,15 @@
     # creates dictionary with VEP info names as keys and index in list as columns
     # Name must be VEPs default "CSQ"
     if "CSQ" in in_vcf.infos:
         logger.info("Filtering vcf file")
 
         vep_dict = {name: pos for pos, name in enumerate(in_vcf.infos["CSQ"].desc.split(":")[1].strip().split("|"))}
         """
-        Exemplary for nf-core/sarek (https://nf-co.re/sarek) output 
+        Exemplary for nf-core/sarek (https://nf-co.re/sarek) output
         {'Allele': 0,
         'Consequence': 1,
         'IMPACT': 2,
         'SYMBOL': 3,
         'Gene': 4,
         'Feature_type': 5,
         'Feature': 6,
@@ -229,16 +231,14 @@
     :param vcf_record_list: list of pysam records
     :type vcf_record_list: list
     :param out_name: name for the created vcf file
     :type out_name: str
     :return: None
     :rtype: None
     """
-    if not os.path.isdir("vcf_files"):
-        os.mkdir("vcf_files")
 
     # add querynator_id info to header
     vcf_template.infos["QID"] = VcfInfo("QID", ".", "String", "Querynator ID", ".", ".", ".")
     writer = vcf.Writer(open(f"{out_name}", "w"), vcf_template, lineterminator="\n")
 
     for record in vcf_record_list:
         # add querynator_id to record
@@ -424,16 +424,16 @@
     help="if set, filters out synoymous and low impact variants based on VEP annotation",
     is_flag=True,
     show_default=True,
     default=False,
 )
 def query_api_civic(vcf, outdir, genome, filter_vep):
     try:
-        dirname, basename = os.path.split(outdir)
         result_dir = get_unique_querynator_dir(f"{outdir}")
+        dirname, basename = os.path.split(result_dir)
         if filter_vep:
             in_vcf_header, candidate_variants, removed_variants = filter_vcf_by_vep(vcf, logger)
             # create result directories
             os.makedirs(f"{result_dir}/vcf_files")
             write_vcf(in_vcf_header, removed_variants, f"{result_dir}/vcf_files/{basename}.removed_variants.vcf")
             write_vcf(in_vcf_header, candidate_variants, f"{result_dir}/vcf_files/{basename}.filtered_variants.vcf")
 
@@ -445,9 +445,52 @@
             logger.info("Query the Clinical Interpretations of Variants In Cancer (CIViC)")
             query_civic(vcf, result_dir, logger, vcf, genome, filter_vep)
 
     except FileNotFoundError:
         print("The provided file cannot be found. Please try another path.")
 
 
+# querynator create report
+@querynator_cli.command()
+@click.option(
+    "-c",
+    "--cgi_path",
+    help="Path to a CGI result folder generated using the querynator",
+    required=True,
+    type=click.Path(exists=True),
+)
+@click.option(
+    "-j",
+    "--civic_path",
+    help="Path to a CIViC result folder generated using the querynator",
+    required=True,
+    type=click.Path(exists=True),
+)
+@click.option(
+    "-o",
+    "--outdir",
+    required=True,
+    type=click.STRING,
+    help="Name of new directory in which reports will be stored.",
+)
+def create_report(cgi_path, civic_path, outdir):
+    # create outdir
+    report_dir = get_unique_querynator_dir(outdir)
+    dirname, basename = os.path.split(report_dir)
+    os.makedirs(f"{report_dir}/combined_files")
+    os.makedirs(f"{report_dir}/report/variant_reports")
+    os.makedirs(f"{report_dir}/report/plots")
+
+    # combine the results
+    combine_civic(civic_path, report_dir, logger)
+    combine_cgi(cgi_path, report_dir, logger)
+    combine_cgi_civic(report_dir, logger)
+
+    # add tiers & ranking-score to merged results
+    add_tiers_and_scores_to_df(report_dir, logger)
+
+    # create report
+    create_report_htmls(report_dir, basename, civic_path, logger)
+
+
 if __name__ == "__main__":
     run_querynator()
```

### Comparing `querynator-0.2.2/querynator/query_api/cancertypes.js` & `querynator-0.3.0/querynator/query_api/cancertypes.js`

 * *Files identical despite different names*

### Comparing `querynator-0.2.2/querynator/query_api/cgi_api.py` & `querynator-0.3.0/querynator/query_api/cgi_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,44 +14,15 @@
 
 import click
 import httplib2 as http
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
-
-def gzipped(file_path):
-    """
-    Helper function to test if given vcf is gzipped.
-    If so, the first 2 bytes are "1f 8b"
-
-    :param file_path: Path to gzipped input file
-    :type file_path: str
-    """
-    with open(file_path, "rb") as test_f:
-        return test_f.read(2) == b"\x1f\x8b"
-
-
-def gunzip_compressed_files(file_path, logger):
-    """
-    gunzips gzipped vcf file
-
-    :param file_path: Path to gzipped input file
-    :type file_path: str
-    """
-    logger.info(f"Unzipping input file ({os.path.basename(os.path.normpath(file_path))})")
-
-    if not file_path.endswith(".gz"):
-        logger.error("Given file does not end with '.gz'")
-        exit(1)
-    else:
-        with gzip.open(file_path, "rb") as f_in:
-            with open(file_path[: -len(".gz")], "wb") as f_out:
-                shutil.copyfileobj(f_in, f_out)
-        return file_path[: -len(".gz")]
+from querynator.helper_functions import gunzip_compressed_files, gzipped
 
 
 def hg_assembly(genome):
     """
     Use correct assembly name
 
     :param genome: Genome build version, defaults to hg38
@@ -195,15 +166,40 @@
         r = requests.get(url, headers=headers, params=payload)
         r.raise_for_status()
         with open(output + ".cgi_results.zip", "wb") as fd:
             fd.write(r._content)
     except requests.exceptions.HTTPError as err:
         raise SystemExit(err)
     except Exception:
-        logger.exception("Ooops, sth went wrong with the download. Sorry for the inconvenience.")
+        logger.exception("An unexpected error has occured during the download." + type(err))
+
+
+def delete_job_cgi(url, headers, output, logger):
+    """
+    Delete query from the CGI server after analysis is complete
+
+    :param url: API url with job_id
+    :type url: str
+    :param headers: Valid headers for API query
+    :type headers: dict
+    :param output: sample name
+    :type output: str
+    :raises: Exception
+
+    """
+    try:
+        payload = {"action": "download"}
+        r = requests.delete(url, headers=headers)
+        r.raise_for_status()
+    except requests.exceptions.HTTPError as err:
+        raise SystemExit(err)
+    except Exception:
+        logger.exception(
+            "Deleting the job from the CGI Server was not successful. If this happens more often, please login to the website and remove old jobs or you will not be able to make more queries with your account."
+        )
 
 
 def add_cgi_metadata(url, output, original_input, genome, filter_vep):
     """
     Attach metadata to cgi query
 
     :param url: API url with job_id
@@ -269,7 +265,8 @@
     )
     done = status_done(url, headers, logger)
     logger.info("CGI Query finished")
     if done:
         logger.info("Downloading CGI results")
         download_cgi(url, headers, output, logger)
         add_cgi_metadata(url, output, original_input, genome, filter_vep)
+        delete_job_cgi(url, headers, output, logger)
```

### Comparing `querynator-0.2.2/querynator/query_api/civic_api.py` & `querynator-0.3.0/querynator/query_api/civic_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Query the Clinical Interpretations of Variants In Cancer (CIViC) API via its python tool CIViCPY"""
+""" Query the Clinical Interpretations of Variants In Cancer (CIViC) API via its python tool CIViCPY """
 
 import warnings
 
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 import os
 import random
@@ -10,15 +10,19 @@
 
 import civicpy
 import numpy as np
 import pandas as pd
 import vcf
 from civicpy import civic
 
-from querynator.query_api import gunzip_compressed_files, gzipped
+from querynator.helper_functions import (
+    get_num_from_chr,
+    gunzip_compressed_files,
+    gzipped,
+)
 
 # load the civic cache (necessary for bulk run)
 civic.load_cache()
 
 
 def check_vcf_input(vcf_path, logger):
     """
@@ -95,43 +99,43 @@
             querynator_id = random.randint(1000000, 9999999)
         for alt_base in record.ALT:
             # INSERTION
             if len(record.REF) < len(alt_base):
                 coord_dict.update(
                     {
                         civic.CoordinateQuery(
-                            chr=str(record.CHROM),
+                            chr=get_num_from_chr(record.CHROM),
                             start=int(record.start) + 1,
                             stop=int(record.start) + 2,
                             alt=str(alt_base)[1:],
                             ref="",
                             build=build,
                         ): querynator_id
                     }
                 )
             # DELETION
             elif len(record.REF) > len(alt_base) and len(alt_base) == 1:
                 coord_dict.update(
                     {
                         civic.CoordinateQuery(
-                            chr=str(record.CHROM),
+                            chr=get_num_from_chr(record.CHROM),
                             start=int(record.start) + 1,
                             stop=int(record.end),
                             alt="",
                             ref=record.REF,
                             build=build,
                         ): querynator_id
                     }
                 )
             # SNPs, DelIns
             else:
                 coord_dict.update(
                     {
                         civic.CoordinateQuery(
-                            chr=str(record.CHROM),
+                            chr=get_num_from_chr(record.CHROM),
                             start=int(record.start) + 1,
                             stop=int(record.end),
                             alt=str(alt_base),
                             ref=record.REF,
                             build=build,
                         ): querynator_id
                     }
@@ -162,19 +166,16 @@
     else:
         input_dict = coord_dict
 
     # actual search for each variant
     variant_list = []
     for coord_obj, querynator_id in input_dict.items():
         variant = civic.search_variants_by_coordinates(coord_obj, search_mode="exact")
-        # variant is None and the program stops executing when the wrong build was chosen.
-        if variant == None:
-            logger.error("Variant was None. Did you choose the correct reference genome?")
-            exit(1)
-        if len(variant) > 0:
+
+        if variant != None and len(variant) > 0:
             for variant_obj in variant:
                 variant_list.append([{coord_obj: querynator_id}, [variant_obj]])
 
     # break if no variants are found
     if variant_list == None:
         logger.error("No hits are found in CIViC for this vcf file")
         exit(1)
@@ -269,15 +270,15 @@
             "assertion_phenotypes": ", ".join([i.name for i in assertion.phenotypes]),
             "assertion_significance": assertion.significance,
             "assertion_status": assertion.status,
             "assertion_summary": assertion.summary,
             "assertion_therapies_name": ", ".join([i.name for i in assertion.therapies]),
             "assertion_therapies_ncit_id": ", ".join([i.ncit_id for i in assertion.therapies]),
             "assertion_therapies_aliases": ", ".join([", ".join(i.aliases) for i in assertion.therapies]),
-            "assertion_therapy_interaction_type": assertion.therapy_interaction_type,
+            "assertion_therapies_interaction_type": assertion.therapy_interaction_type,
             "assertion_variant_origin": assertion.variant_origin,
         }
     except IndexError:
         assertion_dict = {
             "assertion_name": np.nan,
             "assertion_acmg_codes": np.nan,
             "assertion_acmg_codes_description": np.nan,
@@ -289,18 +290,18 @@
             "assertion_disease_doid": np.nan,
             "assertion_disease_url": np.nan,
             "assertion_disease_aliases": np.nan,
             "assertion_phenotypes": np.nan,
             "assertion_significance": np.nan,
             "assertion_status": np.nan,
             "assertion_summary": np.nan,
-            "assertion_therapies": np.nan,
+            "assertion_therapies_name": np.nan,
             "assertion_therapies_ncit_id": np.nan,
             "assertion_therapies_aliases": np.nan,
-            "assertion_therapy_interaction_type": np.nan,
+            "assertion_therapies_interaction_type": np.nan,
             "assertion_variant_origin": np.nan,
         }
     return assertion_dict
 
 
 def get_evidence_information_from_variant(variant_obj):
     """
@@ -438,19 +439,41 @@
     :type coord_list: list
     :return: sorted coordinates
     :rtype: list
     """
     return {
         key: value
         for key, value in sorted(
-            coord_dict.items(), key=lambda x: (int(x[0][0]) if x[0][0] != "X" else np.inf, x[0][1], x[0][2])
+            coord_dict.items(),
+            key=lambda x: (
+                int(x[0][0]) if x[0][0] != "X" and x[0][0] != "Y" and x[0][0] != "M" else sort_rules(x[0][0]),
+                x[0][1],
+                x[0][2],
+            ),
         )
     }
 
 
+def sort_rules(s):
+    """
+    Set rules to correctly sort chromosomes X,Y,M
+
+    :param s: "string" chromosome (X,Y,M)
+    :type s: str
+    :return: integer to sort by
+    :rtype: int
+    """
+    if s == "X":
+        return 100
+    elif s == "Y":
+        return 1000
+    elif s == "M":
+        return 10000
+
+
 def add_civic_metadata(out_path, input_file, search_mode, genome, filter_vep):
     """
     Attach metadata to civic query
 
     :param out_path: Name of directory in which results are stored
     :type out_path: str
     :param input_file: path of original input file
```

### Comparing `querynator-0.2.2/querynator.egg-info/PKG-INFO` & `querynator-0.3.0/querynator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,29 @@
 
 
 
 
 Changelog
 ============
 
+0.3.0 - Iron Mercury  (2023-05-04)
+---------------------------------------------
+
+**Added**
+
+* Added functionality to combine the results of the Knowledgebases in an HTML report
+* Added possibility to have non-numerical chromosome columns in the input vcf
+* Added deletion of CGI jobs from CGI Server after completion
+
+**Fixed**
+
+**Dependencies**
+
+**Deprecated**
+
 0.2.2 - Sour Venus  (2023-03-16)
 ---------------------------------------------
 
 **Added**
 
 * Optional VEP annotation based filtering
 * Additional metadata
```

### Comparing `querynator-0.2.2/querynator.egg-info/SOURCES.txt` & `querynator-0.3.0/querynator.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,13 +21,21 @@
 querynator.egg-info/PKG-INFO
 querynator.egg-info/SOURCES.txt
 querynator.egg-info/dependency_links.txt
 querynator.egg-info/entry_points.txt
 querynator.egg-info/not-zip-safe
 querynator.egg-info/requires.txt
 querynator.egg-info/top_level.txt
+querynator/helper_functions/__init__.py
+querynator/helper_functions/helper_functions.py
 querynator/query_api/__init__.py
 querynator/query_api/cancertypes.js
 querynator/query_api/cgi_api.py
 querynator/query_api/civic_api.py
+querynator/report_scripts/__init__.py
+querynator/report_scripts/combine_cgi.py
+querynator/report_scripts/combine_cgi_civic.py
+querynator/report_scripts/combine_civic.py
+querynator/report_scripts/create_report.py
+querynator/report_scripts/sort_variants.py
 tests/__init__.py
 tests/test_querynator.py
```

### Comparing `querynator-0.2.2/setup.py` & `querynator-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     include_package_data=True,
     keywords="querynator",
     name="querynator",
     packages=find_packages(exclude=("docs")),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/qbic-pipelines/querynator",
-    version="0.2.2",
+    version="0.3.0",
     zip_safe=False,
 )
```

### Comparing `querynator-0.2.2/tests/test_querynator.py` & `querynator-0.3.0/tests/test_querynator.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     assert "--help                          Show this message and exit." in cgi_help_result.output
 
     """Test CIVIC help message"""
     civic_help_result = runner.invoke(querynator.__main__.querynator_cli, ["query-api-civic", "--help"])
     assert civic_help_result.exit_code == 0
     assert "--help                          Show this message and exit." in civic_help_result.output
 
+    """Test CREATE-REPORT help message"""
+    civic_help_result = runner.invoke(querynator.__main__.querynator_cli, ["create-report", "--help"])
+    assert civic_help_result.exit_code == 0
+    assert "--help                 Show this message and exit." in civic_help_result.output
+
     """Test non-existing subcommand"""
     result = runner.invoke(querynator.__main__.querynator_cli, ["query-api-clinvar"])
     assert result.exit_code == 2
     assert "No such command" in result.output
 
     """Test non-existing option"""
     result = runner.invoke(querynator.__main__.querynator_cli, ["query-api-cgi", "--baz"])
```

