# Comparing `tmp/pdfschedule-0.3.4.tar.gz` & `tmp/pdfschedule-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfschedule-0.3.4.tar", last modified: Sun Feb  6 21:13:08 2022, max compression
+gzip compressed data, was "pdfschedule-0.4.0.tar", last modified: Wed May  3 22:58:04 2023, max compression
```

## Comparing `pdfschedule-0.3.4.tar` & `pdfschedule-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     1078 2022-02-06 21:13:01.000000 pdfschedule-0.3.4/CHANGELOG.md
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     1101 2022-02-06 21:13:01.000000 pdfschedule-0.3.4/LICENSE
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      131 2020-11-26 03:26:11.000000 pdfschedule-0.3.4/MANIFEST.in
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     6378 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/PKG-INFO
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     5205 2022-02-06 21:12:45.000000 pdfschedule-0.3.4/README.rst
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/examples/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      209 2022-02-06 21:06:50.000000 pdfschedule-0.3.4/examples/Makefile
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     2724 2022-02-06 21:10:13.000000 pdfschedule-0.3.4/examples/example01.pdf
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    27778 2022-02-06 21:10:13.000000 pdfschedule-0.3.4/examples/example01.png
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      467 2019-05-27 21:29:23.000000 pdfschedule-0.3.4/examples/example01.yml
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      118 2020-11-25 18:56:18.000000 pdfschedule-0.3.4/pyproject.toml
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     1344 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/setup.cfg
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/src/
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2022-02-06 21:13:08.164270 pdfschedule-0.3.4/src/pdfschedule.egg-info/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     6378 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/PKG-INFO
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      418 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/SOURCES.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)        1 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/dependency_links.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       50 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/entry_points.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       55 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/requires.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       12 2022-02-06 21:13:08.000000 pdfschedule-0.3.4/src/pdfschedule.egg-info/top_level.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    13032 2022-02-06 21:13:01.000000 pdfschedule-0.3.4/src/pdfschedule.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      465 2022-02-06 21:11:01.000000 pdfschedule-0.3.4/tox.ini
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-05-03 22:58:04.120664 pdfschedule-0.4.0/
+-rw-r--r--   0 jwodder    (501) staff       (20)     1290 2023-05-03 22:57:57.000000 pdfschedule-0.4.0/CHANGELOG.md
+-rw-r--r--   0 jwodder    (501) staff       (20)     1118 2023-05-03 22:57:57.000000 pdfschedule-0.4.0/LICENSE
+-rw-r--r--   0 jwodder    (501) staff       (20)      131 2021-06-12 00:52:02.000000 pdfschedule-0.4.0/MANIFEST.in
+-rw-r--r--   0 jwodder    (501) staff       (20)     7259 2023-05-03 22:58:04.120817 pdfschedule-0.4.0/PKG-INFO
+-rw-r--r--   0 jwodder    (501) staff       (20)     6148 2023-05-03 22:57:48.000000 pdfschedule-0.4.0/README.rst
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-05-03 22:58:04.116919 pdfschedule-0.4.0/examples/
+-rw-r--r--   0 jwodder    (501) staff       (20)      209 2021-06-12 00:52:02.000000 pdfschedule-0.4.0/examples/Makefile
+-rw-r--r--   0 jwodder    (501) staff       (20)     2724 2020-11-22 23:55:02.000000 pdfschedule-0.4.0/examples/example01.pdf
+-rw-r--r--   0 jwodder    (501) staff       (20)    27778 2020-11-22 23:55:02.000000 pdfschedule-0.4.0/examples/example01.png
+-rw-r--r--   0 jwodder    (501) staff       (20)      467 2020-11-22 23:55:02.000000 pdfschedule-0.4.0/examples/example01.yml
+-rw-r--r--   0 jwodder    (501) staff       (20)       91 2022-07-07 12:48:58.000000 pdfschedule-0.4.0/pyproject.toml
+-rw-r--r--   0 jwodder    (501) staff       (20)     1313 2023-05-03 22:58:04.121462 pdfschedule-0.4.0/setup.cfg
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-05-03 22:58:04.117587 pdfschedule-0.4.0/src/
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-05-03 22:58:04.120338 pdfschedule-0.4.0/src/pdfschedule.egg-info/
+-rw-r--r--   0 jwodder    (501) staff       (20)     7259 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/PKG-INFO
+-rw-r--r--   0 jwodder    (501) staff       (20)      418 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/SOURCES.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)        1 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/dependency_links.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       49 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/entry_points.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       55 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/requires.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       12 2023-05-03 22:58:04.000000 pdfschedule-0.4.0/src/pdfschedule.egg-info/top_level.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)    13537 2023-05-03 22:57:57.000000 pdfschedule-0.4.0/src/pdfschedule.py
+-rw-r--r--   0 jwodder    (501) staff       (20)      461 2022-12-26 21:57:17.000000 pdfschedule-0.4.0/tox.ini
```

### Comparing `pdfschedule-0.3.4/CHANGELOG.md` & `pdfschedule-0.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v0.4.0 (2023-05-03)
+-------------------
+- Drop support for Python 3.6
+- Support Python 3.11
+- Added `--start-time` and `--end-time` command-line options
+  (contributed by [@bikdney](https://github.com/bikdney))
+
 v0.3.4 (2022-02-06)
 -------------------
 - Support PyYAML 6.0
 
 v0.3.3 (2021-06-12)
 -------------------
 - Fix error message displayed when an event is missing a "days" or "time" field
```

### Comparing `pdfschedule-0.3.4/LICENSE` & `pdfschedule-0.4.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2014, 2017-2022 John Thorvald Wodder II
+Copyright (c) 2014, 2017-2023 John Thorvald Wodder II and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pdfschedule-0.3.4/PKG-INFO` & `pdfschedule-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: pdfschedule
-Version: 0.3.4
+Version: 0.4.0
 Summary: Weekly schedule typesetter
 Home-page: https://github.com/jwodder/schedule
 Author: John Thorvald Wodder II
 Author-email: pdfschedule@varonathe.org
 License: MIT
 Project-URL: Source Code, https://github.com/jwodder/schedule
 Project-URL: Bug Tracker, https://github.com/jwodder/schedule/issues
 Keywords: pdf,schedule,week
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Topic :: Printing
-Requires-Python: ~=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
@@ -47,15 +45,15 @@
 
 ``pdfschedule`` is a Python 3 script for creating PDF documents showing
 one's weekly schedule of events.
 
 
 Installation
 ============
-``pdfschedule`` requires Python 3.6 or higher.  Just use `pip
+``pdfschedule`` requires Python 3.7 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``pdfschedule`` and its dependencies::
 
     python3 -m pip install pdfschedule
 
 
 Usage
@@ -73,14 +71,22 @@
 
 Options
 -------
 
 -C, --color             Color the event boxes various colors instead of just
                         grey.
 
+-E TIME, --end-time TIME
+                        Specify the time of day at which each day should start.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour before the earliest
+                        event start time or 00:00, whichever is later.
+
 -F FONT, --font FONT    Typeset text in the given font.  ``FONT`` must be
                         either the name of a builtin PostScript font or the
                         path to a ``.ttf`` file.  By default, text is typeset
                         in Helvetica.
 
 -f SIZE, --font-size SIZE
                         Set the size of the font used for event information to
@@ -96,14 +102,22 @@
                         to typeset it in "landscape mode."
 
 -s FACTOR, --scale FACTOR
                         Divide the length of each side of the table by
                         ``FACTOR``.  Without this option, the table fills the
                         whole page, except for a one-inch margin on each side.
 
+-S TIME, --start-time TIME
+                        Specify the time of day at which each day should end.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour after the latest
+                        event end time or 24:00, whichever is earlier.
+
 -T, --no-times          Do not show the times for each hour line.
 
 --no-weekends           Do not show Sunday and Saturday.
 
 
 Input Format
 ============
@@ -182,10 +196,8 @@
     - name: Sleep in
       days: SatSun
       time: 7-12
       color: "4226C4"
 
 produces (using the default options) an output file that looks like this:
 
-.. image:: https://github.com/jwodder/schedule/raw/v0.3.4/examples/example01.png
-
-
+.. image:: https://github.com/jwodder/schedule/raw/v0.4.0/examples/example01.png
```

### Comparing `pdfschedule-0.3.4/README.rst` & `pdfschedule-0.4.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ``pdfschedule`` is a Python 3 script for creating PDF documents showing
 one's weekly schedule of events.
 
 
 Installation
 ============
-``pdfschedule`` requires Python 3.6 or higher.  Just use `pip
+``pdfschedule`` requires Python 3.7 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``pdfschedule`` and its dependencies::
 
     python3 -m pip install pdfschedule
 
 
 Usage
@@ -43,14 +43,22 @@
 
 Options
 -------
 
 -C, --color             Color the event boxes various colors instead of just
                         grey.
 
+-E TIME, --end-time TIME
+                        Specify the time of day at which each day should start.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour before the earliest
+                        event start time or 00:00, whichever is later.
+
 -F FONT, --font FONT    Typeset text in the given font.  ``FONT`` must be
                         either the name of a builtin PostScript font or the
                         path to a ``.ttf`` file.  By default, text is typeset
                         in Helvetica.
 
 -f SIZE, --font-size SIZE
                         Set the size of the font used for event information to
@@ -66,14 +74,22 @@
                         to typeset it in "landscape mode."
 
 -s FACTOR, --scale FACTOR
                         Divide the length of each side of the table by
                         ``FACTOR``.  Without this option, the table fills the
                         whole page, except for a one-inch margin on each side.
 
+-S TIME, --start-time TIME
+                        Specify the time of day at which each day should end.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour after the latest
+                        event end time or 24:00, whichever is earlier.
+
 -T, --no-times          Do not show the times for each hour line.
 
 --no-weekends           Do not show Sunday and Saturday.
 
 
 Input Format
 ============
@@ -152,8 +168,8 @@
     - name: Sleep in
       days: SatSun
       time: 7-12
       color: "4226C4"
 
 produces (using the default options) an output file that looks like this:
 
-.. image:: https://github.com/jwodder/schedule/raw/v0.3.4/examples/example01.png
+.. image:: https://github.com/jwodder/schedule/raw/v0.4.0/examples/example01.png
```

### Comparing `pdfschedule-0.3.4/examples/example01.pdf` & `pdfschedule-0.4.0/examples/example01.pdf`

 * *Files identical despite different names*

### Comparing `pdfschedule-0.3.4/examples/example01.png` & `pdfschedule-0.4.0/examples/example01.png`

 * *Files identical despite different names*

### Comparing `pdfschedule-0.3.4/setup.cfg` & `pdfschedule-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 license_files = LICENSE
 url = https://github.com/jwodder/schedule
 keywords = 
 	pdf
 	schedule
 	week
 classifiers = 
-	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	License :: OSI Approved :: MIT License
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
 	Topic :: Office/Business :: Scheduling
 	Topic :: Printing
 project_urls = 
 	Source Code = https://github.com/jwodder/schedule
 	Bug Tracker = https://github.com/jwodder/schedule/issues
 
 [options]
 py_modules = pdfschedule
 package_dir = 
 	=src
-python_requires = ~=3.6
+python_requires = >=3.7
 install_requires = 
 	attrs     >= 18.2
 	click     >= 7.0
 	PyYAML    >= 5.0, < 7.0
 	reportlab ~= 3.4
 
 [options.entry_points]
```

### Comparing `pdfschedule-0.3.4/src/pdfschedule.egg-info/PKG-INFO` & `pdfschedule-0.4.0/src/pdfschedule.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: pdfschedule
-Version: 0.3.4
+Version: 0.4.0
 Summary: Weekly schedule typesetter
 Home-page: https://github.com/jwodder/schedule
 Author: John Thorvald Wodder II
 Author-email: pdfschedule@varonathe.org
 License: MIT
 Project-URL: Source Code, https://github.com/jwodder/schedule
 Project-URL: Bug Tracker, https://github.com/jwodder/schedule/issues
 Keywords: pdf,schedule,week
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Office/Business :: Scheduling
 Classifier: Topic :: Printing
-Requires-Python: ~=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
@@ -47,15 +45,15 @@
 
 ``pdfschedule`` is a Python 3 script for creating PDF documents showing
 one's weekly schedule of events.
 
 
 Installation
 ============
-``pdfschedule`` requires Python 3.6 or higher.  Just use `pip
+``pdfschedule`` requires Python 3.7 or higher.  Just use `pip
 <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to install
 ``pdfschedule`` and its dependencies::
 
     python3 -m pip install pdfschedule
 
 
 Usage
@@ -73,14 +71,22 @@
 
 Options
 -------
 
 -C, --color             Color the event boxes various colors instead of just
                         grey.
 
+-E TIME, --end-time TIME
+                        Specify the time of day at which each day should start.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour before the earliest
+                        event start time or 00:00, whichever is later.
+
 -F FONT, --font FONT    Typeset text in the given font.  ``FONT`` must be
                         either the name of a builtin PostScript font or the
                         path to a ``.ttf`` file.  By default, text is typeset
                         in Helvetica.
 
 -f SIZE, --font-size SIZE
                         Set the size of the font used for event information to
@@ -96,14 +102,22 @@
                         to typeset it in "landscape mode."
 
 -s FACTOR, --scale FACTOR
                         Divide the length of each side of the table by
                         ``FACTOR``.  Without this option, the table fills the
                         whole page, except for a one-inch margin on each side.
 
+-S TIME, --start-time TIME
+                        Specify the time of day at which each day should end.
+                        Times are specified in the format ``HH:MM`` using
+                        24-hour time, the minutes being optional (and
+                        optionally separated from the hour by a colon or
+                        period).  Defaults to half an hour after the latest
+                        event end time or 24:00, whichever is earlier.
+
 -T, --no-times          Do not show the times for each hour line.
 
 --no-weekends           Do not show Sunday and Saturday.
 
 
 Input Format
 ============
@@ -182,10 +196,8 @@
     - name: Sleep in
       days: SatSun
       time: 7-12
       color: "4226C4"
 
 produces (using the default options) an output file that looks like this:
 
-.. image:: https://github.com/jwodder/schedule/raw/v0.3.4/examples/example01.png
-
-
+.. image:: https://github.com/jwodder/schedule/raw/v0.4.0/examples/example01.png
```

### Comparing `pdfschedule-0.3.4/src/pdfschedule.py` & `pdfschedule-0.4.0/src/pdfschedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Weekly schedule typesetter
 
 Run ``pdfschedule --help`` or visit <https://github.com/jwodder/schedule> for
 more information.
 """
 
-__version__ = "0.3.4"
+__version__ = "0.4.0"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "pdfschedule@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/schedule"
 
 from collections.abc import Mapping
 from datetime import time
@@ -255,14 +255,22 @@
     def lry(self):
         return self.uly - self.height
 
     def rect(self):
         return (self.ulx, self.lry, self.width, self.height)
 
 
+def parse_time(s):
+    m = re.fullmatch(r"([0-9]{1,2})(?:[:.]?([0-9]{2}))?", s.strip())
+    if m:
+        return time(int(m[1]), int(m[2] or 0))
+    else:
+        raise ValueError(s)
+
+
 @click.command(context_settings={"help_option_names": ["-h", "--help"]})
 @click.option(
     "-C",
     "--color",
     is_flag=True,
     help="Use more colors for the event boxes than just grey",
 )
@@ -288,14 +296,28 @@
 @click.option(
     "-p",
     "--portrait",
     is_flag=True,
     help="Output in portrait mode instead of landscape",
 )
 @click.option(
+    "-S",
+    "--start-time",
+    type=parse_time,
+    help="Start time for each day",
+    metavar="HH:MM",
+)
+@click.option(
+    "-E",
+    "--end-time",
+    type=parse_time,
+    help="End time for each day",
+    metavar="HH:MM",
+)
+@click.option(
     "-s",
     "--scale",
     type=float,
     help="Scale down the table's dimensions by the given factor",
 )
 @click.option(
     "-T", "--no-times", is_flag=True, help="Do not show the times for each hour line"
@@ -311,14 +333,16 @@
     font,
     font_size,
     portrait,
     scale,
     no_times,
     no_weekends,
     start_monday,
+    start_time,
+    end_time,
 ):
     """
     Weekly schedule typesetter
 
     Visit <https://github.com/jwodder/schedule> for more information.
     """
     if font in available_fonts():
@@ -362,14 +386,16 @@
         c,
         x=inch,
         y=page_height - inch,
         width=page_width - 2 * inch,
         height=page_height - 2 * inch,
         font_size=font_size,
         show_times=not no_times,
+        min_time=time2hours(start_time) if start_time is not None else None,
+        max_time=time2hours(end_time) if end_time is not None else None,
     )
     c.showPage()
     c.save()
 
 
 def read_events(infile, colors):
     indata = yaml.safe_load(infile)
@@ -378,22 +404,20 @@
     for i, entry in enumerate(indata):
         text = entry.get("name", "").splitlines()
         try:
             days = entry["days"]
             timestr = entry["time"]
         except KeyError as e:
             raise click.UsageError(f"{str(e)!r} field missing from event #{i+1}")
-        m = re.match(
-            r"^\s*(\d{1,2})(?:[:.]?(\d{2}))?\s*" r"-\s*(\d{1,2})(?:[:.]?(\d{2}))?\s*$",
-            timestr,
-        )
-        if not m:
-            raise click.UsageError("Invalid time: " + repr(timestr))
-        start = time(int(m.group(1)), int(m.group(2) or 0))
-        end = time(int(m.group(3)), int(m.group(4) or 0))
+        start_str, _, end_str = timestr.partition("-")
+        try:
+            start = parse_time(start_str)
+            end = parse_time(end_str)
+        except ValueError:
+            raise click.UsageError(f"Invalid time: {timestr!r}")
         if "color" in entry:
             m = re.fullmatch(
                 r"\s*#?\s*([a-fA-F0-9]{2})([a-fA-F0-9]{2})([a-fA-F0-9]{2})\s*",
                 entry["color"],
             )
             if not m:
                 raise click.UsageError("Invalid color: " + repr(entry["color"]))
```

