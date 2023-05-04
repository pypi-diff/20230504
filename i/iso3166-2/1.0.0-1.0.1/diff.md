# Comparing `tmp/iso3166-2-1.0.0.tar.gz` & `tmp/iso3166-2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-2-1.0.0.tar", last modified: Mon Apr 17 08:56:26 2023, max compression
+gzip compressed data, was "iso3166-2-1.0.1.tar", last modified: Thu May  4 21:48:53 2023, max compression
```

## Comparing `iso3166-2-1.0.0.tar` & `iso3166-2-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1089432 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/iso3166-2-min.json
--rw-r--r--   0 runner    (1001) docker     (123)  2787107 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/iso3166-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 08:56:26.000000 iso3166-2-1.0.0/iso3166_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/tests/test_iso3166_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.112526 iso3166-2-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-04 21:48:53.116526 iso3166-2-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1578148 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2-min.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3357755 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166-2-data/iso3166-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/iso3166_2/iso3166_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.108526 iso3166-2-1.0.1/iso3166_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:48:51.000000 iso3166-2-1.0.1/iso3166_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 21:48:53.000000 iso3166-2-1.0.1/iso3166_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-04 21:48:53.116526 iso3166-2-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:53.112526 iso3166-2-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-05-04 21:48:38.000000 iso3166-2-1.0.1/tests/test_iso3166_2.py
```

### Comparing `iso3166-2-1.0.0/LICENSE` & `iso3166-2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-2-1.0.0/PKG-INFO` & `iso3166-2-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 Metadata-Version: 2.1
 Name: iso3166-2
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 Home-page: https://github.com/amckenna41/iso3166-2
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
 Description: # ISO3166-2
         
