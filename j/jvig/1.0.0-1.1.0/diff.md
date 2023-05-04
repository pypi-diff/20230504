# Comparing `tmp/jvig-1.0.0.tar.gz` & `tmp/jvig-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvig-1.0.0.tar", last modified: Sat Sep 24 11:16:19 2022, max compression
+gzip compressed data, was "jvig-1.1.0.tar", last modified: Thu May  4 05:17:28 2023, max compression
```

## Comparing `jvig-1.0.0.tar` & `jvig-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.133112 jvig-1.0.0/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2020 2022-09-24 11:16:19.133112 jvig-1.0.0/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1817 2022-09-24 10:56:11.000000 jvig-1.0.0/README.md
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.129112 jvig-1.0.0/jvig/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      344 2022-09-24 11:06:43.000000 jvig-1.0.0/jvig/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2022-09-24 07:15:33.000000 jvig-1.0.0/jvig/__main__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13630 2022-09-24 08:30:07.000000 jvig-1.0.0/jvig/cli.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10611 2022-09-24 08:30:10.000000 jvig-1.0.0/jvig/gtfs.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.133112 jvig-1.0.0/jvig/static/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    21548 2022-09-24 08:27:57.000000 jvig-1.0.0/jvig/static/cal.js
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    62635 2022-09-24 07:15:33.000000 jvig-1.0.0/jvig/static/jvig.png
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3221 2022-09-24 08:28:13.000000 jvig-1.0.0/jvig/static/style.css
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.133112 jvig-1.0.0/jvig/tables/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 07:15:33.000000 jvig-1.0.0/jvig/tables/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1010 2022-09-24 08:29:32.000000 jvig-1.0.0/jvig/tables/agency.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1796 2022-09-24 08:29:41.000000 jvig-1.0.0/jvig/tables/calendar.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1506 2022-09-24 08:29:38.000000 jvig-1.0.0/jvig/tables/calendar_dates.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1999 2022-09-24 08:29:44.000000 jvig-1.0.0/jvig/tables/frequencies.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3703 2022-09-24 08:29:48.000000 jvig-1.0.0/jvig/tables/routes.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2459 2022-09-24 08:29:52.000000 jvig-1.0.0/jvig/tables/stops.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2885 2022-09-24 08:29:55.000000 jvig-1.0.0/jvig/tables/times.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2712 2022-09-24 08:30:00.000000 jvig-1.0.0/jvig/tables/trips.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.133112 jvig-1.0.0/jvig/templates/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1827 2022-09-24 08:28:21.000000 jvig-1.0.0/jvig/templates/agency.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2820 2022-09-24 08:28:50.000000 jvig-1.0.0/jvig/templates/calendar.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2335 2022-09-24 08:28:35.000000 jvig-1.0.0/jvig/templates/calendars.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1831 2022-09-24 08:28:39.000000 jvig-1.0.0/jvig/templates/routes.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7816 2022-09-24 08:29:02.000000 jvig-1.0.0/jvig/templates/stop.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4891 2022-09-24 08:29:05.000000 jvig-1.0.0/jvig/templates/stops.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8087 2022-09-24 08:29:07.000000 jvig-1.0.0/jvig/templates/trip.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2051 2022-09-24 08:29:09.000000 jvig-1.0.0/jvig/templates/trips.html.jinja
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2257 2022-09-24 08:30:14.000000 jvig-1.0.0/jvig/util.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2160 2022-09-24 08:30:17.000000 jvig-1.0.0/jvig/valid.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 11:16:19.129112 jvig-1.0.0/jvig.egg-info/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2020 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      844 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/SOURCES.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       39 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/entry_points.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2022-04-24 15:27:12.000000 jvig-1.0.0/jvig.egg-info/not-zip-safe
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       17 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/requires.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       20 2022-09-24 11:16:19.000000 jvig-1.0.0/jvig.egg-info/top_level.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      728 2022-09-24 10:56:35.000000 jvig-1.0.0/pyproject.toml
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2022-09-24 11:16:19.133112 jvig-1.0.0/setup.cfg
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.326231 jvig-1.1.0/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3014 2023-05-04 05:17:28.326231 jvig-1.1.0/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2811 2022-09-24 11:30:50.000000 jvig-1.1.0/README.md
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.322231 jvig-1.1.0/jvig/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      162 2023-05-04 05:10:53.000000 jvig-1.1.0/jvig/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2022-09-24 07:15:33.000000 jvig-1.1.0/jvig/__main__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      343 2023-05-04 05:14:24.000000 jvig-1.1.0/jvig/__version__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13649 2023-05-04 05:13:09.000000 jvig-1.1.0/jvig/cli.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11328 2023-05-04 05:08:58.000000 jvig-1.1.0/jvig/gtfs.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.326231 jvig-1.1.0/jvig/static/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    21548 2022-09-24 08:27:57.000000 jvig-1.1.0/jvig/static/cal.js
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    62635 2022-09-24 07:15:33.000000 jvig-1.1.0/jvig/static/jvig.png
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3221 2022-09-24 08:28:13.000000 jvig-1.1.0/jvig/static/style.css
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.326231 jvig-1.1.0/jvig/tables/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        0 2022-09-24 07:15:33.000000 jvig-1.1.0/jvig/tables/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1010 2022-09-24 08:29:32.000000 jvig-1.1.0/jvig/tables/agency.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1796 2022-09-24 08:29:41.000000 jvig-1.1.0/jvig/tables/calendar.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1506 2022-09-24 08:29:38.000000 jvig-1.1.0/jvig/tables/calendar_dates.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1999 2022-09-24 08:29:44.000000 jvig-1.1.0/jvig/tables/frequencies.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3703 2022-09-24 08:29:48.000000 jvig-1.1.0/jvig/tables/routes.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2459 2022-09-24 08:29:52.000000 jvig-1.1.0/jvig/tables/stops.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2885 2022-09-24 08:29:55.000000 jvig-1.1.0/jvig/tables/times.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2712 2022-09-24 08:30:00.000000 jvig-1.1.0/jvig/tables/trips.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.326231 jvig-1.1.0/jvig/templates/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1827 2022-09-24 08:28:21.000000 jvig-1.1.0/jvig/templates/agency.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2820 2022-09-24 08:28:50.000000 jvig-1.1.0/jvig/templates/calendar.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2335 2022-09-24 08:28:35.000000 jvig-1.1.0/jvig/templates/calendars.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1831 2022-09-24 08:28:39.000000 jvig-1.1.0/jvig/templates/routes.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7816 2022-09-24 08:29:02.000000 jvig-1.1.0/jvig/templates/stop.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4891 2022-09-24 08:29:05.000000 jvig-1.1.0/jvig/templates/stops.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8087 2022-09-24 08:29:07.000000 jvig-1.1.0/jvig/templates/trip.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2051 2022-09-24 08:29:09.000000 jvig-1.1.0/jvig/templates/trips.html.jinja
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2257 2022-09-24 08:30:14.000000 jvig-1.1.0/jvig/util.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2160 2022-09-24 08:30:17.000000 jvig-1.1.0/jvig/valid.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.322231 jvig-1.1.0/jvig.egg-info/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3014 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      922 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/SOURCES.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       39 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/entry_points.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2022-04-24 15:27:12.000000 jvig-1.1.0/jvig.egg-info/not-zip-safe
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       17 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/requires.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       20 2023-05-04 05:17:28.000000 jvig-1.1.0/jvig.egg-info/top_level.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      728 2023-05-04 05:14:25.000000 jvig-1.1.0/pyproject.toml
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-05-04 05:17:28.326231 jvig-1.1.0/setup.cfg
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-04 05:17:28.326231 jvig-1.1.0/tests/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7185 2023-05-04 05:09:10.000000 jvig-1.1.0/tests/test_gtfs.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2578 2022-09-24 08:30:25.000000 jvig-1.1.0/tests/test_util.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2570 2022-09-24 08:30:28.000000 jvig-1.1.0/tests/test_valid.py
```

### Comparing `jvig-1.0.0/PKG-INFO` & `jvig-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 Metadata-Version: 2.1
 Name: jvig
