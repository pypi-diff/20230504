# Comparing `tmp/raga-cli-0.1.7.tar.gz` & `tmp/raga-cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.1.7.tar", last modified: Tue May  2 05:13:07 2023, max compression
+gzip compressed data, was "raga-cli-0.1.8.tar", last modified: Thu May  4 07:16:41 2023, max compression
```

## Comparing `raga-cli-0.1.7.tar` & `raga-cli-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.733879 raga-cli-0.1.7/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.7/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.7/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-02 05:13:07.733586 raga-cli-0.1.7/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.7/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-05-02 05:12:38.000000 raga-cli-0.1.7/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.727245 raga-cli-0.1.7/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      631 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-05-02 05:13:07.000000 raga-cli-0.1.7/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.728021 raga-cli-0.1.7/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.729301 raga-cli-0.1.7/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.7/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.7/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2073 2023-05-02 05:12:33.000000 raga-cli-0.1.7/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)    11674 2023-05-01 18:16:51.000000 raga-cli-0.1.7/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.730540 raga-cli-0.1.7/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3383 2023-05-02 05:10:12.000000 raga-cli-0.1.7/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.7/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1839 2023-05-01 17:31:10.000000 raga-cli-0.1.7/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)    10377 2023-05-01 17:27:49.000000 raga-cli-0.1.7/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.731335 raga-cli-0.1.7/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5562 2023-05-01 17:58:40.000000 raga-cli-0.1.7/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.7/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.731609 raga-cli-0.1.7/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-02 05:13:07.733088 raga-cli-0.1.7/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1996 2023-05-01 08:38:56.000000 raga-cli-0.1.7/rc/utils/config.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6721 2023-05-01 16:53:53.000000 raga-cli-0.1.7/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-05-01 07:24:17.000000 raga-cli-0.1.7/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.7/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-05-02 05:13:07.733939 raga-cli-0.1.7/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.7/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.401707 raga-cli-0.1.8/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.1.8/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.1.8/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-04 07:16:41.401297 raga-cli-0.1.8/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.8/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2482 2023-05-04 07:15:56.000000 raga-cli-0.1.8/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.393064 raga-cli-0.1.8/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      631 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1014 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-05-04 07:16:41.000000 raga-cli-0.1.8/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.394040 raga-cli-0.1.8/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.395657 raga-cli-0.1.8/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-25 11:42:11.000000 raga-cli-0.1.8/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.1.8/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2073 2023-05-04 07:16:17.000000 raga-cli-0.1.8/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    13691 2023-05-04 06:38:24.000000 raga-cli-0.1.8/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.397134 raga-cli-0.1.8/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3406 2023-05-04 07:06:44.000000 raga-cli-0.1.8/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.1.8/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1915 2023-05-04 06:33:09.000000 raga-cli-0.1.8/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    10482 2023-05-04 07:09:20.000000 raga-cli-0.1.8/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.398218 raga-cli-0.1.8/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5589 2023-05-04 06:38:29.000000 raga-cli-0.1.8/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-27 06:30:44.000000 raga-cli-0.1.8/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.398644 raga-cli-0.1.8/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-05-04 07:16:41.400709 raga-cli-0.1.8/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1906 2023-05-04 06:47:33.000000 raga-cli-0.1.8/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1996 2023-05-01 08:38:56.000000 raga-cli-0.1.8/rc/utils/config.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6905 2023-05-04 06:55:58.000000 raga-cli-0.1.8/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-05-01 07:24:17.000000 raga-cli-0.1.8/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.1.8/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-05-04 07:16:41.401796 raga-cli-0.1.8/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.1.8/setup.py
```

### Comparing `raga-cli-0.1.7/.gitignore` & `raga-cli-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/LICENSE` & `raga-cli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/PKG-INFO` & `raga-cli-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.7/pyproject.toml` & `raga-cli-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
@@ -19,15 +19,15 @@
     "ai",
     "raga",
 ]
 license = { text = "Apache License 2.0" }
 authors = [{ name = "Manab Roy", email = "manabr@observancegroup.com" }]
 maintainers = [{ name = "Manab Roy", email = "support@observancegroup.com" }]
 dependencies = [
-    "dvc==2.38.1",
+    "dvc==2.45.1",
     "dvc_s3==2.21.0"
 ]
 [project.optional-dependencies]
 azure = ["dvc-azure==2.20.5"]
 gdrive = ["dvc-gdrive==2.19.1"]
 gs = ["dvc-gs==2.20.0"]
 hdfs = ["dvc-hdfs==2.19.0"]
