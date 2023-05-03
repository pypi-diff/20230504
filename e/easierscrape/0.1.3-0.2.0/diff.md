# Comparing `tmp/easierscrape-0.1.3.tar.gz` & `tmp/easierscrape-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierscrape-0.1.3.tar", last modified: Mon Apr 24 14:39:39 2023, max compression
+gzip compressed data, was "easierscrape-0.2.0.tar", last modified: Wed May  3 22:06:34 2023, max compression
```

## Comparing `easierscrape-0.1.3.tar` & `easierscrape-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:39.000491 easierscrape-0.1.3/
--rw-rw-rw-   0        0        0      550 2023-04-24 14:34:54.000000 easierscrape-0.1.3/.bumpversion.cfg
--rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.1.3/.readthedocs.yml
--rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.1.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.1.3/Makefile
--rw-rw-rw-   0        0        0    18297 2023-04-24 14:39:38.999419 easierscrape-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4265 2023-04-19 16:51:19.000000 easierscrape-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.948028 easierscrape-0.1.3/docs/
--rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.1.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.911862 easierscrape-0.1.3/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.913993 easierscrape-0.1.3/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.953859 easierscrape-0.1.3/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/_build/html/_images/cli_recording.gif
--rw-rw-rw-   0        0        0   158783 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/_build/html/_images/demo_recording.gif
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.956942 easierscrape-0.1.3/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     2386 2023-04-23 18:18:13.000000 easierscrape-0.1.3/docs/_build/html/_sources/index.md.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.960484 easierscrape-0.1.3/docs/_build/html/_sources/source/
--rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.1.3/docs/_build/html/_sources/source/easierscrape.rst.txt
--rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.1.3/docs/_build/html/_sources/source/modules.rst.txt
--rw-rw-rw-   0        0        0     1098 2023-04-24 14:34:54.000000 easierscrape-0.1.3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.966377 easierscrape-0.1.3/docs/images/
--rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/images/cli_recording.gif
--rw-rw-rw-   0        0        0   158783 2023-04-05 17:40:22.000000 easierscrape-0.1.3/docs/images/demo_recording.gif
--rw-rw-rw-   0        0        0     2386 2023-04-24 13:49:29.000000 easierscrape-0.1.3/docs/index.md
--rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.1.3/docs/make.bat
--rw-rw-rw-   0        0        0      109 2023-04-24 14:34:54.000000 easierscrape-0.1.3/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.972614 easierscrape-0.1.3/docs/source/
--rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.1.3/docs/source/easierscrape.rst
--rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.1.3/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.985129 easierscrape-0.1.3/easierscrape/
--rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.1.3/easierscrape/__init__.py
--rw-rw-rw-   0        0        0      742 2023-04-24 13:49:29.000000 easierscrape-0.1.3/easierscrape/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-24 14:34:54.000000 easierscrape-0.1.3/easierscrape/_version.py
--rw-rw-rw-   0        0        0     8420 2023-04-24 14:03:25.000000 easierscrape-0.1.3/easierscrape/easierscrape.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.998034 easierscrape-0.1.3/easierscrape/tests/
--rw-rw-rw-   0        0        0    11335 2023-04-24 14:03:25.000000 easierscrape-0.1.3/easierscrape/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:39:38.992878 easierscrape-0.1.3/easierscrape.egg-info/
--rw-rw-rw-   0        0        0    18297 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      846 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 14:39:38.000000 easierscrape-0.1.3/easierscrape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2434 2023-04-24 14:34:54.000000 easierscrape-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 14:39:39.000491 easierscrape-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.095369 easierscrape-0.2.0/
+-rw-rw-rw-   0        0        0      550 2023-05-03 21:59:41.000000 easierscrape-0.2.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.2.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.2.0/Makefile
+-rw-rw-rw-   0        0        0    18403 2023-05-03 22:06:34.094078 easierscrape-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4371 2023-05-03 21:17:56.000000 easierscrape-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.061998 easierscrape-0.2.0/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0     1098 2023-05-03 21:59:41.000000 easierscrape-0.2.0/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.066963 easierscrape-0.2.0/docs/images/
+-rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.2.0/docs/images/cli_recording.gif
+-rw-rw-rw-   0        0        0   108334 2023-05-03 21:17:56.000000 easierscrape-0.2.0/docs/images/demo_recording.gif
+-rw-rw-rw-   0        0        0     2377 2023-05-03 21:17:56.000000 easierscrape-0.2.0/docs/index.md
+-rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0      109 2023-05-03 21:59:41.000000 easierscrape-0.2.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.071333 easierscrape-0.2.0/docs/source/
+-rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.2.0/docs/source/easierscrape.rst
+-rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.2.0/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.079802 easierscrape-0.2.0/easierscrape/
+-rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.2.0/easierscrape/__init__.py
+-rw-rw-rw-   0        0        0      699 2023-05-03 21:17:56.000000 easierscrape-0.2.0/easierscrape/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-03 21:59:41.000000 easierscrape-0.2.0/easierscrape/_version.py
+-rw-rw-rw-   0        0        0     9469 2023-05-03 21:31:47.000000 easierscrape-0.2.0/easierscrape/easierscrape.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.091756 easierscrape-0.2.0/easierscrape/tests/
+-rw-rw-rw-   0        0        0    11498 2023-05-03 21:17:56.000000 easierscrape-0.2.0/easierscrape/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.090603 easierscrape-0.2.0/easierscrape.egg-info/
+-rw-rw-rw-   0        0        0    18403 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2434 2023-05-03 21:59:41.000000 easierscrape-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 22:06:34.095369 easierscrape-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.2.0/setup.py
```

### Comparing `easierscrape-0.1.3/.bumpversion.cfg` & `easierscrape-0.2.0/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:easierscrape/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `easierscrape-0.1.3/CONTRIBUTING.md` & `easierscrape-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/LICENSE` & `easierscrape-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/MANIFEST.in` & `easierscrape-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/Makefile` & `easierscrape-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/PKG-INFO` & `easierscrape-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.1.3
+Version: 0.2.0
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,41 +246,42 @@
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
 
 ## Basic Usage
 Install with pip: `pip install easierscrape`
 
-Import `Scraper` from `easierscrape` as seen below and then call class methods to scrape varying resources:
+Import `Scraper` from `easierscrape` and instantiate it with a url as seen below:
 ```python
 from easierscrape import Scraper
 
