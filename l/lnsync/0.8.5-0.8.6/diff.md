# Comparing `tmp/lnsync-0.8.5.tar.gz` & `tmp/lnsync-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lnsync-0.8.5.tar", last modified: Mon Aug 22 13:28:25 2022, max compression
+gzip compressed data, was "dist/lnsync-0.8.6.tar", last modified: Thu May  4 15:02:35 2023, max compression
```

## Comparing `lnsync-0.8.5.tar` & `lnsync-0.8.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2022-08-22 13:28:25.000000 lnsync-0.8.5/
-drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2022-08-22 13:28:24.000000 lnsync-0.8.5/lnsync.egg-info/
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       22 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/top_level.txt
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     1049 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/SOURCES.txt
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      175 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/entry_points.txt
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       14 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/requires.txt
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)        1 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/dependency_links.txt
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23039 2022-08-22 13:28:21.000000 lnsync-0.8.5/lnsync.egg-info/PKG-INFO
-drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2022-08-22 13:28:25.000000 lnsync-0.8.5/random_pkg/
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    11627 2021-03-15 14:41:14.000000 lnsync-0.8.5/random_pkg/random_tree.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)        0 2019-07-03 12:20:35.000000 lnsync-0.8.5/random_pkg/__init__.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     2841 2020-12-17 13:26:58.000000 lnsync-0.8.5/random_pkg/random_extras.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    19609 2022-08-22 13:26:30.000000 lnsync-0.8.5/README.md
-drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2022-08-22 13:28:25.000000 lnsync-0.8.5/lnsync_pkg/
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     3633 2022-05-23 07:31:25.000000 lnsync-0.8.5/lnsync_pkg/prefixdbname.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12799 2022-04-27 16:25:44.000000 lnsync-0.8.5/lnsync_pkg/lnsync_treeargs.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5154 2022-05-23 07:31:25.000000 lnsync-0.8.5/lnsync_pkg/fileid.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     7053 2022-06-11 13:20:42.000000 lnsync-0.8.5/lnsync_pkg/miscutils.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5120 2022-04-27 11:55:48.000000 lnsync-0.8.5/lnsync_pkg/thread_utils.py
--rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)    37689 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/lnsync.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4191 2021-10-16 09:16:01.000000 lnsync-0.8.5/lnsync_pkg/human2bytes.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5142 2022-02-19 09:06:06.000000 lnsync-0.8.5/lnsync_pkg/groupedfileprinter.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    10183 2022-03-08 21:26:31.000000 lnsync-0.8.5/lnsync_pkg/glob_matcher.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     8449 2022-03-09 23:40:45.000000 lnsync-0.8.5/lnsync_pkg/printutils.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12468 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/fdupes.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     2066 2022-04-27 11:55:48.000000 lnsync-0.8.5/lnsync_pkg/lnsync_api.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4714 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/onegraph.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      665 2021-12-26 12:07:22.000000 lnsync-0.8.5/lnsync_pkg/propdbmanager.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4638 2022-04-27 11:55:48.000000 lnsync-0.8.5/lnsync_pkg/filehashtree.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    26453 2022-04-27 11:55:48.000000 lnsync-0.8.5/lnsync_pkg/matcher.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     1544 2022-03-05 13:48:54.000000 lnsync-0.8.5/lnsync_pkg/gnome_thumbnailer.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      218 2021-02-05 11:57:06.000000 lnsync-0.8.5/lnsync_pkg/__init__.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    33299 2022-04-27 11:55:48.000000 lnsync-0.8.5/lnsync_pkg/filetree.py
--rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     3265 2022-05-23 07:31:25.000000 lnsync-0.8.5/lnsync_pkg/image_dhash.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12243 2022-02-02 18:11:16.000000 lnsync-0.8.5/lnsync_pkg/argparse_scoped.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     8726 2021-10-16 09:16:01.000000 lnsync-0.8.5/lnsync_pkg/modaltype.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23973 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/fileproptree.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    29888 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/lnsync_cmd_handlers.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23068 2022-04-01 12:18:52.000000 lnsync-0.8.5/lnsync_pkg/sqlpropdb.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      787 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/metadata.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    20663 2022-08-22 13:26:30.000000 lnsync-0.8.5/lnsync_pkg/argparse_config.py
--rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     5671 2021-10-09 11:15:29.000000 lnsync-0.8.5/lnsync_pkg/backtracker.py
--rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)    12585 2022-04-27 16:25:44.000000 lnsync-0.8.5/lnsync_pkg/hasher_functions.py
--rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     1707 2021-10-16 09:16:01.000000 lnsync-0.8.5/setup.py
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       17 2019-07-03 12:18:59.000000 lnsync-0.8.5/MANIFEST.in
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       38 2022-08-22 13:28:25.000000 lnsync-0.8.5/setup.cfg
--rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23039 2022-08-22 13:28:25.000000 lnsync-0.8.5/PKG-INFO
+drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2023-05-04 15:02:35.000000 lnsync-0.8.6/
+drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2023-05-04 15:02:35.000000 lnsync-0.8.6/lnsync.egg-info/
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       22 2023-05-04 15:02:30.000000 lnsync-0.8.6/lnsync.egg-info/top_level.txt
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     1054 2023-05-04 15:02:31.000000 lnsync-0.8.6/lnsync.egg-info/SOURCES.txt
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      175 2023-05-04 15:02:30.000000 lnsync-0.8.6/lnsync.egg-info/entry_points.txt
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       14 2023-05-04 15:02:30.000000 lnsync-0.8.6/lnsync.egg-info/requires.txt
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)        1 2023-05-04 15:02:30.000000 lnsync-0.8.6/lnsync.egg-info/dependency_links.txt
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23276 2023-05-04 15:02:30.000000 lnsync-0.8.6/lnsync.egg-info/PKG-INFO
+drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2023-05-04 15:02:35.000000 lnsync-0.8.6/random_pkg/
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    11641 2023-05-04 15:01:30.000000 lnsync-0.8.6/random_pkg/random_tree.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)        0 2019-07-03 12:20:35.000000 lnsync-0.8.6/random_pkg/__init__.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     2841 2020-12-17 13:26:58.000000 lnsync-0.8.6/random_pkg/random_extras.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    19795 2023-05-04 15:01:30.000000 lnsync-0.8.6/README.md
+drwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)        0 2023-05-04 15:02:35.000000 lnsync-0.8.6/lnsync_pkg/
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     3633 2022-05-23 07:31:25.000000 lnsync-0.8.6/lnsync_pkg/prefixdbname.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12799 2022-04-27 16:25:44.000000 lnsync-0.8.6/lnsync_pkg/lnsync_treeargs.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     7423 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/miscutils.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5120 2022-04-27 11:55:48.000000 lnsync-0.8.6/lnsync_pkg/thread_utils.py
+-rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)    37024 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/lnsync.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4191 2021-10-16 09:16:01.000000 lnsync-0.8.6/lnsync_pkg/human2bytes.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5144 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/groupedfileprinter.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    10442 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/glob_matcher.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     8450 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/printutils.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     5809 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/filesystems.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12468 2022-08-22 13:26:30.000000 lnsync-0.8.6/lnsync_pkg/fdupes.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     2066 2022-04-27 11:55:48.000000 lnsync-0.8.6/lnsync_pkg/lnsync_api.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4714 2022-08-22 13:26:30.000000 lnsync-0.8.6/lnsync_pkg/onegraph.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      665 2021-12-26 12:07:22.000000 lnsync-0.8.6/lnsync_pkg/propdbmanager.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     4638 2022-04-27 11:55:48.000000 lnsync-0.8.6/lnsync_pkg/filehashtree.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    26453 2022-04-27 11:55:48.000000 lnsync-0.8.6/lnsync_pkg/matcher.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     1544 2022-03-05 13:48:54.000000 lnsync-0.8.6/lnsync_pkg/gnome_thumbnailer.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      218 2021-02-05 11:57:06.000000 lnsync-0.8.6/lnsync_pkg/__init__.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    33562 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/filetree.py
+-rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     3265 2022-05-23 07:31:25.000000 lnsync-0.8.6/lnsync_pkg/image_dhash.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    12243 2022-02-02 18:11:16.000000 lnsync-0.8.6/lnsync_pkg/argparse_scoped.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)     8726 2021-10-16 09:16:01.000000 lnsync-0.8.6/lnsync_pkg/modaltype.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    24047 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/fileproptree.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    30659 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/lnsync_cmd_handlers.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23068 2022-04-01 12:18:52.000000 lnsync-0.8.6/lnsync_pkg/sqlpropdb.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)      798 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/metadata.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    20663 2022-08-22 13:26:30.000000 lnsync-0.8.6/lnsync_pkg/argparse_config.py
+-rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     5671 2021-10-09 11:15:29.000000 lnsync-0.8.6/lnsync_pkg/backtracker.py
+-rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)    13123 2023-05-04 15:01:30.000000 lnsync-0.8.6/lnsync_pkg/hasher_functions.py
+-rwxr-xr-x   0 mrsimoes  (1001) mrsimoes  (1001)     1707 2021-10-16 09:16:01.000000 lnsync-0.8.6/setup.py
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       17 2019-07-03 12:18:59.000000 lnsync-0.8.6/MANIFEST.in
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)       38 2023-05-04 15:02:35.000000 lnsync-0.8.6/setup.cfg
+-rw-r--r--   0 mrsimoes  (1001) mrsimoes  (1001)    23276 2023-05-04 15:02:35.000000 lnsync-0.8.6/PKG-INFO
```

### Comparing `lnsync-0.8.5/lnsync.egg-info/SOURCES.txt` & `lnsync-0.8.6/lnsync.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 lnsync.egg-info/top_level.txt
 lnsync_pkg/__init__.py
 lnsync_pkg/argparse_config.py
 lnsync_pkg/argparse_scoped.py
 lnsync_pkg/backtracker.py
 lnsync_pkg/fdupes.py
 lnsync_pkg/filehashtree.py
