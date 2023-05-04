# Comparing `tmp/cat_win-1.4.0.tar.gz` & `tmp/cat_win-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_win-1.4.0.tar", last modified: Thu Apr 20 22:34:38 2023, max compression
+gzip compressed data, was "cat_win-1.4.1.tar", last modified: Thu May  4 09:55:21 2023, max compression
```

## Comparing `cat_win-1.4.0.tar` & `cat_win-1.4.1.tar`

### file list

```diff
@@ -1,56 +1,60 @@
--rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.4.0/LICENSE
--rw-r--r--   0        0        0    12243 2023-04-19 11:11:16.578516 cat_win-1.4.0/README.md
--rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.4.0/cat_win/.pytest_cache/README.md
--rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.4.0/cat_win/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.4.0/cat_win/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      289 2023-04-20 12:34:28.496799 cat_win-1.4.0/cat_win/__init__.py
--rw-r--r--   0        0        0      344 2023-04-11 08:42:55.435968 cat_win-1.4.0/cat_win/__main__.py
--rw-r--r--   0        0        0    29624 2023-04-20 22:27:04.760434 cat_win-1.4.0/cat_win/cat.py
--rw-r--r--   0        0        0     3869 2023-04-14 08:51:24.082968 cat_win-1.4.0/cat_win/const/ArgConstants.py
--rw-r--r--   0        0        0     2316 2023-04-12 15:55:33.141057 cat_win-1.4.0/cat_win/const/ColorConstants.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/const/__init__.py
--rw-r--r--   0        0        0     8018 2023-04-12 15:54:59.223056 cat_win-1.4.0/cat_win/persistence/Config.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/persistence/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.4.0/cat_win/tests/__init__.py
--rw-r--r--   0        0        0     1147 2023-03-27 19:59:24.939031 cat_win-1.4.0/cat_win/tests/test_ArgConstants.py
--rw-r--r--   0        0        0     7330 2023-03-27 19:59:45.680091 cat_win-1.4.0/cat_win/tests/test_ArgParser.py
--rw-r--r--   0        0        0     1176 2023-03-27 19:59:53.853442 cat_win-1.4.0/cat_win/tests/test_Base64.py
--rw-r--r--   0        0        0     3703 2023-03-27 20:00:47.420987 cat_win-1.4.0/cat_win/tests/test_Converter.py
--rw-r--r--   0        0        0      906 2023-04-06 12:21:45.835140 cat_win-1.4.0/cat_win/tests/test_File.py
--rw-r--r--   0        0        0     1403 2023-03-27 20:01:02.041966 cat_win-1.4.0/cat_win/tests/test_FileAttributes.py
--rw-r--r--   0        0        0     4384 2023-04-06 12:13:16.999006 cat_win-1.4.0/cat_win/tests/test_Holder.py
--rw-r--r--   0        0        0     7161 2023-04-13 19:54:00.253510 cat_win-1.4.0/cat_win/tests/test_RawViewer.py
--rw-r--r--   0        0        0      386 2023-03-27 20:02:00.130018 cat_win-1.4.0/cat_win/tests/test_StdInHelper.py
--rw-r--r--   0        0        0     3199 2023-03-27 20:02:08.299116 cat_win-1.4.0/cat_win/tests/test_StringFinder.py
--rw-r--r--   0        0        0     3972 2023-03-27 20:02:15.478171 cat_win-1.4.0/cat_win/tests/test_UpdateChecker.py
--rw-r--r--   0        0        0     5829 2023-04-10 10:25:32.430203 cat_win-1.4.0/cat_win/tests/test_cat.py
--rw-r--r--   0        0        0     1622 2023-03-27 20:00:37.654265 cat_win-1.4.0/cat_win/tests/test_checksum.py
--rw-r--r--   0        0        0     6600 2023-04-14 08:29:10.170716 cat_win-1.4.0/cat_win/tests/test_full.py
--rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_B.txt
--rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_C.txt
--rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/full_test_result_D.txt
--rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test.txt
--rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.4.0/cat_win/tests/texts/test_empty.txt
--rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_1.txt
--rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_2.txt
--rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_3.txt
--rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.4.0/cat_win/tests/texts/test_holderEdgeCase_4.txt
--rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.4.0/cat_win/tests/texts/test_peek.txt
--rw-r--r--   0        0        0     4319 2023-04-12 15:45:05.960051 cat_win-1.4.0/cat_win/util/ArgParser.py
--rw-r--r--   0        0        0     2767 2023-04-14 08:30:01.328140 cat_win-1.4.0/cat_win/util/Base64.py
--rw-r--r--   0        0        0     3104 2023-02-25 11:32:26.664586 cat_win-1.4.0/cat_win/util/Converter.py
--rw-r--r--   0        0        0      331 2023-04-06 12:14:05.915760 cat_win-1.4.0/cat_win/util/File.py
--rw-r--r--   0        0        0     3917 2023-04-16 10:54:57.990970 cat_win-1.4.0/cat_win/util/FileAttributes.py
--rw-r--r--   0        0        0     5729 2023-04-14 08:24:12.581241 cat_win-1.4.0/cat_win/util/Holder.py
--rw-r--r--   0        0        0     2706 2023-04-19 12:44:27.293437 cat_win-1.4.0/cat_win/util/RawViewer.py
--rw-r--r--   0        0        0     6520 2023-04-19 17:28:53.675269 cat_win-1.4.0/cat_win/util/StdInHelper.py
--rw-r--r--   0        0        0     3724 2023-04-12 15:28:42.676941 cat_win-1.4.0/cat_win/util/StringFinder.py
--rw-r--r--   0        0        0      389 2023-02-19 10:54:41.299281 cat_win-1.4.0/cat_win/util/TmpFileHelper.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.0/cat_win/util/__init__.py
--rw-r--r--   0        0        0     1614 2023-04-12 15:36:43.277060 cat_win-1.4.0/cat_win/util/checksum.py
--rw-r--r--   0        0        0     5585 2023-03-29 11:31:31.822808 cat_win-1.4.0/cat_win/web/UpdateChecker.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.4.0/cat_win/web/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-14 15:23:59.559474 cat_win-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 cat_win-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.4.1/LICENSE
+-rw-r--r--   0        0        0    13844 2023-05-03 09:54:22.285343 cat_win-1.4.1/README.md
+-rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.4.1/cat_win/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.4.1/cat_win/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.4.1/cat_win/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.4.1/cat_win/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.4.1/cat_win/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      289 2023-05-03 09:25:07.971212 cat_win-1.4.1/cat_win/__init__.py
+-rw-r--r--   0        0        0      363 2023-05-01 18:46:04.882782 cat_win-1.4.1/cat_win/__main__.py
+-rw-r--r--   0        0        0    34673 2023-05-03 14:39:37.447115 cat_win-1.4.1/cat_win/cat.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.1/cat_win/const/__init__.py
+-rw-r--r--   0        0        0     4717 2023-05-03 09:19:54.039073 cat_win-1.4.1/cat_win/const/argconstants.py
+-rw-r--r--   0        0        0     2492 2023-05-01 16:13:49.121661 cat_win-1.4.1/cat_win/const/colorconstants.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.1/cat_win/persistence/__init__.py
+-rw-r--r--   0        0        0     8208 2023-05-01 16:14:23.265362 cat_win-1.4.1/cat_win/persistence/config.py
+-rw-r--r--   0        0        0      319 2023-05-01 18:46:08.801676 cat_win-1.4.1/cat_win/shell.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.4.1/cat_win/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:24.210446 cat_win-1.4.1/cat_win/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1347 2023-05-02 09:52:28.939216 cat_win-1.4.1/cat_win/tests/mocks/std.py
+-rw-r--r--   0        0        0     1170 2023-05-01 15:49:21.685058 cat_win-1.4.1/cat_win/tests/test_argconstants.py
+-rw-r--r--   0        0        0     8294 2023-05-02 08:59:10.289918 cat_win-1.4.1/cat_win/tests/test_argparser.py
+-rw-r--r--   0        0        0     7392 2023-05-03 09:05:55.317568 cat_win-1.4.1/cat_win/tests/test_cat.py
+-rw-r--r--   0        0        0     1131 2023-05-02 19:37:40.487184 cat_win-1.4.1/cat_win/tests/test_cbase64.py
+-rw-r--r--   0        0        0     1569 2023-05-02 19:37:45.944459 cat_win-1.4.1/cat_win/tests/test_checksum.py
+-rw-r--r--   0        0        0     3613 2023-05-02 19:37:53.765103 cat_win-1.4.1/cat_win/tests/test_converter.py
+-rw-r--r--   0        0        0      823 2023-05-02 19:38:00.930937 cat_win-1.4.1/cat_win/tests/test_file.py
+-rw-r--r--   0        0        0     2021 2023-05-01 15:57:01.266856 cat_win-1.4.1/cat_win/tests/test_fileattributes.py
+-rw-r--r--   0        0        0     6186 2023-05-02 19:38:14.571569 cat_win-1.4.1/cat_win/tests/test_full.py
+-rw-r--r--   0        0        0     6086 2023-05-01 18:44:11.062879 cat_win-1.4.1/cat_win/tests/test_holder.py
+-rw-r--r--   0        0        0     7408 2023-05-01 16:03:35.076827 cat_win-1.4.1/cat_win/tests/test_rawviewer.py
+-rw-r--r--   0        0        0     4277 2023-05-02 10:37:50.918683 cat_win-1.4.1/cat_win/tests/test_shell.py
+-rw-r--r--   0        0        0     1270 2023-05-01 16:04:47.934927 cat_win-1.4.1/cat_win/tests/test_stdinhelper.py
+-rw-r--r--   0        0        0     3117 2023-05-02 09:42:04.478371 cat_win-1.4.1/cat_win/tests/test_stringfinder.py
+-rw-r--r--   0        0        0     3951 2023-05-02 19:38:32.100152 cat_win-1.4.1/cat_win/tests/test_updatechecker.py
+-rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.4.1/cat_win/tests/texts/full_test_result_B.txt
+-rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.4.1/cat_win/tests/texts/full_test_result_C.txt
+-rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.4.1/cat_win/tests/texts/full_test_result_D.txt
+-rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.4.1/cat_win/tests/texts/test.txt
+-rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.4.1/cat_win/tests/texts/test_empty.txt
+-rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.4.1/cat_win/tests/texts/test_holderEdgeCase_1.txt
+-rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.4.1/cat_win/tests/texts/test_holderEdgeCase_2.txt
+-rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.4.1/cat_win/tests/texts/test_holderEdgeCase_3.txt
+-rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.4.1/cat_win/tests/texts/test_holderEdgeCase_4.txt
+-rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.4.1/cat_win/tests/texts/test_peek.txt
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.1/cat_win/util/__init__.py
+-rw-r--r--   0        0        0     5959 2023-05-02 19:36:46.470436 cat_win-1.4.1/cat_win/util/argparser.py
+-rw-r--r--   0        0        0     2765 2023-05-01 13:47:22.633145 cat_win-1.4.1/cat_win/util/cbase64.py
+-rw-r--r--   0        0        0     1621 2023-05-01 16:15:32.374189 cat_win-1.4.1/cat_win/util/checksum.py
+-rw-r--r--   0        0        0     3221 2023-05-01 14:51:45.585464 cat_win-1.4.1/cat_win/util/converter.py
+-rw-r--r--   0        0        0      365 2023-05-01 15:43:43.676935 cat_win-1.4.1/cat_win/util/file.py
+-rw-r--r--   0        0        0     3885 2023-05-01 13:59:25.760074 cat_win-1.4.1/cat_win/util/fileattributes.py
+-rw-r--r--   0        0        0     6329 2023-05-01 16:17:00.047671 cat_win-1.4.1/cat_win/util/holder.py
+-rw-r--r--   0        0        0     2736 2023-05-01 14:12:52.471228 cat_win-1.4.1/cat_win/util/rawviewer.py
+-rw-r--r--   0        0        0     6620 2023-05-01 16:17:59.443693 cat_win-1.4.1/cat_win/util/stdinhelper.py
+-rw-r--r--   0        0        0     3762 2023-05-01 16:20:02.002989 cat_win-1.4.1/cat_win/util/stringfinder.py
+-rw-r--r--   0        0        0      386 2023-05-01 18:45:26.688828 cat_win-1.4.1/cat_win/util/tmpfilehelper.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.4.1/cat_win/web/__init__.py
+-rw-r--r--   0        0        0     5682 2023-05-01 18:45:36.714361 cat_win-1.4.1/cat_win/web/updatechecker.py
+-rw-r--r--   0        0        0     1552 2023-04-14 15:23:59.559474 cat_win-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    14828 1970-01-01 00:00:00.000000 cat_win-1.4.1/PKG-INFO
```

### Comparing `cat_win-1.4.0/LICENSE` & `cat_win-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.0/README.md` & `cat_win-1.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div id="top"></div>
 
 <p>
-   <a href="https://pypi.org/project/cat-win/" alt="Downloads">
-      <img src="https://static.pepy.tech/personalized-badge/cat-win?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" align="right">
+   <a href="https://pepy.tech/project/cat-win/" alt="Downloads">
+      <img src="https://static.pepy.tech/personalized-badge/cat-win?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" align="right">
    </a>
-   <a href="https://pepy.tech/project/cat-win/" alt="Visitors">
-      <img src="https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win" align="right">
+   <a href="https://pypi.org/project/cat-win/" alt="Visitors">
+      <img src="https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win&right_color=orange" align="right">
    </a>
    <a href="https://github.com/SilenZcience/cat_win/tree/main/cat_win" alt="CodeSize">
       <img src="https://img.shields.io/github/languages/code-size/SilenZcience/cat_win?color=purple" align="right">
    </a>
 </p>
 
 [![OS-Windows]][OS-Windows]
@@ -101,16 +101,17 @@
 ```console
 python -m pip install --upgrade cat_win
 ```
 and manually install the desired module yourself.
 
 **OR alternatively** you can use the compiled version (*`Windows only`*):
 
