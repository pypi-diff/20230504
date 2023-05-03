# Comparing `tmp/terminal_tracker-0.1.0.tar.gz` & `tmp/terminal_tracker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_tracker-0.1.0.tar", last modified: Thu Mar 23 23:53:45 2023, max compression
+gzip compressed data, was "terminal_tracker-1.0.0.tar", last modified: Wed May  3 23:11:14 2023, max compression
```

## Comparing `terminal_tracker-0.1.0.tar` & `terminal_tracker-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,57 @@
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.591038 terminal_tracker-0.1.0/
--rw-r--r--   0 miloniatal   (501) staff       (20)      401 2023-03-23 23:42:30.000000 terminal_tracker-0.1.0/.bumpversion.cfg
--rw-r--r--   0 miloniatal   (501) staff       (20)       25 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/.coveragerc
--rw-r--r--   0 miloniatal   (501) staff       (20)     1319 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 miloniatal   (501) staff       (20)     1068 2023-02-15 16:49:03.000000 terminal_tracker-0.1.0/LICENSE
--rw-r--r--   0 miloniatal   (501) staff       (20)      406 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/MANIFEST.in
--rw-r--r--   0 miloniatal   (501) staff       (20)     2287 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/Makefile
--rw-r--r--   0 miloniatal   (501) staff       (20)     4700 2023-03-23 23:53:45.590873 terminal_tracker-0.1.0/PKG-INFO
--rw-r--r--   0 miloniatal   (501) staff       (20)     2618 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/README.md
--rw-r--r--   0 miloniatal   (501) staff       (20)     2213 2023-03-23 23:42:30.000000 terminal_tracker-0.1.0/pyproject.toml
--rw-r--r--   0 miloniatal   (501) staff       (20)       38 2023-03-23 23:53:45.591465 terminal_tracker-0.1.0/setup.cfg
--rw-r--r--   0 miloniatal   (501) staff       (20)       56 2023-03-23 23:42:30.000000 terminal_tracker-0.1.0/setup.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.585947 terminal_tracker-0.1.0/terminal_tracker/
--rw-r--r--   0 miloniatal   (501) staff       (20)      118 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/__init__.py
--rw-r--r--   0 miloniatal   (501) staff       (20)       45 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/__main__.py
--rw-r--r--   0 miloniatal   (501) staff       (20)       22 2023-03-23 23:42:30.000000 terminal_tracker-0.1.0/terminal_tracker/_version.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.587076 terminal_tracker-0.1.0/terminal_tracker/configs/
--rw-r--r--   0 miloniatal   (501) staff       (20)      466 2023-02-17 18:38:31.000000 terminal_tracker-0.1.0/terminal_tracker/configs/configuring_bash.sh
--rw-r--r--   0 miloniatal   (501) staff       (20)      291 2023-02-18 20:35:46.000000 terminal_tracker-0.1.0/terminal_tracker/configs/configuring_zsh.sh
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.588796 terminal_tracker-0.1.0/terminal_tracker/history_files/
--rw-r--r--   0 miloniatal   (501) staff       (20)     1973 2023-02-17 18:38:31.000000 terminal_tracker-0.1.0/terminal_tracker/history_files/bash_history.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)     2322 2023-02-18 20:35:46.000000 terminal_tracker-0.1.0/terminal_tracker/history_files/bash_history_timeframe.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)       97 2023-02-17 18:38:31.000000 terminal_tracker-0.1.0/terminal_tracker/history_files/storing_histfiles.sh
--rw-r--r--   0 miloniatal   (501) staff       (20)    33635 2023-02-18 20:35:46.000000 terminal_tracker-0.1.0/terminal_tracker/history_files/zsh_history.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)    15417 2023-02-18 20:35:46.000000 terminal_tracker-0.1.0/terminal_tracker/history_files/zsh_history_timeframe.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)     8866 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/searching.py
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.590016 terminal_tracker-0.1.0/terminal_tracker/tests/
--rw-r--r--   0 miloniatal   (501) staff       (20)     1312 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/tests/test_integration.py
--rw-r--r--   0 miloniatal   (501) staff       (20)    11453 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/tests/test_unit.py
--rw-r--r--   0 miloniatal   (501) staff       (20)      286 2023-03-23 23:29:05.000000 terminal_tracker-0.1.0/terminal_tracker/tests/zsh_test.txt
-drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-03-23 23:53:45.586723 terminal_tracker-0.1.0/terminal_tracker.egg-info/
--rw-r--r--   0 miloniatal   (501) staff       (20)     4700 2023-03-23 23:53:45.000000 terminal_tracker-0.1.0/terminal_tracker.egg-info/PKG-INFO
--rw-r--r--   0 miloniatal   (501) staff       (20)      889 2023-03-23 23:53:45.000000 terminal_tracker-0.1.0/terminal_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)        1 2023-03-23 23:53:45.000000 terminal_tracker-0.1.0/terminal_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)      168 2023-03-23 23:53:45.000000 terminal_tracker-0.1.0/terminal_tracker.egg-info/requires.txt
--rw-r--r--   0 miloniatal   (501) staff       (20)       17 2023-03-23 23:53:45.000000 terminal_tracker-0.1.0/terminal_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.358312 terminal_tracker-1.0.0/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      401 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/.bumpversion.cfg
+-rw-r--r--   0 miloniatal   (501) staff       (20)       25 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/.coveragerc
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1319 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1068 2023-02-15 16:49:03.000000 terminal_tracker-1.0.0/LICENSE
+-rw-r--r--   0 miloniatal   (501) staff       (20)      552 2023-04-10 18:45:13.000000 terminal_tracker-1.0.0/MANIFEST.in
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2623 2023-04-04 22:56:49.000000 terminal_tracker-1.0.0/Makefile
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4955 2023-05-03 23:11:14.358077 terminal_tracker-1.0.0/PKG-INFO
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2893 2023-05-03 22:46:36.000000 terminal_tracker-1.0.0/README.md
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.344465 terminal_tracker-1.0.0/docs/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      634 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/Makefile
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1653 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/conf.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1818 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/examples.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2250 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/index.md
+-rw-r--r--   0 miloniatal   (501) staff       (20)      765 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/make.bat
+-rw-r--r--   0 miloniatal   (501) staff       (20)       85 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/modules.rst
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1195 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/docs/terminal_tracker.rst
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2277 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/pyproject.toml
+-rw-r--r--   0 miloniatal   (501) staff       (20)       38 2023-05-03 23:11:14.358374 terminal_tracker-1.0.0/setup.cfg
+-rw-r--r--   0 miloniatal   (501) staff       (20)       56 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/setup.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.347124 terminal_tracker-1.0.0/terminal_tracker/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      231 2023-05-03 22:40:48.000000 terminal_tracker-1.0.0/terminal_tracker/__init__.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)       45 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/terminal_tracker/__main__.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)       22 2023-05-03 23:00:34.000000 terminal_tracker-1.0.0/terminal_tracker/_version.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.348758 terminal_tracker-1.0.0/terminal_tracker/configs/
+-rw-r--r--   0 miloniatal   (501) staff       (20)      466 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/configs/configuring_bash.sh
+-rw-r--r--   0 miloniatal   (501) staff       (20)      291 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/configs/configuring_zsh.sh
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.350397 terminal_tracker-1.0.0/terminal_tracker/examples/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4707 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/Frequency.ipynb
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2346 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/Searching.ipynb
+-rw-r--r--   0 miloniatal   (501) staff       (20)    13832 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/examples/TagTime.ipynb
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4657 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/export.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4502 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/frequency.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.356273 terminal_tracker-1.0.0/terminal_tracker/history_files/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1973 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2322 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history_timeframe.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)       97 2023-02-17 18:38:31.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/storing_histfiles.sh
+-rw-r--r--   0 miloniatal   (501) staff       (20)    33635 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)    15417 2023-02-18 20:35:46.000000 terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history_timeframe.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4416 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/preprocess.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1487 2023-05-03 22:40:48.000000 terminal_tracker-1.0.0/terminal_tracker/searching.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1298 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tag.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.357569 terminal_tracker-1.0.0/terminal_tracker/tests/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4976 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_export.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4746 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_frequency.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     3576 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_preprocess.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1836 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_searching.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)      520 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_tag.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)     2233 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/tests/test_timeanalysis.py
+-rw-r--r--   0 miloniatal   (501) staff       (20)      286 2023-03-23 23:29:05.000000 terminal_tracker-1.0.0/terminal_tracker/tests/zsh_test.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1177 2023-05-03 22:41:16.000000 terminal_tracker-1.0.0/terminal_tracker/timeanalysis.py
+drwxr-xr-x   0 miloniatal   (501) staff       (20)        0 2023-05-03 23:11:14.348299 terminal_tracker-1.0.0/terminal_tracker.egg-info/
+-rw-r--r--   0 miloniatal   (501) staff       (20)     4955 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 miloniatal   (501) staff       (20)     1435 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)        1 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)      211 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/requires.txt
+-rw-r--r--   0 miloniatal   (501) staff       (20)       17 2023-05-03 23:11:14.000000 terminal_tracker-1.0.0/terminal_tracker.egg-info/top_level.txt
```

### Comparing `terminal_tracker-0.1.0/CONTRIBUTING.md` & `terminal_tracker-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/LICENSE` & `terminal_tracker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/Makefile` & `terminal_tracker-1.0.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -92,7 +92,23 @@
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
 .PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+