-lnsync_pkg/fileid.py
 lnsync_pkg/fileproptree.py
+lnsync_pkg/filesystems.py
 lnsync_pkg/filetree.py
 lnsync_pkg/glob_matcher.py
 lnsync_pkg/gnome_thumbnailer.py
 lnsync_pkg/groupedfileprinter.py
 lnsync_pkg/hasher_functions.py
 lnsync_pkg/human2bytes.py
 lnsync_pkg/image_dhash.py
```

### Comparing `lnsync-0.8.5/lnsync.egg-info/PKG-INFO` & `lnsync-0.8.6/lnsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: lnsync
-Version: 0.8.5
-Summary: Dir sync by content with rename detection, hard link support, plus fast fdupes, and more.
+Version: 0.8.6
+Summary: Sync local dirs by content, with rename detection and hard link support, plus fast fdupes, and more.
 Home-page: https://github.com/mrsimoes/lnsync
 Author: Miguel Simoes
 Author-email: miguelrsimoes@yahoo.com
 License: GNU General Public License v3
-Download-URL: https://github.com/mrsimoes/lnsync/archive/v0.8.5.tar.gz
-Description: ## Overview
-        _lnsync_ provides sync-by-content of local directories (including hard link syncing), plus other features related to matching and finding.
+Download-URL: https://github.com/mrsimoes/lnsync/archive/v0.8.6.tar.gz
+Description: # This package will be renamed to `hlnsync` starting with v0.9.0
+        
+        ## Overview
+        This tool provides sync-by-content of local directories, including hard links, plus other matching and searching features.
         
         ###  Features
-        The main feature is (partial) one-way sync of local directories by only renaming/linking/delinking on the target directory, without copying or deleting any file content from source. This may be used as a preprocessing step for a full sync tool (such as rsync).
+        The main feature is partial one-way sync of local directories without copying or deleting data, that is by only renaming/linking/delinking files in the target. This may be used as a perliminary step to a full sync using some other tool, such as rsync.
         
-        This is achieved by maintaining a simple one-file database of file hashes for each top directory.
+        For each file tree processed, a one-file database of file hashes is stored at its top directory.
         
-        Files match if they have the same size and hash value.
+        Using those file hashes, other features are provided, e.g. finding duplicate files, checking for file content changes, and listing all hard links to a file.
         
-        Using file hashes, other features are provided, including: finding duplicate files, checking for file content changes, and listing all hard links to a file.
+        Multiple hashing functions are provided, including dhash, an image hash that is invariant under scaling and recoloring. This allows finding duplicate images.
         
-        Other hashing functions are provided, including dhash, an image invariant under scaling and recoloring. This allows finding duplicate images.
+        Files match if they have the same size and hash. Modification time and permissions are ignored.
         
         ### File Trees: Online and Offline
         
-        The file structure under a directory (path names, file sizes, mod dates) can be saved to a one-file database, along with the file hashes. Such a database is termed here an _offline tree_, whereas local top directories with their hash database are _online trees_,
-        
-        Most _lnsync_ commands accept offline trees as well as local directory. For example, an offline tree may be used as the source to reorganize a target directory according to a certain pattern.
+        The structure of a file tree -- path names, file sizes, mod dates --  may be stored in a one-file database, along with the file hashes.
         
-        Via a config file, specific options may be applied to online trees matching a glob pattern.
+        Such a database file is an _offline tree_, while the top directory of a file tree with their hash database is an _online trees_. (Note: the database file of an online tree is NOT in itself an offline tree, since it does not include the tree directory structure, file names, etc.)
         
-        To describe a tree: `lnsync info <LOCATION>`.
+        Most _lnsync_ commands both offline and online trees. For example, an offline tree database may be used as a pattern to reorganize a target directory.
         
-        Note that the database file of an online tree is NOT an offline tree, since it is missing the file and directory names.
+        Using a config file, specific options may be applied to online trees matching glob patterns.
         
         ### File Hashes
+        
         Files are identified by their content hash, using either 32-bit or 64-bit xxHash (a fast, non-cryptographic hash function), or other functions (see Hashing Functions below).
         
         Hash values are stored in local databases, on a single file per tree, by default with a name matching `lnsync-[0-9]+.db`. Only one such file should exist at each location. At the time of creation, the numeric part is chosen randomly, to avoid overwriting by accident when doing a full sync. Files matching `lnsync-[0-9]+.db` as well as the hash database in use are ignored by _lnsync_ operations.
         
         File modification times are used to detect stale hash values. Modification times are not synced to the target.
         
         ### Hashing Functions
@@ -67,14 +68,15 @@
         Files which cannot be read are skipped. File ownership and permissions are otherwise ignored.
         
         Symbolic links and any other file system objects are ignored.
         
         As with rsync, files and directories may be included/excluded using glob patterns.
         
         ### Directories
+        
         When syncing, directories are created as needed on the target, and target directories left empty and not on the source are removed.
         
         ## Installing
         Install the latest version from the PyPI repository with `pip install --user -U lnsync` or else clone the repo with `git clone https://github.com/mrsimoes/lnsync.git` and then run `python setup.py install`.
         
         ### Alternative Tools for Linux
         Some of the many tools for syncing with rename detection:
@@ -88,15 +90,17 @@
         - _git_ itself identifies and stores files by content, and has been adapted for syncing.
         
         - Support in modern file systems (e.g. btrfs) for snapshots may be adapted for syncing.
         
         In addition to syncing, _lnsync_ allows using the file hash database to search for files according to a variety of criteria.
         
         ## Usage Scenarios
+        
         ### Syncing
+        
         If your photos are at `/home/you/Photos` and its backup is at `/mnt/disk/Photos`, then `lnsync sync /home/you/Photos /mnt/disk/Photos` will sync the target. For a dry run, use the `-n` switch.
         
         After syncing, two database files are created, one at the source `/home/you/Photos` and another at the target `/mnt/disk/Photos`. File hashes are computed, as needed, and stored in those files. The database filenames include a random suffix, to help avoid accidental overwriting when syncing with a tool other than _lsync_.
         
         To obtain an _rsync_ command that will complete syncing, skipping `lnsync` database files, run `lnsync rsync /home/you/Photos /mnt/disk/Photos`. If the `rsync` options provided are suitable, run the command again with the `-x` switch to execute. Alternatively, run `lnsync syncr /home/you/Photos /mnt/disk/Photos` to complete those two steps in one go.
         
         Finally, to compare source and target, run `lnsync cmp /home/you/Photos /mnt/disk/Photos`.
@@ -256,14 +260,15 @@
         
         - Only readable files and readable+accessible directories are read. Other files and dirs, as well as symlinks, pipes, special devices are ignored.
         
         - Minimal support for case-insensitive but case-preserving file systems like vfat: if a target file name differs from source match in case only, target is not updated.
         
         ### Release Notes
         
+        - v0.8.6: Show size in search command results. Add BasenameHasher. Drop dependency on psutil, use lsblk. Bug fixes. Improve documentation.
         - v0.8.5: New `onmorethanone` search command. Small fixes.
         - v0.8.4: Performance improvements on find commamnds. Bug fixes. Allow multiple arguments to `--dbrootmount`.
         - v0.8.3: Performance improvements and bug fixes.
         - v0.8.2: New --show-size and --min-size options. Much faster searches in offline database. Bug fixes.
         - v0.8.1: Implement onfirstnotonly for all hash functions.
         - v0.8.0: Rename hasher options. Rename main config section. New built-in hash functions: dhash and thumbnail_dhash. Bug fixes.
         - v0.7.6: New `onfirstnotonly` search command. Allow mkoffline to operate on non-writeable dirs. Fixed regressions: incomplete reading of config file options, mishandling of single quotes in offline location databases.
```

### Comparing `lnsync-0.8.5/random_pkg/random_tree.py` & `lnsync-0.8.6/random_pkg/random_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         abs_filepath = os.path.join(absdir, bname)
         relpath = os.path.join(reldir, bname)
         with open(abs_filepath, "w") as f:
             f.write(contents)
         st = os.stat(abs_filepath)
         fid = self._id_computer.get_id(relpath)
         f_obj = self._new_file_obj(fid, st)
-        self._add_path(f_obj, reldir_obj, bname)
+        self.add_path(f_obj, reldir_obj, bname)
 
     def exec_cmd(self, cmd):
         """
         Execute a file command (cmdname, path_from, path_to).
         Add cp and rm final path to FileTree.
         """
         if cmd[0] == "cp":
@@ -111,30 +111,31 @@
             fn_from, fn_to = cmd[1:]
             fn_abs_from = self.rel_to_abs(fn_from)
             fn_abs_to = self.rel_to_abs(fn_to)
             shutil.copy2(fn_abs_from, fn_abs_to)
             st = os.stat(fn_abs_to)
             fid = self._id_computer.get_id(fn_to)
             new_f_obj = self._new_file_obj(fid, st)
