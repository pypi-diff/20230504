# Comparing `tmp/google-chad-3.3.tar.gz` & `tmp/google-chad-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-3.3.tar", last modified: Fri Apr 28 13:18:44 2023, max compression
+gzip compressed data, was "google-chad-3.4.tar", last modified: Thu May  4 11:30:33 2023, max compression
```

## Comparing `google-chad-3.3.tar` & `google-chad-3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:13:40.000000 google-chad-3.3/LICENSE
--rwxrwx---   0 root         (0) root         (0)      111 2023-04-28 13:13:40.000000 google-chad-3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10408 2023-04-28 13:18:44.763366 google-chad-3.3/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    10307 2023-04-28 13:17:05.000000 google-chad-3.3/README.md
--rwxrwx---   0 root         (0) root         (0)      893 2023-04-28 13:16:39.000000 google-chad-3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:18:44.763366 google-chad-3.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/chad/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.3/src/chad/__init__.py
--rwxrwx---   0 root         (0) root         (0)    19973 2023-04-28 13:15:26.000000 google-chad-3.3/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/chad_extractor/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.3/src/chad_extractor/__init__.py
--rwxrwx---   0 root         (0) root         (0)    23152 2023-04-28 13:16:23.000000 google-chad-3.3/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/dorks/
--rwxrwx---   0 root         (0) root         (0)      237 2023-04-28 13:13:40.000000 google-chad-3.3/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/google_chad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10408 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/templates/
--rwxrwx---   0 root         (0) root         (0)     1739 2023-04-28 13:13:40.000000 google-chad-3.3/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:13:40.000000 google-chad-3.4/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      111 2023-04-28 13:13:40.000000 google-chad-3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-05-04 11:30:33.569308 google-chad-3.4/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    10307 2023-05-04 10:46:18.000000 google-chad-3.4/README.md
+-rwxrwx---   0 root         (0) root         (0)      912 2023-05-04 10:37:19.000000 google-chad-3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 11:30:33.569308 google-chad-3.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.565310 google-chad-3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/src/chad/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.4/src/chad/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    20062 2023-05-04 10:14:53.000000 google-chad-3.4/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/src/chad_extractor/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.4/src/chad_extractor/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    23152 2023-05-04 09:08:23.000000 google-chad-3.4/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/src/dorks/
+-rwxrwx---   0 root         (0) root         (0)      237 2023-04-28 13:13:40.000000 google-chad-3.4/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/src/google_chad.egg-info/
+-rwxrwx---   0 root         (0) root         (0)    10408 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)      460 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) root         (0)        1 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) root         (0)       92 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/entry_points.txt
+-rwxrwx---   0 root         (0) root         (0)      145 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/requires.txt
+-rwxrwx---   0 root         (0) root         (0)       36 2023-05-04 11:30:33.000000 google-chad-3.4/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:30:33.569308 google-chad-3.4/src/templates/
+-rwxrwx---   0 root         (0) root         (0)     1739 2023-04-28 13:13:40.000000 google-chad-3.4/src/templates/social_media_template.json
```

### Comparing `google-chad-3.3/LICENSE` & `google-chad-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-chad-3.3/PKG-INFO` & `google-chad-3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.3
+Version: 3.4
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
@@ -203,15 +203,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.3 ( github.com/ivan-sincek/chad )
+Chad v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -270,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.3/README.md` & `google-chad-3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.3 ( github.com/ivan-sincek/chad )
+Chad v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -257,15 +257,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.3/pyproject.toml` & `google-chad-3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "google-chad"
-version = "3.3"
+version = "3.4"
 authors = [{ name = "Ivan Sincek" }]
 description = "Not another Google Dorking tool."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
-	"Operating System :: POSIX :: Linux"
+	"Operating System :: OS Independent"
 ]
-dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "nagooglesearch>=6.0", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
+dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "colorama>=0.4.6", "nagooglesearch>=6.0", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/chad"
 
 [project.scripts]
 chad = "chad.chad:main"
 chad-extractor = "chad_extractor.chad_extractor:main"
```

### Comparing `google-chad-3.3/src/chad/chad.py` & `google-chad-3.4/src/chad/chad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #!/usr/bin/env python3
 
 import datetime
 import dateutil.relativedelta as relativedelta
 import sys
 import os
 import termcolor
