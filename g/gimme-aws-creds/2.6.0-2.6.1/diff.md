# Comparing `tmp/gimme aws creds-2.6.0.tar.gz` & `tmp/gimme aws creds-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme aws creds-2.6.0.tar", last modified: Tue May  2 15:51:58 2023, max compression
+gzip compressed data, was "gimme aws creds-2.6.1.tar", last modified: Thu May  4 16:36:43 2023, max compression
```

## Comparing `gimme aws creds-2.6.0.tar` & `gimme aws creds-2.6.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds-autocomplete.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26779 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    47402 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/okta_classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/okta_identity_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 15:51:58.814083 gimme aws creds-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/LONG_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.425546 gimme aws creds-2.6.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.425546 gimme aws creds-2.6.1/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26779 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47402 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/setup.py
```

### Comparing `gimme aws creds-2.6.0/LICENSE` & `gimme aws creds-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/NOTICE` & `gimme aws creds-2.6.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/PKG-INFO` & `gimme aws creds-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme aws creds
-Version: 2.6.0
+Version: 2.6.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme aws creds-2.6.0/README.md` & `gimme aws creds-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/bin/gimme-aws-creds` & `gimme aws creds-2.6.1/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/bin/gimme-aws-creds-autocomplete.sh` & `gimme aws creds-2.6.1/bin/gimme-aws-creds-autocomplete.sh`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/bin/gimme-aws-creds.cmd` & `gimme aws creds-2.6.1/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/aws.py` & `gimme aws creds-2.6.1/gimme_aws_creds/aws.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/common.py` & `gimme aws creds-2.6.1/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/config.py` & `gimme aws creds-2.6.1/gimme_aws_creds/config.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/default.py` & `gimme aws creds-2.6.1/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/duo.py` & `gimme aws creds-2.6.1/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/errors.py` & `gimme aws creds-2.6.1/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/main.py` & `gimme aws creds-2.6.1/gimme_aws_creds/main.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/okta_classic.py` & `gimme aws creds-2.6.1/gimme_aws_creds/okta_classic.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/okta_identity_engine.py` & `gimme aws creds-2.6.1/gimme_aws_creds/okta_identity_engine.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/registered_authenticators.py` & `gimme aws creds-2.6.1/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/u2f.py` & `gimme aws creds-2.6.1/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/ui.py` & `gimme aws creds-2.6.1/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds/webauthn.py` & `gimme aws creds-2.6.1/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds.egg-info/PKG-INFO` & `gimme aws creds-2.6.1/gimme_aws_creds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme-aws-creds
-Version: 2.6.0
+Version: 2.6.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme aws creds-2.6.0/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme aws creds-2.6.1/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+LONG_DESCRIPTION.md
 MANIFEST.in
 NOTICE
 README.md
 requirements.txt
 setup.cfg
 setup.py
 bin/gimme-aws-creds
```

### Comparing `gimme aws creds-2.6.0/setup.py` & `gimme aws creds-2.6.1/setup.py`

 * *Files identical despite different names*

