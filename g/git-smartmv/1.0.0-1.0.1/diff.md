# Comparing `tmp/git-smartmv-1.0.0.tar.gz` & `tmp/git-smartmv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-smartmv-1.0.0.tar", last modified: Wed May  3 21:25:45 2023, max compression
+gzip compressed data, was "git-smartmv-1.0.1.tar", last modified: Wed May  3 22:05:51 2023, max compression
```

## Comparing `git-smartmv-1.0.0.tar` & `git-smartmv-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 21:25:45.294448 git-smartmv-1.0.0/
--rw-r--r--   0 work      (1000) work      (1000)       26 2023-05-03 19:45:45.000000 git-smartmv-1.0.0/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)    35149 2023-05-03 19:17:42.000000 git-smartmv-1.0.0/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)     3036 2023-05-03 21:25:45.294448 git-smartmv-1.0.0/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)     2257 2023-05-03 21:20:41.000000 git-smartmv-1.0.0/README.md
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 21:25:45.294448 git-smartmv-1.0.0/git_smartmv/
--rwxr-xr-x   0 work      (1000) work      (1000)    12569 2023-05-03 21:19:21.000000 git-smartmv-1.0.0/git_smartmv/__init__.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 21:25:45.294448 git-smartmv-1.0.0/git_smartmv.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     3036 2023-05-03 21:25:45.000000 git-smartmv-1.0.0/git_smartmv.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      239 2023-05-03 21:25:45.000000 git-smartmv-1.0.0/git_smartmv.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2023-05-03 21:25:45.000000 git-smartmv-1.0.0/git_smartmv.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       76 2023-05-03 21:25:45.000000 git-smartmv-1.0.0/git_smartmv.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)       12 2023-05-03 21:25:45.000000 git-smartmv-1.0.0/git_smartmv.egg-info/top_level.txt
--rw-r--r--   0 work      (1000) work      (1000)       38 2023-05-03 21:25:45.294448 git-smartmv-1.0.0/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1330 2023-05-03 19:43:10.000000 git-smartmv-1.0.0/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/
+-rw-r--r--   0 work      (1000) work      (1000)       26 2023-05-03 19:45:45.000000 git-smartmv-1.0.1/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)    35149 2023-05-03 19:17:42.000000 git-smartmv-1.0.1/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)     2882 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)     2103 2023-05-03 22:02:12.000000 git-smartmv-1.0.1/README.md
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/git_smartmv/
+-rwxr-xr-x   0 work      (1000) work      (1000)    12569 2023-05-03 21:19:21.000000 git-smartmv-1.0.1/git_smartmv/__init__.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/git_smartmv.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     2882 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      239 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)       76 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)       12 2023-05-03 22:05:51.000000 git-smartmv-1.0.1/git_smartmv.egg-info/top_level.txt
+-rw-r--r--   0 work      (1000) work      (1000)       38 2023-05-03 22:05:51.726343 git-smartmv-1.0.1/setup.cfg
+-rwxr-xr-x   0 work      (1000) work      (1000)     1330 2023-05-03 22:02:35.000000 git-smartmv-1.0.1/setup.py
```

### Comparing `git-smartmv-1.0.0/LICENSE` & `git-smartmv-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-smartmv-1.0.0/PKG-INFO` & `git-smartmv-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-smartmv
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line tool that can decide whether to use `git mv` or `mv`.
 Home-page: https://github.com/jamescherti/git-smartmv
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -15,77 +15,72 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv` is a command-line tool, written by
-[James Cherti](https://www.jamescherti.com), for moving files and
-directories without having to worry about manually choosing whether to use
-`git mv` or `mv`.
-
-The `git-smartmv` tool determines whether to use `git mv` or `mv` based on the
-source and the destination path:
-- If the file or directory is being moved within a Git repository,
+The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
+command-line tool for moving files and/or directories without having to worry
+about manually choosing whether to use `git mv` or `mv`.
+
+It can determines whether to use `git mv` or `mv` based on the source and the
+destination path:
+- If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
-- If the file is being moved between a Git repository and a non-Git directory
-  or a different Git repository, `git-smartmv` uses `mv`.
+- If the files/directories are being moved between a Git repository and a
+  non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
 
 ## Installation
 
 ```
 sudo pip install git-smartmv
 ```
 
 ## Shell alias
 
-It is recommended to add the following alias to `~/.bashrc`:
+To simplify the usage of this tool, you can add the following line to
+your `~/.bashrc`:
 ```
 alias mv="git-smartmv"
 ```
 
 ## Usage
 
-The `git-smartmv` command-line tool accepts the same arguments as the `mv`
+The `git-smartmv` command-line tool accepts similar arguments as the `mv`
 command, including the source file or directory to be moved, and the
 destination file or directory.
-```usage: git-smartmv [--option] <SOURCE>... <DEST>
-
-A command-line tool that can decide whether to use `git mv` or `mv`.
-
-positional arguments:
-  args                  Files and/or directories
+```
+usage: git-smartmv [--option] <SOURCE>... <DEST>
 
 options:
-  -h, --help            show this help message and exit
   -w WARNING_THRESHOLD, --warning-threshold WARNING_THRESHOLD
                         This will raise a warning if the number of files or directories being moved
                         exceeds the specified amount
   -v, --verbose         Report the names of the files and/or directories as they are being moved.
   -f, --force           Force renaming or moving of files and/or directories even if the destination
                         exists.
   -p, --non-interactive
                         Do not prompt the user to confirm before executing 'mv' and/or 'git mv'
                         commands.
 ```
 
 First example:
 ```
-git smartmv file1 dir1/ file2 file3 directory/
+git smartmv file1 file2
 ```
 
 Second example:
 ```
-git smartmv file1 file2
+git smartmv file1 dir1/ file2 file3 directory/
 ```
 
 Third example (non-interactive):
 ```
-git smartmv -f dir1/ dir2/
+git smartmv --non-interactive dir1/ dir2/
 ```
 
 ## License
 
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
```

### Comparing `git-smartmv-1.0.0/README.md` & `git-smartmv-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv` is a command-line tool, written by
-[James Cherti](https://www.jamescherti.com), for moving files and
-directories without having to worry about manually choosing whether to use
-`git mv` or `mv`.
-
-The `git-smartmv` tool determines whether to use `git mv` or `mv` based on the
-source and the destination path:
-- If the file or directory is being moved within a Git repository,
+The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
+command-line tool for moving files and/or directories without having to worry
+about manually choosing whether to use `git mv` or `mv`.
+
+It can determines whether to use `git mv` or `mv` based on the source and the
+destination path:
+- If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
-- If the file is being moved between a Git repository and a non-Git directory
-  or a different Git repository, `git-smartmv` uses `mv`.
+- If the files/directories are being moved between a Git repository and a
+  non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
 
 ## Installation
 
 ```
 sudo pip install git-smartmv
 ```
 
 ## Shell alias
 
-It is recommended to add the following alias to `~/.bashrc`:
+To simplify the usage of this tool, you can add the following line to
+your `~/.bashrc`:
 ```
 alias mv="git-smartmv"
 ```
 
 ## Usage
 
-The `git-smartmv` command-line tool accepts the same arguments as the `mv`
+The `git-smartmv` command-line tool accepts similar arguments as the `mv`
 command, including the source file or directory to be moved, and the
 destination file or directory.
-```usage: git-smartmv [--option] <SOURCE>... <DEST>
-
-A command-line tool that can decide whether to use `git mv` or `mv`.
-
-positional arguments:
-  args                  Files and/or directories
+```
+usage: git-smartmv [--option] <SOURCE>... <DEST>
 
 options:
-  -h, --help            show this help message and exit
   -w WARNING_THRESHOLD, --warning-threshold WARNING_THRESHOLD
                         This will raise a warning if the number of files or directories being moved
                         exceeds the specified amount
   -v, --verbose         Report the names of the files and/or directories as they are being moved.
   -f, --force           Force renaming or moving of files and/or directories even if the destination
                         exists.
   -p, --non-interactive
                         Do not prompt the user to confirm before executing 'mv' and/or 'git mv'
                         commands.
 ```
 
 First example:
 ```
-git smartmv file1 dir1/ file2 file3 directory/
+git smartmv file1 file2
 ```
 
 Second example:
 ```
-git smartmv file1 file2
+git smartmv file1 dir1/ file2 file3 directory/
 ```
 
 Third example (non-interactive):
 ```
-git smartmv -f dir1/ dir2/
+git smartmv --non-interactive dir1/ dir2/
 ```
 
 ## License
 
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
```

### Comparing `git-smartmv-1.0.0/git_smartmv/__init__.py` & `git-smartmv-1.0.1/git_smartmv/__init__.py`

 * *Files identical despite different names*

### Comparing `git-smartmv-1.0.0/git_smartmv.egg-info/PKG-INFO` & `git-smartmv-1.0.1/git_smartmv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-smartmv
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line tool that can decide whether to use `git mv` or `mv`.
 Home-page: https://github.com/jamescherti/git-smartmv
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
@@ -15,77 +15,72 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-smartmv - A tool that can decide whether to use `git mv` or `mv`
 