+docs: 
+	make -C docs/ clean
+	make -C docs/ html
+
+TMPREPO=/tmp/docs/terminal-tracker
+
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages git@github.com:MiloniAtal/terminal-tracker.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
```

### Comparing `terminal_tracker-0.1.0/PKG-INFO` & `terminal_tracker-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_tracker
-Version: 0.1.0
+Version: 1.0.0
 Summary: Terminal command tracker
 Author-email: Miloni <miloniatal@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Miloni Atal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,14 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/columbiaoss/example-project-python
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,40 +44,42 @@
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
 ![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
-
+[![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
+[![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
+    
 ## Overview
 
 This tools helps with analysing, filtering and segregrating your command history. It also provides functions to support storing of this history in a better format, that can be used share with people or used in future. It recommends commands (based of length of command and frequency of use) that should have an alias. 
 
 ## Main features
 - Recommends commands that should have an alias. 
 - It provides support for both zsh and bash shells. 
 - Nice format to store and share history
 
 ## Installing
 
 ```
-pip install terminal_tracker
+pip install terminal-tracker
 ```
 
 ## Dependencies
 
 - pandas
 - pytz
 
 ## Usage
 
 ```
 from terminal_tracker import FrequencyFile
-ff = FrequencyFile("zsh_history_file.txt", time=False, shell="zsh")
+ff = FrequencyFile("zsh_history_file.txt", timeframe=False, shell="zsh")
 most_frequent_command = ff.find_most_frequent()
 
 ```
 
 ## Configurations
 
 These congifurations will help you to better store your history:
@@ -119,9 +120,7 @@
 make coverage
 make test
 ``` 
 
 ## Contributing to terminal_tracker
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
-
-
```

### Comparing `terminal_tracker-0.1.0/README.md` & `terminal_tracker-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
 ![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
-
+[![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
+[![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
+    
 ## Overview
 
 This tools helps with analysing, filtering and segregrating your command history. It also provides functions to support storing of this history in a better format, that can be used share with people or used in future. It recommends commands (based of length of command and frequency of use) that should have an alias. 
 
 ## Main features
 - Recommends commands that should have an alias. 
 - It provides support for both zsh and bash shells. 
 - Nice format to store and share history
 
 ## Installing
 
 ```
-pip install terminal_tracker
+pip install terminal-tracker
 ```
 
 ## Dependencies
 
 - pandas
 - pytz
 
 ## Usage
 
 ```
 from terminal_tracker import FrequencyFile
-ff = FrequencyFile("zsh_history_file.txt", time=False, shell="zsh")
+ff = FrequencyFile("zsh_history_file.txt", timeframe=False, shell="zsh")
 most_frequent_command = ff.find_most_frequent()
 
 ```
 
 ## Configurations
 
 These congifurations will help you to better store your history:
```

### Comparing `terminal_tracker-0.1.0/pyproject.toml` & `terminal_tracker-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "terminal_tracker"
 authors = [{name = "Miloni", email = "miloniatal@gmail.com"}]
 description="Terminal command tracker"
 readme = "README.md"
-version="0.1.0"
+version="1.0.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -45,15 +45,18 @@
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
     "pandas",
-    "pytz"
+    "pytz",
+    "sphinx",
+    "recommonmark",
+    "sphinxcontrib-napoleon"
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

### Comparing `terminal_tracker-0.1.0/terminal_tracker/history_files/bash_history.txt` & `terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/terminal_tracker/history_files/bash_history_timeframe.txt` & `terminal_tracker-1.0.0/terminal_tracker/history_files/bash_history_timeframe.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/terminal_tracker/history_files/zsh_history.txt` & `terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/terminal_tracker/history_files/zsh_history_timeframe.txt` & `terminal_tracker-1.0.0/terminal_tracker/history_files/zsh_history_timeframe.txt`

 * *Files identical despite different names*

### Comparing `terminal_tracker-0.1.0/terminal_tracker.egg-info/PKG-INFO` & `terminal_tracker-1.0.0/terminal_tracker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-tracker
-Version: 0.1.0
+Version: 1.0.0
 Summary: Terminal command tracker
 Author-email: Miloni <miloniatal@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Miloni Atal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,14 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/columbiaoss/example-project-python
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,40 +44,42 @@
 
 Maintaining and organizing a history of terminal commands executed for a folder/project from any terminal.
 
 ![](https://img.shields.io/github/license/MiloniAtal/terminal-tracker)
 ![](https://img.shields.io/github/issues/MiloniAtal/terminal-tracker)
 [![Build Status](https://github.com/MiloniAtal/terminal-tracker/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/MiloniAtal/terminal-tracker/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/MiloniAtal/terminal-tracker/branch/main/graph/badge.svg)](https://codecov.io/gh/MiloniAtal/terminal-tracker)
-
+[![PyPI](https://img.shields.io/pypi/v/terminal-tracker)](https://pypi.org/project/terminal-tracker/)
+[![Documentation Status](https://readthedocs.org/projects/terminal-tracker/badge/?version=latest)](https://terminal-tracker.readthedocs.io/en/latest/?badge=latest)
+    
 ## Overview
 
 This tools helps with analysing, filtering and segregrating your command history. It also provides functions to support storing of this history in a better format, that can be used share with people or used in future. It recommends commands (based of length of command and frequency of use) that should have an alias. 
 
 ## Main features
 - Recommends commands that should have an alias. 
 - It provides support for both zsh and bash shells. 
 - Nice format to store and share history
 
 ## Installing
 
 ```
-pip install terminal_tracker
+pip install terminal-tracker
 ```
 
 ## Dependencies
 
 - pandas
 - pytz
 
 ## Usage
 
 ```
 from terminal_tracker import FrequencyFile
-ff = FrequencyFile("zsh_history_file.txt", time=False, shell="zsh")
+ff = FrequencyFile("zsh_history_file.txt", timeframe=False, shell="zsh")
 most_frequent_command = ff.find_most_frequent()
 
 ```
 
 ## Configurations
 
 These congifurations will help you to better store your history:
@@ -119,9 +120,7 @@
 make coverage
 make test
 ``` 
 
 ## Contributing to terminal_tracker
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
-
-
```