```

### Comparing `raga-cli-0.1.7/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.1.8/raga_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.1.7/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.1.8/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/raga_cli.egg-info/requires.txt` & `raga-cli-0.1.8/raga_cli.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dvc==2.38.1
+dvc==2.45.1
 dvc_s3==2.21.0
 
 [all]
 dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]
 
 [azure]
 dvc-azure==2.20.5
```

### Comparing `raga-cli-0.1.7/rc/cli/__init__.py` & `raga-cli-0.1.8/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/cli/parser.py` & `raga-cli-0.1.8/rc/cli/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         add_help=False,
     )
 
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version='0.1.6',
+        version='0.1.8',
         help="Show program's version.",
     )
 
     # Sub commands
     subparsers = parser.add_subparsers(
         title="Available Commands",
         metavar="COMMAND",
```

### Comparing `raga-cli-0.1.7/rc/cli/utils.py` & `raga-cli-0.1.8/rc/cli/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -178,14 +178,59 @@
         return False
 
 def trim_slash(str):
     if str.endswith("/"):
         str = str.rsplit("/", 1)[0] 
     return str
 
+def valid_cwd_rc():
+    cwd = os.getcwd()   # get the current working directory
+    rc_dir = os.path.join(cwd, ".rc")   # create a path to the .rc directory
+    if not os.path.isdir(rc_dir):   # check if the path is a directory
+        print("Your current location is not a root directory location.")
+        sys.exit()
+    return True
+
+def find_dvc_files():
+    files = []
+    cwd = os.getcwd()   # get the current working directory
+    for file in os.listdir(cwd):   # iterate through the files in the current directory
+        if file.endswith(".dvc") and not os.path.isdir(os.path.join(cwd, file)):   # check if the file has a .dvc extension and is not a directory
+            files.append(os.path.join(cwd, file))
+    return files
+
+def match_and_delete_files(dir_list, file_list):
+    dir_names = [os.path.basename(d) for d in dir_list]   # get the names of the directories in the first list
+    for file in file_list:   # iterate through the files in the second list
+        filename = pathlib.Path(file).stem   # get the filename from the full path
+        if filename not in dir_names:   # check if the filename is not in the list of directory names
+            logger.debug(f"REMOVE DVC FILE : {filename}")
+            os.remove(file)   # delete the file if it does not have a matching directory name
+
+def check_extensions(extensions=["requirements.txt", ".pth"]):
+    found_extensions = set()
+    for extension in extensions:
+        extension_found = False
+        for subdir, dirs, filenames in os.walk("."):
+            for filename in filenames:
+                if filename.endswith(extension):
+                    found_extensions.add(extension)
+                    extension_found = True
+                    break
+            if extension_found:
+                break
+        if not extension_found:
+            print(f"{extension} file not found.")
+            sys.exit()
+    return True
+
+def valid_dot_dvc_with_folder(dirs):
+    files = find_dvc_files()
+    match_and_delete_files(dirs, files)
+    
 def get_all_data_folder():
     directory = os.getcwd()
     dirs = next(os.walk(directory))[1]
     filtered = list(filter(get_only_valid_dir, dirs))
     return filtered
 
 def compare_dot_dvc_file(dir_path):
```

### Comparing `raga-cli-0.1.7/rc/commands/get.py` & `raga-cli-0.1.8/rc/commands/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,32 +29,34 @@
             run_command_on_subprocess('git reset --hard')
             run_command_on_subprocess('git reset --hard {0}'.format(repo_commit['commit_id']))
             if tag == "dataset":
                 run_command_on_subprocess('dvc pull -f') 
             print("Files downloaded successfully") 
             logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
         else:  
+            version = self.args.version
+            commit = get_repo_commit_id(json.dumps({"repo":repo, "version":version}))
+            if not commit:
+                print(f"Version {version} not found on server.")
+                sys.exit()
             if tag == "model":
                 user_input = input("Are you sure you want to get it? [y/n]").lower()
                 if user_input == 'y':
-                    version = self.args.version
-                    commit = get_repo_commit_id(json.dumps({"repo":repo, "version":version}))
-
                     run_command_on_subprocess('git reset --hard')
                     run_command_on_subprocess('git checkout {0}'.format(commit['branch']))
                     run_command_on_subprocess('git reset --hard {0}'.format(commit['commit_id']))
                 else:
                     print("Please enter valid input")
             else:
-                commit_id = get_repo_commit_id(json.dumps({"repo":repo, "version":version}))
+                
             
                 user_input = input("Are you sure you want to get it? [y/n]").lower()
                 if user_input == 'y':
                     print("Files downloading...") 
-                    run_command_on_subprocess('git reset --hard {}'.format(commit_id['commit_id'])) 
+                    run_command_on_subprocess('git reset --hard {}'.format(commit['commit_id'])) 
                     run_command_on_subprocess('dvc pull -f') 
                     run_command_on_subprocess('git clean -df') 
                     print("Files downloaded successfully") 
                     logger.debug('DOWNLOAD TIME {0}'.format(timedelta(seconds=timer()-start))) 
                 else:
                     print("Please enter valid input")
```

### Comparing `raga-cli-0.1.7/rc/commands/list.py` & `raga-cli-0.1.8/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/commands/put.py` & `raga-cli-0.1.8/rc/commands/put.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,20 @@
         if getattr(self.args, "path", None):
             self.dirs = [self.args.path]
         else:
             self.dirs = get_all_data_folder()         
 
     def run(self):        
         log_setup(self.args)
-        # print(get_config_value("repo"))
+        # print()
         # return
+        valid_cwd_rc()
         self.args.path = self.dirs
+        valid_dot_dvc_with_folder(self.args.path)
+        # print(self.dirs)
         put(self.args) 
         return 0
 
 
 def add_parser(subparsers, parent_parser):
     REPO_HELP = "Put File or folder. Use: `rc put <file or folder path> -m <commit message>`"
     REPO_DESCRIPTION = (
```

### Comparing `raga-cli-0.1.7/rc/commands/repo.py` & `raga-cli-0.1.8/rc/commands/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def __init__(self) -> None:
         self.CLOUD_STORAGE_BUCKET = get_config_value_by_key('bucket_name')
         self.CLOUD_STORAGE_DIR = get_config_value_by_key('cloud_storage_dir')
         self.CLOUD_STORAGE_LOCATION = f"s3://{self.CLOUD_STORAGE_BUCKET}/{self.CLOUD_STORAGE_DIR}"
         self.INITIAL_COMMIT = get_config_value_by_key('git_initial_commit')
         self.GIT_BRANCH = get_config_value_by_key('git_initial_branch')
         self.GIT_ORG = get_config_value_by_key('git_org')
+        self.AUTH_TOKEN = get_config_value_by_key('auth_token')
         self.TAGS = {"dataset", "model"}
         self.created_by = pwd.getpwuid(os.getuid()).pw_name 
 
     def run_git_commands(self,repo_name, repo_tag):
         run_command_on_subprocess("git add .rc", repo_name)       
         run_command_on_subprocess("git commit -m '{0}' -a".format(self.INITIAL_COMMIT), repo_name)    
         run_command_on_subprocess("git branch -M {0}".format(self.GIT_BRANCH), repo_name)    
@@ -70,36 +71,36 @@
             "remote_bucket":self.CLOUD_STORAGE_BUCKET,
             "remote_bucket_dir":self.CLOUD_STORAGE_DIR,
             "remote_bucket_location":self.CLOUD_STORAGE_LOCATION,
             "secret_key":secret_key,
             "access_key":access_key,
             "version":0,
             "repo_id":"", 
-            "tag":repo_tag
+            "tag":repo_tag,
+            "auth_token":self.AUTH_TOKEN
         }  
         create_rc_folder(repo_name, configs)
 
     
     def create_repo(self, args):
+        print("Repo creating...")  
         if self.check_git_init():
             print("The repo creating process inside the repository is not possible.")
             sys.exit(50) 
         logger.debug(f"START CREATE REPO COMMAND")
         repository_name = args.name    
         repository_tag = args.tag 
         if is_repo_exist_in_gh("{0}/{1}".format(self.GIT_ORG, repository_name)):
             print("The repo creating process could not be completed because the repo already exists. Please rename repo and try again.")
             sys.exit(50)
 
         if folder_exists(repository_name):
             print("The repo creating process could not be completed because the directory already exists. Please rename repo and try again.")
             sys.exit(50)
 
-        print("Repo creating...")  
-
         if repository_tag not in self.TAGS:
             logger.error("'{0}' tag is not available. Please select from {1}".format(repository_tag, self.TAGS))
             sys.exit(50)   
 
         
         self.run_repo_create_subprocesses(repository_name, repository_tag)
         git_repo = get_git_url(repository_name)
```

### Comparing `raga-cli-0.1.7/rc/exceptions.py` & `raga-cli-0.1.8/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/prompt.py` & `raga-cli-0.1.8/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/repo/get.py` & `raga-cli-0.1.8/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/repo/put.py` & `raga-cli-0.1.8/rc/repo/put.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
         # Start both threads
         
         # Wait for both threads to finish
         http_thread.join()
         make_repo_commit(message)
         
     elif tag == "model":
+        check_extensions()
         if check_push_left():
             print('Please use "git push" to publish your local commits')
             sys.exit()
         model_version = model_current_version(repo)
         model_upload(message, repo, model_version)
     
     update_repo_lock(repo, json.dumps({"locked":False}))
```

### Comparing `raga-cli-0.1.7/rc/utils/__init__.py` & `raga-cli-0.1.8/rc/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import colorama
 from pathlib import Path
 import pathlib
 
 
 BASE_URL = 'http://ec2-13-127-105-156.ap-south-1.compute.amazonaws.com:8092/v1/api'
+WEB_BACKEND_URL = 'http://13.127.105.156:8080/api'
 DEBUG = False
 RCTL_PATH = '.rctl'
 RCTL_LOG_PATH = f'{RCTL_PATH}/logs'
 RCTL_LOG_FILE = f'{RCTL_LOG_PATH}/rctl.log'
 
 
 def format_link(link):
```

### Comparing `raga-cli-0.1.7/rc/utils/config.py` & `raga-cli-0.1.8/rc/utils/config.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.1.7/rc/utils/request.py` & `raga-cli-0.1.8/rc/utils/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import sys
 import requests
 
-from rc.utils import BASE_URL
+from rc.utils import BASE_URL, WEB_BACKEND_URL
+from rc.utils.config import set_config_value
 
 logger = logging.getLogger(__name__)
 
 class RctlValidRequestError(Exception):
     def __init__(self, msg, *args):
         assert msg
         self.msg = msg
@@ -31,16 +32,18 @@
     
     else:
         if 'message' not in response.keys():
             raise RctlValidRequestError("HTTP response `message` keyword not found.")
         raise RctlValidRequestError("HTTP response {0}".format(response["message"]))
 
 
-def make_request(url, method, data = None):
+def make_request(url, method, data = None, auth_token=None):
     headers = {'Content-Type': 'application/json'}
+    if auth_token:
+        headers['Authorization'] = f'Bearer {auth_token}'
     logger.debug("URL: {}".format(url))
     logger.debug("PAYLOAD: {}".format(data))
     try:
         response = requests.request(method, url, headers = headers, data = data)
         if not (200 <= response.status_code < 300):
             logger.error('HTTP {}'.format(response.content))
             if response.json()['status'] == 404:
@@ -181,9 +184,12 @@
 def get_commit_repo(id):
     url = f"{BASE_URL}/repocommit?key={id}"
     response = valid_response(make_request(url, "GET"))
     data = response["data"]
     logger.debug("RESPONSE VALUE FROM URL: {0} --- VALUE : {1}".format(url, data))
     return data
 
+# def model_upload_web():
+
+
```

### Comparing `raga-cli-0.1.7/rc/utils/sshKeyGen.py` & `raga-cli-0.1.8/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

