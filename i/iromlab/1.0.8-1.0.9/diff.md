# Comparing `tmp/iromlab-1.0.8.tar.gz` & `tmp/iromlab-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iromlab-1.0.8.tar", last modified: Thu Sep 16 13:48:31 2021, max compression
+gzip compressed data, was "iromlab-1.0.9.tar", last modified: Thu May  4 10:59:42 2023, max compression
```

## Comparing `iromlab-1.0.8.tar` & `iromlab-1.0.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.417015 iromlab-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      587 2021-09-16 13:48:31.417015 iromlab-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      137 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/cdinfo.py
--rw-rw-r--   0 root         (0) root         (0)    21693 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/cdworker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab/conf/
--rw-rw-r--   0 root         (0) root         (0)     5423 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/conf/config.xml
--rw-rw-r--   0 root         (0) root         (0)      639 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/config.py
--rw-rw-r--   0 root         (0) root         (0)     8451 2021-09-16 13:45:06.000000 iromlab-1.0.8/iromlab/configure.pyw
--rw-rw-r--   0 root         (0) root         (0)     1750 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/dbpoweramp.py
--rw-rw-r--   0 root         (0) root         (0)     4823 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/drivers.py
--rw-rw-r--   0 root         (0) root         (0)    36305 2021-09-16 13:45:15.000000 iromlab-1.0.8/iromlab/iromlab.pyw
--rw-rw-r--   0 root         (0) root         (0)     6441 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/isobuster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab/kbapi/
--rw-rw-r--   0 root         (0) root         (0)      129 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/kbapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12625 2021-03-10 17:52:49.000000 iromlab-1.0.8/iromlab/kbapi/sru.py
--rw-rw-r--   0 root         (0) root         (0)     1004 2021-03-10 17:52:49.000000 iromlab-1.0.8/iromlab/mdo.py
--rw-rw-r--   0 root         (0) root         (0)     1722 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/shared.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab/socketserver/
--rw-rw-r--   0 root         (0) root         (0)       27 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/socketserver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1840 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/socketserver/server.py
--rw-rw-r--   0 root         (0) root         (0)     1831 2021-03-10 17:52:49.000000 iromlab-1.0.8/iromlab/testsru.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.401015 iromlab-1.0.8/iromlab/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab/tools/flac/
--rw-rw-r--   0 root         (0) root         (0)    20403 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/COPYING.FDL
--rw-rw-r--   0 root         (0) root         (0)    18092 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/COPYING.GPL
--rw-rw-r--   0 root         (0) root         (0)    26436 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/COPYING.LGPL
--rw-rw-r--   0 root         (0) root         (0)     1509 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/COPYING.Xiph
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.409015 iromlab-1.0.8/iromlab/tools/flac/html/
--rw-rw-r--   0 root         (0) root         (0)    82369 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/changelog.html
--rw-rw-r--   0 root         (0) root         (0)     5874 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/developers.html
--rw-rw-r--   0 root         (0) root         (0)     5049 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation.html
--rw-rw-r--   0 root         (0) root         (0)     3282 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_bugs.html
--rw-rw-r--   0 root         (0) root         (0)     2857 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_example_code.html
--rw-rw-r--   0 root         (0) root         (0)    11078 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_format_overview.html
--rw-rw-r--   0 root         (0) root         (0)     3580 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools.html
--rw-rw-r--   0 root         (0) root         (0)    74395 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools_flac.html
--rw-rw-r--   0 root         (0) root         (0)    28729 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools_metaflac.html
--rw-rw-r--   0 root         (0) root         (0)    29775 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/faq.html
--rw-rw-r--   0 root         (0) root         (0)     1406 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/favicon.ico
--rw-rw-r--   0 root         (0) root         (0)     8537 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/features.html
--rw-rw-r--   0 root         (0) root         (0)     3044 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/flac.css
--rw-rw-r--   0 root         (0) root         (0)    69576 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/format.html
--rw-rw-r--   0 root         (0) root         (0)     8881 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/id.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.409015 iromlab-1.0.8/iromlab/tools/flac/html/images/
--rw-rw-r--   0 root         (0) root         (0)    31371 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/images/logo.svg
--rw-rw-r--   0 root         (0) root         (0)     3895 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/images/logo130.gif
--rw-rw-r--   0 root         (0) root         (0)     4228 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/index.html
--rw-rw-r--   0 root         (0) root         (0)     5221 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/license.html
--rw-rw-r--   0 root         (0) root         (0)     9334 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/html/ogg_mapping.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.409015 iromlab-1.0.8/iromlab/tools/flac/win32/
--rw-rw-r--   0 root         (0) root         (0)   738816 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/win32/flac.exe
--rw-rw-r--   0 root         (0) root         (0)   483840 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/win32/metaflac.exe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.409015 iromlab-1.0.8/iromlab/tools/flac/win64/
--rw-rw-r--   0 root         (0) root         (0)   709632 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/win64/flac.exe
--rw-rw-r--   0 root         (0) root         (0)   439296 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/flac/win64/metaflac.exe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.409015 iromlab-1.0.8/iromlab/tools/libcdio/
--rw-rw-r--   0 root         (0) root         (0)     3858 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.413015 iromlab-1.0.8/iromlab/tools/libcdio/win64/
--rw-rw-r--   0 root         (0) root         (0)    64123 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-drive.exe
--rw-rw-r--   0 root         (0) root         (0)    87663 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-info.exe
--rw-rw-r--   0 root         (0) root         (0)   100410 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-paranoia.exe
--rw-rw-r--   0 root         (0) root         (0)    68795 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-read.exe
--rw-rw-r--   0 root         (0) root         (0)    69398 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/iso-info.exe
--rw-rw-r--   0 root         (0) root         (0)    67365 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/iso-read.exe
--rw-rw-r--   0 root         (0) root         (0)   119992 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libcddb-2.dll
--rw-rw-r--   0 root         (0) root         (0)    22546 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio++-0.dll
--rw-rw-r--   0 root         (0) root         (0)   208727 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio-16.dll
--rw-rw-r--   0 root         (0) root         (0)    63316 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio_cdda-2.dll
--rw-rw-r--   0 root         (0) root         (0)    40697 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio_paranoia-2.dll
--rw-rw-r--   0 root         (0) root         (0)  1050543 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libiconv-2.dll
--rw-rw-r--   0 root         (0) root         (0)   132717 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libintl-8.dll
--rw-rw-r--   0 root         (0) root         (0)    24441 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libiso9660++-0.dll
--rw-rw-r--   0 root         (0) root         (0)    76264 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libiso9660-10.dll
--rw-rw-r--   0 root         (0) root         (0)    18412 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libsystre-0.dll
--rw-rw-r--   0 root         (0) root         (0)    91386 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libtre-5.dll
--rw-rw-r--   0 root         (0) root         (0)    27494 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libudf-0.dll
--rw-rw-r--   0 root         (0) root         (0)    56978 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/libwinpthread-1.dll
--rw-rw-r--   0 root         (0) root         (0)    70253 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/libcdio/win64/mmc-tool.exe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.413015 iromlab-1.0.8/iromlab/tools/shntool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.413015 iromlab-1.0.8/iromlab/tools/shntool/doc/
--rw-rw-r--   0 root         (0) root         (0)    16233 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/doc/ChangeLog.txt
--rw-rw-r--   0 root         (0) root         (0)     6798 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/doc/Credits.txt
--rw-rw-r--   0 root         (0) root         (0)     2001 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/doc/Install.txt
--rw-rw-r--   0 root         (0) root         (0)    33328 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/doc/shntool.pdf
--rw-rw-r--   0 root         (0) root         (0)    33659 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/doc/shntool.txt
--rw-rw-r--   0 root         (0) root         (0)   214016 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/tools/shntool/shntool.exe
--rw-rw-r--   0 root         (0) root         (0)     3540 2020-08-24 11:54:50.000000 iromlab-1.0.8/iromlab/verifyaudio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 13:48:31.405015 iromlab-1.0.8/iromlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)      587 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2891 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-08-24 12:01:12.000000 iromlab-1.0.8/iromlab.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-09-16 13:48:31.000000 iromlab-1.0.8/iromlab.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       79 2021-09-16 13:48:31.417015 iromlab-1.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2422 2020-08-24 11:54:50.000000 iromlab-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.432861 iromlab-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-05-04 10:59:42.432861 iromlab-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.180859 iromlab-1.0.9/iromlab/
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      137 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/cdinfo.py
+-rw-rw-r--   0 root         (0) root         (0)    21693 2022-02-03 17:06:57.000000 iromlab-1.0.9/iromlab/cdworker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.180859 iromlab-1.0.9/iromlab/conf/
+-rw-rw-r--   0 root         (0) root         (0)     5423 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/conf/config.xml
+-rw-rw-r--   0 root         (0) root         (0)      639 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/config.py
+-rw-rw-r--   0 root         (0) root         (0)     8451 2021-09-16 13:45:06.000000 iromlab-1.0.9/iromlab/configure.pyw
+-rw-rw-r--   0 root         (0) root         (0)     1750 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/dbpoweramp.py
+-rw-rw-r--   0 root         (0) root         (0)     4823 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/drivers.py
+-rw-rw-r--   0 root         (0) root         (0)    36305 2023-05-04 10:57:51.000000 iromlab-1.0.9/iromlab/iromlab.pyw
+-rw-rw-r--   0 root         (0) root         (0)     6959 2023-05-04 10:49:58.000000 iromlab-1.0.9/iromlab/isobuster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.196859 iromlab-1.0.9/iromlab/kbapi/
+-rw-rw-r--   0 root         (0) root         (0)      129 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/kbapi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12625 2021-03-10 17:52:49.000000 iromlab-1.0.9/iromlab/kbapi/sru.py
+-rw-rw-r--   0 root         (0) root         (0)     1004 2021-03-10 17:52:49.000000 iromlab-1.0.9/iromlab/mdo.py
+-rw-rw-r--   0 root         (0) root         (0)     1722 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/shared.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.196859 iromlab-1.0.9/iromlab/socketserver/
+-rw-rw-r--   0 root         (0) root         (0)       27 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/socketserver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1840 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/socketserver/server.py
+-rw-rw-r--   0 root         (0) root         (0)     1831 2022-05-24 10:18:12.000000 iromlab-1.0.9/iromlab/testsru.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.164859 iromlab-1.0.9/iromlab/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.212859 iromlab-1.0.9/iromlab/tools/flac/
+-rw-rw-r--   0 root         (0) root         (0)    20403 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/COPYING.FDL
+-rw-rw-r--   0 root         (0) root         (0)    18092 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/COPYING.GPL
+-rw-rw-r--   0 root         (0) root         (0)    26436 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/COPYING.LGPL
+-rw-rw-r--   0 root         (0) root         (0)     1509 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/COPYING.Xiph
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.256860 iromlab-1.0.9/iromlab/tools/flac/html/
+-rw-rw-r--   0 root         (0) root         (0)    82369 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/changelog.html
+-rw-rw-r--   0 root         (0) root         (0)     5874 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/developers.html
+-rw-rw-r--   0 root         (0) root         (0)     5049 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation.html
+-rw-rw-r--   0 root         (0) root         (0)     3282 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_bugs.html
+-rw-rw-r--   0 root         (0) root         (0)     2857 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_example_code.html
+-rw-rw-r--   0 root         (0) root         (0)    11078 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_format_overview.html
+-rw-rw-r--   0 root         (0) root         (0)     3580 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools.html
+-rw-rw-r--   0 root         (0) root         (0)    74395 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools_flac.html
+-rw-rw-r--   0 root         (0) root         (0)    28729 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools_metaflac.html
+-rw-rw-r--   0 root         (0) root         (0)    29775 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/faq.html
+-rw-rw-r--   0 root         (0) root         (0)     1406 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/favicon.ico
+-rw-rw-r--   0 root         (0) root         (0)     8537 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/features.html
+-rw-rw-r--   0 root         (0) root         (0)     3044 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/flac.css
+-rw-rw-r--   0 root         (0) root         (0)    69576 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/format.html
+-rw-rw-r--   0 root         (0) root         (0)     8881 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/id.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.256860 iromlab-1.0.9/iromlab/tools/flac/html/images/
+-rw-rw-r--   0 root         (0) root         (0)    31371 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/images/logo.svg
+-rw-rw-r--   0 root         (0) root         (0)     3895 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/images/logo130.gif
+-rw-rw-r--   0 root         (0) root         (0)     4228 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/index.html
+-rw-rw-r--   0 root         (0) root         (0)     5221 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/license.html
+-rw-rw-r--   0 root         (0) root         (0)     9334 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/html/ogg_mapping.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.304860 iromlab-1.0.9/iromlab/tools/flac/win32/
+-rw-rw-r--   0 root         (0) root         (0)   738816 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/win32/flac.exe
+-rw-rw-r--   0 root         (0) root         (0)   483840 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/win32/metaflac.exe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.324860 iromlab-1.0.9/iromlab/tools/flac/win64/
+-rw-rw-r--   0 root         (0) root         (0)   709632 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/win64/flac.exe
+-rw-rw-r--   0 root         (0) root         (0)   439296 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/flac/win64/metaflac.exe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.336860 iromlab-1.0.9/iromlab/tools/libcdio/
+-rw-rw-r--   0 root         (0) root         (0)     3858 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.424861 iromlab-1.0.9/iromlab/tools/libcdio/win64/
+-rw-rw-r--   0 root         (0) root         (0)    64123 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-drive.exe
+-rw-rw-r--   0 root         (0) root         (0)    87663 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-info.exe
+-rw-rw-r--   0 root         (0) root         (0)   100410 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-paranoia.exe
+-rw-rw-r--   0 root         (0) root         (0)    68795 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-read.exe
+-rw-rw-r--   0 root         (0) root         (0)    69398 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/iso-info.exe
+-rw-rw-r--   0 root         (0) root         (0)    67365 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/iso-read.exe
+-rw-rw-r--   0 root         (0) root         (0)   119992 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libcddb-2.dll
+-rw-rw-r--   0 root         (0) root         (0)    22546 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio++-0.dll
+-rw-rw-r--   0 root         (0) root         (0)   208727 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio-16.dll
+-rw-rw-r--   0 root         (0) root         (0)    63316 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio_cdda-2.dll
+-rw-rw-r--   0 root         (0) root         (0)    40697 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio_paranoia-2.dll
+-rw-rw-r--   0 root         (0) root         (0)  1050543 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libiconv-2.dll
+-rw-rw-r--   0 root         (0) root         (0)   132717 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libintl-8.dll
+-rw-rw-r--   0 root         (0) root         (0)    24441 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libiso9660++-0.dll
+-rw-rw-r--   0 root         (0) root         (0)    76264 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libiso9660-10.dll
+-rw-rw-r--   0 root         (0) root         (0)    18412 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libsystre-0.dll
+-rw-rw-r--   0 root         (0) root         (0)    91386 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libtre-5.dll
+-rw-rw-r--   0 root         (0) root         (0)    27494 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libudf-0.dll
+-rw-rw-r--   0 root         (0) root         (0)    56978 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/libwinpthread-1.dll
+-rw-rw-r--   0 root         (0) root         (0)    70253 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/libcdio/win64/mmc-tool.exe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.424861 iromlab-1.0.9/iromlab/tools/shntool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.432861 iromlab-1.0.9/iromlab/tools/shntool/doc/
+-rw-rw-r--   0 root         (0) root         (0)    16233 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/doc/ChangeLog.txt
+-rw-rw-r--   0 root         (0) root         (0)     6798 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/doc/Credits.txt
+-rw-rw-r--   0 root         (0) root         (0)     2001 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/doc/Install.txt
+-rw-rw-r--   0 root         (0) root         (0)    33328 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/doc/shntool.pdf
+-rw-rw-r--   0 root         (0) root         (0)    33659 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/doc/shntool.txt
+-rw-rw-r--   0 root         (0) root         (0)   214016 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/tools/shntool/shntool.exe
+-rw-rw-r--   0 root         (0) root         (0)     3540 2020-08-24 11:54:50.000000 iromlab-1.0.9/iromlab/verifyaudio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:59:42.180859 iromlab-1.0.9/iromlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-24 12:01:12.000000 iromlab-1.0.9/iromlab.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 10:59:42.000000 iromlab-1.0.9/iromlab.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-05-04 10:59:42.432861 iromlab-1.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2422 2020-08-24 11:54:50.000000 iromlab-1.0.9/setup.py
```

### Comparing `iromlab-1.0.8/PKG-INFO` & `iromlab-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.2
 Name: iromlab