-        [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
-        [![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-2/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-2/actions)
+        [![iso3166_2](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
+        [![pytest](https://github.com/amckenna41/iso3166-2/workflows/Building%20and%20Testing%20%F0%9F%90%8D/badge.svg)](https://github.com/amckenna41/iso3166-2/actions?query=workflowBuilding%20and%20Testing%20%F0%9F%90%8D)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-2/)
         [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-2)](https://opensource.org/licenses/MIT)
         [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2/issues)
-        [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2)
-        [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2)
-        [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR)
+        <!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2) -->
+        <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2) -->
+        <!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
           <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
         </div>
         
-        > Custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][here].
+        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        iso3166-2 is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO3166-2 standard.
+        <b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
         
         The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
         
         Latest Updates
         --------------
-        An important thing to note about the ISO3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a subdivision. Therefore, it's important that this library and its jsons have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
+        An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
         
         The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
         
         Installaion
         -----------
-        Install the latest version of iso3166-2 via [PyPi][PyPi] using pip:
+        Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-2 --upgrade
         ```
         
         Installation from source:
         ```bash
@@ -67,17 +67,22 @@
         ------------
         * [python][python] >= 3.7
         * [requests][requests] >= 2.28.1
         * [iso3166][iso3166] >= 2.1.1
         
         Usage
         -----
-        Download all ISO3166-2 subdivision data using getISO3166_2.py script, export to two JSONs:
-        ```bash
+        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+        
+        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+        ```
         python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
+        
+        --json_filename: output filename for exported JSONs.
+        --output_folder: output folder to store JSONs.
         ```
         
         Import ISO3166_2 class and access the country and subdivision data:
         ```python
         import iso3166_2 as iso
         
         #access all country data
@@ -111,23 +116,23 @@
         denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
         estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
         fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
         ```
         
         Attributes
         ----------
-        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the json exports.
+        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
         
         Issues or Contributing
         ----------------------
-        Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Due to the nature of the ISO consistently updating the ISO3166-2 codes/names every year the data in the JSON's may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. 
+        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
         
         Contact
         -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
+        If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
         [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
         
         References
         ----------
         \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
         \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         
@@ -137,39 +142,21 @@
         
         [Back to top](#TOP)
         
         [python]: https://www.python.org/downloads/release/python-360/
         [requests]: https://requests.readthedocs.io/
         [iso3166]: https://github.com/deactivated/python-iso3166
         [pycountry]: https://github.com/flyingcircusio/pycountry
-        [PyPi]: https://pypi.org/project/pysar/
+        [rest]: https://restcountries.com/
+        [google-maps-api]: https://github.com/googlemaps/google-maps-services-python
+        [PyPi]: https://pypi.org/project/iso3166-2/
         [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
-        [colab]: https://github.com/amckenna41/iso3166-updates
+        [demo]: https://colab.research.google.com/drive/1btfEx23bgWdkUPiwdwlDqKkmUp1S-_7U?usp=sharing
         [attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
-        
-        <!-- https://github.com/annexare/Countries -->
-        
-        <!-- 
-        Look over below...
-        iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO3166-1 and ISO3166-2 country codes and naming conventions, as per the ISO3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which compromise the ISO3166-2 standard [[2]](#references). 
-        
-        **Problem Statement**
-        
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, this includes the ISO3166. Additions/changes/deletions to country/territorial codes in the ISO3166-1 are a lot less frequent, but changes are much more frequent for the ISO3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references), usually being released at the end of the year, with amendments and updates throughout the year. [[4]](#references)
-        
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO3166-2 codes for free with an easy to use interface and Python package.
-        This software is for anyone working on projects working directly with country codes and who want up-to-date and accurate ISO3166-2 codes and naming conventions.
-        
-        **Intended Audience**
-        This software and accompanying API is for anyone working with country data at the ISO3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). iso3166-updates not only 
-         
-        Also, it's aimed not just at developers of ISO3166 applications but for anyone working in that space, hence the creation of an easy to use API. 
-        
-        <em> The earliest date for any ISO3166 updates is 2000-06-21, and the most recent is 2022-11-29 </em> -->
-        
+        [issues]: https://github.com/amckenna41/iso3166-2/issues
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha2,iso3166-updates,rest countries
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
```

### Comparing `iso3166-2-1.0.0/README.md` & `iso3166-2-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # ISO3166-2
 
-[![iso3166_updates](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
-[![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-2/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-2/actions)
+[![iso3166_2](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
+[![pytest](https://github.com/amckenna41/iso3166-2/workflows/Building%20and%20Testing%20%F0%9F%90%8D/badge.svg)](https://github.com/amckenna41/iso3166-2/actions?query=workflowBuilding%20and%20Testing%20%F0%9F%90%8D)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-2/)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-2)](https://opensource.org/licenses/MIT)
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2/issues)
-[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2)
-[![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2)
-[![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR)
+<!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2) -->
+<!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2) -->
+<!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
   <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
-> Custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][here].
+> Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-iso3166-2 is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO3166-2 standard.
+<b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
 
 The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
 
 Latest Updates
 --------------
-An important thing to note about the ISO3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a subdivision. Therefore, it's important that this library and its jsons have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
+An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
 
 The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
 
 Installaion
 -----------
-Install the latest version of iso3166-2 via [PyPi][PyPi] using pip:
+Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-2 --upgrade
 ```
 
 Installation from source:
 ```bash
@@ -57,17 +57,22 @@
 ------------
 * [python][python] >= 3.7
 * [requests][requests] >= 2.28.1
 * [iso3166][iso3166] >= 2.1.1
 
 Usage
 -----
-Download all ISO3166-2 subdivision data using getISO3166_2.py script, export to two JSONs:
-```bash
+There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+
+The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+```
 python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
+
+--json_filename: output filename for exported JSONs.
+--output_folder: output folder to store JSONs.
 ```
 
 Import ISO3166_2 class and access the country and subdivision data:
 ```python
 import iso3166_2 as iso
 
 #access all country data
@@ -101,23 +106,23 @@
 denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
 estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
 fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
 ```
 
 Attributes
 ----------
-You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the json exports.
+You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
 
 Issues or Contributing
 ----------------------
-Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Due to the nature of the ISO consistently updating the ISO3166-2 codes/names every year the data in the JSON's may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. 
+Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
 
 Contact
 -------
-If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
+If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
 
 References
 ----------
 \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
 \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 
@@ -127,31 +132,14 @@
 
 [Back to top](#TOP)
 
 [python]: https://www.python.org/downloads/release/python-360/
 [requests]: https://requests.readthedocs.io/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [pycountry]: https://github.com/flyingcircusio/pycountry
-[PyPi]: https://pypi.org/project/pysar/
+[rest]: https://restcountries.com/
+[google-maps-api]: https://github.com/googlemaps/google-maps-services-python
+[PyPi]: https://pypi.org/project/iso3166-2/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
-[colab]: https://github.com/amckenna41/iso3166-updates
+[demo]: https://colab.research.google.com/drive/1btfEx23bgWdkUPiwdwlDqKkmUp1S-_7U?usp=sharing
 [attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
-
-<!-- https://github.com/annexare/Countries -->
-
-<!-- 
-Look over below...
-iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO3166-1 and ISO3166-2 country codes and naming conventions, as per the ISO3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which compromise the ISO3166-2 standard [[2]](#references). 
-
-**Problem Statement**
-
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, this includes the ISO3166. Additions/changes/deletions to country/territorial codes in the ISO3166-1 are a lot less frequent, but changes are much more frequent for the ISO3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references), usually being released at the end of the year, with amendments and updates throughout the year. [[4]](#references)
-
-This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO3166-2 codes for free with an easy to use interface and Python package.
-This software is for anyone working on projects working directly with country codes and who want up-to-date and accurate ISO3166-2 codes and naming conventions.
-
-**Intended Audience**
-This software and accompanying API is for anyone working with country data at the ISO3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). iso3166-updates not only 
- 
-Also, it's aimed not just at developers of ISO3166 applications but for anyone working in that space, hence the creation of an easy to use API. 
-
-<em> The earliest date for any ISO3166 updates is 2000-06-21, and the most recent is 2022-11-29 </em> -->
+[issues]: https://github.com/amckenna41/iso3166-2/issues
```

### Comparing `iso3166-2-1.0.0/iso3166_2/iso3166_2.py` & `iso3166-2-1.0.1/iso3166_2/iso3166_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import iso3166
 
 class ISO3166_2():
     """
     This class is used to access all the ISO-3166 and ISO-3166-2 country data and attributes.
     There are two JSON's available in the package, iso3166-2-min.json and iso3166-2.json. The 
     former is a minified JSON of all country's ISO3166-2 subdivision info including subdivision
-    name, code, parent code and type. The latter contains a verbose collection of all country 
-    data pulled from the restcountries API as well as the country's subdivision data appened to 
-    each. Both JSONs are generated using the getISO3166_2.py script in the main directory. All 
-    of the keys and objects in the JSON are accessible via dot notation using the Map class.
+    name, type, code, parent code, lat/longitude and URL to its flag (if applicable). The latter 
+    contains a verbose collection of all country data pulled from the restcountries API as well 
+    as the country's subdivision data appened to each. Both JSONs are generated using the 
+    getISO3166_2.py script in the main directory. All of the keys and objects in the JSON are 
+    accessible via dot notation using the Map class.
     
     Parameters
     ----------
-    :iso3166_json_filename : str (default=iso3166-2-min.json)
+    : iso3166_json_filename : str (default=iso3166-2-min.json)
         filename of iso3166-2 JSON data to import from data folder. Can either be the
         iso3166-2-min or iso3166-2 JSON files. 
 
     Usage
     -----
     import iso3166_2 as iso
```

### Comparing `iso3166-2-1.0.0/iso3166_2.egg-info/PKG-INFO` & `iso3166-2-1.0.1/iso3166_2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 Metadata-Version: 2.1
 Name: iso3166-2
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 Home-page: https://github.com/amckenna41/iso3166-2
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
 Description: # ISO3166-2
         
-        [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
-        [![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-2/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-2/actions)
+        [![iso3166_2](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
+        [![pytest](https://github.com/amckenna41/iso3166-2/workflows/Building%20and%20Testing%20%F0%9F%90%8D/badge.svg)](https://github.com/amckenna41/iso3166-2/actions?query=workflowBuilding%20and%20Testing%20%F0%9F%90%8D)
         [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-2/)
         [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-2)](https://opensource.org/licenses/MIT)
         [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2/issues)
-        [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2)
-        [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2)
-        [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR)
+        <!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2) -->
+        <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2) -->
+        <!-- [![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR) -->
         
         <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
           <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
           <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
         </div>
         
-        > Custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][here].
+        > Custom-built Python wrapper for RestCountries API (https://restcountries.com/) which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
-        iso3166-2 is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO3166-2 standard.
+        <b>iso3166-2</b> is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO 3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO 3166-2 standard.
         
         The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
         
         Latest Updates
         --------------
-        An important thing to note about the ISO3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a subdivision. Therefore, it's important that this library and its jsons have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
+        An important thing to note about the ISO 3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a whole subdivision. Therefore, it's important that this library and its JSONs have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
         
         The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
         
         Installaion
         -----------
-        Install the latest version of iso3166-2 via [PyPi][PyPi] using pip:
+        Install the latest version of `iso3166-2` via [PyPi][PyPi] using pip:
         
         ```bash
         pip3 install iso3166-2 --upgrade
         ```
         
         Installation from source:
         ```bash
@@ -67,17 +67,22 @@
         ------------
         * [python][python] >= 3.7
         * [requests][requests] >= 2.28.1
         * [iso3166][iso3166] >= 2.1.1
         
         Usage
         -----
-        Download all ISO3166-2 subdivision data using getISO3166_2.py script, export to two JSONs:
-        ```bash
+        There are two main JSONs that `iso3166-2` utilises, <i>iso3166-2.json</i> and <i>iso3166-2-min.json</i>. The first JSON contains all country information, including all data pulled from the restcountries API as well as the country's subdivision data, this file is <b>3.4 MB</b>. The <i>iso3166-2-min.json</i> file is a minimised version of the first JSON, only containing each country's ISO3166-2 data, this file is <b>1.6 MB</b>. In the main module <i>iso3166_2.py</i>, all data from the <i>iso3166-2.json</i> is accessible via the `iso.country` object and all data from the <i>iso3166-2-min.json</i> is accessible via the `iso.subdivisions` object.
+        
+        The script `getISO3166_2.py` is used for gathering and exporting all country and subdivision data to the mentioned JSONs. It uses the restcountries api and pycountry package to assemble all of the data together. To download all of the latest ISO 3166-2 subdivision data run the `getISO3166_2.py` in a terminal or cmd, the script takes around 2 hours to execute (the script requires the additional pacakges: pycountry, tqdm and googlemaps):
+        ```
         python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
+        
+        --json_filename: output filename for exported JSONs.
+        --output_folder: output folder to store JSONs.
         ```
         
         Import ISO3166_2 class and access the country and subdivision data:
         ```python
         import iso3166_2 as iso
         
         #access all country data
@@ -111,23 +116,23 @@
         denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
         estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
         fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
         ```
         
         Attributes
         ----------
-        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the json exports.
+        You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the JSIN exports.
         
         Issues or Contributing
         ----------------------
-        Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Due to the nature of the ISO consistently updating the ISO3166-2 codes/names every year the data in the JSON's may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. 
+        Any issues, errors or bugs can be raised via the [Issues][issues] tab in the repository. Due to the nature of the ISO consistently updating the ISO 3166-2 codes/names every year the data in the JSONs may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. Although, if you notice any out of date or missing subdivision info then please similarly raise an Issue in the [Issues][issues] tab.
         
         Contact
         -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
+        If you have any questions or comments, please contact amckenna41@qub.ac.uk. <br><br>
         [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
         
         References
         ----------
         \[1\]: https://en.wikipedia.org/wiki/ISO_3166 <br>
         \[2\]: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
         
@@ -137,39 +142,21 @@
         
         [Back to top](#TOP)
         
         [python]: https://www.python.org/downloads/release/python-360/
         [requests]: https://requests.readthedocs.io/
         [iso3166]: https://github.com/deactivated/python-iso3166
         [pycountry]: https://github.com/flyingcircusio/pycountry
-        [PyPi]: https://pypi.org/project/pysar/
+        [rest]: https://restcountries.com/
+        [google-maps-api]: https://github.com/googlemaps/google-maps-services-python
+        [PyPi]: https://pypi.org/project/iso3166-2/
         [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
-        [colab]: https://github.com/amckenna41/iso3166-updates
+        [demo]: https://colab.research.google.com/drive/1btfEx23bgWdkUPiwdwlDqKkmUp1S-_7U?usp=sharing
         [attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
-        
-        <!-- https://github.com/annexare/Countries -->
-        
-        <!-- 
-        Look over below...
-        iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO3166-1 and ISO3166-2 country codes and naming conventions, as per the ISO3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which compromise the ISO3166-2 standard [[2]](#references). 
-        
-        **Problem Statement**
-        
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, this includes the ISO3166. Additions/changes/deletions to country/territorial codes in the ISO3166-1 are a lot less frequent, but changes are much more frequent for the ISO3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform or Online Browsing Platform or via a database, which usually costs money to subscribe to [[3]](#references), usually being released at the end of the year, with amendments and updates throughout the year. [[4]](#references)
-        
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of countrys' ISO3166-2 codes for free with an easy to use interface and Python package.
-        This software is for anyone working on projects working directly with country codes and who want up-to-date and accurate ISO3166-2 codes and naming conventions.
-        
-        **Intended Audience**
-        This software and accompanying API is for anyone working with country data at the ISO3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). iso3166-updates not only 
-         
-        Also, it's aimed not just at developers of ISO3166 applications but for anyone working in that space, hence the creation of an easy to use API. 
-        
-        <em> The earliest date for any ISO3166 updates is 2000-06-21, and the most recent is 2022-11-29 </em> -->
-        
+        [issues]: https://github.com/amckenna41/iso3166-2/issues
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha2,iso3166-updates,rest countries
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
```

### Comparing `iso3166-2-1.0.0/setup.cfg` & `iso3166-2-1.0.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-2
-version = 1.0.0
+version = 1.0.1
 description = A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amckenna41/iso3166-2
 download_url = https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
```

### Comparing `iso3166-2-1.0.0/setup.py` & `iso3166-2-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-2'
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __description__ = "A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __maintainer__ = "AJ McKenna"
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-2'
 __download_url__ = "https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip"
@@ -59,13 +59,14 @@
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
       install_requires=[
           'requests>=2.28.1',
-          'iso3166'
+          'iso3166',
+          'googlemaps'
       ],
      test_suite=__test_suite__,
      packages=find_packages(),
      include_package_data=True,
      zip_safe=False)
```

### Comparing `iso3166-2-1.0.0/tests/test_iso3166_2.py` & `iso3166-2-1.0.1/tests/test_iso3166_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import iso3166_2 as iso
 import iso3166
 import requests
 import json
 import os
 import getpass
-import importlib_metadata as metadata
+from importlib import metadata
+try:
+    from importlib import metadata
+except ImportError:
+    import importlib_metadata as metadata  
 import unittest
 unittest.TestLoader.sortTestMethodsUsing = None
 
 __version__ = "1.0.0"
 
 class ISO3166_2_Updates(unittest.TestCase):
 
@@ -28,15 +32,15 @@
 
         #base url for flag icons on iso3166-flag-icons repo
         self.flag_icons_base_url = "https://github.com/amckenna41/iso3166-flag-icons/blob/main/iso3166-2-icons/"
 
     @unittest.skip("")
     def test_iso3166_2_metadata(self): 
         """ Testing correct iso3166-2 software version and metadata. """
-        self.assertEqual(metadata.metadata('iso3166-2')['version'], "1.0.0", 
+        self.assertEqual(metadata.metadata('iso3166-2')['version'], "1.0.1", 
             "iso3166-2 version is not correct, got: {}".format(metadata.metadata('iso3166-2')['version']))
         self.assertEqual(metadata.metadata('iso3166-2')['name'], "iso3166-2", 
             "iso3166-2 software name is not correct, got: {}".format(metadata.metadata('iso3166-2')['name']))
         self.assertEqual(metadata.metadata('iso3166-2')['author'], 
             "AJ McKenna, https://github.com/amckenna41", "iso3166-updates author is not correct, got: {}".format(metadata.metadata('iso3166_2')['author']))
         self.assertEqual(metadata.metadata('iso3166-2')['author-email'], 
             "amckenna41@qub.ac.uk", "iso3166-updates author email is not correct, got: {}".format(metadata.metadata('iso3166_2')['author-email']))
@@ -100,14 +104,15 @@
         self.assertEqual(test_alpha2_au.cca3, "AUS")        
         self.assertEqual(test_alpha2_au.currencies.AUD['name'], "Australian dollar")        
         self.assertEqual(test_alpha2_au.capital[0], "Canberra")        
         self.assertEqual(test_alpha2_au.region, "Oceania")        
         self.assertEqual(list(test_alpha2_au.languages.keys())[0], "eng")        
         self.assertEqual(test_alpha2_au.area, 7692024)        
         self.assertEqual(test_alpha2_au.population, 25687041)        
+        self.assertEqual(test_alpha2_au.latlng, [-27.0, 133.0], "")        
         self.assertEqual(len(test_alpha2_au.subdivisions), 8, "")
         self.assertEqual(test_alpha2_au, iso.country['AUS']) #test objects match if using either alpha2/alpha3 codes
 #2.)
         self.assertIsInstance(test_alpha2_lu, dict, "")
         self.assertEqual(len(test_alpha2_lu), 36, "")
         self.assertEqual(test_alpha2_lu.name.common, "Luxembourg")        
         self.assertEqual(test_alpha2_lu.cca2, "LU")        
@@ -115,41 +120,44 @@
         self.assertEqual(test_alpha2_lu.currencies.EUR['name'], "Euro")        
         self.assertEqual(test_alpha2_lu.capital[0], "Luxembourg")        
         self.assertEqual(test_alpha2_lu.region, "Europe")        
         self.assertEqual(list(test_alpha2_lu.languages.keys()), ["deu", "fra", "ltz"])        
         self.assertEqual(test_alpha2_lu.area, 2586)        
         self.assertEqual(test_alpha2_lu.population, 632275)        
         self.assertEqual(len(test_alpha2_lu.subdivisions), 12, "")
+        self.assertEqual(test_alpha2_lu.latlng, [49.75, 6.16666666], "")        
         self.assertEqual(test_alpha2_lu, iso.country['LUX']) #test objects match if using either alpha2/alpha3 codes
 #3.)
         self.assertIsInstance(test_alpha2_mg, dict, "")
         self.assertEqual(len(test_alpha2_mg), 35, "")
         self.assertEqual(test_alpha2_mg.name.common, "Madagascar")        
         self.assertEqual(test_alpha2_mg.cca2, "MG")        
         self.assertEqual(test_alpha2_mg.cca3, "MDG")        
         self.assertEqual(test_alpha2_mg.currencies.MGA['name'], "Malagasy ariary")        
         self.assertEqual(test_alpha2_mg.capital[0], "Antananarivo")        
         self.assertEqual(test_alpha2_mg.region, "Africa")        
         self.assertEqual(list(test_alpha2_mg.languages.keys()), ["fra", "mlg"])        
         self.assertEqual(test_alpha2_mg.area, 587041)        
         self.assertEqual(test_alpha2_mg.population, 27691019)        
+        self.assertEqual(test_alpha2_mg.latlng, [-20.0, 47.0], "")        
         self.assertEqual(len(test_alpha2_mg.subdivisions), 6, "")
         self.assertEqual(test_alpha2_mg, iso.country['MDG']) #test objects match if using either alpha2/alpha3 codes
 #4.)
         self.assertIsInstance(test_alpha2_om, dict, "")
         self.assertEqual(len(test_alpha2_om), 35, "")
         self.assertEqual(test_alpha2_om.name.common, "Oman")        
         self.assertEqual(test_alpha2_om.cca2, "OM")        
         self.assertEqual(test_alpha2_om.cca3, "OMN")        
         self.assertEqual(test_alpha2_om.currencies.OMR['name'], "Omani rial")        
         self.assertEqual(test_alpha2_om.capital[0], "Muscat")        
         self.assertEqual(test_alpha2_om.region, "Asia")        
         self.assertEqual(list(test_alpha2_om.languages.keys()), ["ara"])        
         self.assertEqual(test_alpha2_om.area, 309500)        
         self.assertEqual(test_alpha2_om.population, 5106622)        
+        self.assertEqual(test_alpha2_om.latlng, [21.0, 57.0], "")        
         self.assertEqual(len(test_alpha2_om.subdivisions), 11, "")
         self.assertEqual(test_alpha2_om, iso.country['OMN']) #test objects match if using either alpha2/alpha3 codes
 #5.)
         with (self.assertRaises(ValueError)):
             invalid_country = iso.country["ZZ"]
             invalid_country = iso.country["XY"]
             invalid_country = iso.country["XYZ"]
@@ -167,66 +175,74 @@
         test_alpha2_rw = iso.subdivisions["RW"] #Rwanda
 #1.)    
         ba_subdivision_codes = ['BA-BIH', 'BA-BRC', 'BA-SRP']
         ba_subdivision_names = ['Federacija Bosne i Hercegovine', 'Brčko distrikt', 'Republika Srpska']
         self.assertIsInstance(test_alpha2_ba, dict)
         self.assertEqual(len(test_alpha2_ba), 3)
         self.assertEqual(list(test_alpha2_ba.keys()), ba_subdivision_codes)
-        self.assertEqual(list(test_alpha2_ba['BA-BIH'].keys()), ['name', 'type', 'parent_code', 'flag_url'])
+        self.assertEqual(list(test_alpha2_ba['BA-BIH'].keys()), ['name', 'type', 'parent_code', 'latlng', 'flag_url'])
         for key in test_alpha2_ba:
             self.assertIn(test_alpha2_ba[key].name, ba_subdivision_names)
             if ((test_alpha2_ba[key].flag_url is not None) or (test_alpha2_ba[key].flag_url == "")):
                 self.assertEqual(requests.get(test_alpha2_ba[key].flag_url, headers=self.user_agent_header).status_code, 200)
+            self.assertIsNone(test_alpha2_ba[key]['parent_code'], "")
+            self.assertEqual(len(test_alpha2_ba[key].latlng), 2, "")        
 #2.)
         cy_subdivision_codes = ['CY-01', 'CY-02', 'CY-03', 'CY-04', 'CY-05', 'CY-06']
         cy_subdivision_names = ['Lefkosia', 'Lemesos', 'Larnaka', 'Ammochostos', 'Baf', 'Girne']
         self.assertIsInstance(test_alpha2_cy, dict)
         self.assertEqual(len(test_alpha2_cy), 6)
         self.assertEqual(list(test_alpha2_cy.keys()), cy_subdivision_codes)
-        self.assertEqual(list(test_alpha2_cy['CY-01'].keys()), ['name', 'type', 'parent_code', 'flag_url'])
+        self.assertEqual(list(test_alpha2_cy['CY-01'].keys()), ['name', 'type', 'parent_code', 'latlng', 'flag_url'])
         for key in test_alpha2_cy:
             self.assertIn(test_alpha2_cy[key].name, cy_subdivision_names)
             if ((test_alpha2_cy[key].flag_url is not None) or (test_alpha2_cy[key].flag_url == "")):
                 self.assertEqual(requests.get(test_alpha2_cy[key].flag_url, headers=self.user_agent_header).status_code, 200)
+            self.assertIsNone(test_alpha2_cy[key]['parent_code'], "")
+            self.assertEqual(len(test_alpha2_cy[key].latlng), 2, "")        
 #3.)
         ga_subdivision_codes = ['GA-1', 'GA-2', 'GA-3', 'GA-4', 'GA-5', 'GA-6', 'GA-7', 'GA-8', 'GA-9']
         ga_subdivision_names = ['Estuaire', 'Haut-Ogooué', 'Moyen-Ogooué', 'Ngounié', 'Nyanga', 'Ogooué-Ivindo', 
             'Ogooué-Lolo', 'Ogooué-Maritime', 'Woleu-Ntem']
         self.assertIsInstance(test_alpha2_ga, dict)
         self.assertEqual(len(test_alpha2_ga), 9)
         self.assertEqual(list(test_alpha2_ga.keys()), ga_subdivision_codes)
-        self.assertEqual(list(test_alpha2_ga['GA-1'].keys()), ['name', 'type', 'parent_code', 'flag_url'])
+        self.assertEqual(list(test_alpha2_ga['GA-1'].keys()), ['name', 'type', 'parent_code', 'latlng', 'flag_url'])
         for key in test_alpha2_ga:
             self.assertIn(test_alpha2_ga[key].name, ga_subdivision_names)
             if ((test_alpha2_ga[key].flag_url is not None) or (test_alpha2_ga[key].flag_url == "")):
                 self.assertEqual(requests.get(test_alpha2_ga[key].flag_url, headers=self.user_agent_header).status_code, 200)
+            self.assertIsNone(test_alpha2_ga[key]['parent_code'], "")
+            self.assertEqual(len(test_alpha2_ga[key].latlng), 2, "")        
 #4.)
         rw_subdivision_codes = ['RW-01', 'RW-02', 'RW-03', 'RW-04', 'RW-05']
         rw_subdivision_names = ['City of Kigali', 'Eastern', 'Northern', 'Western', 'Southern']
+        rw_latlng = [[], [], [], [], []]
         self.assertIsInstance(test_alpha2_rw, dict)
         self.assertEqual(len(test_alpha2_rw), 5)
         self.assertEqual(list(test_alpha2_rw.keys()), rw_subdivision_codes)
-        self.assertEqual(list(test_alpha2_rw['RW-01'].keys()), ['name', 'type', 'parent_code', 'flag_url'])
+        self.assertEqual(list(test_alpha2_rw['RW-01'].keys()), ['name', 'type', 'parent_code', 'latlng', 'flag_url'])
         for key in test_alpha2_rw:
             self.assertIn(test_alpha2_rw[key].name, rw_subdivision_names)
             if ((test_alpha2_rw[key].flag_url is not None) or (test_alpha2_rw[key].flag_url == "")):
                 self.assertEqual(requests.get(test_alpha2_rw[key].flag_url, headers=self.user_agent_header).status_code, 200)
+        self.assertIsNone(test_alpha2_rw[key]['parent_code'], "")
+        self.assertEqual(len(test_alpha2_rw[key].latlng), 2, "")        
 #5.)
         with (self.assertRaises(ValueError)):
             invalid_country = iso.subdivisions["ZZ"]
             invalid_country = iso.subdivisions["XY"]
             invalid_country = iso.subdivisions["XYZ"]
 #6.)
         with (self.assertRaises(TypeError)):
             invalid_country = iso.subdivisions[123]
             invalid_country = iso.subdivisions[0.5]
             invalid_country = iso.subdivisions[False]
 
     def tearDown(self):
         """ Delete all iso3166-2 json objects or instances. """
-        # del self.all_subdivisions
         del self.all_iso3166_2_data
         del self.all_iso3166_2_min_data
     
 if __name__ == '__main__':
     #run all unit tests
     unittest.main(verbosity=2)
```

