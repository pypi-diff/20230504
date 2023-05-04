# Comparing `tmp/ecida-0.0.2.tar.gz` & `tmp/ecida-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.2.tar", last modified: Wed May  3 17:17:46 2023, max compression
+gzip compressed data, was "ecida-0.0.3.tar", last modified: Thu May  4 14:36:19 2023, max compression
```

## Comparing `ecida-0.0.2.tar` & `ecida-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-03 17:17:46.047962 ecida-0.0.2/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4707 2023-05-03 17:14:17.000000 ecida-0.0.2/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-03 17:17:46.047962 ecida-0.0.2/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-03-09 17:51:25.000000 ecida-0.0.2/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-03 17:17:46.047962 ecida-0.0.2/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-03 17:17:46.000000 ecida-0.0.2/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-03 17:17:46.000000 ecida-0.0.2/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-03 17:17:46.000000 ecida-0.0.2/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-03 17:17:46.000000 ecida-0.0.2/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-03 17:17:46.000000 ecida-0.0.2/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-03 17:17:46.047962 ecida-0.0.2/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-03 17:17:38.000000 ecida-0.0.2/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-04 14:36:19.913546 ecida-0.0.3/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4773 2023-05-04 14:35:17.000000 ecida-0.0.3/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-04 14:36:19.913546 ecida-0.0.3/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-03-09 17:51:25.000000 ecida-0.0.3/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-04 14:36:19.913546 ecida-0.0.3/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-04 14:36:19.913546 ecida-0.0.3/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-04 14:35:24.000000 ecida-0.0.3/setup.py
```

### Comparing `ecida-0.0.2/Ecida.py` & `ecida-0.0.3/Ecida.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,17 @@
         self._KAFKA_BOOTSTRAP_SERVER = os.environ['KAFKA_BOOTSTRAP_SERVER']
         self._KAFKA_SASL_MECHANISM = os.environ['KAFKA_SASL_MECHANISM']
         self._KAFKA_SECURITY_PROTOCOL = os.environ['KAFKA_SECURITY_PROTOCOL']
         self._KAFKA_USERNAME = os.environ['KAFKA_USERNAME']
         self._KAFKA_PASSWORD = os.environ['KAFKA_PASSWORD']
         self._KAFKA_GROUP_ID = os.environ['KAFKA_USERNAME']
         
-        for key, _ in self._inputs.items():
+        for key, value in self._inputs.items():
+            if value == "directory":
+                continue
             topicName = os.environ[self._topics_envVars[key]]
             self._topics_names[key] = topicName
             consumer = KafkaConsumer(topicName, bootstrap_servers = self._KAFKA_BOOTSTRAP_SERVER, 
                             sasl_plain_username= self._KAFKA_USERNAME,
                             sasl_plain_password= self._KAFKA_PASSWORD,
                             sasl_mechanism=self._KAFKA_SASL_MECHANISM,
                             security_protocol=self._KAFKA_SECURITY_PROTOCOL,
```

### Comparing `ecida-0.0.2/PKG-INFO` & `ecida-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.2
+Version: 0.0.3
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.2/ecida.egg-info/PKG-INFO` & `ecida-0.0.3/ecida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.2
+Version: 0.0.3
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.2/setup.py` & `ecida-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.2',
+   version='0.0.3',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