-Version: 1.0.8
+Version: 1.0.9
 Summary: Image and Rip Optical Media Like A Boss
 Home-page: https://github.com/KBNLresearch/iromlab
 Author: Johan van der Knijff
 Author-email: johan.vanderknijff@kb.nl
 Maintainer: Johan van der Knijff
 Maintainer-email: johan.vanderknijff@kb.nl
 License: Apache License 2.0
-Download-URL: https://github.com/KBNLresearch/iromlab/archive/1.0.8.tar.gz
+Download-URL: https://github.com/KBNLresearch/iromlab/archive/1.0.9.tar.gz
 Description: Loader software for automated imaging of optical media with Nimbie         disc robot 
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.2
```

### Comparing `iromlab-1.0.8/iromlab/cdinfo.py` & `iromlab-1.0.9/iromlab/cdinfo.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/cdworker.py` & `iromlab-1.0.9/iromlab/cdworker.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/conf/config.xml` & `iromlab-1.0.9/iromlab/conf/config.xml`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/config.py` & `iromlab-1.0.9/iromlab/config.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/configure.pyw` & `iromlab-1.0.9/iromlab/configure.pyw`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/dbpoweramp.py` & `iromlab-1.0.9/iromlab/dbpoweramp.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/drivers.py` & `iromlab-1.0.9/iromlab/drivers.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/iromlab.pyw` & `iromlab-1.0.9/iromlab/iromlab.pyw`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from . import config
 from .kbapi import sru
 from .socketserver import server
 from . import cdworker
 from . import cdinfo
 
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 config.version = __version__
 
 class carrierEntry(tk.Frame):
 
     """This class defines the graphical user interface + associated functions
     for associated actions
     """
```