-scraper = Scraper()
+scraper = Scraper("https://quotes.toscrape.com/login")
 ```
+From there, call class methods to scrape varying resources.
 
 Usage examples:
 ```
->>> scraper.parse_text("https://quotes.toscrape.com/login")
+>>> scraper.parse_text()
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(1)
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
-When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
+When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
 positional arguments:
   url         the url to scrape
   depth       the depth of the scrape tree
 
@@ -300,12 +301,12 @@
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Contributing
 
-See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+See [CONTRIBUTING](https://github.com/dag2226/easierscrape/blob/main/CONTRIBUTING.md) for more information.
 
 ## License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://github.com/dag2226/easierscrape/blob/main/LICENSE) for more information.
```

### Comparing `easierscrape-0.1.3/README.md` & `easierscrape-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,41 +24,42 @@
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
 
 ## Basic Usage
 Install with pip: `pip install easierscrape`
 
-Import `Scraper` from `easierscrape` as seen below and then call class methods to scrape varying resources:
+Import `Scraper` from `easierscrape` and instantiate it with a url as seen below:
 ```python
 from easierscrape import Scraper
 
-scraper = Scraper()
+scraper = Scraper("https://quotes.toscrape.com/login")
 ```
+From there, call class methods to scrape varying resources.
 
 Usage examples:
 ```
->>> scraper.parse_text("https://quotes.toscrape.com/login")
+>>> scraper.parse_text()
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(1)
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
-When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
+When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
 positional arguments:
   url         the url to scrape
   depth       the depth of the scrape tree
 
@@ -78,12 +79,12 @@
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Contributing
 
-See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+See [CONTRIBUTING](https://github.com/dag2226/easierscrape/blob/main/CONTRIBUTING.md) for more information.
 
 ## License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://github.com/dag2226/easierscrape/blob/main/LICENSE) for more information.
```

### Comparing `easierscrape-0.1.3/docs/Makefile` & `easierscrape-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/docs/_build/html/_images/cli_recording.gif` & `easierscrape-0.2.0/docs/images/cli_recording.gif`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/docs/_build/html/_sources/index.md.txt` & `easierscrape-0.2.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Welcome to easierscrape's documentation!
 
 ## Basic Usage
 Install with pip: `pip install easierscrape`
 
-Import `Scraper` from `easierscrape` as seen below and then call class methods to scrape varying resources:
+Import `Scraper` from `easierscrape` and instantiate it with a url as seen below:
 ```python
 from easierscrape import Scraper
 
-scraper = Scraper()
+scraper = Scraper("https://quotes.toscrape.com/login")
 ```
+From there, call class methods to scrape varying resources.
 
 Usage examples:
 ```
->>> scraper.parse_text("https://quotes.toscrape.com/login")
+>>> scraper.parse_text()
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(1)
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
 
 ### Downloads
 Using `get_screenshot`, `parse_files`, `parse_images`, or `parse_tables` will result in an "easierscrape_downloads" directory being created in the working directory.
 
 Usage example:
 ```eval_rst
```

### Comparing `easierscrape-0.1.3/docs/conf.py` & `easierscrape-0.2.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Path setup --------------------------------------------------------------
 sys.path.insert(0, os.path.abspath('../'))
 
 # -- Project information -----------------------------------------------------
 project = 'easierscrape'
 copyright = '2023, Daniel Greco'
 author = 'Daniel Greco'
-release = '0.1.3'
+release = '0.2.0'
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
 source_suffix = ['.rst', '.md']
```

### Comparing `easierscrape-0.1.3/docs/make.bat` & `easierscrape-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easierscrape-0.1.3/easierscrape/easierscrape.py` & `easierscrape-0.2.0/easierscrape/easierscrape.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,230 +1,249 @@
 from anytree import Node, RenderTree
 from anytree.search import find
 from bs4 import BeautifulSoup
 from os import getcwd, makedirs
 from os.path import basename, exists, join
-from pandas import read_html
+from pandas import read_html, ExcelWriter
 from re import compile
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from urllib.parse import urlparse
 from urllib.request import urlopen, url2pathname
 from uuid import uuid4
 
 
 class Scraper:
-    def __init__(self):
+    """Class for a scraper that targets `url`. A `Scraper` object acts as a "one-stop-shop" for
+    all scraping functions.
+    """
+
+    def __init__(self, url):
+        """
+        Args:
+            url (str): The url to scrape from.
+
+        """
+        self.url = url
+
         # hide GUI
         options = Options()
         options.add_argument("--headless")
         options.add_argument("--window-size=1920,1080")
         options.add_argument("start-maximized")
-        options.add_experimental_option('excludeSwitches', ['enable-logging'])
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
         options.add_experimental_option("prefs", {"profile.managed_default_content_settings.images": 2})
-        self.driver = webdriver.Chrome(options=options)
 
-    def _soup_url(self, url):
+        self.driver = webdriver.Chrome(options=options)
         self.driver.get(url)
-        return BeautifulSoup(self.driver.page_source, "html.parser")
+
+        self.soup_url = BeautifulSoup(self.driver.page_source, "html.parser")
+
+    def __del__(self):
+        self.driver.quit()
 
     def _concat_urls(self, base_url, child_url):
         parsed = urlparse(base_url)
         if child_url.startswith("/"):
             child_url = parsed.scheme + "://" + parsed.netloc + child_url
         if child_url.startswith("./"):
             child_url = base_url + child_url[1:]
         if not child_url.startswith("http"):
             child_url = base_url + "/" + child_url
         if child_url.endswith("/"):
             child_url = child_url[:-1]
         return child_url
 
-    def _get_download_dir(self, type, url):
-        dir = join(getcwd(), "easierscrape_downloads", type, url2pathname(url)[3:])
+    def _get_download_dir(self, type):
+        dir = join(getcwd(), "easierscrape_downloads", type, url2pathname(self.url)[3:])
         if not exists(dir):
             makedirs(dir)
         return dir
 
     def _tree_gen_rec(self, url, maxdepth, tree, depth):
         if tree is None:
             url = url.replace("www.", "")
             if url.endswith("/"):
                 url = url[:-1]
             tree = Node(url, url=url)
         if depth < maxdepth:
             parent_node = tree
-            for a in self.parse_anchors(url):
+            self.driver.get(url)
+            for a in BeautifulSoup(self.driver.page_source, "html.parser").find_all("a"):
                 try:
                     child_url = self._concat_urls(url, a.attrs["href"].replace("www.", ""))
                     if find(tree.root, lambda node: node.url == child_url) is None:
                         new_leaf = Node(child_url, url=child_url, parent=parent_node)
                         tree = self._tree_gen_rec(child_url, maxdepth, new_leaf, depth + 1)
                 except Exception:
                     pass
         return tree.root
 
-    def get_screenshot(self, url):
-        """Downloads screenshot from provided url to an "easierscrape_downloads"
-        folder in the current working directory
-
-        Args:
-            url (str): The url to screenshot
+    def get_screenshot(self):
+        """Downloads screenshot from the Scraper url to an "easierscrape_downloads" folder in the
+        current working directory.
 
         Returns:
             bool: True
 
         """
-        download_file = join(self._get_download_dir("images", url), "easierscrape_screenshot.png")
+        download_file = join(self._get_download_dir("images"), "easierscrape_screenshot.png")
 
-        self.driver.get(url)
-        self.driver.find_element(By.TAG_NAME, 'body').screenshot(download_file)
-
-        return True  # getsize(download_file)
+        self.driver.find_element(By.TAG_NAME, "body").screenshot(download_file)
 
-    def parse_anchors(self, url):
-        """Parses a list of anchor tags from provided url.
+        return True
 
-        Args:
-            url (str): The url to scrape from
+    def parse_anchors(self):
+        """Parses a list of anchor tags from the Scraper url.
 
         Returns:
-            List[str]: List of anchor tags in the url
+            List[str]: List of anchor tags in the url.
 
         """
-        return self._soup_url(url).find_all("a")
+        return self.soup_url.find_all("a")
 
-    def parse_files(self, url, filetypes=[]):
-        """Downloads provided filetypes from provided url to an "easierscrape_downloads"
-        folder in the current working directory
+    def parse_files(self, filetypes=[]):
+        """Downloads provided filetypes from the Scraper url to an "easierscrape_downloads" folder
+        in the current working directory.
 
         Args:
-            url (str): The url to scrape from
-            filetypes (List[str]): List of filetypes ("pdf", "txt", etc.) to scrape
+            filetypes (List[str]): List of filetypes ("pdf", "txt", etc.) to scrape.
 
         Returns:
             List[int]: List of number of files downloaded per filetype from url (so if
             filetypes=["pdf", "txt"] and the return value is [1, 30] this means that 1
-            pdf file and 30 txt files were downloaded)
+            pdf file and 30 txt files were downloaded).
 
         """
         if len(filetypes) == 0:
             print("No filetype specified")
             return
         file_download_list = []
         for filetype in filetypes:
             file_download_count = 0
-            for file in self._soup_url(url).find_all("a", href=compile(r"(." + filetype + ")")):
+            for file in self.soup_url.find_all("a", href=compile(r"(." + filetype + ")")):
                 try:
-                    fileUrl = self._concat_urls(url, file.attrs["href"])
+                    fileUrl = self._concat_urls(self.url, file.attrs["href"])
                     response = urlopen(fileUrl)
-                    with open(join(self._get_download_dir(filetype, url), basename(fileUrl)), "wb") as file:
+                    with open(join(self._get_download_dir(filetype), basename(fileUrl)), "wb") as file:
                         file.write(response.read())
+                    file.close()
                     file_download_count += 1
                 except Exception:
                     pass
             file_download_list.append(file_download_count)
         return file_download_list
 
-    def parse_images(self, url):
-        """Downloads all images from provided url to an "easierscrape_downloads"
-        folder in the current working directory
-
-        Args:
-            url (str): The url to scrape from
+    def parse_images(self):
+        """Downloads all images from the Scraper url to an "easierscrape_downloads" folder in the
+        current working directory.
 
         Returns:
-            int: Number of images downloaded from url
+            int: Number of images downloaded from url.
 
         """
         image_download_count = 0