-Version: 1.0.0
+Version: 1.1.0
 Summary: GTFS Viewer written using Flask
 License: GNU General Public License v3.0 or later
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-<img src="icon/jvig.svg" alt="logo" width="128" />  
+<img src="https://raw.githubusercontent.com/MKuranowski/jvig/master/icon/jvig.svg" alt="logo" width="128" />  
 
 jvig
 ====
 
 Pronounced d͡ʑvʲik (from 🇵🇱dźwig), it's a GTFS Viewer, created using Flask.
 
 jvig is still work-in-progress, but **it works**.
 
 
+Installation
+------------
+
+Install Python (at least 3.9) and pip. Consult your OS repositories for the package names,
+but these are usually `python3` and `python3-pip`. If you use a system without a package manager,
+I'd strongly recommend using one, like brew (for MacOS) or Chocolatey (for Windows).
+
+After that, install jvig using pip: `pip install --upgrade jvig`.
+
+
 Usage
 -----
 
 ```
+jvig /path/to/gtfs.zip
+```
+
+or (if the place where pip install scripts is not in PATH):
+
+```
 python3 -m jvig /path/to/gtfs.zip
 ```
 
 jvig can open both folders and ZIP archives.
 
+jvig itself doesn't contain a GUI - rather it spawns a web server on localhost and port 5000.
+After seeing ` * Running on http://127.0.0.1:5000` on the console, open up <http://127.0.0.1:5000>.
+
+#### WARNING: This is a development server.
+
+jvig uses the default Flask server, which is not suitable for opening up to the Internet.
+jvig only binds to the loopback address, and the server is only accessible from your own computer.
+
+Please don't serve jvig to the whole web.
+
 
 Features/Todos
 --------------
 
 #### Shown GTFS tables
 
 - [x] agencies