### Comparing `iromlab-1.0.8/iromlab/isobuster.py` & `iromlab-1.0.9/iromlab/isobuster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #! /usr/bin/env python
 """Wrapper module for Isobuster"""
 
 import os
 import io
+import time
 from isolyzer import isolyzer
 from . import config
 from . import shared
 
 
 def extractData(writeDirectory, session, dataTrackLSNStart):
     """Extract data to ISO image using specified session number"""
@@ -33,14 +34,21 @@
     args.append("".join(["/tree:all:", reportFile, '?', reportFormatString]))
 
     # Command line as string (used for logging purposes only)
     cmdStr = " ".join(args)
 
     status, out, err = shared.launchSubProcess(args)
 
+    # For some reason sometimes a FileNotFoundError occurs on the log file, so
+    # we'll wait until it is actually available
+    logFileExists = False
+    while not logFileExists:
+        time.sleep(2)
+        logFileExists = os.path.isfile(logFile)
+
     # Open and read log file
     with io.open(logFile, "r", encoding="cp1252") as fLog:
         log = fLog.read()
     fLog.close()
 
     # Rewrite as UTF-8
     with io.open(logFile, "w", encoding="utf-8") as fLog:
@@ -158,14 +166,21 @@
     args.append("".join(["/tree:all:", reportFile, '?', reportFormatString]))
 
     # Command line as string (used for logging purposes only)
     cmdStr = " ".join(args)
 
     status, out, err = shared.launchSubProcess(args)
 
