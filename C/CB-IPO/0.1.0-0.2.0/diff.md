# Comparing `tmp/CB_IPO-0.1.0.tar.gz` & `tmp/CB_IPO-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CB_IPO-0.1.0.tar", last modified: Mon Mar 27 02:57:32 2023, max compression
+gzip compressed data, was "CB_IPO-0.2.0.tar", last modified: Thu May  4 20:59:35 2023, max compression
```

## Comparing `CB_IPO-0.1.0.tar` & `CB_IPO-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,40 @@
-drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-03-27 02:57:32.648665 CB_IPO-0.1.0/
--rw-r--r--   0 leonwu     (501) staff       (20)      392 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/.bumpversion.cfg
-drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-03-27 02:57:32.647409 CB_IPO-0.1.0/CB_IPO/
--rw-r--r--   0 leonwu     (501) staff       (20)     5526 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/CB_IPO/CB_IPO.py
--rw-r--r--   0 leonwu     (501) staff       (20)       56 2023-03-25 03:03:11.000000 CB_IPO-0.1.0/CB_IPO/__init__.py
--rw-r--r--   0 leonwu     (501) staff       (20)       70 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/CB_IPO/__main__.py
--rw-r--r--   0 leonwu     (501) staff       (20)       22 2023-03-27 02:27:33.000000 CB_IPO-0.1.0/CB_IPO/_version.py
-drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-03-27 02:57:32.648280 CB_IPO-0.1.0/CB_IPO/tests/
--rw-r--r--   0 leonwu     (501) staff       (20)     5337 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/CB_IPO/tests/test_all.py
-drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-03-27 02:57:32.648107 CB_IPO-0.1.0/CB_IPO.egg-info/
--rw-r--r--   0 leonwu     (501) staff       (20)    16628 2023-03-27 02:57:32.000000 CB_IPO-0.1.0/CB_IPO.egg-info/PKG-INFO
--rw-r--r--   0 leonwu     (501) staff       (20)      343 2023-03-27 02:57:32.000000 CB_IPO-0.1.0/CB_IPO.egg-info/SOURCES.txt
--rw-r--r--   0 leonwu     (501) staff       (20)        1 2023-03-27 02:57:32.000000 CB_IPO-0.1.0/CB_IPO.egg-info/dependency_links.txt
--rw-r--r--   0 leonwu     (501) staff       (20)      156 2023-03-27 02:57:32.000000 CB_IPO-0.1.0/CB_IPO.egg-info/requires.txt
--rw-r--r--   0 leonwu     (501) staff       (20)        7 2023-03-27 02:57:32.000000 CB_IPO-0.1.0/CB_IPO.egg-info/top_level.txt
--rw-r--r--   0 leonwu     (501) staff       (20)      939 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 leonwu     (501) staff       (20)    11357 2023-02-19 16:05:29.000000 CB_IPO-0.1.0/LICENSE
--rw-r--r--   0 leonwu     (501) staff       (20)      376 2023-03-25 03:03:11.000000 CB_IPO-0.1.0/MANIFEST.in
--rw-r--r--   0 leonwu     (501) staff       (20)     2346 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/Makefile
--rw-r--r--   0 leonwu     (501) staff       (20)    16628 2023-03-27 02:57:32.648523 CB_IPO-0.1.0/PKG-INFO
--rw-r--r--   0 leonwu     (501) staff       (20)     2840 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/README.md
--rw-r--r--   0 leonwu     (501) staff       (20)     2172 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/pyproject.toml
--rw-r--r--   0 leonwu     (501) staff       (20)       38 2023-03-27 02:57:32.648705 CB_IPO-0.1.0/setup.cfg
--rw-r--r--   0 leonwu     (501) staff       (20)       38 2023-03-27 02:52:33.000000 CB_IPO-0.1.0/setup.py
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.723170 CB_IPO-0.2.0/
+-rw-r--r--   0 leonwu     (501) staff       (20)      392 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/.bumpversion.cfg
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.719017 CB_IPO-0.2.0/CB_IPO/
+-rw-r--r--   0 leonwu     (501) staff       (20)    15225 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/CB_IPO/CB_IPO.py
+-rw-r--r--   0 leonwu     (501) staff       (20)       56 2023-03-25 03:03:11.000000 CB_IPO-0.2.0/CB_IPO/__init__.py
+-rw-r--r--   0 leonwu     (501) staff       (20)       70 2023-03-27 02:52:33.000000 CB_IPO-0.2.0/CB_IPO/__main__.py
+-rw-r--r--   0 leonwu     (501) staff       (20)       22 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/CB_IPO/_version.py
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.719932 CB_IPO-0.2.0/CB_IPO/tests/
+-rw-r--r--   0 leonwu     (501) staff       (20)    15818 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/CB_IPO/tests/test_all.py
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.719790 CB_IPO-0.2.0/CB_IPO.egg-info/
+-rw-r--r--   0 leonwu     (501) staff       (20)    18192 2023-05-04 20:59:35.000000 CB_IPO-0.2.0/CB_IPO.egg-info/PKG-INFO
+-rw-r--r--   0 leonwu     (501) staff       (20)      583 2023-05-04 20:59:35.000000 CB_IPO-0.2.0/CB_IPO.egg-info/SOURCES.txt
+-rw-r--r--   0 leonwu     (501) staff       (20)        1 2023-05-04 20:59:35.000000 CB_IPO-0.2.0/CB_IPO.egg-info/dependency_links.txt
+-rw-r--r--   0 leonwu     (501) staff       (20)      156 2023-05-04 20:59:35.000000 CB_IPO-0.2.0/CB_IPO.egg-info/requires.txt
+-rw-r--r--   0 leonwu     (501) staff       (20)        7 2023-05-04 20:59:35.000000 CB_IPO-0.2.0/CB_IPO.egg-info/top_level.txt
+-rw-r--r--   0 leonwu     (501) staff       (20)      939 2023-03-27 02:52:33.000000 CB_IPO-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 leonwu     (501) staff       (20)    11357 2023-02-19 16:05:29.000000 CB_IPO-0.2.0/LICENSE
+-rw-r--r--   0 leonwu     (501) staff       (20)      527 2023-05-03 20:19:40.000000 CB_IPO-0.2.0/MANIFEST.in
+-rw-r--r--   0 leonwu     (501) staff       (20)     2690 2023-05-03 21:19:48.000000 CB_IPO-0.2.0/Makefile
+-rw-r--r--   0 leonwu     (501) staff       (20)    18192 2023-05-04 20:59:35.722712 CB_IPO-0.2.0/PKG-INFO
+-rw-r--r--   0 leonwu     (501) staff       (20)     4424 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/README.md
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.722062 CB_IPO-0.2.0/docs/
+-rw-r--r--   0 leonwu     (501) staff       (20)     7513 2023-05-03 20:19:40.000000 CB_IPO-0.2.0/docs/Example Cases.ipynb
+-rw-r--r--   0 leonwu     (501) staff       (20)      634 2023-04-05 01:00:03.000000 CB_IPO-0.2.0/docs/Makefile
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.716601 CB_IPO-0.2.0/docs/_build/
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.716538 CB_IPO-0.2.0/docs/_build/doctrees/
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.722190 CB_IPO-0.2.0/docs/_build/doctrees/nbsphinx/
+-rw-r--r--   0 leonwu     (501) staff       (20)     7491 2023-04-05 03:41:14.000000 CB_IPO-0.2.0/docs/_build/doctrees/nbsphinx/Example Cases.ipynb
+drwxr-xr-x   0 leonwu     (501) staff       (20)        0 2023-05-04 20:59:35.722430 CB_IPO-0.2.0/docs/_build/html/
+-rw-r--r--   0 leonwu     (501) staff       (20)     7491 2023-04-05 03:41:14.000000 CB_IPO-0.2.0/docs/_build/html/Example Cases.ipynb
+-rw-r--r--   0 leonwu     (501) staff       (20)     2242 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/docs/conf.py
+-rw-r--r--   0 leonwu     (501) staff       (20)       56 2023-05-03 20:19:40.000000 CB_IPO-0.2.0/docs/examples.rst
+-rw-r--r--   0 leonwu     (501) staff       (20)      392 2023-04-05 03:39:56.000000 CB_IPO-0.2.0/docs/index.rst
+-rw-r--r--   0 leonwu     (501) staff       (20)       97 2023-04-05 01:00:03.000000 CB_IPO-0.2.0/docs/installation.rst
+-rw-r--r--   0 leonwu     (501) staff       (20)      765 2023-04-05 01:00:03.000000 CB_IPO-0.2.0/docs/make.bat
+-rw-r--r--   0 leonwu     (501) staff       (20)       38 2023-04-05 01:00:03.000000 CB_IPO-0.2.0/docs/methods.rst
+-rw-r--r--   0 leonwu     (501) staff       (20)      761 2023-04-05 01:00:03.000000 CB_IPO-0.2.0/docs/usage.rst
+-rw-r--r--   0 leonwu     (501) staff       (20)     2201 2023-05-04 20:53:36.000000 CB_IPO-0.2.0/pyproject.toml
+-rw-r--r--   0 leonwu     (501) staff       (20)       38 2023-05-04 20:59:35.723211 CB_IPO-0.2.0/setup.cfg
+-rw-r--r--   0 leonwu     (501) staff       (20)       38 2023-03-27 02:52:33.000000 CB_IPO-0.2.0/setup.py
```

### Comparing `CB_IPO-0.1.0/CB_IPO.egg-info/PKG-INFO` & `CB_IPO-0.2.0/CB_IPO.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CB-IPO
-Version: 0.1.0
+Version: 0.2.0
 Summary: Crunchbase and SEC filing scraper
 Author-email: Leon <wu.leon@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,14 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/llw2128/CB_IPO
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -223,61 +222,95 @@
 
 # CB_IPO
 This is a library designed for quick webscraping in finding information on SEC filings with a focus on new IPOs and annual reports.
 
 [![Build Status](https://github.com/llw2128/CB_IPO/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/llw2128/CB_IPO/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/llw2128/CB_IPO/branch/main/graph/badge.svg)](https://codecov.io/gh/llw2128/CB_IPO)
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)  ![](https://img.shields.io/github/issues/llw2128/CB_IPO)
+[![PyPI](https://img.shields.io/pypi/v/CB_IPO)](https://pypi.org/project/CB-IPO/)
+[![Documentation](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=GitHub%20Pages&logoColor=white)](https://llw2128.github.io/CB_IPO/)
 
 ## Overview
 Researching information on trends for companies can be incredibly tedious, this library will automate part of the proccess making DCF building and IPO research easier. CB_IPO is a library that will fetch information on recent and historical IPOs by scraping the SEC EDGAR database for S-1 filings. These queries can also be modified to search for certain dates, and additional forms. This data can subsequently be placed in a pandas dataframe for the sake of easy viewing. A second proccess this autmoates is finding the specific 10-K filings for a company. By inputing a cik, a list of 10-k filing links will be returned. With these links, the library also has a function for using a 10-k link and returning a list of info such as assets, liabilities, and income.
 
+## Example
+Suppose I want to find companies that have filed either an S-1, 10-K or 10-Q between January 2021 and March 2023
+```python
+sc = scrape()
+sc.set_search_date("2021-01-01", "2023-03-31")
+sc.add_forms(['S-1','10-K', '10-Q'])
+dataframe = sc.generate_df(10, 1)
+```
+Then this dataframe is returned
+```
+                                                names filing date
+0               Inhibikase Therapeutics, Inc.  (IKT)   2023-03-31
+1                       AMERINST INSURANCE GROUP LTD   2023-03-31
+2                      SLM Student Loan Trust 2013-5   2023-03-31
+3   Games & Esports Experience Acquisition Corp.  ...  2023-03-31
+4   Bilander Acquisition Corp.  (TWCB, TWCBU, TWCBW)   2023-03-31
+5                                VirTra, Inc  (VTSI)   2023-03-31
+6             Actinium Pharmaceuticals, Inc.  (ATNM)   2023-03-31
+7                              Genprex, Inc.  (GNPX)   2023-03-31
+8                           Mega Matrix Corp.  (MPU)   2023-03-31
+9       Digital Media Solutions, Inc.  (DMS, DMS-WT)   2023-03-31
+```
+
 ## Installation
 `CB_IPO` can be installed via PyPi by running:
-```
+```python
 pip install CB_IPO
 ```
 
 ## Quick Start
 To use `CB_IPO` instantiate an instance by calling 
-```
+```python
 instance = scrape()
 ``` 
 
 To adjust search date ranges run (Dates in YYYY-MM-DD)
-```
+```python
 instance.set_search_date(START, END)
 ```
 
 To add form types to the search run
-```
+```python
 instance.add_forms(['S-1','10-K'])
 ```
 
 To get a dataframe with all companies filing within the specified paramateres and filing dates run
 
-```
+```python
 instance.generate_df(Number of entries per page, number of pages)
 ```
 
 To get a list of links to 10-K filings by a company given CIK
-```
+```python
 instance.create_links(cik, number of files needed)
 ```
 
-To scrape a 10-K link for assets, liabilities, and Net Income run
-```
+To scrape a 10-K link for elements like assets, liabilities, and Net Income run
+```python
 instance.scrape_xbrl(link)
 ```
+
+To calculate financial ratios from a dicitonary of financial elements run
+```python
+instance.calculate_ratios(link)
+```
+
+To get a dataframe summarizing the 10-k elements run with an optional flag
+```python
+instance.summarize_10k(link, flag)
+```
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
-
-
```

### Comparing `CB_IPO-0.1.0/CONTRIBUTING.md` & `CB_IPO-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CB_IPO-0.1.0/LICENSE` & `CB_IPO-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CB_IPO-0.1.0/Makefile` & `CB_IPO-0.2.0/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -87,19 +87,39 @@
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
+
+
+#DOCS
+TMPREPO=./tmp/docs/CB_IPO
+
+docs: 
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/llw2128/CB_IPO.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
+
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help docs pages
```

### Comparing `CB_IPO-0.1.0/PKG-INFO` & `CB_IPO-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CB_IPO
-Version: 0.1.0
+Version: 0.2.0
 Summary: Crunchbase and SEC filing scraper
 Author-email: Leon <wu.leon@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,14 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/llw2128/CB_IPO
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -223,61 +222,95 @@
 
 # CB_IPO
 This is a library designed for quick webscraping in finding information on SEC filings with a focus on new IPOs and annual reports.
 
 [![Build Status](https://github.com/llw2128/CB_IPO/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/llw2128/CB_IPO/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/llw2128/CB_IPO/branch/main/graph/badge.svg)](https://codecov.io/gh/llw2128/CB_IPO)
 [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://opensource.org/licenses/Apache-2.0)  ![](https://img.shields.io/github/issues/llw2128/CB_IPO)
+[![PyPI](https://img.shields.io/pypi/v/CB_IPO)](https://pypi.org/project/CB-IPO/)
+[![Documentation](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=GitHub%20Pages&logoColor=white)](https://llw2128.github.io/CB_IPO/)
 
 ## Overview
 Researching information on trends for companies can be incredibly tedious, this library will automate part of the proccess making DCF building and IPO research easier. CB_IPO is a library that will fetch information on recent and historical IPOs by scraping the SEC EDGAR database for S-1 filings. These queries can also be modified to search for certain dates, and additional forms. This data can subsequently be placed in a pandas dataframe for the sake of easy viewing. A second proccess this autmoates is finding the specific 10-K filings for a company. By inputing a cik, a list of 10-k filing links will be returned. With these links, the library also has a function for using a 10-k link and returning a list of info such as assets, liabilities, and income.
 
+## Example
+Suppose I want to find companies that have filed either an S-1, 10-K or 10-Q between January 2021 and March 2023
+```python
+sc = scrape()
+sc.set_search_date("2021-01-01", "2023-03-31")
+sc.add_forms(['S-1','10-K', '10-Q'])
+dataframe = sc.generate_df(10, 1)
+```
+Then this dataframe is returned
+```
+                                                names filing date
+0               Inhibikase Therapeutics, Inc.  (IKT)   2023-03-31
+1                       AMERINST INSURANCE GROUP LTD   2023-03-31
+2                      SLM Student Loan Trust 2013-5   2023-03-31
+3   Games & Esports Experience Acquisition Corp.  ...  2023-03-31
+4   Bilander Acquisition Corp.  (TWCB, TWCBU, TWCBW)   2023-03-31
+5                                VirTra, Inc  (VTSI)   2023-03-31
+6             Actinium Pharmaceuticals, Inc.  (ATNM)   2023-03-31
+7                              Genprex, Inc.  (GNPX)   2023-03-31
+8                           Mega Matrix Corp.  (MPU)   2023-03-31
+9       Digital Media Solutions, Inc.  (DMS, DMS-WT)   2023-03-31
+```
+
 ## Installation
 `CB_IPO` can be installed via PyPi by running:
-```
+```python
 pip install CB_IPO
 ```
 
 ## Quick Start
 To use `CB_IPO` instantiate an instance by calling 
-```
+```python
 instance = scrape()
 ``` 
 
 To adjust search date ranges run (Dates in YYYY-MM-DD)
-```
+```python
 instance.set_search_date(START, END)
 ```
 
 To add form types to the search run
-```
+```python
 instance.add_forms(['S-1','10-K'])
 ```
 
 To get a dataframe with all companies filing within the specified paramateres and filing dates run
 
-```
+```python
 instance.generate_df(Number of entries per page, number of pages)
 ```
 
 To get a list of links to 10-K filings by a company given CIK
-```
+```python
 instance.create_links(cik, number of files needed)
 ```
 
-To scrape a 10-K link for assets, liabilities, and Net Income run
-```
+To scrape a 10-K link for elements like assets, liabilities, and Net Income run
+```python
 instance.scrape_xbrl(link)
 ```
+
+To calculate financial ratios from a dicitonary of financial elements run
+```python
+instance.calculate_ratios(link)
+```
+
+To get a dataframe summarizing the 10-k elements run with an optional flag
+```python
+instance.summarize_10k(link, flag)
+```
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
-
-
```

### Comparing `CB_IPO-0.1.0/pyproject.toml` & `CB_IPO-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "CB_IPO"
 authors = [{name = "Leon", email = "wu.leon@columbia.edu"}]
 description="Crunchbase and SEC filing scraper"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -58,17 +58,18 @@
 
 [tool.check-manifest]
 ignore = [
 ]
 
 [tool.flake8]
 ignore = ['E203', 'W503']
-max-line-length=120
+max-line-length=130
 exclude=[
-    'CB_IPO/tests/*'
+    'CB_IPO/tests/*',
+    'CB_IPO/example.ipynb*'
 ]
 per-file-ignores= [
     'CB_IPO/__init__.py:F401, F403',
     'CB_IPO/__main__.py:F401, F403'
 ]
```

