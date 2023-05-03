# Comparing `tmp/git-smartmv-1.0.1.tar.gz` & `tmp/git-smartmv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-smartmv-1.0.1.tar", last modified: Wed May  3 22:05:51 2023, max compression
+gzip compressed data, was "git-smartmv-1.0.2.tar", last modified: Wed May  3 22:14:42 2023, max compression
```

## Comparing `git-smartmv-1.0.1.tar` & `git-smartmv-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/
--rw-r--r--   0 work      (1000) work      (1000)       26 2023-05-03 19:45:45.000000 git-smartmv-1.0.1/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)    35149 2023-05-03 19:17:42.000000 git-smartmv-1.0.1/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)     2882 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)     2103 2023-05-03 22:02:12.000000 git-smartmv-1.0.1/README.md
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/git_smartmv/
--rwxr-xr-x   0 work      (1000) work      (1000)    12569 2023-05-03 21:19:21.000000 git-smartmv-1.0.1/git_smartmv/__init__.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/git_smartmv.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     2882 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      239 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       76 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)       12 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/top_level.txt
--rw-r--r--   0 work      (1000) work      (1000)       38 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1330 2023-05-03 22:02:35.000000 git-smartmv-1.0.1/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:14:42.338406 git-smartmv-1.0.2/
+-rw-r--r--   0 work      (1000) work      (1000)       26 2023-05-03 19:45:45.000000 git-smartmv-1.0.2/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)    35149 2023-05-03 19:17:42.000000 git-smartmv-1.0.2/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)     2880 2023-05-03 22:14:42.338406 git-smartmv-1.0.2/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)     2101 2023-05-03 22:10:22.000000 git-smartmv-1.0.2/README.md
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:14:42.338406 git-smartmv-1.0.2/git_smartmv/
+-rwxr-xr-x   0 work      (1000) work      (1000)    12569 2023-05-03 21:19:21.000000 git-smartmv-1.0.2/git_smartmv/__init__.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:14:42.338406 git-smartmv-1.0.2/git_smartmv.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     2880 2023-05-03 22:14:42.000000 git-smartmv-1.0.2/git_smartmv.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      239 2023-05-03 22:14:42.000000 git-smartmv-1.0.2/git_smartmv.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2023-05-03 22:14:42.000000 git-smartmv-1.0.2/git_smartmv.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)       76 2023-05-03 22:14:42.000000 git-smartmv-1.0.2/git_smartmv.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)       12 2023-05-03 22:14:42.000000 git-smartmv-1.0.2/git_smartmv.egg-info/top_level.txt
+-rw-r--r--   0 work      (1000) work      (1000)       38 2023-05-03 22:14:42.338406 git-smartmv-1.0.2/setup.cfg
+-rwxr-xr-x   0 work      (1000) work      (1000)     1330 2023-05-03 22:12:42.000000 git-smartmv-1.0.2/setup.py
```

### Comparing `git-smartmv-1.0.1/LICENSE` & `git-smartmv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git-smartmv-1.0.1/PKG-INFO` & `git-smartmv-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-smartmv
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line tool that can decide whether to use `git mv` or `mv`.
 Home-page: https://github.com/jamescherti/git-smartmv
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
-command-line tool for moving files and/or directories without having to worry
-about manually choosing whether to use `git mv` or `mv`.
+The `git-smartmv` command-line tool, written by [James Cherti](https://www.jamescherti.com),
+allows moving files and/or directories without having to worry about
+manually choosing whether to use `git mv` or `mv`.
 
 It can determines whether to use `git mv` or `mv` based on the source and the
 destination path:
 - If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
 - If the files/directories are being moved between a Git repository and a
   non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
```

### Comparing `git-smartmv-1.0.1/README.md` & `git-smartmv-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
-command-line tool for moving files and/or directories without having to worry
-about manually choosing whether to use `git mv` or `mv`.
+The `git-smartmv` command-line tool, written by [James Cherti](https://www.jamescherti.com),
+allows moving files and/or directories without having to worry about
+manually choosing whether to use `git mv` or `mv`.
 
 It can determines whether to use `git mv` or `mv` based on the source and the
 destination path:
 - If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
 - If the files/directories are being moved between a Git repository and a
   non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
```

### Comparing `git-smartmv-1.0.1/git_smartmv/__init__.py` & `git-smartmv-1.0.2/git_smartmv/__init__.py`

 * *Files identical despite different names*

### Comparing `git-smartmv-1.0.1/git_smartmv.egg-info/PKG-INFO` & `git-smartmv-1.0.2/git_smartmv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-smartmv
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command-line tool that can decide whether to use `git mv` or `mv`.
 Home-page: https://github.com/jamescherti/git-smartmv
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
-command-line tool for moving files and/or directories without having to worry
-about manually choosing whether to use `git mv` or `mv`.
+The `git-smartmv` command-line tool, written by [James Cherti](https://www.jamescherti.com),
+allows moving files and/or directories without having to worry about
+manually choosing whether to use `git mv` or `mv`.
 
 It can determines whether to use `git mv` or `mv` based on the source and the
 destination path:
 - If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
 - If the files/directories are being moved between a Git repository and a
   non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
```

### Comparing `git-smartmv-1.0.1/setup.py` & `git-smartmv-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="git-smartmv",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     description=("A command-line tool that can decide whether to "
                  "use `git mv` or `mv`."),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/git-smartmv",
     author="James Cherti",
```

