# Comparing `tmp/crms-2023.4.5.1739.tar.gz` & `tmp/crms-2023.5.3.1340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crms-2023.4.5.1739.tar", last modified: Wed Apr  5 08:53:58 2023, max compression
+gzip compressed data, was "crms-2023.5.3.1340.tar", last modified: Thu May  4 04:42:39 2023, max compression
```

## Comparing `crms-2023.4.5.1739.tar` & `crms-2023.5.3.1340.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-04-05 08:53:58.259377 crms-2023.4.5.1739/
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     4292 2023-04-05 08:53:58.259377 crms-2023.4.5.1739/PKG-INFO
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     3165 2023-03-22 07:27:17.000000 crms-2023.4.5.1739/README.md
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)       38 2023-04-05 08:53:58.259377 crms-2023.4.5.1739/setup.cfg
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      780 2023-04-05 08:40:44.000000 crms-2023.4.5.1739/setup.py
-drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-04-05 08:53:58.223377 crms-2023.4.5.1739/src/
-drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-04-05 08:53:58.223377 crms-2023.4.5.1739/src/crms/
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      352 2022-08-29 00:49:38.000000 crms-2023.4.5.1739/src/crms/__init__.py
--rwxrwxr-x   0 jangcs    (1000) jangcs    (1000)    35290 2023-04-05 08:50:37.000000 crms-2023.4.5.1739/src/crms/crms.py
-drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-04-05 08:53:58.243377 crms-2023.4.5.1739/src/crms/other_data/
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000) 40371968 2022-08-26 07:22:07.000000 crms-2023.4.5.1739/src/crms/other_data/m1.pth
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000) 40393951 2022-08-29 01:56:34.000000 crms-2023.4.5.1739/src/crms/other_data/m2.pth
--rwxrwxr-x   0 jangcs    (1000) jangcs    (1000)    29361 2022-09-16 05:16:03.000000 crms-2023.4.5.1739/src/crms/watchdog.py
-drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-04-05 08:53:58.223377 crms-2023.4.5.1739/src/crms.egg-info/
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     4292 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/PKG-INFO
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      325 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/SOURCES.txt
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)        1 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/dependency_links.txt
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)       41 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/entry_points.txt
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      103 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/requires.txt
--rw-rw-r--   0 jangcs    (1000) jangcs    (1000)        5 2023-04-05 08:53:58.000000 crms-2023.4.5.1739/src/crms.egg-info/top_level.txt
+drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-05-04 04:42:39.404797 crms-2023.5.3.1340/
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     4292 2023-05-04 04:42:39.404797 crms-2023.5.3.1340/PKG-INFO
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     3165 2023-03-22 07:27:17.000000 crms-2023.5.3.1340/README.md
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)       38 2023-05-04 04:42:39.404797 crms-2023.5.3.1340/setup.cfg
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      780 2023-05-04 04:41:46.000000 crms-2023.5.3.1340/setup.py
+drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-05-04 04:42:39.348797 crms-2023.5.3.1340/src/
+drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-05-04 04:42:39.348797 crms-2023.5.3.1340/src/crms/
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      352 2022-08-29 00:49:38.000000 crms-2023.5.3.1340/src/crms/__init__.py
+-rwxrwxr-x   0 jangcs    (1000) jangcs    (1000)    35311 2023-05-04 04:42:10.000000 crms-2023.5.3.1340/src/crms/crms.py
+drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-05-04 04:42:39.376797 crms-2023.5.3.1340/src/crms/other_data/
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000) 40371968 2022-08-26 07:22:07.000000 crms-2023.5.3.1340/src/crms/other_data/m1.pth
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000) 40393951 2022-08-29 01:56:34.000000 crms-2023.5.3.1340/src/crms/other_data/m2.pth
+-rwxrwxr-x   0 jangcs    (1000) jangcs    (1000)    29361 2022-09-16 05:16:03.000000 crms-2023.5.3.1340/src/crms/watchdog.py
+drwxrwxr-x   0 jangcs    (1000) jangcs    (1000)        0 2023-05-04 04:42:39.352797 crms-2023.5.3.1340/src/crms.egg-info/
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)     4292 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/PKG-INFO
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      325 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)        1 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)       41 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/entry_points.txt
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)      103 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/requires.txt
+-rw-rw-r--   0 jangcs    (1000) jangcs    (1000)        5 2023-05-04 04:42:39.000000 crms-2023.5.3.1340/src/crms.egg-info/top_level.txt
```

### Comparing `crms-2023.4.5.1739/PKG-INFO` & `crms-2023.5.3.1340/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crms
-Version: 2023.4.5.1739
+Version: 2023.5.3.1340
 Summary: Cloud Robot Model Sharing Middleware
 Home-page: https://github.com/jangcs/crms
 Author: jangcs
 Author-email: jangcs@etri.re.kr
 License: UNKNOWN
 Description: **CRMS CLI Installation**
         ===