```

### Comparing `jvig-1.0.0/README.md` & `jvig-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,52 @@
-<img src="icon/jvig.svg" alt="logo" width="128" />  
+<img src="https://raw.githubusercontent.com/MKuranowski/jvig/master/icon/jvig.svg" alt="logo" width="128" />  
 
 jvig
 ====
 
 Pronounced d͡ʑvʲik (from 🇵🇱dźwig), it's a GTFS Viewer, created using Flask.
 
 jvig is still work-in-progress, but **it works**.
 
 
+Installation
+------------
+
+Install Python (at least 3.9) and pip. Consult your OS repositories for the package names,
+but these are usually `python3` and `python3-pip`. If you use a system without a package manager,
+I'd strongly recommend using one, like brew (for MacOS) or Chocolatey (for Windows).
+
+After that, install jvig using pip: `pip install --upgrade jvig`.
+
+
 Usage
 -----
 
 ```
+jvig /path/to/gtfs.zip
+```
+
+or (if the place where pip install scripts is not in PATH):
+
+```
 python3 -m jvig /path/to/gtfs.zip
 ```
 
 jvig can open both folders and ZIP archives.
 
+jvig itself doesn't contain a GUI - rather it spawns a web server on localhost and port 5000.
+After seeing ` * Running on http://127.0.0.1:5000` on the console, open up <http://127.0.0.1:5000>.
+
+#### WARNING: This is a development server.
+
+jvig uses the default Flask server, which is not suitable for opening up to the Internet.
+jvig only binds to the loopback address, and the server is only accessible from your own computer.
+
+Please don't serve jvig to the whole web.
+
 
 Features/Todos
 --------------
 
 #### Shown GTFS tables
 
 - [x] agencies
```

### Comparing `jvig-1.0.0/jvig/cli.py` & `jvig-1.1.0/jvig/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # jvig - GTFS Viewer, created using Flask.
-# Copyright © 2022 Mikołaj Kuranowski
+# Copyright © 2022-2023 Mikołaj Kuranowski
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -17,17 +17,18 @@
 import argparse
 from pathlib import Path
 from typing import Any, Optional
 
 from flask import Flask, jsonify, render_template
 from flask.wrappers import Response
 
+from .__version__ import __version__
 from .gtfs import Gtfs, Row
 from .tables import agency, calendar, calendar_dates, frequencies, routes, stops, times, trips
-from .util import sequence_to_int, time_to_int, to_js_literal
+from .util import time_to_int, to_js_literal
 
 
 class Application:
     def __init__(self, gtfs: Gtfs) -> None:
         self.gtfs = gtfs
         self.flask = Flask(__name__)
         self._init_app()
@@ -201,18 +202,15 @@
                 "trip.html.jinja",
                 missing=True,
                 trip={"trip_id": trip_id},
             )
 
         # Prepare data for rendering
         trip = self.gtfs.trips[trip_id]
-        times = sorted(
-            self.gtfs.stop_times.get(trip_id, []),
-            key=lambda r: sequence_to_int(r.get("stop_sequence", "")),
-        )
+        times = self.gtfs.stop_times.get(trip_id, [])
 
         stop_names = [
             self.gtfs.stops.get(i.get("stop_id", ""), {}).get("stop_name", "") for i in times
         ]
 
         return render_template(
             "trip.html.jinja",
@@ -339,14 +337,15 @@
     arg_parser.add_argument("file", type=Path, help="path to GTFS directory/zip")
     arg_parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         help="enable debug mode in Flask",
     )
+    arg_parser.add_argument("-V", "--version", action="version", version=f"jvig {__version__}")
     args = arg_parser.parse_args()
 
     # Load GTFS data
     gtfs = Gtfs.from_user_input(args.file)
 
     # Create the application
     app = Application(gtfs)
