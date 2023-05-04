# Comparing `tmp/solox-2.6.0.tar.gz` & `tmp/solox-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-oece9rip/solox-2.6.0.tar", last modified: Fri Apr 21 09:41:59 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-9295ic1y/solox-2.6.1.tar", last modified: Thu May  4 03:02:47 2023, max compression
```

## Comparing `solox-2.6.0.tar` & `solox-2.6.1.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-21 09:41:51.000000 solox-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-21 09:41:51.000000 solox-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-21 09:41:59.000000 solox-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-21 09:41:51.000000 solox-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-21 09:41:59.000000 solox-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-21 09:41:51.000000 solox-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 09:41:51.000000 solox-2.6.0/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 09:41:51.000000 solox-2.6.0/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-21 09:41:51.000000 solox-2.6.0/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41041 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39139 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-04-21 09:41:51.000000 solox-2.6.0/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-04-21 09:41:51.000000 solox-2.6.0/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    53512 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    92057 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-04-21 09:41:51.000000 solox-2.6.0/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-21 09:41:51.000000 solox-2.6.0/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-21 09:41:51.000000 solox-2.6.0/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 09:41:59.000000 solox-2.6.0/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 03:02:34.000000 solox-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 03:02:34.000000 solox-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-04 03:02:47.000000 solox-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-04 03:02:34.000000 solox-2.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-04 03:02:47.000000 solox-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 03:02:34.000000 solox-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 03:02:34.000000 solox-2.6.1/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 03:02:34.000000 solox-2.6.1/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 03:02:34.000000 solox-2.6.1/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   100609 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-04 03:02:34.000000 solox-2.6.1/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.0/LICENSE` & `solox-2.6.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 SoloX . Rafa Chen
+Copyright (c) 2022 ~ now SoloX . Rafa Chen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `solox-2.6.0/setup.py` & `solox-2.6.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['flask>=2.0.1', 'requests', 'logzero', 'Flask-SocketIO==4.3.1', 'fire',
                       'python-engineio==3.13.2', 'python-socketio==4.6.0', 'Werkzeug==2.0.3',
-                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt'],
+                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt','py-ios-device'],
     version=__version__,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="SoloX - Real-time collection tool for Android/iOS performance data.",
     packages=setuptools.find_namespace_packages(include=["solox", "solox.*"], ),
     include_package_data=True
 )
```

### Comparing `solox-2.6.0/solox/debug.py` & `solox-2.6.1/solox/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 import webbrowser
 import requests
 import socket
 import sys
 from view.apis import api
 from view.pages import page
+from public.adb import adb
 from logzero import logger
 from threading import Lock
 from flask_socketio import SocketIO, disconnect
 from flask import Flask
 import fire as fire
 import signal
 
@@ -40,18 +41,22 @@
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
+        logger.info('Initializing adb environment ...')
+        os.system('adb kill-server')
+        os.system('adb start-server')
         current_time = time.strftime("%Y%m%d%H", time.localtime())
         logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
         logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
+        
         with open(logPath, "r") as f:
             while thread:
                 socketio.sleep(1)
                 for line in f.readlines():
                     socketio.emit('message', {'data': line}, namespace='/logcat')
         if logcat.poll() == 0:
             thread = False
```

### Comparing `solox-2.6.0/solox/public/_iosPerf.py` & `solox-2.6.1/solox/public/_iosPerf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import enum
 import threading
 import time
 import typing
 from collections import defaultdict, namedtuple
 from typing import Any, Iterator, Optional, Tuple, Union
 import weakref
-
 from solox.public.iosperf._device import BaseDevice
 from solox.public.iosperf._proto import *
 
 
 class DataType(str, enum.Enum):
     SCREENSHOT = "screenshot"
     CPU = "cpu"
```

### Comparing `solox-2.6.0/solox/public/adb/mac/adb` & `solox-2.6.1/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/adb.py` & `solox-2.6.1/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/apm.py` & `solox-2.6.1/solox/public/apm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import re
 import time
 import os
+import traceback
 from logzero import logger
 import tidevice
+import multiprocessing
 import solox.public._iosPerf as iosP
 from solox.public.iosperf._perf import DataType, Performance
 from solox.public.adb import adb
 from solox.public.common import Devices, File, Method, Platform
 from solox.public.fps import FPSMonitor, TimeUtils
 
 d = Devices()
@@ -50,15 +52,15 @@
         totalCpu = 0
         for i in range(1, 9):
             totalCpu += float(toks[i])
         return float(totalCpu)
 
     def getCpuCores(self):
         """get Android cpu cores"""
-        cmd = f'cat /sys/devices/system/cpu/online'
+        cmd = 'cat /sys/devices/system/cpu/online'
         result = adb.shell(cmd=cmd, deviceId=self.deviceId)
         try:
             nums = int(result.split('-')[1]) + 1
         except:
             nums = 1
         return nums
 
@@ -335,62 +337,163 @@
             perf = iosP.Performance(self.deviceId, [perfTpe])
             perf_value = perf.start(self.pkgName, callback=self.callback)
         return perf_value
 
 class APM(object):
     """for python api"""
 
-    def __init__(self, pkgName, deviceId=None, platform=Platform.Android, surfaceview=True, noLog=True, pid=None):
+    def __init__(self, pkgName, platform=Platform.Android, deviceId=None,
+                 surfaceview=True, noLog=True, pid=None, duration=0):
         self.pkgName = pkgName
         self.deviceId = deviceId
         self.platform = platform
         self.surfaceview = surfaceview
         self.noLog = noLog
         self.pid = pid
+        self.duration = duration
+        self.end_time = time.time() + self.duration
         d.devicesCheck(platform=self.platform, deviceid=self.deviceId, pkgname=self.pkgName)
 
     def collectCpu(self):
         _cpu = CPU(self.pkgName, self.deviceId, self.platform, pid=self.pid)
