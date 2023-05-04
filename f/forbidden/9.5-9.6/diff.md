# Comparing `tmp/forbidden-9.5.tar.gz` & `tmp/forbidden-9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forbidden-9.5.tar", last modified: Fri Apr 28 13:45:53 2023, max compression
+gzip compressed data, was "forbidden-9.6.tar", last modified: Thu May  4 11:15:56 2023, max compression
```

## Comparing `forbidden-9.5.tar` & `forbidden-9.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.365278 forbidden-9.5/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:41:20.000000 forbidden-9.5/LICENSE
--rwxrwx---   0 root         (0) root         (0)      112 2023-04-28 13:41:20.000000 forbidden-9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-28 13:45:53.365278 forbidden-9.5/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    12428 2023-04-28 13:42:18.000000 forbidden-9.5/README.md
--rwxrwx---   0 root         (0) root         (0)      814 2023-04-28 13:41:36.000000 forbidden-9.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:45:53.365278 forbidden-9.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/forbidden/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.5/src/forbidden/__init__.py
--rwxrwx---   0 root         (0) root         (0)    44708 2023-04-28 13:45:03.000000 forbidden-9.5/src/forbidden/forbidden.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.5/src/forbidden/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/forbidden.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.365278 forbidden-9.5/src/stresser/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.5/src/stresser/__init__.py
--rwxrwx---   0 root         (0) root         (0)    19791 2023-04-28 13:44:58.000000 forbidden-9.5/src/stresser/stresser.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.5/src/stresser/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:41:20.000000 forbidden-9.6/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      112 2023-04-28 13:41:20.000000 forbidden-9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12639 2023-05-04 11:15:56.241732 forbidden-9.6/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    12688 2023-05-04 09:58:59.000000 forbidden-9.6/README.md
+-rwxrwx---   0 root         (0) root         (0)      833 2023-05-04 11:05:25.000000 forbidden-9.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 11:15:56.241732 forbidden-9.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/forbidden/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.6/src/forbidden/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    44751 2023-05-04 09:55:00.000000 forbidden-9.6/src/forbidden/forbidden.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.6/src/forbidden/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/forbidden.egg-info/
+-rwxrwx---   0 root         (0) root         (0)    12639 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)      430 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) root         (0)        1 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) root         (0)       89 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/entry_points.txt
+-rwxrwx---   0 root         (0) root         (0)       79 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/requires.txt
+-rwxrwx---   0 root         (0) root         (0)       19 2023-05-04 11:15:56.000000 forbidden-9.6/src/forbidden.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:15:56.241732 forbidden-9.6/src/stresser/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.6/src/stresser/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    19834 2023-05-04 09:56:11.000000 forbidden-9.6/src/stresser/stresser.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.6/src/stresser/user_agents.txt
```

### Comparing `forbidden-9.5/LICENSE` & `forbidden-9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `forbidden-9.5/PKG-INFO` & `forbidden-9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 9.5
+Version: 9.6
 Summary: Bypass 4xx HTTP response status codes and more.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forbidden
 
 Bypass 4xx HTTP response status codes and more. Based on PycURL.
 
@@ -88,36 +88,40 @@
 * [HTTP Headers](#http-headers)
 * [URL Paths](#url-paths)
 * [Results Format](#results-format)
 * [Usage](#usage)
 
 ## How to Install
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 pip3 install forbidden
 
 pip3 install --upgrade forbidden
 ```
 
 ## How to Build and Install Manually
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 Run the following commands:
 
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.5-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -346,39 +350,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.5 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -421,26 +425,26 @@
     Number of parallel threads to run
     More threads make it quicker but can give worse results
     Heavily depends on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.5
+    Default: Forbidden/9.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
 ```
 
 ```fundamental