```

### Comparing `jvig-1.0.0/jvig/gtfs.py` & `jvig-1.1.0/jvig/gtfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # jvig - GTFS Viewer, created using Flask.
-# Copyright © 2022 Mikołaj Kuranowski
+# Copyright © 2022-2023 Mikołaj Kuranowski
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -17,37 +17,38 @@
 import csv
 import logging
 import zipfile
 from dataclasses import dataclass, field
 from datetime import date, timedelta
 from io import TextIOWrapper
 from math import nan
+from operator import itemgetter
 from pathlib import Path
-from typing import IO, Callable, List, Union
+from typing import IO, Callable, List, Optional, Union
 
-from .util import parse_gtfs_date
+from .util import parse_gtfs_date, sequence_to_int
 
 logger = logging.getLogger("jvig.gtfs")
 
 Row = dict[str, str]
 Point = tuple[float, float]
 
 TableToOne = dict[str, Row]
 TableToMany = dict[str, list[Row]]
 TableToPoints = dict[str, list[Point]]
 Table = Union[TableToOne, TableToMany, TableToPoints]
 
 
-def _get_shape_pt(row: Row) -> Point:
+def _get_shape_pt(row: Row) -> Optional[Point]:
     """Tries to parse a shapes.txt row into a Point tuple.
-    If there's anything wrong with the row, returns (nan, nan)."""
+    If there's anything wrong with the row, returns None"""
     try:
         return float(row.get("shape_pt_lat", nan)), float(row.get("shape_pt_lon", nan))
     except ValueError:
-        return nan, nan
+        return None
 
 
 _table_keys: dict[str, str] = {
     "agency": "agency_id",
     "stops": "stop_id",
     "routes": "route_id",
     "trips": "trip_id",
@@ -113,39 +114,56 @@
             parent = row.get("parent_station")
             if parent and row.get("location_type") != "1":
                 self.stop_children.setdefault(parent, []).append(row["stop_id"])
 
     def load_shapes(self, table_name: str, stream: IO[str]) -> None:
         """Specialized loader for shapes.txt to parse the shape."""
         assert table_name == "shapes"
-        self.shapes.clear()
 
-        # FIXME: First sort by shape_pt_sequence
+        shapes_with_indices: dict[str, list[tuple[int, Point]]] = {}
+
         for row in csv.DictReader(stream):
-            self.shapes.setdefault(row["shape_id"], []).append(_get_shape_pt(row))
+            idx = sequence_to_int(row.get("shape_pt_sequence", ""))
+            pt = _get_shape_pt(row)
+
+            # NOTE: Invalid rows are silently ignored
+            if idx >= 0 and pt is not None:
+                shapes_with_indices.setdefault(row["shape_id"], []).append((idx, pt))
+
+        # Sort shapes by shape_pt_sequence
+        for shape in shapes_with_indices.values():
+            shape.sort(key=itemgetter(0))
+
+        # Set shapes table
+        self.shapes = {
+            shape_id: [i[1] for i in shape] for shape_id, shape in shapes_with_indices.items()
+        }
 
     def load_stop_times(self, table_name: str, stream: IO[str]) -> None:
         """Specialized loader for stop_times.txt, which loads the data
         into self.stop_times and self.stop_times_by_stops."""
-        # FIXME: Sort by stop_sequence
 
         assert table_name == "stop_times"
         self.stop_times.clear()
         self.stop_times_by_stops.clear()
 
         for row in csv.DictReader(stream):
             self.stop_times.setdefault(row["trip_id"], []).append(row)
             self.stop_times_by_stops.setdefault(row["stop_id"], []).append(row)
 
+        # Sort stop_times by stop_sequence
+        for trip_stop_times in self.stop_times.values():
+            trip_stop_times.sort(key=lambda row: sequence_to_int(row.get("stop_sequence", "")))
+
     def header_of(self, table_name: str) -> List[str]:
         """Returns the GTFS header of a particlar table."""
         table: Union[TableToOne, TableToMany] = getattr(self, table_name)
 
         # Get the first entry from the table
-        entry = next(iter(table.values()), {})
+        entry = next(iter(table.values()), Row())
 
         # If it's a list of rows, get its first row
         if isinstance(entry, list):
             entry = entry[0]
 
         # Return the keys of the row
         return list(entry.keys())
```

### Comparing `jvig-1.0.0/jvig/static/cal.js` & `jvig-1.1.0/jvig/static/cal.js`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/static/jvig.png` & `jvig-1.1.0/jvig/static/jvig.png`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/static/style.css` & `jvig-1.1.0/jvig/static/style.css`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/agency.py` & `jvig-1.1.0/jvig/tables/agency.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/calendar.py` & `jvig-1.1.0/jvig/tables/calendar.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/calendar_dates.py` & `jvig-1.1.0/jvig/tables/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/frequencies.py` & `jvig-1.1.0/jvig/tables/frequencies.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/routes.py` & `jvig-1.1.0/jvig/tables/routes.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/stops.py` & `jvig-1.1.0/jvig/tables/stops.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/times.py` & `jvig-1.1.0/jvig/tables/times.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/tables/trips.py` & `jvig-1.1.0/jvig/tables/trips.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/agency.html.jinja` & `jvig-1.1.0/jvig/templates/agency.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/calendar.html.jinja` & `jvig-1.1.0/jvig/templates/calendar.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/calendars.html.jinja` & `jvig-1.1.0/jvig/templates/calendars.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/routes.html.jinja` & `jvig-1.1.0/jvig/templates/routes.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/stop.html.jinja` & `jvig-1.1.0/jvig/templates/stop.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/stops.html.jinja` & `jvig-1.1.0/jvig/templates/stops.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/trip.html.jinja` & `jvig-1.1.0/jvig/templates/trip.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/templates/trips.html.jinja` & `jvig-1.1.0/jvig/templates/trips.html.jinja`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/util.py` & `jvig-1.1.0/jvig/util.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig/valid.py` & `jvig-1.1.0/jvig/valid.py`

 * *Files identical despite different names*

### Comparing `jvig-1.0.0/jvig.egg-info/PKG-INFO` & `jvig-1.1.0/jvig.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 Metadata-Version: 2.1
 Name: jvig
-Version: 1.0.0
+Version: 1.1.0
 Summary: GTFS Viewer written using Flask
 License: GNU General Public License v3.0 or later
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-<img src="icon/jvig.svg" alt="logo" width="128" />  
+<img src="https://raw.githubusercontent.com/MKuranowski/jvig/master/icon/jvig.svg" alt="logo" width="128" />  
 
 jvig
 ====
 
 Pronounced d͡ʑvʲik (from 🇵🇱dźwig), it's a GTFS Viewer, created using Flask.
 
 jvig is still work-in-progress, but **it works**.
 
 
+Installation
+------------
+
+Install Python (at least 3.9) and pip. Consult your OS repositories for the package names,
+but these are usually `python3` and `python3-pip`. If you use a system without a package manager,
+I'd strongly recommend using one, like brew (for MacOS) or Chocolatey (for Windows).
+
+After that, install jvig using pip: `pip install --upgrade jvig`.
+
+
 Usage
 -----
 
 ```
+jvig /path/to/gtfs.zip
+```
+
+or (if the place where pip install scripts is not in PATH):
+
+```
 python3 -m jvig /path/to/gtfs.zip
 ```
 
 jvig can open both folders and ZIP archives.
 
+jvig itself doesn't contain a GUI - rather it spawns a web server on localhost and port 5000.
+After seeing ` * Running on http://127.0.0.1:5000` on the console, open up <http://127.0.0.1:5000>.
+
+#### WARNING: This is a development server.
+
+jvig uses the default Flask server, which is not suitable for opening up to the Internet.
+jvig only binds to the loopback address, and the server is only accessible from your own computer.
+
+Please don't serve jvig to the whole web.
+
 
 Features/Todos
 --------------
 
 #### Shown GTFS tables
 
 - [x] agencies
```

### Comparing `jvig-1.0.0/jvig.egg-info/SOURCES.txt` & `jvig-1.1.0/jvig.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 jvig/__init__.py
 jvig/__main__.py
+jvig/__version__.py
 jvig/cli.py
 jvig/gtfs.py
 jvig/util.py
 jvig/valid.py
 jvig.egg-info/PKG-INFO
 jvig.egg-info/SOURCES.txt
 jvig.egg-info/dependency_links.txt
@@ -28,8 +29,11 @@
 jvig/templates/agency.html.jinja
 jvig/templates/calendar.html.jinja
 jvig/templates/calendars.html.jinja
 jvig/templates/routes.html.jinja
 jvig/templates/stop.html.jinja
 jvig/templates/stops.html.jinja
 jvig/templates/trip.html.jinja
-jvig/templates/trips.html.jinja
+jvig/templates/trips.html.jinja
+tests/test_gtfs.py
+tests/test_util.py
+tests/test_valid.py
```

### Comparing `jvig-1.0.0/pyproject.toml` & `jvig-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=52", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jvig"
-version = "1.0.0"
+version = "1.1.0"
 description = "GTFS Viewer written using Flask"
 readme = "README.md"
 license = {text = "GNU General Public License v3.0 or later"}
 requires-python = ">=3.9"
 dependencies = ["flask", "markupsafe"]
 
 [project.scripts]
```