-            tr_obj = self._create_dir_if_needed_writeback(os.path.dirname(fn_to))
-            self._add_path(new_f_obj, tr_obj, os.path.basename(fn_to))
+            tr_obj = self._create_dir_if_needed_writeback(
+                os.path.dirname(fn_to))
+            self.add_path(new_f_obj, tr_obj, os.path.basename(fn_to))
         elif cmd[0] == "rm" and cmd[2] is None:
             assert self.writeback, "cannot rm file without writeback"
             dirname = os.path.dirname(cmd[1])
             bname = os.path.basename(cmd[1])
             d_obj = self.path_to_obj(dirname)
             assert d_obj is not None
             f_obj = d_obj.get_entry(bname)
             assert f_obj is not None
             assert f_obj.relpaths == [cmd[1]]
             abs_filepath = self.rel_to_abs(cmd[1])
             with open(abs_filepath, "r") as f:
                 contents = f.read()
             self._files_removed[cmd[1]] = contents
-            self._rm_path(f_obj, d_obj, bname)
+            self.rm_path(f_obj, d_obj, bname)
             os.unlink(abs_filepath)
         else:
             super(FileTreeCreator, self).exec_cmd(cmd)
 
     def exec_cmd_reverse(self, cmd):
         """
         Undo a file command (cmdname, path_from, path_to).
```

### Comparing `lnsync-0.8.5/random_pkg/random_extras.py` & `lnsync-0.8.6/random_pkg/random_extras.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/README.md` & `lnsync-0.8.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+# This package will be renamed to `hlnsync` starting with v0.9.0
+
 ## Overview
-_lnsync_ provides sync-by-content of local directories (including hard link syncing), plus other features related to matching and finding.
+This tool provides sync-by-content of local directories, including hard links, plus other matching and searching features.
 
 ###  Features
-The main feature is (partial) one-way sync of local directories by only renaming/linking/delinking on the target directory, without copying or deleting any file content from source. This may be used as a preprocessing step for a full sync tool (such as rsync).
+The main feature is partial one-way sync of local directories without copying or deleting data, that is by only renaming/linking/delinking files in the target. This may be used as a perliminary step to a full sync using some other tool, such as rsync.
 
-This is achieved by maintaining a simple one-file database of file hashes for each top directory.
+For each file tree processed, a one-file database of file hashes is stored at its top directory.
 
-Files match if they have the same size and hash value.
+Using those file hashes, other features are provided, e.g. finding duplicate files, checking for file content changes, and listing all hard links to a file.
 
-Using file hashes, other features are provided, including: finding duplicate files, checking for file content changes, and listing all hard links to a file.
+Multiple hashing functions are provided, including dhash, an image hash that is invariant under scaling and recoloring. This allows finding duplicate images.
 
-Other hashing functions are provided, including dhash, an image invariant under scaling and recoloring. This allows finding duplicate images.
+Files match if they have the same size and hash. Modification time and permissions are ignored.
 
 ### File Trees: Online and Offline
 
-The file structure under a directory (path names, file sizes, mod dates) can be saved to a one-file database, along with the file hashes. Such a database is termed here an _offline tree_, whereas local top directories with their hash database are _online trees_,
-
-Most _lnsync_ commands accept offline trees as well as local directory. For example, an offline tree may be used as the source to reorganize a target directory according to a certain pattern.
+The structure of a file tree -- path names, file sizes, mod dates --  may be stored in a one-file database, along with the file hashes.
 
-Via a config file, specific options may be applied to online trees matching a glob pattern.
+Such a database file is an _offline tree_, while the top directory of a file tree with their hash database is an _online trees_. (Note: the database file of an online tree is NOT in itself an offline tree, since it does not include the tree directory structure, file names, etc.)
 
-To describe a tree: `lnsync info <LOCATION>`.
+Most _lnsync_ commands both offline and online trees. For example, an offline tree database may be used as a pattern to reorganize a target directory.
 
-Note that the database file of an online tree is NOT an offline tree, since it is missing the file and directory names.
+Using a config file, specific options may be applied to online trees matching glob patterns.
 
 ### File Hashes
+
 Files are identified by their content hash, using either 32-bit or 64-bit xxHash (a fast, non-cryptographic hash function), or other functions (see Hashing Functions below).
 
 Hash values are stored in local databases, on a single file per tree, by default with a name matching `lnsync-[0-9]+.db`. Only one such file should exist at each location. At the time of creation, the numeric part is chosen randomly, to avoid overwriting by accident when doing a full sync. Files matching `lnsync-[0-9]+.db` as well as the hash database in use are ignored by _lnsync_ operations.
 
 File modification times are used to detect stale hash values. Modification times are not synced to the target.
 
 ### Hashing Functions
@@ -58,14 +59,15 @@
 Files which cannot be read are skipped. File ownership and permissions are otherwise ignored.
 
 Symbolic links and any other file system objects are ignored.
 
 As with rsync, files and directories may be included/excluded using glob patterns.
 
 ### Directories
+
 When syncing, directories are created as needed on the target, and target directories left empty and not on the source are removed.
 
 ## Installing
 Install the latest version from the PyPI repository with `pip install --user -U lnsync` or else clone the repo with `git clone https://github.com/mrsimoes/lnsync.git` and then run `python setup.py install`.
 
 ### Alternative Tools for Linux
 Some of the many tools for syncing with rename detection:
@@ -79,15 +81,17 @@
 - _git_ itself identifies and stores files by content, and has been adapted for syncing.
 
 - Support in modern file systems (e.g. btrfs) for snapshots may be adapted for syncing.
 
 In addition to syncing, _lnsync_ allows using the file hash database to search for files according to a variety of criteria.
 
 ## Usage Scenarios
+
 ### Syncing
+
 If your photos are at `/home/you/Photos` and its backup is at `/mnt/disk/Photos`, then `lnsync sync /home/you/Photos /mnt/disk/Photos` will sync the target. For a dry run, use the `-n` switch.
 
 After syncing, two database files are created, one at the source `/home/you/Photos` and another at the target `/mnt/disk/Photos`. File hashes are computed, as needed, and stored in those files. The database filenames include a random suffix, to help avoid accidental overwriting when syncing with a tool other than _lsync_.
 
 To obtain an _rsync_ command that will complete syncing, skipping `lnsync` database files, run `lnsync rsync /home/you/Photos /mnt/disk/Photos`. If the `rsync` options provided are suitable, run the command again with the `-x` switch to execute. Alternatively, run `lnsync syncr /home/you/Photos /mnt/disk/Photos` to complete those two steps in one go.
 
 Finally, to compare source and target, run `lnsync cmp /home/you/Photos /mnt/disk/Photos`.
@@ -247,14 +251,15 @@
 
 - Only readable files and readable+accessible directories are read. Other files and dirs, as well as symlinks, pipes, special devices are ignored.
 
 - Minimal support for case-insensitive but case-preserving file systems like vfat: if a target file name differs from source match in case only, target is not updated.
 
 ### Release Notes
 
+- v0.8.6: Show size in search command results. Add BasenameHasher. Drop dependency on psutil, use lsblk. Bug fixes. Improve documentation.
 - v0.8.5: New `onmorethanone` search command. Small fixes.
 - v0.8.4: Performance improvements on find commamnds. Bug fixes. Allow multiple arguments to `--dbrootmount`.
 - v0.8.3: Performance improvements and bug fixes.
 - v0.8.2: New --show-size and --min-size options. Much faster searches in offline database. Bug fixes.
 - v0.8.1: Implement onfirstnotonly for all hash functions.
 - v0.8.0: Rename hasher options. Rename main config section. New built-in hash functions: dhash and thumbnail_dhash. Bug fixes.
 - v0.7.6: New `onfirstnotonly` search command. Allow mkoffline to operate on non-writeable dirs. Fixed regressions: incomplete reading of config file options, mishandling of single quotes in offline location databases.
```

### Comparing `lnsync-0.8.5/lnsync_pkg/prefixdbname.py` & `lnsync-0.8.6/lnsync_pkg/prefixdbname.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/lnsync_treeargs.py` & `lnsync-0.8.6/lnsync_pkg/lnsync_treeargs.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/fileid.py` & `lnsync-0.8.6/lnsync_pkg/filesystems.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,59 +21,80 @@
 (i.e. hard links).
 
 On a POSIX-compliant file system, this is the inode.
 (https://en.wikipedia.org/wiki/Inode#POSIX_inode_description)
 
 On FAT/VFAT: use hash of dirname + int(ctime) + small integer to ensure
 uniqueness.
+
+Possible implementations:
+    - Use disk_partitions from psutils, but this shows all fuse systems as fuseblk.
+    - call "lsblk -fJ -e 7" (exclude loopback devices) and parse the json output
+
 """
 
 import sys
 import os
 import abc
-
-from psutil import disk_partitions
+import subprocess
+import json
 
 import lnsync_pkg.printutils as pr
 from lnsync_pkg.hasher_functions import FileHasherXXHASH64
 from lnsync_pkg.miscutils import MIN_INT64, MAX_INT64
 
 FSE = sys.getfilesystemencoding() # Always UTF8 on Linux.
 
+_mntpoint_to_fstype = {}
+
+def _read_partitions():
+    global _mntpoint_to_fstype
+
+    def store_partition_info(obj):
+        mtpoint = obj["mountpoint"]
+        if mtpoint:
+            _mntpoint_to_fstype[mtpoint] = obj["fstype"]
+
+    try:
+        res = subprocess.run(["lsblk", "-fJ", "-e", "7"] , capture_output=True, check=True)
+    except CalledProcessError as exc:
+        raise RuntimeError("lsblk not installed or outdated")
+
+    dic = json.loads(res.stdout)
+    for blkdev in dic["blockdevices"]:
+        store_partition_info(blkdev)
+        for blkdev_part in blkdev["children"]:
+            store_partition_info(blkdev_part)
+
+
 def get_mountpt_and_fstype(path):