-Stresser v4.5 ( github.com/ivan-sincek/forbidden )
+Stresser v4.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -467,15 +471,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.5
+    Default: Stresser/4.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.5/README.md` & `forbidden-9.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -75,36 +75,40 @@
 * [HTTP Headers](#http-headers)
 * [URL Paths](#url-paths)
 * [Results Format](#results-format)
 * [Usage](#usage)
 
 ## How to Install
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 pip3 install forbidden
 
 pip3 install --upgrade forbidden
 ```
 
 ## How to Build and Install Manually
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 Run the following commands:
 
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.5-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -333,39 +337,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.5 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -408,26 +412,26 @@
     Number of parallel threads to run
     More threads make it quicker but can give worse results
     Heavily depends on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.5
+    Default: Forbidden/9.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
 ```
 
 ```fundamental
-Stresser v4.5 ( github.com/ivan-sincek/forbidden )
+Stresser v4.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -454,15 +458,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.5
+    Default: Stresser/4.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.5/pyproject.toml` & `forbidden-9.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "forbidden"
-version = "9.5"
+version = "9.6"
 authors = [{ name = "Ivan Sincek" }]
 description = "Bypass 4xx HTTP response status codes and more."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
-dependencies = ["datetime>=5.0", "requests>=2.10.0", "pycurl>=7.45.1", "termcolor>=1.1.0"]
+dependencies = ["datetime>=5.0", "requests>=2.10.0", "pycurl>=7.45.1", "termcolor>=1.1.0", "colorama>=0.4.6"]
 
 [project.urls]
 "Homepage" = "https://github.com/ivan-sincek/forbidden"
 
 [project.scripts]
 forbidden = "forbidden.forbidden:main"
 stresser = "stresser.stresser:main"
```

### Comparing `forbidden-9.5/src/forbidden/forbidden.py` & `forbidden-9.6/src/forbidden/forbidden.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 import base64
 import concurrent.futures
 import subprocess
 import io
 import requests
 import pycurl
 import termcolor
+import colorama
 import json
 
 start = datetime.datetime.now()
 
 requests.packages.urllib3.disable_warnings(requests.packages.urllib3.exceptions.InsecureRequestWarning)
 
+colorama.init(autoreset = True)
+
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Forbidden v9.5 ( github.com/ivan-sincek/forbidden )")
+	print("Forbidden v9.6 ( github.com/ivan-sincek/forbidden )")
 	print("")
 	print("Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]")
 	print("Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -75,15 +78,15 @@
 	print("    Number of parallel threads to run")
 	print("    More threads make it quicker but can give worse results")
 	print("    Heavily depends on network bandwidth and server capacity")
 	print("    Default: 5")
 	print("    -th <threads> - 200 | etc.")
 	print("AGENT")
 	print("    User agent to use")
-	print("    Default: Forbidden/9.5")
+	print("    Default: Forbidden/9.6")
 	print("    -a <agent> - curl/3.30.1 | random[-all] | etc.")
 	print("PROXY")
 	print("    Web proxy to use")
 	print("    -x <proxy> - 127.0.0.1:8080 | etc.")
 	print("OUT")
 	print("    Output file")
 	print("    -o <out> - results.json | etc.")
@@ -1113,15 +1116,15 @@
 def remove(array, keys):
 	for entry in array:
 		for key in keys:
 			entry.pop(key, None)
 	return array
 
 def output(record, color):
-	print(termcolor.colored(jdump(record), color))
+	termcolor.cprint(jdump(record), color)
 	return record
 
 def create_table(results):
 	table = [{"code": code, "count": 0} for code in sorted(unique(record["code"] for record in results))]
 	for entry in table:
 		for record in results:
 			if record["code"] == entry["code"]:
@@ -1129,15 +1132,15 @@
 	return table
 
 def table_horizontal_border():
 	print("-" * 22)
 
 def table_row(code, count, color = None):
 	text = ("| {0:<6} | {1:<9} |").format(code, count)
-	print(termcolor.colored(text, color) if color else text)
+	termcolor.cprint(text, color) if color else print(text)
 
 def table_header():
 	table_row("Code", "Count")
 
 def display_table(table):
 	table_horizontal_border()
 	table_header()
@@ -1217,15 +1220,15 @@
 			error("Missing a mandatory option (-u, -t) and/or optional (-f, -v, -p, -e, -i, -l, -th, -a, -x, -o)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                             Forbidden v9.5                             #")
+		print("#                             Forbidden v9.6                             #")
 		print("#                                  by Ivan Sincek                        #")
 		print("#                                                                        #")
 		print("# Bypass 4xx HTTP response status codes and more.                        #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                 #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
@@ -1233,15 +1236,15 @@
 		if not args["path"]:
 			args["path"] = ["/robots.txt"] # can have multiple
 		if not args["evil"]:
 			args["evil"] = "github.com"
 		if not args["threads"]:
 			args["threads"] = 5
 		if not args["agent"]:
-			args["agent"] = "Forbidden/9.5"
+			args["agent"] = "Forbidden/9.6"
 		# --------------------
 		url = parse_url(args["url"])
 		ignore = {"text": args["ignore"], "lengths": args["lengths"] if args["lengths"] else []}
 		# --------------------
 		# NOTE: Fetch content length of base HTTP response.
 		if "base" in ignore["lengths"]:
 			record = fetch(url["full"], args["force"] if args["force"] else "GET", None, None, None, args["agent"], None)
```

### Comparing `forbidden-9.5/src/forbidden/user_agents.txt` & `forbidden-9.6/src/forbidden/user_agents.txt`

 * *Files identical despite different names*

### Comparing `forbidden-9.5/src/forbidden.egg-info/PKG-INFO` & `forbidden-9.6/src/forbidden.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 9.5
+Version: 9.6
 Summary: Bypass 4xx HTTP response status codes and more.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forbidden
 
 Bypass 4xx HTTP response status codes and more. Based on PycURL.
 
@@ -88,36 +88,40 @@
 * [HTTP Headers](#http-headers)
 * [URL Paths](#url-paths)
 * [Results Format](#results-format)
 * [Usage](#usage)
 
 ## How to Install
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 pip3 install forbidden
 
 pip3 install --upgrade forbidden
 ```
 
 ## How to Build and Install Manually
 
+On Windows OS, download and install PycURL from [www.lfd.uci.edu/~gohlke](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycurl).
+
 Run the following commands:
 
 ```bash
 apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.5-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.6-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -346,39 +350,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.5",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.6",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.6' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.5 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -421,26 +425,26 @@
     Number of parallel threads to run
     More threads make it quicker but can give worse results
     Heavily depends on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.5
+    Default: Forbidden/9.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
 ```
 
 ```fundamental
-Stresser v4.5 ( github.com/ivan-sincek/forbidden )
+Stresser v4.6 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -467,15 +471,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.5
+    Default: Stresser/4.6
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.5/src/stresser/stresser.py` & `forbidden-9.6/src/stresser/stresser.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 import shutil
 import re
 import concurrent.futures
 import subprocess
 import io
 import pycurl
 import termcolor
+import colorama
 import json
 
 start = datetime.datetime.now()
 
+colorama.init(autoreset = True)
+
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Stresser v4.5 ( github.com/ivan-sincek/forbidden )")
+	print("Stresser v4.6 ( github.com/ivan-sincek/forbidden )")
 	print("")
 	print("Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]")
 	print("Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]")
 
 def advanced():
 	basic()
 	print("")
@@ -55,15 +58,15 @@
 	print("LENGTHS")
 	print("    Filter out 200 OK false positive results by content lengths")
 	print("    Specify 'base' to ignore content length of base HTTP response")
 	print("    Use comma separated values")
 	print("    -l <lengths> - 12 | base | etc.")
 	print("AGENT")
 	print("    User agent to use")
-	print("    Default: Stresser/4.5")
+	print("    Default: Stresser/4.6")
 	print("    -a <agent> - curl/3.30.1 | random[-all] | etc.")
 	print("PROXY")
 	print("    Web proxy to use")
 	print("    -x <proxy> - 127.0.0.1:8080 | etc.")
 	print("OUT")
 	print("    Output file")
 	print("    -o <out> - results.json | etc.")
@@ -416,15 +419,15 @@
 def remove(array, keys):
 	for entry in array:
 		for key in keys:
 			entry.pop(key, None)
 	return array
 
 def output(record, color):
-	print(termcolor.colored(jdump(record), color))
+	termcolor.cprint(jdump(record), color)
 	return record
 
 def create_table(results):
 	table = [{"code": code, "count": 0} for code in sorted(unique(record["code"] for record in results))]
 	for entry in table:
 		for record in results:
 			if record["code"] == entry["code"]:
@@ -432,15 +435,15 @@
 	return table
 
 def table_horizontal_border():
 	print("-" * 22)
 
 def table_row(code, count, color = None):
 	text = ("| {0:<6} | {1:<9} |").format(code, count)
-	print(termcolor.colored(text, color) if color else text)
+	termcolor.cprint(text, color) if color else print(text)
 
 def table_header():
 	table_row("Code", "Count")
 
 def display_table(table):
 	table_horizontal_border()
 	table_header()
@@ -522,25 +525,25 @@
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["directory"]):
 		os.chdir(args["directory"])
 		print("###########################################################$$$$############")
 		print("#                                                                         #")
-		print("#                              Stresser v4.5                              #")
+		print("#                              Stresser v4.6                              #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Bypass 4xx HTTP response status codes with stress testing.              #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                  #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
 		# --------------------
 		if not args["agent"]:
-			args["agent"] = "Stresser/4.5"
+			args["agent"] = "Stresser/4.6"
 		# --------------------
 		url = parse_url(args["url"])
 		ignore = {"text": args["ignore"], "lengths": args["lengths"] if args["lengths"] else []}
 		# --------------------
 		# NOTE: Fetch content length of base HTTP response.
 		if "base" in ignore["lengths"]:
 			record = fetch(url["full"], args["force"] if args["force"] else "GET", None, None, None, args["agent"], None)
```

### Comparing `forbidden-9.5/src/stresser/user_agents.txt` & `forbidden-9.6/src/stresser/user_agents.txt`

 * *Files identical despite different names*