-1. Simply download the [catw.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/catw.exe) file.
-2. Add the file path to your system-environment `PATH`-variables.
+1. Simply download the [catw.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/catw.exe) file to handle filecontents.
+2. Download the [cats.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/cats.exe) file to use the cat-shell (optional).
+3. Add the file path to your system-environment `PATH`-variables.
 
 > ⚠️ **You should never trust any executable file!** Feel free to compile the package yourself (e.g. using [PyInstaller](https://pyinstaller.org/en/stable/)).
 
 > You can verify the creation of catw.exe yourself by reading the [source code](https://github.com/SilenZcience/cat_win/blob/main/cat_win/cat.py), checking the [origin](https://github.com/SilenZcience/cat_win/tree/main/bin) of the file and validating the corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/main/.github/workflows/build_executable.yml) used.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -119,95 +120,111 @@
 ```console
 catw [FILE]... [OPTION]...
 catw --help
 ```
 
 > ⚠️ *from v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to keep the old command, you will have to define an alias yourself.*
 
-| Argument / Option      | Description                                               |
-|------------------------|-----------------------------------------------------------|
-| *-h, --help*           | show help message and exit                                |
-| *-v, --version*        | output version information                                |
-| *-d, --debug*          | show debug information                                    |
-|                        |                                                           |
-| *-n, --number*         | number all output lines                                   |
-| *-l, --linelength*     | display the length of each line                           |
-| *-e, --ends*           | display $ at the end of each line                         |
-| *-t, --tabs*           | display TAB characters as ^I                              |
-| *--eof, --eof*         | display EOF characters as ^EOF                            |
-| *-u, --unique*         | suppress repeated output lines                            |
-| *-b, --blank*          | hide empty lines                                          |
-| *-r, --reverse*        | reverse output                                            |
-| *-p, --peek*           | only print the first and last lines                       |
-| *-s, --sum*            | show sum of lines                                         |
-| *-S, --SUM*            | ONLY show sum of lines                                    |
-| *-f, --files*          | list applied files                                        |
-| *-F, --FILES*          | ONLY list applied files and file sizes                    |
-| *-g, --grep*           | only show lines containing queried keywords               |
-| *-i, --interactive*    | use stdin                                                 |
-| *-o, --oneline*        | take only the first stdin-line                            |
-| *-E, --ECHO*           | handle every following parameter as stdin                 |
-| *-c, --clip*           | copy output to clipboard                                  |
-| *-m, --checksum*       | show the checksums of all files                           |
-| *-a, --attributes*     | show meta-information about the files                     |
-|                        |                                                           |
-| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         |
-| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         |
-| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         |
-| *--b64e, --b64e*       | encode the input to base64                                |
-| *--b64d, --b64d*       | decode the input from base64                              |
-|                        |                                                           |
-| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        |
-| *--binview, --binview* | display the raw byte representation in binary             |
-|                        |                                                           |
-| *--nc, --nocolor*      | disable colored output                                    |
-| *--nb, --nobreak*      | do not interrupt the output on queried keywords           |
-| *--nk, --nokeyword*    | inverse the grep output                                   |
-| *-R, --reconfigure*    | reconfigure the stdin and stdout with the parsed encoding |
-| *--config, --config*   | change color configuration                                |
-|                        |                                                           |
-| *enc=X*                | set file enconding to X (default is utf-8)                |
-| *find=X*               | find/query a substring X in the given files               |
-| *match=X*              | find/query a pattern X in the given files                 |
-| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              |
-|                        |                                                           |
-| *[a,b]*                | replace a with b in every line                            |
-| *[a:​b:c]*              | python-like string indexing syntax (line by line)         |
+```console
+cats [OPTION]...
+cats --help
+```
+
+| Argument / Option      | Description                                               | works in shell |
+|------------------------|-----------------------------------------------------------|----------------|
+| *-h, --help*           | show help message and exit                                | ✔              |
+| *-v, --version*        | output version information                                | ✔              |
+| *-d, --debug*          | show debug information                                    | ✔              |
+|                        |                                                           |                |
+| *-n, --number*         | number all output lines                                   | ✔              |
+| *-l, --linelength*     | display the length of each line                           | ✔              |
+| *-e, --ends*           | display $ at the end of each line                         | ✔              |
+| *-t, --tabs*           | display TAB characters as ^I                              | ✔              |
+| *--eof, --eof*         | display EOF characters as ^EOF                            | ✔              |
+| *-u, --unique*         | suppress repeated output lines                            | ❌             |
+| *-b, --blank*          | hide empty lines                                          | ✔              |
+| *-r, --reverse*        | reverse output                                            | ❌             |
+| *-p, --peek*           | only print the first and last lines                       | ❌             |
+| *-s, --sum*            | show sum of lines                                         | ❌             |
+| *-S, --SUM*            | ONLY show sum of lines                                    | ❌             |
+| *-f, --files*          | list applied files                                        | ❌             |
+| *-F, --FILES*          | ONLY list applied files and file sizes                    | ❌             |
+| *-g, --grep*           | only show lines containing queried keywords               | ✔              |
+| *-i, --interactive*    | use stdin                                                 | ❌             |
+| *-o, --oneline*        | take only the first stdin-line                            | ❌             |
+| *-E, --ECHO*           | handle every following parameter as stdin                 | ❌             |
+| *-c, --clip*           | copy output to clipboard                                  | ✔              |
+| *-m, --checksum*       | show the checksums of all files                           | ❌             |
+| *-a, --attributes*     | show meta-information about the files                     | ❌             |
+|                        |                                                           |                |
+| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         | ✔              |
+| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         | ✔              |
+| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         | ✔              |
+| *--b64e, --b64e*       | encode the input to base64                                | ✔              |
+| *--b64d, --b64d*       | decode the input from base64                              | ✔              |
+|                        |                                                           |                |
+| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        | ❌             |
+| *--binview, --binview* | display the raw byte representation in binary             | ❌             |
+|                        |                                                           |                |
+| *--nc, --nocolor*      | disable colored output                                    | ✔              |
+| *--nb, --nobreak*      | do not interrupt the output on queried keywords           | ✔              |
+| *--nk, --nokeyword*    | inverse the grep output                                   | ✔              |
+| *--config, --config*   | change color configuration                                | ✔              |
+|                        |                                                           |                |
+| *-R, --R\<stream\>*    | reconfigure the std-stream(s) with the parsed encoding </br> \<stream\> = 'in'/'out'/'err' (default is stdin & stdout)| ✔ |
+|                        |                                                           |                |
+| *enc=X*                | set file enconding to X (default is utf-8)                | ✔              |
+| *find=X*               | find/query a substring X in the given files               | ✔              |
+| *match=X*              | find/query a pattern X in the given files                 | ✔              |
+| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              | ❌             |
+|                        |                                                           |                |
+| *[a,b]*                | replace a with b in every line                            | ✔              |
+| *[a:​b:c]*              | python-like string indexing syntax (line by line)         | ✔              |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
-![Example1](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png "example1")
-
-![Example2](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png "example2")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png" width="49%"/>
+   </p>
 
-![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png "example3")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png" width="49%"/>
+   </p>
 
-![Example4](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png "example4")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png" width="49%"/>
+   </p>
 
-![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png "example5")
+   - - - -
 
-![Example6](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png "example6")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png" width="49%"/>
+   </p>
 
 </details>
 
-```console
+```c
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
+- - - -
+
 ```c
 $ cats --dec -nl
 > >>> 12345
 > 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
-> >>> 54321
-> 2) [55] 54321 {Hexadecimal: 0xd431; Binary: 0b1101010000110001}
-> ...
+> >>> ...
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
 Take a look at the [Changelog](https://github.com/SilenZcience/cat_win/blob/main/CHANGELOG.md) file.
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 [https://static.pepy.tech/personalized-badge/cat-
-win?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads]
-[https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win] [https://
-img.shields.io/github/languages/code-size/SilenZcience/cat_win?color=purple]
+win?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads]
+[https://visitor-badge.laobi.icu/
+badge?page_id=SilenZcience.cat_win&right_color=orange] [https://img.shields.io/
+github/languages/code-size/SilenZcience/cat_win?color=purple]
 [![OS-Windows]][OS-Windows] [![OS-Linux]][OS-Linux] [![OS-MacOS]][OS-MacOS]
                               ***** cat_win *****
                    Simple Command-line Tool made in Python
                              Explore_the_code_Â»
 
                          Report_Bug Â· Request_Feature
  Table of Contents
@@ -45,71 +46,79 @@
 --upgrade cat_win[clip] ``` cat_win uses the [pyperclip](https://pypi.org/
 project/pyperclip/) module by default. Should any problems occur, you can also
 use the [pyperclip3](https://pypi.org/project/pyperclip3/) or [pyclip](https://
 pypi.org/project/pyclip/) module. In this case simply run: ```console python -
 m pip install --upgrade cat_win ``` and manually install the desired module
 yourself. **OR alternatively** you can use the compiled version (*`Windows
 only`*): 1. Simply download the [catw.exe](https://raw.githubusercontent.com/
-SilenZcience/cat_win/main/bin/catw.exe) file. 2. Add the file path to your
-system-environment `PATH`-variables. > â ï¸ **You should never trust any
-executable file!** Feel free to compile the package yourself (e.g. using
+SilenZcience/cat_win/main/bin/catw.exe) file to handle filecontents. 2.
+Download the [cats.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/
+main/bin/cats.exe) file to use the cat-shell (optional). 3. Add the file path
+to your system-environment `PATH`-variables. > â ï¸ **You should never trust
+any executable file!** Feel free to compile the package yourself (e.g. using
 [PyInstaller](https://pyinstaller.org/en/stable/)). > You can verify the
 creation of catw.exe yourself by reading the [source code](https://github.com/
 SilenZcience/cat_win/blob/main/cat_win/cat.py), checking the [origin](https://
 github.com/SilenZcience/cat_win/tree/main/bin) of the file and validating the
 corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/
 main/.github/workflows/build_executable.yml) used.
                                                                   (back_to_top)
 ## Usage ```console catw [FILE]... [OPTION]... catw --help ``` > â ï¸ *from
 v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to
-keep the old command, you will have to define an alias yourself.* | Argument /
-Option | Description | |------------------------|------------------------------
------------------------------| | *-h, --help* | show help message and exit | |
-*-v, --version* | output version information | | *-d, --debug* | show debug
-information | | | | | *-n, --number* | number all output lines | | *-l, --
-linelength* | display the length of each line | | *-e, --ends* | display $ at
-the end of each line | | *-t, --tabs* | display TAB characters as ^I | | *--
-eof, --eof* | display EOF characters as ^EOF | | *-u, --unique* | suppress
-repeated output lines | | *-b, --blank* | hide empty lines | | *-r, --reverse*
-| reverse output | | *-p, --peek* | only print the first and last lines | | *-
-s, --sum* | show sum of lines | | *-S, --SUM* | ONLY show sum of lines | | *-f,
---files* | list applied files | | *-F, --FILES* | ONLY list applied files and
-file sizes | | *-g, --grep* | only show lines containing queried keywords | |
-*-i, --interactive* | use stdin | | *-o, --oneline* | take only the first
-stdin-line | | *-E, --ECHO* | handle every following parameter as stdin | | *-
-c, --clip* | copy output to clipboard | | *-m, --checksum* | show the checksums
-of all files | | *-a, --attributes* | show meta-information about the files | |
-| | | *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | | *-
--hex, --HEX* | convert hexadecimal numbers to decimal and binary | | *--bin, --
-BIN* | convert binary numbers to decimal and hexadecimal | | *--b64e, --b64e* |
-encode the input to base64 | | *--b64d, --b64d* | decode the input from base64
-| | | | | *--hexview, --HEXVIEW* | display the raw byte representation in
-hexadecimal | | *--binview, --binview* | display the raw byte representation in
-binary | | | | | *--nc, --nocolor* | disable colored output | | *--nb, --
-nobreak* | do not interrupt the output on queried keywords | | *--nk, --
-nokeyword* | inverse the grep output | | *-R, --reconfigure* | reconfigure the
-stdin and stdout with the parsed encoding | | *--config, --config* | change
-color configuration | | | | | *enc=X* | set file enconding to X (default is
-utf-8) | | *find=X* | find/query a substring X in the given files | | *match=X*
-| find/query a pattern X in the given files | | *trunc=X:Y* | truncate file to
-lines X and Y (python-like) | | | | | *[a,b]* | replace a with b in every line
-| | *[a:âb:c]* | python-like string indexing syntax (line by line) | ###
-Examples  ð Images ð ![Example1](https://raw.githubusercontent.com/
-SilenZcience/cat_win/main/img/example1.png "example1") ![Example2](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png
-"example2") ![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/
-main/img/example3.png "example3") ![Example4](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png
-"example4") ![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/
-main/img/example5.png "example5") ![Example6](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png
-"example6")  ```console $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1]
--ln > 1) [8] ): dlroW ``` ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
-{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> 54321 > 2) [55] 54321
-{Hexadecimal: 0xd431; Binary: 0b1101010000110001} > ... ```
+keep the old command, you will have to define an alias yourself.* ```console
+cats [OPTION]... cats --help ``` | Argument / Option | Description | works in
+shell | |------------------------|---------------------------------------------
+--------------|----------------| | *-h, --help* | show help message and exit |
+â | | *-v, --version* | output version information | â | | *-d, --debug* |
+show debug information | â | | | | | | *-n, --number* | number all output
+lines | â | | *-l, --linelength* | display the length of each line | â | |
+*-e, --ends* | display $ at the end of each line | â | | *-t, --tabs* |
+display TAB characters as ^I | â | | *--eof, --eof* | display EOF characters
+as ^EOF | â | | *-u, --unique* | suppress repeated output lines | â | | *-
+b, --blank* | hide empty lines | â | | *-r, --reverse* | reverse output | â
+| | *-p, --peek* | only print the first and last lines | â | | *-s, --sum* |
+show sum of lines | â | | *-S, --SUM* | ONLY show sum of lines | â | | *-f,
+--files* | list applied files | â | | *-F, --FILES* | ONLY list applied files
+and file sizes | â | | *-g, --grep* | only show lines containing queried
+keywords | â | | *-i, --interactive* | use stdin | â | | *-o, --oneline* |
+take only the first stdin-line | â | | *-E, --ECHO* | handle every following
+parameter as stdin | â | | *-c, --clip* | copy output to clipboard | â | |
+*-m, --checksum* | show the checksums of all files | â | | *-a, --attributes*
+| show meta-information about the files | â | | | | | | *--dec, --DEC* |
+convert decimal numbers to hexadecimal and binary | â | | *--hex, --HEX* |
+convert hexadecimal numbers to decimal and binary | â | | *--bin, --BIN* |
+convert binary numbers to decimal and hexadecimal | â | | *--b64e, --b64e* |
+encode the input to base64 | â | | *--b64d, --b64d* | decode the input from
+base64 | â | | | | | | *--hexview, --HEXVIEW* | display the raw byte
+representation in hexadecimal | â | | *--binview, --binview* | display the
+raw byte representation in binary | â | | | | | | *--nc, --nocolor* | disable
+colored output | â | | *--nb, --nobreak* | do not interrupt the output on
+queried keywords | â | | *--nk, --nokeyword* | inverse the grep output | â
+| | *--config, --config* | change color configuration | â | | | | | | *-R, --
+R\
+>* | reconfigure the std-stream(s) with the parsed encoding  \
+> = 'in'/'out'/'err' (default is stdin & stdout)| â | | | | | | *enc=X* | set
+file enconding to X (default is utf-8) | â | | *find=X* | find/query a
+substring X in the given files | â | | *match=X* | find/query a pattern X in
+the given files | â | | *trunc=X:Y* | truncate file to lines X and Y (python-
+like) | â | | | | | | *[a,b]* | replace a with b in every line | â | | *[a:
+âb:c]* | python-like string indexing syntax (line by line) | â | ###
+Examples  ð Images ð
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png]
+- - - -
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png]
+ ```c $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
+dlroW ``` - - - - ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
+{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
```

### Comparing `cat_win-1.4.0/cat_win/.pytest_cache/v/cache/nodeids` & `cat_win-1.4.1/cat_win/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.0/cat_win/cat.py` & `cat_win-1.4.1/cat_win/cat.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,102 +6,126 @@
 from functools import lru_cache
 from itertools import groupby
 from platform import system
 from re import sub as resub
 import os
 import sys
 
-from cat_win.const.ArgConstants import *
-from cat_win.const.ColorConstants import C_KW
-from cat_win.util.Base64 import decodeBase64, encodeBase64
-from cat_win.util.FileAttributes import getFileMetaData, getFileSize, _convert_size
-from cat_win.util.RawViewer import getRawViewLinesGen
-from cat_win.web.UpdateChecker import printUpdateInformation
-import cat_win.persistence.Config as Config
-import cat_win.util.ArgParser as ArgParser
-import cat_win.util.checksum as checksum
-import cat_win.util.Converter as Converter
-import cat_win.util.Holder as Holder
-import cat_win.util.StdInHelper as StdInHelper
-import cat_win.util.StringFinder as StringFinder
-import cat_win.util.TmpFileHelper as TmpFileHelper
-
+from cat_win.const.argconstants import *
+from cat_win.const.colorconstants import CKW
+from cat_win.persistence.config import Config
+from cat_win.util.argparser import ArgParser
+from cat_win.util.cbase64 import decode_base64, encode_base64
+from cat_win.util.checksum import get_checksum_from_file
+from cat_win.util.converter import Converter
+from cat_win.util.fileattributes import get_file_meta_data, get_file_size, _convert_size
+from cat_win.util.holder import Holder
+from cat_win.util.rawviewer import get_raw_view_lines_gen
+from cat_win.util.stringfinder import StringFinder
+from cat_win.util.tmpfilehelper import TmpFileHelper
+from cat_win.util import stdinhelper
+from cat_win.web.updatechecker import print_update_information
 from cat_win import __project__, __version__, __sysversion__, __author__, __url__
-workingDir = os.path.dirname(os.path.realpath(__file__))
+
+
+working_dir = os.path.dirname(os.path.realpath(__file__))
 
 coloramaInit()
-config = Config.Config(workingDir)
+config = Config(working_dir)
 
-color_dic = config.loadConfig()
+default_color_dic = config.load_config()
+color_dic = default_color_dic.copy()
 
-converter = Converter.Converter()
-holder = Holder.Holder()
-tmpFileHelper = TmpFileHelper.TmpFileHelper()
+arg_parser = ArgParser()
+converter = Converter()
+holder = Holder()
+tmp_file_helper = TmpFileHelper()
 
-on_windows_os = (system() == 'Windows')
+on_windows_os = system() == 'Windows'
 
 def exception_handler(exception_type: type, exception, traceback, debug_hook=sys.excepthook) -> None:
-    print(color_dic[C_KW.RESET_ALL])
-    if holder.args_id[ARGS_DEBUG]:
+    try:
+        print(color_dic[CKW.RESET_ALL])
+        if holder.args_id[ARGS_DEBUG]:
+            debug_hook(exception_type, exception, traceback)
+            return
+        print(f"\n{exception_type.__name__}{':' * bool(str(exception))} {exception}")
+        if exception_type != KeyboardInterrupt:
+            print('If this Exception is unexpected, please raise an official Issue at:')
+            print(f"{__url__}/issues")
+    except Exception:
         debug_hook(exception_type, exception, traceback)
-        return
-    print(f"\n{exception_type.__name__}{':' * bool(str(exception))} {exception}")
-    if exception_type != KeyboardInterrupt:
-        print(f"If this Exception is unexpected, please raise an official Issue at:\n{__url__}/issues")
 
 
 sys.excepthook = exception_handler
 
 
-def _showHelp() -> None:
+def _show_help(shell: bool = False) -> None:
     """
     Show the Help message and exit.
     """
-    helpMessage = 'Usage: catw [FILE]... [OPTION]...\n'
-    helpMessage += 'Concatenate FILE(s) to standard output.\n\n'
-    for x in ALL_ARGS:
-        helpMessage += f"\t{f'{x.shortForm}, {x.longForm}': <25}{x.help}\n"
-    helpMessage += '\n'
-    helpMessage += f"\t{'enc=X, enc:X'    : <25}set file encoding to X (default is utf-8)\n"
-    helpMessage += f"\t{'find=X, find:X'  : <25}find/query a substring X in the given files\n"
-    helpMessage += f"\t{'match=X, match:X': <25}find/query a pattern X in the given files\n"
-    helpMessage += f"\t{'trunc=X:Y, trunc:X:Y': <25}truncate file to lines x and y (python-like)\n"
-    helpMessage += '\n'
-    helpMessage += f"\t{'[a,b]': <25}replace a with b in every line\n"
-    helpMessage += f"\t{'[a:b:c]': <25}python-like string indexing syntax (line by line)\n"
-    helpMessage += '\n'
-    helpMessage += 'Examples:\n'
-    helpMessage += f"\t{'cat f g -r' : <25}Output g's contents in reverse order, then f's content in reverse order\n"
-    helpMessage += f"\t{'cat f g -ne': <25}Output f's, then g's content, while numerating and showing the end of lines\n"
-    helpMessage += f"\t{'cat f trunc=a:b:c': <25}Output f's content starting at line a, ending at line b, stepping c\n"
-    print(helpMessage)
-    printUpdateInformation(__project__, __version__, color_dic)
+    if shell:
+        help_message = 'Usage: cats [OPTION]...\n'
+        help_message += 'Interactively manipulate standard input.\n\n'
+    else:
+        help_message = 'Usage: catw [FILE]... [OPTION]...\n'
+        help_message += 'Concatenate FILE(s) to standard output.\n\n'
+    for arg in ALL_ARGS:
+        if arg.show_arg and (not shell or arg.show_arg_on_shell):
+            help_message += f"\t{f'{arg.short_form}, {arg.long_form}': <25}{arg.arg_help}\n"
+    help_message += '\n'
+    help_message += f"\t{'-R, --R<stream>': <25}reconfigure the std-stream(s) with the parsed encoding\n"
+    help_message += "\t<stream> == 'in'/'out'/'err' (default is stdin & stdout)\n"
+    help_message += '\n'
+    help_message += f"\t{'enc=X, enc:X'    : <25}set file encoding to X (default is utf-8)\n"
+    help_message += f"\t{'find=X, find:X'  : <25}find/query a substring X in the given files\n"
+    help_message += f"\t{'match=X, match:X': <25}find/query a pattern X in the given files\n"
+    if not shell:
+        help_message += f"\t{'trunc=X:Y, trunc:X:Y': <25}truncate file to lines x and y (python-like)\n"
+    help_message += '\n'
+    help_message += f"\t{'[a,b]': <25}replace a with b in every line\n"
+    help_message += f"\t{'[a:b:c]': <25}python-like string indexing syntax (line by line)\n"
+    help_message += '\n'
+    help_message += 'Examples:\n'
+    if shell:
+        help_message += '\tcats --ln --dec\n'
+        help_message += '\t> >>> 12345\n'
+        help_message += '\t1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}\n'
+        help_message += '\t> >>> !help\n'
+        help_message += '\t> ...\n'
+    else:
+        help_message += f"\t{'catw f g -r' : <25}Output g's contents in reverse order, then f's content in reverse order\n"
+        help_message += f"\t{'catw f g -ne': <25}Output f's, then g's content, while numerating and showing the end of lines\n"
+        help_message += f"\t{'catw f trunc=a:b:c': <25}Output f's content starting at line a, ending at line b, stepping c\n"
+    print(help_message)
+    print_update_information(__project__, __version__, color_dic)
 
 
-def _showVersion() -> None:
+def _show_version() -> None:
     """
     Show the Version message and exit.
     """
-    catVersion = f"Catw {__version__} - from {workingDir}\n"
-    versionMessage = '\n'
-    versionMessage += '-' * len(catVersion) + '\n'
-    versionMessage += catVersion
-    versionMessage += '-' * len(catVersion) + '\n'
-    versionMessage += '\n'
-    versionMessage += f"Built with: \tPython {__sysversion__}\n"  # sys.version
+    cat_version = f"Catw {__version__} - from {working_dir}\n"
+    version_message = '\n'
+    version_message += '-' * len(cat_version) + '\n'
+    version_message += cat_version
+    version_message += '-' * len(cat_version) + '\n'
+    version_message += '\n'
+    version_message += f"Built with: \tPython {__sysversion__}\n"  # sys.version
     try:
-        versionMessage += f"Install time: \t{datetime.fromtimestamp(os.path.getctime(os.path.realpath(__file__)))}\n"
+        version_message += f"Install time: \t{datetime.fromtimestamp(os.path.getctime(os.path.realpath(__file__)))}\n"
     except OSError: # fails on pyinstaller executable
-        versionMessage += f"Install time: \t-\n"
-    versionMessage += f"Author: \t{__author__}\n"
-    print(versionMessage)
-    printUpdateInformation(__project__, __version__, color_dic)
+        version_message += 'Install time: \t-\n'
+    version_message += f"Author: \t{__author__}\n"
+    print(version_message)
+    print_update_information(__project__, __version__, color_dic)
 
 
-def _showDebug(args: list, unknown_args: list, known_files: list, unknown_files: list, echo_args: list) -> None:
+def _show_debug(args: list, unknown_args: list, known_files: list, unknown_files: list,
+                echo_args: list) -> None:
     """
     Print all neccassary debug information
     """
     print('Debug Information:')
     print('args: ', end='')
     print([(arg[0], arg[1], holder.args_id[arg[0]]) for arg in args])
     print('unknown_args: ', end='')
@@ -109,114 +133,115 @@
     print('known_files: ', end='')
     print(known_files)
     print('unknown_files: ', end='')
     print(unknown_files)
     print('echo_args: ', end='')
     print(echo_args)
     print('file encoding: ', end='')
-    print(ArgParser.FILE_ENCODING)
+    print(arg_parser.file_encoding)
     print('search keyword(s): ', end='')
-    print(ArgParser.FILE_SEARCH)
+    print(arg_parser.file_search)
     print('search match(es): ', end='')
-    print(ArgParser.FILE_MATCH)
+    print(arg_parser.file_match)
     print('truncate file: ', end='')
-    print(ArgParser.FILE_TRUNCATE)
+    print(arg_parser.file_truncate)
 
 
-def _showCount() -> None:
+def _show_count() -> None:
     """
     display the line sum of each file individually if
     ARGS_CCOUNT is specified.
-    display the line sum of all files
+    display the line sum of all files.
     """
     if holder.args_id[ARGS_CCOUNT]:
-        longestFileName = max(map(len, holder.allFilesLines.keys())) + 1
-        print(f"{color_dic[C_KW.COUNT_AND_FILES]}{'File': <{longestFileName}}LineCount{color_dic[C_KW.RESET_ALL]}")
-        for file in holder.allFilesLines.keys():
-            print(f"{color_dic[C_KW.COUNT_AND_FILES]}{file: <{longestFileName}}{holder.allFilesLines[file]: >{holder.fileLineNumberPlaceHolder}}{color_dic[C_KW.RESET_ALL]}")
+        longest_file_name = max(map(len, holder.all_files_lines.keys())) + 1
+        print(f"{color_dic[CKW.COUNT_AND_FILES]}{'File': <{longest_file_name}}LineCount{color_dic[CKW.RESET_ALL]}")
+        for file in holder.all_files_lines:
+            print(f"{color_dic[CKW.COUNT_AND_FILES]}{file: <{longest_file_name}}{holder.all_files_lines[file]: >{holder.all_line_number_place_holder}}{color_dic[CKW.RESET_ALL]}")
         print('')
-    print(f"{color_dic[C_KW.COUNT_AND_FILES]}Lines (Sum): {holder.allFilesLinesSum}{color_dic[C_KW.RESET_ALL]}")
+    print(f"{color_dic[CKW.COUNT_AND_FILES]}Lines (Sum): {holder.all_files_lines_sum}{color_dic[CKW.RESET_ALL]}")
 
 
-def _showFiles() -> None:
+def _show_files() -> None:
     """
     displays holder.files including their size and calculates
     their size sum.
     """
     if len(holder.files) == 0:
         return
     file_sizes = []
     msg = 'found' if holder.args_id[ARGS_FFILES] else 'applied'
-    print(color_dic[C_KW.COUNT_AND_FILES], end='')
+    print(color_dic[CKW.COUNT_AND_FILES], end='')
     print(f"{msg} FILE(s):", end='')
-    print(color_dic[C_KW.RESET_ALL])
+    print(color_dic[CKW.RESET_ALL])
     for file in holder.files:
-        size = getFileSize(file.path)
+        size = get_file_size(file.path)
         file_sizes.append(size)
-        print(f"\t{color_dic[C_KW.COUNT_AND_FILES]}{_convert_size(size): <10}{'*' if file.containsQueried else ' '}{file.displayname}{color_dic[C_KW.RESET_ALL]}")
-    print(color_dic[C_KW.COUNT_AND_FILES], end='')
+        print(f"\t{color_dic[CKW.COUNT_AND_FILES]}{_convert_size(size): <10}", end='')
+        print(f"{'*' if file.contains_queried else ' '}{file.displayname}{color_dic[CKW.RESET_ALL]}")
+    print(color_dic[CKW.COUNT_AND_FILES], end='')
     print(f"Sum:\t{_convert_size(sum(file_sizes))}", end='')
-    print(color_dic[C_KW.RESET_ALL])
-    print(color_dic[C_KW.COUNT_AND_FILES], end='')
+    print(color_dic[CKW.RESET_ALL])
+    print(color_dic[CKW.COUNT_AND_FILES], end='')
     print(f"Amount:\t{len(holder.files)}", end='')
-    print(color_dic[C_KW.RESET_ALL])
+    print(color_dic[CKW.RESET_ALL])
 
 
-def _printMeta(file: str) -> None:
+def _print_meta(file: str) -> None:
     """
-    print the information retrieved by getFileMetaData()
+    print the information retrieved by get_file_meta_data()
     
     Parameters:
     file (str):
         a string representation of a file (-path)
     """
-    metaData = getFileMetaData(file, on_windows_os,
-                               [color_dic[C_KW.RESET_ALL],
-                               color_dic[C_KW.ATTRIB],
-                               color_dic[C_KW.ATTRIB_POSITIVE],
-                               color_dic[C_KW.ATTRIB_NEGATIVE]])
-    print(metaData)
+    meta_data = get_file_meta_data(file, on_windows_os,
+                               [color_dic[CKW.RESET_ALL],
+                               color_dic[CKW.ATTRIB],
+                               color_dic[CKW.ATTRIB_POSITIVE],
+                               color_dic[CKW.ATTRIB_NEGATIVE]])
+    print(meta_data)
 
 
-def _printChecksum(file: str) -> None:
+def _print_checksum(file: str) -> None:
     """
-    print the information retrieved by getChecksumFromFile()
+    print the information retrieved by get_checksum_from_file()
     
     Parameters:
     file (str):
         a string representation of a file (-path)
     """
-    print(f"{color_dic[C_KW.CHECKSUM]}Checksum of '{file}':{color_dic[C_KW.RESET_ALL]}")
-    print(checksum.getChecksumFromFile(file, [color_dic[C_KW.CHECKSUM], color_dic[C_KW.RESET_ALL]]))
+    print(f"{color_dic[CKW.CHECKSUM]}Checksum of '{file}':{color_dic[CKW.RESET_ALL]}")
+    print(get_checksum_from_file(file, [color_dic[CKW.CHECKSUM], color_dic[CKW.RESET_ALL]]))
 
 
-def _printMetaAndChecksum(showMeta: bool, showChecksum: bool) -> None:
+def _print_meta_and_checksum(show_meta: bool, show_checksum: bool) -> None:
     """
-    calls _printMeta() and _printChecksum() on every file.
+    calls _print_meta() and _print_checksum() on every file.
     
     Parameters:
-    showMeta (bool):
+    show_meta (bool):
         decides if the metadata of the files should be displayed
-    showChecksum (bool):
+    show_checksum (bool):
         decides if the checksum of the files should be displayed
     """
     for file in holder.files:
-        if showMeta:
-            _printMeta(file.path)
-        if showChecksum:
-            _printChecksum(file.path)
+        if show_meta:
+            _print_meta(file.path)
+        if show_checksum:
+            _print_checksum(file.path)
 
 
-def removeAnsiCodesFromLine(line: str) -> str:
+def remove_ansi_codes_from_line(line: str) -> str:
     """
     Parameters:
     line (str):
         the string to clean ANSI-Colorcodes from
         
-    Returns
+    Returns:
     (str):
         the cleaned string
     """
     # version 1: efficiency is about the same, and does not have any dependency
     # however it is not as safe in case of unusual/broken escape sequences.
     # while (codePosStart := line.find(ESC_CODE)) != -1:
     #     codePosEnd = line[codePosStart:].find('m')
@@ -226,536 +251,634 @@
     #     line = line[:codePosStart] + line[codePosStart+codePosEnd+1:]
     # return line
     # version 2:
     return resub(r'\x1b\[[0-9\;]*m', '', line)
 
 
 # def removeAnsiCodes(content: list) -> list:
-#     return [(removeAnsiCodesFromLine(prefix), removeAnsiCodesFromLine(line)) for prefix, line in content]
+#     return [(remove_ansi_codes_from_line(prefix), remove_ansi_codes_from_line(line)) for prefix, line in content]
 
 
 @lru_cache(maxsize=None)
-def _CalculateLinePrefixSpacing(lineCharLength: int,
-                                includeFilePrefix: bool = False, fileCharLength: int = 0) -> str:
+def _calculate_line_prefix_spacing(line_char_length: int, include_file_prefix: bool = False,
+                                   file_char_length: int = 0) -> str:
     """
     calculate a string template for the line prefix.
     
     Parameters:
-    lineCharLength (int):
+    line_char_length (int):
         the length of the line number
-    includeFilePrefix (bool):
+    include_file_prefix (bool):
         should the file be included in the prefix
-    fileCharLength (int):
+    file_char_length (int):
         the length of the file number
     
     Returns:
     (str):
         a non-finished but correctly formatted string template to insert line number
         and file index into
     """
-    line_prefix = (' ' * (holder.fileLineNumberPlaceHolder - lineCharLength)) + '%i)'
+    line_prefix = (' ' * (holder.all_line_number_place_holder - line_char_length)) + '%i)'
 
-    if includeFilePrefix:
-        file_prefix = (' ' * (holder.fileNumberPlaceHolder - fileCharLength)) + '%i.'
-        return color_dic[C_KW.NUMBER] + file_prefix + line_prefix + color_dic[C_KW.RESET_ALL] + ' '
+    if include_file_prefix:
+        file_prefix = (' ' * (holder.file_number_place_holder - file_char_length)) + '%i.'
+        return color_dic[CKW.NUMBER] + file_prefix + line_prefix + color_dic[CKW.RESET_ALL] + ' '
 
-    return color_dic[C_KW.NUMBER] + line_prefix + color_dic[C_KW.RESET_ALL] + ' '
+    return color_dic[CKW.NUMBER] + line_prefix + color_dic[CKW.RESET_ALL] + ' '
 
 
-def _getLinePrefix(line_num: int, index: int) -> str:
+def _get_line_prefix(line_num: int, index: int) -> str:
     """
     calculates the line prefix in regard to the line number and file count.
     
     Parameters:
     line_num (int):
         the current number identifying the line
     index (int):
         the current number identifying the file
     
     Returns:
     (str):
         the new line prefix including the line number.
     """
     if len(holder.files) > 1:
-        return _CalculateLinePrefixSpacing(len(str(line_num)), True, len(str(index))) % (index, line_num)
-    return _CalculateLinePrefixSpacing(len(str(line_num))) % (line_num)
+        return _calculate_line_prefix_spacing(len(str(line_num)), True, len(str(index))) % (index, line_num)
+    return _calculate_line_prefix_spacing(len(str(line_num))) % (line_num)
 
 
 @lru_cache(maxsize=None)
-def _CalculateLineLengthPrefixSpacing(lineCharLength: int) -> str:
+def _calculate_line_length_prefix_spacing(line_char_length: int) -> str:
     """
     calculate a string template for the line prefix.
     
     Parameters:
-    lineCharLength (int):
+    line_char_length (int):
         the length of the line
     
     Returns:
     (str):
         a non-finished but correctly formatted string template to insert line length into
     """
-    lengthPrefix = '[' + ' ' * (holder.fileLineLengthPlaceHolder - lineCharLength) + '%i]'
-    return '%s' + color_dic[C_KW.LINE_LENGTH] + lengthPrefix + color_dic[C_KW.RESET_ALL] + ' '
+    length_prefix = '[' + ' ' * (holder.file_line_length_place_holder - line_char_length) + '%i]'
+    return '%s' + color_dic[CKW.LINE_LENGTH] + length_prefix + color_dic[CKW.RESET_ALL] + ' '
 
 
-def _getLineLengthPrefix(prefix: str, line) -> str:
+def _get_line_length_prefix(prefix: str, line) -> str:
     """
     calculates the line prefix in regard to the line length.
     
     Parameters:
     prefix (str):
         the current prefix to append to
     line (str|byte):
         a representation of the current line
     
     Returns:
     (str):
         the new line prefix including the line length.
     """
-    if not holder.args_id[ARGS_NOCOL] and type(line) == str:
-        line = removeAnsiCodesFromLine(line)
-    return _CalculateLineLengthPrefixSpacing(len(str(len(line)))) % (prefix, len(line))
+    if not holder.args_id[ARGS_NOCOL] and isinstance(line, str):
+        line = remove_ansi_codes_from_line(line)
+    return _calculate_line_length_prefix_spacing(len(str(len(line)))) % (prefix, len(line))
 
 
-def printFile(content: list) -> bool:
+def print_file(content: list) -> bool:
     """
     print a file and possibly include the substrings and patterns to search for.
     
     Parameters:
     content (list):
         the content of a file like [(prefix, line), ...]
         
-    Returns
+    Returns:
     (bool):
         identifies if the given content parameter contained any
         queried keyword/pattern.
     """
     if not content:
         return False
-    if not (ArgParser.FILE_SEARCH or ArgParser.FILE_MATCH):
+    if not (arg_parser.file_search or arg_parser.file_match):
         print(*[prefix + line for prefix, line in content], sep='\n')
         return False
 
-    containsQueried = False
-    stringFinder = StringFinder.StringFinder(ArgParser.FILE_SEARCH, ArgParser.FILE_MATCH)
+    contains_queried = False
+    string_finder = StringFinder(arg_parser.file_search, arg_parser.file_match)
 
     for line_prefix, line in content:
-        cleanedLine = removeAnsiCodesFromLine(line)
-        intervals, fKeyWords, mKeywords = stringFinder.findKeywords(cleanedLine)
-        
-        if len(fKeyWords + mKeywords) == 0:
+        cleaned_line = remove_ansi_codes_from_line(line)
+        intervals, f_keywords, m_keywords = string_finder.find_keywords(cleaned_line)
+
+        if len(f_keywords + m_keywords) == 0:
             if not holder.args_id[ARGS_GREP]:
                 print(line_prefix + line)
             continue
-        
-        containsQueried = True
+
+        contains_queried = True
         if holder.args_id[ARGS_NOKEYWORD]:
             continue
-        
+
         if not holder.args_id[ARGS_NOCOL]:
             for kw_pos, kw_code in intervals:
-                cleanedLine = cleanedLine[:kw_pos] + color_dic[kw_code] + cleanedLine[kw_pos:]
+                cleaned_line = cleaned_line[:kw_pos] + color_dic[kw_code] + cleaned_line[kw_pos:]
 
-        print(line_prefix + cleanedLine)
+        print(line_prefix + cleaned_line)
 
         if holder.args_id[ARGS_GREP] or holder.args_id[ARGS_NOBREAK]:
             continue
-        
+
         found_sth = False
-        if fKeyWords:
-            print(color_dic[C_KW.FOUND_MESSAGE], end='')
-            print('--------------- Found', fKeyWords, '---------------', end='')
-            print(color_dic[C_KW.RESET_ALL])
+        if f_keywords:
+            print(color_dic[CKW.FOUND_MESSAGE], end='')
+            print('--------------- Found', f_keywords, '---------------', end='')
+            print(color_dic[CKW.RESET_ALL])
             found_sth = True
-        if mKeywords:
-            print(color_dic[C_KW.MATCHED_MESSAGE], end='')
-            print('--------------- Matched', mKeywords, '---------------', end='')
-            print(color_dic[C_KW.RESET_ALL])
+        if m_keywords:
+            print(color_dic[CKW.MATCHED_MESSAGE], end='')
+            print('--------------- Matched', m_keywords, '---------------', end='')
+            print(color_dic[CKW.RESET_ALL])
             found_sth = True
 
         if found_sth:
-            try:  # fails when using -i mode, because the stdin will send en EOF char to input without prompting the user
+            try:
+                # fails when using -i mode, because the stdin will send en EOF char
+                # to input without prompting the user
                 input()
             except (EOFError, UnicodeDecodeError):
                 pass
-            
-    return containsQueried
 
+    return contains_queried
 
-def printExcludedByPeek(content: list, excludedByPeek: int) -> None:
+
+def print_excluded_by_peek(content: list, excluded_by_peek: int) -> None:
     """
     print a paragraph about how many lines have been excluded.
     
     Parameters:
     content (list):
         the content of a file like [(prefix, line), ...]
-    excludedByPeek (int):
+    excluded_by_peek (int):
         the amount of lines that have been excluded
     """
-    if not excludedByPeek or len(content) <= 5:
+    if not excluded_by_peek or len(content) <= 5:
         return
-    excludedByPeek = excludedByPeek + 10 - len(content)
+    excluded_by_peek = excluded_by_peek + 10 - len(content)
     prefix = content[0][0]
-    prefix = prefix.replace(color_dic[C_KW.NUMBER], '')
-    prefix = prefix.replace(color_dic[C_KW.LINE_LENGTH], '')
-    prefix = prefix.replace(color_dic[C_KW.RESET_ALL], '')
-    excludedByPeekLength = (len(str(excludedByPeek))-1)//2
-    excludedByPeekIndent = ' ' * (len(prefix) - excludedByPeekLength + 10)
-    excludedByPeekIndentAdd = ' ' * excludedByPeekLength
-    print(color_dic[C_KW.NUMBER], end='')
-    print(excludedByPeekIndent, excludedByPeekIndentAdd, ' •', sep='')
-    print(excludedByPeekIndent, '(', excludedByPeek, ')', sep='')
-    print(excludedByPeekIndent, excludedByPeekIndentAdd, ' •', sep='', end='')
-    print(color_dic[C_KW.RESET_ALL])
+    prefix = prefix.replace(color_dic[CKW.NUMBER], '')
+    prefix = prefix.replace(color_dic[CKW.LINE_LENGTH], '')
+    prefix = prefix.replace(color_dic[CKW.RESET_ALL], '')
+    excluded_by_peek_length = (len(str(excluded_by_peek))-1)//2
+    excluded_by_peek_indent = ' ' * (len(prefix) - excluded_by_peek_length + 10)
+    excluded_by_peek_indent_add = ' ' * excluded_by_peek_length
+    print(color_dic[CKW.NUMBER], end='')
+    print(excluded_by_peek_indent, excluded_by_peek_indent_add, ' •', sep='')
+    print(excluded_by_peek_indent, '(', excluded_by_peek, ')', sep='')
+    print(excluded_by_peek_indent, excluded_by_peek_indent_add, ' •', sep='', end='')
+    print(color_dic[CKW.RESET_ALL])
 
 
-def editContent(content: list, show_bytecode: bool, fileIndex: int = 0, lineOffset: int = 0) -> None:
+def edit_content(content: list, show_bytecode: bool, file_index: int = 0,
+                 line_offset: int = 0) -> None:
     """
     apply all parameters to a string (file Content).
     
     Parameters:
     content (list):
         the content of a file like [(prefix, line), ...]
     show_bytecode (bool).
         indicates if the content lines are string or bytes
-    fileIndex (int):
+    file_index (int):
         the index of the holder.files list, pointing to the file that
         is currently being processed. a negative value can be used for
         the shell mode
     """
-    excludedByPeek = 0
-    
+    excluded_by_peek = 0
+
     if not show_bytecode and holder.args_id[ARGS_B64D]:
-        content = decodeBase64(content, ArgParser.FILE_ENCODING)
-    
+        content = decode_base64(content, arg_parser.file_encoding)
+
     if holder.args_id[ARGS_NUMBER]:
-        content = [(_getLinePrefix(j+lineOffset, fileIndex+1), c[1])
+        content = [(_get_line_prefix(j+line_offset, file_index+1), c[1])
                    for j, c in enumerate(content, start=1)]
-    content = content[ArgParser.FILE_TRUNCATE[0]:ArgParser.FILE_TRUNCATE[1]:ArgParser.FILE_TRUNCATE[2]]
+    content = content[arg_parser.file_truncate[0]:arg_parser.file_truncate[1]:arg_parser.file_truncate[2]]
     if holder.args_id[ARGS_PEEK] and len(content) > 10:
-        excludedByPeek = len(content) - 10
+        excluded_by_peek = len(content) - 10
         content = content[:5] + content[-5:]
 
     if not show_bytecode:
         for arg, param in holder.args:
             if arg == ARGS_CUT:
                 try:
                     content = [(prefix, eval(repr(line) + param))
                                 for prefix, line in content]
-                except:
+                except Exception:
                     print('Error at operation: ', param)
                     return
-        
+
         for arg, param in holder.args:
             if arg == ARGS_ENDS:
-                content = [(prefix, line + color_dic[C_KW.ENDS] + '$' + color_dic[C_KW.RESET_ALL])
+                content = [(prefix, line + color_dic[CKW.ENDS] + '$' + color_dic[CKW.RESET_ALL])
                            for prefix, line in content]
             elif arg == ARGS_TABS:
-                content = [(prefix, line.replace('\t', color_dic[C_KW.TABS] + '^I' + color_dic[C_KW.RESET_ALL]))
+                content = [(prefix, line.replace('\t', color_dic[CKW.TABS] + '^I' + color_dic[CKW.RESET_ALL]))
                            for prefix, line in content]
             elif arg == ARGS_SQUEEZE:
                 content = [list(group)[0] for _, group in groupby(content, lambda x: x[1])]
             elif arg == ARGS_REVERSE:
                 content.reverse()
             elif arg == ARGS_BLANK:
                 content = [c for c in content if c[1]]
             elif arg == ARGS_DEC:
-                content = [(prefix, line + ' ' + color_dic[C_KW.CONVERSION] + converter._fromDEC(int(line), (param == param.lower())) +
-                            color_dic[C_KW.RESET_ALL]) for prefix, line in content if converter.is_dec(line)]
+                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_dec(int(line), (param == param.lower())) +
+                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_dec(line)]
             elif arg == ARGS_HEX:
-                content = [(prefix, line + ' ' + color_dic[C_KW.CONVERSION] + converter._fromHEX(line, (param == param.lower())) +
-                            color_dic[C_KW.RESET_ALL]) for prefix, line in content if converter.is_hex(line)]
+                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_hex(line, (param == param.lower())) +
+                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_hex(line)]
             elif arg == ARGS_BIN:
-                content = [(prefix, line + ' ' + color_dic[C_KW.CONVERSION] + converter._fromBIN(line, (param == param.lower())) +
-                            color_dic[C_KW.RESET_ALL]) for prefix, line in content if converter.is_bin(line)]
+                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_bin(line, (param == param.lower())) +
+                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_bin(line)]
             elif arg == ARGS_REPLACE:
                 replace_values = param[1:-1].split(",")
-                content = [(prefix, line.replace(replace_values[0], color_dic[C_KW.REPLACE] + replace_values[1] + color_dic[C_KW.RESET_ALL]))
+                content = [(prefix, line.replace(replace_values[0], color_dic[CKW.REPLACE] + replace_values[1] + color_dic[CKW.RESET_ALL]))
                            for prefix, line  in content]
             elif arg == ARGS_EOF:
-                content = [(prefix, line.replace(chr(26), color_dic[C_KW.REPLACE] + '^EOF' + color_dic[C_KW.RESET_ALL]))
+                content = [(prefix, line.replace(chr(26), color_dic[CKW.REPLACE] + '^EOF' + color_dic[CKW.RESET_ALL]))
                            for prefix, line in content]
-            
+
     if holder.args_id[ARGS_LLENGTH]:
-        content = [(_getLineLengthPrefix(c[0], c[1]), c[1]) for c in content]
+        content = [(_get_line_length_prefix(c[0], c[1]), c[1]) for c in content]
     if holder.args_id[ARGS_B64E]:
-        content = encodeBase64(content, ArgParser.FILE_ENCODING)
+        content = encode_base64(content, arg_parser.file_encoding)
+
+    found_queried = print_file(content[:len(content)//2])
+    if file_index >= 0:
+        holder.files[file_index].set_contains_queried(found_queried)
+    print_excluded_by_peek(content, excluded_by_peek)
+    found_queried = print_file(content[len(content)//2:])
+    if file_index >= 0:
+        holder.files[file_index].set_contains_queried(found_queried)
 
-    foundQueried = printFile(content[:len(content)//2])
-    if fileIndex >= 0:
-        holder.files[fileIndex].setContainsQueried(foundQueried)
-    printExcludedByPeek(content, excludedByPeek)
-    foundQueried = printFile(content[len(content)//2:])
-    if fileIndex >= 0:
-        holder.files[fileIndex].setContainsQueried(foundQueried)
-    
     if not show_bytecode:
         if holder.args_id[ARGS_CLIP]:
-            holder.clipBoard += '\n'.join([prefix + line for prefix, line in content])
+            holder.clip_board += '\n'.join([prefix + line for prefix, line in content])
 
 
-def editFile(fileIndex: int = 0) -> None:
+def edit_file(file_index: int = 0) -> None:
     """
     apply all parameters to a file.
     
     Parameters:
-    fileIndex (int):
+    file_index (int):
         the index regarding which file is currently being edited
     """
     show_bytecode = False
-    
+
     content = [('', '')]
     try:
-        with open(holder.files[fileIndex].path, 'r', encoding=ArgParser.FILE_ENCODING) as f:
+        with open(holder.files[file_index].path, 'r', encoding=arg_parser.file_encoding) as file:
             # splitlines() gives a slight inaccuracy, in case the last line is empty.
             # the alternative would be worse: split('\n') would increase the linecount each
             # time catw touches a file.
-            content = [('', line) for line in f.read().splitlines()]
-    except:
-        print('Failed to open:', holder.files[fileIndex].displayname)
+            content = [('', line) for line in file.read().splitlines()]
+    except Exception as exc:
+        print('Failed to open:', holder.files[file_index].displayname)
         try:
-            enterChar = '⏎'
+            enter_char = '⏎'
             try:
-                if len(enterChar.encode(ArgParser.FILE_ENCODING)) != 3:
-                    raise UnicodeEncodeError('', '', -1, -1, '')
+                if len(enter_char.encode(arg_parser.file_encoding)) != 3:
+                    raise UnicodeEncodeError('', '', -1, -1, '') from exc
             except UnicodeEncodeError:
-                enterChar = 'ENTER'
-            print(f"Do you want to open the file as a binary, without parameters? [Y/{enterChar}]:", end='')
+                enter_char = 'ENTER'
+            print(f"Do you want to open the file as a binary, without parameters? [Y/{enter_char}]:", end='')
             inp = input()
             if not 'Y' in inp.upper() and inp:
                 print('Aborting...')
                 return
         except EOFError:
             pass
         except UnicodeError:
-            print(f"Input is not recognized in the given encoding: {ArgParser.FILE_ENCODING}")
+            print(f"Input is not recognized in the given encoding: {arg_parser.file_encoding}")
             print('Aborting...')
             return
         try:
-            with open(holder.files[fileIndex].path, 'rb') as f:
+            with open(holder.files[file_index].path, 'rb') as raw_f:
                 # in binary splitlines() is our only option
-                content = [('', repr(line)[2:-1]) for line in f.read().splitlines()]
+                content = [('', repr(line)[2:-1]) for line in raw_f.read().splitlines()]
             show_bytecode = True
-        except:
+        except Exception:
             print('Operation failed! Try using the enc=X parameter.')
             return
-    
-    editContent(content, show_bytecode, fileIndex)
+
+    edit_content(content, show_bytecode, file_index)
 
 
-def _copyToClipboard(content: str, __dependency: int = 3, __clipBoardError: bool = False) -> None:
+def _copy_to_clipboard(content: str, __dependency: int = 3,
+                       __clip_board_error: bool = False) -> None:
     """
     copy a string to the clipboard, by recursively checking which module exists and could
-    be used, this function should only be called by copyToClipboard()
+    be used, this function should only be called by copy_to_clipboard()
     
     Parameters:
     content (str):
         the string to copy
     __dependency (int):
         do not change!
-    __clipBoardError (bool):
+    __clip_board_error (bool):
         do not change!
     """
     if __dependency == 0:
-        if __clipBoardError:
-            errorMsg = '\n'
-            errorMsg += "ClipBoardError: You can use either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
-            errorMsg += "Try to install a different one using 'python -m pip install ...'"
+        if __clip_board_error:
+            error_msg = '\n'
+            error_msg += "ClipBoardError: You can use either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
+            error_msg += "Try to install a different one using 'python -m pip install ...'"
         else:
-            errorMsg = '\n'
-            errorMsg += "ImportError: You need either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
-            errorMsg += "Should you have any problem with either module, try to install a different one using 'python -m pip install ...'"
-        print(errorMsg)
+            error_msg = '\n'
+            error_msg += "ImportError: You need either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
+            error_msg += "Should you have any problem with either module, try to install a different one using 'python -m pip install ...'"
+        print(error_msg)
         return
     try:
         if __dependency == 3:
             import pyperclip as pc
         elif __dependency == 2:
             import pyclip as pc
         elif __dependency == 1:
             import pyperclip3 as pc
         pc.copy(content)
     except ImportError:
-        _copyToClipboard(content, __dependency-1, False or __clipBoardError)
+        _copy_to_clipboard(content, __dependency-1, False or __clip_board_error)
     except Exception:
-        _copyToClipboard(content, __dependency-1, True or __clipBoardError)
-    
+        _copy_to_clipboard(content, __dependency-1, True or __clip_board_error)
 
-def copyToClipboard(content: str) -> None:
+
+def copy_to_clipboard(content: str) -> None:
     """
-    entry point to recursive function _copyToClipboard()
+    entry point to recursive function _copy_to_clipboard()
     
     Parameters:
     content (str):
         the string to copy
     """
-    _copyToClipboard(content)
+    _copy_to_clipboard(content)
 
 
-def printRawView(fileIndex: int = 0, mode: str = 'X') -> None:
+def print_raw_view(file_index: int = 0, mode: str = 'X') -> None:
     """
     print the raw byte representation of a file in hexadecimal or binary
     
     Parameters:
-    fileIndex (int):
+    file_index (int):
         the index regarding which file is currently being edited
     mode (str):
         either 'x', 'X' for hexadecimal (lower- or upper case letters),
         or 'b' for binary
     """
-    print(holder.files[fileIndex].displayname, ':', sep='')
-    for line in getRawViewLinesGen(holder.files[fileIndex].path, mode, [color_dic[C_KW.RAWVIEWER], color_dic[C_KW.RESET_ALL]], ArgParser.FILE_ENCODING):
+    print(holder.files[file_index].displayname, ':', sep='')
+    for line in get_raw_view_lines_gen(holder.files[file_index].path, mode, \
+        [color_dic[CKW.RAWVIEWER], color_dic[CKW.RESET_ALL]], arg_parser.file_encoding):
         print(line)
     print('')
 
 
-def editFiles() -> None:
+def edit_files() -> None:
     """
-    manage the calls to editFile() for each file.
+    manage the calls to edit_file() for each file.
     """
     start = len(holder.files)-1 if holder.reversed else 0
     end = -1 if holder.reversed else len(holder.files)
 
-    rawViewMode = None
+    raw_view_mode = None
     if holder.args_id[ARGS_HEXVIEW] or holder.args_id[ARGS_BINVIEW]:
         for arg, param in holder.args:
             if arg == ARGS_HEXVIEW:
-                rawViewMode = 'X' if param == param.upper() else 'x'
+                raw_view_mode = 'X' if param == param.upper() else 'x'
                 break
-            elif arg == ARGS_BINVIEW:
-                rawViewMode = 'b'
+            if arg == ARGS_BINVIEW:
+                raw_view_mode = 'b'
                 break
-    
+
     for i in range(start, end, -1 if holder.reversed else 1):
-        if rawViewMode:
-            printRawView(i, rawViewMode)
+        if raw_view_mode:
+            print_raw_view(i, raw_view_mode)
         else:
-            editFile(i)
+            edit_file(i)
     if holder.args_id[ARGS_COUNT]:
         print('')
-        _showCount()
+        _show_count()
     if holder.args_id[ARGS_FILES]:
         print('')
-        _showFiles()
+        _show_files()
     if holder.args_id[ARGS_CLIP]:
-        copyToClipboard(removeAnsiCodesFromLine(holder.clipBoard))
+        copy_to_clipboard(remove_ansi_codes_from_line(holder.clip_board))
+
+
+def init_colors() -> None:
+    """
+    set the color dictionary to be used. either empty for no colors
+    or the default color dictionary.
+    """
+    # do not use colors if requested, or output will be piped anyways
+    global color_dic
+    if holder.args_id[ARGS_NOCOL] or (not sys.stdout.isatty() or sys.stdout.closed):
+        color_dic = dict.fromkeys(color_dic, '')
+    else:
+        color_dic = default_color_dic.copy()
 
 
 def init(shell: bool = False) -> tuple:
     """
     initiate the code by calling the argparser and handling the default
     parameters: -h, -v, -d, --config.
     
     Parameters:
-    contenshellt (bool):
+    shell (bool):
         indicates if the shell entry point was used, and the stdin will therefor
         be used by default
         
-    Returns
+    Returns:
     (tuple):
         contains (known_files, unknown_files, echo_args) from the argparser
     """
     # read parameter-args
-    args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(sys.argv)
+    args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(sys.argv)
 
-    holder.setArgs(args)
+    holder.set_args(args)
+
+    if holder.args_id[ARGS_RECONFIGURE] or holder.args_id[ARGS_RECONFIGURE_IN]:
+        sys.stdin.reconfigure(encoding=arg_parser.file_encoding)
+    if holder.args_id[ARGS_RECONFIGURE] or holder.args_id[ARGS_RECONFIGURE_OUT]:
+        sys.stdout.reconfigure(encoding=arg_parser.file_encoding)
+    if holder.args_id[ARGS_RECONFIGURE_ERR]:
+        sys.stderr.reconfigure(encoding=arg_parser.file_encoding)
+
+    init_colors()
 
-    if holder.args_id[ARGS_RECONFIGURE]:
-        sys.stdout.reconfigure(encoding=ArgParser.FILE_ENCODING)
-        sys.stdin.reconfigure(encoding=ArgParser.FILE_ENCODING)
-    
-    # do not use colors if requested, or output will be piped anyways
-    if holder.args_id[ARGS_NOCOL] or (not sys.stdout.isatty() or sys.stdout.closed):
-        global color_dic
-        color_dic = dict.fromkeys(color_dic,'')
-    
     # check for special cases
     if holder.args_id[ARGS_DEBUG]:
-        _showDebug(args, unknown_args, known_files, unknown_files, echo_args)
-    if (len(known_files) + len(unknown_files) + len(holder.args) == 0 and not shell) or holder.args_id[ARGS_HELP]:
-        _showHelp()
+        _show_debug(holder.args, unknown_args, known_files, unknown_files, echo_args)
+    if (len(known_files) + len(unknown_files) + len(holder.args) == 0 and not shell) or \
+        holder.args_id[ARGS_HELP]:
+        _show_help(shell)
         sys.exit(0)
     if holder.args_id[ARGS_VERSION]:
-        _showVersion()
+        _show_version()
         sys.exit(0)
     if holder.args_id[ARGS_CONFIG]:
-        config.saveConfig()
+        config.save_config()
         sys.exit(0)
-    
+
     return (known_files, unknown_files, echo_args)
 
 
 def main():
     piped_input = temp_file = ''
     known_files, unknown_files, echo_args = init(False)
-    
+
     if holder.args_id[ARGS_ECHO]:
-        temp_file = StdInHelper.writeTemp(' '.join(echo_args), tmpFileHelper.generateTempFileName(), ArgParser.FILE_ENCODING)
+        temp_file = stdinhelper.write_temp(' '.join(echo_args), \
+            tmp_file_helper.generate_temp_file_name(), arg_parser.file_encoding)
         known_files.append(temp_file)
-        holder.setTempFileEcho(temp_file)
+        holder.set_temp_file_echo(temp_file)
     if holder.args_id[ARGS_INTERACTIVE]:
-        piped_input = ''.join(StdInHelper.getStdInContent(holder.args_id[ARGS_ONELINE]))
-        temp_file = StdInHelper.writeTemp(piped_input, tmpFileHelper.generateTempFileName(), ArgParser.FILE_ENCODING)
+        piped_input = ''.join(stdinhelper.get_stdin_content(holder.args_id[ARGS_ONELINE]))
+        temp_file = stdinhelper.write_temp(piped_input, tmp_file_helper.generate_temp_file_name(), \
+            arg_parser.file_encoding)
         known_files.append(temp_file)
-        unknown_files = StdInHelper.writeFiles(unknown_files, piped_input, ArgParser.FILE_ENCODING)
-        holder.setTempFileStdIn(temp_file)
+        unknown_files = stdinhelper.write_files(unknown_files, piped_input, arg_parser.file_encoding)
+        holder.set_temp_file_stdin(temp_file)
     else:
-        unknown_files = StdInHelper.readWriteFilesFromStdIn(
-            unknown_files, ArgParser.FILE_ENCODING, on_windows_os, holder.args_id[ARGS_ONELINE])
+        unknown_files = stdinhelper.read_write_files_from_stdin(
+            unknown_files, arg_parser.file_encoding, on_windows_os, holder.args_id[ARGS_ONELINE])
 
-    if (len(known_files) + len(unknown_files) == 0):
+    if len(known_files) + len(unknown_files) == 0:
         return
 
     # fill holder object with neccessary values
-    holder.setFiles([*known_files, *unknown_files])
-    
+    holder.set_files([*known_files, *unknown_files])
+
     if holder.args_id[ARGS_FFILES]:
-        _showFiles()
+        _show_files()
         return
     if holder.args_id[ARGS_DATA] or holder.args_id[ARGS_CHECKSUM]:
-        _printMetaAndChecksum(holder.args_id[ARGS_DATA], holder.args_id[ARGS_CHECKSUM])
+        _print_meta_and_checksum(holder.args_id[ARGS_DATA], holder.args_id[ARGS_CHECKSUM])
         return
-    
+
     if holder.args_id[ARGS_B64D]:
-        holder.setDecodingTempFiles([tmpFileHelper.generateTempFileName() for _ in holder.files])
-    holder.generateValues(ArgParser.FILE_ENCODING)
+        holder.set_decoding_temp_files([tmp_file_helper.generate_temp_file_name() for _ in holder.files])
+    holder.generate_values(arg_parser.file_encoding)
 
     if holder.args_id[ARGS_CCOUNT]:
-        _showCount()
+        _show_count()
         return
 
     try:
-        editFiles()  # print the cat-output
+        edit_files()  # print the cat-output
     except IOError: # catch broken-pipe error
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stdout.fileno())
         sys.exit(1)  # Python exits with error code 1 on EPIPE
 
     # clean-up
-    for tmp_file in tmpFileHelper.getGeneratedTempFiles():
+    for tmp_file in tmp_file_helper.get_generated_temp_files():
         if holder.args_id[ARGS_DEBUG]:
             print('Cleaning', tmp_file)
         try:
             os.remove(tmp_file)
         except FileNotFoundError:
             if holder.args_id[ARGS_DEBUG]:
                 print('FileNotFoundError', tmp_file)
 
 
 def shell_main():
     init(True)
-    
-    shellPrefix = '>>> '
-    EOFControlChar = 'Z' if on_windows_os else 'D'
-    
-    print(__project__, 'v' + __version__, 'shell', '(' + __url__ + ')')
-    print(f"Use 'catw' to handle files. Type ^{EOFControlChar} (Ctrl + {EOFControlChar}) to exit.")
-    
-    print(shellPrefix, end='', flush=True)
-    for i, line in enumerate(StdInHelper.getStdInContent(holder.args_id[ARGS_ONELINE])):
-        editContent([('', line.rstrip('\n'))], False, -1, i)
-        if not holder.args_id[ARGS_ONELINE]:
-            print(shellPrefix, end='', flush=True)
+
+    shell_prefix = '>>> '
+    eof_control_char = 'Z' if on_windows_os else 'D'
+    oneline = holder.args_id[ARGS_ONELINE]
+
+    class CmdExec:
+        exit_shell = False
+
+        def exec_colors(self) -> None:
+            init_colors()
+            _calculate_line_prefix_spacing.cache_clear()
+            _calculate_line_length_prefix_spacing.cache_clear()
+
+        def exec(self, cmd: str) -> bool:
+            """
+            check if a shell line is an executable command,
+            executes it if it is.
+            
+            Parameters:
+            cmd (str):
+                the line entered in the cat shell
+                
+            Returns:
+            (bool):
+                indicates if a valid command has been found
+                and executed
+            """
+            if cmd[:1] != '!':
+                return False
+            line_split = cmd[1:].split(' ')
+            method = getattr(self, '_command_' + line_split[0], lambda _: False)
+            method(line_split[1:])
+            return True
+
+        def _command_cat(self, _) -> None:
+            cat = " ,_     _\n |\\\\_,-~/\n / _  _ |    ,--.\n(  @  @ )   / ,-'\n \  _T_/"
+            cat += "-._( (\n /         `. \\\n|         _  \ |\n \ \ ,  /      |\n  || |-_\__   /\n ((_/`(____,-'\n"
+            print('\n'.join(['\t\t\t' + c for c in cat.split('\n')]))
+
+        def _command_help(self, _) -> None:
+            print(f"Type ^{eof_control_char} (Ctrl + {eof_control_char}) or '!exit' to exit.")
+            print("Type '!add <OPTION>', '!del <OPTION>', '!see' to change/see the active parameters.")
+
+        def _command_add(self, cmd: list) -> None:
+            arg_parser.gen_arguments([''] + cmd)
+            holder.add_args(arg_parser.args)
+            self.exec_colors()
+            print(f"successfully added {[arg for _, arg in arg_parser.args] if arg_parser.args else 'parameters'}.")
+
+        def _command_del(self, cmd: list) -> None:
+            arg_parser.gen_arguments([''] + cmd, True)
+            holder.delete_args(arg_parser.args)
+            self.exec_colors()
+            print(f"successfully removed {[arg for _, arg in arg_parser.args] if arg_parser.args else 'parameters'}.")
+
+        def _command_see(self, _) -> None:
+            print(f"{'Active Args:': <12} {[arg for _, arg in holder.args]}")
+            if arg_parser.file_search:
+                print(f"{'Literals:':<12} {arg_parser.file_search}")
+            if arg_parser.file_match:
+                print(f"{'Matches:': <12} {arg_parser.file_match}")
+
+        def _command_exit(self, _) -> None:
+            self.exit_shell = True
+
+
+    cmd = CmdExec()
+    command_count = 0
+
+    print(__project__, 'v' + __version__, 'shell', '(' + __url__ + ')', end=' - ')
+    print("Use 'catw' to handle files.")
+    print("Type '!help' for more information.")
+
+    print(shell_prefix, end='', flush=True)
+    for i, line in enumerate(stdinhelper.get_stdin_content(oneline)):
+        stripped_line = line.rstrip('\n')
+        if cmd.exec(stripped_line):
+            command_count += 1
+            if cmd.exit_shell:
+                break
+        else:
+            stripped_line = stripped_line[:1].replace('\\', '') + stripped_line[1:]
+            if stripped_line:
+                edit_content([('', stripped_line)], False, -1, i-command_count)
+                if holder.args_id[ARGS_CLIP]:
+                    copy_to_clipboard(remove_ansi_codes_from_line(holder.clip_board))
+                    holder.clip_board = ''
+        if not oneline:
+            print(shell_prefix, end='', flush=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `cat_win-1.4.0/cat_win/const/ColorConstants.py` & `cat_win-1.4.1/cat_win/const/colorconstants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 
 ESC_CODE = '\x1b'
 
 
-def idToCode(code: int) -> str:
+def id_to_code(code: int) -> str:
+    """
+    converts a color id to a usable escape sequence
+    """
     return f"{ESC_CODE}[{code}m"
 
 
 class ColorOptions:
+    """
+    Holds the dictionaries mapping colors to ANSI-Escape codes.
+    """
     __Fore = {
         'RESET': 39,
-            
+
         'BLACK':   30,
         'RED':     31,
         'GREEN':   32,
         'YELLOW':  33,
         'BLUE':    34,
         'MAGENTA': 35,
         'CYAN':    36,
         'WHITE':   37,
-        
+
         'LIGHTBLACK':   90,
         'LIGHTRED':     91,
         'LIGHTGREEN':   92,
         'LIGHTYELLOW':  93,
         'LIGHTBLUE':    94,
         'LIGHTMAGENTA': 95,
         'LIGHTCYAN':    96,
         'LIGHTWHITE':   97
         }
     __Back = {
         'RESET': 49,
-            
+
         'BLACK':   40,
         'RED':     41,
         'GREEN':   42,
         'YELLOW':  43,
         'BLUE':    44,
         'MAGENTA': 45,
         'CYAN':    46,
         'WHITE':   47,
-          
+
         'LIGHTBLACK':   100,
         'LIGHTRED':     101,
         'LIGHTGREEN':   102,
         'LIGHTYELLOW':  103,
         'LIGHTBLUE':    104,
         'LIGHTMAGENTA': 105,
         'LIGHTCYAN':    106,
@@ -52,24 +58,27 @@
     __Style = {
         'RESET': 0
         }
 
     Fore  = {'NONE': ''}
     Back  = {'NONE': ''}
     Style = {'NONE': ''}
-    
+
     for key in __Fore:
-        Fore[key]  = idToCode(__Fore[key])
+        Fore[key]  = id_to_code(__Fore[key])
     for key in __Back:
-        Back[key]  = idToCode(__Back[key])
+        Back[key]  = id_to_code(__Back[key])
     for key in __Style:
-        Style[key] = idToCode(__Style[key])
+        Style[key] = id_to_code(__Style[key])
 
 
-class C_KW:
+class CKW:
+    """
+    The collection of all different color options
+    """
     RESET_ALL = 'reset_all'
     RESET_FOUND = 'reset_found'
     RESET_MATCHED = 'reset_matched'
 
     NUMBER = 'line_numbers'
     LINE_LENGTH = 'line_length'
     ENDS = 'line_ends'
@@ -81,13 +90,13 @@
     MATCHED = 'matched_pattern'
     MATCHED_MESSAGE = 'matched_pattern_message'
     CHECKSUM = 'checksum_message'
     COUNT_AND_FILES = 'processed_message'
     ATTRIB = 'file_attribute_message'
     ATTRIB_POSITIVE = 'active_file_attributes'
     ATTRIB_NEGATIVE = 'missing_file_attributes'
-    
+
     MESSAGE_INFORMATION = 'message_information'
     MESSAGE_IMPORTANT = 'message_important'
     MESSAGE_WARNING = 'message_warning'
-    
+
     RAWVIEWER = 'raw_viewer'
```

### Comparing `cat_win-1.4.0/cat_win/persistence/Config.py` & `cat_win-1.4.1/cat_win/persistence/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,170 @@
 from configparser import ConfigParser
 from os.path import join as path_join
 
-from cat_win.const.ColorConstants import ColorOptions, C_KW
+from cat_win.const.colorconstants import ColorOptions, CKW
 
 
 class Config:
-    default_dic = {C_KW.NUMBER: ColorOptions.Fore['GREEN'],
-                   C_KW.LINE_LENGTH: ColorOptions.Fore['LIGHTBLUE'],
-                   C_KW.ENDS: ColorOptions.Back['YELLOW'],
-                   C_KW.TABS: ColorOptions.Back['YELLOW'],
-                   C_KW.CONVERSION: ColorOptions.Fore['CYAN'],
-                   C_KW.REPLACE: ColorOptions.Fore['YELLOW'],
-                   C_KW.FOUND: ColorOptions.Fore['RED'],
-                   C_KW.FOUND_MESSAGE: ColorOptions.Fore['MAGENTA'],
-                   C_KW.MATCHED: ColorOptions.Back['CYAN'],
-                   C_KW.MATCHED_MESSAGE: ColorOptions.Fore['LIGHTCYAN'],
-                   C_KW.CHECKSUM: ColorOptions.Fore['CYAN'],
-                   C_KW.COUNT_AND_FILES: ColorOptions.Fore['CYAN'],
-                   C_KW.ATTRIB_POSITIVE: ColorOptions.Fore['LIGHTGREEN'],
-                   C_KW.ATTRIB_NEGATIVE: ColorOptions.Fore['LIGHTRED'],
-                   C_KW.ATTRIB: ColorOptions.Fore['CYAN'],
-                   C_KW.MESSAGE_INFORMATION: ColorOptions.Fore['LIGHTBLACK'],
-                   C_KW.MESSAGE_IMPORTANT: ColorOptions.Fore['YELLOW'],
-                   C_KW.MESSAGE_WARNING: ColorOptions.Fore['RED'],
-                   C_KW.RAWVIEWER: ColorOptions.Fore['LIGHTBLACK']}
+    """
+    manages the color configuration. Displays the user interface,
+    allows for reading and writing the config file.
+    """
+    default_dic = {CKW.NUMBER: ColorOptions.Fore['GREEN'],
+                   CKW.LINE_LENGTH: ColorOptions.Fore['LIGHTBLUE'],
+                   CKW.ENDS: ColorOptions.Back['YELLOW'],
+                   CKW.TABS: ColorOptions.Back['YELLOW'],
+                   CKW.CONVERSION: ColorOptions.Fore['CYAN'],
+                   CKW.REPLACE: ColorOptions.Fore['YELLOW'],
+                   CKW.FOUND: ColorOptions.Fore['RED'],
+                   CKW.FOUND_MESSAGE: ColorOptions.Fore['MAGENTA'],
+                   CKW.MATCHED: ColorOptions.Back['CYAN'],
+                   CKW.MATCHED_MESSAGE: ColorOptions.Fore['LIGHTCYAN'],
+                   CKW.CHECKSUM: ColorOptions.Fore['CYAN'],
+                   CKW.COUNT_AND_FILES: ColorOptions.Fore['CYAN'],
+                   CKW.ATTRIB_POSITIVE: ColorOptions.Fore['LIGHTGREEN'],
+                   CKW.ATTRIB_NEGATIVE: ColorOptions.Fore['LIGHTRED'],
+                   CKW.ATTRIB: ColorOptions.Fore['CYAN'],
+                   CKW.MESSAGE_INFORMATION: ColorOptions.Fore['LIGHTBLACK'],
+                   CKW.MESSAGE_IMPORTANT: ColorOptions.Fore['YELLOW'],
+                   CKW.MESSAGE_WARNING: ColorOptions.Fore['RED'],
+                   CKW.RAWVIEWER: ColorOptions.Fore['LIGHTBLACK']}
     elements = list(default_dic.keys())
 
-    def __init__(self, workingDir: str) -> None:
+    def __init__(self, working_dir: str) -> None:
         """
         Initialise the Config() object to load and save
         the color configs.
         
         Parameters:
-        workingDir (str):
+        working_dir (str):
             the working directory path of the package
         """
-        self.workingDir = workingDir
-        self.configFile = path_join(self.workingDir, 'cat.config')
-        
-        self.exclusive_definitions = {'Fore': [C_KW.FOUND],  # can only be Foreground
-                                      'Back': [C_KW.MATCHED]}  # can only be Background
-        self.configParser = ConfigParser()
+        self.working_dir = working_dir
+        self.config_file = path_join(self.working_dir, 'cat.config')
+
+        self.exclusive_definitions = {'Fore': [CKW.FOUND],  # can only be Foreground
+                                      'Back': [CKW.MATCHED]}  # can only be Background
+        self.config_parser = ConfigParser()
         self.color_dic = {}
-        
-        self.longestCharCount = 30
-        self.ROWS = 3
 
-    def loadConfig(self) -> dict:
+        self.longest_char_count = 30
+        self.rows = 3
+
+    def load_config(self) -> dict:
         """
         Load the Color Configuration from the config file.
         
         Returns:
         color_dic (dict):
-            a dictionary translating from C_KW-keywords to ANSI-Colorcodes
+            a dictionary translating from CKW-keywords to ANSI-Colorcodes
         On Error: Return the default color config
         """
         try:
-            self.configParser.read(self.configFile)
-            configColors = self.configParser['COLORS']
+            self.config_parser.read(self.config_file)
+            config_colors = self.config_parser['COLORS']
             for element in self.elements:
                 try:
-                    type, color = configColors[element].split('.')
+                    color_type, color = config_colors[element].split('.')
                     self.color_dic[element] = (
-                        ColorOptions.Fore[color] if type == 'Fore' else ColorOptions.Back[color]
+                        ColorOptions.Fore[color] if color_type == 'Fore'
+                        else ColorOptions.Back[color]
                         )
                 except KeyError:
                     self.color_dic[element] = self.default_dic[element]
         except KeyError:
-            self.configParser['COLORS'] = {}
+            self.config_parser['COLORS'] = {}
             # If an error occures we simplfy use the default colors
             self.color_dic = self.default_dic
 
         # The Reset Codes should always be the same
-        self.color_dic[C_KW.RESET_ALL] = ColorOptions.Style['RESET']
-        self.color_dic[C_KW.RESET_FOUND] = ColorOptions.Fore['RESET']
-        self.color_dic[C_KW.RESET_MATCHED] = ColorOptions.Back['RESET']
+        self.color_dic[CKW.RESET_ALL] = ColorOptions.Style['RESET']
+        self.color_dic[CKW.RESET_FOUND] = ColorOptions.Fore['RESET']
+        self.color_dic[CKW.RESET_MATCHED] = ColorOptions.Back['RESET']
 
         return self.color_dic
 
-    def _printGetAllAvailableColors(self) -> list:
+    def _print_get_all_available_colors(self) -> list:
         """
         prints all available color options to choose from.
         
         Returns:
         options (list):
             the same list containing all available colors.
         """
         print('Here is a list of all available color options you may choose:')
-        
-        ForeOptions = list(ColorOptions.Fore.items())
-        ForeOptions = [(k, v) for k, v in ForeOptions if k != 'RESET']
-        BackOptions = list(ColorOptions.Back.items())
-        BackOptions = [(k, v) for k, v in BackOptions if k != 'RESET']
-        indexOffset = len(str(len(ForeOptions) + len(BackOptions) + 1))
-        
-        configMenu = ''
+
+        fore_options = list(ColorOptions.Fore.items())
+        fore_options = [(k, v) for k, v in fore_options if k != 'RESET']
+        back_options = list(ColorOptions.Back.items())
+        back_options = [(k, v) for k, v in back_options if k != 'RESET']
+        index_offset = len(str(len(fore_options) + len(back_options) + 1))
+
+        config_menu = ''
         options = []
-        
-        for index in range(len(ForeOptions)):
-            key, value = ForeOptions[index]
-            coloredOption = f"{value}Fore.{key}{ColorOptions.Style['RESET']}"
-            configMenu += f"{index+1: <{indexOffset}}: {coloredOption: <{self.longestCharCount+len(value)}}"
-            if index % self.ROWS == self.ROWS-1:
-                configMenu += '\n'
+
+        for index in range(len(fore_options)):
+            key, value = fore_options[index]
+            colored_option = f"{value}Fore.{key}{ColorOptions.Style['RESET']}"
+            config_menu += f"{index+1: <{index_offset}}: {colored_option: <{self.longest_char_count+len(value)}}"
+            if index % self.rows == self.rows-1:
+                config_menu += '\n'
             options.append('Fore.' + key)
-        configMenu += '\n'
-        for index in range(len(BackOptions)):
-            key, value = BackOptions[index]
-            coloredOption = f"{value}Back.{key}{ColorOptions.Style['RESET']}"
-            configMenu += f"{len(ForeOptions)+index+1: <{indexOffset}}: {coloredOption: <{self.longestCharCount+len(value)}}"
-            if index % self.ROWS == self.ROWS-1:
-                configMenu += '\n'
+        config_menu += '\n'
+        for index in range(len(back_options)):
+            key, value = back_options[index]
+            colored_option = f"{value}Back.{key}{ColorOptions.Style['RESET']}"
+            config_menu += f"{len(fore_options)+index+1: <{index_offset}}: {colored_option: <{self.longest_char_count+len(value)}}"
+            if index % self.rows == self.rows-1:
+                config_menu += '\n'
             options.append('Back.' + key)
-        configMenu += '\n'
-        
-        print(configMenu)
+        config_menu += '\n'
+
+        print(config_menu)
         return options
 
-    def _printAllAvailableElements(self) -> None:
+    def _print_all_available_elements(self) -> None:
         """
         print all available elements which color can be changed.
         """
         print('Here is a list of all available elements you may change:')
-        
-        self.longestCharCount = max(map(len, self.elements)) + 12
-        indexOffset = len(str(len(self.elements) + 1))
 
-        configMenu = ''
+        self.longest_char_count = max(map(len, self.elements)) + 12
+        index_offset = len(str(len(self.elements) + 1))
+
+        config_menu = ''
         for index in range(len(self.elements)):
             element = self.elements[index]
-            coloredElement = f"{self.color_dic[element]}{element}{ColorOptions.Style['RESET']}"
-            configMenu += f"{index+1: <{indexOffset}}: {coloredElement: <{self.longestCharCount+len(self.color_dic[element])}}"
-            if index % self.ROWS == self.ROWS-1:
-                configMenu += '\n'
-        
-        print(configMenu)
+            colored_element = f"{self.color_dic[element]}{element}{ColorOptions.Style['RESET']}"
+            config_menu += f"{index+1: <{index_offset}}: {colored_element: <{self.longest_char_count+len(self.color_dic[element])}}"
+            if index % self.rows == self.rows-1:
+                config_menu += '\n'
+
+        print(config_menu)
 
-    def saveConfig(self) -> None:
+    def save_config(self) -> None:
         """
         Guide the User through the configuration options and save the changes.
-        Assume, that the current config is already loaded/the method loadConfig() was already called.
+        Assume, that the current config is already loaded/
+        the method load_config() was already called.
         """
-        self._printAllAvailableElements()
+        self._print_all_available_elements()
         keyword = ''
-        while (not keyword in self.elements):
+        while keyword not in self.elements:
             if keyword != '':
                 print(f"Something went wrong. Unknown keyword '{keyword}'")
             keyword = input('Input name of keyword to change: ')
             if keyword.isdigit():
                 keyword = self.elements[int(keyword)-1] if (
                     0 < int(keyword) <= len(self.elements)) else keyword
         print(f"Successfully selected element '{keyword}'.")
 
-        color_options = self._printGetAllAvailableColors()
+        color_options = self._print_get_all_available_colors()
         color = ''
-        while (not color in color_options):
+        while color not in color_options:
             if color != '':
                 print(f"Something went wrong. Unknown option '{color}'.")
             color = input('Input color: ')
             if color.isdigit():
                 color = color_options[int(color)-1] if (
                     0 < int(color) <= len(color_options)) else color
 
@@ -167,14 +173,14 @@
             return
         if keyword in self.exclusive_definitions['Back'] and color.startswith('Fore'):
             print(f"An Error occured: '{keyword}' can only be of style 'Back'")
             return
 
         print(f"Successfully selected element '{color}'.")
 
-        self.configParser['COLORS'][keyword] = color
+        self.config_parser['COLORS'][keyword] = color
         try:
-            with open(self.configFile, 'w') as conf:
-                self.configParser.write(conf)
-            print(f"Successfully updated config file:\n\t{self.configFile}")
+            with open(self.config_file, 'w', encoding='utf-8') as conf:
+                self.config_parser.write(conf)
+            print(f"Successfully updated config file:\n\t{self.config_file}")
         except OSError:
-            print(f"Could not write to config file:\n\t{self.configFile}")
+            print(f"Could not write to config file:\n\t{self.config_file}")
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_ArgConstants.py` & `cat_win-1.4.1/cat_win/tests/test_argconstants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from unittest import TestCase
 
-from cat_win.const.ArgConstants import *
+from cat_win.const.argconstants import ALL_ARGS
 # import sys
 # sys.path.append('../cat_win')
 
 
 class TestArgConstants(TestCase):
     def test_unique_parameters(self):
-        parameters_shortForm = [x.shortForm for x in ALL_ARGS]
-        parameters_longForm = [x.longForm for x in ALL_ARGS]
-        parameters_help = [x.help for x in ALL_ARGS]
-        parameters_id= [x.id for x in ALL_ARGS]
-        self.assertEqual(len(set(parameters_shortForm)), len(parameters_shortForm))
-        self.assertEqual(len(set(parameters_longForm)), len(parameters_longForm))
+        parameters_short_form = [x.short_form for x in ALL_ARGS]
+        parameters_long_form = [x.long_form for x in ALL_ARGS]
+        parameters_help = [x.arg_help for x in ALL_ARGS]
+        parameters_id= [x.arg_id for x in ALL_ARGS]
+        self.assertEqual(len(set(parameters_short_form)), len(parameters_short_form))
+        self.assertEqual(len(set(parameters_long_form)), len(parameters_long_form))
         self.assertEqual(len(set(parameters_help)), len(parameters_help))
         self.assertEqual(len(set(parameters_id)), len(parameters_id))
-        
+
     def test_no_concats(self):
-        parameters_shortForm = [x.shortForm for x in ALL_ARGS]
-        parameters_longForm = [x.longForm for x in ALL_ARGS]
-        parameters = parameters_shortForm + parameters_longForm
+        parameters_short_form = [x.short_form for x in ALL_ARGS]
+        parameters_long_form = [x.long_form for x in ALL_ARGS]
+        parameters = parameters_short_form + parameters_long_form
         for param in parameters:
             self.assertEqual(param[:1], '-')
             if not param.startswith('--'):
-                self.assertEqual(len(param), 2)
+                self.assertEqual(len(param), 2)
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_ArgParser.py` & `cat_win-1.4.1/cat_win/tests/test_argparser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,173 @@
 from unittest import TestCase
 import os
 
-from cat_win.const.ArgConstants import *
-import cat_win.util.ArgParser as ArgParser
+from cat_win.const.argconstants import ARGS_CUT, ARGS_REPLACE
+from cat_win.util.argparser import ArgParser
 # import sys
 # sys.path.append('../cat_win')
 
 
 test_file_dir = os.path.join(os.path.dirname(__file__), 'texts')
 
 
-
 class TestArgParser(TestCase):
     maxDiff = None
-    
-    def tearDown(self):
-        ArgParser.FILE_ENCODING = 'utf-8'
-        ArgParser.FILE_MATCH = []
-        ArgParser.FILE_SEARCH = []
-        ArgParser.FILE_TRUNCATE = [None, None, None]
-        
-    def test_getArguments_empty(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT'])
+
+    def test_get_arguments_empty(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT'])
         self.assertCountEqual(args, [])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_duplicate(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', '-n', '-n', '-c'])
+
+    def test_get_arguments_duplicate(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '-n', '-n', '-c'])
         args = list(map(lambda x: x[1], args))
         self.assertCountEqual(args, ['-n', '-c', '-n'])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_concatenated(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', '-abcdef'])
+
+    def test_get_arguments_concatenated(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '-abcef'])
         args = list(map(lambda x: x[1], args))
-        self.assertCountEqual(args, ['-a', '-b', '-c', '-d', '-e', '-f'])
+        self.assertCountEqual(args, ['-a', '-b', '-c', '-e', '-f'])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_concatenated_unknown(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', '-+abcde?fϵg'])
+
+    def test_get_arguments_concatenated_unknown(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '-+abce?fϵg'])
         args = list(map(lambda x: x[1], args))
-        self.assertCountEqual(args, ['-a', '-b', '-c', '-d', '-e', '-f', '-g'])
+        self.assertCountEqual(args, ['-a', '-b', '-c', '-e', '-f', '-g'])
         self.assertCountEqual(unknown_args, ['-+', '-?', '-ϵ'])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_concatenated_invalid(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', '--abcde?fg'])
+
+    def test_get_arguments_concatenated_invalid(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '--abcde?fg'])
         args = list(map(lambda x: x[1], args))
         self.assertCountEqual(args, [])
         self.assertCountEqual(unknown_args, ['--abcde?fg'])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_encoding(self):
-        ArgParser.getArguments(['CAT', 'enc:ascii'])
-        self.assertEqual(ArgParser.FILE_ENCODING, 'ascii')
-        ArgParser.getArguments(['CAT', 'enc=utf-8'])
-        self.assertEqual(ArgParser.FILE_ENCODING, 'utf-8')
-        
-    def test_getArguments_match(self):
-        ArgParser.getArguments(['CAT', 'match:\\Atest\\Z'])
-        self.assertCountEqual(ArgParser.FILE_MATCH, ['\\Atest\\Z'])
-        ArgParser.getArguments(['CAT', 'match=\\Atest\\Z'])
-        self.assertCountEqual(ArgParser.FILE_MATCH, ['\\Atest\\Z'] * 2)
-        
-    def test_getArguments_find(self):
-        ArgParser.getArguments(['CAT', 'find=Test123'])
-        self.assertCountEqual(ArgParser.FILE_SEARCH, ['Test123'])
-        ArgParser.getArguments(['CAT', 'find:Test123'])
-        self.assertCountEqual(ArgParser.FILE_SEARCH, ['Test123'] * 2)
-        
-    def test_getArguments_trunc(self):
-        ArgParser.getArguments(['CAT', 'trunc=0:'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [0, None, None])
-        ArgParser.getArguments(['CAT', 'trunc:1:'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [0, None, None])
-        ArgParser.getArguments(['CAT', 'trunc:2:'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [1, None, None])
-        ArgParser.getArguments(['CAT', 'trunc:::-1'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [None, None, -1])
-        ArgParser.getArguments(['CAT', 'trunc:4::-5'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [3, None, -5])
-        ArgParser.getArguments(['CAT', 'trunc:4:6:-5'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [3, 6, -5])
-        ArgParser.getArguments(['CAT', 'trunc=:2*4-3:'])
-        self.assertListEqual(ArgParser.FILE_TRUNCATE, [None, 5, None])
-        
-    def test_getArguments_cut(self):
-        args, _, _, _, _ = ArgParser.getArguments(['CAT', '[2*5:20]'])
-        self.assertCountEqual(args, [(ARGS_CUT, '[2*5:20]')])
-        
-    def test_getArguments_replace(self):
-        args, _, _, _, _ = ArgParser.getArguments(['CAT', '[test,404]'])
+
+    def test_get_arguments_encoding(self):
+        arg_parser = ArgParser()
+        arg_parser.get_arguments(['CAT', 'enc:ascii'])
+        self.assertEqual(arg_parser.file_encoding, 'ascii')
+        arg_parser.get_arguments(['CAT', 'enc=utf-8'])
+        self.assertEqual(arg_parser.file_encoding, 'utf-8')
+
+    def test_get_arguments_match(self):
+        arg_parser = ArgParser()
+        arg_parser.get_arguments(['CAT', 'match:\\Atest\\Z'])
+        self.assertCountEqual(arg_parser.file_match, set(['\\Atest\\Z']))
+        arg_parser.get_arguments(['CAT', 'match=\\Atest\\Z'])
+        self.assertCountEqual(arg_parser.file_match, set(['\\Atest\\Z']))
+
+    def test_get_arguments_find(self):
+        arg_parser = ArgParser()
+        arg_parser.get_arguments(['CAT', 'find=Test123'])
+        self.assertCountEqual(arg_parser.file_search, set(['Test123']))
+        arg_parser.get_arguments(['CAT', 'find:Test123'])
+        self.assertCountEqual(arg_parser.file_search, set(['Test123']))
+
+    def test_get_arguments_trunc(self):
+        arg_parser = ArgParser()
+        arg_parser.get_arguments(['CAT', 'trunc=0:'])
+        self.assertListEqual(arg_parser.file_truncate, [0, None, None])
+        arg_parser.get_arguments(['CAT', 'trunc:1:'])
+        self.assertListEqual(arg_parser.file_truncate, [0, None, None])
+        arg_parser.get_arguments(['CAT', 'trunc:2:'])
+        self.assertListEqual(arg_parser.file_truncate, [1, None, None])
+        arg_parser.get_arguments(['CAT', 'trunc:::-1'])
+        self.assertListEqual(arg_parser.file_truncate, [None, None, -1])
+        arg_parser.get_arguments(['CAT', 'trunc:4::-5'])
+        self.assertListEqual(arg_parser.file_truncate, [3, None, -5])
+        arg_parser.get_arguments(['CAT', 'trunc:4:6:-5'])
+        self.assertListEqual(arg_parser.file_truncate, [3, 6, -5])
+        arg_parser.get_arguments(['CAT', 'trunc=:2*4-3:'])
+        self.assertListEqual(arg_parser.file_truncate, [None, 5, None])
+
+    def test_get_arguments_cut(self):
+        arg_parser = ArgParser()
+        arg_parser.gen_arguments(['CAT', '[2*5:20]'])
+        self.assertCountEqual(arg_parser.args, [(ARGS_CUT, '[2*5:20]')])
+
+    def test_get_arguments_replace(self):
+        arg_parser = ArgParser()
+        args, _, _, _, _ = arg_parser.get_arguments(['CAT', '[test,404]'])
         self.assertCountEqual(args, [(ARGS_REPLACE, '[test,404]')])
-        
-    def test_getArguments_dir(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', test_file_dir])
+
+    def test_get_arguments_dir(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', test_file_dir])
         self.assertCountEqual(args, [])
         self.assertCountEqual(unknown_args, [])
         self.assertGreaterEqual(len(known_files), 7)
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, [])
-        
-    def test_getArguments_files_equal_dir(self):
-        _, _, known_files_dir, _, _ = ArgParser.getArguments(['CAT', test_file_dir])
-        _, _, known_files_files, _, _ = ArgParser.getArguments(['CAT', test_file_dir + '/**.txt'])
+
+    def test_get_arguments_files_equal_dir(self):
+        arg_parser = ArgParser()
+        _, _, known_files_dir, _, _ = arg_parser.get_arguments(['CAT', test_file_dir])
+        _, _, known_files_files, _, _ = arg_parser.get_arguments(['CAT', test_file_dir + '/**.txt'])
         self.assertCountEqual(known_files_dir, known_files_files)
-        
-    def test_getArguments_unknown_file(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', 'testTesttest', 'test-file.txt'])
+
+    def test_get_arguments_unknown_file(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', 'testTesttest', 'test-file.txt'])
         self.assertCountEqual(args, [])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(echo_args, [])
         self.assertEqual(len(unknown_files), 2)
         self.assertIn('testTesttest', ''.join(unknown_files))
         self.assertIn('test-file.txt', ''.join(unknown_files))
-        
-    def test_getArguments_unknown_args(self):
-        _, unknown_args, _, _, _ = ArgParser.getArguments(['CAT', '--test-file.txt'])
-        self.assertCountEqual(unknown_args, ['--test-file.txt'])
-        
-    def test_getArguments_echo_args(self):
-        args, unknown_args, known_files, unknown_files, echo_args = ArgParser.getArguments(['CAT', '-n', '-E', '-n', 'random', test_file_dir])
+
+    def test_get_arguments_unknown_args(self):
+        arg_parser = ArgParser()
+        arg_parser.gen_arguments(['CAT', '--test-file.txt'])
+        self.assertCountEqual(arg_parser.unknown_args, ['--test-file.txt'])
+
+    def test_get_arguments_echo_args(self):
+        arg_parser = ArgParser()
+        args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '-n', '-E', '-n', 'random', test_file_dir])
         args = list(map(lambda x: x[1], args))
         self.assertCountEqual(args, ['-n', '-E'])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, ['-n', 'random', test_file_dir])
-        
-    def test_getArguments_echo_args_recursive(self):
-        args = []
-        echo = ArgParser.__addArgument__(args, [], [], [], '-nEn')
-        args = list(map(lambda x: x[1], args))
+
+    def test_get_arguments_echo_args_recursive(self):
+        arg_parser = ArgParser()
+        echo = arg_parser._add_argument('-nEn')
+        args = list(map(lambda x: x[1], arg_parser.args))
         self.assertCountEqual(args, ['-n', '-E'])
-        self.assertEqual(echo, True)
+        self.assertEqual(echo, True)
+
+    def test_delete_queried(self):
+        arg_parser = ArgParser()
+        arg_parser._add_argument('find=hello')
+        arg_parser._add_argument('find=world')
+        self.assertSetEqual(arg_parser.file_search, set(['hello', 'world']))
+        arg_parser._add_argument('find=hello', True)
+        self.assertSetEqual(arg_parser.file_search, set(['world']))
+
+        arg_parser._add_argument('match=[a-z]')
+        arg_parser._add_argument('match=[0-9]')
+        self.assertSetEqual(arg_parser.file_match, set(['[a-z]', '[0-9]']))
+        arg_parser._add_argument('match=[0-9]', True)
+        self.assertSetEqual(arg_parser.file_match, set(['[a-z]']))
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_Base64.py` & `cat_win-1.4.1/cat_win/tests/test_cbase64.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from unittest import TestCase
 
-from cat_win.util.Base64 import encodeBase64, decodeBase64
+from cat_win.util.cbase64 import encode_base64, decode_base64
 # import sys
 # sys.path.append('../cat_win')
 
 
 class TestBase64(TestCase):
-    def test_encodeBase64(self):
+    def test_encode_base64(self):
         test_input = [('', 'Test'),
                       ('', '123404'),
                       ('', 'ÄÖÜ  TEST')]
         expected_output = [('', 'VGVzdAoxMjM0MDQKw4TDlsOcICBURVNU')]
-        self.assertEqual(encodeBase64(test_input), expected_output)
+        self.assertEqual(encode_base64(test_input), expected_output)
 
-    def test_decodeBase64(self):
+    def test_decode_base64(self):
         test_input = [('', 'VGVzdAoxMjM0MDQKw4TDlsOcICBURVNU')]
         expected_output = [('', 'Test'),
                            ('', '123404'),
                            ('', 'ÄÖÜ  TEST')]
-        self.assertEqual(decodeBase64(test_input), expected_output)
+        self.assertEqual(decode_base64(test_input), expected_output)
 
-    def test_decodeBase64_lineBreak(self):
+    def test_decode_base64_linebreak(self):
         test_input = [('', 'VGVzdAoxMjM0MDQKw4'),
                       ('', 'TDlsOcICBURVNU')]
         expected_output = [('', 'Test'),
                            ('', '123404'),
                            ('', 'ÄÖÜ  TEST')]
-        self.assertEqual(decodeBase64(test_input), expected_output)
-
-# python -m unittest discover -s tests -p test*.py
+        self.assertEqual(decode_base64(test_input), expected_output)
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_Converter.py` & `cat_win-1.4.1/cat_win/tests/test_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 from unittest import TestCase
 
-from cat_win.util.Converter import Converter
+from cat_win.util.converter import Converter
 # import sys
 # sys.path.append('../cat_win')
 
 
 converter = Converter()
 
 
 class TestConverter(TestCase):
     def test_converter_dec(self):
         expected_output = '{Hexadecimal: 0x3039; Binary: 0b11000000111001}'
-        self.assertEqual(converter._fromDEC(12345, True), expected_output)
+        self.assertEqual(converter.c_from_dec(12345, True), expected_output)
 
         expected_output = '{Hexadecimal: 3039; Binary: 11000000111001}'
-        self.assertEqual(converter._fromDEC(12345, False), expected_output)
+        self.assertEqual(converter.c_from_dec(12345, False), expected_output)
 
     def test_converter_hex(self):
         expected_output = '{Decimal: 12345; Binary: 0b11000000111001}'
-        self.assertEqual(converter._fromHEX('0x3039', True), expected_output)
+        self.assertEqual(converter.c_from_hex('0x3039', True), expected_output)
 
         expected_output = '{Decimal: 12345; Binary: 11000000111001}'
-        self.assertEqual(converter._fromHEX('0x3039', False), expected_output)
+        self.assertEqual(converter.c_from_hex('0x3039', False), expected_output)
 
         expected_output = '{Decimal: 12345; Binary: 0b11000000111001}'
-        self.assertEqual(converter._fromHEX('3039', True), expected_output)
+        self.assertEqual(converter.c_from_hex('3039', True), expected_output)
 
         expected_output = '{Decimal: 12345; Binary: 11000000111001}'
-        self.assertEqual(converter._fromHEX('3039', False), expected_output)
+        self.assertEqual(converter.c_from_hex('3039', False), expected_output)
 
     def test_converter_bin(self):
         expected_output = '{Decimal: 12345; Hexadecimal: 0x3039}'
-        self.assertEqual(converter._fromBIN(
+        self.assertEqual(converter.c_from_bin(
             '0b11000000111001', True), expected_output)
 
         expected_output = '{Decimal: 12345; Hexadecimal: 3039}'
-        self.assertEqual(converter._fromBIN(
+        self.assertEqual(converter.c_from_bin(
             '0b11000000111001', False), expected_output)
 
         expected_output = '{Decimal: 12345; Hexadecimal: 0x3039}'
-        self.assertEqual(converter._fromBIN(
+        self.assertEqual(converter.c_from_bin(
             '11000000111001', True), expected_output)
 
         expected_output = '{Decimal: 12345; Hexadecimal: 3039}'
-        self.assertEqual(converter._fromBIN(
+        self.assertEqual(converter.c_from_bin(
             '11000000111001', False), expected_output)
-        
+
     def test_empty_input(self):
         expected_output = False
         self.assertEqual(converter.is_dec(''), expected_output)
         self.assertEqual(converter.is_hex(''), expected_output)
         self.assertEqual(converter.is_bin(''), expected_output)
-        
+
     def test_correct_input(self):
         expected_output = True
         self.assertEqual(converter.is_dec('1'), expected_output)
         self.assertEqual(converter.is_dec('-1'), expected_output)
         self.assertEqual(converter.is_dec('999'), expected_output)
-        
+
         self.assertEqual(converter.is_hex('1'), expected_output)
         self.assertEqual(converter.is_hex('-1'), expected_output)
         self.assertEqual(converter.is_hex('999'), expected_output)
         self.assertEqual(converter.is_hex('0x999'), expected_output)
         self.assertEqual(converter.is_hex('-0x999'), expected_output)
-        
+
         self.assertEqual(converter.is_bin('1'), expected_output)
         self.assertEqual(converter.is_bin('-1'), expected_output)
         self.assertEqual(converter.is_bin('0101'), expected_output)
         self.assertEqual(converter.is_bin('0b0101'), expected_output)
         self.assertEqual(converter.is_bin('-0b0101'), expected_output)
-        
+
     def test_wrong_input(self):
         expected_output = False
         self.assertEqual(converter.is_dec('0x1'), expected_output)
         self.assertEqual(converter.is_dec('1.5'), expected_output)
-        
+
         self.assertEqual(converter.is_hex('FG'), expected_output)
         self.assertEqual(converter.is_hex('0x-999'), expected_output)
-        
+
         self.assertEqual(converter.is_bin('2'), expected_output)
         self.assertEqual(converter.is_bin('0x1'), expected_output)
-
-# python -m unittest discover -s tests -p test*.py
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_RawViewer.py` & `cat_win-1.4.1/cat_win/tests/test_rawviewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 from unittest import TestCase
 import os
 
-from cat_win.util.RawViewer import getRawViewLinesGen
+from cat_win.util.rawviewer import get_raw_view_lines_gen
 
 
 test_file_path = os.path.join(os.path.dirname(__file__), 'texts', 'test.txt')
 
 
 class TestRawViewer(TestCase):
     maxDiff = None
-    
-    def testModeX(self):
+
+    def test_mode_x_upper(self):
         expected_result = """Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   
 00000000 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 69 73 20 69 73 20 61 20 54 61 62 2D 43 68 61 72 # i s   i s   a   T a b - C h a r
 00000020 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 65 20 61 72 65 20 53 70 65 63 69 61 6C 20 43 68 # e   a r e   S p e c i a l   C h
 00000040 61 72 73 3A 20 C3 A4 C3 B6 C3 BC C3 84 C3 96 C3 # a r s :   · · · · · · · · · · ·
 00000050 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 # · ␍ ␤ N - A r y   S u m m a t i
 00000060 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C # o n :   · · · ␍ ␤ T h e   f o l
 00000070 6C 6F 77 69 6E 67 20 4C 69 6E 65 20 69 73 20 45 # l o w i n g   L i n e   i s   E
 00000080 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 6E 65 20 69 73 20 61 20 44 75 70 6C 69 63 61 74 # n e   i s   a   D u p l i c a t
 000000A0 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 20 61 20 44 75 70 6C 69 63 61 74 65 21          #   a   D u p l i c a t e !"""
-    
-        self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'X')), expected_result)
-        
-    def testModex(self):
+
+        self.assertEqual('\n'.join(get_raw_view_lines_gen(test_file_path, 'X')), expected_result)
+
+    def test_mode_x(self):
         expected_result = """Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   
 00000000 53 61 6d 70 6c 65 20 54 65 78 74 3a 0d 0a 54 68 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 69 73 20 69 73 20 61 20 54 61 62 2d 43 68 61 72 # i s   i s   a   T a b - C h a r
 00000020 61 63 74 65 72 3a 20 3e 09 3c 0d 0a 54 68 65 73 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 65 20 61 72 65 20 53 70 65 63 69 61 6c 20 43 68 # e   a r e   S p e c i a l   C h
 00000040 61 72 73 3a 20 c3 a4 c3 b6 c3 bc c3 84 c3 96 c3 # a r s :   · · · · · · · · · · ·
 00000050 9c 0d 0a 4e 2d 41 72 79 20 53 75 6d 6d 61 74 69 # · ␍ ␤ N - A r y   S u m m a t i
 00000060 6f 6e 3a 20 e2 88 91 0d 0a 54 68 65 20 66 6f 6c # o n :   · · · ␍ ␤ T h e   f o l
 00000070 6c 6f 77 69 6e 67 20 4c 69 6e 65 20 69 73 20 45 # l o w i n g   L i n e   i s   E
 00000080 6d 70 74 79 3a 0d 0a 0d 0a 54 68 69 73 20 4c 69 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 6e 65 20 69 73 20 61 20 44 75 70 6c 69 63 61 74 # n e   i s   a   D u p l i c a t
 000000A0 65 21 0d 0a 54 68 69 73 20 4c 69 6e 65 20 69 73 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 20 61 20 44 75 70 6c 69 63 61 74 65 21          #   a   D u p l i c a t e !"""
-    
-        self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'x')), expected_result)
-        
-    def testModeb(self):
+
+        self.assertEqual('\n'.join(get_raw_view_lines_gen(test_file_path, 'x')), expected_result)
+
+    def test_mode_b(self):
         expected_result = """Address  00       01       02       03       04       05       06       07       08       09       0A       0B       0C       0D       0E       0F       # Decoded Text                   
 00000000 01010011 01100001 01101101 01110000 01101100 01100101 00100000 01010100 01100101 01111000 01110100 00111010 00001101 00001010 01010100 01101000 # S a m p l e   T e x t : ␍ ␤ T h
 00000010 01101001 01110011 00100000 01101001 01110011 00100000 01100001 00100000 01010100 01100001 01100010 00101101 01000011 01101000 01100001 01110010 # i s   i s   a   T a b - C h a r
 00000020 01100001 01100011 01110100 01100101 01110010 00111010 00100000 00111110 00001001 00111100 00001101 00001010 01010100 01101000 01100101 01110011 # a c t e r :   > · < ␍ ␤ T h e s
 00000030 01100101 00100000 01100001 01110010 01100101 00100000 01010011 01110000 01100101 01100011 01101001 01100001 01101100 00100000 01000011 01101000 # e   a r e   S p e c i a l   C h
 00000040 01100001 01110010 01110011 00111010 00100000 11000011 10100100 11000011 10110110 11000011 10111100 11000011 10000100 11000011 10010110 11000011 # a r s :   · · · · · · · · · · ·
 00000050 10011100 00001101 00001010 01001110 00101101 01000001 01110010 01111001 00100000 01010011 01110101 01101101 01101101 01100001 01110100 01101001 # · ␍ ␤ N - A r y   S u m m a t i
 00000060 01101111 01101110 00111010 00100000 11100010 10001000 10010001 00001101 00001010 01010100 01101000 01100101 00100000 01100110 01101111 01101100 # o n :   · · · ␍ ␤ T h e   f o l
 00000070 01101100 01101111 01110111 01101001 01101110 01100111 00100000 01001100 01101001 01101110 01100101 00100000 01101001 01110011 00100000 01000101 # l o w i n g   L i n e   i s   E
 00000080 01101101 01110000 01110100 01111001 00111010 00001101 00001010 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 # m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 00000090 01101110 01100101 00100000 01101001 01110011 00100000 01100001 00100000 01000100 01110101 01110000 01101100 01101001 01100011 01100001 01110100 # n e   i s   a   D u p l i c a t
 000000A0 01100101 00100001 00001101 00001010 01010100 01101000 01101001 01110011 00100000 01001100 01101001 01101110 01100101 00100000 01101001 01110011 # e ! ␍ ␤ T h i s   L i n e   i s
 000000B0 00100000 01100001 00100000 01000100 01110101 01110000 01101100 01101001 01100011 01100001 01110100 01100101 00100001                            #   a   D u p l i c a t e !"""
-    
-        self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'b')), expected_result)
-        
-    def testModeXColored(self):
+
+        self.assertEqual('\n'.join(get_raw_view_lines_gen(test_file_path, 'b')), expected_result)
+
+    def test_mode_x_upper_colored(self):
         expected_result = """*Address  00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F # Decoded Text                   !
 *00000000! 53 61 6D 70 6C 65 20 54 65 78 74 3A 0D 0A 54 68 *#! S a m p l e   T e x t : ␍ ␤ T h
 *00000010! 69 73 20 69 73 20 61 20 54 61 62 2D 43 68 61 72 *#! i s   i s   a   T a b - C h a r
 *00000020! 61 63 74 65 72 3A 20 3E 09 3C 0D 0A 54 68 65 73 *#! a c t e r :   > · < ␍ ␤ T h e s
 *00000030! 65 20 61 72 65 20 53 70 65 63 69 61 6C 20 43 68 *#! e   a r e   S p e c i a l   C h
 *00000040! 61 72 73 3A 20 C3 A4 C3 B6 C3 BC C3 84 C3 96 C3 *#! a r s :   · · · · · · · · · · ·
 *00000050! 9C 0D 0A 4E 2D 41 72 79 20 53 75 6D 6D 61 74 69 *#! · ␍ ␤ N - A r y   S u m m a t i
 *00000060! 6F 6E 3A 20 E2 88 91 0D 0A 54 68 65 20 66 6F 6C *#! o n :   · · · ␍ ␤ T h e   f o l
 *00000070! 6C 6F 77 69 6E 67 20 4C 69 6E 65 20 69 73 20 45 *#! l o w i n g   L i n e   i s   E
 *00000080! 6D 70 74 79 3A 0D 0A 0D 0A 54 68 69 73 20 4C 69 *#! m p t y : ␍ ␤ ␍ ␤ T h i s   L i
 *00000090! 6E 65 20 69 73 20 61 20 44 75 70 6C 69 63 61 74 *#! n e   i s   a   D u p l i c a t
 *000000A0! 65 21 0D 0A 54 68 69 73 20 4C 69 6E 65 20 69 73 *#! e ! ␍ ␤ T h i s   L i n e   i s
 *000000B0! 20 61 20 44 75 70 6C 69 63 61 74 65 21          *#!   a   D u p l i c a t e !"""
-    
-        self.assertEqual('\n'.join(getRawViewLinesGen(test_file_path, 'X', ['*', '!'])), expected_result)
+
+        self.assertEqual('\n'.join(get_raw_view_lines_gen(test_file_path, 'X', ['*', '!'])), expected_result)
+
+    def test_encoding_error(self):
+        result = '\n'.join(get_raw_view_lines_gen(test_file_path, 'X', None, 'utf-16'))
+
+        self.assertNotIn('␍', result)
+        self.assertNotIn('␤', result)
+        self.assertIn('·', result)
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_UpdateChecker.py` & `cat_win-1.4.1/cat_win/tests/test_updatechecker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 from unittest import TestCase
 
-import cat_win.web.UpdateChecker as UpdateChecker
+from cat_win.web import updatechecker
 # import sys
 # sys.path.append('../cat_win')
 
 
 class TestUpdateChecker(TestCase):
-    def test_onlyNumeric(self):
-        self.assertEqual(UpdateChecker.onlyNumeric('1nh589h15io125b085218'), 158915125085218)
-        self.assertEqual(UpdateChecker.onlyNumeric('1nh'), 1)
-        self.assertEqual(UpdateChecker.onlyNumeric('123'), 123)
-        self.assertEqual(UpdateChecker.onlyNumeric('abc'), 0)
-    
-    def test_genVersionTuples(self):
-        self.assertEqual(UpdateChecker.genVersionTuples('1.0.33.0', '1.1.0a'),
+    def test_only_numeric(self):
+        self.assertEqual(updatechecker.only_numeric('1nh589h15io125b085218'), 158915125085218)
+        self.assertEqual(updatechecker.only_numeric('1nh'), 1)
+        self.assertEqual(updatechecker.only_numeric('123'), 123)
+        self.assertEqual(updatechecker.only_numeric('abc'), 0)
+
+    def test_gen_version_tuples(self):
+        self.assertEqual(updatechecker.gen_version_tuples('1.0.33.0', '1.1.0a'),
                          (('01', '00', '33', '00'), ('01', '01', '0a', '00')))
-        self.assertEqual(UpdateChecker.genVersionTuples('1.2.3', '1.2.3.4.5'),
+        self.assertEqual(updatechecker.gen_version_tuples('1.2.3', '1.2.3.4.5'),
                          (('1', '2', '3', '0', '0'), ('1', '2', '3', '4', '5')))
-        self.assertEqual(UpdateChecker.genVersionTuples('1.12345', '1.2'),
+        self.assertEqual(updatechecker.gen_version_tuples('1.12345', '1.2'),
                          (('00001', '12345'), ('00001', '00002')))
-    
+
     def test_version_comparison_up_to_date(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.0.9'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.0.09'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.10.9', 'v1.10.9'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.7a.9', '1.7a.9'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('09.0.8b', '9.0.08b'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('v7b.4', '07b.04.00'), 0)
-        self.assertEqual(UpdateChecker.newVersionAvailable('9', '9.0.0'), 0)
-        
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.0.9'), 0)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.0.09'), 0)
+        self.assertEqual(updatechecker.new_version_available('1.10.9', 'v1.10.9'), 0)
+        self.assertEqual(updatechecker.new_version_available('1.7a.9', '1.7a.9'), 0)
+        self.assertEqual(updatechecker.new_version_available('09.0.8b', '9.0.08b'), 0)
+        self.assertEqual(updatechecker.new_version_available('v7b.4', '07b.04.00'), 0)
+        self.assertEqual(updatechecker.new_version_available('9', '9.0.0'), 0)
+
     def test_version_comparison_stable_release(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.0.10'), 1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.15', 'v1.0.016'), 1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.12', '1.000.020'), 1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.0.0', 'v01.00.01'), 1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('2.1.5a', '2.1.6'), 1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('v2.1b.5a', '2.1b.051'), 1)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.0.10'), 1)
+        self.assertEqual(updatechecker.new_version_available('1.0.15', 'v1.0.016'), 1)
+        self.assertEqual(updatechecker.new_version_available('1.0.12', '1.000.020'), 1)
+        self.assertEqual(updatechecker.new_version_available('v1.0.0', 'v01.00.01'), 1)
+        self.assertEqual(updatechecker.new_version_available('2.1.5a', '2.1.6'), 1)
+        self.assertEqual(updatechecker.new_version_available('v2.1b.5a', '2.1b.051'), 1)
 
     def test_version_comparison_pre_release(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.0.9', '1.0.9a'), 2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.0.09b'), 2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', 'v1.0.10b'), 2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('2.1.5a', '2.1.5b'), 2)
-    
+        self.assertEqual(updatechecker.new_version_available('v1.0.9', '1.0.9a'), 2)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.0.09b'), 2)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', 'v1.0.10b'), 2)
+        self.assertEqual(updatechecker.new_version_available('2.1.5a', '2.1.5b'), 2)
+
     def test_version_comparison_stable_release_unsafe(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.01.10'), -1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.15', '1.1.9'), -1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', 'v2.0.9'), -1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.12', '1.001.0'), -1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.0.0', 'v01.001.01'), -1)
-        self.assertEqual(UpdateChecker.newVersionAvailable('2.1.5a', '2.2.5'), -1)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.01.10'), -1)
+        self.assertEqual(updatechecker.new_version_available('1.0.15', '1.1.9'), -1)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', 'v2.0.9'), -1)
+        self.assertEqual(updatechecker.new_version_available('1.0.12', '1.001.0'), -1)
+        self.assertEqual(updatechecker.new_version_available('v1.0.0', 'v01.001.01'), -1)
+        self.assertEqual(updatechecker.new_version_available('2.1.5a', '2.2.5'), -1)
 
     def test_version_comparison_pre_release_unsafe(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.0.9', '1a.0.9a'), -2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '1.0a.9'), -2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', 'v1a.0.9'), -2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('1.0.9', '2b.0.10b'), -2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.0.9', '1.0b.10'), -2)
-        self.assertEqual(UpdateChecker.newVersionAvailable('2.1.5a', '2.1a.5'), -2)
-        
-    def test_version_availability_current_is_newest(self):
-        self.assertEqual(UpdateChecker.newVersionAvailable('v1.1.9', '1.0.9a'), 0)
+        self.assertEqual(updatechecker.new_version_available('v1.0.9', '1a.0.9a'), -2)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '1.0a.9'), -2)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', 'v1a.0.9'), -2)
+        self.assertEqual(updatechecker.new_version_available('1.0.9', '2b.0.10b'), -2)
+        self.assertEqual(updatechecker.new_version_available('v1.0.9', '1.0b.10'), -2)
+        self.assertEqual(updatechecker.new_version_available('2.1.5a', '2.1a.5'), -2)
 
-# python -m unittest discover -s tests -p test*.py
+    def test_version_availability_current_is_newest(self):
+        self.assertEqual(updatechecker.new_version_available('v1.1.9', '1.0.9a'), 0)
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_checksum.py` & `cat_win-1.4.1/cat_win/tests/test_checksum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 import os
 
-from cat_win.util.checksum import getChecksumFromFile
+from cat_win.util.checksum import get_checksum_from_file
 # import sys
 # sys.path.append('../cat_win')
 
 
 test_file_path = os.path.join(os.path.dirname(__file__), 'texts', 'test.txt')
 
 
@@ -13,19 +13,17 @@
     def test_checksum(self):
         expected_output = ''
         expected_output += '\tCRC32:   C7222F64\n'
         expected_output += '\tMD5:     0f85f8d2b6783c06d40755ab54906862\n'
         expected_output += '\tSHA1:    1c50f01c5be5fc4795817e14f5deccbd51bf0934\n'
         expected_output += '\tSHA256:  dfb46efd198ad4b1204308c2be1c5e0254effe0de3ed314dea394cafdfd1749f\n'
         expected_output += '\tSHA512:  bf35256e790288a6dbf93b7327e1f97840349e0490b48848273663d34ad493e73a325df6725d7b0d5eb680d751bfe3cc49bd82ce9e8527412ce2cc8355a391a1\n'
-        self.assertEqual(getChecksumFromFile(test_file_path), expected_output)
-        
+        self.assertEqual(get_checksum_from_file(test_file_path), expected_output)
+
     def test_checksum_colored(self):
         expected_output = ''
         expected_output += '\tXCRC32:   C7222F64Y\n'
         expected_output += '\tXMD5:     0f85f8d2b6783c06d40755ab54906862Y\n'
         expected_output += '\tXSHA1:    1c50f01c5be5fc4795817e14f5deccbd51bf0934Y\n'
         expected_output += '\tXSHA256:  dfb46efd198ad4b1204308c2be1c5e0254effe0de3ed314dea394cafdfd1749fY\n'
         expected_output += '\tXSHA512:  bf35256e790288a6dbf93b7327e1f97840349e0490b48848273663d34ad493e73a325df6725d7b0d5eb680d751bfe3cc49bd82ce9e8527412ce2cc8355a391a1Y\n'
-        self.assertEqual(getChecksumFromFile(test_file_path, ['X', 'Y']), expected_output)
-
-# python -m unittest discover -s tests -p test*.py
+        self.assertEqual(get_checksum_from_file(test_file_path, ['X', 'Y']), expected_output)
```

### Comparing `cat_win-1.4.0/cat_win/tests/test_full.py` & `cat_win-1.4.1/cat_win/tests/test_full.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,145 +1,126 @@
-from io import StringIO
 from unittest.mock import patch
 from unittest import TestCase
 import os
 
-import cat_win.cat as cat
-import cat_win.util.ArgParser as ArgParser
-
+from cat_win import cat
+from cat_win.tests.mocks.std import StdInMock, StdOutMock
+from cat_win.util.argparser import ArgParser
 # import sys
 # sys.path.append('../cat_win')
 
+
 test_file_dir = os.path.join(os.path.dirname(__file__), 'texts')
 test_file_path  = os.path.join(test_file_dir, 'test.txt')
 test_empty_path = os.path.join(test_file_dir, 'test_empty.txt')
 test_peek       = os.path.join(test_file_dir, 'test_peek.txt')
 test_result_B   = os.path.join(test_file_dir, 'full_test_result_B.txt')
 test_result_C   = os.path.join(test_file_dir, 'full_test_result_C.txt')
 test_result_D   = os.path.join(test_file_dir, 'full_test_result_D.txt')
 
 
-class StdOutMock(StringIO):
-    def reconfigure(self, encoding = None) -> None:
-        return
-
-    def fileno(self) -> int:
-        return 0
-    
-# class StdInMock(DontReadFromInput):
-class StdInMock:
-    def reconfigure(self, encoding = None) -> None:
-        return
-    
-    def readline(self) -> str:
-        return ''
-
-
 @patch('cat_win.cat.sys.stdin', StdInMock())
 class TestCatFull(TestCase):
     maxDiff = None
 
     def tearDown(self):
-        cat._CalculateLinePrefixSpacing.cache_clear()
-        cat._CalculateLineLengthPrefixSpacing.cache_clear()
-        ArgParser.FILE_ENCODING = 'utf-8'
-        ArgParser.FILE_SEARCH = []
-        ArgParser.FILE_MATCH = []
-        ArgParser.FILE_TRUNCATE = [None, None, None]
+        cat._calculate_line_prefix_spacing.cache_clear()
+        cat._calculate_line_length_prefix_spacing.cache_clear()
+        cat.arg_parser = ArgParser()
         for i in range(len(cat.holder.args_id)):
             cat.holder.args_id[i] = False
-    
+
     # no files parsed
     @patch('cat_win.cat.sys.argv', ['<CAT>', '-ln', '--nc', '[::-2]', 'enc=utf8'])
-    def test_cat_output_full_A(self):
+    def test_cat_output_full_a(self):
         expected_output = ''
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, '-ln', '--nc', '[::-2]', 'enc=utf8'])
-    def test_cat_output_full_B(self):
+    def test_cat_output_full_b(self):
         expected_output = ''
         with open(test_result_B, 'r', encoding='utf-8') as output:
             expected_output = output.read()
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc:UTF-8', test_file_path, '-ub', '[Sample,TEST]', '--nc', '-le'])
-    def test_cat_output_full_C(self):
+    def test_cat_output_full_c(self):
         expected_output = ''
         with open(test_result_C, 'r', encoding='utf-8') as output:
             expected_output = output.read()
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc=utf-8', test_file_path, 'trunc=2:6', '-n', '--reverse', '--nc', '-t'])
-    def test_cat_output_full_D(self):
+    def test_cat_output_full_d(self):
         expected_output = ''
         with open(test_result_D, 'r', encoding='utf-8') as output:
             expected_output = output.read()
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'trunc=0:0',])
     def test_cat_output_full_empty(self):
         expected_output = ''
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=cp1252', '--nc'])
-    def test_cat_output_full_Cp1252(self):
+    def test_cat_output_full_cp1252(self):
         expected_output = ''
         with open(test_file_path, 'r', encoding='cp1252') as output:
             expected_output = output.read() + '\n'
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=latin_1', '--nc'])
-    def test_cat_output_full_Latin1(self):
+    def test_cat_output_full_latin1(self):
         expected_output = ''
         with open(test_file_path, 'r', encoding='latin_1') as output:
             expected_output = output.read() + '\n'
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=ple ', 'match=:', '--nc'])
     def test_cat_output_full_find_found(self):
         expected_output = "Sample Text:\n--------------- Found [('ple ', [3, 7])] ---------------\n--------------- Matched [(':', [11, 12])] ---------------\n"
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=NOTINLINE', '--nc'])
     def test_cat_output_full_find_not_found(self):
         expected_output = 'Sample Text:\n'
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=Text', '--nc', '--nk'])
     def test_cat_output_full_find_found_nokeyword(self):
         expected_output = ''
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'find=Text', '--nc', '--grep'])
     def test_cat_output_full_find_found_grep(self):
         expected_output = 'Sample Text:\n'
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
+
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_peek, 'enc=utf-8', '--peek'])
     def test_cat_output_full_peek(self):
         expected_output = """1
 2
 3
 4
 5
@@ -148,13 +129,12 @@
            •
 6
 7
 8
 9
 10
 """
-        with patch('sys.stdout', new=StdOutMock()) as fake_out:
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
-            
 
-# python -m unittest discover -s tests -p test*.py
+# python -m unittest discover -s cat_win.tests -p test*.py
```

### Comparing `cat_win-1.4.0/cat_win/util/Base64.py` & `cat_win-1.4.1/cat_win/util/cbase64.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 from base64 import b64encode, b64decode
 
 
-def _encodeBase64(content: str, encoding: str) -> bytes:
+def _encode_base64(content: str, encoding: str) -> bytes:
     """
     Encode a string to base64.
     
     Parameters:
     content (str):
         the string to encode
     encoding (str):
         the encoding the string is using
         
     Returns:
     encoded_content (bytes):
         the base64 encoded string
     """
     # encode the string to bytes and encode with base64
-    contentBytes = content.encode(encoding=encoding)
-    encoded_content = b64encode(contentBytes)
-    
+    content_bytes = content.encode(encoding=encoding)
+    encoded_content = b64encode(content_bytes)
+
     # return as a single line
     return encoded_content
 
 
-def encodeBase64(content: list, encoding: str = 'utf-8') -> list:
+def encode_base64(content: list, encoding: str = 'utf-8') -> list:
     """
-    Encode the file content to base64 by calling _encodeBase64()
+    Encode the file content to base64 by calling _encode_base64()
     
     Parameters:
     content (list):
         the file content represented as [(prefix, line), ...]
     encoding (str):
         the file encoding used
         
     Returns:
     [('', encoded_content)] (list):
         the encoded base64 content as a single line without any prefix
     """
     # concatenate all lines and join them with line breaks
-    contentLines = list(map(lambda x: x[1], content))
-    contentLine = '\n'.join(contentLines)
-    
-    encoded_content = _encodeBase64(contentLine, encoding)
+    content_lines = list(map(lambda x: x[1], content))
+    content_line = '\n'.join(content_lines)
+
+    encoded_content = _encode_base64(content_line, encoding)
     encoded_content = encoded_content.decode(encoding='ascii')
     # return as a list containing a single line
     return [('', encoded_content)]
 
 
-def _decodeBase64(content: str) -> bytes:
+def _decode_base64(content: str) -> bytes:
     """
     Decode a string from base64.
     
     Parameters:
     content (str):
         the string to decode
         
     Returns:
     decoded_content (bytes):
         the base64 decoded string
     """
     # encode the string to bytes and decode with base64
     base64_bytes = content.encode(encoding='ascii')
     decoded_content = b64decode(base64_bytes)
-    
+
     # return as a single line
     return decoded_content
 
 
-def decodeBase64(content: list, encoding: str = 'utf-8') -> list:
+def decode_base64(content: list, encoding: str = 'utf-8') -> list:
     """
-    decode the file content from base64 by calling _decodeBase64()
+    decode the file content from base64 by calling _decode_base64()
     
     Parameters:
     content (list):
         the file content represented as [(prefix, line), ...]
     encoding (str):
         the file encoding used
         
     Returns:
     [('', line), ...] (list):
         the decoded base64 content line by line without any prefix
     """
     # concatenate all lines and join them
-    contentLines = list(map(lambda x: x[1], content))
-    contentLine = ''.join(contentLines)
-    
-    decoded_content = _decodeBase64(contentLine)
+    content_lines = list(map(lambda x: x[1], content))
+    content_line = ''.join(content_lines)
+
+    decoded_content = _decode_base64(content_line)
     decoded_content = decoded_content.decode(encoding=encoding)
-    
+
     # return as content list, split at line breaks
     decoded_content = decoded_content.split('\n')
     return [('', line) for line in decoded_content]
```

### Comparing `cat_win-1.4.0/cat_win/util/Converter.py` & `cat_win-1.4.1/cat_win/util/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,97 @@
 import string
 
 
 class Converter():
-    def is_dec(self, v: str) -> bool:
+    """
+    converts a decimal, hex, binary number
+    to the two corresponding others.
+    """
+    def is_dec(self, _v: str) -> bool:
         """
         Parameters:
         v (str):
             the string to check
             
         Returns:
             True if v is a Decimal number.
             False if it is not.
         """
-        if v[:1] == '-':
-            v = v[1:]
-        return v.isdecimal() and v != ""
+        if _v[:1] == '-':
+            _v = _v[1:]
+        return _v.isdecimal() and _v != ""
 
-    def is_hex(self, v: str) -> bool:
+    def is_hex(self, _v: str) -> bool:
         """
         Parameters:
         v (str):
             the string to check
             
         Returns:
             True if v is a Hexadecimal number.
             False if it is not.
         """
-        if v[:1] == '-':
-            v = v[1:]
+        if _v[:1] == '-':
+            _v = _v[1:]
         hex_digits = set(string.hexdigits)
-        if v[:2] == '0x':
-            v = v[2:]
-        return all(c in hex_digits for c in v) and v != ""
+        if _v[:2] == '0x':
+            _v = _v[2:]
+        return all(c in hex_digits for c in _v) and _v != ""
 
-    def is_bin(self, v: str) -> bool:
+    def is_bin(self, _v: str) -> bool:
         """
         Parameters:
         v (str):
             the string to check
             
         Returns:
             True if v is a Binary number.
             False if it is not.
         """
-        if v[:1] == '-':
-            v = v[1:]
-        if v[:2] == '0b':
-            v = v[2:]
-        v_set = set(v)
-        return (v_set == {'0', '1'} or v_set == {'0'} or v_set == {'1'}) and v != ""
+        if _v[:1] == '-':
+            _v = _v[1:]
+        if _v[:2] == '0b':
+            _v = _v[2:]
+        v_set = set(_v)
+        return v_set in [{'0', '1'}, {'0'}, {'1'}] and _v != ""
 
     def __dec_to_hex__(self, value: int, leading: bool = False) -> str:
-        return '{0:#x}'.format(value) if leading else '{0:x}'.format(value)
+        return f"{value:#x}" if leading else f"{value:x}"
 
     def __dec_to_bin__(self, value: int, leading: bool = False) -> str:
-        return '{0:#b}'.format(value) if leading else '{0:b}'.format(value)
+        return f"{value:#b}" if leading else f"{value:b}"
 
-    def _fromDEC(self, value: int, leading: bool = False) -> str:
+    def c_from_dec(self, value: int, leading: bool = False) -> str:
         """
         returns a String representation of a Decimal Int including the corresponding
         Hexadecimal and Binary number.
         """
-        return '{Hexadecimal: ' + self.__dec_to_hex__(value, leading) + '; Binary: ' + self.__dec_to_bin__(value, leading) + '}'
+        return '{Hexadecimal: ' + self.__dec_to_hex__(value, leading) + '; Binary: ' + \
+            self.__dec_to_bin__(value, leading) + '}'
 
     def __hex_to_dec__(self, value: str) -> str:
         return str(int(value, 16))
 
     def __hex_to_bin__(self, value: str, leading: bool = False) -> str:
         return bin(int(value, 16)) if leading else bin(int(value, 16))[2:]
 
-    def _fromHEX(self, value: str, leading: bool = False) -> str:
+    def c_from_hex(self, value: str, leading: bool = False) -> str:
         """
         returns a String representation of a Hexadecimal String including the corresponding
         Decimal and Binary number.
         """
-        return '{Decimal: ' + self.__hex_to_dec__(value) + '; Binary: ' + self.__hex_to_bin__(value, leading) + '}'
+        return '{Decimal: ' + self.__hex_to_dec__(value) + '; Binary: ' + \
+            self.__hex_to_bin__(value, leading) + '}'
 
     def __bin_to_dec__(self, value: str) -> str:
         return str(int(value, 2))
 
     def __bin_to_hex__(self, value: str, leading: bool = False) -> str:
         return hex(int(value, 2)) if leading else hex(int(value, 2))[2:]
 
-    def _fromBIN(self, value: str, leading: bool = False) -> str:
+    def c_from_bin(self, value: str, leading: bool = False) -> str:
         """
         returns a String representation of a Binary String including the corresponding
         Decimal and Hexadecimal number.
         """
-        return '{Decimal: ' + self.__bin_to_dec__(value) + '; Hexadecimal: ' + self.__bin_to_hex__(value, leading) + '}'
+        return '{Decimal: ' + self.__bin_to_dec__(value) + '; Hexadecimal: ' + \
+            self.__bin_to_hex__(value, leading) + '}'
```

### Comparing `cat_win-1.4.0/cat_win/util/FileAttributes.py` & `cat_win-1.4.1/cat_win/util/fileattributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime
-from math import log, pow, floor
+from math import log, floor
 from os import stat
-from platform import system
 from stat import (
     FILE_ATTRIBUTE_ARCHIVE as A,
     FILE_ATTRIBUTE_SYSTEM as S,
     FILE_ATTRIBUTE_HIDDEN as H,
     FILE_ATTRIBUTE_READONLY as R,
     FILE_ATTRIBUTE_NOT_CONTENT_INDEXED as I,
     FILE_ATTRIBUTE_COMPRESSED as C,
@@ -25,17 +24,17 @@
     (str):
         a string representation with a size value suffix
     """
     if size_bytes == 0:
         return '0 B'
     size_name = ('B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB')
     i = int(floor(log(size_bytes, 1024)))
-    p = pow(1024, i)
-    s = round(size_bytes / p, 2)
-    return f"{s} {size_name[i] if i < len(size_name) else '?'}"
+    power = pow(1024, i)
+    size = round(size_bytes / power, 2)
+    return f"{size} {size_name[i] if i < len(size_name) else '?'}"
 
 
 def read_attribs(file: str) -> list:
     """
     check which attributes a file has set.
     
     Parameters:
@@ -58,15 +57,15 @@
          # Because this attribute is true when the file is _not_ indexed
          ['Indexed', not bool(attrs & I)],
          ['Compressed', bool(attrs & C)],
          ['Encrypted', bool(attrs & E)]]
     )
 
 
-def getFileSize(file: str) -> int:
+def get_file_size(file: str) -> int:
     """
     calculate the size of a file
     
     Parameters:
     file (str):
         a string representation of a file (-path)
         
@@ -76,52 +75,52 @@
     """
     try:
         return stat(file).st_size
     except OSError:
         return 0
 
 
-def getFileMetaData(file: str, on_windows_os: bool, colors = None) -> str:
+def get_file_meta_data(file: str, on_windows_os: bool, colors = None) -> str:
     """
     calculate file metadata information.
     
     Parameters:
     file (str):
         a string representation of a file (-path)
     on_windows_os (bool):
         indicates if the user is on windows os using
         platform.system() == 'Windows'
     colors (list):
         a list containing the ANSI-Colorcodes to display
         the attributes like [RESET_ALL, ATTRIB, +ATTRIB, -ATTRIB]
     
     Returns:
-    metaData (str):
+    meta_data (str):
         representation containing file size, creation/modified/accessed time.
         on windows: also contains file attribute information
     """
-    if colors == None or len(colors) < 4:
+    if colors is None or len(colors) < 4:
         colors = ['', '', '', '']
     try:
         stats = stat(file)
-        
-        metaData = colors[1] + file + colors[0] + '\n'
-        
-        metaData += f"{colors[1]}{'Size:' : <16}{_convert_size(stats.st_size)}{colors[0]}\n"
-        metaData += f"{colors[1]}{'ATime:': <16}{datetime.fromtimestamp(stats.st_atime)}{colors[0]}\n"
-        metaData += f"{colors[1]}{'MTime:': <16}{datetime.fromtimestamp(stats.st_mtime)}{colors[0]}\n"
-        metaData += f"{colors[1]}{'CTime:': <16}{datetime.fromtimestamp(stats.st_ctime)}{colors[0]}\n"
-        
+
+        meta_data = colors[1] + file + colors[0] + '\n'
+
+        meta_data += f"{colors[1]}{'Size:' : <16}{_convert_size(stats.st_size)}{colors[0]}\n"
+        meta_data += f"{colors[1]}{'ATime:': <16}{datetime.fromtimestamp(stats.st_atime)}{colors[0]}\n"
+        meta_data += f"{colors[1]}{'MTime:': <16}{datetime.fromtimestamp(stats.st_mtime)}{colors[0]}\n"
+        meta_data += f"{colors[1]}{'CTime:': <16}{datetime.fromtimestamp(stats.st_ctime)}{colors[0]}\n"
+
         if not on_windows_os:
-            metaData += '\n'
-            return metaData
-        
+            meta_data += '\n'
+            return meta_data
+
         attribs = read_attribs(file)
-        metaData += colors[2]
-        metaData += '+' + ", ".join([x for x, y in attribs if y])
-        metaData += colors[0] + '\n'
-        metaData += colors[3]
-        metaData += '-' + ", ".join([x for x, y in attribs if not y])
-        metaData += colors[0] + '\n'
-        return metaData
+        meta_data += colors[2]
+        meta_data += '+' + ", ".join([x for x, y in attribs if y])
+        meta_data += colors[0] + '\n'
+        meta_data += colors[3]
+        meta_data += '-' + ", ".join([x for x, y in attribs if not y])
+        meta_data += colors[0] + '\n'
+        return meta_data
     except OSError:
         return ''
```

### Comparing `cat_win-1.4.0/cat_win/util/Holder.py` & `cat_win-1.4.1/cat_win/util/holder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from functools import lru_cache
+from functools import lru_cache, reduce
 from heapq import nlargest
 
-from cat_win.const.ArgConstants import *
-from cat_win.util.File import File
+from cat_win.const.argconstants import HIGHEST_ARG_ID, ARGS_NOCOL, ARGS_LLENGTH, ARGS_NUMBER, \
+    ARGS_REVERSE, ARGS_B64D, ARGS_B64E
+from cat_win.util.cbase64 import _decode_base64
+from cat_win.util.file import File
 
 
 class Holder():
     def __init__(self) -> None:
-        self.files = []  # all files, including tmp-file from stdin
-        self._inner_files = []
-        self.args = []  # list of all used parameters: format [[id, param]]
-        self.args_id = [False] * (HIGHEST_ARG_ID + 1)
+        self.files: list = []  # all files, including tmp-file from stdin
+        self._inner_files: list = []
+        self.args: list = []  # list of all used parameters: format [[id, param]]
+        self.args_id: list = [False] * (HIGHEST_ARG_ID + 1)
         self.temp_file_stdin = None  # if stdin is used, this temp_file will contain the stdin-input
         self.temp_file_echo = None  # if ARGS_ECHO is used, this temp_file will contain the following parameters
         self.reversed = False
-        
+
         # the amount of chars neccessary to display the last file
-        self.fileNumberPlaceHolder = 0
+        self.file_number_place_holder = 0
         # the sum of all lines of all files
-        self.allFilesLinesSum = 0
+        self.all_files_lines_sum = 0
         # the sum of lines for each file individually
-        self.allFilesLines = {}
+        self.all_files_lines = {}
         # the amount of chars neccessary to display the last line (breaks on base64 decoding)
-        self.fileLineNumberPlaceHolder = 0
+        self.all_line_number_place_holder = 0
         # the amount of chars neccessary to display the longest line within all files (breaks on base64 decoding)
-        self.fileLineLengthPlaceHolder = 0
+        self.file_line_length_place_holder = 0
 
-        self.clipBoard = ''
-    
-    def _getFileDisplayName(self, file: str) -> str:
+        self.clip_board = ''
+
+    def _get_file_display_name(self, file: str) -> str:
         """
         return the display name of a file. Expects self.temp_file_stdin
         and self.temp_file_echo to be set already.
         
         Parameters_
         file (str):
             a path of a file
@@ -40,112 +42,119 @@
         Returns:
         (str):
             the display name for the file. Either the path itself
             or a special identifier von stdin or echo inputs
         """
         if file == self.temp_file_stdin:
             return '<STDIN>'
-        elif file == self.temp_file_echo:
+        if file == self.temp_file_echo:
             return '<ECHO>'
         return file
-    
-    def setFiles(self, files: list) -> None:
-        self.files = [File(path, self._getFileDisplayName(path)) for path in files]
+
+    def set_files(self, files: list) -> None:
+        self.files = [File(path, self._get_file_display_name(path)) for path in files]
         self._inner_files = files[:]
 
-    def setArgs(self, args: list) -> None:
-        self.args = args
-        for id, _ in self.args:
-            self.args_id[id] = True
+    def set_args(self, args: list) -> None:
+        self.args = reduce(lambda l, x: l + [x] if x not in l else l, args, [])
+        for arg_id, _ in self.args:
+            self.args_id[arg_id] = True
         if self.args_id[ARGS_B64E]:
             self.args_id[ARGS_NOCOL] = True
             # prefix will be deleted anyway
             self.args_id[ARGS_LLENGTH] = False
             self.args_id[ARGS_NUMBER] = False
         self.reversed = self.args_id[ARGS_REVERSE]
 
-    def setTempFileStdIn(self, file: str) -> None:
+    def add_args(self, args: list) -> None:
+        self.args_id = [False] * (HIGHEST_ARG_ID + 1)
+        self.set_args(self.args + args)
+
+    def delete_args(self, args: list) -> None:
+        self.args_id = [False] * (HIGHEST_ARG_ID + 1)
+        self.set_args([arg for arg in self.args if not arg in args])
+
+    def set_temp_file_stdin(self, file: str) -> None:
         self.temp_file_stdin = file
-        
-    def setTempFileEcho(self, file: str) -> None:
+
+    def set_temp_file_echo(self, file: str) -> None:
         self.temp_file_echo = file
-    
-    def __calcFileNumberPlaceHolder__(self) -> None:
-        self.fileNumberPlaceHolder = len(str(len(self.files)))
+
+    def __calc_file_number_place_holder__(self) -> None:
+        self.file_number_place_holder = len(str(len(self.files)))
 
     def __count_generator__(self, reader):
         """
         Parameters:
         reader (method):
             the method to read from
         
         Yields:
         b (bytes):
             the bytes in chunks read from the reader
         """
-        b = reader(1024 * 1024)
-        while b:
-            yield b
-            b = reader(1024 * 1024)
+        byt = reader(1024 * 1024)
+        while byt:
+            yield byt
+            byt = reader(1024 * 1024)
 
     @lru_cache(maxsize=10)
-    def __getFileLinesSum__(self, file: str) -> int:
-        with open(file, 'rb') as fp:
-            c_generator = self.__count_generator__(fp.raw.read)
-            linesSum = sum(buffer.count(b'\n') for buffer in c_generator) + 1
-        return linesSum
+    def __get_file_lines_sum__(self, file: str) -> int:
+        with open(file, 'rb') as raw_f:
+            c_generator = self.__count_generator__(raw_f.raw.read)
+            lines_sum = sum(buffer.count(b'\n') for buffer in c_generator) + 1
+        return lines_sum
 
-    def __calcPlaceHolder__(self) -> None:
-        fileLines = []
+    def __calc_place_holder__(self) -> None:
+        file_lines = []
         for file in self._inner_files:
-            fileLineSum = self.__getFileLinesSum__(file)
-            fileLines.append(fileLineSum)
-            self.allFilesLines[file] = fileLineSum
-        self.allFilesLinesSum = sum(fileLines)
-        self.fileLineNumberPlaceHolder = len(str(max(fileLines)))
+            file_line_sum = self.__get_file_lines_sum__(file)
+            file_lines.append(file_line_sum)
+            self.all_files_lines[file] = file_line_sum
+        self.all_files_lines_sum = sum(file_lines)
+        self.all_line_number_place_holder = len(str(max(file_lines)))
 
     @lru_cache(maxsize=10)
-    def __calcMaxLineLength__(self, file: str) -> int:
+    def __calc_max_line_length__(self, file: str) -> int:
         """
-        Calculate self.fileLineLengthPlaceHolder for a single file.
+        Calculate self.file_line_length_place_holder for a single file.
         
         Parameters:
         file (str):
             a string representation of a file (-path)
             
         Returns:
         (int):
             the length of the placeholder to represent
             the longest line within the file
         """
         heap = []
         lines = []
-        with open(file, 'rb') as fp:
-            lines = fp.readlines()
-        
+        with open(file, 'rb') as raw_f:
+            lines = raw_f.readlines()
+
         heap = nlargest(1, lines, len)
         if len(heap) == 0:
             return 0
         # also check the longest line against the last line because
         # the lines still contain (\r)\n, except the last line does not
         longest_line_len = len(heap[0][:-1].rstrip(b'\n').rstrip(b'\r'))
         last_line_len = len(lines[-1].rstrip(b'\n').rstrip(b'\r'))
-        
+
         return len(str(max(longest_line_len, last_line_len)))
 
-    def __calcFileLineLengthPlaceHolder__(self) -> None:
-        self.fileLineLengthPlaceHolder = max(self.__calcMaxLineLength__(file)
+    def __calc_file_line_length_place_holder__(self) -> None:
+        self.file_line_length_place_holder = max(self.__calc_max_line_length__(file)
                                              for file in self._inner_files)
-        
-    def setDecodingTempFiles(self, temp_files: list) -> None:
+
+    def set_decoding_temp_files(self, temp_files: list) -> None:
         self._inner_files = temp_files[:]
 
-    def generateValues(self, encoding: str) -> None:
-        self.__calcFileNumberPlaceHolder__()
+    def generate_values(self, encoding: str) -> None:
+        self.__calc_file_number_place_holder__()
         if self.args_id[ARGS_B64D]:
-            from cat_win.util.Base64 import _decodeBase64
             for i, file in enumerate(self.files):
-                with open(file.path, 'rb') as fp:
-                    with open(self._inner_files[i], 'wb') as f:
-                        f.write(_decodeBase64(fp.read().decode(encoding)))
-        self.__calcPlaceHolder__()
-        self.__calcFileLineLengthPlaceHolder__()
+                with open(file.path, 'rb') as raw_f_read:
+                    with open(self._inner_files[i], 'wb') as raw_f_write:
+                        raw_f_write.write(_decode_base64(raw_f_read.read().decode(encoding)))
+        self.__calc_place_holder__()
+        self.__calc_file_line_length_place_holder__()
```

### Comparing `cat_win-1.4.0/cat_win/util/RawViewer.py` & `cat_win-1.4.1/cat_win/util/rawviewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 
-def getRawViewLinesGen(file: str = '', mode: str = 'X', colors = None, file_encoding: str = 'utf-8'):
+def get_raw_view_lines_gen(file: str = '', mode: str = 'X', colors = None,
+                           file_encoding: str = 'utf-8'):
     """
     return the raw byte representation of a file in hexadecimal or binary
     line by line
     
     Parameters:
     file (str):
         the file to use
     mode (str):
         either 'x', 'X' for hexadecimal (lower- or upper case letters),
         or 'b' for binary
     colors (list):
-        a list of two elements. Index 0 holds the color C_KW.RAWVIEWER,
-        Index 1 holds the color C_KW.RESET_ALL
+        a list of two elements. Index 0 holds the color CKW.RAWVIEWER,
+        Index 1 holds the color CKW.RESET_ALL
     file_encoding (str):
         the encoding used (possibly for stdout)
         
     Yields:
-    currentLine (str):
+    current_line (str):
         a string representation that, when put together, forms the hexviewer
         output containing the header and line information aswell
         as the bytes themselves
     """
-    if colors == None or len(colors) < 2:
+    if colors is None or len(colors) < 2:
         colors = ['', '']
-    
+
     CRLF = {10: '␤', 13: '␍'}
 
     try:
         if len(CRLF[10].encode(file_encoding)) != 3:
             raise UnicodeEncodeError('', '', -1, -1, '')
     except UnicodeEncodeError:
         CRLF = {10: '·', 13: '·'}
-    
-    def getDisplayChar(byte: int) -> str:
+
+    def get_display_char(byte: int) -> str:
         # 32 - 126 => ' ' - '~' (ASCII)
         if 32 <= byte <= 126:
             return chr(byte)
-        elif byte in [10, 13]:
+        if byte in [10, 13]:
             return CRLF[byte]
         return '·'
-    
-    rawFile = open(file, 'rb')
-    rawFileContent = rawFile.read()
-    rawFileContentLength = len(rawFileContent)
-    rawFile.close()
-    
-    reprLength = 2 * (mode.upper() == 'X') + 8 * (mode == 'b')
-     
-    currentLine = f"{colors[0]}Address  "
+
+    with open(file, 'rb') as raw_file:
+        raw_file_content = raw_file.read()
+        raw_file_content_length = len(raw_file_content)
+
+    repr_length = 2 * (mode.upper() == 'X') + 8 * (mode == 'b')
+
+    current_line = f"{colors[0]}Address  "
     for i in range(16):
-        currentLine += f"{i:0{2}X} " + '      ' * (mode == 'b')
-    currentLine += f"# Decoded Text                   {colors[1]}"
-    yield currentLine
-    
-    currentLine = f"{colors[0]}{0:0{8}X}{colors[1]} "
+        current_line += f"{i:0{2}X} " + '      ' * (mode == 'b')
+    current_line += f"# Decoded Text                   {colors[1]}"
+    yield current_line
+
+    current_line = f"{colors[0]}{0:0{8}X}{colors[1]} "
     line = []
-    for i, byte in enumerate(rawFileContent, start=1):
+    for i, byte in enumerate(raw_file_content, start=1):
         line.append(byte)
-        if not (i % 16):
-            currentLine +=  ' '.join([f"{b:0{reprLength}{mode}}" for b in line]) + \
+        if not i % 16:
+            current_line +=  ' '.join([f"{b:0{repr_length}{mode}}" for b in line]) + \
                             f" {colors[0]}#{colors[1]} " + \
-                            ' '.join(map(getDisplayChar, line))
-            yield currentLine
-            if i < rawFileContentLength:
-                currentLine = f"{colors[0]}{i:0{8}X}{colors[1]} "
+                            ' '.join(map(get_display_char, line))
+            yield current_line
+            if i < raw_file_content_length:
+                current_line = f"{colors[0]}{i:0{8}X}{colors[1]} "
             line = []
     if line:
-        currentLine +=  ' '.join([f"{b:0{reprLength}{mode}}" for b in line]) + ' ' + \
-                        ' ' * ((reprLength + 1) * (16-len(line)) - 1) + \
+        current_line +=  ' '.join([f"{b:0{repr_length}{mode}}" for b in line]) + ' ' + \
+                        ' ' * ((repr_length + 1) * (16-len(line)) - 1) + \
                         f" {colors[0]}#{colors[1]} " + \
-                        ' '.join(map(getDisplayChar, line))
-        yield currentLine
+                        ' '.join(map(get_display_char, line))
+        yield current_line
```

### Comparing `cat_win-1.4.0/cat_win/util/StdInHelper.py` & `cat_win-1.4.1/cat_win/util/stdinhelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sys import stdin
 import os
 
 
-def writeTemp(content: str, tmp_file: str, file_encoding: str) -> str:
+def write_temp(content: str, tmp_file: str, file_encoding: str) -> str:
     """
     Writes content into a generated temp-file.
     
     Parameters:
     content (str):
         the content to write in a file
     tmp_file (str):
@@ -14,33 +14,33 @@
     file_encoding (str):
         an encoding the open the file with
     
     Returns:
     tmp_file (str):
         the path to the temporary file written
     """
-    with open(tmp_file, 'wb') as f:
-        f.write(content.encode(file_encoding))
+    with open(tmp_file, 'wb') as raw_f:
+        raw_f.write(content.encode(file_encoding))
     return tmp_file
 
 
-def getStdInContent(oneLine: bool = False):
+def get_stdin_content(one_line: bool = False):
     """
     read the stdin.
     
     Parameters:
-    oneLine (bool):
+    one_line (bool):
         determines if only the first stdin line should be read
         
     Yields:
     line (str):
         the input (line by line) delivered by stdin
         until the first EOF (Chr(26)) character
     """
-    if oneLine:
+    if one_line:
         first_line = stdin.readline().rstrip('\n')
         if first_line[-1:] == chr(26):
             first_line = first_line[:-1]
         yield first_line
         return
     for line in stdin:
         if line[-2:-1] == chr(26):
@@ -58,19 +58,19 @@
         a file/dir path
         
     Returns:
     (list):
         contains each drive/directory/file in the path seperated
         "C:/a/b/c/d.txt" -> ['C:/', 'a', 'b', 'c', 'd.txt']
     """
-    p, f = os.path.split(path)
-    return path_parts(p) + [f] if f and p else [p] if p else []
+    _p, _f = os.path.split(path)
+    return path_parts(_p) + [_f] if _f and _p else [_p] if _p else []
 
 
-def createFile(file: str, content: str, file_encoding: str) -> bool:
+def create_file(file: str, content: str, file_encoding: str) -> bool:
     """
     create the directory path to a file, and the file itself.
     on error: cleanup all created subdirectories
     
     Parameters:
     file (str):
         a string representation of a file (-path)
@@ -95,29 +95,29 @@
         for subpath in unknown_subpaths:
             try:
                 os.rmdir(subpath)
             except OSError:
                 continue
         return False
     try:
-        with open(file, 'wb') as f:
-            f.write(content.encode(file_encoding))
+        with open(file, 'wb') as raw_f:
+            raw_f.write(content.encode(file_encoding))
     except OSError:
         print(f"Error: The file '{file}' could not be written.")
         # cleanup (delete the folders that have been created)
         for subpath in unknown_subpaths:
             try:
                 os.rmdir(subpath)
             except OSError:
                 continue
         return False
     return True
 
 
-def writeFiles(file_list: list, content: str, file_encoding: str) -> list:
+def write_files(file_list: list, content: str, file_encoding: str) -> list:
     """
     write to multiple files. ask if an empty file should be created
     when there is nothing to write.
     try to create the path to the files if it does not yet exist.
     delete the created path again (cleanup) if the file still could
     not be written.
     
@@ -131,77 +131,79 @@
     
     Returns:
     (list):
         containing all files, that could succesfully be written.
     """
     if len(file_list) == 0:
         return file_list
-    
+
     if content == '':
-        abort_command = '' 
+        abort_command = ''
         try:
             print('You are about to create an empty file. Do you want to continue?')
-            enterChar = '⏎'
+            enter_char = '⏎'
 
             try:
-                if len(enterChar.encode(file_encoding)) != 3:
+                if len(enter_char.encode(file_encoding)) != 3:
                     raise UnicodeEncodeError('', '', -1, -1, '')
             except UnicodeEncodeError:
-                enterChar = 'ENTER'
-            print(f"[Y/{enterChar}] Yes, Continue       [N] No, Abort :", end='')
+                enter_char = 'ENTER'
+            print(f"[Y/{enter_char}] Yes, Continue       [N] No, Abort :", end='')
             abort_command = input()
         except EOFError:
             pass
-        except UnicodeDecodeError:
+        except UnicodeError:
             print(f"Input is not recognized in the given encoding: {file_encoding}")
             abort_command = 'n'
         finally:
             if abort_command and abort_command.upper() != 'Y':
                 print('Aborting...')
                 file_list.clear()
-    
+
     success_file_list = []
-    
+
     for file in file_list:
         try:
-            with open(file, 'wb') as f:
-                f.write(content.encode(file_encoding))
+            with open(file, 'wb') as raw_file:
+                raw_file.write(content.encode(file_encoding))
             success_file_list.append(file)
         except FileNotFoundError: # the os.pardir path to the file does not exist
-            if createFile(file, content, file_encoding):
+            if create_file(file, content, file_encoding):
                 success_file_list.append(file)
         except OSError:
             print(f"Error: The file '{file}' could not be written.")
-            
+
     return success_file_list
 
 
-def readWriteFilesFromStdIn(file_list: list, file_encoding: str, on_windows_os: bool, oneLine: bool = False) -> list:
+def read_write_files_from_stdin(file_list: list, file_encoding: str, on_windows_os: bool,
+                                one_line: bool = False) -> list:
     """
     Write stdin input to multiple files.
     
     Parameters:
     file_list (list):
         all files that should be written
     file_encoding (str):
         the encoding to use for writing the files
     on_windows_os (bool):
         indicates if the user is on windows os using
         platform.system() == 'Windows'
-    oneLine (bool):
+    one_line (bool):
         determines if only the first stdin line should be read
         
     Returns:
     (list):
         containing all files, that could succesfully be written.
     """
     if len(file_list) == 0:
         return file_list
 
     print('The given FILE(s)', end='')
     print('', *file_list, sep='\n\t')
-    EOFControlChar = 'Z' if on_windows_os else 'D'
-    print(f"do/does not exist. Write the FILE(s) and finish with the ^{EOFControlChar}-suffix (Ctrl + {EOFControlChar}):")
+    eof_control_char = 'Z' if on_windows_os else 'D'
+    print('do/does not exist. Write the FILE(s) and finish with the ', end='')
+    print(f"^{eof_control_char}-suffix (Ctrl + {eof_control_char}):")
 
-    input = ''.join(getStdInContent(oneLine))
+    std_input = ''.join(get_stdin_content(one_line))
 
-    return writeFiles(file_list, input, file_encoding)
+    return write_files(file_list, std_input, file_encoding)
```

### Comparing `cat_win-1.4.0/cat_win/util/checksum.py` & `cat_win-1.4.1/cat_win/util/checksum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from zlib import crc32 as crc32_hash
 import hashlib
 
 
-def getChecksumFromFile(file: str, colors = None) -> str:
+def get_checksum_from_file(file: str, colors = None) -> str:
     """
     Calculates and returns the CRC32, MD5, SHA1, SHA256, SHA512
     hashes of a file.
     
     Parameters:
     file (str):
         a string representation of a file (-path)
@@ -14,35 +14,35 @@
         a list with 2 elements like [COLOR_CHECKSUM, COLOR_RESET]
         containing the ANSI-Colorcodes used in the returned string.
     
     Returns:
     checksum (str):
         a formatted string representation of all checksums calculated
     """
-    if colors == None or len(colors) < 2:
+    if colors is None or len(colors) < 2:
         colors = ['', '']
-    BUF_SIZE = 65536  # 64kb
+    buf_size = 65536  # 64kb
     md5 = hashlib.md5()
     sha1 = hashlib.sha1()
     sha256 = hashlib.sha256()
     sha512 = hashlib.sha512()
     crc32 = 0
 
-    with open(file, 'rb') as f:
+    with open(file, 'rb') as raw_f:
         while True:
-            data = f.read(BUF_SIZE)
+            data = raw_f.read(buf_size)
             if not data:
                 break
             md5.update(data)
             sha1.update(data)
             sha256.update(data)
             sha512.update(data)
             crc32 = crc32_hash(data, crc32)
 
     crc32 = f"{(crc32 & 0xFFFFFFFF):08X}"
-    
+
     checksum =  f"\t{colors[0]}{'CRC32:' : <9}{str(crc32)}{colors[1]}\n"
     checksum += f"\t{colors[0]}{'MD5:'   : <9}{str(md5.hexdigest())}{colors[1]}\n"
     checksum += f"\t{colors[0]}{'SHA1:'  : <9}{str(sha1.hexdigest())}{colors[1]}\n"
     checksum += f"\t{colors[0]}{'SHA256:': <9}{str(sha256.hexdigest())}{colors[1]}\n"
     checksum += f"\t{colors[0]}{'SHA512:': <9}{str(sha512.hexdigest())}{colors[1]}\n"
     return checksum
```

### Comparing `cat_win-1.4.0/cat_win/web/UpdateChecker.py` & `cat_win-1.4.1/cat_win/web/updatechecker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from json import loads as loadJSON
 from urllib.request import urlopen
 
-from cat_win.const.ColorConstants import C_KW
-
+from cat_win.const.colorconstants import CKW
 from cat_win import __url__
 
 
 # UNSAFE:
 # UPDATE MAY INCLUDE FUNDAMENTAL CHANGES
 # recognized by a higher version number in earlier position
 # !.!._
@@ -16,15 +15,15 @@
 STATUS_UP_TO_DATE = 0
 STATUS_STABLE_RELEASE_AVAILABLE = 1
 STATUS_UNSAFE_STABLE_RELEASE_AVAILABLE = -1
 STATUS_PRE_RELEASE_AVAILABLE = 2
 STATUS_UNSAFE_PRE_RELEASE_AVAILABLE = -2
 
 
-def getLastestPackageVersion(package: str) -> str:
+def get_latest_package_version(package: str) -> str:
     """
     retrieve the official PythonPackageIndex information regarding
     a package.
     
     Parameters:
     package (str):
         the package name to check
@@ -34,132 +33,132 @@
         a version representation
         on Error: a zero version '0.0.0
     """
     try:
         with urlopen(f"https://pypi.org/pypi/{package}/json", timeout=2) as _response:
             response = _response.read()
         return loadJSON(response)['info']['version']
-    except:
+    except (ValueError, OSError):
         return '0.0.0'
 
 
-def onlyNumeric(s: str) -> int:
+def only_numeric(_s: str) -> int:
     """
     strips every non-numeric character of a string.
     
     Parameters:
     s (str):
         the string to filter.
         
     Returns:
     (int):
         the resulting number of the string containing
         only numeric values
     """
-    return int('0' + ''.join(filter(str.isdigit, s)))
+    return int('0' + ''.join(filter(str.isdigit, _s)))
 
 
-def genVersionTuples(v: str, w: str) -> tuple:
+def gen_version_tuples(_v: str, _w: str) -> tuple:
     """
     create comparable version tuples.
     
     Parameters:
     v (str):
         a version representation like '1.0.33.0'
     w (str):
         a version representation like '1.1.0a'
     
     Returns:
     (tuple(tuple, tuple)):
         the version tuples of both inputs like
         (('01', '00', '33', '00'), ('01', '01', '0a', '00'))
     """
-    vSplit, wSplit = v.split('.'), w.split('.')
-    maxSplitLen = max(map(len, vSplit + wSplit))
-    vList = [s.zfill(maxSplitLen) for s in vSplit]
-    wList = [s.zfill(maxSplitLen) for s in wSplit]
-    maxLength = max(len(vList), len(wList))
-    vList += [''.zfill(maxSplitLen)] * (maxLength - len(vList))
-    wList += [''.zfill(maxSplitLen)] * (maxLength - len(wList))
-    return (tuple(vList), tuple(wList))
+    v_split, w_split = _v.split('.'), _w.split('.')
+    max_split_length = max(map(len, v_split + w_split))
+    v_list = [s.zfill(max_split_length) for s in v_split]
+    w_list = [s.zfill(max_split_length) for s in w_split]
+    max_length = max(len(v_list), len(w_list))
+    v_list += [''.zfill(max_split_length)] * (max_length - len(v_list))
+    w_list += [''.zfill(max_split_length)] * (max_length - len(w_list))
+    return (tuple(v_list), tuple(w_list))
 
-def newVersionAvailable(currentVersion: str, latestVersion: str) -> int:
+def new_version_available(current_version: str, latest_version: str) -> int:
     """
     Checks whether or not a new version is available.
     
     Parameters:
-    currentVersion (str):
+    current_version (str):
         a version representation as string
-    latestVersion (str):
+    latest_version (str):
         a version representation as string
     
     Returns:
     (int):
         a global status code describing the situation
     """
-    if currentVersion.startswith('v'):
-        currentVersion = currentVersion[1:]
-    if latestVersion.startswith('v'):
-        latestVersion = latestVersion[1:]
+    if current_version.startswith('v'):
+        current_version = current_version[1:]
+    if latest_version.startswith('v'):
+        latest_version = latest_version[1:]
     status = STATUS_UP_TO_DATE
-    current, latest = genVersionTuples(currentVersion, latestVersion)
+    current, latest = gen_version_tuples(current_version, latest_version)
     i = 0
-    for c, l in zip(current, latest):
+    for _c, _l in zip(current, latest):
         i += 1
-        cNum, lNum = onlyNumeric(c), onlyNumeric(l)
-        if cNum > lNum:
+        c_num, l_num = only_numeric(_c), only_numeric(_l)
+        if c_num > l_num:
             break
-        if cNum < lNum:
+        if c_num < l_num:
             status = STATUS_STABLE_RELEASE_AVAILABLE
-            if not l.isdigit():
+            if not _l.isdigit():
                 status = STATUS_PRE_RELEASE_AVAILABLE
             break
-        if c < l:
+        if _c < _l:
             status = STATUS_PRE_RELEASE_AVAILABLE
             break
     if i < len(current):
         status *= -1
     return status
 
 
-def printUpdateInformation(package: str, currentVersion: str, color_dic: dict) -> None:
+def print_update_information(package: str, current_version: str, color_dic: dict) -> None:
     """
     prints update information if there are any.
     
     Parameters:
     package (str):
         the package name to check
-    currentVersion (str):
+    current_version (str):
         a version representation as string of the current version
     color_dic (dict):
         a dictionary translating the color-keywords to ANSI-Colorcodes
     """
-    latestVersion = getLastestPackageVersion(package)
-    status = newVersionAvailable(currentVersion, latestVersion)
+    latest_version = get_latest_package_version(package)
+    status = new_version_available(current_version, latest_version)
     if status == STATUS_UP_TO_DATE:
         return
-    message = f""
-    warning = f""
-    info    = f""
+    message = ''
+    warning = ''
+    info    = ''
     if abs(status) == STATUS_STABLE_RELEASE_AVAILABLE:
-        message += f"{color_dic[C_KW.MESSAGE_IMPORTANT]}"
-        message += f"A new stable release of {package} is available: v{latestVersion}"
-        message += f"{color_dic[C_KW.RESET_ALL]}\n{color_dic[C_KW.MESSAGE_IMPORTANT]}"
-        message += f"To update, run:"
-        message += f"{color_dic[C_KW.RESET_ALL]}\n{color_dic[C_KW.MESSAGE_IMPORTANT]}"
+        message += f"{color_dic[CKW.MESSAGE_IMPORTANT]}"
+        message += f"A new stable release of {package} is available: v{latest_version}"
+        message += f"{color_dic[CKW.RESET_ALL]}\n{color_dic[CKW.MESSAGE_IMPORTANT]}"
+        message += 'To update, run:'
+        message += f"{color_dic[CKW.RESET_ALL]}\n{color_dic[CKW.MESSAGE_IMPORTANT]}"
         message += f"python -m pip install --upgrade {package}"
     elif abs(status) == STATUS_PRE_RELEASE_AVAILABLE:
-        message += f"{color_dic[C_KW.MESSAGE_INFORMATION]}"
-        message += f"A new pre-release of {package} is available: v{latestVersion}"
-    message += f"{color_dic[C_KW.RESET_ALL]}"
+        message += f"{color_dic[CKW.MESSAGE_INFORMATION]}"
+        message += f"A new pre-release of {package} is available: v{latest_version}"
+    message += f"{color_dic[CKW.RESET_ALL]}"
     if status < STATUS_UP_TO_DATE:
-        warning += f"{color_dic[C_KW.MESSAGE_WARNING]}"
-        warning += f"Warning: Due to the drastic version increase, backwards compatibility is no longer guaranteed!"
-        warning += f"{color_dic[C_KW.RESET_ALL]}\n{color_dic[C_KW.MESSAGE_WARNING]}"
-        warning += f"You may experience fundamental differences."
-        warning += f"{color_dic[C_KW.RESET_ALL]}"
-    info += f"{color_dic[C_KW.MESSAGE_INFORMATION]}Take a look at the changelog here:"
-    info += f"{color_dic[C_KW.RESET_ALL]}\n{color_dic[C_KW.MESSAGE_INFORMATION]}"
-    info += f"{__url__}/blob/main/CHANGELOG.md{color_dic[C_KW.RESET_ALL]}"
+        warning += f"{color_dic[CKW.MESSAGE_WARNING]}"
+        warning += 'Warning: Due to the drastic version increase, backwards compatibility is no longer guaranteed!'
+        warning += f"{color_dic[CKW.RESET_ALL]}\n{color_dic[CKW.MESSAGE_WARNING]}"
+        warning += 'You may experience fundamental differences.'
+        warning += f"{color_dic[CKW.RESET_ALL]}"
+    info += f"{color_dic[CKW.MESSAGE_INFORMATION]}Take a look at the changelog here:"
+    info += f"{color_dic[CKW.RESET_ALL]}\n{color_dic[CKW.MESSAGE_INFORMATION]}"
+    info += f"{__url__}/blob/main/CHANGELOG.md{color_dic[CKW.RESET_ALL]}"
     print(message)
     print(warning)
     print(info)
```

### Comparing `cat_win-1.4.0/pyproject.toml` & `cat_win-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.0/PKG-INFO` & `cat_win-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cat_win
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple OS Independent 'cat' Command-line Tool made in Python.
 Keywords: cat,cli,console,crossplatform,python,terminal
 Author-email: "Silas A. Kraume" <silas.kraume1552@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -25,19 +25,19 @@
 Project-URL: Github, https://github.com/SilenZcience/cat_win
 Project-URL: Tracker, https://github.com/SilenZcience/cat_win/issues
 Provides-Extra: clip
 
 <div id="top"></div>
 
 <p>
-   <a href="https://pypi.org/project/cat-win/" alt="Downloads">
-      <img src="https://static.pepy.tech/personalized-badge/cat-win?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" align="right">
+   <a href="https://pepy.tech/project/cat-win/" alt="Downloads">
+      <img src="https://static.pepy.tech/personalized-badge/cat-win?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" align="right">
    </a>
-   <a href="https://pepy.tech/project/cat-win/" alt="Visitors">
-      <img src="https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win" align="right">
+   <a href="https://pypi.org/project/cat-win/" alt="Visitors">
+      <img src="https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win&right_color=orange" align="right">
    </a>
    <a href="https://github.com/SilenZcience/cat_win/tree/main/cat_win" alt="CodeSize">
       <img src="https://img.shields.io/github/languages/code-size/SilenZcience/cat_win?color=purple" align="right">
    </a>
 </p>
 
 [![OS-Windows]][OS-Windows]
@@ -129,16 +129,17 @@
 ```console
 python -m pip install --upgrade cat_win
 ```
 and manually install the desired module yourself.
 
 **OR alternatively** you can use the compiled version (*`Windows only`*):
 
-1. Simply download the [catw.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/catw.exe) file.
-2. Add the file path to your system-environment `PATH`-variables.
+1. Simply download the [catw.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/catw.exe) file to handle filecontents.
+2. Download the [cats.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/main/bin/cats.exe) file to use the cat-shell (optional).
+3. Add the file path to your system-environment `PATH`-variables.
 
 > ⚠️ **You should never trust any executable file!** Feel free to compile the package yourself (e.g. using [PyInstaller](https://pyinstaller.org/en/stable/)).
 
 > You can verify the creation of catw.exe yourself by reading the [source code](https://github.com/SilenZcience/cat_win/blob/main/cat_win/cat.py), checking the [origin](https://github.com/SilenZcience/cat_win/tree/main/bin) of the file and validating the corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/main/.github/workflows/build_executable.yml) used.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -147,95 +148,111 @@
 ```console
 catw [FILE]... [OPTION]...
 catw --help
 ```
 
 > ⚠️ *from v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to keep the old command, you will have to define an alias yourself.*
 
-| Argument / Option      | Description                                               |
-|------------------------|-----------------------------------------------------------|
-| *-h, --help*           | show help message and exit                                |
-| *-v, --version*        | output version information                                |
-| *-d, --debug*          | show debug information                                    |
-|                        |                                                           |
-| *-n, --number*         | number all output lines                                   |
-| *-l, --linelength*     | display the length of each line                           |
-| *-e, --ends*           | display $ at the end of each line                         |
-| *-t, --tabs*           | display TAB characters as ^I                              |
-| *--eof, --eof*         | display EOF characters as ^EOF                            |
-| *-u, --unique*         | suppress repeated output lines                            |
-| *-b, --blank*          | hide empty lines                                          |
-| *-r, --reverse*        | reverse output                                            |
-| *-p, --peek*           | only print the first and last lines                       |
-| *-s, --sum*            | show sum of lines                                         |
-| *-S, --SUM*            | ONLY show sum of lines                                    |
-| *-f, --files*          | list applied files                                        |
-| *-F, --FILES*          | ONLY list applied files and file sizes                    |
-| *-g, --grep*           | only show lines containing queried keywords               |
-| *-i, --interactive*    | use stdin                                                 |
-| *-o, --oneline*        | take only the first stdin-line                            |
-| *-E, --ECHO*           | handle every following parameter as stdin                 |
-| *-c, --clip*           | copy output to clipboard                                  |
-| *-m, --checksum*       | show the checksums of all files                           |
-| *-a, --attributes*     | show meta-information about the files                     |
-|                        |                                                           |
-| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         |
-| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         |
-| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         |
-| *--b64e, --b64e*       | encode the input to base64                                |
-| *--b64d, --b64d*       | decode the input from base64                              |
-|                        |                                                           |
-| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        |
-| *--binview, --binview* | display the raw byte representation in binary             |
-|                        |                                                           |
-| *--nc, --nocolor*      | disable colored output                                    |
-| *--nb, --nobreak*      | do not interrupt the output on queried keywords           |
-| *--nk, --nokeyword*    | inverse the grep output                                   |
-| *-R, --reconfigure*    | reconfigure the stdin and stdout with the parsed encoding |
-| *--config, --config*   | change color configuration                                |
-|                        |                                                           |
-| *enc=X*                | set file enconding to X (default is utf-8)                |
-| *find=X*               | find/query a substring X in the given files               |
-| *match=X*              | find/query a pattern X in the given files                 |
-| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              |
-|                        |                                                           |
-| *[a,b]*                | replace a with b in every line                            |
-| *[a:​b:c]*              | python-like string indexing syntax (line by line)         |
+```console
+cats [OPTION]...
+cats --help
+```
+
+| Argument / Option      | Description                                               | works in shell |
+|------------------------|-----------------------------------------------------------|----------------|
+| *-h, --help*           | show help message and exit                                | ✔              |
+| *-v, --version*        | output version information                                | ✔              |
+| *-d, --debug*          | show debug information                                    | ✔              |
+|                        |                                                           |                |
+| *-n, --number*         | number all output lines                                   | ✔              |
+| *-l, --linelength*     | display the length of each line                           | ✔              |
+| *-e, --ends*           | display $ at the end of each line                         | ✔              |
+| *-t, --tabs*           | display TAB characters as ^I                              | ✔              |
+| *--eof, --eof*         | display EOF characters as ^EOF                            | ✔              |
+| *-u, --unique*         | suppress repeated output lines                            | ❌             |
+| *-b, --blank*          | hide empty lines                                          | ✔              |
+| *-r, --reverse*        | reverse output                                            | ❌             |
+| *-p, --peek*           | only print the first and last lines                       | ❌             |
+| *-s, --sum*            | show sum of lines                                         | ❌             |
+| *-S, --SUM*            | ONLY show sum of lines                                    | ❌             |
+| *-f, --files*          | list applied files                                        | ❌             |
+| *-F, --FILES*          | ONLY list applied files and file sizes                    | ❌             |
+| *-g, --grep*           | only show lines containing queried keywords               | ✔              |
+| *-i, --interactive*    | use stdin                                                 | ❌             |
+| *-o, --oneline*        | take only the first stdin-line                            | ❌             |
+| *-E, --ECHO*           | handle every following parameter as stdin                 | ❌             |
+| *-c, --clip*           | copy output to clipboard                                  | ✔              |
+| *-m, --checksum*       | show the checksums of all files                           | ❌             |
+| *-a, --attributes*     | show meta-information about the files                     | ❌             |
+|                        |                                                           |                |
+| *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         | ✔              |
+| *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         | ✔              |
+| *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         | ✔              |
+| *--b64e, --b64e*       | encode the input to base64                                | ✔              |
+| *--b64d, --b64d*       | decode the input from base64                              | ✔              |
+|                        |                                                           |                |
+| *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        | ❌             |
+| *--binview, --binview* | display the raw byte representation in binary             | ❌             |
+|                        |                                                           |                |
+| *--nc, --nocolor*      | disable colored output                                    | ✔              |
+| *--nb, --nobreak*      | do not interrupt the output on queried keywords           | ✔              |
+| *--nk, --nokeyword*    | inverse the grep output                                   | ✔              |
+| *--config, --config*   | change color configuration                                | ✔              |
+|                        |                                                           |                |
+| *-R, --R\<stream\>*    | reconfigure the std-stream(s) with the parsed encoding </br> \<stream\> = 'in'/'out'/'err' (default is stdin & stdout)| ✔ |
+|                        |                                                           |                |
+| *enc=X*                | set file enconding to X (default is utf-8)                | ✔              |
+| *find=X*               | find/query a substring X in the given files               | ✔              |
+| *match=X*              | find/query a pattern X in the given files                 | ✔              |
+| *trunc=X:Y*            | truncate file to lines X and Y (python-like)              | ❌             |
+|                        |                                                           |                |
+| *[a,b]*                | replace a with b in every line                            | ✔              |
+| *[a:​b:c]*              | python-like string indexing syntax (line by line)         | ✔              |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
-![Example1](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png "example1")
-
-![Example2](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png "example2")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png" width="49%"/>
+   </p>
 
-![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png "example3")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png" width="49%"/>
+   </p>
 
-![Example4](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png "example4")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png" width="49%"/>
+   </p>
 
-![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png "example5")
+   - - - -
 
-![Example6](https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png "example6")
+   <p float="left">
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png" width="49%"/>
+      <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png" width="49%"/>
+   </p>
 
 </details>
 
-```console
+```c
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
+- - - -
+
 ```c
 $ cats --dec -nl
 > >>> 12345
 > 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
-> >>> 54321
-> 2) [55] 54321 {Hexadecimal: 0xd431; Binary: 0b1101010000110001}
-> ...
+> >>> ...
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
 Take a look at the [Changelog](https://github.com/SilenZcience/cat_win/blob/main/CHANGELOG.md) file.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cat_win Version: 1.4.0 Summary: Simple OS
+Metadata-Version: 2.1 Name: cat_win Version: 1.4.1 Summary: Simple OS
 Independent 'cat' Command-line Tool made in Python. Keywords:
 cat,cli,console,crossplatform,python,terminal Author-email: "Silas A. Kraume"
 kraume1552@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -12,17 +12,18 @@
 System :: OS Independent Classifier: Topic :: Terminals Classifier: Topic ::
 Text Processing :: Linguistic Requires-Dist: colorama~=0.4.6 Requires-Dist:
 pyperclip~=1.8.0 ; extra == "clip" Project-URL: Download, https://github.com/
 SilenZcience/cat_win/tarball/master Project-URL: Github, https://github.com/
 SilenZcience/cat_win Project-URL: Tracker, https://github.com/SilenZcience/
 cat_win/issues Provides-Extra: clip
 [https://static.pepy.tech/personalized-badge/cat-
-win?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads]
-[https://visitor-badge.laobi.icu/badge?page_id=SilenZcience.cat_win] [https://
-img.shields.io/github/languages/code-size/SilenZcience/cat_win?color=purple]
+win?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads]
+[https://visitor-badge.laobi.icu/
+badge?page_id=SilenZcience.cat_win&right_color=orange] [https://img.shields.io/
+github/languages/code-size/SilenZcience/cat_win?color=purple]
 [![OS-Windows]][OS-Windows] [![OS-Linux]][OS-Linux] [![OS-MacOS]][OS-MacOS]
                               ***** cat_win *****
                    Simple Command-line Tool made in Python
                              Explore_the_code_Â»
 
                          Report_Bug Â· Request_Feature
  Table of Contents
@@ -62,71 +63,79 @@
 --upgrade cat_win[clip] ``` cat_win uses the [pyperclip](https://pypi.org/
 project/pyperclip/) module by default. Should any problems occur, you can also
 use the [pyperclip3](https://pypi.org/project/pyperclip3/) or [pyclip](https://
 pypi.org/project/pyclip/) module. In this case simply run: ```console python -
 m pip install --upgrade cat_win ``` and manually install the desired module
 yourself. **OR alternatively** you can use the compiled version (*`Windows
 only`*): 1. Simply download the [catw.exe](https://raw.githubusercontent.com/
-SilenZcience/cat_win/main/bin/catw.exe) file. 2. Add the file path to your
-system-environment `PATH`-variables. > â ï¸ **You should never trust any
-executable file!** Feel free to compile the package yourself (e.g. using
+SilenZcience/cat_win/main/bin/catw.exe) file to handle filecontents. 2.
+Download the [cats.exe](https://raw.githubusercontent.com/SilenZcience/cat_win/
+main/bin/cats.exe) file to use the cat-shell (optional). 3. Add the file path
+to your system-environment `PATH`-variables. > â ï¸ **You should never trust
+any executable file!** Feel free to compile the package yourself (e.g. using
 [PyInstaller](https://pyinstaller.org/en/stable/)). > You can verify the
 creation of catw.exe yourself by reading the [source code](https://github.com/
 SilenZcience/cat_win/blob/main/cat_win/cat.py), checking the [origin](https://
 github.com/SilenZcience/cat_win/tree/main/bin) of the file and validating the
 corresponding [workflow](https://github.com/SilenZcience/cat_win/blob/
 main/.github/workflows/build_executable.yml) used.
                                                                   (back_to_top)
 ## Usage ```console catw [FILE]... [OPTION]... catw --help ``` > â ï¸ *from
 v1.0.33 to v1.1.0 the entrypoint changes from `cat` to `catw`. If you wish to
-keep the old command, you will have to define an alias yourself.* | Argument /
-Option | Description | |------------------------|------------------------------
------------------------------| | *-h, --help* | show help message and exit | |
-*-v, --version* | output version information | | *-d, --debug* | show debug
-information | | | | | *-n, --number* | number all output lines | | *-l, --
-linelength* | display the length of each line | | *-e, --ends* | display $ at
-the end of each line | | *-t, --tabs* | display TAB characters as ^I | | *--
-eof, --eof* | display EOF characters as ^EOF | | *-u, --unique* | suppress
-repeated output lines | | *-b, --blank* | hide empty lines | | *-r, --reverse*
-| reverse output | | *-p, --peek* | only print the first and last lines | | *-
-s, --sum* | show sum of lines | | *-S, --SUM* | ONLY show sum of lines | | *-f,
---files* | list applied files | | *-F, --FILES* | ONLY list applied files and
-file sizes | | *-g, --grep* | only show lines containing queried keywords | |
-*-i, --interactive* | use stdin | | *-o, --oneline* | take only the first
-stdin-line | | *-E, --ECHO* | handle every following parameter as stdin | | *-
-c, --clip* | copy output to clipboard | | *-m, --checksum* | show the checksums
-of all files | | *-a, --attributes* | show meta-information about the files | |
-| | | *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | | *-
--hex, --HEX* | convert hexadecimal numbers to decimal and binary | | *--bin, --
-BIN* | convert binary numbers to decimal and hexadecimal | | *--b64e, --b64e* |
-encode the input to base64 | | *--b64d, --b64d* | decode the input from base64
-| | | | | *--hexview, --HEXVIEW* | display the raw byte representation in
-hexadecimal | | *--binview, --binview* | display the raw byte representation in
-binary | | | | | *--nc, --nocolor* | disable colored output | | *--nb, --
-nobreak* | do not interrupt the output on queried keywords | | *--nk, --
-nokeyword* | inverse the grep output | | *-R, --reconfigure* | reconfigure the
-stdin and stdout with the parsed encoding | | *--config, --config* | change
-color configuration | | | | | *enc=X* | set file enconding to X (default is
-utf-8) | | *find=X* | find/query a substring X in the given files | | *match=X*
-| find/query a pattern X in the given files | | *trunc=X:Y* | truncate file to
-lines X and Y (python-like) | | | | | *[a,b]* | replace a with b in every line
-| | *[a:âb:c]* | python-like string indexing syntax (line by line) | ###
-Examples  ð Images ð ![Example1](https://raw.githubusercontent.com/
-SilenZcience/cat_win/main/img/example1.png "example1") ![Example2](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png
-"example2") ![Example3](https://raw.githubusercontent.com/SilenZcience/cat_win/
-main/img/example3.png "example3") ![Example4](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png
-"example4") ![Example5](https://raw.githubusercontent.com/SilenZcience/cat_win/
-main/img/example5.png "example5") ![Example6](https://
-raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png
-"example6")  ```console $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1]
--ln > 1) [8] ): dlroW ``` ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
-{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> 54321 > 2) [55] 54321
-{Hexadecimal: 0xd431; Binary: 0b1101010000110001} > ... ```
+keep the old command, you will have to define an alias yourself.* ```console
+cats [OPTION]... cats --help ``` | Argument / Option | Description | works in
+shell | |------------------------|---------------------------------------------
+--------------|----------------| | *-h, --help* | show help message and exit |
+â | | *-v, --version* | output version information | â | | *-d, --debug* |
+show debug information | â | | | | | | *-n, --number* | number all output
+lines | â | | *-l, --linelength* | display the length of each line | â | |
+*-e, --ends* | display $ at the end of each line | â | | *-t, --tabs* |
+display TAB characters as ^I | â | | *--eof, --eof* | display EOF characters
+as ^EOF | â | | *-u, --unique* | suppress repeated output lines | â | | *-
+b, --blank* | hide empty lines | â | | *-r, --reverse* | reverse output | â
+| | *-p, --peek* | only print the first and last lines | â | | *-s, --sum* |
+show sum of lines | â | | *-S, --SUM* | ONLY show sum of lines | â | | *-f,
+--files* | list applied files | â | | *-F, --FILES* | ONLY list applied files
+and file sizes | â | | *-g, --grep* | only show lines containing queried
+keywords | â | | *-i, --interactive* | use stdin | â | | *-o, --oneline* |
+take only the first stdin-line | â | | *-E, --ECHO* | handle every following
+parameter as stdin | â | | *-c, --clip* | copy output to clipboard | â | |
+*-m, --checksum* | show the checksums of all files | â | | *-a, --attributes*
+| show meta-information about the files | â | | | | | | *--dec, --DEC* |
+convert decimal numbers to hexadecimal and binary | â | | *--hex, --HEX* |
+convert hexadecimal numbers to decimal and binary | â | | *--bin, --BIN* |
+convert binary numbers to decimal and hexadecimal | â | | *--b64e, --b64e* |
+encode the input to base64 | â | | *--b64d, --b64d* | decode the input from
+base64 | â | | | | | | *--hexview, --HEXVIEW* | display the raw byte
+representation in hexadecimal | â | | *--binview, --binview* | display the
+raw byte representation in binary | â | | | | | | *--nc, --nocolor* | disable
+colored output | â | | *--nb, --nobreak* | do not interrupt the output on
+queried keywords | â | | *--nk, --nokeyword* | inverse the grep output | â
+| | *--config, --config* | change color configuration | â | | | | | | *-R, --
+R\
+>* | reconfigure the std-stream(s) with the parsed encoding  \
+> = 'in'/'out'/'err' (default is stdin & stdout)| â | | | | | | *enc=X* | set
+file enconding to X (default is utf-8) | â | | *find=X* | find/query a
+substring X in the given files | â | | *match=X* | find/query a pattern X in
+the given files | â | | *trunc=X:Y* | truncate file to lines X and Y (python-
+like) | â | | | | | | *[a,b]* | replace a with b in every line | â | | *[a:
+âb:c]* | python-like string indexing syntax (line by line) | â | ###
+Examples  ð Images ð
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png]
+- - - -
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png]
+[https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png]
+ ```c $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
+dlroW ``` - - - - ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
+{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
```