-    """
-    Return file_system for a path.
-    """
-    path = os.path.realpath(path)
-    mntpoint_to_fstype = {}
-    for part in disk_partitions():
-        mntpoint_to_fstype[part.mountpoint] = part.fstype
     while True:
-        if path in mntpoint_to_fstype:
-            return path, mntpoint_to_fstype[path]
+        if path in _mntpoint_to_fstype:
+            return path, _mntpoint_to_fstype[path]
         if path == os.sep:
             raise RuntimeError(f"could not find mountpoint for: {path}")
         path = os.path.dirname(path)
 
+
 SYSTEMS_W_INODE = ['ext2', 'ext3', 'ext4', 'ecryptfs',
-                   'btrfs', 'ntfs', 'fuse.encfs', 'fuseblk']
-SYSTEMS_WO_INODE = ['vfat', 'fat', 'FAT', 'iso9660']
+                   'btrfs', 'ntfs', 'fuse.encfs']
+SYSTEMS_WO_INODE = ['vfat', 'fat', 'FAT', 'iso9660', 'exfat']
 
 for fs_list in SYSTEMS_W_INODE, SYSTEMS_WO_INODE:
     fs_list.extend([s.swapcase() for s in fs_list])
 
 def make_id_computer(topdir_path):
     """
     Return an instance of the appropriate IDComputer class.
     """
     mtpoint, fstype = get_mountpt_and_fstype(topdir_path)
     if fstype in SYSTEMS_W_INODE:
         return InodeIDComputer(topdir_path, fstype)
     elif fstype in SYSTEMS_WO_INODE:
-        pr.warning(f"using path hash as file id for: {topdir_path}")
+        pr.warning(f"found {fstype}, using path hash as file id for: {topdir_path}")
         return HashPathIDComputer(topdir_path, fstype, mtpoint)
     else:
         raise NotImplementedError(
             f"IDComputer: not implemented for file system: {fstype}")
 
 class IDComputer:
     """
@@ -137,7 +158,9 @@
         while file_id in self._hash_plus_size_uniq:
             if self._hash_plus_size_uniq[file_id] == rel_path_to_mt:
                 return file_id
             else:
                 file_id += 1
         self._hash_plus_size_uniq[file_id] = rel_path_to_mt
         return file_id
+
+_read_partitions()
```

### Comparing `lnsync-0.8.5/lnsync_pkg/miscutils.py` & `lnsync-0.8.6/lnsync_pkg/miscutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,27 @@
         res = value
     else:
         res = MAX_INT32 - value
     assert 0 <= res <= MAX_UINT32, \
         f"int32_to_uint32 overflow: {value}"
     return res
 
+def argmin(seq, key=None):
+    if not seq:
+        raise ValueError("attempt to get argmin of an empty sequence")
+    if key is None:
+        key = lambda x: x
+    minval = key(seq[0])
+    argmin_res = 0
+    for ind, item in enumerate(seq[1:]):
+        val = key(item)
+        if val < minval:
+            minval = val
+            argmin_res = ind
+    return argmin_res
 
 def iter_is_empty(iterator):
     """
     Check if iterator is empty, consuming one element to test.
     """
     try:
         next(iterator)
```

### Comparing `lnsync-0.8.5/lnsync_pkg/thread_utils.py` & `lnsync-0.8.6/lnsync_pkg/thread_utils.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/lnsync.py` & `lnsync-0.8.6/lnsync_pkg/lnsync.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,31 +101,27 @@
     ArgumentParserConfig.set_optionals_section(LNSYNC_CONFIG_MAIN_SECTION)
     ArgumentParserConfig.set_default_config_files(
         "./lnsync.cfg",
         os.path.expanduser("~/lnsync.cfg"))
 except NoValidConfigFile:
     pass
 
-####################
-# Argument parsing
-####################
+## Argument parsing
 
 # Utilities.
 
 def relative_path_type(value):
     """
     Argument type function: accept relative paths, exclude absolute paths.
     """
     if os.path.isabs(value):
         raise argparse.ArgumentTypeError("not a relative path: %s." % value)
     return value
 
-####################
-# Top-level parsers
-####################
+## Top-level parsers
 
 # Verbosity control.
 
 class SetVerbosityAction(argparse.Action):
     """
     Adjust verbosity level of print module up and down.
     """
@@ -209,17 +205,15 @@
 debugtrees_option_parser = argparse.ArgumentParser(add_help=False)
 debugtrees_option_parser.add_argument(
     "--debugtrees", action="store_true",
     dest="debugtrees", default=False,
     help=argparse.SUPPRESS)
 
 
-####################
-# Options applying to all tree arguments.
-####################
+## Options applying to all tree arguments.
 
 # Many optional arguments are shared by multiple command parsers.
 # To factor out these arguments, define as many single-argument parsers:
 
 def human2bytes_or_none(value):
     if value is None:
         return None
@@ -272,21 +266,17 @@
 
 hard_links_option_parser.add_argument(
     "-A", "--all-links", "--no-all-links",
     action=ConfigTreeOptionAction, sc_scope=Scope.ALL, sc_action="store_bool",
     default=True,
     help="on results, print all hard links, not just one")
 
-####################
-# Options applying to one or more tree args.
-####################
-
-##########
-# Database file location options
-##########
+## Options applying to one or more tree args.
+
+## Database file location options
 
 dblocation_option_parser = argparse.ArgumentParser(add_help=False)
 
 class DBPrefixTreeOption(ConfigTreeOptionAction):
     def sc_action(self, _parser, _namespace,
                   pos_val, opt_val, _option_string=None):
         pos_val.set_dbprefix(opt_val)
@@ -312,17 +302,15 @@
         pos_val.set_dblocation(opt_val)
 
 dblocation_option_parser.add_argument(
     "-b", "--dblocation", metavar="DBLOCATION", type=str,
     action=DBLocationTreeOption, sc_scope=Scope.NEXT,
     help="database file location for following online tree")
 
-##########
-# Include/exclude pattern options.
-##########
+## Include/exclude pattern options.
 
 class IncExcPatternOptionBase(ConfigTreeOptionAction):
     """
     Common to all include/exclude option Actions.
     """
     def make_pattern_obj_list(self, pattern_strings, option_string):
         """
@@ -412,17 +400,15 @@
     parents=[exclude_option_parser,
              excludeonce_option_parser,
              includeonly_option_parser,
              includeonlyonce_option_parser,
             ],
     )
 
-##########
-# dbrootdir options.
-##########
+## dbrootdir options.
 
 # Specify directories where the hash database actually is.
 
 dbrootdir_option_parser = argparse.ArgumentParser(add_help=False)
 
 def readable_dir(path):
     if not os.path.exists(path) or not os.path.isdir(path):
@@ -478,30 +464,26 @@
     "--dbrootmount", metavar="DBROOTS_MOUNTS_LOCATION",
     type=readable_dir,
     action=DBRootMountLocationOption, sc_scope=Scope.ALL,
     nargs="+",
     help="set directory whose immediate subdirs will be database directories " \
     "for online trees contained within")
 
-####################
-# Other shared options parsers, unrelated to trees.
-####################
+## Other shared options parsers, unrelated to trees.
 
 # Dry-run.
 
 dryrun_option_parser = argparse.ArgumentParser(add_help=False)
 
 dryrun_option_parser.add_argument(
     "-n", "--dry-run", "--no-dry-run",
     action=StoreBoolAction, dest="dry_run", default=False,
     help="dry run")
 
-####################
-# Output formatting options.
-####################
+## Output formatting options.
 
 class SetOutputOptionAction(StoreBoolAction):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         setattr(GroupedFileListPrinter, self.dest, self.default)
 
     def __call__(self, parser, namespace, values, option_string=None):
@@ -524,17 +506,15 @@
 
 showsize_option_parser = argparse.ArgumentParser(add_help=False)
 showsize_option_parser.add_argument(
     "--show-size", "--no-show-size",
     action=SetOutputOptionAction, dest="showsize", default=False,
     help="show size of each file")
 
-####################
-# Top parser and subcommand parsers and handlers.
-####################
+## Top parser and subcommand parsers and handlers.
 
 class CustomArgumentParserConfig(ArgumentParserConfig):
     """
     Register handlers for each main command parser.
     Raise exception on parsing error.
     """
     def __init__(self, *args, **kwargs):
@@ -567,17 +547,15 @@
     formatter_class=FormatLateDescription,
     parents=[verbosity_options_parser,
              builtin_hasher_option_parser,
              external_hasher_option_parser, # TODO filter_option_parser
              debugtrees_option_parser],
     add_help=False, usage=argparse.SUPPRESS,)
 