-The `git-smartmv` is a command-line tool, written by
-[James Cherti](https://www.jamescherti.com), for moving files and
-directories without having to worry about manually choosing whether to use
-`git mv` or `mv`.
-
-The `git-smartmv` tool determines whether to use `git mv` or `mv` based on the
-source and the destination path:
-- If the file or directory is being moved within a Git repository,
+The `git-smartmv`, written by [James Cherti](https://www.jamescherti.com), is a
+command-line tool for moving files and/or directories without having to worry
+about manually choosing whether to use `git mv` or `mv`.
+
+It can determines whether to use `git mv` or `mv` based on the source and the
+destination path:
+- If the files/directories are being moved within a Git repository,
   `git-smartmv` uses `git mv`.
-- If the file is being moved between a Git repository and a non-Git directory
-  or a different Git repository, `git-smartmv` uses `mv`.
+- If the files/directories are being moved between a Git repository and a
+  non-Git directory or a different Git repository, `git-smartmv` uses `mv`.
 
 ## Installation
 
 ```
 sudo pip install git-smartmv
 ```
 
 ## Shell alias
 
-It is recommended to add the following alias to `~/.bashrc`:
+To simplify the usage of this tool, you can add the following line to
+your `~/.bashrc`:
 ```
 alias mv="git-smartmv"
 ```
 
 ## Usage
 
-The `git-smartmv` command-line tool accepts the same arguments as the `mv`
+The `git-smartmv` command-line tool accepts similar arguments as the `mv`
 command, including the source file or directory to be moved, and the
 destination file or directory.
-```usage: git-smartmv [--option] <SOURCE>... <DEST>
-
-A command-line tool that can decide whether to use `git mv` or `mv`.
-
-positional arguments:
-  args                  Files and/or directories
+```
+usage: git-smartmv [--option] <SOURCE>... <DEST>
 
 options:
-  -h, --help            show this help message and exit
   -w WARNING_THRESHOLD, --warning-threshold WARNING_THRESHOLD
                         This will raise a warning if the number of files or directories being moved
                         exceeds the specified amount
   -v, --verbose         Report the names of the files and/or directories as they are being moved.
   -f, --force           Force renaming or moving of files and/or directories even if the destination
                         exists.
   -p, --non-interactive
                         Do not prompt the user to confirm before executing 'mv' and/or 'git mv'
                         commands.
 ```
 
 First example:
 ```
-git smartmv file1 dir1/ file2 file3 directory/
+git smartmv file1 file2
 ```
 
 Second example:
 ```
-git smartmv file1 file2
+git smartmv file1 dir1/ file2 file3 directory/
 ```
 
 Third example (non-interactive):
 ```
-git smartmv -f dir1/ dir2/
+git smartmv --non-interactive dir1/ dir2/
 ```
 
 ## License
 
 Distributed under terms of the GNU General Public License version 3.
 
 ## Links
```

### Comparing `git-smartmv-1.0.0/setup.py` & `git-smartmv-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="git-smartmv",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     description=("A command-line tool that can decide whether to "
                  "use `git mv` or `mv`."),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/git-smartmv",
     author="James Cherti",
```