```

### Comparing `crms-2023.4.5.1739/README.md` & `crms-2023.5.3.1340/README.md`

 * *Files identical despite different names*

### Comparing `crms-2023.4.5.1739/setup.py` & `crms-2023.5.3.1340/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'protobuf==3.20.1',
 	'requests>=2.28.1',
 	'fsspec==2022.2.0'
 ]
 
 setup(
     name='crms',
-    version='2023.04.05.1739',
+    version='2023.05.03.1340',
     description='Cloud Robot Model Sharing Middleware',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='jangcs',
     author_email='jangcs@etri.re.kr',
     url="https://github.com/jangcs/crms",
     packages=find_packages(where='src'),
```

### Comparing `crms-2023.4.5.1739/src/crms/crms.py` & `crms-2023.5.3.1340/src/crms/crms.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,16 +612,15 @@
         if len(doc_dicts) ==  0 :
             print_verbose(verbose, "ERROR: model for " +  arg_model_url  + " does not exist.")
             raise Exception("CRMS ERROR: model for " +  arg_model_url  + " does not exist.")
 
         doc = doc_dicts[0]
         git_repository = doc['git_repository']
 
-        modified_model_url = git_repository.replace('git@github.com:', 'https://github.com/',1)
-
+        modified_model_url = git_repository.replace('https://github.com/','git@github.com:', 1)
 
     if arg_target != '' :
         target = arg_target
     else :
         # target = os.path.join( os.getcwd(), args.model_name)
         # target = os.path.join( os.getcwd(), "model_crms")
         target = os.path.join( os.getcwd(), os.path.basename(arg_model_url).split('.')[0] )   # git@github.com:jangcs/KKK.git -> KKK.git -> ['KKK', 'git']
@@ -761,15 +760,15 @@
     print_verbose(args.verbose, "CRMS LIST....")
     doc_ids = crms_list(verbose=args.verbose)
 
     for doc_id in doc_ids:
         print(doc_id)
     print_verbose(args.verbose, "CRMS LIST Completed !!!")
 
-CRMS_VERSION_STR = "2023.04.05.1739"
+CRMS_VERSION_STR = "2023.05.04.1340"
 
 def crms_ver(verbose=False):
     print_verbose(verbose, "Print Version")
     return CRMS_VERSION_STR
 
 def crms_ver_cli(args):
     print(crms_ver(args.verbose))
@@ -805,16 +804,16 @@
     sub_parsers = arg_parser.add_subparsers(dest="cmd", help="sub-command help", required=True)
     
     parser_conf =   sub_parsers.add_parser('conf',  help="CRMS CONFIG : crms conf <git_remote_url> <dvc_remote_url>")
     parser_conf_mod =   sub_parsers.add_parser('conf_mod',  help="CRMS CONFIG MODIFY : crms conf_mod [-g <git_remote_url>] [-d <dvc_remote_url>]" )
     parser_init =   sub_parsers.add_parser('init',  help="CRMS INIT : crms init <model_name>" )
     parser_add  =   sub_parsers.add_parser('add',   help="CRMS ADDS MODEL_FILES: crms add <model_files>...")
     parser_push =   sub_parsers.add_parser('push',  help="CRMS PUSHES MODEL_FILES With VERSION_TAG : crms push <version>")
-    parser_pull =   sub_parsers.add_parser('pull',  help="CRMS PULL MODEL With VERSION_TAG : crms pull <model_url> [--version=<latest>|<version_tag>] [--target=<target_dir>] ")
-    parser_clone =  sub_parsers.add_parser('clone',  help="CRMS CLONE MODEL With Latest Version : crms clone <model_url> [--target=<target_dir>] ")
+    parser_pull =   sub_parsers.add_parser('pull',  help="CRMS PULL MODEL With VERSION_TAG : crms pull <model_url|model_name> [--version=<latest>|<version_tag>] [--target=<target_dir>] ")
+    parser_clone =  sub_parsers.add_parser('clone',  help="CRMS CLONE MODEL With Latest Version : crms clone <model_url|model_name> [--target=<target_dir>] ")
     parser_list =   sub_parsers.add_parser('list',  help="CRMS LIST Models : crms list")
     parser_desc =   sub_parsers.add_parser('desc',  help="CRMS DESCRIBE MODEL Versions : crms desc <model_name> ")
     parser_ver  =   sub_parsers.add_parser('version',  help="CRMS Version Print : crms version")
 
     parser_conf.add_argument("git_remote", type=str,  action="store", help="git_remote_url is required")
     parser_conf.add_argument("dvc_remote", type=str,  action="store", help="dvc_remote_url is required")
     parser_conf.add_argument("-V", "--verbose", action="store_true", help="verbose mode")
```

### Comparing `crms-2023.4.5.1739/src/crms/other_data/m1.pth` & `crms-2023.5.3.1340/src/crms/other_data/m1.pth`

 * *Files identical despite different names*

### Comparing `crms-2023.4.5.1739/src/crms/other_data/m2.pth` & `crms-2023.5.3.1340/src/crms/other_data/m2.pth`

 * *Files identical despite different names*

### Comparing `crms-2023.4.5.1739/src/crms/watchdog.py` & `crms-2023.5.3.1340/src/crms/watchdog.py`

 * *Files identical despite different names*

### Comparing `crms-2023.4.5.1739/src/crms.egg-info/PKG-INFO` & `crms-2023.5.3.1340/src/crms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crms
-Version: 2023.4.5.1739
+Version: 2023.5.3.1340
 Summary: Cloud Robot Model Sharing Middleware
 Home-page: https://github.com/jangcs/crms
 Author: jangcs
 Author-email: jangcs@etri.re.kr
 License: UNKNOWN
 Description: **CRMS CLI Installation**
         ===
```