+import colorama
 import time
 import random
 from nagooglesearch import nagooglesearch
 import regex as re
 import concurrent.futures
 import subprocess
 import requests
 import urllib.parse
 import json
 
 start = datetime.datetime.now()
 
 requests.packages.urllib3.disable_warnings(requests.packages.urllib3.exceptions.InsecureRequestWarning)
 
+colorama.init(autoreset = True)
+
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad v3.3 ( github.com/ivan-sincek/chad )")
+	print("Chad v3.4 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]")
 	print("Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -275,27 +278,28 @@
 			count += 1
 	return argc - count == argc / 2
 
 # --------------------- VALIDATION END ---------------------
 
 # ----------------------- TASK BEGIN -----------------------
 
-def get_timestamp(text):
-	return print(("{0} - {1}").format(datetime.datetime.now().strftime("%H:%M:%S"), text))
+def get_timestamp(text, color = None):
+	text = ("{0} - {1}").format(datetime.datetime.now().strftime("%H:%M:%S"), text)
+	return termcolor.cprint(text, color) if color else print(text)
 
 def status(current, total, query, proxy = None, color = "green"):
-	text = ("QUERY {0}/{1}: {2}").format(current, total, termcolor.colored(query, color))
+	text = ("QUERY {0}/{1}: {2}").format(current, total, query)
 	if proxy:
 		text = ("{0} | PROXY: {1}").format(text, proxy)
-	get_timestamp(text)
+	get_timestamp(text, color)
 
 def print_ignored(ignored, color = "cyan"):
 	print(("{0} QUERIES IGNORED:").format(len(ignored)))
 	for query in ignored:
-		print(termcolor.colored(query, color))
+		termcolor.cprint(query, color)
 
 def get_site(query):
 	return re.search(r"(?<!in|\-)site\:", query, re.IGNORECASE)
 
 def validate_queries(queries, site = None):
 	tmp = []
 	ignored = []
@@ -401,15 +405,15 @@
 						proxy = entry["proxy"],
 						min_sleep = min_p,
 						max_sleep = max_p,
 						verbose = debug
 					)
 					entry["urls"] = client.search()
 					if "429_TOO_MANY_REQUESTS" in entry["urls"]:
-						print(termcolor.colored("[ HTTP 429 Too Many Requests ]", "yellow"))
+						termcolor.cprint("[ HTTP 429 Too Many Requests ]", "yellow")
 						entry["urls"].pop(entry["urls"].index("429_TOO_MANY_REQUESTS"))
 						if entry["proxy"]:
 							remove = True
 						else:
 							exit = True
 					if entry["urls"]:
 						if not get_site(entry["query"]):
@@ -522,15 +526,15 @@
 			error("Missing a mandatory option (-q) and/or optional (-s, -t, -tr, -pr, -min-q, -max-q, -min-p, -max-p, -a, -p, -th, -d, -o, -sos, -dbg)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                                Chad v3.3                                #")
+		print("#                                Chad v3.4                                #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Search Google Dorks like Chad.                                          #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `google-chad-3.3/src/chad_extractor/chad_extractor.py` & `google-chad-3.4/src/chad_extractor/chad_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Chad Extractor v3.3 ( github.com/ivan-sincek/chad )")
+	print("Chad Extractor v3.4 ( github.com/ivan-sincek/chad )")
 	print("")
 	print("Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]")
 	print("Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]")
 
 def advanced():
 	basic()
 	print("")
@@ -542,15 +542,15 @@
 			error("Missing a mandatory option (-t, -res, -o) and/or optional (-pt, -e, -th, -r, -w, -a, -v)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                           Chad Extractor v3.3                           #")
+		print("#                           Chad Extractor v3.4                           #")
 		print("#                                   by Ivan Sincek                        #")
 		print("#                                                                         #")
 		print("# Extract and validate data from Chad results.                            #")
 		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
```

### Comparing `google-chad-3.3/src/google_chad.egg-info/PKG-INFO` & `google-chad-3.4/src/google_chad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.3
+Version: 3.4
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
@@ -203,15 +203,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.3 ( github.com/ivan-sincek/chad )
+Chad v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -270,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.4 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.3/src/templates/social_media_template.json` & `google-chad-3.4/src/templates/social_media_template.json`

 * *Files identical despite different names*