-        for image in self._soup_url(url).findAll("img"):
+        for image in self.soup_url.findAll("img"):
             try:
-                imageUrl = self._concat_urls(url, image.attrs["src"])
+                imageUrl = self._concat_urls(self.url, image.attrs["src"])
                 response = urlopen(imageUrl)
-                with open(join(self._get_download_dir("images", url), basename(imageUrl)), "wb") as file:
+                with open(join(self._get_download_dir("images"), basename(imageUrl)), "wb") as file:
                     file.write(response.read())
+                    file.close()
                 image_download_count += 1
             except Exception:
                 pass
         return image_download_count
 
-    def parse_lists(self, url):
-        """Parses a list of lists from provided url.
-
-        Args:
-            url (str): The url to scrape from
+    def parse_lists(self):
+        """Parses a list of lists from the Scraper url.
 
         Returns:
-            List[List[str]]: List of lists (each stored as a List) in the url
+            List[List[str]]: List of lists (each stored as a List) in the url.
 
         """
         # This covers unordered and ordered, but not description lists (dl)
-        # TODO: The unit test for this could be improved
         out = []
-        for list in self._soup_url(url).findAll(["ul", "ol"]):
+        for list in self.soup_url.findAll(["ul", "ol"]):
             out.append([item for item in list.stripped_strings])
             if out[-1] == []:
                 out.pop()
         return out
 
-    def parse_tables(self, url):
-        """Downloads all tables from provided url to an "easierscrape_downloads"
-        folder in the current working directory
+    def parse_tables(self, output_type="csv"):
+        """Downloads all tables from the Scraper url to an "easierscrape_downloads" folder in the
+        current working directory.
+
+        Supported output types are csv and xlsx (defaults to csv).
+
+        - If downloaded as a csv file, each table will be stored in a separate csv.
+        - If downloaded as an xlsx file, all tables will be stored as separate sheets in a
+          "tables.xlsx" file.
 
         Args:
-            url (str): The url to scrape from
+            output_type (str): The filetype to output to (defaults to csv).
 
         Returns:
-            int: Number of tables downloaded from url
+            int: Number of tables downloaded from url.
 
         """
