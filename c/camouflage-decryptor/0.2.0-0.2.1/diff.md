# Comparing `tmp/camouflage_decryptor-0.2.0.tar.gz` & `tmp/camouflage_decryptor-0.2.1.tar.gz`

## Comparing `camouflage_decryptor-0.2.0.tar` & `camouflage_decryptor-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/src/camouflage_decryptor/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/src/camouflage_decryptor/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/src/camouflage_decryptor/__main__.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/src/camouflage_decryptor/decryptor.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/src/camouflage_decryptor/cli/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/README.md
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/src/camouflage_decryptor/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/src/camouflage_decryptor/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/src/camouflage_decryptor/__main__.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/src/camouflage_decryptor/decryptor.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/src/camouflage_decryptor/cli/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/README.md
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 camouflage_decryptor-0.2.1/PKG-INFO
```

### Comparing `camouflage_decryptor-0.2.0/.github/workflows/pypi-publish.yml` & `camouflage_decryptor-0.2.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.2.0/src/camouflage_decryptor/decryptor.py` & `camouflage_decryptor-0.2.1/src/camouflage_decryptor/decryptor.py`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.2.0/LICENSE.txt` & `camouflage_decryptor-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.2.0/README.md` & `camouflage_decryptor-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,25 @@
 ```console
 pip install camouflage-decryptor
 ```
 
 ## Usage
 This tool provides different tools for analyzing a file that has been generated with [camouflage](http://camouflage.unfiction.com/). This includes the following:
 
+#### Command Line Help
+For the tool and all its subcommands, help can be retrieved by calling the tool with the `--help` flag:
+```console
+camouflage-decryptor --help
+```
+
+
 #### Metadata retrieval
 To retrieve all the camouflage metadata from a prepared file the following command can be used:
 ```console
-camouflage-decryptor get-key camouflaged-file.jpg
+camouflage-decryptor get-info camouflaged-file.jpg
 ```
 The output will look similar to this one:
 
     File Name Carrier:             normal_file.png
     File Name Secret:              secret.txt
     Size secret file:              4.00 B
     File size unmodified carrier:  4.00 B
```

### Comparing `camouflage_decryptor-0.2.0/pyproject.toml` & `camouflage_decryptor-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `camouflage_decryptor-0.2.0/PKG-INFO` & `camouflage_decryptor-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camouflage-decryptor
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/unknown/camouflage-decryptor#readme
 Project-URL: Issues, https://github.com/unknown/camouflage-decryptor/issues
 Project-URL: Source, https://github.com/unknown/camouflage-decryptor
 Author-email: anjomro <py@anjomro.de>
 License-Expression: EUPL-1.2
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -39,18 +39,25 @@
 ```console
 pip install camouflage-decryptor
 ```
 
 ## Usage
 This tool provides different tools for analyzing a file that has been generated with [camouflage](http://camouflage.unfiction.com/). This includes the following:
 
+#### Command Line Help
+For the tool and all its subcommands, help can be retrieved by calling the tool with the `--help` flag:
+```console
+camouflage-decryptor --help
+```
+
+
 #### Metadata retrieval
 To retrieve all the camouflage metadata from a prepared file the following command can be used:
 ```console
-camouflage-decryptor get-key camouflaged-file.jpg
+camouflage-decryptor get-info camouflaged-file.jpg
 ```
 The output will look similar to this one:
 
     File Name Carrier:             normal_file.png
     File Name Secret:              secret.txt
     Size secret file:              4.00 B
     File size unmodified carrier:  4.00 B
```