-        appCpuRate, systemCpuRate = _cpu.getCpuRate(noLog=self.noLog)
-        result = {'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}
-        logger.info(f'cpu: {result}')
+        result = {}
+        while True:
+            appCpuRate, systemCpuRate = _cpu.getCpuRate(noLog=self.noLog)
+            result = {'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}
+            logger.info(f'cpu: {result}')
+            if time.time() > self.end_time:
+                break
         return result
 
     def collectMemory(self):
         _memory = MEM(self.pkgName, self.deviceId, self.platform, pid=self.pid)
-        totalPass, nativePass, dalvikPass = _memory.getProcessMem(noLog=self.noLog)
-        result = {'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
-        logger.info(f'memory: {result}')
+        result = {}
+        while True:
+            totalPass, nativePass, dalvikPass = _memory.getProcessMem(noLog=self.noLog)
+            result = {'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
+            logger.info(f'memory: {result}')
+            if time.time() > self.end_time:
+                break
         return result
 
     def collectBattery(self):
         _battery = Battery(self.deviceId, self.platform)
-        final = _battery.getBattery(noLog=self.noLog)
-        if self.platform == Platform.Android:
-            result = {'level': final[0], 'temperature': final[1]}
-        else:
-            result = {'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]}
-        logger.info(f'battery: {result}')
+        result = {}
+        while True:
+            final = _battery.getBattery(noLog=self.noLog)
+            if self.platform == Platform.Android:
+                result = {'level': final[0], 'temperature': final[1]}
+            else:
+                result = {'temperature': final[0], 'current': final[1], 'voltage': final[2], 'power': final[3]}
+            logger.info(f'battery: {result}')
+            if time.time() > self.end_time:
+                break
         return result
 
     def collectFlow(self, wifi=True):
         _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
-        upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,noLog=self.noLog)
-        result = {'upFlow': upFlow, 'downFlow': downFlow}
-        logger.info(f'network: {result}')
+        if self.noLog is False:
+            data = _flow.setAndroidNet(wifi=wifi)
+            f.record_net('pre', data[0], data[1])
+        result = {}
+        while True:
+            upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,noLog=self.noLog)
+            result = {'upFlow': upFlow, 'downFlow': downFlow}
+            logger.info(f'network: {result}')
+            if time.time() > self.end_time:
+                break
         return result
 
     def collectFps(self):
         _fps = FPS(self.pkgName, self.deviceId, self.platform, self.surfaceview)
-        fps, jank = _fps.getFPS(noLog=self.noLog)
-        result = {'fps': fps, 'jank': jank}
-        logger.info(f'fps: {result}')
+        result = {}
+        while True:
+            fps, jank = _fps.getFPS(noLog=self.noLog)
+            result = {'fps': fps, 'jank': jank}
+            logger.info(f'fps: {result}')
+            if time.time() > self.end_time:
+                break
         return result
     
     def collectGpu(self):
         _gpu = GPU(self.pkgName)
-        if self.platform == Platform.Android:
-            raise Exception('not support android')
-        gpu = _gpu.getGPU(noLog=self.noLog)
-        result = {'gpu': gpu}
-        logger.info(f'gpu: {result}')
+        result = {}
+        while True:
+            if self.platform == Platform.Android:
+                raise Exception('not support android')
+            gpu = _gpu.getGPU(noLog=self.noLog)
+            result = {'gpu': gpu}
+            logger.info(f'gpu: {result}')
+            if time.time() > self.end_time:
+                break
         return result
+    
+
+    def collectAll(self):
+        try:
+            f.clear_file()
+            pool = multiprocessing.Pool(processes=6)
+            pool.apply_async(self.collectCpu)
+            pool.apply_async(self.collectMemory)
+            pool.apply_async(self.collectBattery)
+            pool.apply_async(self.collectFps)
+            pool.apply_async(self.collectFlow)
+            pool.apply_async(self.collectGpu)
+            pool.close()
+            pool.join()
+            match(self.platform):
+                case Platform.Android:
+                    adb.shell(cmd='dumpsys battery reset', deviceId=self.deviceId)
+                    _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
+                    data = _flow.setAndroidNet()
+                    f.record_net('end', data[0], data[1])
+                    scene = f.make_report(app=self.pkgName, devices=self.deviceId, 
+                                          platform=self.platform, model='normal')
+                    summary = f._setAndroidPerfs(scene)
+                    summary_dict = {}
+                    summary_dict['cpu_app'] = summary['cpuAppRate']
+                    summary_dict['cpu_sys'] = summary['cpuSystemRate']
+                    summary_dict['mem_total'] = summary['totalPassAvg']
+                    summary_dict['mem_native'] = summary['nativePassAvg']
+                    summary_dict['mem_dalvik'] = summary['dalvikPassAvg']
+                    summary_dict['fps'] = summary['fps']
+                    summary_dict['jank'] = summary['jank']
+                    summary_dict['level'] = summary['batteryLevel']
+                    summary_dict['tem'] = summary['batteryTeml']
+                    summary_dict['net_send'] = summary['flow_send']
+                    summary_dict['net_recv'] = summary['flow_recv']
+                    summary_dict['cpu_charts'] = f.getCpuLog(Platform.Android, scene)
+                    summary_dict['mem_charts'] = f.getMemLog(Platform.Android, scene)
+                    summary_dict['net_charts'] = f.getFlowLog(Platform.Android, scene)
+                    summary_dict['battery_charts'] = f.getBatteryLog(Platform.Android, scene)
+                    summary_dict['fps_charts'] = f.getFpsLog(Platform.Android, scene)['fps']
+                    summary_dict['jank_charts'] = f.getFpsLog(Platform.Android, scene)['jank']
+                    f.make_android_html(scene=scene, summary=summary_dict)
+                case Platform.iOS:
+                    scene = f.make_report(app=self.pkgName, devices=self.deviceId, 
+                                          platform=self.platform, model='normal')
+                    summary = f._setiOSPerfs(scene)
+                    summary_dict = {}
+                    summary_dict['cpu_app'] = summary['cpuAppRate']
+                    summary_dict['cpu_sys'] = summary['cpuSystemRate']
+                    summary_dict['mem_total'] = summary['totalPassAvg']
+                    summary_dict['fps'] = summary['fps']
+                    summary_dict['current'] = summary['batteryCurrent']
+                    summary_dict['voltage'] = summary['batteryVoltage']
+                    summary_dict['power'] = summary['batteryPower']
+                    summary_dict['tem'] = summary['batteryTeml']
+                    summary_dict['gpu'] = summary['gpu']
+                    summary_dict['net_send'] = summary['flow_send']
+                    summary_dict['net_recv'] = summary['flow_recv']
+                    summary_dict['cpu_charts'] = f.getCpuLog(Platform.iOS, scene)
+                    summary_dict['mem_charts'] = f.getMemLog(Platform.iOS, scene)
+                    summary_dict['net_charts'] = f.getFlowLog(Platform.iOS, scene)
+                    summary_dict['battery_charts'] = f.getBatteryLog(Platform.iOS, scene)
+                    summary_dict['fps_charts'] = f.getFpsLog(Platform.iOS, scene)
+                    summary_dict['gpu_charts'] = f.getGpuLog(Platform.iOS, scene)
+                    f.make_ios_html(scene=scene, summary=summary_dict)
+                case _:
+                    raise Exception('platfrom is invalid')        
+        except KeyboardInterrupt:
+            logger.info('End of testing')
+        except Exception:
+            traceback.print_exc()
```

### Comparing `solox-2.6.0/solox/public/apm_pk.py` & `solox-2.6.1/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/common.py` & `solox-2.6.1/solox/public/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         devices_name = os.popen(f'{self.adb} -s {deviceId} shell getprop ro.product.model').readlines()
         return devices_name[0].strip()
 
     def getDevices(self):
         """Get all Android devices"""
         DeviceIds = self.getDeviceIds()
         Devices = [f'{id}({self.getDevicesName(id)})' for id in DeviceIds]
+        logger.info('Connected devices: {}'.format(Devices))
         return Devices
 
     def getIdbyDevice(self, deviceinfo, platform):
         """Obtain the corresponding device id according to the Android device information"""
         if platform == Platform.Android:
             deviceId = re.sub(u"\\(.*?\\)|\\{.*?}|\\[.*?]", "", deviceinfo)
             if deviceId not in self.getDeviceIds():
@@ -104,33 +105,34 @@
         """Get a list of all successfully connected iOS devices"""
         deviceResult = json.loads(self.execCmd('tidevice list --json'))
         deviceInfo = []
         for i in range(len(deviceResult)):
             deviceName = deviceResult[i]['name']
             deviceUdid = deviceResult[i]['udid']
             deviceInfo.append(f'{deviceName}:{deviceUdid}')
+        logger.info('Connected devices: {}'.format(deviceInfo))    
         return deviceInfo
 
     def getPkgnameByiOS(self, udid):
         """Get all package names of the corresponding iOS device"""
         pkgResult = self.execCmd(f'tidevice --udid {udid} applist').split('\n')
         pkgNames = [pkgResult[i].split(' ')[0] for i in range(len(pkgResult))]
         return pkgNames
 
     def devicesCheck(self, platform, deviceid=None, pkgname=None):
         """Check the device environment"""
         match(platform):
             case Platform.Android:
                 if len(self.getDeviceIds()) == 0:
-                    raise Exception('no devices')
-                if not self.getPid(deviceId=deviceid, pkgName=pkgname):
-                    raise Exception('no found app process')
+                    raise Exception('no devices found')
+                if len(self.getPid(deviceId=deviceid, pkgName=pkgname)) == 0:
+                    raise Exception('no process found')
             case Platform.iOS:
                 if len(self.getDeviceInfoByiOS()) == 0:
-                    raise Exception('no devices')
+                    raise Exception('no devices found')
             case _:
                 raise Exception('platform must be Android or iOS')        
             
     def getDdeviceDetail(self, deviceId, platform):
         result = {}
         match(platform):
             case Platform.Android:
@@ -145,22 +147,47 @@
                 result['brand'] = iosInfo['DeviceClass']
                 result['name'] = iosInfo['DeviceName']
                 result['version'] = iosInfo['ProductVersion']
                 result['serialno'] = iosInfo['SerialNumber']
                 result['wifiadr'] = iosInfo['WiFiAddress']
             case _:
                 raise Exception('{} is undefined'.format(platform)) 
-        return result       
+        return result
+
+    def getCurrentActivity(self, deviceId):
+        result = adb.shell(cmd='dumpsys window | {} mCurrentFocus'.format(self.filterType()), deviceId=deviceId)
+        if result.__contains__('mCurrentFocus'):
+            activity = str(result).split(' ')[-1].replace('}','') 
+            return activity
+        else:
+            raise Exception('no activity found')
+
+    def getStartupTimeByAndroid(self, activity, deviceId):
+        result = adb.shell(cmd='am start -W {}'.format(activity), deviceId=deviceId)
+        return result
+
+    def getStartupTimeByiOS(self, pkgname):
+        result = self.execCmd('pyidevice instruments app_lifecycle -b {}'.format(pkgname))
+        return result          
 
 class File:
 
     def __init__(self, fileroot='.'):
         self.fileroot = fileroot
         self.report_dir = self.get_repordir()
-    
+
+    def clear_file(self):
+        logger.info('Clean up useless files ...')
+        if os.path.exists(self.report_dir):
+            for f in os.listdir(self.report_dir):
+                filename = os.path.join(self.report_dir, f)
+                if f.split(".")[-1] in ['log', 'json']:
+                    os.remove(filename)
+        logger.info('Clean up useless files success')            
+
     def export_excel(self, platform, scene):
         logger.info('Exporting excel ...')
         android_log_file_list = ['cpu_app','cpu_sys','mem_total','mem_native','mem_dalvik',
                                  'battery_level', 'battery_tem','upflow','downflow','fps']
         ios_log_file_list = ['cpu_app','cpu_sys', 'mem_total', 'battery_tem', 'battery_current', 
                              'battery_voltage', 'battery_power','upflow','downflow','fps','gpu']
         log_file_list = android_log_file_list if platform == 'Android' else ios_log_file_list
@@ -226,14 +253,19 @@
                                            net_charts=summary['net_charts'],battery_charts=summary['battery_charts'],
                                            fps_charts=summary['fps_charts'],gpu_charts=summary['gpu_charts'])            
             fout.write(html_content)
         html_path = os.path.join(self.report_dir, scene, 'report.html')    
         logger.info('Generating HTML success : {}'.format(html_path))  
         return html_path
   
+    def filter_secen(self, scene):
+        dirs = os.listdir(self.report_dir)
+        dir_list = list(reversed(sorted(dirs, key=lambda x: os.path.getmtime(os.path.join(self.report_dir, x)))))
+        dir_list.remove(scene)
+        return dir_list
 
     def get_repordir(self):
         report_dir = os.path.join(os.getcwd(), 'report')
         if not os.path.exists(report_dir):
             os.mkdir(report_dir)
         return report_dir
 
@@ -262,34 +294,35 @@
                 content = json.dumps(net_dict)
                 self.create_file(filename='end_net.json', content=content)
             case _:
                 logger.error('record network data failed')
     
     def make_report(self, app, devices, platform='Android', model='normal'):
         logger.info('Generating test results ...')
-        current_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+        current_time = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
         result_dict = {
             "app": app,
             "icon": "",
             "platform": platform,
             "model": model,
             "devices": devices,
             "ctime": current_time
         }
         content = json.dumps(result_dict)
         self.create_file(filename='result.json', content=content)
-        report_new_dir = os.path.join(self.report_dir, self.fileroot)
+        report_new_dir = os.path.join(self.report_dir, f'apm_{current_time}')
         if not os.path.exists(report_new_dir):
             os.mkdir(report_new_dir)
 
         for f in os.listdir(self.report_dir):
             filename = os.path.join(self.report_dir, f)
             if f.split(".")[-1] in ['log', 'json']:
-                shutil.move(filename, report_new_dir)
-        logger.info('Generating test results success: {}'.format(report_new_dir))        
+                shutil.move(filename, report_new_dir)        
+        logger.info('Generating test results success: {}'.format(report_new_dir))
+        return f'apm_{current_time}'        
 
     def instance_type(self, data):
         if isinstance(data, float):
             return 'float'
         elif isinstance(data, int):
             return 'int'
         else:
@@ -321,34 +354,55 @@
     def getCpuLog(self, platform, scene):
         targetDic = {}
         targetDic['cpuAppData'] = self.readLog(scene=scene, filename='cpu_app.log')[0]
         targetDic['cpuSysData'] = self.readLog(scene=scene, filename='cpu_sys.log')[0]
         result = {'status': 1, 'cpuAppData': targetDic['cpuAppData'], 'cpuSysData': targetDic['cpuSysData']}
         return result
     
+    def getCpuLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='cpu_app.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='cpu_app.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
+    
     def getGpuLog(self, platform, scene):
         targetDic = {}
         targetDic['gpu'] = self.readLog(scene=scene, filename='gpu.log')[0]
         result = {'status': 1, 'gpu': targetDic['gpu']}
         return result
     
+    def getGpuLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='gpu.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='gpu.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
+    
     def getMemLog(self, platform, scene):
         targetDic = {}
         targetDic['memTotalData'] = self.readLog(scene=scene, filename='mem_total.log')[0]
         if platform == Platform.Android:
             targetDic['memNativeData']  = self.readLog(scene=scene, filename='mem_native.log')[0]
             targetDic['memDalvikData']  = self.readLog(scene=scene, filename='mem_dalvik.log')[0]
             result = {'status': 1, 
                       'memTotalData': targetDic['memTotalData'], 
                       'memNativeData': targetDic['memNativeData'],
                       'memDalvikData': targetDic['memDalvikData']}
         else:
             result = {'status': 1, 'memTotalData': targetDic['memTotalData']}
         return result
     
+    def getMemLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='mem_total.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='mem_total.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
+    
     def getBatteryLog(self, platform, scene):
         targetDic = {}
         if platform == Platform.Android:
             targetDic['batteryLevel'] = self.readLog(scene=scene, filename='battery_level.log')[0]
             targetDic['batteryTem'] = self.readLog(scene=scene, filename='battery_tem.log')[0]
             result = {'status': 1, 
                       'batteryLevel': targetDic['batteryLevel'], 
@@ -361,30 +415,63 @@
             result = {'status': 1, 
                       'batteryTem': targetDic['batteryTem'], 
                       'batteryCurrent': targetDic['batteryCurrent'],
                       'batteryVoltage': targetDic['batteryVoltage'], 
                       'batteryPower': targetDic['batteryPower']}    
         return result
     
+    def getBatteryLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        if platform == Platform.Android:
+            targetDic['scene1'] = self.readLog(scene=scene1, filename='battery_level.log')[0]
+            targetDic['scene2'] = self.readLog(scene=scene2, filename='battery_level.log')[0]
+            result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        else:
+            targetDic['scene1'] = self.readLog(scene=scene1, filename='batteryPower.log')[0]
+            targetDic['scene2'] = self.readLog(scene=scene2, filename='batteryPower.log')[0]
+            result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}    
+        return result
+    
     def getFlowLog(self, platform, scene):
         targetDic = {}
         targetDic['upFlow'] = self.readLog(scene=scene, filename='upflow.log')[0]
         targetDic['downFlow'] = self.readLog(scene=scene, filename='downflow.log')[0]
         result = {'status': 1, 'upFlow': targetDic['upFlow'], 'downFlow': targetDic['downFlow']}
         return result
     
+    def getFlowSendLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='upflow.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='upflow.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
+    
+    def getFlowRecvLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='downflow.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='downflow.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
+    
     def getFpsLog(self, platform, scene):
         targetDic = {}
         targetDic['fps'] = self.readLog(scene=scene, filename='fps.log')[0]
         if platform == Platform.Android:
             targetDic['jank'] = self.readLog(scene=scene, filename='jank.log')[0]
             result = {'status': 1, 'fps': targetDic['fps'], 'jank': targetDic['jank']}
         else:
             result = {'status': 1, 'fps': targetDic['fps']}     
         return result
+
+    def getFpsLogCompare(self, platform, scene1, scene2):
+        targetDic = {}
+        targetDic['scene1'] = self.readLog(scene=scene1, filename='fps.log')[0]
+        targetDic['scene2'] = self.readLog(scene=scene2, filename='fps.log')[0]
+        result = {'status': 1, 'scene1': targetDic['scene1'], 'scene2': targetDic['scene2']}
+        return result
         
     def approximateSize(self, size, a_kilobyte_is_1024_bytes=True):
         '''
         convert a file size to human-readable form.
         Keyword arguments:
         size -- file size in bytes
         a_kilobyte_is_1024_bytes -- if True (default),use multiples of 1024
@@ -596,15 +683,15 @@
             pbar.close()
             return True
         except:
             traceback.print_exc()
             return False
 
     def installAPK(self, path):
-        result = adb.shell_noDevice(cmd = 'install -r {}'.format(path))
+        result = adb.shell_noDevice(cmd='install -r {}'.format(path))
         if result == 0:
             os.remove(path)
             return True, result
         else:
             return False, result
 
     def installIPA(self, path):
```

### Comparing `solox-2.6.0/solox/public/fps.py` & `solox-2.6.1/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/__main__.py` & `solox-2.6.1/solox/public/iosperf/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 from typing import Optional, Union
 
 import requests
 from logzero import setup_logger
 from tabulate import tabulate
 from loguru import logger as ulogger
 
-from ._device import Device
-from ._imagemounter import cache_developer_image
-from ._ipautil import IPAReader
-from ._perf import DataType
-from ._proto import LOG, MODELS, PROGRAM_NAME
-from ._relay import relay
-from ._types import ConnectionType
-from ._usbmux import Usbmux
-from ._utils import get_app_dir, get_binary_by_name, is_atty
-from ._version import __version__
-from ._wdaproxy import WDAService
-from .exceptions import MuxError, MuxServiceError, ServiceError
+from solox.public.iosperf._device import Device
+from solox.public.iosperf._imagemounter import cache_developer_image
+from solox.public.iosperf._ipautil import IPAReader
+from solox.public.iosperf._perf import DataType
+from solox.public.iosperf._proto import LOG, MODELS, PROGRAM_NAME
+from solox.public.iosperf._relay import relay
+from solox.public.iosperf._types import ConnectionType
+from solox.public.iosperf._usbmux import Usbmux
+from solox.public.iosperf._utils import get_app_dir, get_binary_by_name, is_atty
+from solox.public.iosperf._version import __version__
+from solox.public.iosperf._wdaproxy import WDAService
+from solox.public.iosperf.exceptions import MuxError, MuxServiceError, ServiceError
 
 um: Usbmux = None  # Usbmux
 logger = logging.getLogger(PROGRAM_NAME)
 
 
 # ulogger.remove()
 # ulogger.add(sys.stderr, level="INFO")
```

### Comparing `solox-2.6.0/solox/public/iosperf/_crash.py` & `solox-2.6.1/solox/public/iosperf/_crash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from genericpath import isdir
-from ._sync import Sync
+from solox.public.iosperf._sync import Sync
 import logging
-from ._proto import LOG
-from ._safe_socket import PlistSocketProxy
+from solox.public.iosperf._proto import LOG
+from solox.public.iosperf._safe_socket import PlistSocketProxy
 
 
 logger = logging.getLogger(LOG.main)
 
 # Ref: https://github.com/libimobiledevice/libimobiledevice/blob/master/tools/idevicecrashreport.c
 
 class CrashManager:
```

### Comparing `solox-2.6.0/solox/public/iosperf/_device.py` & `solox-2.6.1/solox/public/iosperf/_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 from typing import Iterator, Optional, Union
 
 import requests
 from deprecation import deprecated
 from logzero import setup_logger
 from PIL import Image
 
-from . import bplist
-from ._crash import CrashManager
-from ._imagemounter import ImageMounter, cache_developer_image
-from ._installation import Installation
-from ._instruments import (AUXMessageBuffer, DTXMessage, DTXService, Event,
+from solox.public.iosperf import bplist
+from solox.public.iosperf._crash import CrashManager
+from solox.public.iosperf._imagemounter import ImageMounter, cache_developer_image
+from solox.public.iosperf._installation import Installation
+from solox.public.iosperf._instruments import (AUXMessageBuffer, DTXMessage, DTXService, Event,
                            ServiceInstruments)
-from ._ipautil import IPAReader
-from ._proto import *
-from ._safe_socket import *
-from ._sync import Sync
-from ._types import DeviceInfo
-from ._usbmux import Usbmux
-from ._utils import ProgressReader, get_app_dir, set_socket_timeout
-from .exceptions import *
+from solox.public.iosperf._ipautil import IPAReader
+from solox.public.iosperf._proto import *
+from solox.public.iosperf._safe_socket import *
+from solox.public.iosperf._sync import Sync
+from solox.public.iosperf._types import DeviceInfo
+from solox.public.iosperf._usbmux import Usbmux
+from solox.public.iosperf._utils import ProgressReader, get_app_dir, set_socket_timeout
+from solox.public.iosperf.exceptions import *
 
 logger = logging.getLogger(LOG.main)
 
 
 def pil_imread(data: Union[str, pathlib.Path, bytes, bytearray]) -> Image.Image:
     """ Convert data(path, binary) to PIL.Image.Image
```

### Comparing `solox-2.6.0/solox/public/iosperf/_hexdump.py` & `solox-2.6.1/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/_imagemounter.py` & `solox-2.6.1/solox/public/iosperf/_imagemounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import typing
 import zipfile
 from typing import List
 
 import retry
 import requests
 
-from ._safe_socket import PlistSocketProxy
-from ._utils import get_app_dir, logger
-from .exceptions import MuxError, MuxServiceError
+from solox.public.iosperf._safe_socket import PlistSocketProxy
+from solox.public.iosperf._utils import get_app_dir, logger
+from solox.public.iosperf.exceptions import MuxError, MuxServiceError
 
 _REQUESTS_TIMEOUT = 30.0
 
 
 @retry.retry(exceptions=requests.ReadTimeout, tries=5, delay=.5)
 def _urlretrieve(url, local_filename):
     """ download url to local """
```

### Comparing `solox-2.6.0/solox/public/iosperf/_installation.py` & `solox-2.6.1/solox/public/iosperf/_installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 #  - SandboxingApplication (80%)
 #  - GeneratingApplicationMap (90%)
 #  - Complete
 
 import logging
 from typing import Optional
 
-from ._proto import LOG
-from ._safe_socket import PlistSocketProxy
-from .exceptions import ServiceError
+from solox.public.iosperf._proto import LOG
+from solox.public.iosperf._safe_socket import PlistSocketProxy
+from solox.public.iosperf.exceptions import ServiceError
 
 logger = logging.getLogger(LOG.main)
 
 
 class Installation(PlistSocketProxy):
     SERVICE_NAME = "com.apple.mobile.installation_proxy"
```

### Comparing `solox-2.6.0/solox/public/iosperf/_instruments.py` & `solox-2.6.1/solox/public/iosperf/_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 import typing
 import weakref
 from collections import defaultdict, namedtuple
 from typing import Any, Iterator, List, Optional, Tuple, Union
 
 from retry import retry
 
-from . import bplist
-from . import struct2 as ct
-from ._proto import LOG, InstrumentsService
-from ._safe_socket import PlistSocketProxy
-from .exceptions import MuxError, ServiceError
+from solox.public.iosperf import bplist
+from solox.public.iosperf import struct2 as ct
+from solox.public.iosperf._proto import LOG, InstrumentsService
+from solox.public.iosperf._safe_socket import PlistSocketProxy
+from solox.public.iosperf.exceptions import MuxError, ServiceError
 
 logger = logging.getLogger(LOG.xctest)
 
 DTXMessageHeader = ct.Struct("DTXMessageHeader",
     ct.UInt32("magic", 0x1F3D5B79),
     ct.UInt32("header_length", 0x20),
     ct.UInt16("fragment_id", 0),
```

### Comparing `solox-2.6.0/solox/public/iosperf/_ipautil.py` & `solox-2.6.1/solox/public/iosperf/_ipautil.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import sys
 import tempfile
 import typing
 import zipfile
 from pprint import pprint
 from typing import Union
 
-from . import bplist, plistlib2
-from ._compat import cache
-from .exceptions import IPAError
+from solox.public.iosperf import bplist, plistlib2
+from solox.public.iosperf._compat import cache
+from solox.public.iosperf.exceptions import IPAError
 
 
 class IPAReader(zipfile.ZipFile):
     def get_infoplist_zipinfo(self) -> zipfile.ZipInfo:
         re_infoplist = re.compile(r"^Payload/[^/]+\.app/Info.plist$")
         for zipinfo in self.filelist:
             if re_infoplist.match(zipinfo.filename):
```

### Comparing `solox-2.6.0/solox/public/iosperf/_perf.py` & `solox-2.6.1/solox/public/iosperf/_perf.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import time
 import typing
 import uuid
 from collections import defaultdict, namedtuple
 from typing import Any, Iterator, Optional, Tuple, Union
 import weakref
 
-from ._device import BaseDevice
-from ._proto import *
+from solox.public.iosperf._device import BaseDevice
+from solox.public.iosperf._proto import *
 
 
 class DataType(str, enum.Enum):
     SCREENSHOT = "screenshot"
     CPU = "cpu"
     MEMORY = "memory"
     NETWORK = "network"  # 流量
```

### Comparing `solox-2.6.0/solox/public/iosperf/_proto.py` & `solox-2.6.1/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/_relay.py` & `solox-2.6.1/solox/public/iosperf/_relay.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import colored
 import simple_tornado
 from logzero import logger
 from tornado.ioloop import IOLoop
 from tornado.iostream import IOStream, StreamClosedError
 from tornado.tcpserver import TCPServer
 
-from ._device import Device
-from ._hexdump import hexdump
-from ._safe_socket import PlistSocketProxy
-from .exceptions import MuxReplyError
+from solox.public.iosperf._device import Device
+from solox.public.iosperf._hexdump import hexdump
+from solox.public.iosperf._safe_socket import PlistSocketProxy
+from solox.public.iosperf.exceptions import MuxReplyError
 
 
 class RelayTCPServer(TCPServer):
     def __init__(self, device: Device, device_port: int, debug: bool = False):
         """
         Args:
             port (int): forward to port
```

### Comparing `solox-2.6.0/solox/public/iosperf/_safe_socket.py` & `solox-2.6.1/solox/public/iosperf/_safe_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import ssl
 import struct
 import threading
 import typing
 import weakref
 from typing import Any, Union
 
-from ._proto import PROGRAM_NAME
-from ._utils import set_socket_timeout
-from .exceptions import *
+from solox.public.iosperf._proto import PROGRAM_NAME
+from solox.public.iosperf._utils import set_socket_timeout
+from solox.public.iosperf.exceptions import *
 
 from loguru import logger
 
 
 _n = [0]
 _nlock = threading.Lock()
 _id_numbers = []
```

### Comparing `solox-2.6.0/solox/public/iosperf/_ssl.py` & `solox-2.6.1/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/_sync.py` & `solox-2.6.1/solox/public/iosperf/_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 import pathlib
 import re
 import struct
 import typing
 from collections import namedtuple
 from typing import Iterator, List, Union
 
-from . import bplist
-from . import struct2 as ct
-from ._proto import *
-from ._safe_socket import PlistSocketProxy
-from ._utils import pathjoin
-from .exceptions import MuxError, MuxServiceError
+from solox.public.iosperf import bplist
+from solox.public.iosperf import struct2 as ct
+from solox.public.iosperf._proto import *
+from solox.public.iosperf._safe_socket import PlistSocketProxy
+from solox.public.iosperf._utils import pathjoin
+from solox.public.iosperf.exceptions import MuxError, MuxServiceError
 
 # 00000000: 43 46 41 36 4C 50 41 41  84 00 00 00 00 00 00 00  magic(CFA6LPAA), length(0x84)
 # 00000010: 28 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00  unknown(0x28), tag(0x0)
 # 00000020: 02 00 00 00 00 00 00 00                           operation(0x02)
 #
 # Ref: https://github.com/anonymous5l/iConsole/blob/master/services/afc.go
```

### Comparing `solox-2.6.0/solox/public/iosperf/_types.py` & `solox-2.6.1/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/_usbmux.py` & `solox-2.6.1/solox/public/iosperf/_usbmux.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import pprint
 import socket
 import sys
 import typing
 import uuid
 from typing import Optional, Union
 
-from ._types import DeviceInfo, ConnectionType
-from ._proto import PROGRAM_NAME, UsbmuxReplyCode, LOG
-from ._safe_socket import PlistSocket, PlistSocketProxy
-from .exceptions import * # pragma warning disables S2208
+from solox.public.iosperf._types import DeviceInfo, ConnectionType
+from solox.public.iosperf._proto import PROGRAM_NAME, UsbmuxReplyCode, LOG
+from solox.public.iosperf._safe_socket import PlistSocket, PlistSocketProxy
+from solox.public.iosperf.exceptions import * # pragma warning disables S2208
 
 
 logger = logging.getLogger(LOG.main)
 
 class Usbmux:
     def __init__(self, address: Optional[Union[str, tuple]] = None):
         if address is None:
```

### Comparing `solox-2.6.0/solox/public/iosperf/_utils.py` & `solox-2.6.1/solox/public/iosperf/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import socket
 import subprocess
 import sys
 import threading
 import time
 import typing
 
-from ._proto import PROGRAM_NAME
+from solox.public.iosperf._proto import PROGRAM_NAME
 
 logger = logging.getLogger(PROGRAM_NAME)
 is_atty = getattr(sys.stdout, 'isatty', lambda: False)()
 
 
 def get_app_dir(*paths) -> str:
     home = os.path.expanduser("~")
```

### Comparing `solox-2.6.0/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.1/solox/public/iosperf/_wdaproxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import time
 import typing
 import traceback
 
 import logzero
 import requests
 
-from . import requests_usbmux
-from ._device import Device
-from ._proto import UsbmuxReplyCode
-from .exceptions import MuxReplyError
+from solox.public.iosperf import requests_usbmux
+from solox.public.iosperf._device import Device
+from solox.public.iosperf._proto import UsbmuxReplyCode
+from solox.public.iosperf.exceptions import MuxReplyError
 
 
 class WDAService:
     _DEFAULT_TIMEOUT = 90 # http request timeout
 
     def __init__(self, d: Device, bundle_id: str = "com.*.xctrunner", env: dict={}):
         self._d = d
```

### Comparing `solox-2.6.0/solox/public/iosperf/bplist.py` & `solox-2.6.1/solox/public/iosperf/bplist.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # - https://github.com/xa4a/bpylist2/blob/master/bpylist/archiver.py
 
 import copy
 import uuid
 import pprint
 import datetime
 from typing import Any, Union, List
-from .plistlib2 import (InvalidFileException,
+from solox.public.iosperf.plistlib2 import (InvalidFileException,
                         load, dump, loads, dumps,
                         FMT_BINARY, FMT_XML, UID) # yapf: disable
 
 class DecodeNotSupportedError(Exception):
     pass
```

### Comparing `solox-2.6.0/solox/public/iosperf/exceptions.py` & `solox-2.6.1/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/plistlib2.py` & `solox-2.6.1/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.1/solox/public/iosperf/requests_usbmux.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 #
 
 from urllib.parse import splitport, unquote, urlparse
 
 import requests
 import urllib3
 from requests.adapters import HTTPAdapter
-from ._usbmux import Usbmux
-from ._device import Device
+from solox.public.iosperf._usbmux import Usbmux
+from solox.public.iosperf._device import Device
 
 try:
     import http.client as httplib
 except ImportError:
     import httplib
 
 DEFAULT_SCHEME = "http+usbmux://"
```

### Comparing `solox-2.6.0/solox/public/iosperf/struct2.py` & `solox-2.6.1/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/report_template/android.html` & `solox-2.6.1/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/public/report_template/ios.html` & `solox-2.6.1/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/highlight.min.css` & `solox-2.6.1/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/select2.min.css` & `solox-2.6.1/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/sweetalert2.min.css` & `solox-2.6.1/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/tabler.demo.min.css` & `solox-2.6.1/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/css/tabler.min.css` & `solox-2.6.1/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/404.png` & `solox-2.6.1/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/500.png` & `solox-2.6.1/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/avatar.png` & `solox-2.6.1/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/coffee.png` & `solox-2.6.1/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/empty.png` & `solox-2.6.1/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/readme/home.png` & `solox-2.6.1/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/image/readme/pk.png` & `solox-2.6.1/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/apexcharts.js` & `solox-2.6.1/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/gray.js` & `solox-2.6.1/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/highlight.min.js` & `solox-2.6.1/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/highstock.js` & `solox-2.6.1/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/html2canvas.min.js` & `solox-2.6.1/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/jquery.min.js` & `solox-2.6.1/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/select2.min.js` & `solox-2.6.1/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/socket.io.js` & `solox-2.6.1/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/sweetalert2.min.js` & `solox-2.6.1/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/tabler.demo.min.js` & `solox-2.6.1/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/js/tabler.min.js` & `solox-2.6.1/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/static/logo/logo.png` & `solox-2.6.1/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/templates/404.html` & `solox-2.6.1/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/templates/500.html` & `solox-2.6.1/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/templates/analysis.html` & `solox-2.6.1/solox/templates/analysis_compare.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 {% extends 'base.html' %}
-{% block title %}SoloX - {% if lan == 'cn' %} 报告分析 {% else %} Analysis {% endif %}{% endblock %}
+{% block title %}SoloX - {% if lan == 'cn' %} 数据比对 {% else %} Data Comparison {% endif %}{% endblock %}
 
 {% block css %}{% endblock %}
 
 {% block page_title %}
 <a class="active" style="color: #1e71df" href="/report?lan={{ lan }}">{% if lan == 'cn' %} 报告管理 {% else %} Report {% endif %}</a>
 <svg t="1635085520789" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="165732" width="200" height="200"><path d="M360.704 280.746667l45.226667-45.226667 246.570666 246.528a42.666667 42.666667 0 0 1 0 60.330667l-246.528 246.570666-45.22666601-45.269333 231.42400001-231.466667-231.466667-231.424z" p-id="165733"></path></svg>
 {{ app }}
-<svg t="1635085520789" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="165732" width="200" height="200"><path d="M360.704 280.746667l45.226667-45.226667 246.570666 246.528a42.666667 42.666667 0 0 1 0 60.330667l-246.528 246.570666-45.22666601-45.269333 231.42400001-231.466667-231.466667-231.424z" p-id="165733"></path></svg>
-{{ scene }}
 {% endblock %}
 
 {% block ms_auto %}
 <div class="col-auto ms-auto d-print-none">
     <div class="btn-list">
-        <a onclick="saveHtml('{{ platform }}','{{ scene }}')" class="btn">
-            <svg t="1681980190479" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="13623" width="50" height="50"><path d="M192 384h640a42.666667 42.666667 0 0 1 42.666667 42.666667v362.666666a42.666667 42.666667 0 0 1-42.666667 42.666667H192v106.666667a21.333333 21.333333 0 0 0 21.333333 21.333333h725.333334a21.333333 21.333333 0 0 0 21.333333-21.333333V308.821333L949.909333 298.666667h-126.528A98.048 98.048 0 0 1 725.333333 200.618667V72.661333L716.714667 64H213.333333a21.333333 21.333333 0 0 0-21.333333 21.333333v298.666667zM128 832H42.666667a42.666667 42.666667 0 0 1-42.666667-42.666667V426.666667a42.666667 42.666667 0 0 1 42.666667-42.666667h85.333333V85.333333a85.333333 85.333333 0 0 1 85.333333-85.333333h530.026667L1024 282.453333V938.666667a85.333333 85.333333 0 0 1-85.333333 85.333333H213.333333a85.333333 85.333333 0 0 1-85.333333-85.333333v-106.666667zM64 472.490667V746.666667h37.226667v-121.344h93.866666V746.666667h37.248V472.490667H195.093333v114.432h-93.866666v-114.432H64z m195.370667 0v38.4h52.544V746.666667h37.248V510.890667h52.522666v-38.4h-142.293333z m169.386666 0V746.666667h37.226667v-188.928h1.28L534.058667 746.666667h32.128l66.837333-188.928h1.28V746.666667h37.226667V472.490667h-43.605334l-77.013333 215.04h-1.28l-77.312-215.04h-43.605333z m287.36 0V746.666667H832v-38.4h-78.976V472.490667h-36.906667z" fill="#6CB600" p-id="13624"></path></svg>
-            {% if lan == 'cn' %} 保存Html {% else %} Save Html {% endif %}
-        </a>
-        <a download="report.png" onclick="screenshot('sceen-body','report.png')" class="btn">
+        <a download="compare.png" onclick="screenshot('sceen-body','compare.png')" class="btn">
             <svg t="1681980127752" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="11730" width="50" height="50"><path d="M957.31 368.25L903.1 732.12c-6 40.19-33.93 71.32-69.35 82.48a96.61 96.61 0 0 1-44.19 3.26L213.21 727c-39.51-6.23-70-35.53-80.55-72.54l90.55-64.06L363.29 702l193.4-234.78L847.8 681.67V394c0-56.57-44.59-102.43-99.6-102.43H177.34l6.73-45.17c8.33-55.92 59.16-94.3 113.53-85.73l576.35 90.83c54.37 8.56 91.69 60.83 83.36 116.75z" fill="#C5E3FF" p-id="11731"></path><path d="M804.86 831.57a110.71 110.71 0 0 1-17.24-1.36l-576.35-90.83c-42.89-6.76-78.46-38.74-90.62-81.47a12.5 12.5 0 0 1 4.8-13.62L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L835.3 656.93V394c0-49.59-39.07-89.93-87.1-89.93H177.34A12.5 12.5 0 0 1 165 289.71l6.73-45.17a114.5 114.5 0 0 1 45.56-76.09 109.35 109.35 0 0 1 82.29-20.14l576.35 90.83c61 9.62 103.11 68.37 93.78 131L915.46 734A115.87 115.87 0 0 1 889 792.38a112.1 112.1 0 0 1-51.45 34.14 108.3 108.3 0 0 1-32.69 5.05zM147.47 659.32c11.42 29.21 37.19 50.55 67.69 55.36l576.35 90.83a83.72 83.72 0 0 0 38.49-2.84c31.84-10 55.68-38.44 60.74-72.4l54.21-363.87c7.31-49.07-25.41-95.08-72.95-102.58L295.65 173a84.54 84.54 0 0 0-63.6 15.6 89.67 89.67 0 0 0-35.62 59.63l-4.59 30.82h556.37c61.81 0 112.1 51.56 112.1 114.93v287.69a12.5 12.5 0 0 1-19.91 10.06L558.81 484.3 372.93 709.93a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11732"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V394c0-63.37 50.29-114.93 112.1-114.93h583.11c61.81 0 112.1 51.56 112.1 114.93v368.11C860.3 825.48 810 877 748.21 877zM165.13 304c-48 0-87.1 40.34-87.1 89.93v368.18C78 811.7 117.1 852 165.12 852h583.09c48 0 87.1-40.34 87.1-89.93V394c0-49.59-39.07-89.93-87.1-89.93z" fill="#3D9FF9" p-id="11733"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V702a12.5 12.5 0 0 1 5.28-10.2L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L855.22 671.6a12.5 12.5 0 0 1 5.09 10.06v80.44a117 117 0 0 1-15.75 58.77 114.17 114.17 0 0 1-40.07 40.64A109.94 109.94 0 0 1 748.21 877zM78 708.46v53.65C78 811.7 117.1 852 165.12 852h583.09c30.88 0 58.82-16.35 74.74-43.73a92 92 0 0 0 12.36-46.21V688l-276.5-203.7-185.88 225.63a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11734"></path><path d="M847.8 681.67v80.44a104.16 104.16 0 0 1-14.05 52.49c-17.39 29.91-49.19 49.94-85.54 49.94H165.12c-55 0-99.6-45.86-99.6-102.43V702l67.14-47.5 90.55-64.06L363.29 702l193.4-234.78z" fill="#C5E3FF" p-id="11735"></path><path d="M748.21 877H165.12C103.31 877 53 825.48 53 762.11V702a12.5 12.5 0 0 1 5.28-10.2L216 580.22a12.5 12.5 0 0 1 15 0.43l130.45 103.9L547 459.27a12.5 12.5 0 0 1 17.06-2.12L855.22 671.6a12.5 12.5 0 0 1 5.09 10.06v80.44a117 117 0 0 1-15.75 58.77 114.17 114.17 0 0 1-40.07 40.64A109.94 109.94 0 0 1 748.21 877zM78 708.46v53.65C78 811.7 117.1 852 165.12 852h583.09c30.88 0 58.82-16.35 74.74-43.73a92 92 0 0 0 12.36-46.21V688l-276.5-203.7-185.88 225.63a12.5 12.5 0 0 1-17.44 1.83L222.77 606z" fill="#3D9FF9" p-id="11736"></path><path d="M226.91 418.1m-69.43 0a69.43 69.43 0 1 0 138.86 0 69.43 69.43 0 1 0-138.86 0Z" fill="#C5E3FF" p-id="11737"></path><path d="M226.91 500a81.93 81.93 0 1 1 81.93-81.93A82 82 0 0 1 226.91 500z m0-138.86a56.93 56.93 0 1 0 56.93 56.93 57 57 0 0 0-56.93-56.9z" fill="#3D9FF9" p-id="11738"></path></svg>
             {% if lan == 'cn' %} 保存图片 {% else %} Save Image {% endif %}
         </a>
     </div>
 </div>
 {% endblock %}
 
@@ -45,366 +39,164 @@
     </a>
   </li>
 </ul>
 {% endblock %}
 
 {% block page_body %}
 <div class="col-12 mb-3">
-    <div class="row row-cards">
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-dark text-white avatar">
-                                CPU
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                APP
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.cpuAppRate }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-dark text-white avatar">
-                                CPU
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                System
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.cpuSystemRate }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Total
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.totalPassAvg }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% if platform == 'Android' %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Native
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.nativePassAvg }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-yellow text-white avatar">
-                                MEM
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Dalvik
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.dalvikPassAvg }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% endif %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                FPS
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                FPS
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.fps }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% if platform == 'Android' %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-pink text-white avatar">
-                                Jank
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Jank
-                            </div>
-                            <div class="text-muted">
-                                All：{{ apm_data.jank }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% if platform == 'Android' %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Level
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryLevel }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Temperature
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryTeml }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% else %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Temperature
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryTeml }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Current
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryCurrent }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Voltage
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryVoltage }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-green text-white avatar">
-                                A.C
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Power
-                            </div>
-                            <div class="text-muted">
-                                Avg：{{ apm_data.batteryPower }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% endif %}
-        {% endif %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Send
-                            </div>
-                            <div class="text-muted">
-                                All：{{ apm_data.flow_send }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-blue text-white avatar">
-                                NET
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                Recv
-                            </div>
-                            <div class="text-muted">
-                                All：{{ apm_data.flow_recv }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
+    <div class="card">
+        <div class="table-responsive">
+            <table class="table table-vcenter table-bordered table-nowrap card-table">
+                <tbody>
+                    <tr class="bg-light"><th colspan="6" class="subheader">CPU</th></tr>
+                    <tr>
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">APP</td>
+                        <td class="text-center subheader" style="width: 20%;">System</td> 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        <td class="text-center">{{ apm_data1.cpuAppRate }}</td>
+                        <td class="text-center">{{ apm_data1.cpuSystemRate }}</td> 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        <td class="text-center">{{ apm_data2.cpuAppRate }}</td>
+                        <td class="text-center">{{ apm_data2.cpuSystemRate }}</td> 
+                    </tr>
+                    <tr>
+                    <tr class="bg-light"><th colspan="6" class="subheader">Memory</th></tr>
+                    <tr>
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">Total</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center subheader" style="width: 20%;">Native</td>
+                        <td class="text-center subheader" style="width: 20%;">Dalivik</td> 
+                        {% endif %}
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        <td class="text-center">{{ apm_data1.totalPassAvg }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data1.nativePassAvg }}</td>
+                        <td class="text-center">{{ apm_data1.dalvikPassAvg }}</td>
+                        {% endif %} 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        <td class="text-center">{{ apm_data2.totalPassAvg }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data2.nativePassAvg }}</td>
+                        <td class="text-center">{{ apm_data2.dalvikPassAvg }}</td>
+                        {% endif %}   
+                    </tr>
+                    <tr>
+                    <tr class="bg-light"><th colspan="6" class="subheader">Network</th></tr>
+                    <tr>
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">Recv</td>
+                        <td class="text-center subheader" style="width: 20%;">Send</td> 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        <td class="text-center">{{ apm_data1.flow_recv }}</td>
+                        <td class="text-center">{{ apm_data1.flow_send }}</td> 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        <td class="text-center">{{ apm_data2.flow_recv }}</td>
+                        <td class="text-center">{{ apm_data2.flow_send }}</td> 
+                    </tr>
+                    <tr>
+                    <tr class="bg-light"><th colspan="6" class="subheader">FPS</th></tr>
+                    <tr>
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">fps</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center subheader" style="width: 20%;">jank</td>
+                        {% endif %}  
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        <td class="text-center">{{ apm_data1.fps }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data1.jank }}</td>
+                        {% endif %} 
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        <td class="text-center">{{ apm_data2.fps }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data2.jank }}</td>
+                        {% endif %} 
+                    </tr>
+                    <tr class="bg-light"><th colspan="6" class="subheader">Battery</th></tr>
+                    <tr>
+                        
+                        {% if platform == 'Android' %}
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">Level</td>
+                        <td class="text-center subheader" style="width: 20%;">Temperature</td>
+                        {% else %}
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">Temperature</td>
+                        <td class="text-center subheader" style="width: 20%;">Current</td>
+                        <td class="text-center subheader" style="width: 20%;">Voltage</td>
+                        <td class="text-center subheader" style="width: 20%;">Power</td>  
+                        {% endif %}
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data1.batteryLevel }}</td>
+                        <td class="text-center">{{ apm_data1.batteryTeml }}</td>
+                        {% else %}
+                        <td class="text-center">{{ apm_data1.batteryTeml }}</td>
+                        <td class="text-center">{{ apm_data1.batteryCurrent }}</td> 
+                        <td class="text-center">{{ apm_data1.batteryVoltage }}</td>
+                        <td class="text-center">{{ apm_data1.batteryPower }}</td>
+                        {% endif %}
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        {% if platform == 'Android' %}
+                        <td class="text-center">{{ apm_data2.batteryLevel }}</td>
+                        <td class="text-center">{{ apm_data2.batteryTeml }}</td>
+                        {% else %}
+                        <td class="text-center">{{ apm_data2.batteryTeml }}</td>
+                        <td class="text-center">{{ apm_data2.batteryCurrent }}</td> 
+                        <td class="text-center">{{ apm_data2.batteryVoltage }}</td>
+                        <td class="text-center">{{ apm_data2.batteryPower }}</td>
+                        {% endif %} 
+                    </tr>
+                    {% if platform == 'iOS' %}
+                    <tr class="bg-light"><th colspan="6" class="subheader">GPU</th></tr>
+                    <tr>
+                        <td class="text-center subheader" style="width: 20%;">Scene</td>
+                        <td class="text-center subheader" style="width: 20%;">gpu</td>
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene1 }}</td>
+                        <td class="text-center">{{ apm_data1.gpu }}</td>
+                    </tr>
+                    <tr>
+                        <td class="text-center">{{ scene2 }}</td>
+                        <td class="text-center">{{ apm_data2.gpu }}</td>
+                    </tr>
+                    {% endif %}
+                </tbody>
+                <tfoot></tfoot>
+          </table>
         </div>
-        {% if platform == 'iOS' %}
-        <div class="col-sm-6 col-lg-2">
-            <div class="card card-sm">
-                <div class="card-body">
-                    <div class="row align-items-center">
-                        <div class="col-auto">
-                            <span class="bg-purple text-white avatar">
-                                GPU
-                            </span>
-                        </div>
-                        <div class="col">
-                            <div class="font-weight-medium">
-                                GPU
-                            </div>
-                            <div class="text-muted">
-                                Avg: {{ apm_data.gpu }}
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% endif %}
-    </div>
+      </div>
 </div>
 <div class="col-12">
     <div class="card cpu-card">
         <div class="card-header">
-            <div class='card-title'>CPU（%）</div>
+            <div class='card-title'>CPU（%）: APP Usage</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="cpu_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
                 <a class="btn-action cursor-pointer" id="cpu_png" onclick="screenshot('cpu-card','cpu.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
@@ -412,15 +204,15 @@
         </div>
         <div class="card-body">
             <div id="chart-cpu"></div>
         </div>
     </div>
     <div class="card mem-card mt-3">
         <div class="card-header">
-            <div class='card-title'>MEM（MB）</div>
+            <div class='card-title'>MEM（MB）: Total Usage</div>
             <div class="card-actions btn-actions">
                 <a class="btn-action cursor-pointer" id="mem_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
                 <a class="btn-action cursor-pointer" id="mem_png" onclick="screenshot('mem-card','mem.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
@@ -442,62 +234,60 @@
                 </a>
             </div>
         </div>
         <div class="card-body">
             <div id="chart-fps"></div>
         </div>
     </div>
-    {% if platform == 'Android' %}
-    <div class="card jank-card mt-3">
+    <div class="card battery-card mt-3">
         <div class="card-header">
-            <div class='card-title'>JANK</div>
+            <div class='card-title'>Battery: Level</div>
             <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="jank_loading">
+                <a class="btn-action cursor-pointer" id="battery_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
-                <a class="btn-action cursor-pointer" id="jank_png" onclick="screenshot('jank-card','jank.png')">
+                <a class="btn-action cursor-pointer" id="battery_png" onclick="screenshot('battery-card','battery.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
             </div>
         </div>
         <div class="card-body">
-            <div id="chart-jank"></div>
+            <div id="chart-battery"></div>
         </div>
     </div>
-    <div class="card battery-card mt-3">
+    <div class="card networkdata-card-recv mt-3">
         <div class="card-header">
-            <div class='card-title'>A.C（%）</div>
+            <div class='card-title'>Network Data（KB）: Recv</div>
             <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="battery_loading">
+                <a class="btn-action cursor-pointer" id="networkdata_recv_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
-                <a class="btn-action cursor-pointer" id="battery_png" onclick="screenshot('battery-card','battery.png')">
+                <a class="btn-action cursor-pointer" id="networkdata_recv_png" onclick="screenshot('networkdata-card-recv','networkdata_recv.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
             </div>
         </div>
         <div class="card-body">
-            <div id="chart-battery"></div>
+            <div id="chart-networkdata-recv"></div>
         </div>
     </div>
-    {% endif %}
-    <div class="card networkdata-card mt-3">
+    <div class="card networkdata-card-send mt-3">
         <div class="card-header">
-            <div class='card-title'>Network Data（KB）</div>
+            <div class='card-title'>Network Data（KB）: Send</div>
             <div class="card-actions btn-actions">
-                <a class="btn-action cursor-pointer" id="networkdata_loading">
+                <a class="btn-action cursor-pointer" id="networkdata_send_loading">
                     <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4" /><path d="M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4" /></svg>
                 </a>
-                <a class="btn-action cursor-pointer" id="networkdata_png" onclick="screenshot('networkdata-card','networkdata.png')">
+                <a class="btn-action cursor-pointer" id="networkdata_send_png" onclick="screenshot('networkdata-card-send','networkdata_send.png')">
                     <svg t="1646303797379" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5790" width="2000" height="2000"><path d="M897.856 842.56c14.464-6.72 18.624-20.48 9.28-30.848l-241.216-263.296a25.792 25.792 0 0 0-7.68-5.888c-14.016-7.296-33.6-5.184-43.776 4.8l-241.152 233.088-103.808-70.528a30.912 30.912 0 0 0-3.52-1.92c-14.08-7.36-33.664-4.992-43.776 4.864l-101.056 97.728a18.368 18.368 0 0 0-6.08 13.952c0.512 12.288 14.848 22.016 32.128 21.696h732.8a40.768 40.768 0 0 0 17.856-3.648zM259.84 399.68a78.464 78.464 0 0 0 117.504 67.84 78.272 78.272 0 0 0 0-135.744A78.208 78.208 0 0 0 259.84 399.68" p-id="5791"></path><path d="M864.832 872.256H159.232a83.84 83.84 0 0 1-83.776-83.776V235.52a83.84 83.84 0 0 1 83.776-83.776h705.536a83.84 83.84 0 0 1 83.776 83.776v552.96a83.84 83.84 0 0 1-83.712 83.776zM159.232 183.744a51.84 51.84 0 0 0-51.776 51.776v552.96a51.84 51.84 0 0 0 51.776 51.776h705.536a51.84 51.84 0 0 0 51.776-51.776V235.52a51.84 51.84 0 0 0-51.776-51.776H159.232z" p-id="5792"></path></svg>
                 </a>
             </div>
         </div>
         <div class="card-body">
-            <div id="chart-networkdata"></div>
+            <div id="chart-networkdata-send"></div>
         </div>
     </div>
     {% if platform == 'iOS' %}
     <div class="card gpu-card mt-3">
         <div class="card-header">
             <div class='card-title'>GPU（%）</div>
             <div class="card-actions btn-actions">
@@ -510,109 +300,40 @@
             </div>
         </div>
         <div class="card-body">
             <div id="chart-gpu"></div>
         </div>
     </div>
     {% endif %}
-
 </div>
 {% endblock %}
 
 {% block js %}
 <script>
 
     $(document).ready(function() {
         $('#cpu_loading').click();
         $('#mem_loading').click();
         $('#fps_loading').click();
-        if(platform == 'Android'){
-            $('#jank_loading').click();
-        }
+        $('#battery_loading').click();
+        $('#networkdata_send_loading').click();
+        $('#networkdata_recv_loading').click();
         if(platform == 'iOS'){
             $('#gpu_loading').click();
         }
-        $('#battery_loading').click();
-        $('#networkdata_loading').click();
     });
 
     function saveHtml(platform, scene){
         if(platform=='Android'){
             saveAndroidHtml(scene)
         }else{
             saveiOSHtml(scene)
         }
     }
 
-    function saveAndroidHtml(scene){
-        $.ajax({
-            url: "/apm/export/html/android",
-            type: "GET",
-            async: true,
-            cache: false,
-            data:{
-                scene: scene,
-                cpu_app:'{{ apm_data.cpuAppRate }}',
-                cpu_sys:'{{ apm_data.cpuSystemRate }}',
-                mem_total:'{{ apm_data.totalPassAvg }}',
-                mem_native:'{{ apm_data.nativePassAvg }}',
-                mem_dalvik:'{{ apm_data.dalvikPassAvg }}',
-                fps:'{{ apm_data.fps }}',
-                jank:'{{ apm_data.jank }}',
-                level:'{{ apm_data.batteryLevel }}',
-                temperature:'{{ apm_data.batteryTeml }}',
-                net_send:'{{ apm_data.flow_send }}',
-                net_recv:'{{ apm_data.flow_recv }}'
-            },
-            beforeSend: function () {
-                SwalLoading('Save Html','Saving html.')
-            },
-            success: function (data) {
-                if(data['status']  == 1 ){
-                    SwalFire('success', 'Save successuly !', data['path'], 5000);
-                }else{
-                    SwalFire('error', 'Save failed !', data['msg'], 2000);
-                }
-            }
-        });
-    }
-
-    function saveiOSHtml(scene){
-        $.ajax({
-            url: "/apm/export/html/ios",
-            type: "GET",
-            async: true,
-            cache: false,
-            data:{
-                scene: scene,
-                cpu_app:'{{ apm_data.cpuAppRate }}',
-                cpu_sys:'{{ apm_data.cpuSystemRate }}',
-                gpu:'{{ apm_data.gpu }}',
-                mem_total:'{{ apm_data.totalPassAvg }}',
-                fps:'{{ apm_data.fps }}',
-                temperature:'{{ apm_data.batteryTeml }}',
-                current:'{{ apm_data.batteryCurrent }}',
-                voltage:'{{ apm_data.batteryVoltage }}',
-                power:'{{ apm_data.batteryPower }}',
-                net_send:'{{ apm_data.flow_send }}',
-                net_recv:'{{ apm_data.flow_recv }}'
-            },
-            beforeSend: function () {
-                SwalLoading('Save Html','Saving html.')
-            },
-            success: function (data) {
-                if(data['status']  == 1 ){
-                    SwalFire('success', 'Save successuly !', data['path'], 5000);
-                }else{
-                    SwalFire('error', 'Save failed !', data['msg'], 2000);
-                }
-            }
-        });
-    }
-
     function options(type,dataLabels=false) {
         let options = {
             chart: {
                 type: type,
                 fontFamily: 'inherit',
                 height: 240,
                 parentHeightOffset: 0,
@@ -642,246 +363,234 @@
                 },
             strokeDashArray: 4,
             },
         };
         return options
     }
 
-    var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
+    var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('bar'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
             data:{
-                scene:'{{ scene }}',
+                scene1:'{{ scene1 }}',
+                scene2:'{{ scene2 }}',
                 target:'cpu',
                 platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
                 cpu_chart.updateSeries([{
-                    name: 'app',
-                    data: data['cpuAppData']
+                    name: '{{ scene1 }}',
+                    data: data['scene1']
                 },{
-                    name: 'sys',
-                    data: data['cpuSysData']
+                    name: '{{ scene2 }}',
+                    data: data['scene2']
                 }])
             }
         });
     });
     
-    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('line'));
+    var battery_chart = new ApexCharts(document.querySelector("#chart-battery"), options('bar'));
         battery_chart.render();
         $('#battery_loading').click(function () {
             $.ajax({
-                url: '/apm/log',
+                url: '/apm/log/compare',
                 type: "GET",
                 async: true,
                 cache: false,
                 data:{
-                    scene:'{{ scene }}',
+                    scene1:'{{ scene1 }}',
+                    scene2:'{{ scene2 }}',
                     target:'battery',
                     platform:platform
                 },
                 beforeSend: function () {
                     SwalLoading('Loading','')
                 },
                 complete: function () {
                     swal.close();
                 },
                 success: function (data) {
-                    if(platform == 'Android'){
-                        battery_chart.updateSeries([{
-                            name: 'level',
-                            data: data['batteryLevel']
-                        },{
-                            name: 'temperature',
-                            data: data['batteryTem']
-                        }])
-                    }else {
-                        battery_chart.updateSeries([{
-                            name: 'temperature',
-                            data: data['batteryTem']
-                        },{
-                            name: 'Current',
-                            data: data['batteryCurrent']
-                        },{
-                            name: 'Voltage',
-                            data: data['batteryVoltage']
-                        },{
-                            name: 'Power',
-                            data: data['batteryPower']
-                        }])
-                    }
-                }
-            });
-        });
-
-    if(platform == 'Android'){
-        var jank_chart = new ApexCharts(document.querySelector("#chart-jank"), options('line'));
-        jank_chart.render();
-        $('#jank_loading').click(function () {
-            $.ajax({
-                url: '/apm/log',
-                type: "GET",
-                async: true,
-                cache: false,
-                data:{
-                    scene:'{{ scene }}',
-                    target:'fps',
-                    platform:platform
-                },
-                beforeSend: function () {
-                    SwalLoading('Loading','')
-                },
-                complete: function () {
-                    swal.close();
-                },
-                success: function (data) {
-                    jank_chart.updateSeries([{
-                        name: 'jank',
-                        data: data['jank']
+                    battery_chart.updateSeries([{
+                        name: '{{ scene1 }}',
+                        data: data['scene1']
+                    },{
+                        name: '{{ scene2 }}',
+                        data: data['scene2']
                     }])
                 }
             });
         });
-    }
-
     if(platform == 'iOS'){
-        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('line'));
+        var gpu_chart = new ApexCharts(document.querySelector("#chart-gpu"), options('bar'));
         gpu_chart.render();
         $('#gpu_loading').click(function () {
             $.ajax({
-                url: '/apm/log',
+                url: '/apm/log/compare',
                 type: "GET",
                 async: true,
                 cache: false,
                 data:{
-                    scene:'{{ scene }}',
+                    scene1:'{{ scene1 }}',
+                    scene2:'{{ scene2 }}',
                     target:'gpu',
                     platform:platform
                 },
                 beforeSend: function () {
                     SwalLoading('Loading','')
                 },
                 complete: function () {
                     swal.close();
                 },
                 success: function (data) {
                     gpu_chart.updateSeries([{
-                        name: 'gpu',
-                        data: data['gpu']
+                        name: '{{ scene1 }}',
+                        data: data['scene1']
+                    },{
+                        name: '{{ scene2 }}',
+                        data: data['scene2']
                     }])
                 }
             });
         });
     }
 
-    var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('line'));
+    var fps_chart = new ApexCharts(document.querySelector("#chart-fps"), options('bar'));
     fps_chart.render();
     $('#fps_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
             data:{
-                scene:'{{ scene }}',
+                scene1:'{{ scene1 }}',
+                scene2:'{{ scene2 }}',
                 target:'fps',
                 platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
                 fps_chart.updateSeries([{
-                    name: 'fps',
-                    data: data['fps']
+                    name: '{{ scene1 }}',
+                    data: data['scene1']
+                },{
+                    name: '{{ scene2 }}',
+                    data: data['scene2']
                 }])
             }
         });
     });
 
-    var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('line'));
+    var mem_chart = new ApexCharts(document.querySelector("#chart-mem"), options('bar'));
     mem_chart.render();
     $('#mem_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
             data:{
-                scene:'{{ scene }}',
-                target:'mem',
+                scene1:'{{ scene1 }}',
+                scene2:'{{ scene2 }}',
+                target:'memory',
                 platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                if(platform == 'Android'){
-                    mem_chart.updateSeries([{
-                        name: 'total',
-                        data: data['memTotalData']
-                    },{
-                        name: 'native',
-                        data: data['memNativeData']
-                    },{
-                        name: 'dalvik',
-                        data: data['memDalvikData']
-                    }])
-                }else{
-                    mem_chart.updateSeries([{
-                        name: 'total',
-                        data: data['memTotalData']
-                    }])
-                }
+                mem_chart.updateSeries([{
+                    name: '{{ scene1 }}',
+                    data: data['scene1']
+                },{
+                    name: '{{ scene2 }}',
+                    data: data['scene2']
+                }])
+            }
+        });
+    });
+
+    var network_recv_chart = new ApexCharts(document.querySelector("#chart-networkdata-recv"), options('bar',false));
+    network_recv_chart.render();
+    $('#networkdata_recv_loading').click(function () {
+        $.ajax({
+            url: '/apm/log/compare',
+            type: "GET",
+            async: true,
+            cache: false,
+            data:{
+                scene1:'{{ scene1 }}',
+                scene2:'{{ scene2 }}',
+                target:'net_recv',
+                platform:platform
+            },
+            beforeSend: function () {
+                SwalLoading('Loading','')
+            },
+            complete: function () {
+                swal.close();
+            },
+            success: function (data) {
+                network_recv_chart.updateSeries([{
+                    name: '{{ scene1 }}',
+                    data: data['scene1']
+                },{
+                    name: '{{ scene2 }}',
+                    data: data['scene2']
+                }])
             }
         });
     });
 
-    var network_chart = new ApexCharts(document.querySelector("#chart-networkdata"), options('line',false));
-    network_chart.render();
-    $('#networkdata_loading').click(function () {
+    var network_send_chart = new ApexCharts(document.querySelector("#chart-networkdata-send"), options('bar',false));
+    network_send_chart.render();
+    $('#networkdata_send_loading').click(function () {
         $.ajax({
-            url: '/apm/log',
+            url: '/apm/log/compare',
             type: "GET",
             async: true,
             cache: false,
             data:{
-                scene:'{{ scene }}',
-                target:'flow',
+                scene1:'{{ scene1 }}',
+                scene2:'{{ scene2 }}',
+                target:'net_send',
                 platform:platform
             },
             beforeSend: function () {
                 SwalLoading('Loading','')
             },
             complete: function () {
                 swal.close();
             },
             success: function (data) {
-                network_chart.updateSeries([{
-                    name: 'send',
-                    data: data['upFlow']
+                console.log(data)
+                network_send_chart.updateSeries([{
+                    name: '{{ scene1 }}',
+                    data: data['scene1']
                 },{
-                    name: 'recv',
-                    data: data['downFlow']
+                    name: '{{ scene2 }}',
+                    data: data['scene2']
                 }])
             }
         });
     });
 </script>
 {% endblock %}
```

### Comparing `solox-2.6.0/solox/templates/analysis_pk.html` & `solox-2.6.1/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/templates/base.html` & `solox-2.6.1/solox/templates/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 <div class="d-flex flex-column flex-md-row flex-fill align-items-stretch align-items-md-center">
                     {% block navbar_nav %}{% endblock %}
                 </div>
             </div>
             {% if model in ['2-app','2-devices'] %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
                 <a  href="/?platform=Android&lan={{ lan }}" class="btn  btn-pill w-100" >
-                    <svg t="1661854459800" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="24106" width="2000" height="2000"><path d="M555.52 943.616C339.456 943.616 163.84 768 163.84 552.448s175.616-391.68 391.68-391.68S947.2 336.384 947.2 552.448s-176.128 391.168-391.68 391.168z" fill="#38CEB1" p-id="24107"></path><path d="M815.616 820.224m-20.48 0a20.48 20.48 0 1 0 40.96 0 20.48 20.48 0 1 0-40.96 0Z" fill="#231815" p-id="24108"></path><path d="M512 61.952c-248.32 0-450.56 202.24-450.56 450.56s202.24 450.56 450.56 450.56c93.184 0 182.272-28.16 258.048-81.408 9.216-6.656 11.264-19.456 5.12-28.672-6.656-9.216-19.456-11.264-28.672-5.12-69.12 48.128-150.016 73.728-235.008 73.728-225.792 0-409.6-183.808-409.6-409.6s183.808-409.6 409.6-409.6 409.6 183.808 409.6 409.6c0 87.552-27.136 171.008-78.848 241.152-6.656 9.216-4.608 22.016 4.608 28.672 9.216 6.656 22.016 4.608 28.672-4.608 56.832-77.312 86.528-169.472 86.528-265.728 0.512-247.296-201.728-449.536-450.048-449.536z" fill="#231815" p-id="24109"></path><path d="M641.536 267.776c-8.192-8.192-20.992-8.192-29.184 0L389.632 491.008c-5.632 5.632-9.216 13.312-9.216 21.504s3.072 15.872 9.216 21.504l223.232 223.232c4.096 4.096 9.216 6.144 14.336 6.144s10.24-2.048 14.336-6.144c8.192-8.192 8.192-20.992 0-29.184L425.472 512l216.064-216.064c8.192-7.168 8.192-20.48 0-28.16z" fill="#231815" p-id="24110"></path></svg>
+                    <svg t="1682331413507" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="9942" width="50" height="50"><path d="M512.149985 512.049995m-511.950005 0a511.950005 511.950005 0 1 0 1023.90001 0 511.950005 511.950005 0 1 0-1023.90001 0Z" fill="#1BAF96" p-id="9943"></path><path d="M634.738014 267.273899l-122.288058 265.974026L440.956938 734.92823l-125.087785 37.796309L286.971975 782.923543l-13.998633 23.997656 314.16932 211.579338c247.175862-36.296455 436.957328-249.175666 436.957328-506.450542 0-39.596133-4.499561-78.192364-12.99873-115.288741L740.927644 208.979592l-106.18963 58.294307z" fill="#199E85" p-id="9944"></path><path d="M650.03652 582.14315l-59.3942-56.894444c-13.998633-13.398692 0-27.197344 0-27.197344l63.79377-60.994043c43.295772-41.395957 41.495948-101.79006 41.495948-101.79006V256.974905l-183.382092-15.298506L329.167855 256.974905v78.292354s-1.799824 60.294112 41.495947 101.79006l63.793771 60.994043s13.998633 13.798652 0 27.197344L374.963382 582.14315s-45.795528 43.495752-45.795527 112.888976v77.692413h366.664193v-77.692413c0-69.393223-45.795528-112.888976-45.795528-112.888976z" fill="#FFFFFF" p-id="9945"></path><path d="M497.25144 679.83361l0.499951-168.083586c0.19998-31.496924-14.598574-51.394981-20.298017-57.094424L412.959672 392.961625c-21.897862-20.897959-22.697783-55.494581-22.697784-55.794551h244.476126s-0.399961 34.496631-22.697784 55.794551l-63.79377 60.994043c-6.499365 6.399375-20.797969 26.297432-20.597988 57.794356v168.083586h-30.397032z" fill="#4F5D73" p-id="9946"></path><path d="M757.026072 236.676887c0 16.89835-13.698662 30.597012-30.597012 30.597012H298.570843c-16.89835 0-30.597012-13.698662-30.597012-30.597012s13.698662-30.597012 30.597012-30.597012h427.758226c16.99834 0.09999 30.697002 13.798652 30.697003 30.597012z m0 550.046285c0 16.89835-13.698662 30.597012-30.597012 30.597012H298.570843c-16.89835 0-30.597012-13.698662-30.597012-30.597012 0-16.89835 13.698662-30.597012 30.597012-30.597012h427.758226c16.99834 0.09999 30.697002 13.798652 30.697003 30.597012z" fill="#F2B955" p-id="9947"></path><path d="M650.03652 756.22615H374.963382L512.549946 633.938092l137.486574 122.288058z" fill="#4F5D73" p-id="9948"></path></svg>
                     {% if lan == 'cn' %} 普通模式 {% else %} Normal Model {% endif %}
                 </a>
             </div>
             {% else %}
             <div class="nav-item dropdown d-none d-md-flex me-3">
                 <a href="/pk?model=2-devices&lan={{ lan }}" class="btn  btn-pill w-100" >
                     <svg t="1661854041585" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="10784" width="2000" height="2000"><path d="M17.408 862.208a450.56 129.024 0 1 0 901.12 0 450.56 129.024 0 1 0-901.12 0Z" fill="#EEF2FF" p-id="10785"></path><path d="M509.952 880.64H75.776c-17.408 0-30.72-13.312-30.72-30.72V293.888c0-64.512 52.224-116.736 116.736-116.736h522.24c35.84 0 64.512 28.672 64.512 64.512v400.384C748.544 774.144 642.048 880.64 509.952 880.64z" fill="#70D4FF" p-id="10786"></path><path d="M764.928 880.64H212.992c-17.408 0-30.72-13.312-30.72-30.72V60.416h755.712c35.84 0 64.512 28.672 64.512 64.512v517.12C1002.496 774.144 896 880.64 764.928 880.64z" fill="#4E8EFF" p-id="10787"></path><path d="M555.008 403.456c0 20.48-7.168 35.84-22.528 48.128-14.336 11.264-30.72 16.384-51.2 16.384h-28.672v48.128c0 9.216 2.048 15.36 6.144 19.456 4.096 4.096 11.264 5.12 21.504 5.12V563.2H373.76v-22.528c15.36 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-23.552-24.576v-22.528h109.568c19.456 0 35.84 5.12 49.152 15.36 14.336 12.288 22.528 27.648 22.528 46.08z m-59.392 2.048c0-26.624-11.264-39.936-34.816-39.936h-9.216v80.896h11.264c13.312 0 22.528-3.072 26.624-10.24 4.096-7.168 6.144-17.408 6.144-30.72zM800.768 563.2h-60.416c-8.192-7.168-15.36-15.36-21.504-22.528l-57.344-74.752v50.176c0 16.384 9.216 24.576 26.624 24.576V563.2H584.704v-22.528c16.384 0 23.552-8.192 23.552-24.576V389.12c0-16.384-8.192-24.576-24.576-24.576v-22.528h105.472v22.528c-17.408 0-26.624 8.192-26.624 24.576v50.176l39.936-37.888c13.312-12.288 19.456-21.504 19.456-27.648 0-5.12-5.12-8.192-15.36-8.192v-22.528h81.92v22.528c-9.216 0-15.36 1.024-20.48 4.096-3.072 2.048-8.192 6.144-15.36 13.312L705.536 430.08l70.656 94.208c7.168 9.216 15.36 15.36 25.6 16.384V563.2z" fill="#FFFFFF" p-id="10788"></path></svg>
@@ -116,31 +116,25 @@
                             </a>
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX" target="_blank" class="link-secondary" rel="noopener">
                                 {% if lan == 'cn' %} 源码 {% else %} Source code {% endif %}
                             </a>
                         </li>
-                        <li class="list-inline-item">
-                            <a href="https://github.com/sponsors/codecalm" target="_blank" class="link-secondary" rel="noopener" data-bs-toggle="modal" data-bs-target="#modal-coffee">
-                              <svg xmlns="http://www.w3.org/2000/svg" class="icon text-pink icon-filled icon-inline" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M19.5 12.572l-7.5 7.428l-7.5 -7.428a5 5 0 1 1 7.5 -6.566a5 5 0 1 1 7.5 6.572" /></svg>
-                              {% if lan == 'cn' %} 喝杯咖啡 {% else %} Sponsor {% endif %}
-                            </a>
-                        </li>
                     </ul>
                 </div>
                 <div class="col-12 col-lg-auto mt-3 mt-lg-0">
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.5.9
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.1
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
@@ -257,27 +251,14 @@
           </div>
         
         <a class="btn btn-primary mt-3" onclick="saveWorningValue()">
             {% if lan == 'cn' %} 保存 {% else %} Save {% endif %}
         </a>
     </div>
 </div>
-<div class="modal modal-blur fade" id="modal-coffee" tabindex="-1" role="dialog" aria-hidden="true">
-    <div class="modal-dialog modal-sm modal-dialog-centered" role="document">
-        <div class="modal-content">
-            <div class="modal-header">
-                <h5 class="modal-title">{% if lan == 'cn' %} 买杯咖啡 {% else %} Buy me coffee {% endif %}</h5>
-                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-            </div>
-            <div class="modal-body">
-                <img  alt="" src="./static/image/coffee.png">
-            </div>
-        </div>
-    </div>
-</div>
 
 <!-- JQ JS -->
 <script src="./static/js/jquery.min.js"></script>
 <!-- tabler -->
 <script src="./static/js/tabler.min.js"></script>
 <script src="./static/js/tabler.demo.min.js"></script>
 <!-- Sweetalert2 -->
@@ -296,15 +277,15 @@
 <script src="./static/js/html2canvas.min.js"></script>
 <script src="./static/js/socket.io.js"></script>
 <script>
 
     var platform = '{{ platform }}'; // 平台
     var lan = '{{ lan }}' ;
     
-    var domain = $('.host_switch').is(':checked') == true ? $('#host').val() : window.location.host ;
+    var domain = $('.host_switch').is(':checked') == true ? $('#host').val().trim() : window.location.host ;
     var Host = 'http://' + domain
 
     $(document).ready(function() {
         $('.select2-selection--single').select2({
             theme: "bootstrap-5",
             containerCssClass: "select2--small",
             selectionCssClass: "select2--small",
```

#### html2text {}

```diff
@@ -22,18 +22,17 @@
 ä¸­æ English
 
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
-    * _{%_if_lan_==_'cn'_%}_åæ¯åå¡_{%_else_%}_Sponsor_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.5.9
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.1
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
@@ -48,15 +47,14 @@
 value {% endif %} [{{ netdataRecvWarning }}]
 {% if lan == 'cn' %} æç»­æ§è¡æ¶é´ï¼åéï¼ {% else %}
 Durationï¼minutesï¼ {% endif %} [{{ runningTime }}   ]
 PC HOST              SWITCH
    [{{ solox_host }}  {% if host_switch == '1' %} * {% else %} ⁰ {% endif
    ]                 %}
 {% if lan == 'cn' %} ä¿å­ {% else %} Save {% endif %}
-** {% if lan == 'cn' %} ä¹°æ¯åå¡ {% else %} Buy me coffee {% endif %} **
```

### Comparing `solox-2.6.0/solox/templates/index.html` & `solox-2.6.1/solox/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -178,21 +178,28 @@
                     </div>
                 </div>
             </div>
             {% if platform == 'Android' %}
             <a class="dropdown-item" style="margin-top: 10px;">
                 <svg t="1657093102367" class="icon me-2" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="27860" width="2000" height="2000"><path d="M938.362 256.2V149.626c0-23.576-19.11-42.654-42.652-42.654H43.046C19.502 106.972 0.392 126.05 0.392 149.626V256.2h937.97z" fill="#E6E9ED" p-id="27861"></path><path d="M792.164 831.75H0.392V192.25h937.97v446.306z" fill="#656D78" p-id="27862"></path><path d="M85.67 149.626c0 11.772-9.526 21.296-21.328 21.296-11.74 0-21.294-9.524-21.294-21.296S52.602 128.3 64.342 128.3c11.802 0 21.328 9.556 21.328 21.326z" fill="#ED5564" p-id="27863"></path><path d="M149.62 149.626c0 11.772-9.524 21.296-21.326 21.296-11.742 0-21.296-9.524-21.296-21.296S116.55 128.3 128.292 128.3c11.804 0 21.328 9.556 21.328 21.326z" fill="#FFCE54" p-id="27864"></path><path d="M213.568 149.626c0 11.772-9.524 21.296-21.326 21.296-11.74 0-21.294-9.524-21.294-21.296S180.502 128.3 192.242 128.3c11.802 0 21.326 9.556 21.326 21.326z" fill="#A0D468" p-id="27865"></path><path d="M746.512 277.496H106.996c-11.772 0-21.326 9.554-21.326 21.326s9.554 21.328 21.326 21.328h639.516c11.74 0 21.294-9.556 21.294-21.328s-9.554-21.326-21.294-21.326z" fill="#FC6E51" p-id="27866"></path><path d="M106.996 405.426h341.046c11.802 0 21.326-9.554 21.326-21.328 0-11.772-9.524-21.326-21.326-21.326H106.996c-11.772 0-21.326 9.554-21.326 21.326 0 11.774 9.554 21.328 21.326 21.328z" fill="#AC92EB" p-id="27867"></path><path d="M575.958 448.05H106.996c-11.772 0-21.326 9.556-21.326 21.328s9.554 21.296 21.326 21.296h468.962c11.8 0 21.294-9.524 21.294-21.296s-9.492-21.328-21.294-21.328z" fill="#48CFAD" p-id="27868"></path><path d="M106.996 575.952H405.42c11.772 0 21.326-9.556 21.326-21.328s-9.554-21.296-21.326-21.296H106.996c-11.772 0-21.326 9.526-21.326 21.296s9.554 21.328 21.326 21.328z" fill="#5D9CEC" p-id="27869"></path><path d="M615.678 669.22c8.618 0 16.734-5.278 19.984-13.832 4.122-11.024-1.5-23.326-12.492-27.45-41.03-15.392-47.336-54.708-47.336-55.112a21.332 21.332 0 0 0-24.232-17.956c-11.662 1.716-19.688 12.552-17.97 24.2 0.376 2.624 10.242 64.668 74.55 88.776 2.5 0.938 4.996 1.374 7.496 1.374zM959.534 917.028c1 0 2.06-0.094 3.122-0.25 11.68-1.716 19.674-12.552 17.988-24.2-0.376-2.624-10.242-64.668-74.566-88.776-11.054-4.152-23.296 1.438-27.48 12.458-4.122 11.024 1.5 23.326 12.492 27.448 41.03 15.394 47.336 54.708 47.398 55.114a21.28 21.28 0 0 0 21.046 18.206zM448.042 618.572H106.996c-11.772 0-21.326 9.554-21.326 21.328 0 11.772 9.554 21.326 21.326 21.326h341.046c11.802 0 21.326-9.554 21.326-21.326a21.312 21.312 0 0 0-21.326-21.328z" fill="#FFCE54" p-id="27870"></path><path d="M277.52 703.85H106.996c-11.772 0-21.326 9.554-21.326 21.328 0 11.772 9.554 21.294 21.326 21.294h170.524c11.772 0 21.326-9.524 21.326-21.294 0-11.774-9.554-21.328-21.326-21.328z" fill="#ED5564" p-id="27871"></path><path d="M1002.312 746.472H533.318a21.28 21.28 0 0 1-21.294-21.294c0-11.774 9.524-21.328 21.294-21.328h468.994c11.74 0 21.294 9.554 21.294 21.328 0.002 11.772-9.554 21.294-21.294 21.294zM725.592 555.53a21.332 21.332 0 0 1-18.298-10.368l-64.388-107.478c-5.994-10.086-2.746-23.202 7.372-29.228a21.276 21.276 0 0 1 29.226 7.338l64.324 107.478c6.058 10.086 2.81 23.17-7.306 29.228a21.286 21.286 0 0 1-10.93 3.03zM810.212 555.53c-3.686 0-7.496-0.968-10.93-3.03-10.054-6.058-13.364-19.142-7.306-29.26l64.324-107.446a21.278 21.278 0 0 1 29.228-7.338c10.118 6.026 13.364 19.11 7.368 29.228l-64.324 107.478c-3.996 6.65-11.116 10.368-18.36 10.368zM920.002 669.22c-8.62 0-16.738-5.278-19.922-13.832-4.184-11.024 1.436-23.326 12.426-27.45 41.094-15.392 47.34-54.708 47.402-55.112 1.686-11.648 12.55-19.674 24.168-17.956 11.68 1.716 19.734 12.552 17.986 24.2-0.376 2.624-10.242 64.668-74.568 88.776a20.884 20.884 0 0 1-7.492 1.374zM575.958 917.028c-1 0-2.062-0.094-3.124-0.25-11.616-1.716-19.672-12.552-17.984-24.2 0.438-2.624 10.242-64.668 74.566-88.776 11.054-4.152 23.356 1.438 27.478 12.458 4.124 11.024-1.436 23.326-12.49 27.448-41.032 15.394-47.276 54.708-47.338 55.114-1.56 10.586-10.68 18.206-21.108 18.206z" fill="#FFCE54" p-id="27872"></path><path d="M938.236 682.524c0 129.524-48.71 234.504-170.43 234.504-121.716 0-170.43-104.98-170.43-234.504 0-129.494 63.39-191.85 170.43-191.85 107.044-0.002 170.43 62.356 170.43 191.85z" fill="#ED5564" p-id="27873"></path><path d="M746.512 915.872c6.806 0.75 13.928 1.156 21.294 1.156 7.372 0 14.49-0.406 21.296-1.156v-297.3h-42.592v297.3z" fill="#DA4453" p-id="27874"></path><path d="M603.56 618.572h328.494c-18.298-86.12-76.626-127.9-164.248-127.9-87.616 0-145.946 41.782-164.246 127.9z" fill="#DA4453" p-id="27875"></path></svg>
                 {% if lan == 'cn' %} 错误日志 {% else %} Error Log {% endif %}
-                <span class="ms-auto badge bg-red" data-bs-toggle="offcanvas" href="#offcanvasBottom" role="button" aria-controls="offcanvasBottom">
+                <span class="ms-auto badge" data-bs-toggle="offcanvas" href="#offcanvasBottom" role="button" aria-controls="offcanvasBottom">
                     OPEN
                 </span>
             </a>
-            <div class="dropdown-divider"></div>
             {% endif %}
             <a class="dropdown-item" style="margin-top: 10px;">
+                <svg t="1682332095813" class="icon me-2" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="18522" width="50" height="50"><path d="M512 640a64 64 0 1 1 0.032-128.032A64 64 0 0 1 512 640m69.344-474.112a413.12 413.12 0 0 0-138.624 0A414.304 414.304 0 0 0 96 576c0 229.376 186.624 416 416 416s416-186.624 416-416A414.304 414.304 0 0 0 581.344 165.888" fill="#1BB5EC" p-id="18523"></path><path d="M512 928C317.92 928 160 770.08 160 576S317.92 224 512 224s352 157.92 352 352-157.92 352-352 352zM480 96h64v65.632A407.232 407.232 0 0 0 512 160c-10.784 0-21.408 0.8-32 1.632V96z m128 75.616V96a32 32 0 1 0 0-64h-192a32 32 0 0 0 0 64v75.616C232.8 215.136 96 379.712 96 576c0 229.376 186.624 416 416 416s416-186.624 416-416c0-196.288-136.832-360.864-320-404.384z" fill="#364F6B" p-id="18524"></path><path d="M512 608c-17.632 0-32-14.368-32-32 0-17.632 14.368-32 32-32 17.632 0 32 14.368 32 32 0 17.632-14.368 32-32 32m32-122.112V320a32 32 0 0 0-64 0v165.888A95.872 95.872 0 0 0 416 576c0 52.928 43.072 96 96 96s96-43.072 96-96a95.904 95.904 0 0 0-64-90.112" fill="#364F6B" p-id="18525"></path></svg>
+                {% if lan == 'cn' %} 启动时间 {% else %} Start-up Time {% endif %}
+                <span class="ms-auto badge" data-bs-toggle="offcanvas" href="#offcanvas-startup-time" role="button" aria-controls="offcanvas-startup-time">
+                    OPEN
+                </span>
+            </a>
+            <div class="dropdown-divider"></div>
+            <a class="dropdown-item" style="margin-top: 10px;">
                 <input type="file" class="form-control" id="app-file" accept=".apk,.ipa"/>
             </a>
             <strong style="margin-top: 5px;margin-left: 140px;">{% if lan == 'cn' %} 或 {% else %} OR {% endif %}</strong>
             <a class="dropdown-item" >
                 {% if lan == 'cn' %}
                 <input type="text" class="app-link form-control" name="example-text-input"  placeholder="请输入文件链接">
                 {% else %}
@@ -247,14 +254,55 @@
                 {% if lan == 'cn' %} 清除 {% else %} Clear {% endif %}
             </a>
         </div>
         <div class="mt-2" id="logcat-content" style="color: rgba(214, 39, 8, 0.849);"></div>
     </div>
   </div>
 </div>
+<div class="offcanvas offcanvas-bottom layout-boxed" tabindex="-1" id="offcanvas-startup-time" aria-labelledby="offcanvasBottomLabel" style="height: 85%;margin-left: 10%;margin-right: 10%;">
+    <div class="offcanvas-header">
+      <h2 class="offcanvas-title" id="offcanvasBottomLabel">Start-up Time</h2>
+      <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
+    </div>
+    <div class="offcanvas-body">
+        <div class="row">
+            {% if platform == 'Android' %}
+            <div class="col-auto">
+                <div class="input-group" style="width:550px">
+                    <span class="input-group-text">
+                      Activity
+                    </span>
+                    <input type="text" id="activity" class="form-control"  placeholder="Input activity"  autocomplete="off">
+                    <a onclick="getCurActivity()" class="input-group-text" style="cursor: pointer;color: rgb(0, 132, 255);">
+                      <strong>Get current activity</strong>
+                    </a>
+                </div>
+            </div>
+            {% endif %}
+            <div class="col-auto">
+                {% if platform == 'Android' %}
+                <a onclick="getStartupTimeByAndroid()" class="btn btn-default">
+                    <svg t="1647757457022" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="21859" width="200" height="200"><path d="M511.4 512.1m-448 0a448 448 0 1 0 896 0 448 448 0 1 0-896 0Z" fill="#006DFC" p-id="21860"></path><path d="M658.4 555.6L475.5 661.1c-33.4 19.3-75-4.8-75-43.3V406.6c0-38.5 41.7-62.6 75-43.3l182.9 105.6c33.3 19.3 33.3 67.4 0 86.7z" fill="#FFFFFF" p-id="21861"></path></svg>
+                    {% if lan == 'cn' %} 开始 {% else %} Start {% endif %}
+                </a>
+                {% else %}
+                <a onclick="getStartupTimeByiOS()" class="btn btn-default">
+                    <svg t="1647757457022" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="21859" width="200" height="200"><path d="M511.4 512.1m-448 0a448 448 0 1 0 896 0 448 448 0 1 0-896 0Z" fill="#006DFC" p-id="21860"></path><path d="M658.4 555.6L475.5 661.1c-33.4 19.3-75-4.8-75-43.3V406.6c0-38.5 41.7-62.6 75-43.3l182.9 105.6c33.3 19.3 33.3 67.4 0 86.7z" fill="#FFFFFF" p-id="21861"></path></svg>
+                    {% if lan == 'cn' %} 开始 {% else %} Start {% endif %}
+                </a>
+                <span class="form-help" style="margin-left: 10px;" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="
+                If no results are returned, please reinstall py-ios-device [pip install py-ios-device].
+                <p class='mb-0'><a href='https://github.com/YueChen-C/py-ios-device' target='_blank'>Documentation</a></p>">?</span> 
+                {% endif %}
+            </div>
+        </div>
+        <pre class="mt-2" id="startup-time-content"></pre>
+    </div>
+  </div>
+</div>
 {% endblock %}
 
 {% block js %}
 <script>
 
     var stop = false; // 任务状态
 
@@ -410,16 +458,17 @@
                     $('#device_name').text(data['device_detail']['name']);
                     $('#os_version').text(data['device_detail']['version']);
                     $('#serialno').text(data['device_detail']['serialno']);
                     $('#wifiadr').text(data['device_detail']['wifiadr']);
                     swal.close();
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error)
             }
         });
     }
 
     var timerQ = null;
 
     function getCpuRate(pkgname,device){
@@ -453,16 +502,17 @@
                             timerQ = setTimeout(getCpuRate(pkgname,device), 1500);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function getGpu(pkgname){
         $.ajax({
             url: Host + "/apm/gpu",
@@ -487,16 +537,17 @@
                             timerQ = setTimeout(getGpu(pkgname), 1000);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function getBattery(device){
         $.ajax({
             url: Host + "/apm/battery",
@@ -542,16 +593,17 @@
                             timerQ = setTimeout(getBattery(device), 10000);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function getMemPss(pkgname,device)  {
         $.ajax({
             url: Host + "/apm/mem",
@@ -594,16 +646,17 @@
 
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function setNetWork(type,device,pkgname,net_switch){
         $.ajax({
             url: Host + "/apm/set/network",
@@ -619,16 +672,17 @@
                 process:$('.select-pid').val()
             },
             success: function (data) {
                 if(data['status'] != 1){
                     SwalFire('error','something error',data['msg'],2000);
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function getNetWork(pkgname,device,net_switch)  {
         $.ajax({
             url: Host + "/apm/network",
@@ -663,16 +717,17 @@
                             console.log(e)
                         }
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     function getFps(pkgname,device,fps_switch)  {
         $.ajax({
             url: Host + "/apm/fps",
@@ -707,16 +762,17 @@
                             timerQ = setTimeout(getFps(pkgname,device,fps_switch), 1500);
                         }catch (e) {}
                     }else{
                         SwalFire('error','something error',data['msg'],2000);
                     }
                 }
             },
-            error: function(){
-                SwalFire('error','Host Error','Host is invalid',5000);
+            error: function(error){
+                SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
+                console.log(error);
             }
         });
     }
 
     var rangeSelector =  {
         buttons: [{
             count: 1,
@@ -1358,15 +1414,19 @@
                 SwalFire('error','Execution error','No device or package name selected',2000);
             }
             $('#run-apm').show();
             $('#stop-apm').hide();
         }});
 
     var status = false;
-    var socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
+    var socket
+    if(platform == 'Android'){
+        socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
+        
+    }
     function startLogcat() {
         let device = $('.select-device').val();
         if(device){
             $('#run-logcat').hide();
             $('#stop-logcat').show();
             socket = io.connect('http://' + document.domain + ':' + location.port + '/logcat',{'forceNew':true });
             socket.on('message', function (msg) {
@@ -1399,14 +1459,110 @@
         SwalFire('success','Copy Success','',1000);
     };
 
     function clearLogcat() {
         $('#logcat-content').empty();
     };
     
+    function getCurActivity(){
+        let device = $('.select-device').val();
+        if(device){
+            $.ajax({
+                url: "/package/activity",
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    platform:platform,
+                    device:$('.select-device').val(),
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                success: function (data) {
+                    if(data['status']==1){
+                        $('#activity').val(data['activity']);
+                    }else{
+                        SwalFire('error','Execution error',data['msg'],2000)
+                    }
+                },
+                complete: function(){
+                    swal.close();
+                }
+            });
+        }else{
+            SwalFire('error','Execution error','device is empty',2000)
+        }
+    }
+
+    function getStartupTimeByAndroid(){
+        let device = $('.select-device').val();
+        let activity = $('#activity').val().trim();
+        if(device && activity){
+            $.ajax({
+                url: "/package/start/time/android",
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    platform:platform,
+                    device:$('.select-device').val(),
+                    activity: activity
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                success: function (data) {
+                    if(data['status']==1){
+                        console.log(data['time'])
+                        $('#startup-time-content').text(data['time']);
+                    }else{
+                        SwalFire('error','Execution error',data['msg'],2000)
+                    }
+                },
+                complete: function(){
+                    swal.close();
+                }
+            });
+        }else{
+            SwalFire('error','Execution error','device or activity is empty',2000)
+        }
+    }
+
+    function getStartupTimeByiOS(){
+        let pkgname = $('.select-app').val();
+        if(pkgname){
+            $.ajax({
+                url: "/package/start/time/ios",
+                type: "GET",
+                async: true,
+                cache: false,
+                data:{
+                    pkgname:pkgname
+                },
+                beforeSend: function () {
+                    SwalLoading('Loading','')
+                },
+                success: function (data) {
+                    if(data['status']==1){
+                        console.log(data['time'])
+                        $('#startup-time-content').text(data['time']);
+                    }else{
+                        SwalFire('error','Execution error',data['msg'],2000)
+                    }
+                },
+                complete: function(){
+                    swal.close();
+                }
+            });
+        }else{
+            SwalFire('error','Execution error','pkgname is empty',2000)
+        }
+    }
+
     function install(){
         var fileObj = document.getElementById("app-file").files[0];
         var type = (fileObj) ? 'file' : 'link'
         if(type == 'file'){
             installFile()
         }else{
             installLink()
```

### Comparing `solox-2.6.0/solox/templates/pk.html` & `solox-2.6.1/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/templates/report.html` & `solox-2.6.1/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.0/solox/view/apis.py` & `solox-2.6.1/solox/view/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,15 @@
     return resp
 
 
 @api.route('/apm/initialize', methods=['post', 'get'])
 def initialize():
     """initialize apm env"""
     try:
-        report_dir = os.path.join(os.getcwd(), 'report')
-        if os.path.exists(report_dir):
-            for f in os.listdir(report_dir):
-                filename = os.path.join(report_dir, f)
-                if f.split(".")[-1] in ['log', 'json']:
-                    os.remove(filename)
+        f.clear_file()
         result = {'status': 1, 'msg': 'initialize env success'}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg': str(e)}
 
     return result
 
@@ -126,14 +121,53 @@
         pids = d.getPid(deviceId, pkgname)
         result = {'status': 1, 'pids': pids} 
     except Exception:
         traceback.print_exc()
         result = {'status': 0, 'msg': 'no pid found'} 
     return result        
 
+@api.route('/package/activity', methods=['post', 'get'])
+def getPackageActivity():
+    platform = method._request(request, 'platform')
+    device = method._request(request, 'device')
+    try:
+        deviceId = d.getIdbyDevice(device, platform)
+        activity = d.getCurrentActivity(deviceId)
+        result = {'status': 1, 'activity': activity} 
+    except Exception:
+        traceback.print_exc()
+        result = {'status': 0, 'msg': 'no activity found'} 
+    return result
+
+
+@api.route('/package/start/time/android', methods=['post', 'get'])
+def getStartupTimeByAndroid():
+    platform = method._request(request, 'platform')
+    device = method._request(request, 'device')
+    activity = method._request(request, 'activity')
+    try:
+        deviceId = d.getIdbyDevice(device, platform)
+        time = d.getStartupTimeByAndroid(activity, deviceId)
+        result = {'status': 1, 'time': time} 
+    except Exception:
+        traceback.print_exc()
+        result = {'status': 0, 'msg': 'no result found'} 
+    return result
+
+@api.route('/package/start/time/ios', methods=['post', 'get'])
+def getStartupTimeByiOS():
+    pkgname = method._request(request, 'pkgname')
+    try:
+        time = d.getStartupTimeByiOS(pkgname)
+        result = {'status': 1, 'time': time} 
+    except Exception:
+        traceback.print_exc()
+        result = {'status': 0, 'msg': 'no result found'} 
+    return result
+
 @api.route('/apm/cpu', methods=['post', 'get'])
 def getCpuRate():
     """get process cpu rate"""
     model = method._request(request, 'model')
     platform = method._request(request, 'platform')
     pkgname = method._request(request, 'pkgname')
     device = method._request(request, 'device')
@@ -329,15 +363,15 @@
     return result
 
 @api.route('/apm/gpu', methods=['post', 'get'])
 def getGpu():
     """get gpu data"""
     pkgname = method._request(request, 'pkgname')
     try:
-        gpu = GPU(pkgname=pkgname)
+        gpu = GPU(pkgName=pkgname)
         final = gpu.getGPU()
         result = {'status': 1, 'gpu': final}
     except Exception:
         traceback.print_exc()
         result = {'status': 1, 'gpu': 0}
     return result
 
@@ -360,15 +394,15 @@
             wifi = False if wifi_switch == 'false' else True
             deviceId = d.getIdbyDevice(devices, platform)
             pid = process.split(':')[0] if platform == Platform.Android else None
             flow = Flow(pkgName=app, deviceId=deviceId, platform=platform, pid=pid)
             data = flow.setAndroidNet(wifi=wifi)
             f.record_net('end', data[0], data[1])
             app = process
-        File(fileroot=f'apm_{current_time}').make_report(app=app, devices=devices, platform=platform, model=model)
+        f.make_report(app=app, devices=devices, platform=platform, model=model)
         result = {'status': 1}
     except Exception as e:
         traceback.print_exc()
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
@@ -499,14 +533,43 @@
             'gpu': f.getGpuLog(platform, scene)
         }
         result = fucDic[target]
     except Exception as e:
         result = {'status': 0, 'msg': str(e)}
     return result
 
+@api.route('/apm/log/compare', methods=['post', 'get'])
+def getLogCompareData():
+    """Get apm detailed data"""
+    scene1 = method._request(request, 'scene1')
+    scene2 = method._request(request, 'scene2')
+    target = method._request(request, 'target')
+    platform = method._request(request, 'platform')
+    try:
+        match(target):
+            case Target.CPU:
+                result = f.getCpuLogCompare(platform, scene1, scene2)
+            case Target.Memory:
+                result = f.getMemLogCompare(platform, scene1, scene2)
+            case Target.Battery:
+                result = f.getBatteryLogCompare(platform, scene1, scene2)
+            case Target.FPS:
+                result = f.getFpsLogCompare(platform, scene1, scene2)
+            case Target.GPU:
+                result = f.getGpuLogCompare(platform, scene1, scene2)
+            case 'net_send':
+                result = f.getFlowSendLogCompare(platform, scene1, scene2)
+            case 'net_recv':
+                result = f.getFlowRecvLogCompare(platform, scene1, scene2)                     
+            case _:
+                result = {'status': 0, 'msg': 'no target found'}        
+    except Exception as e:
+        result = {'status': 0, 'msg': str(e)}
+    return result
+
 @api.route('/apm/log/pk', methods=['post', 'get'])
 def getpkLogData():
     """Get apm detailed data"""
     scene = method._request(request, 'scene')
     target1 = method._request(request, 'target1')
     target2 = method._request(request, 'target2')
     try:
```

### Comparing `solox-2.6.0/solox/web.py` & `solox-2.6.1/solox/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,17 @@
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
+        logger.info('Initializing adb environment ...')
+        os.system('adb kill-server')
+        os.system('adb start-server')
         current_time = time.strftime("%Y%m%d%H", time.localtime())
         logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
         logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
         with open(logPath, "r") as f:
             while thread:
                 socketio.sleep(1)
@@ -60,24 +63,14 @@
 @socketio.on('disconnect_request', namespace='/logcat')
 def disconnect():
     global thread
     logger.warning('Logcat client disconnected')
     thread = False
     disconnect()
 
-
-def checkPyVer():
-    versions = platform.python_version().split('.')
-    if int(versions[0]) < 3:
-        logger.error('python version must be 3.10+ ,your python version is {}'.format(platform.python_version()))
-        sys.exit()
-    elif int(versions[1]) < 10:
-        logger.error('python version must be 3.10+ ,your python version is {}'.format(platform.python_version()))
-        sys.exit()
-
 def hostIP():
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.connect(('8.8.8.8', 80))
         ip = s.getsockname()[0]
     except Exception as e:
         raise e
```

### Comparing `solox-2.6.0/solox.egg-info/SOURCES.txt` & `solox-2.6.1/solox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 solox/static/js/sweetalert2.min.js
 solox/static/js/tabler.demo.min.js
 solox/static/js/tabler.min.js
 solox/static/logo/logo.png
 solox/templates/404.html
 solox/templates/500.html
 solox/templates/analysis.html
+solox/templates/analysis_compare.html
 solox/templates/analysis_pk.html
 solox/templates/base.html
 solox/templates/index.html
 solox/templates/pk.html
 solox/templates/report.html
 solox/view/__init__.py
 solox/view/apis.py
```