-##########
-# sync
-##########
+## sync
 
 parser_sync = top_parser.add_parser_command(
     'sync', lnsync_cmd_handlers.do_sync,
     parents=[dryrun_option_parser, exclude_option_parser,
              maxminsize_option_parser,
              bysize_option_parser, skipempty_option_parser,
              dbrootdir_option_parser, dblocation_option_parser],
@@ -586,17 +564,15 @@
 
 parser_sync.add_argument(
     "source", type=TreeLocation, action=TreeLocationAction)
 
 parser_sync.add_argument(
     "target", type=TreeLocationOnline, action=TreeLocationAction)
 
-##########
-# rsync
-##########
+## rsync
 
 parser_rsync = top_parser.add_parser_command(
     'rsync', lnsync_cmd_handlers.do_rsync,
     extra_args_cmd=True,
     parents=[dryrun_option_parser, exclude_option_parser,
              hard_links_option_parser,
              maxminsize_option_parser, skipempty_option_parser,
@@ -640,17 +616,15 @@
 parser_syncr.add_argument(
     "target", type=TreeLocationOnline, action=TreeLocationAction)
 
 parser_syncr.add_argument(
     "--cmp", default=False, action="store_true",
     help="compare source and target after rsync")
 
-##########
-# Search commands
-##########
+## Search commands
 
 _SEARCH_CMD_PARENTS = \
     [exclude_all_options_parser,
      hard_links_option_parser, bysize_option_parser,
      maxminsize_option_parser, skipempty_option_parser,
      sameline_option_parser, sort_option_parser, showsize_option_parser,
      dbrootdir_option_parser, dblocation_option_parser,
@@ -735,17 +709,15 @@
 
 parser_search.add_argument(
     "locations", type=TreeLocation, action=TreeLocationAction, nargs="+")
 
 parser_search.add_argument(
     "--glob", type=Pattern, action="store", default=None)
 
-##########
-# update
-##########
+## update
 
 def do_update(args):
     with FileHashTree.listof(d.kws() for d in args.dirs) as trees:
         for tree in trees:
             tree.db_update_all()
 
 parser_update = top_parser.add_parser_command(
@@ -754,66 +726,58 @@
              skipempty_option_parser, maxminsize_option_parser,
              dbrootdir_option_parser, dblocation_option_parser],
     help='update hashes for new and modified files')
 
 parser_update.add_argument(
     "dirs", type=TreeLocationOnline, action=TreeLocationAction, nargs="+")
 
-##########
-# rehash
-##########
+## rehash
 
 def do_rehash(args):
     return lnsync_cmd_handlers.do_rehash(args.topdir, args.relpath_patterns)
 
 parser_rehash = top_parser.add_parser_command(
     'rehash', do_rehash,
     parents=[dbrootdir_option_parser, dblocation_option_parser],
     help='force hash updates for given files')
 
 parser_rehash.add_argument("topdir",
                            type=TreeLocationOnline, action=TreeLocationAction)
 
 parser_rehash.add_argument("relpath_patterns", type=relative_path_type, nargs='+')
 
-##########
-# lookup
-##########
+## lookup
 
 parser_lookup = top_parser.add_parser_command(
         'lookup', lnsync_cmd_handlers.do_lookup,
         parents=[dbrootdir_option_parser,
                  dblocation_option_parser,
                  ],
         help='retrieve file hashes')
 
 parser_lookup.add_argument("location",
                            type=TreeLocation, action=TreeLocationAction)
 
 parser_lookup.add_argument("relpaths", type=relative_path_type, nargs="*")
 
-##########
-# aliases
-##########
+## aliases
 
 parser_aliases = top_parser.add_parser_command(
         'aliases', lnsync_cmd_handlers.do_aliases,
         parents=[dbrootdir_option_parser,
                  dblocation_option_parser,
                 ],
         help='find all hard links to a file')
 
 parser_aliases.add_argument("location",
                             type=TreeLocation, action=TreeLocationAction)
 
 parser_aliases.add_argument("relpath", type=relative_path_type)
 
-##########
-# cmp
-##########
+## cmp
 
 parser_cmp = top_parser.add_parser_command(
     'cmp', lnsync_cmd_handlers.do_cmp,
     parents=[exclude_all_options_parser,
              hard_links_option_parser, bysize_option_parser,
              maxminsize_option_parser, skipempty_option_parser,
              dbrootdir_option_parser, dblocation_option_parser,
@@ -822,17 +786,15 @@
 
 parser_cmp.add_argument(
     "leftlocation", type=TreeLocation, action=TreeLocationAction)
 
 parser_cmp.add_argument(
     "rightlocation", type=TreeLocation, action=TreeLocationAction)
 
-##########
-# check
-##########
+## check
 
 parser_check_files = top_parser.add_parser_command(
     'check', lnsync_cmd_handlers.do_check,
     parents=[exclude_all_options_parser,
              hard_links_option_parser,
              maxminsize_option_parser, skipempty_option_parser,
              dbrootdir_option_parser, dblocation_option_parser,
@@ -843,17 +805,15 @@
     "location", metavar="ROOT_DIRECTORY",
     type=TreeLocationOnline, action=TreeLocationAction)
 
 parser_check_files.add_argument(
     "relpaths", metavar="RELATIVE_PATHS",
     type=relative_path_type, nargs="*")
 
-##########
-# info
-##########
+## info
 
 def do_get_info(args):
     for tree_arg in args.locations:
         with FileHashTree(**tree_arg.kws()) as tree:
             if tree.mode == Mode.ONLINE:
                 pr.print(f"[ONLINE]: {tree_arg.real_location}")
                 pr.print(f"Using database at: {tree.db.dbpath}")
@@ -878,17 +838,15 @@
     help='describe the given locations')
 
 parser_get_info.add_argument(
     "locations", metavar="LOCATION",
     type=TreeLocation, action=TreeLocationAction,
     nargs="*")
 
-##########
-# subdir
-##########
+## subdir
 
 parser_subdir = top_parser.add_parser_command(
         'subdir', lnsync_cmd_handlers.do_subdir,
         parents=[dblocation_option_parser,
                 ],
         help='copy hashes to new database at relative subdir')
 
@@ -896,17 +854,15 @@
     "topdir",
     type=TreeLocationOnline, action=TreeLocationAction)
 
 parser_subdir.add_argument(
     "relativesubdir",
     type=relative_path_type)
 
-##########
-# mkoffline
-##########
+## mkoffline
 
 def writable_file_or_empty_path(path):
     if not os.path.exists(path):
         try:
             f = open(path, 'w')
         except OSError as exc:
             msg = "cannot write to %s" % (path,)
@@ -938,30 +894,26 @@
 parser_mkoffline.add_argument(
     "sourcedir", type=TreeLocationOnline, action=TreeLocationAction)
 
 parser_mkoffline.add_argument(
     "-o", "--outputpath", type=writable_file_or_empty_path, default=None,
     required=True)
 
-##########
 ## cleandb
-##########
 
 parser_cleandb = top_parser.add_parser_command(
         'cleandb', lnsync_cmd_handlers.do_cleandb,
         parents=[dblocation_option_parser,
                 ],
         help="purge old entries and compact the hash database at dir")
 
 parser_cleandb.add_argument(
     "location", type=TreeLocationOnline, action=TreeLocationAction)
 
-####################
-# main
-####################
+## main
 
 def debug_tree_info(args):
     xargs = vars(args)
     def excstr(tr):
         if not hasattr(tr, "dbprefix"):
             tr.kws = "No kws, path=" + tr.real_location
         elif callable(tr.kws):
```

### Comparing `lnsync-0.8.5/lnsync_pkg/human2bytes.py` & `lnsync-0.8.6/lnsync_pkg/human2bytes.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/groupedfileprinter.py` & `lnsync-0.8.6/lnsync_pkg/groupedfileprinter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 Files in each group are either presented one per line, separated by empty lines,
 or concatenated on a single line.
 """
 
 import lnsync_pkg.printutils as pr
 from lnsync_pkg.human2bytes import bytes2human
 
+
 class GroupedFileListPrinter:
     """
     Output filepaths in groups, either separated by empty lines or by empty
     spaces, sorted or not.
     """
     # Clients may set these global options in the class.
     sameline = False
@@ -56,15 +57,15 @@
             self.groups = []
         self._output_group_linebreak = False # Not before first group.
         if self.sameline:
             self._built_line = None
 
     def add_group(self, located_files):
         """
-        located files is {tree_1: [files_1],... {tree_k, [files_k]}
+        located files is {tree_1: [files_1, ...], ... , tree_k: [files_k, ...]}
         """
         if self.sort:
             self.groups.append(located_files)
         else:
             self._print_group(located_files)
 
     def flush(self):
@@ -95,15 +96,15 @@
                 self._print_file(tree, fobj)
         if self.sameline:
             pr.print(self._built_line)
 
     def _print_file(self, tree, fobj):
         if self.showsize:
             size = fobj.file_metadata.size
-            size_str = f"{bytes2human(size)}"
+            size_str = f"{bytes2human(size)} "
         else:
             size_str = ""
         if self.sameline:
             if self._built_line != "":
                 self._built_line += " "
             else:
                 self._built_line = size_str + " "
@@ -119,17 +120,17 @@
                     # Escape a few choice characters.
                     for char in ("\\", " ", "'", '"', "(", ")"):
                         pr_path = pr_path.replace(char, "\\"+char)
                     self._built_line += prefix + pr_path
         else:
             for k, relpath in enumerate(fobj.relpaths):
                 if k == 0:
-                    include, prefix = (True, size_str + " ")
+                    include, prefix = (True, size_str)
                 elif not self.hard_links:
-                    include, prefix = (True, size_str + " ")
+                    include, prefix = (True, size_str)
                 elif self.all_links:
                     include, prefix = (True, " ")
                 else:
                     include = False
                 if include:
                     pr_path = tree.printable_path(relpath)
                     pr.print(prefix + pr_path, end="\n")
```

### Comparing `lnsync-0.8.5/lnsync_pkg/glob_matcher.py` & `lnsync-0.8.6/lnsync_pkg/glob_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,16 +280,22 @@
                 (prnt_pats(l1), prnt_pats(l2)))
         elif e1 in l2:
             return [e2, *merge_lists(l1, l2[1:])]
         elif e2 in l1:
             return [e1, *merge_lists(l1[1:], l2)]
         else:
             return [e1, e2, *merge_lists(l1[1:], l2[1:])]
+    if pats1 == pats2:
+        return list(pats1)
     common_pats = merge_lists(list(pats1), list(pats2))
-    if common_pats != pats1 or common_pats != pats1:
+    if common_pats != pats1 and common_pats != pats2:
+        # If the merge result is different from both
+        # inputs, issue a message to the user.
+        # Merging all includes or all excludes produces
+        # only a info message, otherwise a warning.
         if any(all(all(getattr(p, f)() for p in pset)
                    for pset in (pats1, pats2))
                for f in ("is_include", "is_exclude")):
             outf = pr.info
         else:
             outf = pr.warning
         outf("merged rules [%s] and [%s] to [%s]" % \
```

### Comparing `lnsync-0.8.5/lnsync_pkg/printutils.py` & `lnsync-0.8.6/lnsync_pkg/printutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 import threading
 
 FSE = sys.getfilesystemencoding() # Always UTF8 on Linux.
 
 # Make printing sequences of terminal ctrl codes thread-safe.
 PRINT_LOCK = threading.RLock()
 
-FATAL_LEVEL = -2
-ERROR_LEVEL = -1
-WARNING_LEVEL = 0
+FATAL_LEVEL = -3
+ERROR_LEVEL = -2
+WARNING_LEVEL = -1
 PRINT_LEVEL = 0
 INFO_LEVEL = 1
 DEBUG_LEVEL = 2
 TRACE_LEVEL = 3
 PROGRESS_LEVEL = 0
 
 # Tell pylint not to mistake module variables for constants
```

### Comparing `lnsync-0.8.5/lnsync_pkg/fdupes.py` & `lnsync-0.8.6/lnsync_pkg/fdupes.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/lnsync_api.py` & `lnsync-0.8.6/lnsync_pkg/lnsync_api.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/onegraph.py` & `lnsync-0.8.6/lnsync_pkg/onegraph.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/propdbmanager.py` & `lnsync-0.8.6/lnsync_pkg/propdbmanager.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/filehashtree.py` & `lnsync-0.8.6/lnsync_pkg/filehashtree.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/matcher.py` & `lnsync-0.8.6/lnsync_pkg/matcher.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/gnome_thumbnailer.py` & `lnsync-0.8.6/lnsync_pkg/gnome_thumbnailer.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/filetree.py` & `lnsync-0.8.6/lnsync_pkg/filetree.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 """
 
 # pylint: disable=too-many-public-methods, too-many-instance-attributes
 
 import os
 
 import lnsync_pkg.printutils as pr
-from lnsync_pkg.fileid import make_id_computer
+from lnsync_pkg.filesystems import make_id_computer
 from lnsync_pkg.glob_matcher import GlobMatcher
 
 class TreeError(Exception):
     def __init__(self, msg, tree=None, file_obj=None, pprint=str):
         super().__init__(msg)
         self.tree = tree
         self.file_obj = file_obj
@@ -197,19 +197,26 @@
     def __str__(self):
         return "md[%d;%d;%d]" % (self.size, self.mtime, self.ctime)
 
 class FileTree:
     """
     A file tree that can read from disk and write back changes.
 
-    Support files with multiple paths (hard links) and persistent serial number
-    id (inode), dirs, and explicit 'other'.
-    Files are accessible by file id.
+    Each file may have multiple paths (hard links).
+    Each file is identified by a persistent serial number id (inode).
+    Paths may be added or removed to a file object.
+    When a path is added to a file, it is registered into the tree.
+    If a file has a single path and that path is removed, the file is
+    de-registered from the tree.
+
+    Directory entries may also be "other," to represent pipes, etc.
+
     Optionally, associate metadata (size, ctime, mtime) to files. In this case,
     files are accessible by size.
+
     Files can be excluded by size limit. File paths and dirs can be excluded by
     glob pattern. Exclude patterns may be set so long as the root dir hasn't
     been scanned yet.
     """
 
     def __init__(self, **kwargs):
         """
@@ -488,15 +495,15 @@
                 and not self.is_size_ok(file_obj.file_metadata.size):
                 obj_path = \
                     self.printable_path(os.path.join(
                         parent_obj.get_relpath(), basename))
                 pr.debug("ignored file by size: %s", obj_path)
                 parent_obj.add_entry(basename, ExcludedItem(basename))
                 return
-        self._add_path(file_obj, parent_obj, basename)
+        self.add_path(file_obj, parent_obj, basename)
 
     def _scan_dir_process_dir(
             self, parent_obj, obj_id, parent_glob, basename):
         self._next_free_dir_id = max(self._next_free_dir_id, obj_id + 1)
         subdir_obj = self._new_dir_obj(obj_id)
         parent_obj.add_entry(basename, subdir_obj)
         if self._use_metadata:
@@ -573,15 +580,15 @@
                         and glob_matcher.exclude_file_bname(obj_bname):
                     pr.debug("excluded special file %s", obj_abspath)
                     yield (obj_bname, None, ExcludedItem, None)
                 else:
                     pr.debug("ignored special file %s", obj_abspath)
                     yield (obj_bname, None, OtherItem, None)
 
-    def _add_path(self, file_obj, dir_obj, fbasename):
+    def add_path(self, file_obj, dir_obj, fbasename):
         """
         Add a new path to a file object:  fbasename at dir_obj.
         If this is the first path, the file is registered into
         the tree indices.
         """
         if file_obj.relpaths == []:
             fid = file_obj.file_id
@@ -592,25 +599,25 @@
                     self._size_to_files[f_size].append(file_obj)
                 else:
                     self._size_to_files[f_size] = [file_obj]
         dir_obj.add_entry(fbasename, file_obj)
         relpath = os.path.join(dir_obj.get_relpath(), fbasename)
         file_obj.relpaths.append(relpath)
 
-    def _rm_path(self, file_obj, dir_obj, fbasename):
+    def rm_path(self, file_obj, dir_obj, fbasename):
         """
         Remove a path from an existing file: fbasename at dir.
         dir must have already been scanned.
         If the final path of a file is removed, the file is removed
         from tree indices.
         """
         dir_obj.rm_entry(fbasename)
         relpath = os.path.join(dir_obj.get_relpath(), fbasename)
         assert relpath in file_obj.relpaths, \
-            "_rm_path: non-existing relpath."
+            "rm_path: non-existing relpath."
         file_obj.relpaths.remove(relpath)
         if file_obj.relpaths == []:
             fid = file_obj.file_id
             del self._id_to_file[fid]
             if self._use_metadata:
                 file_sz = file_obj.file_metadata.size
                 self._size_to_files[file_sz].remove(file_obj)
@@ -619,16 +626,16 @@
 
     def _rm_file(self, file_obj):
         """
         Remove a file, i.e. remove all paths.
         """
         paths = list(file_obj.relpaths)
         for path in paths:
-            tr_obj = self.path_to_obj(os.path.dirname(path))
-            self._rm_path(file_obj, tr_obj, os.path.basename(path))
+            dir_obj = self.path_to_obj(os.path.dirname(path))
+            self.rm_path(file_obj, dir_obj, os.path.basename(path))
 
     def path_to_obj(self, relpath):
         """
         Return file or dir or other object by relpath from root, or None.
         Do not follow symlinks.
         """
         assert self.rootdir_obj is not None, \
@@ -742,46 +749,46 @@
                 yield k
 
     def add_path_writeback(self, file_obj, relpath):
         """
         Add a new path to an existing file, creating intermediate dirs if
         needed.
         """
-        tr_obj = self._create_dir_if_needed_writeback(os.path.dirname(relpath))
-        self._add_path(file_obj, tr_obj, os.path.basename(relpath))
+        dir_obj = self._create_dir_if_needed_writeback(os.path.dirname(relpath))
+        self.add_path(file_obj, dir_obj, os.path.basename(relpath))
         if self.writeback:
             assert file_obj is not None, \
                 "add_path_writeback: no file_obj."
             assert file_obj.relpaths, \
                 "add_path_writeback: no path exists."
             os.link(self.rel_to_abs(file_obj.relpaths[0]),
                     self.rel_to_abs(relpath))
 
     def rm_path_writeback(self, file_obj, relpath):
         if self.writeback:
             os.unlink(self.rel_to_abs(relpath))
-        tr_obj = self.path_to_obj(os.path.dirname(relpath))
-        assert tr_obj is not None and tr_obj.is_dir(), \
+        dir_obj = self.path_to_obj(os.path.dirname(relpath))
+        assert dir_obj is not None and dir_obj.is_dir(), \
             "rm_path_writeback: expected a dir at " + \
                 os.path.dirname(relpath)
-        self._rm_path(file_obj, tr_obj, os.path.basename(relpath))
+        self.rm_path(file_obj, dir_obj, os.path.basename(relpath))
 
     def mv_path_writeback(self, file_obj, fn_from, fn_to):
         """
         Rename one of the file's paths.
         """
         # Cannot be done by adding/removing links
         # on filesystems not supporting hard links.
         d_from = self.path_to_obj(os.path.dirname(fn_from))
         assert d_from is not None and d_from.is_dir(), \
             "mv_path_writeback: expected a dir at " + \
                 os.path.dirname(fn_from)
         d_to = self._create_dir_if_needed_writeback(os.path.dirname(fn_to))
-        self._add_path(file_obj, d_to, os.path.basename(fn_to))
-        self._rm_path(file_obj, d_from, os.path.basename(fn_from))
+        self.add_path(file_obj, d_to, os.path.basename(fn_to))
+        self.rm_path(file_obj, d_from, os.path.basename(fn_from))
         if self.writeback:
             os.rename(self.rel_to_abs(fn_from), self.rel_to_abs(fn_to))
 
     def rm_dir_writeback(self, dir_obj):
         """
         Execute a rmdir, write back to source tree if self.writeback is set.
         dir_obj cannot be the root directory.
@@ -799,27 +806,27 @@
         dir_obj.parent.rm_entry(basename)
 
     def _create_dir_if_needed_writeback(self, dir_relpath):
         """
         Return dir obj corresponding to dir_relpath, creating all needed
         directories. May raise TreeError.
         """
-        tr_obj = self.path_to_obj(dir_relpath)
-        if tr_obj is None:
+        dir_obj = self.path_to_obj(dir_relpath)
+        if dir_obj is None:
             supdname = os.path.dirname(dir_relpath)
             dbasename = os.path.basename(dir_relpath)
             supd = self._create_dir_if_needed_writeback(supdname)
             newd = self._new_dir_obj()
             newd.mark_scanned()
             supd.add_entry(dbasename, newd)
             if self.writeback:
                 os.mkdir(self.rel_to_abs(dir_relpath))
             return newd
-        elif tr_obj.is_dir():
-            return tr_obj
+        elif dir_obj.is_dir():
+            return dir_obj
         else:
             raise TreeError("cannot create dir " + dir_relpath)
 
     def exec_cmd(self, cmd):
         """
         Execute a (cmd, arg1, arg2).
         cms is one of "mv" ln" "rm"
```

### Comparing `lnsync-0.8.5/lnsync_pkg/image_dhash.py` & `lnsync-0.8.6/lnsync_pkg/image_dhash.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/argparse_scoped.py` & `lnsync-0.8.6/lnsync_pkg/argparse_scoped.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/modaltype.py` & `lnsync-0.8.6/lnsync_pkg/modaltype.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/fileproptree.py` & `lnsync-0.8.6/lnsync_pkg/fileproptree.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 # pylint: disable=invalid-name, abstract-method, no-member
 # pylint: disable=unused-import # Fails to detect metaclass parameters.
 
 import os
 import abc
 
 import lnsync_pkg.printutils as pr
-from lnsync_pkg.fileid import make_id_computer
+from lnsync_pkg.filesystems import make_id_computer
 from lnsync_pkg.miscutils import ListContextManager
 from lnsync_pkg.modaltype import onofftype, Mode
 from lnsync_pkg.filetree import \
     FileTree, FileItem, DirItem, ExcludedItem, TreeError
 from lnsync_pkg.propdbmanager import PropDBException, PropDBError, \
     PropDBNoValue, PropDBStaleValue
 from lnsync_pkg.sqlpropdb import SQLPropDBManager
@@ -484,14 +484,15 @@
             self.db.commit()
 
     def db_check_prop(self, file_obj):
         """
         Compare the file prop value from source against an up-to-date
         prop value in the db and return True or False accordingly.
         Do not update the database.
+        file_obj should be a file, not anyt other type of tree item.
         Raise PropDBStaleValue if the db value is not up-to-date.
         May raise TreeNoPropValueError if there was an error computing the
         prop from source.
         """
         assert self.rootdir_obj is not None, \
             "db_check_prop: missing root"
         assert file_obj is not None and file_obj.is_file(), \
```

### Comparing `lnsync-0.8.5/lnsync_pkg/lnsync_cmd_handlers.py` & `lnsync-0.8.6/lnsync_pkg/lnsync_cmd_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from lnsync_pkg.sqlpropdb import SQLPropDBManager
 import lnsync_pkg.printutils as pr
 from lnsync_pkg.miscutils import is_subdir, iter_is_empty, HelperAppError
 from lnsync_pkg.human2bytes import bytes2human
 import lnsync_pkg.fdupes as fdupes
 from lnsync_pkg.prefixdbname import pick_db_basename, get_default_dbprefix
-from lnsync_pkg.fileid import make_id_computer
+from lnsync_pkg.filesystems import make_id_computer
 from lnsync_pkg.groupedfileprinter import GroupedFileListPrinter
 from lnsync_pkg.matcher import TreePairMatcher
 from lnsync_pkg.filehashtree import \
     FileHashTree, TreeError, TreeNoPropValueError, PropDBException
 from lnsync_pkg.lnsync_treeargs import TreeLocation, TreeLocationOnline
 from lnsync_pkg.modaltype import Mode
 from lnsync_pkg.hasher_functions import HasherManager
@@ -177,37 +177,53 @@
         except subprocess.SubprocessError as exc:
             raise HelperAppError(rsync_cmd, str(exc)) from exc
 
 def do_search(args):
     """
     Search for files by relative pattern glob pattern.
     """
+# TODO group together file paths for the same file.
+#    grouper = GroupedFileListPrinter(args.hard_links, args.all_links)
+
+    return_code = 1  # If no files are found, return 1.
+
+    if args.glob is None:
+        return return_code
+
     def print_file_match(tree, fobj):
-        nonlocal return_code
+        if args.showsize:
+            pr.print(bytes2human(fobj.file_metadata.size), end=" ")
         pr.print(tree.printable_path(files_paths_matched[fobj][0]))
         for fpath in files_paths_matched[fobj][1:]:
             pr.print(" " + tree.printable_path(fpath))
         if args.all_links:
             for fpath in fobj.relpaths:
                 if fpath not in files_paths_matched[fobj]:
                     pr.print(" " + tree.printable_path(fpath))
 
+    def print_file_match_simple(tree, fobj, path):
+        """ Print just the first path.
+        """
+        if args.showsize:
+            pr.print(bytes2human(fobj.file_metadata.size), end=" ")
+        pr.print(tree.printable_path(fobj.relpaths[0]))
+
     def search_dir(tree, dir_obj, patterns):
         nonlocal files_paths_to_check
         nonlocal files_paths_matched
         nonlocal return_code
         if not patterns:
             return
         tree.scan_dir(dir_obj)
         patterns = set(patterns)
 
         def handle_file_match(obj, basename):
             path = os.path.join(dir_obj.get_relpath(), basename)
             if not args.hard_links or len(obj.relpaths) == 1:
-                pr.print(tree.printable_path(path))
+                print_file_match_simple(tree, obj)
             else:
                 if obj not in files_paths_to_check:
                     files_paths_to_check[obj] = list(obj.relpaths)
                     files_paths_matched[obj] = []
                 assert path in files_paths_to_check[obj], \
                     "handle_file_match: path not in paths to check"
                 files_paths_to_check[obj].remove(path)
@@ -251,19 +267,14 @@
                 continue
             return_code = 0
             if not args.hard_links or len(fobj.relpaths) == 1:
                 pr.print(tree.printable_path(fobj.relpaths[0]))
             else:
                 files_paths_matched[fobj] = paths_matched
 
-    return_code = 1 # If no files are found, return 1.
-
-    if args.glob is None:
-        return return_code
-
     tree_kws = (treearg.kws() for treearg in args.locations)
     glob_string = args.glob.to_str()
     glob_is_simple = not any(p in glob_string for p in("**", "/"))
     with FileHashTree.listof(tree_kws) as all_trees:
         for tree in all_trees:
             if args.hard_links:
                 files_paths_to_check = {}
@@ -429,14 +440,21 @@
                 res = 1
             else:
                 pr.info("no files failed check")
                 res = 0
             return res
 
         def check_one_file(fobj, path):
+            """
+            fobj can be any type of tree object, or None if path does not
+            correspond to any item, or if some containing dir is excluded.
+            """
+            if fobj is None or not fobj.is_file():
+                pr.warning("skipping: " + tree.printable_path(path))
+                return
             if tree.db_check_prop(fobj):
                 pr.info(
                     "passed check: " + tree.printable_path(path))
                 file_objs_checked_ok.add(fobj)
             else:
                 pr.print(
                     "failed check: " + tree.printable_path(path))
```

### Comparing `lnsync-0.8.5/lnsync_pkg/sqlpropdb.py` & `lnsync-0.8.6/lnsync_pkg/sqlpropdb.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/metadata.py` & `lnsync-0.8.6/lnsync_pkg/metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 lnsync project metadata.
 """
 
 # pylint: disable-all
 
 # The package name, which is also the "UNIX name" for the project.
 package = 'lnsync'
-version = '0.8.5'
-description = "Dir sync by content with rename detection, " \
+version = '0.8.6'
+description = "Sync local dirs by content, with rename detection and " \
               "hard link support, plus fast fdupes, and more."
 summary = description
 project = 'lnsync dir sync tool'
 project_no_spaces = project.replace(' ', '')
 url = 'https://github.com/mrsimoes/lnsync'
 download_url = 'https://github.com/mrsimoes/lnsync/archive/v%s.tar.gz' % version
 keywords = 'sync rsync fast rename backup link hardlink fdupes'
```

### Comparing `lnsync-0.8.5/lnsync_pkg/argparse_config.py` & `lnsync-0.8.6/lnsync_pkg/argparse_config.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/backtracker.py` & `lnsync-0.8.6/lnsync_pkg/backtracker.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/lnsync_pkg/hasher_functions.py` & `lnsync-0.8.6/lnsync_pkg/hasher_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     Value is stored in the db in a 8-bit field, so restrict values to 0-255.
     """
     XXHASH32 = 0 # Default.
     XXHASH64 = 1
     IMAGE_DHASH = 2
     THUMB_DHASH = 3
     THUMB_DHASH_SYM = 4
+    BASENAME_HASH = 5
     EXTERNAL = 255
 
     @staticmethod
     def get_values():
         return [e.name for e in HasherFunctionID if e.name != "EXTERNAL"]
 
     def __str__(self):
@@ -128,15 +129,15 @@
     _hasher_function_id = HasherFunctionID.THUMB_DHASH
 
     def __init__(self):
         super().__init__()
         try:
             from lnsync_pkg.gnome_thumbnailer \
                 import GnomeThumbnailer, ThumbnailerError
-        except ThumbnailerError as exc:
+        except Exception as exc:
             msg = f"cannot load gnome thumbnail module: {str(exc)};"
             msg += "'gnome-desktop' is needed"
             raise RuntimeError(msg) from exc
         self.gnome_thumbnailer = GnomeThumbnailer()
 
     def hash_file(self, fpath):
         thumbnail_path = self.gnome_thumbnailer.make_thumbnail(fpath)
@@ -147,14 +148,28 @@
     _hasher_function_id = HasherFunctionID.THUMB_DHASH_SYM
 
     def __init__(self):
         super().__init__()
         import lnsync_pkg.image_dhash as image_dhash
         self.dhash = image_dhash.dhash_symmetric_int64
 
+class BasenameHasher(DigestHasher):
+    _hasher_function_id = HasherFunctionID.BASENAME_HASH
+    def __init__(self):
+        super().__init__()
+        import xxhash # In the requirements, no check needed.
+        self._xxhash = xxhash
+
+    def hash_file(self, fpath):
+        # TODO handle files with multiple paths.
+        # TODO This just picks one filename.
+        basename = os.path.split(fpath)[-1]
+        hash_val_uint64 = self._xxhash.xxh64(basename).intdigest()
+        return uint64_to_int64(hash_val_uint64)
+
 class ExternalHasher(DigestHasher):
     _hasher_function_id = HasherFunctionID.EXTERNAL
 
     def __init__(self, external_exec):
         self.external_exec = external_exec
 
     def get_hasher_algo_id_plus(self):
```

### Comparing `lnsync-0.8.5/setup.py` & `lnsync-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `lnsync-0.8.5/PKG-INFO` & `lnsync-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: lnsync
-Version: 0.8.5
-Summary: Dir sync by content with rename detection, hard link support, plus fast fdupes, and more.
+Version: 0.8.6
+Summary: Sync local dirs by content, with rename detection and hard link support, plus fast fdupes, and more.
 Home-page: https://github.com/mrsimoes/lnsync
 Author: Miguel Simoes
 Author-email: miguelrsimoes@yahoo.com
 License: GNU General Public License v3
-Download-URL: https://github.com/mrsimoes/lnsync/archive/v0.8.5.tar.gz
-Description: ## Overview
-        _lnsync_ provides sync-by-content of local directories (including hard link syncing), plus other features related to matching and finding.
+Download-URL: https://github.com/mrsimoes/lnsync/archive/v0.8.6.tar.gz
+Description: # This package will be renamed to `hlnsync` starting with v0.9.0
+        
+        ## Overview
+        This tool provides sync-by-content of local directories, including hard links, plus other matching and searching features.
         
         ###  Features
-        The main feature is (partial) one-way sync of local directories by only renaming/linking/delinking on the target directory, without copying or deleting any file content from source. This may be used as a preprocessing step for a full sync tool (such as rsync).
+        The main feature is partial one-way sync of local directories without copying or deleting data, that is by only renaming/linking/delinking files in the target. This may be used as a perliminary step to a full sync using some other tool, such as rsync.
         
-        This is achieved by maintaining a simple one-file database of file hashes for each top directory.
+        For each file tree processed, a one-file database of file hashes is stored at its top directory.
         
-        Files match if they have the same size and hash value.
+        Using those file hashes, other features are provided, e.g. finding duplicate files, checking for file content changes, and listing all hard links to a file.
         
-        Using file hashes, other features are provided, including: finding duplicate files, checking for file content changes, and listing all hard links to a file.
+        Multiple hashing functions are provided, including dhash, an image hash that is invariant under scaling and recoloring. This allows finding duplicate images.
         
-        Other hashing functions are provided, including dhash, an image invariant under scaling and recoloring. This allows finding duplicate images.
+        Files match if they have the same size and hash. Modification time and permissions are ignored.
         
         ### File Trees: Online and Offline
         
-        The file structure under a directory (path names, file sizes, mod dates) can be saved to a one-file database, along with the file hashes. Such a database is termed here an _offline tree_, whereas local top directories with their hash database are _online trees_,
-        
-        Most _lnsync_ commands accept offline trees as well as local directory. For example, an offline tree may be used as the source to reorganize a target directory according to a certain pattern.
+        The structure of a file tree -- path names, file sizes, mod dates --  may be stored in a one-file database, along with the file hashes.
         
-        Via a config file, specific options may be applied to online trees matching a glob pattern.
+        Such a database file is an _offline tree_, while the top directory of a file tree with their hash database is an _online trees_. (Note: the database file of an online tree is NOT in itself an offline tree, since it does not include the tree directory structure, file names, etc.)
         
-        To describe a tree: `lnsync info <LOCATION>`.
+        Most _lnsync_ commands both offline and online trees. For example, an offline tree database may be used as a pattern to reorganize a target directory.
         
-        Note that the database file of an online tree is NOT an offline tree, since it is missing the file and directory names.
+        Using a config file, specific options may be applied to online trees matching glob patterns.
         
         ### File Hashes
+        
         Files are identified by their content hash, using either 32-bit or 64-bit xxHash (a fast, non-cryptographic hash function), or other functions (see Hashing Functions below).
         
         Hash values are stored in local databases, on a single file per tree, by default with a name matching `lnsync-[0-9]+.db`. Only one such file should exist at each location. At the time of creation, the numeric part is chosen randomly, to avoid overwriting by accident when doing a full sync. Files matching `lnsync-[0-9]+.db` as well as the hash database in use are ignored by _lnsync_ operations.
         
         File modification times are used to detect stale hash values. Modification times are not synced to the target.
         
         ### Hashing Functions
@@ -67,14 +68,15 @@
         Files which cannot be read are skipped. File ownership and permissions are otherwise ignored.
         
         Symbolic links and any other file system objects are ignored.
         
         As with rsync, files and directories may be included/excluded using glob patterns.
         
         ### Directories
+        
         When syncing, directories are created as needed on the target, and target directories left empty and not on the source are removed.
         
         ## Installing
         Install the latest version from the PyPI repository with `pip install --user -U lnsync` or else clone the repo with `git clone https://github.com/mrsimoes/lnsync.git` and then run `python setup.py install`.
         
         ### Alternative Tools for Linux
         Some of the many tools for syncing with rename detection:
@@ -88,15 +90,17 @@
         - _git_ itself identifies and stores files by content, and has been adapted for syncing.
         
         - Support in modern file systems (e.g. btrfs) for snapshots may be adapted for syncing.
         
         In addition to syncing, _lnsync_ allows using the file hash database to search for files according to a variety of criteria.
         
         ## Usage Scenarios
+        
         ### Syncing
+        
         If your photos are at `/home/you/Photos` and its backup is at `/mnt/disk/Photos`, then `lnsync sync /home/you/Photos /mnt/disk/Photos` will sync the target. For a dry run, use the `-n` switch.
         
         After syncing, two database files are created, one at the source `/home/you/Photos` and another at the target `/mnt/disk/Photos`. File hashes are computed, as needed, and stored in those files. The database filenames include a random suffix, to help avoid accidental overwriting when syncing with a tool other than _lsync_.
         
         To obtain an _rsync_ command that will complete syncing, skipping `lnsync` database files, run `lnsync rsync /home/you/Photos /mnt/disk/Photos`. If the `rsync` options provided are suitable, run the command again with the `-x` switch to execute. Alternatively, run `lnsync syncr /home/you/Photos /mnt/disk/Photos` to complete those two steps in one go.
         
         Finally, to compare source and target, run `lnsync cmp /home/you/Photos /mnt/disk/Photos`.
@@ -256,14 +260,15 @@
         
         - Only readable files and readable+accessible directories are read. Other files and dirs, as well as symlinks, pipes, special devices are ignored.
         
         - Minimal support for case-insensitive but case-preserving file systems like vfat: if a target file name differs from source match in case only, target is not updated.
         
         ### Release Notes
         
+        - v0.8.6: Show size in search command results. Add BasenameHasher. Drop dependency on psutil, use lsblk. Bug fixes. Improve documentation.
         - v0.8.5: New `onmorethanone` search command. Small fixes.
         - v0.8.4: Performance improvements on find commamnds. Bug fixes. Allow multiple arguments to `--dbrootmount`.
         - v0.8.3: Performance improvements and bug fixes.
         - v0.8.2: New --show-size and --min-size options. Much faster searches in offline database. Bug fixes.
         - v0.8.1: Implement onfirstnotonly for all hash functions.
         - v0.8.0: Rename hasher options. Rename main config section. New built-in hash functions: dhash and thumbnail_dhash. Bug fixes.
         - v0.7.6: New `onfirstnotonly` search command. Allow mkoffline to operate on non-writeable dirs. Fixed regressions: incomplete reading of config file options, mishandling of single quotes in offline location databases.
```