-        soup_tables = self._soup_url(url).findAll("table")
+        soup_tables = self.soup_url.findAll("table")
         if len(soup_tables) != 0:
-            tables = read_html(url)
+            tables = read_html(self.url)
             # soup_tables is only used to get the ids of tables (for naming purposes)
             # and find the number of tables. pandas read_html does all the work
             for i in range(0, len(tables)):
                 if soup_tables[i].has_attr("id"):
                     table_name = soup_tables[i]["id"]
                 else:
-                    table_name = str(uuid4())
-                tables[i].to_csv(join(self._get_download_dir("tables", url), table_name + ".csv"))
+                    table_name = uuid4().hex[0:31]
+                if output_type == "csv":
+                    tables[i].to_csv(join(self._get_download_dir("tables"), table_name + ".csv"))
+                elif output_type == "xlsx":
+                    excel_file = join(self._get_download_dir("tables"), "tables.xlsx")
+                    if exists(excel_file):
+                        with ExcelWriter(excel_file, mode="a") as writer:
+                            tables[i].to_excel(writer, sheet_name=table_name)
+                    else:
+                        with ExcelWriter(excel_file, mode="w") as writer:
+                            tables[i].to_excel(writer, sheet_name=table_name)
+                else:
+                    print(
+                        "output_type = "
+                        + output_type
+                        + " not implemented.\nCurrently supported filetypes are csv and xlsx."
+                    )
         return len(soup_tables)
 