+    # For some reason sometimes a FileNotFoundError occurs on the log file, so
+    # we'll wait until it is actually available
+    logFileExists = False
+    while not logFileExists:
+        time.sleep(2)
+        logFileExists = os.path.isfile(logFile)
+
     # Open and read log file
     with io.open(logFile, "r", encoding="cp1252") as fLog:
         log = fLog.read()
     fLog.close()
 
     # Rewrite as UTF-8
     with io.open(logFile, "w", encoding="utf-8") as fLog:
```

### Comparing `iromlab-1.0.8/iromlab/kbapi/sru.py` & `iromlab-1.0.9/iromlab/kbapi/sru.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/mdo.py` & `iromlab-1.0.9/iromlab/mdo.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/shared.py` & `iromlab-1.0.9/iromlab/shared.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/socketserver/server.py` & `iromlab-1.0.9/iromlab/socketserver/server.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/testsru.py` & `iromlab-1.0.9/iromlab/testsru.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .kbapi import sru
 
 def main():
     """
     Script for testing SRU interface outside Iromlab
     (not used by main Iromlab application)
     """
-    catid = "184556155"
+    catid = "312537689"
 
     # Lookup catalog identifier
     #sruSearchString = '"PPN=' + str(catid) + '"'
     sruSearchString = 'OaiPmhIdentifier="GGC:AC:' + str(catid) + '"'
     print(sruSearchString)
     response = sru.search(sruSearchString, "GGC")
```

### Comparing `iromlab-1.0.8/iromlab/tools/flac/COPYING.FDL` & `iromlab-1.0.9/iromlab/tools/flac/COPYING.FDL`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/COPYING.GPL` & `iromlab-1.0.9/iromlab/tools/flac/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/COPYING.LGPL` & `iromlab-1.0.9/iromlab/tools/flac/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/COPYING.Xiph` & `iromlab-1.0.9/iromlab/tools/flac/COPYING.Xiph`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/changelog.html` & `iromlab-1.0.9/iromlab/tools/flac/html/changelog.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/developers.html` & `iromlab-1.0.9/iromlab/tools/flac/html/developers.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_bugs.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_bugs.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_example_code.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_example_code.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_format_overview.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_format_overview.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools_flac.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools_flac.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/documentation_tools_metaflac.html` & `iromlab-1.0.9/iromlab/tools/flac/html/documentation_tools_metaflac.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/faq.html` & `iromlab-1.0.9/iromlab/tools/flac/html/faq.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/favicon.ico` & `iromlab-1.0.9/iromlab/tools/flac/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/features.html` & `iromlab-1.0.9/iromlab/tools/flac/html/features.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/flac.css` & `iromlab-1.0.9/iromlab/tools/flac/html/flac.css`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/format.html` & `iromlab-1.0.9/iromlab/tools/flac/html/format.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/id.html` & `iromlab-1.0.9/iromlab/tools/flac/html/id.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/images/logo.svg` & `iromlab-1.0.9/iromlab/tools/flac/html/images/logo.svg`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/images/logo130.gif` & `iromlab-1.0.9/iromlab/tools/flac/html/images/logo130.gif`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/index.html` & `iromlab-1.0.9/iromlab/tools/flac/html/index.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/license.html` & `iromlab-1.0.9/iromlab/tools/flac/html/license.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/html/ogg_mapping.html` & `iromlab-1.0.9/iromlab/tools/flac/html/ogg_mapping.html`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/win32/flac.exe` & `iromlab-1.0.9/iromlab/tools/flac/win32/flac.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/win32/metaflac.exe` & `iromlab-1.0.9/iromlab/tools/flac/win32/metaflac.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/win64/flac.exe` & `iromlab-1.0.9/iromlab/tools/flac/win64/flac.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/flac/win64/metaflac.exe` & `iromlab-1.0.9/iromlab/tools/flac/win64/metaflac.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/readme.md` & `iromlab-1.0.9/iromlab/tools/libcdio/readme.md`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-drive.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-drive.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-info.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-info.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-paranoia.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-paranoia.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/cd-read.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/cd-read.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/iso-info.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/iso-info.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/iso-read.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/iso-read.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libcddb-2.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libcddb-2.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio++-0.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio++-0.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio-16.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio-16.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio_cdda-2.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio_cdda-2.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libcdio_paranoia-2.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libcdio_paranoia-2.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libiconv-2.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libiconv-2.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libintl-8.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libintl-8.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libiso9660++-0.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libiso9660++-0.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libiso9660-10.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libiso9660-10.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libsystre-0.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libsystre-0.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libtre-5.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libtre-5.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libudf-0.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libudf-0.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/libwinpthread-1.dll` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/libwinpthread-1.dll`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/libcdio/win64/mmc-tool.exe` & `iromlab-1.0.9/iromlab/tools/libcdio/win64/mmc-tool.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/doc/ChangeLog.txt` & `iromlab-1.0.9/iromlab/tools/shntool/doc/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/doc/Credits.txt` & `iromlab-1.0.9/iromlab/tools/shntool/doc/Credits.txt`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/doc/Install.txt` & `iromlab-1.0.9/iromlab/tools/shntool/doc/Install.txt`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/doc/shntool.pdf` & `iromlab-1.0.9/iromlab/tools/shntool/doc/shntool.pdf`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/doc/shntool.txt` & `iromlab-1.0.9/iromlab/tools/shntool/doc/shntool.txt`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/tools/shntool/shntool.exe` & `iromlab-1.0.9/iromlab/tools/shntool/shntool.exe`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab/verifyaudio.py` & `iromlab-1.0.9/iromlab/verifyaudio.py`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/iromlab.egg-info/PKG-INFO` & `iromlab-1.0.9/iromlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.2
 Name: iromlab
-Version: 1.0.8
+Version: 1.0.9
 Summary: Image and Rip Optical Media Like A Boss
 Home-page: https://github.com/KBNLresearch/iromlab
 Author: Johan van der Knijff
 Author-email: johan.vanderknijff@kb.nl
 Maintainer: Johan van der Knijff
 Maintainer-email: johan.vanderknijff@kb.nl
 License: Apache License 2.0
-Download-URL: https://github.com/KBNLresearch/iromlab/archive/1.0.8.tar.gz
+Download-URL: https://github.com/KBNLresearch/iromlab/archive/1.0.9.tar.gz
 Description: Loader software for automated imaging of optical media with Nimbie         disc robot 
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.2
```

### Comparing `iromlab-1.0.8/iromlab.egg-info/SOURCES.txt` & `iromlab-1.0.9/iromlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iromlab-1.0.8/setup.py` & `iromlab-1.0.9/setup.py`

 * *Files identical despite different names*