-    def parse_text(self, url):
-        """Parses a list of text fragments from provided url.
-
-        Args:
-            url (str): The url to scrape from
+    def parse_text(self):
+        """Parses a list of text fragments from the Scraper url.
 
         Returns:
-            List[str]: List of text fragments in the url
+            List[str]: List of text fragments in the url.
 
         """
-        return [text for text in self._soup_url(url).stripped_strings]
+        return [text for text in self.soup_url.stripped_strings]
 
-    def tree_gen(self, url, maxdepth):
-        """Generates a tree of depth=maxdepth starting at url
+    def tree_gen(self, maxdepth):
+        """Generates a tree of depth=maxdepth starting at the Scraper url.
 
         Args:
-            url (str): The head url to generate the tree from
-            maxdepth (int): The depth you want to generate the tree to
+            maxdepth (int): The depth you want to generate the tree to.
 
         Returns:
-            Node: Head node of an anytree hyperlink tree
+            Node: Head node of an anytree hyperlink tree.
 
         """
-        return self._tree_gen_rec(url, maxdepth, None, 0)
+        return self._tree_gen_rec(self.url, maxdepth, None, 0)
 
-    def print_tree(self, tree):
-        """Prints out the tree of the provided anytree Node structure
+    def print_tree(self, maxdepth):
+        """Prints a tree of depth=maxdepth starting at the Scraper url.
 
         Args:
-            tree (Node): The head anytree Node of the tree to print
+            maxdepth (int): The depth you want to print the tree to.
 
         """
         tree_print = ""
-        for pre, fill, node in RenderTree(tree):
+        for pre, fill, node in RenderTree(self.tree_gen(maxdepth)):
             tree_print += "%s%s\n" % (pre, node.name)
         print(tree_print[:-1])
```

### Comparing `easierscrape-0.1.3/easierscrape/tests/test_all.py` & `easierscrape-0.2.0/easierscrape/tests/test_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,64 +2,70 @@
 from easierscrape.__main__ import main
 from os import getcwd, makedirs
 from os.path import exists, join
 from shutil import rmtree
 from unittest.mock import patch
 
 
-scraper = easierscrape.Scraper()
+toscrape = easierscrape.Scraper("https://toscrape.com")
+jaescrape = easierscrape.Scraper("https://www.cs.columbia.edu/~jae/")
+quotescrape = easierscrape.Scraper("https://quotes.toscrape.com")
+webio = easierscrape.Scraper("https://webscraper.io/test-sites/e-commerce/static")
+quoteslogin = easierscrape.Scraper("https://quotes.toscrape.com/login")
+quotesjs = easierscrape.Scraper("http://quotes.toscrape.com/js/")
+
 download_dir = join(getcwd(), "easierscrape_downloads")
 
 
 # UNIT TESTS=======================================================================================
 def test_get_screenshot():
-    assert True  # scraper.get_screenshot("https://toscrape.com") in [191320, 230509]
-    # rmtree(download_dir)
+    assert toscrape.get_screenshot() == True
+    rmtree(download_dir)
 
 
 def test_parse_anchors():
-    assert len(scraper.parse_anchors("https://toscrape.com/")) == 13
+    assert len(toscrape.parse_anchors()) == 13
 
 
 def test_parse_files_txt():
-    assert scraper.parse_files("https://www.cs.columbia.edu/~jae/", ["txt"]) == [1]
+    assert jaescrape.parse_files(["txt"]) == [1]
     rmtree(download_dir)
 
 
 def test_parse_files_pdf():
-    assert scraper.parse_files("https://www.cs.columbia.edu/~jae/", ["pdf"]) == [22]
+    assert jaescrape.parse_files(["pdf"]) == [22]
     rmtree(download_dir)
 
 
 def test_parse_files_txt_pdf():
-    assert scraper.parse_files("https://www.cs.columbia.edu/~jae/", ["txt", "pdf"]) == [1, 22]
+    assert jaescrape.parse_files(["txt", "pdf"]) == [1, 22]
     rmtree(download_dir)
 
 
 @patch("builtins.print")
 def test_parse_files_without_filetype(mock_print):
-    scraper.parse_files("https://toscrape.com/", [])
+    toscrape.parse_files([])
     assert mock_print.call_args.args == ("No filetype specified",)
 
 
 def test_parse_files_without_txt_file():
-    assert scraper.parse_files("https://toscrape.com/", ["txt"]) == [0]
+    assert toscrape.parse_files(["txt"]) == [0]
 
 
 def test_parse_images_with_image():
-    assert scraper.parse_images("https://toscrape.com/") == 3
+    assert toscrape.parse_images() == 3
     rmtree(download_dir)
 
 
 def test_parse_images_without_image():
-    assert scraper.parse_images("https://quotes.toscrape.com/") == 0
+    assert quotescrape.parse_images() == 0
 
 
 def test_parse_lists():
-    assert scraper.parse_lists("https://webscraper.io/test-sites/e-commerce/static") == [
+    assert webio.parse_lists() == [
         [
             "Web Scraper",
             "Cloud Scraper",
             "Pricing",
             "Learn",
             "Documentation",
             "Video Tutorials",
@@ -83,28 +89,41 @@
         ],
         ["Resources", "Blog", "Documentation", "Video Tutorials", "Screenshots", "Test Sites", "Forum"],
         ["CONTACT US", "info@webscraper.io", "Ubelu 5-71,", "Adazi, Latvia, LV-2164"],
     ]
 
 
 def test_parse_no_lists():
-    assert scraper.parse_lists("https://toscrape.com/") == []
+    assert toscrape.parse_lists() == []
+
+
+def test_parse_tables_to_csv():
+    assert toscrape.parse_tables() == 2
+    rmtree(download_dir)
 
 
-def test_parse_tables():
-    assert scraper.parse_tables("https://toscrape.com/") == 2
+def test_parse_tables_to_xlsx():
+    assert toscrape.parse_tables("xlsx") == 2
     rmtree(download_dir)
 
 
 def test_parse_no_tables():
-    assert scraper.parse_tables("https://quotes.toscrape.com/") == 0
+    assert quotescrape.parse_tables() == 0
+
+
+@patch("builtins.print")
+def test_parse_tables_to_unsupported_type(mock_print):
+    assert toscrape.parse_tables("unsup") == 2
+    assert mock_print.call_args.args == (
+        "output_type = unsup not implemented.\nCurrently supported filetypes are csv and xlsx.",
+    )
 
 
 def test_parse_text():
-    assert scraper.parse_text("https://quotes.toscrape.com/login") == [
+    assert quoteslogin.parse_text() == [
         "Quotes to Scrape",
         "Quotes to Scrape",
         "Login",
         "Username",
         "Password",
         "Quotes by:",
         "GoodReads.com",
@@ -114,47 +133,47 @@
         "Scrapinghub",
     ]
 
 
 # INTEGRATION TESTS================================================================================
 @patch("builtins.print")
 def test_print_tree_1(mock_print):
-    scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
+    toscrape.print_tree(1)
     assert mock_print.call_args.args == (
         "https://toscrape.com\n├── http://books.toscrape.com\n├── http://quotes.toscrape.com\n├── http://quotes.toscrape.com/scroll\n├── http://quotes.toscrape.com/js\n├── http://quotes.toscrape.com/js-delayed\n├── http://quotes.toscrape.com/tableful\n├── http://quotes.toscrape.com/login\n├── http://quotes.toscrape.com/search.aspx\n└── http://quotes.toscrape.com/random",
     )
 
 
 @patch("builtins.print")
 def test_print_tree_2(mock_print):
-    scraper.print_tree(scraper.tree_gen("https://toscrape.com", 0))
+    toscrape.print_tree(0)
     assert mock_print.call_args.args == ("https://toscrape.com",)
 
 
 @patch("builtins.print")
 def test_print_tree_3(mock_print):
-    scraper.print_tree(scraper.tree_gen("https://quotes.toscrape.com/", 2))
+    quotescrape.print_tree(2)
     assert mock_print.call_args.args == (
         "https://quotes.toscrape.com\n├── https://quotes.toscrape.com/login\n│   ├── https://goodreads.com/quotes\n│   └── https://scrapinghub.com\n├── https://quotes.toscrape.com/author/Albert-Einstein\n├── https://quotes.toscrape.com/tag/change/page/1\n│   ├── https://quotes.toscrape.com/tag/deep-thoughts/page/1\n│   ├── https://quotes.toscrape.com/tag/thinking/page/1\n│   ├── https://quotes.toscrape.com/tag/world/page/1\n│   ├── https://quotes.toscrape.com/tag/love\n│   ├── https://quotes.toscrape.com/tag/inspirational\n│   ├── https://quotes.toscrape.com/tag/life\n│   ├── https://quotes.toscrape.com/tag/humor\n│   ├── https://quotes.toscrape.com/tag/books\n│   ├── https://quotes.toscrape.com/tag/reading\n│   ├── https://quotes.toscrape.com/tag/friendship\n│   ├── https://quotes.toscrape.com/tag/friends\n│   ├── https://quotes.toscrape.com/tag/truth\n│   └── https://quotes.toscrape.com/tag/simile\n├── https://quotes.toscrape.com/author/J-K-Rowling\n├── https://quotes.toscrape.com/tag/abilities/page/1\n│   └── https://quotes.toscrape.com/tag/choices/page/1\n├── https://quotes.toscrape.com/tag/inspirational/page/1\n│   ├── https://quotes.toscrape.com/tag/life/page/1\n│   ├── https://quotes.toscrape.com/tag/live/page/1\n│   ├── https://quotes.toscrape.com/tag/miracle/page/1\n│   ├── https://quotes.toscrape.com/tag/miracles/page/1\n│   ├── https://quotes.toscrape.com/author/Marilyn-Monroe\n│   ├── https://quotes.toscrape.com/tag/be-yourself/page/1\n│   ├── https://quotes.toscrape.com/author/Thomas-A-Edison\n│   ├── https://quotes.toscrape.com/tag/edison/page/1\n│   ├── https://quotes.toscrape.com/tag/failure/page/1\n│   ├── https://quotes.toscrape.com/tag/paraphrased/page/1\n│   ├── https://quotes.toscrape.com/tag/friends/page/1\n│   ├── https://quotes.toscrape.com/tag/heartbreak/page/1\n│   ├── https://quotes.toscrape.com/tag/love/page/1\n│   ├── https://quotes.toscrape.com/tag/sisters/page/1\n│   ├── https://quotes.toscrape.com/author/Elie-Wiesel\n│   ├── https://quotes.toscrape.com/tag/activism/page/1\n│   ├── https://quotes.toscrape.com/tag/apathy/page/1\n│   ├── https://quotes.toscrape.com/tag/hate/page/1\n│   ├── https://quotes.toscrape.com/tag/indifference/page/1\n│   ├── https://quotes.toscrape.com/tag/opposite/page/1\n│   ├── https://quotes.toscrape.com/tag/philosophy/page/1\n│   ├── https://quotes.toscrape.com/tag/death/page/1\n│   ├── https://quotes.toscrape.com/author/George-Eliot\n│   ├── https://quotes.toscrape.com/author/C-S-Lewis\n│   ├── https://quotes.toscrape.com/tag/books/page/1\n│   ├── https://quotes.toscrape.com/tag/reading/page/1\n│   ├── https://quotes.toscrape.com/tag/tea/page/1\n│   ├── https://quotes.toscrape.com/author/Martin-Luther-King-Jr\n│   ├── https://quotes.toscrape.com/tag/hope/page/1\n│   ├── https://quotes.toscrape.com/author/Helen-Keller\n│   └── https://quotes.toscrape.com/tag/inspirational/page/2\n├── https://quotes.toscrape.com/author/Jane-Austen\n├── https://quotes.toscrape.com/tag/aliteracy/page/1\n│   ├── https://quotes.toscrape.com/tag/classic/page/1\n│   └── https://quotes.toscrape.com/tag/humor/page/1\n├── https://quotes.toscrape.com/tag/adulthood/page/1\n│   ├── https://quotes.toscrape.com/tag/success/page/1\n│   └── https://quotes.toscrape.com/tag/value/page/1\n├── https://quotes.toscrape.com/author/Andre-Gide\n├── https://quotes.toscrape.com/author/Eleanor-Roosevelt\n├── https://quotes.toscrape.com/tag/misattributed-eleanor-roosevelt/page/1\n├── https://quotes.toscrape.com/author/Steve-Martin\n├── https://quotes.toscrape.com/tag/obvious/page/1\n│   └── https://quotes.toscrape.com/tag/simile/page/1\n└── https://quotes.toscrape.com/page/2\n    ├── https://quotes.toscrape.com/tag/courage/page/1\n    ├── https://quotes.toscrape.com/tag/simplicity/page/1\n    ├── https://quotes.toscrape.com/tag/understand/page/1\n    ├── https://quotes.toscrape.com/author/Bob-Marley\n    ├── https://quotes.toscrape.com/author/Dr-Seuss\n    ├── https://quotes.toscrape.com/tag/fantasy/page/1\n    ├── https://quotes.toscrape.com/author/Douglas-Adams\n    ├── https://quotes.toscrape.com/tag/navigation/page/1\n    ├── https://quotes.toscrape.com/author/Friedrich-Nietzsche\n    ├── https://quotes.toscrape.com/tag/friendship/page/1\n    ├── https://quotes.toscrape.com/tag/lack-of-friendship/page/1\n    ├── https://quotes.toscrape.com/tag/lack-of-love/page/1\n    ├── https://quotes.toscrape.com/tag/marriage/page/1\n    ├── https://quotes.toscrape.com/tag/unhappy-marriage/page/1\n    ├── https://quotes.toscrape.com/author/Mark-Twain\n    ├── https://quotes.toscrape.com/tag/contentment/page/1\n    ├── https://quotes.toscrape.com/author/Allen-Saunders\n    ├── https://quotes.toscrape.com/tag/fate/page/1\n    ├── https://quotes.toscrape.com/tag/misattributed-john-lennon/page/1\n    ├── https://quotes.toscrape.com/tag/planning/page/1\n    ├── https://quotes.toscrape.com/tag/plans/page/1\n    ├── https://quotes.toscrape.com/page/1\n    └── https://quotes.toscrape.com/page/3",
     )
 
 
 @patch("builtins.print")
 def test_dynamic_tree(mock_print):
-    scraper.print_tree(scraper.tree_gen("http://quotes.toscrape.com/js/", 1))
+    quotesjs.print_tree(1)
     assert mock_print.call_args.args == (
         "http://quotes.toscrape.com/js\n├── http://quotes.toscrape.com\n├── http://quotes.toscrape.com/login\n├── http://quotes.toscrape.com/js/page/2\n├── https://goodreads.com/quotes\n└── https://scrapinghub.com",
     )
 
 
 @patch("builtins.print")
 def test_main(mock_print):
     cli_args = ["https://toscrape.com", "1"]
     main_out = main(cli_args)
     assert mock_print.call_args.args == (
         "https://toscrape.com\n├── http://books.toscrape.com\n├── http://quotes.toscrape.com\n├── http://quotes.toscrape.com/scroll\n├── http://quotes.toscrape.com/js\n├── http://quotes.toscrape.com/js-delayed\n├── http://quotes.toscrape.com/tableful\n├── http://quotes.toscrape.com/login\n├── http://quotes.toscrape.com/search.aspx\n└── http://quotes.toscrape.com/random",
     )
-    assert main_out[0]  # in [191320, 230509]
+    assert main_out[0]
     assert main_out[1] == 3
     assert main_out[2] == [0, 0]
     assert main_out[3] == 2
     rmtree(download_dir)
```

### Comparing `easierscrape-0.1.3/easierscrape.egg-info/PKG-INFO` & `easierscrape-0.2.0/easierscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.1.3
+Version: 0.2.0
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,41 +246,42 @@
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
 
 ## Basic Usage
 Install with pip: `pip install easierscrape`
 
-Import `Scraper` from `easierscrape` as seen below and then call class methods to scrape varying resources:
+Import `Scraper` from `easierscrape` and instantiate it with a url as seen below:
 ```python
 from easierscrape import Scraper
 
-scraper = Scraper()
+scraper = Scraper("https://quotes.toscrape.com/login")
 ```
+From there, call class methods to scrape varying resources.
 
 Usage examples:
 ```
->>> scraper.parse_text("https://quotes.toscrape.com/login")
+>>> scraper.parse_text()
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
 
->>> scraper.print_tree(scraper.tree_gen("https://toscrape.com/", 1))
+>>> scraper.print_tree(1)
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
-When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
+When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
 usage: python -m easierscrape [-h] url depth
 
 positional arguments:
   url         the url to scrape
   depth       the depth of the scrape tree
 
@@ -300,12 +301,12 @@
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Contributing
 
-See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
+See [CONTRIBUTING](https://github.com/dag2226/easierscrape/blob/main/CONTRIBUTING.md) for more information.
 
 ## License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](./LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://github.com/dag2226/easierscrape/blob/main/LICENSE) for more information.
```

### Comparing `easierscrape-0.1.3/easierscrape.egg-info/SOURCES.txt` & `easierscrape-0.2.0/easierscrape.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 pyproject.toml
 setup.py
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/requirements.txt
-docs/_build/html/_images/cli_recording.gif
-docs/_build/html/_images/demo_recording.gif
-docs/_build/html/_sources/index.md.txt
-docs/_build/html/_sources/source/easierscrape.rst.txt
-docs/_build/html/_sources/source/modules.rst.txt
 docs/images/cli_recording.gif
 docs/images/demo_recording.gif
 docs/source/easierscrape.rst
 docs/source/modules.rst
 easierscrape/__init__.py
 easierscrape/__main__.py
 easierscrape/_version.py
```

### Comparing `easierscrape-0.1.3/pyproject.toml` & `easierscrape-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "easierscrape"
 authors = [{name = "Daniel Greco", email = "dag2226@columbia.edu"}]
 description="A library which does some basic web scraping operations"
 readme = "README.md"
-version = "0.1.3"
+version = "0.2.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "anytree",
     "beautifulsoup4",
-    "html5lib",
     "lxml",
+    "openpyxl",
     "pandas",
     "selenium",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

