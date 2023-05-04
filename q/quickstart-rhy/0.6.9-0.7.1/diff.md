# Comparing `tmp/QuickStart_Rhy-0.6.9.tar.gz` & `tmp/quickstart_rhy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickStart_Rhy-0.6.9.tar", last modified: Wed Mar  2 09:21:30 2022, max compression
+gzip compressed data, was "quickstart_rhy-0.7.1.tar", max compression
```

## Comparing `QuickStart_Rhy-0.6.9.tar` & `quickstart_rhy-0.7.1.tar`

### file list

```diff
@@ -1,62 +1,51 @@
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288929 QuickStart_Rhy-0.6.9/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-20 01:32:29.000000 QuickStart_Rhy-0.6.9/LICENSE
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.289005 QuickStart_Rhy-0.6.9/PKG-INFO
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.283704 QuickStart_Rhy-0.6.9/QuickStart_Rhy/
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.285666 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5540 2021-06-02 09:40:32.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3312 2022-01-25 08:11:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1207 2022-01-14 15:40:03.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5783 2021-06-02 09:41:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     8909 2022-02-20 18:53:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     6365 2021-05-15 16:08:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1110 2021-02-23 18:02:37.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    20384 2022-01-31 06:47:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/alapi.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.286469 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2307 2021-08-07 06:49:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    10325 2022-02-18 15:11:23.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      478 2021-08-07 06:47:43.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4005 2021-10-29 01:06:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       75 2021-01-14 15:40:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.287544 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1716 2021-04-14 06:04:07.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4934 2021-06-11 16:15:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3649 2022-03-02 09:15:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    11332 2022-03-02 05:36:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3673 2021-04-25 15:34:28.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3103 2021-01-27 06:50:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5763 2021-02-23 14:24:09.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288114 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     8861 2021-04-27 13:27:14.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4941 2021-04-30 07:48:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1127 2021-01-14 16:13:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1786 2021-04-04 02:34:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Monitor.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      623 2021-06-11 16:14:44.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288228 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2794 2021-01-14 16:19:31.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288698 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4118 2022-03-02 05:29:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1292 2021-04-04 02:31:01.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      549 2021-04-25 15:17:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      102 2022-02-19 14:45:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288813 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4765 2021-01-25 08:16:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9563 2022-02-19 14:36:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__config__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     7076 2022-02-20 18:27:06.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    36966 2022-02-25 17:33:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/api.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    12754 2022-02-24 10:06:39.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/funcList.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5368 2021-10-27 04:35:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3648 2022-02-13 16:31:26.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/main.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9085 2022-01-29 04:45:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/netTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2288 2022-02-14 15:11:41.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4882 2021-08-07 07:00:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.284587 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1636 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/SOURCES.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/dependency_links.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       49 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/entry_points.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       56 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/requires.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       15 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/top_level.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2020-04-02 18:40:53.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/zip-safe
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      425 2021-10-31 04:57:47.000000 QuickStart_Rhy-0.6.9/README.md
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-03-02 09:21:30.289244 QuickStart_Rhy-0.6.9/setup.cfg
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-03-02 09:21:22.000000 QuickStart_Rhy-0.6.9/setup.py
+-rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.1/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.1/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0        0        0     3419 2023-04-15 03:33:34.034264 quickstart_rhy-0.7.1/QuickStart_Rhy/API/ChatGPT.py
+-rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.1/QuickStart_Rhy/API/DeepL.py
+-rw-r--r--   0        0        0      778 2023-04-28 07:11:41.378497 quickstart_rhy-0.7.1/QuickStart_Rhy/API/DeepLX.py
+-rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.1/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.1/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.1/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.1/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.1/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.1/QuickStart_Rhy/API/alapi.py
+-rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/__init__.py
+-rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0        0        0     9151 2023-04-24 09:10:36.431917 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.1/QuickStart_Rhy/NumbaTools/__init__.py
+-rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/DiskMac.py
+-rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/__init__.py
+-rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.1/QuickStart_Rhy/ThreadTools/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.1/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.1/QuickStart_Rhy/__cache__.py
+-rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.1/QuickStart_Rhy/__config__.py
+-rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.1/QuickStart_Rhy/__init__.py
+-rw-r--r--   0        0        0    38783 2023-05-04 11:22:21.159295 quickstart_rhy-0.7.1/QuickStart_Rhy/apiTools.py
+-rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.1/QuickStart_Rhy/funcList.py
+-rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.1/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0        0        0    35036 2023-05-04 11:39:59.498252 quickstart_rhy-0.7.1/QuickStart_Rhy/lang.json
+-rw-r--r--   0        0        0     1728 2023-05-04 11:40:39.962676 quickstart_rhy-0.7.1/QuickStart_Rhy/main.py
+-rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.1/QuickStart_Rhy/netTools.py
+-rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.1/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.1/QuickStart_Rhy/system.py
+-rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.1/README.md
+-rw-r--r--   0        0        0      548 2023-05-04 11:48:24.493927 quickstart_rhy-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.1/setup.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.1/PKG-INFO
```

### Comparing `QuickStart_Rhy-0.6.9/LICENSE` & `quickstart_rhy-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/API/AliCloud.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # coding=utf-8
 """
 阿里云相关API
 
 Alibaba cloud API
 """
-from . import pre_check, user_lang, dir_char
+from . import pre_check, user_lang
 from .. import requirePackage
-oss2 = requirePackage('oss2')
 
 
 class AliyunOSS:
-    def __init__(self, ac_id=pre_check('aliyun_oss_acid'), ac_key=pre_check('aliyun_oss_ackey'),
-                 bucket_url=pre_check('aliyun_oss_df_endpoint'), df_bucket=pre_check('aliyun_oss_df_bucket')):
+    def __init__(
+        self,
+        ac_id=pre_check("aliyun_oss_acid"),
+        ac_key=pre_check("aliyun_oss_ackey"),
+        bucket_url=pre_check("aliyun_oss_df_endpoint"),
+        df_bucket=pre_check("aliyun_oss_df_bucket"),
+    ):
         """
         初始化并登陆阿里云对象存储
 
         Initializes and logs into ali cloud object storage
 
         :param ac_id: Access id
         :param ac_key: Access key
@@ -23,105 +27,125 @@
         :param df_bucket: 桶名称
         """
         self.ac_id = ac_id
         self.ac_key = ac_key
         self.bucket_url = bucket_url
         self.df_bucket = df_bucket
         self.progress, self.trans_id, self._progress_file_name = None, None, None
-        self.auth = oss2.Auth(self.ac_id, self.ac_key)
+        self.auth = requirePackage("oss2", "Auth")(self.ac_id, self.ac_key)
 
     def get_func_table(self):
         """
         获取OSS类支持的操作
 
         Get the operations supported by the OSS class
 
         :return: 支持的函数字典
         """
         return {
-            '-up': self.upload,
-            '-rm': self.remove,
-            '-dl': self.download,
-            '-ls': self.list_bucket
+            "-up": self.upload,
+            "-rm": self.remove,
+            "-dl": self.download,
+            "-ls": self.list_bucket,
         }
 
     def _progress_bar(self, cur, total):
         """
         创建一个进度条并启动
 
         Create a progress bar and start
 
         :param cur: 当前完成量
         :param total: 总任务量
         :return: None
         """
         if not self.progress:
             from ..TuiTools.Bar import DataTransformBar
+
             self.progress = DataTransformBar(True if total else False)
-            self.trans_id = self.progress.add_task('Transform', total=total if total else -1,
-                                                   filename=self._progress_file_name)
+            self.trans_id = self.progress.add_task(
+                "Transform",
+                total=total if total else -1,
+                filename=self._progress_file_name,
+            )
             self.progress.start()
             self.progress.start_task(self.trans_id)
         self.progress.update(self.trans_id, completed=cur)
 
-    def upload(self, filePath: str, bucket: str = None):
+    def upload(self, filePath: str, bucket: str = None, key: str = None):
         """
         上传文件（支持断点续传）
 
         Upload file (support breakpoint continuation)
 
         :param filePath: 文件路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
-        from .. import qs_default_console, qs_info_string
+        from .. import qs_default_console, qs_info_string, dir_char
         from ..SystemTools import get_core_num
+
         bucket = bucket if bucket else self.df_bucket
-        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
+        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
         filePath = filePath.strip()
         self._progress_file_name = os.path.basename(filePath)
-        oss2.resumable_upload(bucket, filePath.replace(dir_char, '/'), filePath, num_threads=get_core_num() * 4,
-                              progress_callback=self._progress_bar)
+        requirePackage("oss2", "resumable_upload")(
+            bucket,
+            key if key else filePath.replace(dir_char, "/"),
+            filePath,
+            num_threads=get_core_num() * 4,
+            progress_callback=self._progress_bar,
+        )
         self.progress.stop()
-        qs_default_console.print(qs_info_string, 'Transform Completed!' if user_lang != 'zh' else '传输完成!')
+        qs_default_console.print(
+            qs_info_string, "Transform Completed!" if user_lang != "zh" else "传输完成!"
+        )
 
     def download(self, filename: str, bucket: str = None):
         """
         下载文件（支持断点续传）
 
         Download file (support breakpoint continuation)
 
         :param filename: 文件在bucket中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
         from .. import qs_default_console, qs_info_string
         from ..SystemTools import get_core_num
+
         bucket = bucket if bucket else self.df_bucket
-        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
+        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
         self._progress_file_name = os.path.basename(filename)
-        oss2.resumable_download(bucket, filename, filename, num_threads=get_core_num() * 4,
-                                progress_callback=self._progress_bar)
+        requirePackage("oss2", "resumable_download")(
+            bucket,
+            filename,
+            filename,
+            num_threads=get_core_num() * 4,
+            progress_callback=self._progress_bar,
+        )
         self.progress.stop()
-        qs_default_console.print(qs_info_string, 'Transform Completed!' if user_lang != 'zh' else '传输完成!')
+        qs_default_console.print(
+            qs_info_string, "Transform Completed!" if user_lang != "zh" else "传输完成!"
+        )
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除文件
 
         delete file
 
         :param filePath: 文件在bucket中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         bucket = bucket if bucket else self.df_bucket
-        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
+        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
         bucket.delete_object(filePath)
 
     def list_bucket(self, bucket: str = None):
         """
         打印桶中的文件表
 
         Print the file table in the bucket
@@ -131,20 +155,25 @@
         """
         from .. import qs_default_console, qs_info_string
         from ..NetTools.NormalDL import size_format
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
 
         bucket = bucket if bucket else self.df_bucket
-        ls = oss2.Bucket(self.auth, self.bucket_url, bucket)
-        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='Aliyun OSS')
+        ls = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
+        tb = qs_default_table(
+            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="Aliyun OSS"
+        )
         prefix = dict()
-        for obj in oss2.ObjectIterator(ls):
-            if '/' in obj.key:
-                prefix[obj.key[obj.key[:obj.key.index('/')]]] = 0
-            tb.add_row(Text(obj.key, justify='left'), Text(size_format(obj.size, True), justify='right'))
+        for obj in requirePackage("oss2", "ObjectIterator")(ls):
+            if "/" in obj.key:
+                prefix[obj.key[obj.key[: obj.key.index("/")]]] = 0
+            tb.add_row(
+                Text(obj.key, justify="left"),
+                Text(size_format(obj.size, True), justify="right"),
+            )
         qs_default_console.print(
             qs_info_string,
-            'Bucket Url:' if user_lang != 'zh' else '桶链接:',
-            'https://' + bucket + '.' + self.bucket_url + '/'
+            "Bucket Url:" if user_lang != "zh" else "桶链接:",
+            "https://" + bucket + "." + self.bucket_url + "/",
         )
         qs_default_console.print(tb, justify="center")
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,80 +3,104 @@
 百度云相关API
 
 Baidu cloud API
 """
 import os
 from . import pre_check, user_lang
 from .. import qs_default_console, qs_error_string, qs_info_string, requirePackage
-aip = requirePackage('aip', real_name='baidu-aip')
+
+imgp = requirePackage("aip", "imageprocess", real_name="baidu-aip")
+aip = requirePackage("aip", real_name="baidu-aip")
 
 
 class ImageDeal:
     """
     百度图像处理类
 
     Baidu image processing class
     """
+
     import base64
 
-    def __init__(self, app_id: str = pre_check('AipImageAPP_ID'),
-                 app_key: str = pre_check('AipImageAPP_KEY'),
-                 secret_key: str = pre_check('AipImageSECRET_KEY')):
+    def __init__(
+        self,
+        app_id: str = pre_check("AipImageAPP_ID"),
+        app_key: str = pre_check("AipImageAPP_KEY"),
+        secret_key: str = pre_check("AipImageSECRET_KEY"),
+    ):
         """
         初始化并登陆百度图像处理
 
         Initialize and log in Baidu image processing
 
         :param app_id: 应用ID
         :param app_key: 应用key
         :param secret_key: 密钥
         """
-        self.client = aip.AipImageProcess(app_id, app_key, secret_key)
+        self.client = imgp.AipImageProcess(app_id, app_key, secret_key)
 
-    def largeImage(self, path: str, st: qs_default_console.status = None):
+    def largeImage(self, path: str):
         """
         放大图片 (图像效果增强)
 
         Enlarge image (Image Enhancement)
 
         :param st: console状态
         :param path: 图片路径
         :return: None
         """
         if not os.path.exists(path) or not os.path.isfile(path):
-            qs_default_console.log(qs_error_string, ('No file named: %s' if user_lang != 'zh' else '没有文件: %s') % path)
+            qs_default_console.log(
+                qs_error_string,
+                ("No file named: %s" if user_lang != "zh" else "没有文件: %s") % path,
+            )
             return
         img_name = os.path.basename(path)
-        img_name = img_name[:img_name.index('.')] + '_LG.' + '.'.join(img_name.split('.')[1:])
-
-        with qs_default_console.status(f'{"Reading Image" if user_lang != "zh" else "读取图片"}: {path}') if not st else st as status:
-            with open(path, 'rb') as f:
+        img_name = (
+            img_name[: img_name.index(".")] + "_LG." + ".".join(img_name.split(".")[1:])
+        )
+
+        from .. import qs_default_status
+
+        with qs_default_status(
+            f'{"Reading Image" if user_lang != "zh" else "读取图片"}: {path}'
+        ) as status:
+            with open(path, "rb") as f:
                 img = f.read()
-            status.update(status=f'{qs_info_string} {"Dealing..." if user_lang != "zh" else "处理中..."}')
+            status.update(
+                f'{qs_info_string} {"Dealing..." if user_lang != "zh" else "处理中..."}'
+            )
             img = self.client.imageQualityEnhance(img)
             try:
-                status.update(status=f'{qs_info_string} {"Write to" if user_lang != "zh" else "写入"}: {img_name}')
-                img = ImageDeal.base64.b64decode(img['image'])
-                with open(img_name, 'wb') as f:
+                status.update(
+                    f'{qs_info_string} {"Write to" if user_lang != "zh" else "写入"}: {img_name}'
+                )
+                img = ImageDeal.base64.b64decode(img["image"])
+                with open(img_name, "wb") as f:
                     f.write(img)
             except:
                 qs_default_console.print(qs_error_string, img)
-        qs_default_console.print(qs_info_string, "Deal Done!" if user_lang != "zh" else "处理完成!")
+        qs_default_console.print(
+            qs_info_string, "Deal Done!" if user_lang != "zh" else "处理完成!"
+        )
 
 
 class AipNLP:
     """
     百度语言处理类
 
     Baidu language processing class
     """
-    def __init__(self,
-                 appid: str = pre_check("AipNlpAPP_ID"),
-                 appkey: str = pre_check("AipNlpAPP_KEY"),
-                 sckey: str = pre_check("AipNlpSECRET_KEY")):
+
+    def __init__(
+        self,
+        appid: str = pre_check("AipNlpAPP_ID"),
+        appkey: str = pre_check("AipNlpAPP_KEY"),
+        sckey: str = pre_check("AipNlpSECRET_KEY"),
+    ):
         """
         初始化并登陆百度语言处理应用
 
         Initialize and log in baidu language processing application
 
         :param appid: 应用ID
         :param appkey: 应用Key
@@ -90,12 +114,12 @@
 
         Text error correction
 
         :param words: 待处理文本
         :return: 处理后的文本 | proceed words
         """
         try:
-            res = self.client.ecnet(words)['item']['correct_query']
+            res = self.client.ecnet(words)["item"]["correct_query"]
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
         else:
             return res
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # coding=utf-8
 """
 七牛云对象存储API
 
 Qiniu cloud OSS API
 """
-from . import pre_check, dir_char, user_lang
+from . import pre_check, user_lang
 from .. import requirePackage
 
 
 class QiniuOSS:
-    qiniu = requirePackage('qiniu')
+    qiniu = requirePackage("qiniu")
 
-    def __init__(self, ac_key: str = pre_check('qiniu_ac_key'),
-                 sc_key: str = pre_check('qiniu_sc_key'),
-                 df_bucket: str = pre_check('qiniu_bk_name')):
+    def __init__(
+        self,
+        ac_key: str = None,
+        sc_key: str = None,
+        df_bucket: str = None,
+    ):
         """
         初始化并登陆七牛云对象存储
 
         Initializes and logs in qiniu cloud object storage
 
         :param ac_key: Access Key
         :param sc_key: Secret Key
         :param df_bucket: 默认桶名称
         """
+        if not (ac_key and sc_key and df_bucket):
+            ac_key, sc_key, df_bucket = pre_check(
+                "qiniu_ac_key", "qiniu_sc_key", "qiniu_bk_name"
+            )
         self.ac_key = ac_key
         self.sc_key = sc_key
         self.auth = QiniuOSS.qiniu.Auth(self.ac_key, self.sc_key)
         self.df_bucket = df_bucket
         self.bar, self.tid = None, None
 
     def get_func_table(self):
@@ -34,46 +41,58 @@
         获取对象支持的操作
 
         Gets the operations supported by the object
 
         :return: 函数表
         """
         return {
-            '-up': self.upload,
-            '-rm': self.remove,
-            '-cp': self.copy_url,
-            '-dl': self.download,
-            '-ls': self.list_bucket
+            "-up": self.upload,
+            "-rm": self.remove,
+            "-cp": self.copy_url,
+            "-dl": self.download,
+            "-ls": self.list_bucket,
         }
 
-    def upload(self, filePath: str, bucket: str = None):
+    def upload(self, filePath: str, bucket: str = None, key: str = None):
         """
         上传文件
 
         Upload file
 
         :param filePath: 文件路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
+        from .. import dir_char
+
         filename = os.path.basename(filePath)
 
         def progress(cur, total):
             if not self.bar:
                 from ..TuiTools.Bar import DataTransformBar
+
                 self.bar = DataTransformBar()
-                self.tid = self.bar.add_task('Transform' if user_lang != 'zh' else '传输', filename=filename, total=total)
+                self.tid = self.bar.add_task(
+                    "Transform" if user_lang != "zh" else "传输",
+                    filename=filename,
+                    total=total,
+                )
                 self.bar.start()
                 self.bar.start_task(self.tid)
             self.bar.update(self.tid, completed=cur)
 
         filePath = filePath.strip()
         tk = self.auth.upload_token(bucket if bucket else self.df_bucket, filePath)
-        QiniuOSS.qiniu.put_file(tk, filePath.replace(dir_char, '/'), filePath, progress_handler=progress)
+        QiniuOSS.qiniu.put_file(
+            tk,
+            key if key else filePath.replace(dir_char, "/"),
+            filePath,
+            progress_handler=progress,
+        )
         self.bar.stop()
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除文件
 
         Delete file
@@ -92,32 +111,38 @@
         Copy files through URL (this interface seems to have no egg use, qiniu cloud will not work)
 
         :param filePath: 文件链接
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         bk = QiniuOSS.qiniu.BucketManager(self.auth)
-        bk.fetch(filePath, bucket if bucket else self.df_bucket, filePath.split('/')[-1])
+        bk.fetch(
+            filePath, bucket if bucket else self.df_bucket, filePath.split("/")[-1]
+        )
 
     def get_bucket_url(self, bucket: str = None):
         """
         获取当前桶的访问链接
 
         Gets the access link for the current bucket
 
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: 成功返回json，否则False
         """
         import requests
+
         bucket = bucket if bucket else self.df_bucket
-        url = 'http://api.qiniu.com/v6/domain/list?tbl=%s' % bucket
-        res = requests.get(url, headers={
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Authorization": "QBox %s" % self.auth.token_of_request(url)
-        })
+        url = "http://api.qiniu.com/v6/domain/list?tbl=%s" % bucket
+        res = requests.get(
+            url,
+            headers={
+                "Content-Type": "application/x-www-form-urlencoded",
+                "Authorization": "QBox %s" % self.auth.token_of_request(url),
+            },
+        )
         if res.status_code == requests.codes.ok:
             return res.json()
         else:
             return False
 
     def list_bucket(self, bucket: str = None):
         """
@@ -127,42 +152,52 @@
 
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from .. import qs_default_console, qs_info_string
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
+
         bk = QiniuOSS.qiniu.BucketManager(self.auth)
         ret = bk.list(bucket if bucket else self.df_bucket)
         if not ret[1]:
-            print("ERROR!" if user_lang != 'zh' else '错误!')
+            print("ERROR!" if user_lang != "zh" else "错误!")
             exit(0)
-        root_url = 'http://' + self.get_bucket_url(bucket)[0] + '/'
-        ret = ret[0]['items']
+        root_url = "http://" + self.get_bucket_url(bucket)[0] + "/"
+        ret = ret[0]["items"]
         from ..NetTools.NormalDL import size_format
-        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='七牛 OSS')
+
+        tb = qs_default_table(
+            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="七牛 OSS"
+        )
         for i in ret:
-            tb.add_row(Text(i['key'], justify="left"), Text(size_format(i['fsize'], True), justify='right'))
-        qs_default_console.print(qs_info_string, "Bucket url:" if user_lang != 'zh' else '桶链接:', root_url)
+            tb.add_row(
+                Text(i["key"], justify="left"),
+                Text(size_format(i["fsize"], True), justify="right"),
+            )
+        qs_default_console.print(
+            qs_info_string, "Bucket url:" if user_lang != "zh" else "桶链接:", root_url
+        )
         qs_default_console.print(tb, justify="center")
 
     def download(self, filePath: str, bucket: str = None):
         """
         下载文件
 
         Download file
 
         :param filePath: 文件在桶中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from ..NetTools.NormalDL import normal_dl
+
         bucket = bucket if bucket else self.df_bucket
         root_url = self.get_bucket_url(bucket)[0]
         if root_url:
-            root_url = 'http://' + root_url + '/'
+            root_url = "http://" + root_url + "/"
         else:
-            exit('Get Bucket Url Failed!' if user_lang != 'zh' else '获取桶链接失败!')
+            exit("Get Bucket Url Failed!" if user_lang != "zh" else "获取桶链接失败!")
         dl_url = root_url + filePath
-        if bucket.startswith('admin'):
+        if bucket.startswith("admin"):
             dl_url = self.auth.private_download_url(dl_url)
         normal_dl(dl_url)
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     删除图片背景
 
     Delete image background
 
     :param filePath: 图片的路径
     :return: None
     """
-    api_key = pre_check('rmbg')
+    api_key = pre_check("rmbg")
     res = requests.post(
-        'https://api.remove.bg/v1.0/removebg',
-        files={'image_file': open(filePath, 'rb')},
-        data={'size': 'auto'},
-        headers={'X-Api-Key': api_key},
+        "https://api.remove.bg/v1.0/removebg",
+        files={"image_file": open(filePath, "rb")},
+        data={"size": "auto"},
+        headers={"X-Api-Key": api_key},
     )
     if res.status_code == requests.codes.ok:
-        img_name = filePath.split(dir_char)[-1].split('.')[0]
-        if dir_char in filePath:
-            img_root = dir_char.join(filePath.split(dir_char)[:-1]) + dir_char
-        else:
-            img_root = ''
-        with open(img_root + img_name + '_rmbg.png', 'wb') as imgfile:
+        import os
+
+        img_name = os.path.basename(filePath).split(".")[0]
+        img_root = os.path.dirname(os.path.abspath(filePath))
+
+        with open(os.path.join(img_root, img_name + "_rmbg.png"), "wb") as imgfile:
             imgfile.write(res.content)
     else:
         qs_default_console.log(qs_error_string, res.status_code, res.text)
 
 
 def smms(filePath: str):
     """
@@ -44,177 +44,212 @@
 
     Upload images or all images from Markdown to SMMS
 
     :param filePath: 图片或Markdown文件的路径
     :return: None
     """
     import os
+    from .. import user_root
     from ..TuiTools.Table import qs_default_table
 
-    api_key = pre_check('smms')
-    res_tb = qs_default_table(['File', 'Status', 'url'] if user_lang != 'zh' else ['文件', '状态', '链接'])
+    api_key = pre_check("smms")
+    res_tb = qs_default_table(
+        ["File", "Status", "url"] if user_lang != "zh" else ["文件", "状态", "链接"]
+    )
 
     def post_img(path: str) -> dict:
         try:
-            data = {
-                'smfile': (path.split('/')[-1], open(path, 'rb')),
-                'format': 'json'
-            }
+            data = {"smfile": (path.split("/")[-1], open(path, "rb")), "format": "json"}
         except:
             return {}
-        res_json = requests.post('https://sm.ms/api/v2/upload', headers={'Authorization': api_key}, files=data).text
+        res_json = requests.post(
+            "https://sm.ms/api/v2/upload",
+            headers={"Authorization": api_key},
+            files=data,
+        ).text
         return json.loads(res_json)
 
     def get_path(rt, rel):
-        return os.path.abspath(rt + rel)
+        return os.path.abspath(os.path.join(rt, rel))
 
     def format_markdown(path):
         import re
-        _user_path = os.path.expanduser('~')
-        rt_path = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
+
+        rt_path = os.path.dirname(os.path.abspath(path))
         img_set = {}
-        with open(path, 'r') as fp:
+        with open(path, "r") as fp:
             ct = fp.read()
-        aims = re.findall('!\[.*?]\((.*?)\)', ct, re.M) + re.findall('<img.*?src="(.*?)".*?>', ct, re.M)
+        aims = re.findall("!\[.*?]\((.*?)\)", ct, re.M) + re.findall(
+            '<img.*?src="(.*?)".*?>', ct, re.M
+        )
         for aim in aims:
             raw_path = aim
-            aim = aim.replace('~', _user_path)
-            aim = aim if aim.startswith(dir_char) else get_path(rt_path, aim)
+            aim = get_path(rt_path, aim.replace("~", user_root))
             if aim not in img_set:
                 res_dict = post_img(aim)
                 if not res_dict:
-                    res_tb.add_row(aim.split(dir_char)[-1], 'No File', '')
+                    res_tb.add_row(os.path.basename(aim), "No File", "")
                     img_set[aim] = False
                 else:
                     res_tb.add_row(
-                        aim.split(dir_char)[-1], res_dict['success'],
-                        res_dict['message'] if not res_dict['success'] else res_dict['data']['url']
+                        os.path.basename(aim),
+                        res_dict["success"],
+                        res_dict["message"]
+                        if not res_dict["success"]
+                        else res_dict["data"]["url"],
                     )
-                    if not res_dict['success'] and res_dict['code'] == 'unauthorized':
+                    if not res_dict["success"] and res_dict["code"] == "unauthorized":
                         break
-                    img_set[aim] = res_dict['data']['url'] if res_dict['success'] else False
+                    img_set[aim] = (
+                        res_dict["data"]["url"] if res_dict["success"] else False
+                    )
             if img_set[aim]:
                 ct = ct.replace(raw_path, img_set[aim])
-        with open(path, 'w') as fp:
+        with open(path, "w") as fp:
             fp.write(ct)
         qs_default_console.print(res_tb, justify="center")
 
     try:
-        is_md = filePath.endswith('.md')
+        is_md = filePath.endswith(".md")
     except IndexError:
-        exit('Usage: qs {*.md} | {picture}')
+        exit("Usage: qs {*.md} | {picture}")
     else:
         if is_md:
             format_markdown(filePath)
         else:
             res = post_img(filePath)
             if not res:
-                res_tb.add_row(filePath.split(dir_char)[-1], 'No File', '')
+                res_tb.add_row(os.path.basename(filePath), "No File", "")
             else:
                 res_tb.add_row(
-                    filePath.split(dir_char)[-1], res['success'], '' if not res['success'] else res['data']['url'])
+                    os.path.basename(filePath),
+                    res["success"],
+                    "" if not res["success"] else res["data"]["url"],
+                )
             qs_default_console.print(res_tb, justify="center")
 
 
 def imgs_in_url(url: str, save: bool = False):
     """
     提取url中的img标签链接
 
     Extract img tag links from url
 
     :param url:
     :param save:
     :return:
     """
-    from .. import headers
+    from ..NetTools import headers
+
     html = requests.get(url, headers=headers)
     if html.status_code != requests.codes.ok:
-        qs_default_console.log(qs_error_string, 'Network Error' if user_lang != 'zh' else '网络错误')
+        qs_default_console.log(
+            qs_error_string, "Network Error" if user_lang != "zh" else "网络错误"
+        )
         return
     import re
     from ..ImageTools.ImagePreview import image_preview
+
     normal_dl = None
     if save:
         from ..NetTools.NormalDL import normal_dl
 
     imgs = re.findall('<img.*?src="(.*?)".*?>', html.text)
     a_ls = re.findall('<a.*?href="(.*?)".*?>', html.text)
     for i in a_ls:
         aim = i.lower()
-        for j in ['.png', '.jpg', 'jpeg']:
+        for j in [".png", ".jpg", "jpeg"]:
             if j in aim:
                 imgs.append(i)
                 break
     for url in imgs:
-        if not url.startswith('http') or url.endswith('svg'):
+        if not url.startswith("http") or url.endswith("svg"):
             continue
-        url = url.replace('&#46;', '.')
+        url = url.replace("&#46;", ".")
         qs_default_console.log(
-            qs_info_string, 'Link:' if user_lang != 'zh' else '链接:', url[:100] + ('' if len(url) <= 100 else '...'))
+            qs_info_string,
+            "Link:" if user_lang != "zh" else "链接:",
+            url[:100] + ("" if len(url) <= 100 else "..."),
+        )
         if save:
-            normal_dl(url)
-        if system == 'darwin':
-            try:
-                image_preview(url, True)
-            except Exception as e:
-                qs_default_console.log(qs_error_string, repr(e))
+            file_name = normal_dl(url)
+        else:
+            file_name = url
+        image_preview(file_name, True)
 
 
 def acg2():
     """
     随机获取一张acg图片链接
 
     Get a random link to an ACG image
 
     :return: 请求状态, 链接或报错, 宽度, 高度 | status, url or error, width, height
     """
     try:
-        res = requests.get('https://api.luvying.com/acgimg?return=json')
+        res = requests.get("https://api.luvying.com/acgimg?return=json")
     except Exception as e:
         return False, repr(e), None, None
     else:
         import json
+
         res = json.loads(res.text)
-        return res['code'] == '200', (res['acgurl'] if res['code'] == '200' else 'Error'), res['width'], res['height']
+        return (
+            res["code"] == "200",
+            (res["acgurl"] if res["code"] == "200" else "Error"),
+            res["width"],
+            res["height"],
+        )
 
 
-def wallhaven(set_search_url: str = pre_check('wallhaven_aim_url', False), randomOne: bool = False):
+def wallhaven(
+    set_search_url: str = pre_check("wallhaven_aim_url", ext=False),
+    randomOne: bool = False,
+):
     """
     获取wallhaven toplist或指定图片列表
 
     Get wallhaven toplist or specified picture list
 
     :param set_search_url: 用于搜索的URL
     :param randomOne: 随机抽一张返回
     :return: 包含链接的列表 | [link1, link2, ...]
     """
     from .. import qs_default_console, qs_error_string
-    from . import headers
+    from ..NetTools import headers
     import requests
     import re
 
     if not set_search_url:
-        set_search_url = 'https://wallhaven.cc/search?categories=010&purity=011&topRange=1M&sorting=toplist&order=desc'
+        set_search_url = "https://wallhaven.cc/search?categories=010&purity=011&topRange=1M&sorting=toplist&order=desc"
 
-    urlTemplate = 'https://w.wallhaven.cc/full/{}/wallhaven-{}'
+    urlTemplate = "https://w.wallhaven.cc/full/{}/wallhaven-{}"
     html = requests.get(set_search_url, headers=headers)
     if html.status_code != requests.codes.ok:
-        qs_default_console.print(qs_error_string, f'Http Status: {html.status_code}')
+        qs_default_console.print(qs_error_string, f"Http Status: {html.status_code}")
         return None
-    html = re.findall('<section.*?>(.*?)</section', html.text, re.S)[0]
-    lis = re.findall('<li>(.*?)</li', html, re.S)
+    html = re.findall("<section.*?>(.*?)</section", html.text, re.S)[0]
+    lis = re.findall("<li>(.*?)</li", html, re.S)
     res = []
     for i in lis:
-        url, size = re.findall('<img.*?data-src="(.*?)".*?<span.*?class="wall-res".*?>(.*?)<', i, re.S)[0]
-        url = url.split('/')[-2:]
+        url, size = re.findall(
+            '<img.*?data-src="(.*?)".*?<span.*?class="wall-res".*?>(.*?)<', i, re.S
+        )[0]
+        url = url.split("/")[-2:]
         if '<span class="png">' in i:
-            url[-1] = url[-1].replace('.jpg', '.png')
-        res.append({'url': urlTemplate.format(*url), 'size': [int(i) for i in re.findall('\d+\.?\d*', size)]})
+            url[-1] = url[-1].replace(".jpg", ".png")
+        res.append(
+            {
+                "url": urlTemplate.format(*url),
+                "size": [int(i) for i in re.findall("\d+\.?\d*", size)],
+            }
+        )
     if randomOne:
         import random
+
         return [random.choice(res)]
     return res
 
 
 def lmgtfy(keyword: str):
     """
     让我帮你Google一下
@@ -222,47 +257,64 @@
     Let me google that for you
 
     :param keyword: 关键词
     :return: 目标链接 | http link
     """
     import random
     import base64
-    supportLs = [
-        'https://moedog.org/tools/google/?q='
-    ]
-    return random.choice(supportLs) + base64.b64encode(bytes(keyword, 'utf-8')).decode('utf-8')
+
+    supportLs = ["https://moedog.org/tools/google/?q="]
+    return random.choice(supportLs) + base64.b64encode(bytes(keyword, "utf-8")).decode(
+        "utf-8"
+    )
 
 
 class Designation2magnet:
     import re
 
     def __init__(self, description):
-        self.rt_url = 'https://3mag.net'
+        self.rt_url = "https://18mag.net"
+        self.cover_url = "https://www5.javmost.com/search/{designation}/"
         self.description = description
 
     def search_designation(self):
         """
         番号搜索
 
         :return:
         """
         infos = [
-            Designation2magnet.re.findall('<a.*?href="(.*?)".*?>(.*?)<.*?td-size.*?>(.*?)<', item, Designation2magnet.re.S) for item in
-            Designation2magnet.re.findall('<tr>(.*?)</tr>', requests.get(self.rt_url + '/search?q={}'.format(self.description)).text.replace('<b>', '').replace('</b>', ''), Designation2magnet.re.S)
+            Designation2magnet.re.findall(
+                '<a.*?href="(.*?)".*?>(.*?)<.*?td-size.*?>(.*?)<',
+                item,
+                Designation2magnet.re.S,
+            )
+            for item in Designation2magnet.re.findall(
+                "<tr>(.*?)</tr>",
+                requests.get(self.rt_url + "/search?q={}".format(self.description))
+                .text.replace("<b>", "")
+                .replace("</b>", ""),
+                Designation2magnet.re.S,
+            )
         ]
         if [] in infos:
-            return [(i[0][0], i[0][1].strip(), i[0][2]) for i in infos[:infos.index([])]]
+            return [
+                (i[0][0], i[0][1].strip(), i[0][2]) for i in infos[: infos.index([])]
+            ]
         else:
             return [(i[0][0], i[0][1].strip(), i[0][2]) for i in infos]
 
     def get_magnet(self, info: str):
         """
         将选定的信息转为磁力链
 
         :param info:
         :return:
         """
-        return 'magnet:?xt=urn:btih:' + Designation2magnet.re.findall(
-            '种子特征码.*?<dd>(.*?)<',
-            requests.get(self.rt_url + info).text,
-            Designation2magnet.re.S
-        )[0]
+        return (
+            "magnet:?xt=urn:btih:"
+            + Designation2magnet.re.findall(
+                "种子特征码.*?<dd>(.*?)<",
+                requests.get(self.rt_url + info).text,
+                Designation2magnet.re.S,
+            )[0]
+        )
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/API/TencentCloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,110 @@
 # coding=utf-8
 """
 腾讯云相关API
 
 Tencent cloud API
 """
 import json
-from .. import requirePackage
-from . import pre_check, user_lang, dir_char
+from .. import requirePackage, user_lang
+from . import pre_check
 
 
 class TxCOS:
-    qcloud_cos = requirePackage('qcloud_cos', real_name='cos-python-sdk-v5')
-
-    def __init__(self):
+    def __init__(self, scid=None, sckey=None, region=None, bucket=None, cdn_url=None):
         """
         初始化并登陆腾讯云对象存储
 
         Initialize and log in Tencent Cloud object storage
+
+        :param scid: SecretId
+        :param sckey: SecretKey
+        :param region: 地区
+        :param bucket: 桶名称
+        :param cdn_url: CDN地址
+
+        :return: None
         """
-        scid = pre_check('txyun_scid')
-        sckey = pre_check('txyun_sckey')
-        self.region = pre_check('txyun_df_region')
-        self.df_bucket = pre_check('txyun_cos_df_bucket')
-        self.cdn_url = pre_check('txyun_df_cdn_url', ext=False)
-        if self.cdn_url and not self.cdn_url.endswith('/'):
-            self.cdn_url += '/'
-        config = TxCOS.qcloud_cos.CosConfig(Region=self.region,
-                                            SecretId=scid,
-                                            SecretKey=sckey)
-        self.client = TxCOS.qcloud_cos.CosS3Client(config)
+        if not (scid and sckey and region and bucket):
+            scid, sckey, self.region, self.df_bucket = pre_check(
+                "txyun_scid", "txyun_sckey", "txyun_df_region", "txyun_cos_df_bucket"
+            )
+        self.cdn_url = (
+            pre_check("txyun_df_cdn_url", ext=False) if not cdn_url else cdn_url
+        )
+        if self.cdn_url and not self.cdn_url.endswith("/"):
+            self.cdn_url += "/"
+
+        qcloud_cos = requirePackage("qcloud_cos", real_name="cos-python-sdk-v5")
+
+        config = qcloud_cos.CosConfig(
+            Region=self.region, SecretId=scid, SecretKey=sckey
+        )
+        self.client = qcloud_cos.CosS3Client(config)
 
     def get_func_table(self):
         """
         获取对象支持的函数表
 
         Gets a table of functions supported by the object
 
         :return: 函数表
         """
         return {
-            '-up': self.upload,
-            '-rm': self.remove,
-            '-dl': self.download,
-            '-ls': self.list_bucket
+            "-up": self.upload,
+            "-rm": self.remove,
+            "-dl": self.download,
+            "-ls": self.list_bucket,
         }
 
-    def upload(self, filePath: str, bucket: str = None):
+    def upload(self, filePath: str, bucket: str = None, key: str = None):
         """
         上传文件
 
         Upload file
 
+        :param key: 在COS上的文件路径
         :param filePath: 文件地址
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
+        from .. import dir_char
+
         bucket = bucket if bucket else self.df_bucket
         filename = filePath.strip()
-        self.client.upload_file(Bucket=bucket, LocalFilePath=filename, Key=filename.replace(dir_char, '/'))
+        self.client.upload_file(
+            Bucket=bucket,
+            LocalFilePath=filename,
+            Key=key if key else filename.replace(dir_char, "/"),
+        )
 
     def download(self, filename: str, bucket: str = None):
         """
         下载文件
 
         Download file
 
         :param filename: 文件在桶中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from ..NetTools.NormalDL import normal_dl
+
         bucket = bucket if bucket else self.df_bucket
 
-        url = self.cdn_url + filename \
-            if bucket == self.df_bucket and self.cdn_url else \
-            'https://' + bucket + '.cos.' + self.region + '.myqcloud.com/' + filename
+        url = (
+            self.cdn_url + filename
+            if bucket == self.df_bucket and self.cdn_url
+            else "https://"
+            + bucket
+            + ".cos."
+            + self.region
+            + ".myqcloud.com/"
+            + filename
+        )
         normal_dl(url)  # * 由于腾讯云没有提供可调用的下载sdk，因此使用qs下载引擎下载
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除桶中的文件
 
         Delete files in the bucket
@@ -99,82 +125,111 @@
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from .. import qs_default_console, qs_info_string
         from ..NetTools.NormalDL import size_format
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
+
         bucket = bucket if bucket else self.df_bucket
-        ls = self.client.list_objects(Bucket=bucket)['Contents']
-        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='Tencnet COS')
+        ls = self.client.list_objects(Bucket=bucket)["Contents"]
+        tb = qs_default_table(
+            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="Tencnet COS"
+        )
         for obj in ls:
-            tb.add_row(Text(obj['Key'], justify='left'), Text(size_format(int(obj['Size']), align=True), justify='right'))
-        qs_default_console.print(qs_info_string, 'Bucket Url:' if user_lang != 'zh' else '桶链接:',
-                                 self.cdn_url if bucket == self.df_bucket and self.cdn_url else
-                                 'https://' + bucket + '.cos.' + self.region + '.myqcloud.com/')
+            tb.add_row(
+                Text(obj["Key"], justify="left"),
+                Text(size_format(int(obj["Size"]), align=True), justify="right"),
+            )
+        qs_default_console.print(
+            qs_info_string,
+            "Bucket Url:" if user_lang != "zh" else "桶链接:",
+            self.cdn_url
+            if bucket == self.df_bucket and self.cdn_url
+            else "https://" + bucket + ".cos." + self.region + ".myqcloud.com/",
+        )
         qs_default_console.print(tb, justify="center")
 
 
 class Translate:
-    requirePackage('tencentcloud', real_name='tencentcloud-sdk-python')
-    detect = requirePackage('langdetect', 'detect')
-    DetectorFactory = requirePackage('langdetect', 'DetectorFactory')
-
-    from tencentcloud.common import credential
-    from tencentcloud.common.profile.client_profile import ClientProfile
-    from tencentcloud.common.profile.http_profile import HttpProfile
-    from tencentcloud.tmt.v20180321 import tmt_client, models
 
-    def __init__(self, scid: str = pre_check('txyun_scid'), sckey: str = pre_check('txyun_sckey'),
-                 region: str = pre_check('txyun_df_region')):
+    from tencentcloud.tmt.v20180321 import models
+
+    def __init__(self, scid, sckey, region):
         """
         初始化并登陆腾讯翻译接口
 
         Initialize and log in Tencent translation interface
 
         :param scid: secret id
         :param sckey: secret key
         :param region: 地区
         """
-        Translate.DetectorFactory.seed = 0
-        cred = Translate.credential.Credential(scid, sckey)
-        http_profile = Translate.HttpProfile()
+        if not (scid and sckey and region):
+            scid, sckey, region = pre_check(
+                "txyun_scid", "txyun_sckey", "txyun_df_region"
+            )
+        requirePackage("langdetect", "DetectorFactory").seed = 0
+        cred = requirePackage(
+            "tencentcloud.common", "credential", real_name="tencentcloud-sdk-python"
+        )
+        http_profile = requirePackage(
+            "tencentcloud.common.profile.http_profile",
+            "HttpProfile",
+            real_name="tencentcloud-sdk-python",
+        )()
         http_profile.endpoint = "tmt.tencentcloudapi.com"
-        clientProfile = Translate.ClientProfile()
+        clientProfile = requirePackage(
+            "tencentcloud.common.profile.client_profile",
+            "ClientProfile",
+            real_name="tencentcloud-sdk-python",
+        )()
         clientProfile.httpProfile = http_profile
-        self.client = Translate.tmt_client.TmtClient(cred, region, clientProfile)
+        self.client = requirePackage(
+            "tencentcloud.tmt.v20180321.tmt_client",
+            "TmtClient",
+            real_name="tencentcloud-sdk-python",
+        )(cred, region, clientProfile)
 
     @staticmethod
     def langdetect(text: str) -> str:
         """
         获取文本的语言类型
 
         Gets the language type of the text
 
         :param text: 待识别文本
         :return: 语言类型
         """
-        return Translate.detect(text)
+        return requirePackage("langid", "classify")(text)[0]
 
-    def translate(self, text: str, from_lang: str = None, to_lang: str = user_lang) -> str:
+    def translate(
+        self, text: str, from_lang: str = None, target_lang: str = user_lang
+    ) -> str:
         """
         翻译文本至默认语言
 
         Translate text to the default language
 
         :param from_lang: 文本语言
-        :param to_lang: 目标语言
+        :param target_lang: 目标语言
         :param text: 文本
         :return: 翻译结果
         """
-        req = Translate.models.TextTranslateRequest()
-        req.from_json_string(json.dumps({
-            "SourceText": text,
-            "Source": self.langdetect(text) if not from_lang else from_lang,
-            "Target": to_lang,
-            "ProjectId": 0
-        }))
-        return json.loads(self.client.TextTranslate(req).to_json_string())['TargetText']
+        req = requirePackage(
+            "tencentcloud.tmt.v20180321.models", "TextTranslateRequest"
+        )()
+        req.from_json_string(
+            json.dumps(
+                {
+                    "SourceText": text,
+                    "Source": self.langdetect(text) if not from_lang else from_lang,
+                    "Target": target_lang,
+                    "ProjectId": 0,
+                }
+            )
+        )
+        return json.loads(self.client.TextTranslate(req).to_json_string())["TargetText"]
 
 
-def translate(text: str, from_lang: str = None, to_lang: str = user_lang) -> str:
-    return Translate().translate(text, from_lang, to_lang)
+def translate(text: str, from_lang: str = None, target_lang: str = user_lang) -> str:
+    return Translate().translate(text, from_lang, target_lang)
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # coding=utf-8
 """
 修改图像颜色工具
 
 Modify image color tool
 """
-from PIL import Image
+from .. import requirePackage
 
+Image = requirePackage("PIL", "Image")
 
-def transport_back(src: str, to_color: tuple, from_color: tuple = (0, 0, 0, 0)) -> Image.Image:
+
+def transport_back(
+    src: str, to_color: tuple, from_color: tuple = (0, 0, 0, 0)
+) -> Image.Image:
     """
     图片颜色替换
 
     Image color replacement
 
     :param src: 图片路径
     :param to_color: RGBA四元组 -> 转换至目标颜色
     :param from_color: RGBA四元组 -> 需要被转换的颜色
     :return:
     """
     src = Image.open(src)
-    src = src.convert('RGBA')
+    src = src.convert("RGBA")
     L, H = src.size
     color_0 = from_color
     transparency_flag = False if color_0[-1] else True
     for h_indx in range(H):
         for l_indx in range(L):
             dot = (l_indx, h_indx)
             color_1 = src.getpixel(dot)
@@ -44,15 +48,15 @@
     :param to_color: RGBA四元组 -> 转换至目标颜色
     :param except_color: RGBA四元组 -> 忽略的颜色
     :return:
     """
     if except_color is None:
         except_color = [(0, 0, 0, 0)]
     src = Image.open(src)
-    src = src.convert('RGBA')
+    src = src.convert("RGBA")
     L, H = src.size
     for h_indx in range(H):
         for l_indx in range(L):
             color_1 = src.getpixel(dot := (l_indx, h_indx))
             if color_1 not in except_color:
                 src.putpixel(dot, to_color)
     return src
@@ -63,17 +67,22 @@
     解析字符串为RGBA四元组
 
     Parse strings for RGBA quaternions
 
     :param str_color: 表示颜色的字符串(支持16进制、RGB或RGBA) | String representing color (hex, RGB, or RGBA support)
     :return: RGBA四元组 | RGBA quad
     """
-    if ',' in str_color:
-        str_color = [int(i) for i in str_color.split(',')]
+    if "," in str_color:
+        str_color = [int(i) for i in str_color.split(",")]
         if len(str_color) == 3:
             str_color.append(255)
         str_color = tuple(str_color)
     elif len(str_color) == 6:
-        str_color = (int(str_color[:2], 16), int(str_color[2:4], 16), int(str_color[4:], 16), 255)
+        str_color = (
+            int(str_color[:2], 16),
+            int(str_color[2:4], 16),
+            int(str_color[4:], 16),
+            255,
+        )
     else:
-        exit('ERROR COLOR!')
+        exit("ERROR COLOR!")
     return str_color
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # coding=utf-8
 """
 视频处理库, 你需要额外安装moviepy库
 
 Video processing library, you need to install additional moviepy library
 """
 import os
-from .. import dir_char, user_lang, qs_default_console, qs_error_string, requirePackage
+from .. import user_lang, qs_default_console, qs_error_string, requirePackage
 
 
 def VideoWrapper(func):
     """
     视频处理的函数装饰器
 
     Video processing function decorator
 
     :param func: 函数
     :return: wrapper
     """
+
     def wrapper(path, *args, **kwargs):
         if not os.path.exists(path):
-            qs_default_console.log(qs_error_string, f'{"No such file" if user_lang != "zh" else "文件不存在"}: {path}')
+            qs_default_console.log(
+                qs_error_string,
+                f'{"No such file" if user_lang != "zh" else "文件不存在"}: {path}',
+            )
             return
         if not os.path.isfile(path):
-            qs_default_console.log(qs_error_string, f'{"No a file" if user_lang != "zh" else "不是文件"}: {path}')
-        mpy = requirePackage('moviepy', 'editor')
+            qs_default_console.log(
+                qs_error_string,
+                f'{"No a file" if user_lang != "zh" else "不是文件"}: {path}',
+            )
+        mpy = requirePackage("moviepy", "editor")
         func(path, *args, **kwargs, mpy=mpy)
 
     return wrapper
 
 
 @VideoWrapper
 def video_2_gif(path: str, size: tuple = (480, 320), fps: int = None, mpy=None):
@@ -38,75 +45,83 @@
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :param size: gif尺寸
     :param fps: fps
     :return: None
     """
-    file_name = '.'.join(os.path.basename(path).split('.')[:-1]) + '.gif'
-    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
+    file_name = ".".join(os.path.basename(path).split(".")[:-1]) + ".gif"
+    dir_name = os.path.abspath(os.path.dirname(path))
     ct = mpy.VideoFileClip(path) if not size else mpy.VideoFileClip(path).resize(size)
-    ct.write_gif(dir_name + file_name, fps=fps) if fps else ct.write_gif(dir_name + file_name)
+    ct.write_gif(os.path.join(dir_name, file_name), fps=fps)
 
 
 @VideoWrapper
 def rm_audio(path: str, mpy=None):
     """
     删除视频的音频
 
     Delete the audio of the video
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :return: None
     """
     file_name = os.path.basename(path)
-    if '.' in file_name:
-        indx = file_name.index('.')
-        file_name = file_name[:indx] + '_rm_audio' + file_name[indx:]
-        file_name = file_name.split('.')
-        file_name = '.'.join(file_name[:-1]) + '.mp4'
+    if "." in file_name:
+        indx = file_name.index(".")
+        file_name = file_name[:indx] + "_rm_audio" + file_name[indx:]
+        file_name = file_name.split(".")
+        file_name = ".".join(file_name[:-1]) + ".mp4"
     else:
-        file_name += '_rm_audio'
-    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
+        file_name += "_rm_audio"
+    dir_name = os.path.abspath(os.path.dirname(path))
     ct = mpy.VideoFileClip(path).set_audio(None)
-    ct.write_videofile(dir_name + file_name)
+    ct.write_videofile(os.path.join(dir_name, file_name))
 
 
 @VideoWrapper
 def tomp4(path: str, mpy=None):
     """
     将视频转为mp4
 
     Convert the video to MP4
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :return: None
     """
     file_name = os.path.basename(path)
-    file_name = '.'.join(file_name.split('.')[:-1]) + '.mp4' if '.' in file_name else file_name + '.mp4'
-    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
+    file_name = (
+        ".".join(file_name.split(".")[:-1]) + ".mp4"
+        if "." in file_name
+        else file_name + ".mp4"
+    )
+    dir_name = os.path.abspath(os.path.dirname(path))
     ct = mpy.VideoFileClip(path)
-    ct.write_videofile(dir_name + file_name, audio_codec='aac')
+    ct.write_videofile(os.path.join(dir_name, file_name))
 
 
 @VideoWrapper
 def video_2_mp3(path: str, mpy=None):
     """
     提取视频的音频并保存为mp3格式
 
     Extract the audio from the video and save it in MP3 format
 
     :return:
     """
     file_name = os.path.basename(path)
-    file_name = '.'.join(file_name[:-1].split('.')) + '.mp3' if '.' in file_name else file_name + '.mp3'
-    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
-    mpy.VideoFileClip(path).audio.write_audiofile(dir_name + file_name)
+    file_name = (
+        ".".join(file_name[:-1].split(".")) + ".mp3"
+        if "." in file_name
+        else file_name + ".mp3"
+    )
+    dir_name = os.path.abspath(os.path.dirname(path))
+    mpy.VideoFileClip(path).audio.write_audiofile(os.path.join(dir_name, file_name))
 
 
 @VideoWrapper
 def set_video_audio(v_path: str, a_path: str, mpy=None):
     """
     设置视频的音频
 
@@ -114,13 +129,17 @@
 
     :param v_path: 视频路径 | video path
     :param a_path: 音频路径 | audio path
     :param mpy: None, DO NOT SET IT
     :return:
     """
     file_name = os.path.basename(v_path)
-    file_name = '.'.join(file_name.split('.')[:-1]) + '_sta.mp4' if '.' in file_name else file_name + '_sta.mp4'
-    dir_name = dir_char.join(os.path.abspath(v_path).split(dir_char)[:-1]) + dir_char
+    file_name = (
+        ".".join(file_name.split(".")[:-1]) + "_sta.mp4"
+        if "." in file_name
+        else file_name + "_sta.mp4"
+    )
+    dir_name = os.path.abspath(os.path.dirname(v_path))
     v = mpy.VideoFileClip(v_path)
     a = mpy.AudioFileClip(a_path)
     v = v.set_audio(a)
-    v.write_videofile(dir_name + file_name, audio_codec='aac')
+    v.write_videofile(os.path.join(dir_name, file_name), audio_codec="aac")
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from socketserver import ThreadingMixIn
 from http.server import SimpleHTTPRequestHandler
 from http.server import HTTPServer
 from .. import qs_default_console, qs_info_string, requirePackage
 
 
 class HttpServers:
-    qrcode_terminal = requirePackage('qrcode_terminal')
+    qrcode_terminal = requirePackage("qrcode_terminal", real_name="qrcode-terminal")
     import signal
 
-    def __init__(self, ip='localhost', port=8000, url=''):
+    def __init__(self, ip="localhost", port=8000, url=""):
         """
         http服务类初始化
 
         HTTP service class initialization
 
         :param ip: 绑定的ip
         :param port: 端口
@@ -37,26 +37,29 @@
         开启http服务
 
         Start the HTTP service
 
         :return: None
         """
         HttpServers.signal.signal(HttpServers.signal.SIGINT, self.shutdown)
-        self.httpd = HttpServers.Server((self.web_address, self.web_port), SimpleHTTPRequestHandler)
+        self.httpd = HttpServers.Server(
+            (self.web_address, self.web_port), SimpleHTTPRequestHandler
+        )
         if not self.bind_url:
-            self.bind_url = 'http://' + self.web_address + ':' + str(self.web_port)
+            self.bind_url = "http://" + self.web_address + ":" + str(self.web_port)
         qs_default_console.print(qs_info_string, self.bind_url)  # * 展示待访问的url
         HttpServers.qrcode_terminal.draw(self.bind_url)  # * 为待访问的url绘制二维码
         try:
             self.httpd.serve_forever()
         except TypeError:
             self.shutdown()
 
     def shutdown(self):
         """
         Ctrl C
         :return: None
         """
         import os
+
         self.httpd.shutdown()
-        qs_default_console.print(qs_info_string, 'HTTP Server: Closed.')
+        qs_default_console.print(qs_info_string, "HTTP Server: Closed.")
         os._exit(0)
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,71 +5,76 @@
 The downloader of m3u8 file
 """
 import urllib3
 from concurrent.futures import ThreadPoolExecutor, wait
 import requests
 import os
 import queue
-from .. import dir_char, remove, headers, user_lang, qs_default_console, qs_error_string, qs_info_string
+from .. import (
+    remove,
+    user_lang,
+    qs_default_console,
+    qs_error_string,
+    qs_info_string,
+)
+from . import headers
+
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def merge_file(path, ts_ls, name):
     """
     将全部ts文件合并
 
     Merge all TS files
 
     :param path: 文件夹路径
     :param ts_ls: ts文件路径列表
     :param name: 合并后的ts文件名
     :return:
     """
-    if not path.endswith(dir_char):
-        path += dir_char
-    with open(name + '.ts', 'wb') as f:
+    with open(name + ".ts", "wb") as f:
         for ts in ts_ls:
-            with open(path + ts, 'rb') as ff:
+            with open(os.path.join(path, ts), "rb") as ff:
                 f.write(ff.read())
 
 
 class M3U8DL:
     from rich.progress import Progress, TimeRemainingColumn, TextColumn, BarColumn
 
     proxies = {}
 
-    def __init__(self, target, name, proxy: str = ''):
+    def __init__(self, target, name, proxy: str = ""):
         """
         初始化M3U8下载引擎
 
         Initialize the M3U8 download engine
 
         :param target: 目标url
         :param name: 文件名
         """
-        self.path = ''
+        self.path = ""
         self._cur = 0
         self._all = 0
         self.target = target
         self.name = name
         self.job_queue = queue.Queue()
         if proxy:
-            M3U8DL.proxies = {
-                'http': 'http://'+proxy,
-                'https': 'https://'+proxy
-            }
+            M3U8DL.proxies = {"http": "http://" + proxy, "https": "https://" + proxy}
         self.main_progress = M3U8DL.Progress(
             M3U8DL.TextColumn("[bold blue]{task.fields[taskName]}", justify="right"),
             M3U8DL.BarColumn(bar_width=None),
             "[progress.percentage]{task.percentage:>3.1f}%",
             "•",
             M3U8DL.TimeRemainingColumn(),
-            console=qs_default_console
+            console=qs_default_console,
+        )
+        self.dl_id = self.main_progress.add_task(
+            "Download", taskName="Downloading" if user_lang != "zh" else "下载中"
         )
-        self.dl_id = self.main_progress.add_task("Download", taskName='Downloading' if user_lang != 'zh' else '下载中')
 
     def _dl_one(self, job):
         """
         下载一个ts文件
 
         Download a TS file
 
@@ -78,54 +83,64 @@
         """
         try:
             if job[-1]:
                 pd_url = job[0]
                 c_fule_name = job[1]
                 if not os.path.exists(os.path.join(self.path, c_fule_name)):
                     res = requests.get(pd_url, verify=False, proxies=M3U8DL.proxies)
-                    with open(os.path.join(self.path, c_fule_name), 'ab') as f:
+                    with open(os.path.join(self.path, c_fule_name), "ab") as f:
                         f.write(res.content)
                         f.flush()
             self.main_progress.advance(self.dl_id, 1)
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
             self.job_queue.put(job)
 
     def download(self):
         """
         下载
 
         :return: None
         """
         target = self.target
-        download_path = os.getcwd() + dir_char + self.name
+        download_path = os.path.join(os.getcwd(), self.name)
         self.path = download_path
         if not os.path.exists(download_path):
             os.mkdir(download_path)
         try:
-            all_content = requests.get(target, verify=False, headers=headers, proxies=M3U8DL.proxies).text
+            all_content = requests.get(
+                target, verify=False, headers=headers, proxies=M3U8DL.proxies
+            ).text
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
             return
         if "#EXTM3U" not in all_content:
-            raise Exception("Not M3U8 Link" if user_lang != 'zh' else "非M3U8的链接")
+            raise Exception("Not M3U8 Link" if user_lang != "zh" else "非M3U8的链接")
         if "EXT-X-STREAM-INF" in all_content:
             file_line = all_content.split("\n")
             for line in file_line:
-                if '.m3u8' in line:
+                if ".m3u8" in line:
                     target = target.rsplit("/", 1)[0] + "/" + line
-                    all_content = requests.get(target, verify=False, headers=headers, proxies=M3U8DL.proxies).text
+                    all_content = requests.get(
+                        target, verify=False, headers=headers, proxies=M3U8DL.proxies
+                    ).text
         file_line = all_content.split("\n")
         _rt = target.rsplit("/", 1)[0] + "/"
         tmp = []
         for index, line in enumerate(file_line):
             if "#EXT-X-KEY" in line:
                 tmp.append((_rt, line, 0))
             if "EXTINF" in line:
-                tmp.append((_rt + file_line[index + 1], file_line[index + 1].rsplit("/", 1)[-1], 1))
+                tmp.append(
+                    (
+                        _rt + file_line[index + 1],
+                        file_line[index + 1].rsplit("/", 1)[-1],
+                        1,
+                    )
+                )
         file_line = tmp[::-1]
         self._all = len(file_line)
         tmp = [jb[1] for jb in file_line]
 
         self.main_progress.update(self.dl_id, total=len(file_line))
         for i in file_line:
             self.job_queue.put(i)
@@ -135,11 +150,15 @@
         while not self.job_queue.empty():
             cur_work = []
             while not self.job_queue.empty():
                 cur_work.append(pool.submit(self._dl_one, self.job_queue.get()))
             wait(cur_work)
         self.main_progress.stop()
 
-        qs_default_console.print(qs_info_string, "Download completed! Start merge.."
-                                 if user_lang != 'zh' else '下载完成! 开始合并..')
+        qs_default_console.print(
+            qs_info_string,
+            "Download completed! Start merge.."
+            if user_lang != "zh"
+            else "下载完成! 开始合并..",
+        )
         merge_file(download_path, tmp, self.name)
         remove(download_path)
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 qs的普通文件下载器！干翻迅雷，并且支持设置代理，设置referer，好看的命令行交互，啥j8文件都能下；(仅支持http[s]协议)
 
 QS ordinary file downloader! Dry out Thunder, and support to set the proxy, set the Referer,
 good-looking command line interaction, and it can download fuck any files; (only supports HTTP[S])
 
 Author: RhythmLian (https://rhythmlian.cn)
 """
-from . import size_format, get_fileinfo
+from . import size_format, get_fileinfo, headers
 from concurrent.futures import ThreadPoolExecutor, wait
-from ..ThreadTools import FileWriters
 from ..SystemTools import get_core_num
-from .. import user_lang, qs_default_console, qs_error_string, qs_info_string, qs_warning_string, headers
+from .. import (
+    user_lang,
+    qs_default_console,
+    qs_default_status,
+    qs_error_string,
+    qs_info_string,
+    qs_warning_string,
+    requirePackage,
+)
 from threading import Lock
 from requests import get
 import signal
 import queue
 import time
 import sys
 import os
@@ -39,176 +46,256 @@
     elif sz <= minBlockSize << 3:
         return minBlockSize
     else:
         return max(sz >> 9, minBlockSize)
 
 
 def ask_overwrite(path: str):
-    from PyInquirer import prompt
+    from .. import _ask
 
-    return prompt({
-        'type': 'confirm',
-        'name': 'overwrite',
-        'message': f'"{path}" 已存在, 是否覆盖?' if user_lang == 'zh' else f'"{path}" already exists, overwrite?',
-        'default': False
-    })['overwrite']
+    return _ask(
+        {
+            "type": "confirm",
+            "message": f'"{path}" 已存在, 是否覆盖?'
+            if user_lang == "zh"
+            else f'"{path}" already exists, overwrite?',
+            "default": False,
+        }
+    )
 
 
 class Downloader:
     from ..TuiTools.Bar import DataTransformBar
 
-    def __init__(self, url: str, num: int, name: str = '', proxy: str = '',
-                 referer: str = '', output_error: bool = False, failed2exit: bool = False, exit_if_exist: bool = False,
-                 disableStatus: bool = False, disableParallel: bool = False):
+    def __init__(
+        self,
+        url: str,
+        num: int,
+        name: str = "",
+        proxy: str = "",
+        referer: str = "",
+        output_error: bool = False,
+        failed2exit: bool = False,
+        exit_if_exist: bool = False,
+        disableStatus: bool = False,
+        disableParallel: bool = False,
+        write_to_memory: bool = False,
+        ignore_404: bool = False,
+    ):
         """
         qs普通文件下载引擎
 
         Qs general file download engine
 
         :param url: 文件url
         :param num: 线程数量
+        :param name: 文件名
+        :param proxy: 代理
+        :param referer: referer
+        :param output_error: 是否输出错误
+        :param failed2exit: 是否下载失败就退出
+        :param exit_if_exist: 如果文件已存在，是否退出
+        :param disableStatus: 是否禁用状态栏
+        :param disableParallel: 是否禁用并行下载
+        :param write_to_memory: 是否写入内存
+        :param ignore_404: 是否忽略404错误
         """
         signal.signal(signal.SIGINT, self._kill_self)
         info_flag = True
         self.url, self.num, self.output_error, self.proxies = url, num, output_error, {}
         self.exit_if_exist = exit_if_exist
         self.enabled = True
-        if not disableStatus:
-            with qs_default_console.status('Getting file info..' if user_lang != 'zh' else '获取文件信息中..'):
+        self.disableStatus = disableStatus
+        self.write_to_memory = write_to_memory
+        if not self.disableStatus:
+            with qs_default_status(
+                "Getting file info.." if user_lang != "zh" else "获取文件信息中.."
+            ):
                 self.url, self.name, r = get_fileinfo(url, proxy, referer)
         else:
             self.url, self.name, r = get_fileinfo(url, proxy, referer)
         if not (self.url and self.name and r):
             info_flag = False
-            qs_default_console.print(qs_error_string if failed2exit else qs_warning_string,
-                                     'Get File information failed, please check network!'
-                                     if user_lang != 'zh' else '获取文件信息失败，请检查网络!')
-            if failed2exit:
+            if not self.disableStatus:
+                qs_default_console.print(
+                    qs_error_string if failed2exit else qs_warning_string,
+                    "Get File information failed, please check network!"
+                    if user_lang != "zh"
+                    else "获取文件信息失败，请检查网络!",
+                )
+            if failed2exit and not ignore_404:
                 self.enabled = False
                 return
-        if self.name and '.' not in self.name:
+        if not self.url:
+            qs_default_console.print(
+                qs_error_string,
+                "Connection Error!" if user_lang != "zh" else "连接失败!",
+                self.name,
+            )
+            self.enabled = False
+            return
+
+        if self.name and "." not in self.name:
             self.name = os.path.basename(url)
         if name:
             self.name = name
 
         if os.path.exists(self.name) and self.exit_if_exist:
             self.enabled = False
             return
 
         if proxy:
-            self.proxies = {
-                'http': 'http://'+proxy,
-                'https': 'https://'+proxy
-            }
+            self.proxies = {"http": "http://" + proxy, "https": "https://" + proxy}
         self.headers = headers
         if referer:
-            self.headers['Referer'] = referer
-        if not self.url:
-            qs_default_console.print(qs_error_string, self.name)
-            raise Exception('Connection Error!' if user_lang != 'zh' else '连接失败!')
+            self.headers["Referer"] = referer
         try:
             if not info_flag:
                 raise KeyError
-            self.size = int(r.headers['content-length'])
+            self.size = int(r.headers["content-length"])
             self.main_progress = Downloader.DataTransformBar()
-            self.dl_id = self.main_progress.add_task('Download', filename=self.name, start=False)
+            self.dl_id = self.main_progress.add_task(
+                "Download", filename=self.name, start=False
+            )
             self.main_progress.update(self.dl_id, total=self.size)
             if self.size < 5e6 or disableParallel:
-                qs_default_console.print(qs_info_string, 'FILE SIZE' if user_lang != 'zh' else '文件大小'
-                                         , size_format(self.size))
+                if not self.disableStatus:
+                    qs_default_console.print(
+                        qs_info_string,
+                        "FILE SIZE" if user_lang != "zh" else "文件大小",
+                        size_format(self.size),
+                    )
                 self.size = -self.size
             else:
                 self.fileBlock = GetBlockSize(self.size)
         except KeyError:
             self.size = -1
             self.main_progress = Downloader.DataTransformBar(False)
-            self.dl_id = self.main_progress.add_task('Download', filename=self.name, start=False)
+            self.dl_id = self.main_progress.add_task(
+                "Download", filename=self.name, start=False
+            )
         if self.size > 0:
             self.pool = ThreadPoolExecutor(max_workers=self.num)
             self.futures, self.fileLock = [], Lock()
             self.job_queue = queue.Queue()
-            if os.path.exists(self.name + '.qs_dl'):
-                self.ctn_file = open(self.name + '.qs_dl', 'r+')
-                self.ctn = [int(i) for i in self.ctn_file.read().strip().split()]
+            if os.path.exists(self.name + ".qs_dl"):
+                qs_default_console.print(
+                    qs_info_string,
+                    "Resuming task from:" if user_lang != "zh" else "从文件恢复任务:",
+                    self.name + ".qs_dl",
+                )
+                self.ctn_file = open(self.name + ".qs_dl", "r+")
+                self.ctn = {int(i) for i in self.ctn_file.read().strip().split()}
+            elif not self.write_to_memory:
+                self.ctn_file = open(self.name + ".qs_dl", "w")
+                self.ctn = set()
             else:
-                self.ctn_file = open(self.name + '.qs_dl', 'w')
-                self.ctn = []
-            self.writers = FileWriters(self.name, max(2, int(core_num / 2)), "rb+" if self.ctn else "wb")
-            qs_default_console.print(qs_info_string, 'FILE  SIZE' if user_lang != 'zh' else '文件大小'
-                                     , size_format(self.size, align=True))
-            qs_default_console.print(qs_info_string, 'THRAED NUM' if user_lang != 'zh' else '线程数量'
-                                     , '%7d' % num)
+                self.ctn = set()
+            self.writers = (
+                requirePackage(".ThreadTools", "FileWriters")(
+                    self.name, max(2, int(core_num / 2)), "rb+" if self.ctn else "wb"
+                )
+                if not self.write_to_memory
+                else requirePackage(".ThreadTools", "MemWriter")()
+            )
+            if not self.disableStatus:
+                qs_default_console.print(
+                    qs_info_string,
+                    "FILE  SIZE" if user_lang != "zh" else "文件大小",
+                    size_format(self.size, align=True),
+                )
+                qs_default_console.print(
+                    qs_info_string,
+                    "THRAED NUM" if user_lang != "zh" else "线程数量",
+                    "%7d" % num,
+                )
 
     def _kill_self(self, signum, frame):
         """
         终止下载任务，保存断点
 
         Terminate the download and save the breakpoint
 
         :param signum: 信号
         :param frame: frame
         :return: None
         """
         if self.size > 0:
             self.main_progress.stop_task(self.dl_id)
             self.main_progress.stop()
-            qs_default_console.print(qs_info_string,
-                                     'Get Ctrl-C, exiting...' if user_lang != 'zh' else '捕获Ctrl-C, 正在退出...')
-            self.ctn_file.close()
+            qs_default_console.print(
+                qs_info_string,
+                "Get Ctrl-C, exiting..." if user_lang != "zh" else "捕获Ctrl-C, 正在退出...",
+            )
+            if not self.write_to_memory:
+                self.ctn_file.close()
             self.pool.shutdown(wait=False)
             self.writers.wait()
-            qs_default_console.print(qs_info_string, 'Deal Done!' if user_lang != 'zh' else '处理完成!')
+            qs_default_console.print(
+                qs_info_string, "Deal Done!" if user_lang != "zh" else "处理完成!"
+            )
         os._exit(0)
 
     def _dl(self, start):
         """
         执行文件块下载任务
 
         Perform the file block download task
 
         :param start: 文件块起始偏移量
         :return: None
         """
         try:
             _sz = min(start + self.fileBlock, self.size - 1)
             _headers = self.headers.copy()
-            _headers['Range'] = 'bytes={}-{}'.format(start, _sz)
-            _content = b''
-            for chunk in get(self.url, headers=_headers, timeout=50, proxies=self.proxies).iter_content(65536):
+            _headers["Range"] = "bytes={}-{}".format(start, _sz)
+            _content = b""
+            for chunk in get(
+                self.url, headers=_headers, timeout=50, proxies=self.proxies
+            ).iter_content(65536):
                 _content += chunk
-                self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
+                if not self.disableStatus:
+                    self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
             self.writers.new_job(_content, start)
         except Exception as e:
             if self.output_error:
                 qs_default_console.print(qs_error_string, repr(e))
             self.job_queue.put(start)
         else:
-            self.fileLock.acquire()
-            self.ctn.append(start)
-            self.ctn_file.write('%d\n' % start)
-            self.fileLock.release()
+            self.ctn.add(start)
+            if not self.write_to_memory:
+                self.fileLock.acquire()
+                self.ctn_file.write("%d\n" % start)
+                self.fileLock.release()
 
     def _single_dl(self):
         """
         无法并行下载或无需并行下载时采用串行下载
 
         Parallel downloads are not possible or serial downloads are not required
 
         :return: None
         """
         r = get(self.url, stream=True, proxies=self.proxies, headers=self.headers)
         flag = self.size != -1
 
-        if flag:
-            self.main_progress.start_task(self.dl_id)
+        if not self.disableStatus:
+            if flag:
+                self.main_progress.start_task(self.dl_id)
+            else:
+                self.main_progress.update(self.dl_id, total=-1)
+        if self.write_to_memory == False:
+            with open(self.name, "wb") as f:
+                for chunk in r.iter_content(32768):
+                    f.write(chunk)
+                    self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
         else:
-            self.main_progress.update(self.dl_id, total=-1)
-        with open(self.name, 'wb') as f:
+            self.name = b""
             for chunk in r.iter_content(32768):
-                f.write(chunk)
+                self.name += chunk
                 self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
 
     def run(self):
         """
         规划下载任务并开始下载
 
         qs可以有效应对网络问题对下载任务造成的影响，如：
@@ -216,69 +303,114 @@
 
           2.链路异常
         并确保下载任务顺利完成
 
         :return: None
         """
         if not self.enabled:
-            return self.name if self.exit_if_exist else ''
-        self.main_progress.start()
+            return self.name if self.exit_if_exist else None
+        if not self.disableStatus:
+            self.main_progress.start()
         if self.size > 0:
-            self.main_progress.start_task(self.dl_id)
-            if not self.ctn:
-                with open(self.name, "wb") as fp:
-                    fp.truncate(self.size)
-            self.main_progress.advance(self.dl_id, self.fileBlock*len(self.ctn))
-            for i in range(0, self.size, self.fileBlock):
-                if self.ctn and i in self.ctn:
-                    continue
-                else:
+            if not self.disableStatus:
+                self.main_progress.start_task(self.dl_id)
+            if not self.write_to_memory:
+                if not self.ctn:
+                    with open(self.name, "wb") as fp:
+                        fp.truncate(self.size)
+                if not self.disableStatus:
+                    self.main_progress.advance(
+                        self.dl_id, self.fileBlock * len(self.ctn)
+                    )
+                for i in range(0, self.size, self.fileBlock):
+                    if self.ctn and i in self.ctn:
+                        continue
+                    else:
+                        self.job_queue.put(i)
+            else:
+                for i in range(0, self.size, self.fileBlock):
                     self.job_queue.put(i)
             retry_cnt = 0
             while not self.job_queue.empty():
                 self.futures.clear()
                 while not self.job_queue.empty():
                     cur = self.job_queue.get()
                     if cur not in self.ctn:
                         self.futures.append(self.pool.submit(self._dl, cur))
                 wait(self.futures)
                 if not self.job_queue.empty() and retry_cnt > 2:
-                    qs_default_console.print(qs_warning_string, 'Exists File Block Lost, Retrying after 0.5 sec'
-                                             if user_lang != 'zh' else '存在文件块丢失，0.5秒后重试')
+                    qs_default_console.print(
+                        qs_warning_string,
+                        "Exists File Block Lost, Retrying after 0.5 sec"
+                        if user_lang != "zh"
+                        else "存在文件块丢失，0.5秒后重试",
+                    )
                     time.sleep(0.5)
                 retry_cnt += 1
             self.writers.wait()
-            self.ctn_file.close()
-            os.remove(self.name + '.qs_dl')
+            if not self.write_to_memory:
+                self.ctn_file.close()
+                os.remove(self.name + ".qs_dl")
+            else:
+                self.name = self.writers.content
         else:
             self._single_dl()
-        self.main_progress.stop()
-        qs_default_console.print(qs_info_string, self.name, 'download done!' if user_lang != 'zh' else '下载完成!')
+        if not self.disableStatus:
+            self.main_progress.stop()
+            qs_default_console.print(
+                qs_info_string,
+                self.name,
+                "download done!" if user_lang != "zh" else "下载完成!",
+            )
         return self.name
 
 
-def normal_dl(url, set_name: str = '', set_proxy: str = '', set_referer: str = '',
-              thread_num: int = min(16, core_num * 4), output_error: bool = False, failed2exit: bool = False, exit_if_exist: bool = False,
-              disableStatus: bool = False, disableParallel: bool = False):
+def normal_dl(
+    url,
+    set_name: str = "",
+    set_proxy: str = "",
+    set_referer: str = "",
+    thread_num: int = min(16, core_num * 4),
+    output_error: bool = False,
+    failed2exit: bool = False,
+    exit_if_exist: bool = False,
+    disableStatus: bool = False,
+    disableParallel: bool = False,
+    write_to_memory: bool = False,
+    ignore_404: bool = False,
+):
     """
     自动规划下载线程数量并开始并行下载
 
     Automatically schedule the number of download threads and begin parallel downloads
 
     :param disableStatus:
     :param url: 文件url
-    :param set_name: 设置文件名（默认采用url所指向的资源名）
+    :param set_name: 设置文件路径
     :param set_proxy: 设置代理（默认无代理）
     :param set_referer: 设置referer
     :param thread_num: 线程数
     :param output_error: 输出报错信息
-    :param failed2exit: 获取文件信息失败则不下载，否则qs将继续尝试下载
+    :param failed2exit: 获取文件信息失败则不下载, 否则qs将继续尝试下载
+    :param exit_if_exist: 如果文件已存在则不下载
     :param disableStatus: 是否显示当前任务状态
-    :return: file name
+    :param disableParallel: 是否禁用并行下载
+    :param write_to_memory: 是否将下载内容直接写入内存（默认写入文件）
+    :param ignore_404: 忽略404错误, 因无法获取文件信息，所以需自行设置文件名
+    :return: 文件路径或二进制内容 | file path or bytes
     """
     if set_name and os.path.exists(set_name) and not ask_overwrite(set_name):
-        return ''
+        return ""
     return Downloader(
-        url=url, num=thread_num, name=set_name, proxy=set_proxy,
-        referer=set_referer, output_error=output_error, failed2exit=failed2exit, exit_if_exist=exit_if_exist,
-        disableStatus=disableStatus, disableParallel=disableParallel
+        url=url,
+        num=thread_num,
+        name=set_name,
+        proxy=set_proxy,
+        referer=set_referer,
+        output_error=output_error,
+        failed2exit=failed2exit,
+        exit_if_exist=exit_if_exist,
+        disableStatus=disableStatus,
+        disableParallel=disableParallel,
+        write_to_memory=write_to_memory,
+        ignore_404=ignore_404,
     ).run()
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 qs的WIFI模块, 协助连接WIFI, 但不支持机构WIFI自动登录
 
 The WiFi module of QS helps to connect WiFi, but does not support the automatic login of institutional WiFi
 """
 import time
 from .. import user_lang, qs_default_console, qs_error_string, requirePackage
 
-const = requirePackage('pywifi', 'const')
-PyWiFi = requirePackage('pywifi', 'PyWiFi')
+const = requirePackage("pywifi", "const")
+PyWiFi = requirePackage("pywifi", "PyWiFi")
 
 
 class WiFi:
     def __init__(self) -> None:
         """
         qs的wifi工具 (Windows 或 Linux)
         """
@@ -25,15 +25,15 @@
         判断当前wifi连接状态
 
         Determine the current wifi connection status
 
         :return: 连接的wifi名 | The name of the connecting wifi
         """
         flag = self.iface.status() in [const.IFACE_CONNECTED, const.IFACE_CONNECTING]
-        return self.iface.name if flag else ''
+        return self.iface.name if flag else ""
 
     def scan(self):
         """
         扫描附近可连接的wifi
 
         Scan for nearby wifi connections
 
@@ -55,47 +55,57 @@
         Set Network port
 
         :return: None
         """
         num = len(self.ifaces)
         if num <= 0:
             qs_default_console.log(
-                qs_error_string, "There is no recognizable network card interface"
-                if user_lang != 'zh' else '没有可识别的网卡接口')
+                qs_error_string,
+                "There is no recognizable network card interface"
+                if user_lang != "zh"
+                else "没有可识别的网卡接口",
+            )
             return
         elif num != 1:
             from ..TuiTools.Table import qs_default_table
-            table = qs_default_table(['id', 'interface'] if user_lang != 'zh' else ['序号', '网卡'])
+
+            table = qs_default_table(
+                ["id", "interface"] if user_lang != "zh" else ["序号", "网卡"]
+            )
             for i, w in enumerate(self.ifaces):
                 table.add_row(str(i), w.name())
             qs_default_console.print(table)
             while True:
-                iface_no = input('请选择网卡接口序号: ' if user_lang != 'zh' else 'Select interface by id: ')
+                iface_no = input(
+                    "请选择网卡接口序号: " if user_lang != "zh" else "Select interface by id: "
+                )
                 try:
                     no = int(iface_no)
                     if 0 <= no < num:
                         self.iface = self.ifaces[no]
                         break
                 except:
                     continue
         else:
-            qs_default_console.print(f"{'Only one' if user_lang != 'zh' else '仅有可用'}: {self.iface.name()}")
+            qs_default_console.print(
+                f"{'Only one' if user_lang != 'zh' else '仅有可用'}: {self.iface.name()}"
+            )
 
     def conn(self, ssid, password):
         """
         连接WiFi
 
         connect WiFi
 
         :param ssid: wifi名称
         :param password: 密码
         :return: status
         """
         # from pywifi import Profile
-        Profile = requirePackage('pywifi', 'Profile')
+        Profile = requirePackage("pywifi", "Profile")
         self.iface.disconnect()
         time.sleep(1)
         pinfo = Profile()
         pinfo.ssid = ssid
         pinfo.auth = const.AUTH_ALG_OPEN
         pinfo.akm.append(const.AKM_TYPE_WPA2PSK)
         pinfo.cipher = const.CIPHER_TYPE_CCMP
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,67 +12,70 @@
 class WiFi:
     def __init__(self) -> None:
         """
         适用于Mac OS X的wifi工具
 
         Wifi tools for Mac OS X
         """
-        with os.popen('networksetup -listallhardwareports') as pipe:
+        with os.popen("networksetup -listallhardwareports") as pipe:
             ifaces = pipe.read()
-        ifaces = [i.split('\n') for i in ifaces.strip().split('\n\n')]
-        ifaces.remove(['VLAN Configurations', '==================='])
+        ifaces = [i.split("\n") for i in ifaces.strip().split("\n\n")]
+        ifaces.remove(["VLAN Configurations", "==================="])
         self.ifaces = ifaces
         for i in self.ifaces:
-            if i[0].endswith('Wi-Fi'):
+            if i[0].endswith("Wi-Fi"):
                 self.iface = [j.split()[-1] for j in i[1:]]
                 return
 
     def status(self) -> str:
         """
         判断当前wifi连接状态
 
         Determine the current wifi connection status
 
         :return: 连接的wifi名 | The name of the connecting wifi
         """
-        with os.popen('networksetup -getairportnetwork %s' % self.iface[0]) as pipe:
+        with os.popen("networksetup -getairportnetwork %s" % self.iface[0]) as pipe:
             res = pipe.read().strip()
-            res = re.sub('.*?:', '', res).strip()
-        qs_default_console.print(qs_info_string, f"{'已' if res else '未'}连接", res if res else '')
+            res = re.sub(".*?:", "", res).strip()
+        qs_default_console.print(
+            qs_info_string, f"{'已' if res else '未'}连接", res if res else ""
+        )
         return res
 
     @staticmethod
     def scan():
         """
         扫描附近可连接的wifi
 
         Scan for nearby wifi connections
 
         :return: 按信号强度排序好的可连接wifi列表 | A list of available wifi connections sorted by signal strength
         """
-        from . import is_mac
         with os.popen(
-                '/System/Library/PrivateFrameworks/Apple80211.framework/Versions/A/Resources/airport scan') as pipe:
-            res = pipe.read().strip().split('\n')[1:]
+            "/System/Library/PrivateFrameworks/Apple80211.framework/Versions/A/Resources/airport scan"
+        ) as pipe:
+            res = pipe.read().strip().split("\n")[1:]
             tmp_ls = [i.strip().split() for i in res]
             has_add = set()
             res = []
             for i in tmp_ls:
-                mac_index = 0
-                while mac_index < len(i):
-                    if is_mac(i[mac_index]):
-                        break
-                    else:
-                        mac_index += 1
-                if mac_index >= len(i):
-                    qs_default_console.log(qs_warning_string, "Failed to get info with:", i)
-                    continue
-                ssid = ' '.join(i[:mac_index])
-                if i[0] not in has_add:
-                    res.append([ssid, int(i[mac_index+1]), i[-1]])
+                # mac_index = 0
+                # while mac_index < len(i):
+                #     if is_mac(i[mac_index]):
+                #         break
+                #     else:
+                #         mac_index += 1
+                # if mac_index >= len(i):
+                #     qs_default_console.log(qs_warning_string, "Failed to get info with:", i)
+                #     continue
+                index = i.index("--") - 3
+                ssid = " ".join(i[:index])
+                if ssid not in has_add:
+                    res.append([ssid, int(i[index]), i[-1]])
                     has_add.add(ssid)
         return sorted(res, key=lambda x: x[1], reverse=True)
 
     def set_iface(self):
         raise NotImplementedError
 
     def conn(self, ssid: list, password: str):
@@ -81,12 +84,17 @@
 
         connect WiFi
 
         :param ssid: wifi名称
         :param password: 密码
         :return: status
         """
-        os.system('networksetup -setairportnetwork %s %s "%s"' % (self.iface[0], ssid[0], password))
+        from .. import external_exec
+
+        external_exec(
+            'networksetup -setairportnetwork %s %s "%s"'
+            % (self.iface[0], ssid[0], password)
+        )
         return self.status()
 
     def disconn(self):
         return NotImplementedError
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/NetTools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 qs的网络工具库
 
 The network tool library of QS
 """
 import socket
 import requests
 from requests.exceptions import RequestException
+from typing import Tuple
 
 
 headers = {
-    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/604.4.7 (KHTML, like Gecko) '
-                  'Version/11.0.2 Safari/604.4.7'}
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/604.4.7 (KHTML, like Gecko) "
+    "Version/11.0.2 Safari/604.4.7"
+}
 
 
 def is_ipv4(ip: str) -> bool:
     """
     判断ip是否为可连接的ipv4
 
     Determine whether the IP is a connectable IPv4
@@ -25,15 +27,15 @@
     try:
         socket.inet_pton(socket.AF_INET, ip)
     except AttributeError:  # no inet_pton here, sorry
         try:
             socket.inet_aton(ip)
         except socket.error:
             return False
-        return ip.count('.') == 3
+        return ip.count(".") == 3
     except socket.error:  # not a valid ip
         return False
     return True
 
 
 def is_ipv6(ip: str) -> bool:
     """
@@ -54,36 +56,36 @@
     """
     判断ip是否为可连接的
 
     Determine whether the IP is a connectable
     :param ip: like fe80::1862:5a79:a8a0:aae5, 8.8.8.8 etc.
     :return: bool
     """
-    if ip == 'localhost':
+    if ip == "localhost":
         return True
     return is_ipv4(ip) or is_ipv6(ip)
 
 
 def is_mac(addr: str) -> bool:
     """
     检查addr是否为mac地址
 
     Check whether addr is a mac address
 
     :param addr: string like '80:8f:1d:e2:f2:f5'
     :return: bool
     """
-    part = addr.split(':')
+    part = addr.split(":")
     if len(part) != 6:
         return False
     for i in part:
         if len(i) != 2:
             return False
         for j in i:
-            if j not in '0123456789abcdefABCDEF':
+            if j not in "0123456789abcdefABCDEF":
                 return False
     return True
 
 
 def check_one_page(url: str) -> bool:
     """
     检查url是否可访问
@@ -105,50 +107,52 @@
     为url添加https或http使其能被访问
 
     Add HTTPS or HTTP to the URL to make it accessible
 
     :param try_url: 待尝试的url
     :return: 能被成功访问的url
     """
-    if try_url.startswith('http://') or try_url.startswith('https://'):
+    if try_url.startswith("http://") or try_url.startswith("https://"):
         return try_url
     res_url = try_url
     if not check_one_page(res_url):
-        res_url = 'https://' + try_url
+        res_url = "https://" + try_url
         if not check_one_page(res_url):
-            res_url = 'http://' + try_url
+            res_url = "http://" + try_url
     return res_url
 
 
 def open_url(url: str):
     """
     使用默认浏览器打开url
 
     Open url using the default browser
 
     :param url:
     :return:
     """
     import webbrowser as wb
+
     url = formatUrl(url)
     wb.open_new_tab(url)
 
 
 def get_ip() -> str:
     """
     获取本机ip
 
     Get native IP
 
     :return: ip
     """
     import socket
+
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
-        s.connect(('8.8.8.8', 80))
+        s.connect(("8.8.8.8", 80))
         ip = s.getsockname()[0]
         return ip
     except Exception:
         s.close()
         return socket.gethostbyname(socket.gethostname())
 
 
@@ -159,69 +163,80 @@
     Format file size display
 
     :param sz: 整数，表示文件大小
     :param align: 是否对齐
     :return: 文件大小字符串
     """
     if sz >= 1e9:
-        return '%.3f GB' % (sz / 1e9) if not align else '%7.3f GB' % (sz / 1e9)
+        return (
+            "%.3f GB" % (sz / 1024**3) if not align else "%7.3f GB" % (sz / 1024**3)
+        )
     elif sz >= 1e6:
-        return '%.3f MB' % (sz / 1e6) if not align else '%7.3f MB' % (sz / 1e6)
+        return (
+            "%.3f MB" % (sz / 1024**2) if not align else "%7.3f MB" % (sz / 1024**2)
+        )
     elif sz >= 1e3:
-        return '%.3f KB' % (sz / 1e3) if not align else '%7.3f KB' % (sz / 1e3)
+        return "%.3f KB" % (sz / 1024) if not align else "%7.3f KB" % (sz / 1024)
     else:
-        return '%.2f B' % sz if not align else '%7.2f B' % sz
+        return "%.2f B" % sz if not align else "%7.2f B" % sz
 
 
 def get_ip_info() -> dict:
     """
     通过ip-api获取本机ip信息
 
     Get native IP information through IP-API
 
     :return: ip信息的dict，失败返回None
     """
     import json
-    res = requests.get('http://ip-api.com/json/', headers=headers)
+
+    res = requests.get("http://ip-api.com/json/", headers=headers)
     if res.status_code == requests.codes.ok:
         return json.loads(res.text)
     else:
         return {}
 
 
-def get_fileinfo(url: str, proxy: str = '', referer: str = '') -> (str, str, requests.Response):
+def get_fileinfo(
+    url: str, proxy: str = "", referer: str = ""
+) -> Tuple[str, str, requests.Response]:
     """
     获取待下载的文件信息
 
     Gets information about the file to be downloaded
 
     :param url: 文件url
     :param proxy: 代理
     :param referer: 绕反爬
     :return: 真实url，文件名，http头部信息 (headers中键值均为小写)
     """
     import re
     import os
-    proxies = {
-        'http': 'http://'+proxy,
-        'https': 'https://'+proxy
-    } if proxy else {}
+
+    proxies = {"http": "http://" + proxy, "https": "https://" + proxy} if proxy else {}
     if referer:
-        headers['referer'] = referer
+        headers["referer"] = referer
     try:
         res = requests.head(url, headers=headers, proxies=proxies)
+        if res.status_code == 404:
+            return url, "", res  # 某些网站会返回404，但是文件还是可以下载的
     except Exception as e:
-        return '', repr(e), None
+        return "", repr(e), None
     while res.status_code in [301, 302]:
-        url = {i[0]: i[1] for i in res.headers.lower_items()}['location']
+        url = {i[0]: i[1] for i in res.headers.lower_items()}["location"]
         res = requests.head(url, headers=headers, proxies=proxies)
     res.headers = {i[0]: i[1] for i in res.headers.lower_items()}
-    if 'content-disposition' in res.headers:
+    if "content-disposition" in res.headers:
         try:
-            filename = re.findall('filename=(.*?);', res.headers['content-disposition'])[0]
+            filename = re.findall(
+                "filename=(.*?);", res.headers["content-disposition"]
+            )[0]
         except IndexError:
             from urllib.parse import urlparse
-            filename = os.path.basename(urlparse(url).path.strip('/'))
+
+            filename = os.path.basename(urlparse(url).path.strip("/"))
     else:
         from urllib.parse import urlparse
-        filename = os.path.basename(urlparse(url).path.strip('/'))
+
+        filename = os.path.basename(urlparse(url).path.strip("/"))
     return url, re.sub(r"^\W+|\W+$", "", filename), res
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,149 +3,166 @@
 压缩与解压缩各种文件
 
 Compress and decompress all kinds of files
 """
 import io
 import os
 import sys
-import tarfile
-import zipfile
-import rarfile
-import py7zr
-from .. import dir_char, user_lang, qs_default_console, qs_warning_string
+
+from .. import (
+    user_lang,
+    qs_default_console,
+    qs_warning_string,
+    requirePackage,
+)
 
 
 def get_compress_package_name():
     """
     从命令行参数中，解析并返回压缩包名称
 
     From the command line arguments, the package name is parsed and returned.
 
     :return: 压缩包名称，合法的文件列表 | Compressed package name, a list of legitimate files.
     """
     file_names = sys.argv[2:]
     if not file_names:
-        exit('No enough parameters')
+        exit("No enough parameters")
     if len(file_names) > 1:
-        tar_name = 'pigeonhole'
+        name = "pigeonhole"
     else:
-        ls = file_names[0].split(dir_char)
-        while not ls[-1]:
-            ls.pop()
-        tar_name = ls[-1].split('.')[0]
+        name = os.path.basename(file_names[0]).split(".")[0]
     ls = []
     for file_name in file_names:
         if os.path.exists(file_name):
             ls.append(file_name)
         else:
-            print("No such file or dictionary:%s" % file_name)
-    return tar_name, ls
+            qs_default_console.print(
+                qs_warning_string,
+                f"{file_name} not found" if user_lang != "zh" else f"{file_name} 未找到",
+            )
+    return name, ls
 
 
-def checkIsProtocolFile(protocol, path):
+def checkIsProtocolFile(protocol, verify_func, path):
     """
     验证压缩包文件
 
     Verify compressed package file
+
     :param protocol: 压缩协议 | compress protocol
     :param path: 文件路径 | File Path
     :return:
     """
+
+    protocol_name = {
+        "tarfile": "tar",
+        "zipfile": "zip",
+        "rarfile": "rar",
+        "py7zr": "7z",
+    }
+
     if os.path.exists(path):
-        if protocol == tarfile and not tarfile.is_tarfile(path):
-            raise TypeError(f"{path} " + ('Not recognized by tar protocol' if user_lang != 'zh' else '无法被tar协议识别'))
-        elif protocol == zipfile and not zipfile.is_zipfile(path):
-            raise TypeError(f"{path} " + ('Not recognized by zip protocol' if user_lang != 'zh' else '无法被zip协议识别'))
-        elif protocol == rarfile and not rarfile.is_rarfile(path):
-            raise TypeError(f"{path} " + ('Not recognized by rar protocol' if user_lang != 'zh' else '无法被rar协议识别'))
-        elif protocol == py7zr and not py7zr.is_7zfile(path):
-            raise TypeError(f"{path} " + ('Not recognized by 7z protocol' if user_lang != 'zh' else '无法被7z协议识别'))
+        if not requirePackage(protocol, verify_func)(path):
+            raise TypeError(
+                f"{path} "
+                + (
+                    f"Not recognized by {protocol_name[protocol]} protocol"
+                    if user_lang != "zh"
+                    else f"无法被{protocol_name[protocol]}协议识别"
+                )
+            )
     else:
         raise FileNotFoundError
 
 
 class _NormalCompressedPackage:
     """
     通用压缩协议类，如果你不懂它是做什么的，请不要调用它
 
     General compression protocol class, if you do not understand what it does, please do not call it
     """
-    def __init__(self, _protocol, path: str, mode='r'):
+
+    def __init__(self, protocol, verify_func, obj_name, path: str, mode="r"):
         """
         通用压缩协议类初始化
 
         General compression protocol class initialization
 
-        :param _protocol: 压缩协议包 | General compression protocol packages
+        :param protocol: 压缩协议包 | General compression protocol packages
+        :param verify_func: 验证函数 | Verification function
+        :param obj_name: 对象名称 | Object name
         :param path: 压缩包路径 | compression package path
         :param mode: 读写模式 | 'r' or 'w', which 'r' means read and 'w' means write
         """
-        self._protocol = _protocol
+        self._protocol = protocol
         self.path = path
-        if mode not in ('r', 'w'):
+        if mode not in ("r", "w"):
             raise ValueError("Requires mode 'r', 'w'")
-        if mode == 'r':
-            checkIsProtocolFile(_protocol, path)
-            if _protocol == zipfile:
-                self.src = zipfile.ZipFile(path, 'r')
-            elif _protocol == rarfile:
-                self.src = rarfile.RarFile(path)
-            elif _protocol == py7zr:
-                self.src = py7zr.SevenZipFile(path, 'r')
+        if mode == "r":
+            checkIsProtocolFile(protocol, verify_func, path)
+            if protocol != "rarfile":
+                self.src = requirePackage(protocol, obj_name)(path, "r")
             else:
-                self.src = _protocol.open(path, 'r')
+                self.src = requirePackage(protocol, obj_name)(path)
             self.mode = True
-        elif mode == 'w':
-            if _protocol == tarfile:
-                self.src = _protocol.open(path, 'x:gz')
-            elif _protocol == zipfile:
-                self.src = _protocol.ZipFile(path, 'w')
-            elif _protocol == rarfile:
-                raise NotImplementedError('qs not support to create rar file because `RarFile`')
-            elif _protocol == py7zr:
-                self.src = _protocol.SevenZipFile(path, 'w')
+        elif mode == "w":
+            if protocol != "rarfile":
+                self.src = requirePackage(protocol, obj_name)(path, "w")
+            else:
+                raise NotImplementedError(
+                    "qs not support to create rar file because `RarFile`"
+                )
             self.mode = False
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add file to the compressed package (works in 'w' mode)
 
         :param path: 文件路径 | File path
         :return: None
         """
         if self.mode:
             raise io.UnsupportedOperation
-        if os.path.exists(path):
-            if self._protocol == tarfile:
+        if not os.path.exists(path):
+            raise FileNotFoundError
+        if os.path.isdir(path):
+            for root, dirs, files in os.walk(path):
+                for file in files:
+                    if self._protocol == "tarfile":
+                        self.src.add(os.path.join(root, file))
+                    elif self._protocol in ["zipfile", "py7zr"]:
+                        self.src.write(os.path.join(root, file))
+        else:
+            if self._protocol == "tarfile":
                 self.src.add(path)
-            elif self._protocol in [zipfile, py7zr]:
+            elif self._protocol in ["zipfile", "py7zr"]:
                 self.src.write(path)
-        else:
-            raise FileNotFoundError
 
     def extract(self):
         """
         解压缩 | extract
 
         :return: None
         """
         if self.mode:
-            if self._protocol in [tarfile, rarfile, py7zr]:
+            if self._protocol in ["tarfile", "rarfile", "py7zr"]:
                 self.src.extractall()
-            elif self._protocol in [zipfile]:
+            elif self._protocol == "zipfile":
                 from pathlib import Path
+
                 for fn in self.src.namelist():
                     path = Path(self.src.extract(fn))
                     try:
-                        path.rename(fn.encode('cp437').decode('utf-8'))
+                        path.rename(fn.encode("cp437").decode("utf-8"))
                     except:
                         try:
-                            path.rename(fn.encode('cp437').decode('gbk'))
+                            path.rename(fn.encode("cp437").decode("gbk"))
                         except Exception as e:
                             qs_default_console.log(qs_warning_string, repr(e))
 
             else:
                 raise NotImplementedError
             self.save()
         else:
@@ -157,24 +174,24 @@
 
         :return: None
         """
         self.src.close()
 
 
 class Tar(_NormalCompressedPackage):
-    def __init__(self, path, mode='r'):
+    def __init__(self, path, mode="r"):
         """
         Tar协议初始化
 
         Tar protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__(tarfile, path, mode)
+        super().__init__("tarfile", "is_tarfile", "TarFile", path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'write'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -195,24 +212,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class Zip(_NormalCompressedPackage):
-    def __init__(self, path, mode='r'):
+    def __init__(self, path, mode="r"):
         """
         Zip协议初始化
 
         Zip protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__(zipfile, path, mode)
+        super().__init__("zipfile", "is_zipfile", "ZipFile", path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -233,24 +250,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class Rar(_NormalCompressedPackage):
-    def __init__(self, path, mode='r'):
+    def __init__(self, path, mode="r"):
         """
         Rar协议初始化
 
         Rar protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__(rarfile, path, mode)
+        super().__init__("rarfile", "is_rarfile", "RarFile", path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -271,24 +288,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class SevenZip(_NormalCompressedPackage):
-    def __init__(self, path, mode='r'):
+    def __init__(self, path, mode="r"):
         """
         7z协议初始化
 
         7z protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__(py7zr, path, mode)
+        super().__init__("py7zr", "is_7zfile", "SevenZipFile", path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from .. import dir_char, qs_default_console, qs_error_string, qs_warning_string, user_lang
+from .. import (
+    qs_default_console,
+    qs_error_string,
+    qs_warning_string,
+    user_lang,
+    dir_char,
+)
 from ..SystemTools.FileHash import md5
 import os
 import re
 
 
 class DictionaryFiles(set):
     def __init__(self, rt: str, ignorePatterns: list = None):
@@ -11,19 +17,19 @@
         """
         super().__init__()
         if ignorePatterns is None:
             ignorePatterns = []
         if not (os.path.exists(rt) or os.path.isdir(rt)):
             qs_default_console.log(
                 qs_error_string,
-                f'"{rt}" {"Not exist or Not a dictionary!" if user_lang != "zh" else "不存在或不是文件夹"}'
+                f'"{rt}" {"Not exist or Not a dictionary!" if user_lang != "zh" else "不存在或不是文件夹"}',
             )
             self.available = False
             return
-        self.name = rt.strip(dir_char).split(dir_char)[-1]
+        self.name = os.path.basename(rt)
         self.rt = os.path.abspath(rt)
         self.available = True
         self.ignored = set(ignorePatterns) if ignorePatterns else None
         self.__getAllPaths()
 
     def checkIgnore(self, path):
         if self.ignored:
@@ -31,15 +37,15 @@
                 if re.findall(item, path):
                     return True
         return False
 
     def __getAllPaths(self):
         for rt, sonDir, files in os.walk(self.rt):
             for file in files:
-                filePath = os.path.join(rt, file).replace(self.rt, '')
+                filePath = os.path.join(rt, file).replace(self.rt, "")
                 if self.checkIgnore(filePath):
                     continue
                 self.add(filePath)
 
     def getMd5ByFileItem(self, item: str):
         return md5(self.rt + item)
 
@@ -51,42 +57,43 @@
     from concurrent.futures import ThreadPoolExecutor, wait
     from rich.progress import Progress
     from difflib import HtmlDiff
 
     def __init__(self, d1: DictionaryFiles, d2: DictionaryFiles):
         self.d1 = d1
         self.d2 = d2
-        self.rt = os.getcwd() + dir_char + d1.name + '-vs-' + d2.name + '.qs_diff'
+        self.rt = os.path.join(os.getcwd(), d1.name + "-vs-" + d2.name + ".qs_diff")
         self.pool = DiffFilesToStructHtml.ThreadPoolExecutor(max_workers=8)
         self.jobLs = []
         self.progress = DiffFilesToStructHtml.Progress(console=qs_default_console)
-        self.pid = self.progress.add_task('compare' if user_lang != 'zh' else '对比')
+        self.pid = self.progress.add_task("compare" if user_lang != "zh" else "对比")
 
     def _run(self, item: str):
         pathLs = item.strip(dir_char).split(dir_char)[:-1]
         for i in range(len(pathLs)):
-            dirName = self.rt + dir_char + dir_char.join(pathLs[:i+1])
+            dirName = os.path.join(self.rt, *pathLs[: i + 1])
             if not os.path.exists(dirName):
                 os.mkdir(dirName)
-        with open(self.d1.getFilepathByItem(item), 'r') as f:
+        with open(self.d1.getFilepathByItem(item), "r") as f:
             _d1 = f.readlines()
-        with open(self.d2.getFilepathByItem(item), 'r') as f:
+        with open(self.d2.getFilepathByItem(item), "r") as f:
             _d2 = f.readlines()
         _diff = DiffFilesToStructHtml.HtmlDiff().make_file(_d1, _d2)
-        with open(self.rt + item + '.html', 'w') as f:
+        with open(self.rt + item + ".html", "w") as f:
             f.write(_diff)
         self.progress.advance(self.pid, 1)
 
     def generate(self):
         if os.path.exists(self.rt):
             qs_default_console.log(
                 qs_warning_string,
-                f'"{self.rt}" {"Already exists! QS will delete it and regenerate." if user_lang != "zh" else "已经存在! QS将删除它并重新生成."}'
+                f'"{self.rt}" {"Already exists! QS will delete it and regenerate." if user_lang != "zh" else "已经存在! QS将删除它并重新生成."}',
             )
             from .. import remove
+
             remove(self.rt)
 
         os.mkdir(self.rt)
         _tmpLs = []
         for item in list(self.d1 & self.d2):
             if self.d1.getMd5ByFileItem(item) != self.d2.getMd5ByFileItem(item):
                 _tmpLs.append(item)
@@ -96,31 +103,42 @@
 
         for item in _tmpLs:
             self.jobLs.append(self.pool.submit(self._run, item))
 
         DiffFilesToStructHtml.wait(self.jobLs)
         self.progress.stop()
 
-        with open(self.rt + dir_char + 'README.md', 'w') as f:
-            print("# Diff Results | 目录对比结果", file=f, end='\n\n')
+        with open(os.path.join(self.rt, "README.md"), "w") as f:
+            print("# Diff Results | 目录对比结果", file=f, end="\n\n")
 
             print(
                 "## Several documents with differences as shown in the table below"
-                if user_lang != 'zh' else '## 存在若干有差异的文件如下表',
+                if user_lang != "zh"
+                else "## 存在若干有差异的文件如下表",
                 file=f,
-                end='\n\n'
+                end="\n\n",
             )
 
-            print(f'|{"Path" if user_lang != "zh" else "路径"}|{"Results Link" if user_lang != "zh" else "结果链接"}|\n|---|:---:|', file=f)
+            print(
+                f'|{"Path" if user_lang != "zh" else "路径"}|{"Results Link" if user_lang != "zh" else "结果链接"}|\n|---|:---:|',
+                file=f,
+            )
             for item in sorted(_tmpLs):
-                print(f'|{item}|[{"result" if user_lang != "zh" else "结果"}](file://{self.rt + item + ".html"})|', file=f)
+                print(
+                    f'|{item}|[{"result" if user_lang != "zh" else "结果"}](file://{self.rt + item + ".html"})|',
+                    file=f,
+                )
 
             print(
                 "## There are several non-shared documents as shown in the table below"
-                if user_lang != 'zh' else '## 存在若干非共有文件如下表',
+                if user_lang != "zh"
+                else "## 存在若干非共有文件如下表",
                 file=f,
-                end='\n\n'
+                end="\n\n",
             )
 
-            print(f'|{self.d1.name}|{self.d2.name}|\n|---|---|', file=f)
+            print(f"|{self.d1.name}|{self.d2.name}|\n|---|---|", file=f)
             for item in sorted(list(self.d1 ^ self.d2)):
-                print(f'|{item if item in self.d1 else " "}|{item if item in self.d2 else " "}|', file=f)
+                print(
+                    f'|{item if item in self.d1 else " "}|{item if item in self.d2 else " "}|',
+                    file=f,
+                )
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,44 +12,47 @@
 def hashWrapper(algorithm):
     """
     计算文件哈希值(通用)
 
     :param algorithm: 算法名 [md5, sha1, sha256, sha512]
     :return:
     """
+
     def Wrapper(func):
         def wrapper(filePath: str) -> str:
             global cal
             if not os.path.exists(filePath):
-                return 'No such file: ' + filePath
+                return "No such file: " + filePath
             if not os.path.isfile(filePath):
-                return 'Not a file: ' + filePath
+                return "Not a file: " + filePath
             cal = func()
-            with open(filePath, 'rb') as f:
+            with open(filePath, "rb") as f:
                 while True:
                     data = f.read(BlockSize)
                     if not data:
                         break
                     cal.update(data)
             return cal.hexdigest()
+
         return wrapper
+
     return Wrapper
 
 
-@hashWrapper('md5')
+@hashWrapper("md5")
 def md5():
     return hashlib.md5()
 
 
-@hashWrapper('sha1')
+@hashWrapper("sha1")
 def sha1():
     return hashlib.sha1()
 
 
-@hashWrapper('sha256')
+@hashWrapper("sha256")
 def sha256():
     return hashlib.sha256()
 
 
-@hashWrapper('sha512')
+@hashWrapper("sha512")
 def sha512():
     return hashlib.sha512()
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         (Multiple file pointer acceleration)
 
         :param filename: 文件名
         :param workers: 线程数
         :param mode: 读写模式，如'wb', 'rb+'
         """
         self.workers = workers
-        self.handles = [open(filename, mode) for i in range(workers)]
-        self.handles_lock = [threading.Lock() for i in range(workers)]
+        self.handles = [open(filename, mode) for _ in range(workers)]
+        self.handles_lock = [threading.Lock() for _ in range(workers)]
         self.pool = ThreadPoolExecutor(max_workers=workers)
         self.job_q = []
         self.cur_handle = 0
 
     def wait(self):
         """
         等待完全完成任务
@@ -88,20 +88,45 @@
 
         Write a new file block
 
         :param content: 文件内容
         :param index: 起始位置
         :return:
         """
-        self.job_q.append(self.pool.submit(self._write, self.cur_handle, content, index))
-        self.cur_handle = (self.cur_handle+1) % self.workers
+        self.job_q.append(
+            self.pool.submit(self._write, self.cur_handle, content, index)
+        )
+        self.cur_handle = (self.cur_handle + 1) % self.workers
 
     def __del__(self):
         """
         删除对象，必须等待线程池工作结束
 
         To delete an object, you must wait for the thread pool to finish working
 
         :return:
         """
         self.wait()
         self.pool.shutdown()
+
+
+class MemWriter:
+    def __init__(self):
+        """
+        线程安全的写内存。
+        """
+        from io import BytesIO
+
+        self.q = BytesIO()
+
+    def new_job(self, content: bytes, index: int):
+        # 将内容写入内存
+        self.q.seek(index)
+        self.q.write(content)
+
+    @property
+    def content(self):
+        # 获取内存内容
+        return self.q.getvalue()
+
+    def wait(self):
+        pass
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/TuiTools/Line.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 曲线图
 
 Line Graph
 """
 import io
 from .. import requirePackage
 
-diagram = requirePackage('diagram')
+diagram = requirePackage("diagram")
 
 
 class Line:
     def __init__(self, values: list, height: int, width: int):
         """
         折线图
 
@@ -31,20 +31,18 @@
 
         Draw and return a string
 
         :return: 折线图的字符串
         """
         opt = diagram.DOption()
         opt.size = diagram.Point([self.height, self.width])
-        opt.mode = 'g'
+        opt.mode = "g"
         stream = io.BytesIO()
         gram = diagram.DGWrapper(
-            data=[self.values, range(len(self.values))],
-            dg_option=opt,
-            ostream=stream
+            data=[self.values, range(len(self.values))], dg_option=opt, ostream=stream
         )
         gram.show()
         return str(stream.getvalue(), encoding="utf-8")
 
     def push(self, x: float):
         """
         尾部添加值
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,14 @@
 # coding=utf-8
 """
 qs用到的函数装饰器, 在使用它们前, 请确保你理解注释描述的内容
 
 Before using function decorators used by QS, please make sure that you understand the content described by the annotation.
 """
-
-
-def set_timeout(num: int):
-    """
-    定时函数装饰器
-
-    Timing function decorator
-
-    :param num: 时间（秒）
-    :return: wrapper
-    """
-    def wrapper(func):
-        def handle(signum, frame):
-            raise RuntimeError
-
-        def run(*args, **kwargs):
-            import signal
-            try:
-                signal.signal(signal.SIGALRM, handle)
-                signal.alarm(num)
-                res = func(*args, **kwargs)
-                signal.alarm(0)
-                return res
-            except RuntimeError:
-                return False
-        return run
-    return wrapper
+from QuickProject.__config__ import set_timeout
 
 
 def mkCompressPackageWrap(func):
     """
     创建压缩文件的通用函数装饰器, 被装饰的函数将被传递压缩文件名, 你需要返回:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     的子类对象, 并将读写状态设为 写 状态
@@ -43,34 +17,25 @@
     name, which you need to return:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     's sub object, and set read-write mode as write
 
     :param func: func(filePath: str = '') -> QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     :return: 装饰器 | wrapper
     """
+
     def wrapper():
-        import os
-        from .. import dir_char
         from ..SystemTools.Compress import get_compress_package_name
+
         packages_name, ls = get_compress_package_name()
         packages = func(packages_name)
 
-        def dfs(cur_p):
-            if os.path.isfile(cur_p):
-                packages.add_file(cur_p)
-                return
-            file_ls = os.listdir(cur_p)
-            flag_ch = '' if cur_p.endswith(dir_char) else dir_char
-            for fp in file_ls:
-                fp = cur_p + flag_ch + fp
-                dfs(fp)
-
         for i in ls:
-            dfs(i)
+            packages.add_file(i)
         packages.save()
+
     return wrapper
 
 
 def unCompressPackageWrap(func):
     """
     解压缩文件的通用函数装饰器, 被装饰的函数将被传递压缩文件名, 你需要返回:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
@@ -80,61 +45,71 @@
     name, which you need to return:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     's sub object, and set read-write mode as read
 
     :param func: func(filePath: str = '') -> QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     :return: 装饰器 | wrapper
     """
+
     def wrapper():
         import os
         import sys
 
         file_names = sys.argv[2:]
         if not file_names:
             exit("No enough parameters")
         from .. import qs_default_console, qs_error_string
         from ..NetTools.NormalDL import core_num
         from ..ThreadTools import ThreadPoolExecutor, wait
+
         pool = ThreadPoolExecutor(max_workers=max(core_num // 2, 4))
         job_q = []
 
         def run(path):
             if os.path.exists(path):
                 try:
                     cur_tar = func(path)
                     cur_tar.extract()
                 except Exception as e:
                     qs_default_console.log(qs_error_string, repr(e))
             else:
-                qs_default_console.log(qs_error_string, "No such file or dictionary: %s" % path)
+                qs_default_console.log(
+                    qs_error_string, "No such file or dictionary: %s" % path
+                )
 
         for file_name in file_names:
             job_q.append(pool.submit(run, file_name))
         wait(job_q)
+
     return wrapper
 
 
-def HashWrapper(algorithm: str):
+def HashWrapper():
     """
     文件哈希值计算(通用函数)
-
-    :param algorithm: 算法名称 [md5, sha1, sha256, sha512]
     :return:
     """
+
     def Wrapper(func):
+        algorithm = func.__name__
+
         def _wrapper():
             import sys, os
-            from .. import qs_default_console, qs_info_string, user_lang
+            from .. import qs_default_console, qs_info_string, requirePackage
 
             ls = sys.argv[2:]
             if not ls:
-                qs_default_console.print(qs_info_string, 'Usage: qs %s file1 file2 ...' % algorithm)
+                qs_default_console.print(
+                    qs_info_string, "Usage: qs %s file1 file2 ..." % algorithm
+                )
                 return
 
-            exec('from QuickStart_Rhy.SystemTools.FileHash import %s' % algorithm)
+            func = requirePackage(".SystemTools.FileHash", algorithm)
             for file in ls:
                 qs_default_console.print(
-                    qs_info_string, 'Calculate:' if user_lang != 'zh' else '计算:', os.path.basename(file)
+                    f"\[[bold magenta]{algorithm}[/]]",
+                    f"[underline]{os.path.basename(file)}[/]: '{func(file)}'",
                 )
-                exec(f'qs_default_console.print(qs_info_string, "{algorithm}" + ":", {algorithm}("{file}"))')
+
         return _wrapper
+
     return Wrapper
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/api.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/apiTools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,505 +1,480 @@
 # coding=utf-8
 """
 调用各种qs的API
 
 Call various QS API
 """
 import sys
-from . import user_lang, system, qs_default_console, qs_error_string, qs_info_string, qs_warning_string, requirePackage
+
+from . import (
+    user_lang,
+    platform,
+    qs_default_console,
+    qs_default_status,
+    qs_error_string,
+    qs_info_string,
+    qs_warning_string,
+    requirePackage,
+)
 
 
 def remove_bg():
     """
     删除图片背景
 
     Delete image background
     """
-    try:
-        path = sys.argv[2]
-    except IndexError:
-        qs_default_console.log(qs_error_string,
-                               '%s: qs rmbg <%s>' % (('Usage', 'picture') if user_lang != 'zh' else ('用法', '图像')))
-        return
-    else:
-        if path == '-helpF':
-            qs_default_console.print(qs_info_string,
-                                     '%s: qs rmbg <%s>' % (('Usage', 'picture')
-                                                           if user_lang != 'zh' else ('用法', '图像')))
-            return
-        from .API.SimpleAPI import rmbg
-        with qs_default_console.status('Dealing..' if user_lang != 'zh' else '处理中..') as st:
-            rmbg(path)
-            st.update(status='Done')
+    path = sys.argv[2]
+    from .API.SimpleAPI import rmbg
+
+    with qs_default_status("Dealing.." if user_lang != "zh" else "处理中.."):
+        rmbg(path)
 
 
 def smms():
     """
     上传图片或Markdown中图片到smms
 
     Upload images or Markdown images to SMMS
     """
-    try:
-        path = sys.argv[2]
-    except IndexError:
-        qs_default_console.log(
-            qs_error_string,
-            '%s: qs smms <%s>' % (('Usage', 'picture | *.md')
-                                  if user_lang != 'zh' else ('用法', '图像 | *.md'))
-        )
-        return
-    else:
-        if path == '-help':
-            qs_default_console.print(
-                qs_info_string,
-                '%s: qs smms <%s>' % (('Usage', 'picture | *.md')
-                                      if user_lang != 'zh' else ('用法', '图像 | *.md'))
-            )
-            return
-        from .API.SimpleAPI import smms
-        with qs_default_console.status('Dealing..' if user_lang != 'zh' else '处理中..') as st:
-            smms(path)
-            st.update(status='Done')
-
-
-def up_img():
-    """
-    上传图片或Markdown中图片到多平台（不保证数据安全）
-
-    Upload images or Markdown images to multiple platforms (data security is not guaranteed)
-    """
+    from .API.SimpleAPI import smms
 
-    def showSptPlatform(dt, ls):
-        from rich.table import Table
-        from rich.box import SIMPLE
-
-        tb = Table('1', '2', '3', show_header=False, show_edge=False, box=SIMPLE)
-        for indx in range(0, len(ls), 3):
-            row = []
-            for i in range(indx, indx + 3):
-                if i < len(ls):
-                    row.append(f'{ls[i]}: {dt[ls[i]]}')
-                else:
-                    break
-            tb.add_row(*row)
-        qs_default_console.print(
-            qs_info_string,
-            'Usage: qs upimg <picture | *.md> [platform]\n\nSupport ([platform]: description):'
-            if user_lang != 'zh' else '用法: qs -upimg <图像 | *.md> [平台]\n\n支持 ([可选平台]: 描述):')
-        qs_default_console.print(tb, justify="center")
-
-    try:
-        path = sys.argv[2]
-    except IndexError:
-        qs_default_console.log(qs_error_string, '%s: qs upimg <%s>' % (('Usage', 'picture | *.md')
-                                                                       if user_lang != 'zh' else ('用法', '图像 | *.md')))
-        return
-    else:
-        from .API.alapi import upload_image, _upimg_get_avaliable_platform
-        import random
-
-        spt_type = _upimg_get_avaliable_platform()
-        spt_type_keys = list(spt_type.keys())
-        if '-h' in sys.argv or '--help' in sys.argv:
-            showSptPlatform(spt_type, spt_type_keys)
-            qs_default_console.print(
-                qs_info_string,
-                'If you do not set platform, qs will randomly choose one.' if user_lang != 'zh' else
-                '如果你没有设置平台，qs将随机抽取一个可用平台')
-            return
-        argv_len_3 = len(sys.argv) > 3
-        if argv_len_3:
-            sys.argv[3] = sys.argv[3].lower()
-            type_map = {}
-            for i in spt_type:
-                type_map[i.lower()] = i
-
-            upload_image(path, type_map[sys.argv[3]]) \
-                if argv_len_3 and sys.argv[3] in type_map else (
-                qs_default_console.print(
-                    qs_warning_string,
-                    ('No such platform: %s' if user_lang != 'zh' else '不支持设定的平台: %s') % sys.argv[3]),
-                showSptPlatform(spt_type, spt_type_keys),
-                qs_default_console.print(qs_error_string, 'Upload Failed' if user_lang != 'zh' else '上传失败!')
-            )
-
-        else:
-            upload_image(path, plt_type=random.choice(spt_type_keys))
+    with qs_default_status("Dealing.." if user_lang != "zh" else "处理中.."):
+        smms(sys.argv[2])
 
 
 def ali_oss():
     """
     阿里云对象存储
 
     Ali Cloud object storage
     """
-    try:
-        op = sys.argv[2]
-        if op not in ['-dl', '-up', '-ls', '-rm']:
-            raise IndexError
-        file = sys.argv[3] if op != '-ls' else None
-        try:
-            bucket = sys.argv[4] if op != '-ls' else sys.argv[3]
-        except IndexError:
-            bucket = None
-    except IndexError:
-        qs_default_console.print(
-            qs_info_string,
-            'qs alioss:\n'
-            '    -up <file> [bucket]: upload file to bucket\n'
-            '    -dl <file> [bucket]: download file from bucket\n'
-            '    -rm <file> [bucket]: remove file in bucket\n'
-            '    -ls [bucket]       : get file info of bucket'
-        ) if user_lang != 'zh' else qs_default_console.print(
-            qs_info_string,
-            'qs alioss:\n'
-            '    -up <文件> [桶]: 上传文件至桶\n'
-            '    -dl <文件> [桶]: 从桶下载文件\n'
-            '    -rm <文件> [桶]: 从桶删除文件\n'
-            '    -ls [桶]       : 获取桶文件信息'
-        )
-        return
+    op = sys.argv[2]
+    if op not in ["-dl", "-up", "-ls", "-rm"]:
+        raise NotImplementedError
+    if op != "-ls" and "--bucket" in sys.argv:
+        bucket = sys.argv[sys.argv.index("--bucket") + 1]
+    elif op == "-ls":
+        bucket = None if len(sys.argv) < 4 else sys.argv[3]
     else:
-        from .API.AliCloud import AliyunOSS
-        ali_api = AliyunOSS()
-        func_table = ali_api.get_func_table()
-        if not file:
-            func_table[op](bucket)
-        else:
-            func_table[op](file, bucket)
+        bucket = None
+    files = sys.argv[3:] if op != "-ls" else []
+
+    from .API.AliCloud import AliyunOSS
+
+    ali_api = AliyunOSS()
+    func_table = ali_api.get_func_table()
+    for file in files:
+        func_table[op](file, bucket)
+    if not files:
+        func_table[op](bucket)
 
 
 def qiniu():
     """
     七牛云对象存储
 
     Qiniu cloud object storage
     """
-    try:
-        op = sys.argv[2]
-        if op not in ['-up', '-rm', '-cp', '-ls', '-dl']:
-            raise IndexError
-        file = sys.argv[3] if op != '-ls' else None
-        try:
-            bucket = sys.argv[4] if op != '-ls' else sys.argv[3]
-        except IndexError:
-            bucket = None
-    except IndexError:
-        qs_default_console.print(
-            qs_info_string,
-            'qs qiniu:\n'
-            '    -up <file> [bucket]: upload file to bucket\n'
-            '    -dl <file> [bucket]: download file from bucket\n'
-            '    -cp <url > [bucket]: copy file from url\n'
-            '    -rm <file> [bucket]: remove file in bucket\n'
-            '    -ls [bucket]       : get file info of bucket'
-        ) if user_lang != 'zh' else qs_default_console.print(
-            qs_info_string,
-            'qs qiniu:\n'
-            '    -up <文件> [桶]: 上传文件至桶\n'
-            '    -dl <文件> [桶]: 从桶下载文件\n'
-            '    -cp <链接> [桶]: 从链接下载文件到桶\n'
-            '    -rm <文件> [桶]: 从桶删除文件\n'
-            '    -ls [桶]       : 获取桶文件信息'
-        )
-        return
+    op = sys.argv[2]
+    if op not in ["-dl", "-up", "-ls", "-rm"]:
+        raise NotImplementedError
+    if op != "-ls" and "--bucket" in sys.argv:
+        bucket = sys.argv[sys.argv.index("--bucket") + 1]
+    elif op == "-ls":
+        bucket = None if len(sys.argv) < 4 else sys.argv[3]
     else:
-        from .API.QiniuOSS import QiniuOSS
-        qiniu_api = QiniuOSS()
-        func_table = qiniu_api.get_func_table()
-        if not file:
-            func_table[op](bucket)
-        else:
-            func_table[op](file, bucket)
+        bucket = None
+    files = sys.argv[3:] if op != "-ls" else []
+
+    from .API.QiniuOSS import QiniuOSS
+
+    qiniu_api = QiniuOSS()
+    func_table = qiniu_api.get_func_table()
+    for file in files:
+        func_table[op](file, bucket)
+    if not files:
+        func_table[op](bucket)
 
 
 def txcos():
     """
     腾讯云对象存储
 
     Tencent Cloud object storage
     """
-    try:
-        op = sys.argv[2]
-        if op not in ['-dl', '-up', '-ls', '-rm']:
-            raise IndexError
-        file = sys.argv[3] if op != '-ls' else None
-        try:
-            bucket = sys.argv[4] if op != '-ls' else sys.argv[3]
-        except IndexError:
-            bucket = None
-    except IndexError:
-        qs_default_console.print(
-            qs_info_string,
-            'qs alioss:\n'
-            '    -up <file> [bucket]: upload file to bucket\n'
-            '    -dl <file> [bucket]: download file from bucket\n'
-            '    -rm <file> [bucket]: remove file in bucket\n'
-            '    -ls [bucket]       : get file info of bucket'
-        ) if user_lang != 'zh' else qs_default_console.print(
-            qs_info_string,
-            'qs alioss:\n'
-            '    -up <文件> [桶]: 上传文件至桶\n'
-            '    -dl <文件> [桶]: 从桶下载文件\n'
-            '    -rm <文件> [桶]: 从桶删除文件\n'
-            '    -ls [桶]       : 获取桶文件信息'
-        )
-        return
+    op = sys.argv[2]
+    if op not in ["-dl", "-up", "-ls", "-rm"]:
+        raise IndexError
+    if op != "-ls" and "--bucket" in sys.argv:
+        bucket = sys.argv[sys.argv.index("--bucket") + 1]
+    elif op == "-ls":
+        bucket = None if len(sys.argv) < 4 else sys.argv[3]
     else:
-        from .API.TencentCloud import TxCOS
-        tx_api = TxCOS()
-        func_table = tx_api.get_func_table()
-        if not file:
-            func_table[op](bucket)
-        else:
-            func_table[op](file, bucket)
+        bucket = None
+    files = sys.argv[3:] if op != "-ls" else []
+
+    from .API.TencentCloud import TxCOS
+
+    tx_api = TxCOS()
+    func_table = tx_api.get_func_table()
+    for file in files:
+        func_table[op](file, bucket)
+    if not files:
+        func_table[op](bucket)
 
 
-def translate():
+def translate(content: str = None, target_lang: str = user_lang):
     """
     qs默认的翻译引擎
 
     Qs default Translation engine
+
+    :param content: 需要翻译的内容
     """
     from . import trans_engine
-    pyperclip = requirePackage('pyperclip')
-    if trans_engine != 'default':
-        from .API.TencentCloud import translate
-    else:
-        from .API.alapi import translate
+    from requests.exceptions import SSLError
+
+    if trans_engine == "default":
+        trans_engine = "alapi"
+
+    _translate = requirePackage(f".API.{trans_engine}", "translate")
 
-    content = ' '.join(sys.argv[2:])
+    output_flag = False if content else True
+    if not content:
+        content = " ".join(sys.argv[2:])
     if not content:
         try:
-            content = pyperclip.paste()
+            content = requirePackage("pyperclip", "paste")()
         except:
             from . import qs_default_input
+
             content = qs_default_input.ask(
-                'Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: '
-                if user_lang != 'zh' else '抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:')
+                "Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: "
+                if user_lang != "zh"
+                else "抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:"
+            )
     if content:
-        ret = translate(content.replace('\n', ' '))
-        qs_default_console.print(ret) if ret else qs_default_console.log(qs_error_string, 'Translate Failed!')
+        retry = 3
+        lang = requirePackage("langid", "classify")(content)[0]
+        while retry:
+            try:
+                ret = _translate(
+                    content,
+                    target_lang="en"
+                    if target_lang == user_lang == lang
+                    else target_lang,
+                )
+                break
+            except SSLError:
+                retry -= 1
+                qs_default_console.log(
+                    qs_warning_string,
+                    f"SSL Error, Retrying... \[{3 - retry} / 3]"
+                    if user_lang != "zh"
+                    else f"SSL错误，重试中... \[{3 - retry} / 3]",
+                )
+            except Exception as e:
+                # qs_default_console.log(qs_error_string, e)
+                qs_default_console.print_exception()
+                return None
+
+        if output_flag and ret:
+            if ret:
+                from . import cut_string
+
+                display = "\n".join(
+                    [
+                        " ".join(
+                            cut_string(
+                                line, qs_default_console.width, ignore_charset="`"
+                            )
+                        )
+                        for line in ret.split("\n")
+                    ]
+                )
+                qs_default_console.print(display)
+            else:
+                qs_default_console.log(qs_error_string, "Translate Failed!")
+        return ret
     else:
         qs_default_console.log(
             qs_warning_string,
             "No content in your clipboard or command parameters!"
-            if user_lang != 'zh' else
-            '剪贴板或命令参数没有内容!')
+            if user_lang != "zh"
+            else "剪贴板或命令参数没有内容!",
+        )
+        return None
 
 
 def weather():
     """查天气 | Check weather"""
-    from . import headers, dir_char
+    from .NetTools import headers
     from .ThreadTools import ThreadFunctionWrapper
     import requests
 
     def get_data(url):
         try:
             ct = requests.get(url, headers)
         except:
             return
-        ct.encoding = 'utf-8'
-        ct = ct.text.split('\n')
-        if dir_char == '/':
+        ct.encoding = "utf-8"
+        ct = ct.text.split("\n")
+        if not platform.startswith("win"):
             res = ct.copy()
         else:
             import re
+
             for line in range(len(ct)):
-                ct[line] = re.sub('\x1b.*?m', '', ct[line])
+                ct[line] = re.sub("\x1b.*?m", "", ct[line])
             res = ct.copy()
         return res
 
     try:
         loc = sys.argv[2]
     except IndexError:
-        loc = ''
-    tls = [ThreadFunctionWrapper(get_data, 'https://wttr.in/' + (loc if loc else '?lang={}'.format(user_lang))),
-           ThreadFunctionWrapper(get_data, 'https://v2.wttr.in/' + loc)]
+        loc = ""
+    tls = [
+        ThreadFunctionWrapper(
+            get_data,
+            "https://wttr.in/" + (loc if loc else "?lang={}".format(user_lang)),
+        ),
+        ThreadFunctionWrapper(get_data, "https://v2.wttr.in/" + loc),
+    ]
     for i in tls:
         i.start()
-    with qs_default_console.status('Requesting..' if user_lang != 'zh' else '请求中..') as st:
+    with qs_default_status("Requesting.." if user_lang != "zh" else "请求中.."):
         for i in tls:
             i.join()
-        st.update(status='Done')
     simple = tls[0].get_res()
     table = tls[1].get_res()
     if simple:
         if not loc:
-            if user_lang == 'zh':
+            if user_lang == "zh":
                 from .API.alapi import translate
-                enLocation = simple[0].split('：')[-1].strip()
+
+                enLocation = simple[0].split("：")[-1].strip()
                 trans_loaction = translate(enLocation)
-                qs_default_console.print('地区：' + trans_loaction if trans_loaction else enLocation)
+                qs_default_console.print(
+                    "地区：" + trans_loaction if trans_loaction else enLocation
+                )
             else:
-                qs_default_console.print('Location' + simple[0][simple[0].index(':'):])
+                qs_default_console.print("Location" + simple[0][simple[0].index(":") :])
         simple = simple[2:7]
-        print('\n'.join(simple))
+        print("\n".join(simple))
     else:
-        qs_default_console.log(qs_error_string, 'Get data failed.' if user_lang != 'zh' else '错误: 获取数据失败')
+        qs_default_console.log(
+            qs_error_string, "Get data failed." if user_lang != "zh" else "错误: 获取数据失败"
+        )
     if table:
         qs_default_console.print(table[3][:-1])
         bottom_line = 7
         try:
-            while '╂' not in table[bottom_line]:
+            while "╂" not in table[bottom_line]:
                 bottom_line += 1
         except IndexError:
-            qs_default_console.log(qs_error_string, 'Get Weather Data failed!' if user_lang != 'zh' else '获取天气数据失败')
+            qs_default_console.log(
+                qs_error_string,
+                "Get Weather Data failed!" if user_lang != "zh" else "获取天气数据失败",
+            )
             return
-        for i in table[7:bottom_line + 2]:
+        for i in table[7 : bottom_line + 2]:
             print(i[:-1])
-        print('└────────────────────────────────────────────────────────────────────────')
-        print('\n'.join(table[-3 if not loc else -4:]))
+        print(
+            "└────────────────────────────────────────────────────────────────────────"
+        )
+        print("\n".join(table[-3 if not loc else -4 :]))
     else:
-        print('Error: Get data failed.' if user_lang != 'zh' else '错误: 获取数据失败')
+        print("Error: Get data failed." if user_lang != "zh" else "错误: 获取数据失败")
 
 
 def largeImage():
     """
     百度图片效果增强
 
     Baidu picture effect enhancement
     """
     try:
         path = sys.argv[2]
     except IndexError:
-        qs_default_console.log(qs_error_string, '%s: qs LG <img>' % 'Usage' if user_lang != 'zh' else '用法')
+        qs_default_console.log(
+            qs_error_string, "%s: qs LG <img>" % "Usage" if user_lang != "zh" else "用法"
+        )
         return
     else:
         from .API.BaiduCloud import ImageDeal
+
         aip_cli = ImageDeal()
-        with qs_default_console.status('Dealing..' if user_lang != 'zh' else '处理中..') as st:
-            aip_cli.largeImage(path, st)
-            st.update(status='Done')
+        with qs_default_status("Dealing.." if user_lang != "zh" else "处理中.."):
+            aip_cli.largeImage(path)
 
 
 def AipNLP():
     """百度NLP | Baidu NLP"""
     from .API.BaiduCloud import AipNLP
-    pyperclip = requirePackage('pyperclip')
+
+    pyperclip = requirePackage("pyperclip")
+
+    pyperclip.paste()
     ct = sys.argv[2:]
     if not ct:
         try:
             ct = [pyperclip.paste()]
         except:
             from . import qs_default_input
-            ct = [qs_default_input.ask(
-                'Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: '
-                if user_lang != 'zh' else '抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:')]
+
+            ct = [
+                qs_default_input.ask(
+                    "Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: "
+                    if user_lang != "zh"
+                    else "抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:"
+                )
+            ]
     NLP = AipNLP()
     for _id, line in enumerate(ct):
         ct[_id] = NLP.get_res(line)
         if _id == 9:
-            qs_default_console.print('...')
+            qs_default_console.print("...")
         elif _id < 9:
             qs_default_console.print(ct[_id])
     try:
-        pyperclip.copy('\n'.join(ct))
+        pyperclip.copy("\n".join(ct))
     except:
         pass
 
 
 def bili_cover():
     """下载Bilibili视频、直播的封面图片（视频链接、视频号均可识别）"""
     from .API.alapi import bili_cover as bc
-    pyperclip = requirePackage('pyperclip')
+
+    pyperclip = requirePackage("pyperclip")
 
     try:
         url = sys.argv[2]
     except IndexError:
         try:
             url = pyperclip.paste()
         except:
             qs_default_console.log(
-                qs_error_string, 'Sorry, but your system may not be suppported by `pyperclip`'
-                if user_lang != 'zh' else '抱歉，但是“pyperclip”不支持你的系统')
+                qs_error_string,
+                "Sorry, but your system may not be suppported by `pyperclip`"
+                if user_lang != "zh"
+                else "抱歉，但是“pyperclip”不支持你的系统",
+            )
             return
     if not url:
         qs_default_console.log(
-            qs_error_string, 'Usage: qs bcv <url | video code>'
-            if user_lang != 'zh' else '用法: qs bcv <链接 | 视频码>')
+            qs_error_string,
+            "Usage: qs bcv <url | video code>"
+            if user_lang != "zh"
+            else "用法: qs bcv <链接 | 视频码>",
+        )
         return
     bc(url)
 
 
 def gbc():
     """查询中国垃圾分类（且仅支持中文查询）"""
     from .API.alapi import garbage_classification
+
     try:
-        with qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..') as st:
+        with qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中.."):
             res = garbage_classification(sys.argv[2:])
-            st.update(status='Done')
-        qs_default_console.print(res, justify='center')
+        qs_default_console.print(res, justify="center")
     except Exception as e:
         qs_default_console.print(qs_error_string, repr(e))
         qs_default_console.print(
             qs_error_string,
-            'Usage: qs gbc <garbage...>' if user_lang != 'zh' else '用法: qs gbc <垃圾...>')
+            "Usage: qs gbc <garbage...>" if user_lang != "zh" else "用法: qs gbc <垃圾...>",
+        )
 
 
 def short_video_info(son_call=False):
     """
     获取短视频信息 | Get short video information
 
     :return:
     """
     from .API.alapi import short_video_info
     from .NetTools import get_fileinfo, size_format
-    pyperclip = requirePackage('pyperclip')
+
+    pyperclip = requirePackage("pyperclip")
     import re
+
     try:
         url = sys.argv[2]
     except IndexError:
         try:
             url = pyperclip.paste()
-            url = re.findall('https?://(?:[-\w.]|%[\da-fA-F]{2}|[/])+', url)[0]
+            url = re.findall("https?://(?:[-\w.]|%[\da-fA-F]{2}|[/])+", url)[0]
         except:
             qs_default_console.print(
-                qs_error_string, 'Sorry, but your system may not be suppported by `pyperclip`'
-                if user_lang != 'zh' else '抱歉，但是“pyperclip”不支持你的系统')
+                qs_error_string,
+                "Sorry, but your system may not be suppported by `pyperclip`"
+                if user_lang != "zh"
+                else "抱歉，但是“pyperclip”不支持你的系统",
+            )
             return
     if not url:
         qs_default_console.print(
-            qs_error_string, 'Usage: qs svi <url/video code>' if not son_call else 'Usage: qs svd <url/video code>')
+            qs_error_string,
+            "Usage: qs svi <url/video code>"
+            if not son_call
+            else "Usage: qs svd <url/video code>",
+        )
         return
     output_prefix = {
-        'title': 'Title ' if user_lang != 'zh' else '标题',
-        'video': 'Video ' if user_lang != 'zh' else '视频',
-        'cover': 'Cover ' if user_lang != 'zh' else '封面',
-        'source': 'Source' if user_lang != 'zh' else '来源'
+        "title": "Title " if user_lang != "zh" else "标题",
+        "video": "Video " if user_lang != "zh" else "视频",
+        "cover": "Cover " if user_lang != "zh" else "封面",
+        "source": "Source" if user_lang != "zh" else "来源",
     }
-    with qs_default_console.status('正在获取视频信息') as _:
-        status, res = short_video_info(url.strip('/'))
+
+    with qs_default_status("正在获取视频信息"):
+        status, res = short_video_info(url.strip("/"))
         if not status:
-            qs_default_console.print(qs_info_string, res['title'] + ':' + res['source'])
+            qs_default_console.print(qs_info_string, res["title"] + ":" + res["source"])
             return status
-        showStatus = '-url' in sys.argv
-        qs_default_console.print(qs_info_string, '[{}] {}'.format(output_prefix['title'], res['title']))
-        if res['video_url']:
-            sz = int(get_fileinfo(res['video_url'])[-1].headers['content-length']) if not son_call else -1
+        showStatus = "-url" in sys.argv
+        qs_default_console.print(
+            qs_info_string, "[{}] {}".format(output_prefix["title"], res["title"])
+        )
+        if res["video_url"]:
+            sz = (
+                int(get_fileinfo(res["video_url"])[-1].headers["content-length"])
+                if not son_call
+                else -1
+            )
             qs_default_console.print(
                 qs_info_string,
-                '[{}] {}\n{}'.format(
-                    output_prefix['video'],
-                    size_format(sz, True) if sz > 0 else '--',
-                    res['video_url'] if showStatus else ''
-                )
+                "[{}] {}\n{}".format(
+                    output_prefix["video"],
+                    size_format(sz, True) if sz > 0 else "--",
+                    res["video_url"] if showStatus else "",
+                ),
             )
         if showStatus:
-            sz = int(get_fileinfo(res['cover_url'])[-1].headers['content-length'])
+            sz = int(get_fileinfo(res["cover_url"])[-1].headers["content-length"])
             qs_default_console.print(
                 qs_info_string,
-                '[{}] {}\n{}'.format(output_prefix['cover'], size_format(sz, True),
-                                     res['cover_url'] if showStatus else '')
+                "[{}] {}\n{}".format(
+                    output_prefix["cover"],
+                    size_format(sz, True),
+                    res["cover_url"] if showStatus else "",
+                ),
             )
-    if system == 'darwin':
+    if platform == "darwin":
         from .ImageTools.ImagePreview import image_preview
-        image_preview(res['cover_url'], True)
-    if 'source' in res and res['source']:
-        qs_default_console.print(qs_info_string, '[{}] {}'.format(output_prefix['source'], res['source']))
+
+        image_preview(res["cover_url"], True)
+    if "source" in res and res["source"]:
+        qs_default_console.print(
+            qs_info_string, "[{}] {}".format(output_prefix["source"], res["source"])
+        )
     return res
 
 
 def short_video_dl():
     """
     下载短视频为mp4格式
 
@@ -510,26 +485,29 @@
     from .NetTools.NormalDL import normal_dl
     from .ImageTools.VideoTools import tomp4
     from . import remove
 
     res = short_video_info(son_call=True)
 
     if not res:
-        qs_default_console.print(qs_error_string, 'Download failed' if user_lang != 'zh' else '下载失败')
+        qs_default_console.print(
+            qs_error_string, "Download failed" if user_lang != "zh" else "下载失败"
+        )
         return
 
-    fileName = res['title'] if res['title'] else 'UnknownTitle'
-    if 'pics' in res and res['pics']:
+    fileName = res["title"] if res["title"] else "UnknownTitle"
+    if "pics" in res and res["pics"]:
         from .ImageTools.ImageTools import topng
-        for index, url in enumerate(res['pics']):
+
+        for index, url in enumerate(res["pics"]):
             normal_dl(url, set_name=fileName + str(index + 1))
             topng(fileName + str(index + 1))
             remove(fileName + str(index + 1))
-    elif res['video_url']:
-        normal_dl(res['video_url'], set_name=fileName)
+    elif res["video_url"]:
+        normal_dl(res["video_url"], set_name=fileName)
         tomp4(fileName)
         remove(fileName)
 
 
 def acg():
     """
     获取随机acg图片链接（可选择下载）
@@ -538,132 +516,178 @@
 
     :return:
     """
     import random
     from .API.alapi import acg
     from .API.SimpleAPI import acg2
 
-    st = qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..')
-    st.start()
+    qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中..").start()
     try:
         status, acg_link, width, height = random.choice([acg, acg2])()
-        qs_default_console.print(qs_info_string, f"{'链接' if user_lang == 'zh' else 'LINK'}: {acg_link}") \
-            if status else qs_default_console.log(qs_error_string, acg_link)
+        qs_default_console.print(
+            qs_info_string, f"{'链接' if user_lang == 'zh' else 'LINK'}: {acg_link}"
+        ) if status else qs_default_console.log(qs_error_string, acg_link)
         if status:
-            qs_default_console.print(qs_info_string, '尺寸:' if user_lang == 'zh' else 'SIZE:', width, '×', height)
-            if '--save' in sys.argv[2:]:
-                from . import dir_char
+            qs_default_console.print(
+                qs_info_string,
+                "尺寸:" if user_lang == "zh" else "SIZE:",
+                width,
+                "×",
+                height,
+            )
+            if "--save" in sys.argv[2:]:
                 from .NetTools.NormalDL import normal_dl
-                st.stop()
-                acg_link = normal_dl(acg_link)  # disable download status for Windows
-            if system == 'darwin':  # Only support iTerm for Mac OS X
-                from .ImageTools.ImagePreview import image_preview
-                st.update(status='Loading image...\n' if user_lang != 'zh' else '加载图片中..\n')
-                image_preview(open(acg_link) if '--save' in sys.argv[2:] else acg_link,
-                              '--save' not in sys.argv[2:], qs_console_status=st)
-                return
+
+                # disable download status for Windows
+                acg_link = normal_dl(acg_link)
+            from .ImageTools.ImagePreview import image_preview
+
+            qs_default_status(
+                status="Loading image...\n" if user_lang != "zh" else "加载图片中..\n"
+            ).start()
+            image_preview(
+                open(acg_link) if "--save" in sys.argv[2:] else acg_link,
+                "--save" not in sys.argv[2:],
+            )
+            return
     except Exception as e:
         qs_default_console.print(qs_error_string, repr(e))
     finally:
-        st.stop()
+        qs_default_status.stop()
 
 
 def bingImg():
     """
     获取bing图片链接（可选择下载）
 
     Get links to bing images (download optional)
 
     :return:
     """
     from .API.alapi import bingImg
 
-    st = qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..')
-    st.start()
+    qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中..").start()
 
     try:
         status, acg_link, cprt = bingImg()
-        qs_default_console.print(qs_info_string, f"{'链接' if user_lang == 'zh' else 'LINK'}: {acg_link}") \
-            if status else qs_default_console.log(qs_error_string, acg_link)
+        qs_default_console.print(
+            qs_info_string, f"{'链接' if user_lang == 'zh' else 'LINK'}: {acg_link}"
+        ) if status else qs_default_console.log(qs_error_string, acg_link)
         if status:
-            qs_default_console.print(qs_info_string, '版权:' if user_lang == 'zh' else 'CPRT:', cprt)
-            if '--save' in sys.argv[2:]:
+            qs_default_console.print(
+                qs_info_string, "版权:" if user_lang == "zh" else "CPRT:", cprt
+            )
+            if "--save" in sys.argv[2:]:
                 from .NetTools.NormalDL import normal_dl
-                st.stop()
+
+                qs_default_status.stop()
                 acg_link = normal_dl(acg_link)
-            if system == 'darwin':  # Only support iTerm for Mac OS X
-                from .ImageTools.ImagePreview import image_preview
-                st.update(status='Loading image...' if user_lang != 'zh' else '加载图片中..')
-                image_preview(open(acg_link) if '--save' in sys.argv[2:] else acg_link,
-                              '--save' not in sys.argv[2:], qs_console_status=st)
+            from .ImageTools.ImagePreview import image_preview
+
+            qs_default_status.update(
+                status="Loading image..." if user_lang != "zh" else "加载图片中.."
+            )
+            image_preview(
+                open(acg_link) if "--save" in sys.argv[2:] else acg_link,
+                "--save" not in sys.argv[2:],
+            )
     except Exception as e:
         qs_default_console.print(qs_error_string, repr(e))
     finally:
-        st.stop()
+        qs_default_status.stop()
 
 
 def preview_html_images():
     """
     获取网页中图片链接（可在Mac::iTerm中自动预览）
 
     Get links to pictures in the web page (automatically previewed in Mac::iTerm)
 
     :return:
     """
     from .API.SimpleAPI import imgs_in_url
-    save_flag = '--save' in sys.argv
+
+    save_flag = "--save" in sys.argv
     if save_flag:
-        sys.argv.remove('--save')
+        sys.argv.remove("--save")
     for url in sys.argv[2:]:
         imgs_in_url(url, save_flag)
 
 
 def kdCheck():
     """
     查国内快递
 
     Check domestic express
 
     :return:
     """
-    from .API.alapi import kdCheck
+    from . import _ask
+    from .API.alapi import kdCheck as kdCheckAPI
 
-    with qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..'):
-        status, code, msg = kdCheck(sys.argv[2])
+    with qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中.."):
+        status, code, msg = kdCheckAPI(
+            sys.argv[2]
+            + (
+                ":"
+                + _ask(
+                    {
+                        "type": "input",
+                        "message": "顺丰快递需要输入手机后四位",
+                    }
+                )
+                if sys.argv[2][:2].lower() == "sf" and ':' not in sys.argv[2]
+                else ""
+            )
+        )
         if not status:
             qs_default_console.print(qs_error_string, msg)
             return
 
     from .TuiTools.Table import qs_default_table
     from . import table_cell
     from rich.text import Text
 
     width = qs_default_console.width // 4 * 3
     tb = qs_default_table(
         [
-            {'header': "Time" if user_lang != 'zh' else '时间', 'justify': "center", 'style': "bold cyan"},
-            {'header': "Description" if user_lang != 'zh' else '描述', 'justify': "center", 'no_wrap': False},
-            {'header': "Status" if user_lang != 'zh' else '状态', 'justify': "center"},
-        ], ([
-                '[bold underline red]Unknown:heavy_exclamation_mark:', '[bold underline yellow]In transit:airplane:',
-                '[bold underline green]In delivery:delivery_truck:', '[bold underline bold green]Signed receipt:hearts:'
-            ][code] if user_lang != 'zh' else [
-            '[bold underline red]未知:heavy_exclamation_mark:', '[bold underline yellow]运输中:airplane:',
-            '[bold underline green]派送中:delivery_truck:', '[bold underline magenta]已签收:hearts:'
-        ][code]) + '\n'
-    )
-    for info in msg[:-1] if code != 3 else msg:
-        tb.add_row(
-            info['time'], Text(table_cell(info['content'], width), justify='full')
-            , '[green]:heavy_check_mark:'
+            {
+                "header": "Time" if user_lang != "zh" else "时间",
+                "justify": "center",
+                "style": "bold cyan",
+            },
+            {
+                "header": "Description" if user_lang != "zh" else "描述",
+                "justify": "center",
+                "no_wrap": False,
+            },
+            {"header": "Status" if user_lang != "zh" else "状态", "justify": "center"},
+        ],
+        (
+            [
+                ":heavy_exclamation_mark: [bold underline red]Unknown",
+                ":airplane: [bold underline yellow]In transit",
+                ":delivery_truck: [bold underline green]In delivery",
+                ":hearts: [bold underline bold green]Signed receipt",
+            ][code]
+            if user_lang != "zh"
+            else [
+                ":heavy_exclamation_mark: [bold underline red]未知",
+                ":airplane: [bold underline yellow]运输中",
+                ":delivery_truck: [bold underline green]派送中",
+                ":hearts: [bold underline magenta]已签收:hearts:",
+            ][code]
         )
-    if code != 3:
+        + "\n",
+    )
+    for _id, info in enumerate(msg):
         tb.add_row(
-            msg[-1]['time'], Text(table_cell(msg[-1]['content'], width), justify='full')
-            , '[bold yellow]:arrow_left:'
+            info["time"],
+            Text(table_cell(info["content"], width), justify="full"),
+            "[bold green]:heavy_check_mark:" if _id else "[bold yellow]:arrow_left:",
         )
     qs_default_console.print(tb, justify="center")
 
 
 def loli():
     """
     获取一张"可爱"萝莉图的URL，Mac+iTerm2下可在终端预览
@@ -672,195 +696,220 @@
 
     :return:
     """
     from .API.Lolicon import loli_img
     from .ImageTools import ImagePreview
     from .NetTools import NormalDL
 
-    with qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..'):
+    with qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中.."):
         status, msg, data = loli_img()
         if not status:
             qs_default_console.print(qs_error_string, msg)
             return
 
-    save_flag = '--save' in sys.argv
-    proxy = ''
+    save_flag = "--save" in sys.argv
+    proxy = ""
 
-    if '-p' in sys.argv:
+    if "-p" in sys.argv:
         from . import qs_config
-        proxy = qs_config.basicSelect('default_proxy')
+
+        proxy = qs_config.basicSelect("default_proxy")
 
     for img in data:
-        qs_default_console.print(f'[bold underline]{img["title"]} [dim]{img["author"]}', justify="center")
-        qs_default_console.print(qs_info_string, '[bold]link' if user_lang != 'zh' else '[bold]链接', img['url'])
-        qs_default_console.print(qs_info_string, '[bold]size' if user_lang != 'zh' else '[bold]尺寸',
-                                 img['width'], 'x', img['height'])
+        qs_default_console.print(
+            f'[bold underline]{img["title"]} [dim]{img["author"]}', justify="center"
+        )
+        qs_default_console.print(
+            qs_info_string,
+            "[bold]link" if user_lang != "zh" else "[bold]链接",
+            img["url"],
+        )
+        qs_default_console.print(
+            qs_info_string,
+            "[bold]size" if user_lang != "zh" else "[bold]尺寸",
+            img["width"],
+            "x",
+            img["height"],
+        )
         if save_flag:
-            img['url'] = NormalDL.normal_dl(img['url'], set_proxy=proxy, set_referer='https://i.pximg.net')
-        if system == 'darwin':
-            ImagePreview.image_preview(open(img['url']) if save_flag else img['url'], not save_flag
-                                       , set_proxy=proxy, set_referer='https://i.pximg.net')
-
-        qs_default_console.print('-' * (qs_default_console.width // 4 * 3), justify='center')
+            img["url"] = NormalDL.normal_dl(
+                img["url"], set_proxy=proxy, set_referer="https://i.pximg.net"
+            )
+        if platform == "darwin":
+            ImagePreview.image_preview(
+                open(img["url"]) if save_flag else img["url"],
+                not save_flag,
+                set_proxy=proxy,
+                set_referer="https://i.pximg.net",
+            )
 
 
 def pinyin():
     from .API.alapi import pinyin
 
-    content = ' '.join(sys.argv[2:])
+    content = " ".join(sys.argv[2:])
     if not content:
         try:
-            pyperclip = requirePackage('pyperclip')
+            pyperclip = requirePackage("pyperclip")
             content = pyperclip.paste()
         except:
             from . import qs_default_input
+
             content = qs_default_input.ask(
-                'Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: '
-                if user_lang != 'zh' else '抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:')
-    with qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..') as st:
+                "Sorry, but your system is not supported by `pyperclip`\nSo you need input content manually: "
+                if user_lang != "zh"
+                else "抱歉，但是“pyperclip”不支持你的系统\n，所以你需要手动输入内容:"
+            )
+    with qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中.."):
         status, res = pinyin(content)
-        st.update(status='Done' if user_lang != 'zh' else '请求完成')
     qs_default_console.print(qs_info_string, content)
     qs_default_console.print(qs_info_string if status else qs_error_string, res)
 
 
 def setu():
     import random
+
     random.choice([acg, loli])()
 
 
 def exchange():
     from .API.alapi import exchange
 
-    st = qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..')
-    st.start()
+    qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中..").start()
     try:
-        status, data = exchange(sys.argv[3], float(sys.argv[2]))
-        qs_default_console.print(f"{sys.argv[2]} {sys.argv[3]} ==> {data['exchange']} × {sys.argv[2]} = "
-                                 f"{data['exchange_round']} {data['currency_to']}\n"
-                                 f"{'Update' if user_lang != 'zh' else '更新时间'}: {data['update_time']}",
-                                 justify="center") \
-            if status else qs_default_console.log(qs_error_string, data)
+        status, data = exchange(sys.argv[3], 1)
+        qs_default_console.print(
+            f"{sys.argv[2]} {sys.argv[3]} ==> {data['exchange']} × {sys.argv[2]} = "
+            f"{data['exchange'] * float(sys.argv[2])} {data['currency_to']}\n"
+            f"{'Update' if user_lang != 'zh' else '更新时间'}: {data['update_time']}",
+            justify="center",
+        ) if status else qs_default_console.log(qs_error_string, data)
     except Exception as e:
         qs_default_console.print(qs_error_string, repr(e))
     finally:
-        st.stop()
+        qs_default_status.stop()
 
 
 def zhihuDaily():
     from .API.alapi import zhihuDaily
     from rich.panel import Panel
     from .ImageTools.ImagePreview import image_preview
 
-    st = qs_default_console.status('Requesting data..' if user_lang != 'zh' else '请求数据中..')
-    st.start()
+    qs_default_status("Requesting data.." if user_lang != "zh" else "请求数据中..").start()
     try:
         status, data = zhihuDaily()
-        st.stop()
+        qs_default_status.stop()
         if not status:
             qs_default_console.log(qs_error_string, data)
             return
-        data = data['stories'] + data['top_stories']
+        data = data["stories"] + data["top_stories"]
         for item in data:
-            res = '[bold cyan]' + ('Author: ' if user_lang != 'zh' else '作者: ')
-            res += '[bold white]' + item['hint'] + '[/bold white]\n'
-            res += '[bold cyan]' + ('Link:' if user_lang != 'zh' else '链接: ')
-            res += '[bold blue]' + item['url'] + '[/bold blue]'
-            if 'images' in item:
-                if system == 'darwin':
-                    image_preview(item['images'][0], True)
+            res = "[bold cyan]" + ("Author: " if user_lang != "zh" else "作者: ")
+            res += "[bold white]" + item["hint"] + "[/bold white]\n"
+            res += "[bold cyan]" + ("Link:" if user_lang != "zh" else "链接: ")
+            res += "[bold blue]" + item["url"] + "[/bold blue]"
+            if "images" in item:
+                if platform == "darwin":
+                    image_preview(item["images"][0], True)
                 else:
-                    res += '\n[bold cyan]' + ('Image: \n' if user_lang != 'zh' else '图像: \n')
-                    res += '[bold blue]  ' + '\n  '.join(item['images'])
-            elif 'image' in item:
-                if system == 'darwin':
-                    image_preview(item['image'], True)
-                else:
-                    res += '\n[bold cyan]' + ('Image: \n' if user_lang != 'zh' else '图像: \n')
-                    res += '[bold blue]  ' + item['image']
-            qs_default_console.print(Panel(res, title='[b]' + item['title'], width=qs_default_console.width),
-                                     justify="center", end='/n/n')
+                    res += "\n[bold cyan]" + (
+                        "Image: \n" if user_lang != "zh" else "图像: \n"
+                    )
+                    res += "[bold blue]  " + "\n  ".join(item["images"])
+            elif "image" in item:
+                image_preview(item["image"], True)
+            qs_default_console.print(
+                Panel(res, title="[b]" + item["title"], width=qs_default_console.width),
+                justify="center",
+                end="/n/n",
+            )
     except Exception as e:
         qs_default_console.print(qs_error_string, repr(e))
     finally:
-        st.stop()
+        qs_default_status.stop()
 
 
 def wallhaven():
     from .API.SimpleAPI import wallhaven
 
-    url, oneFlag = '', False
-    if '-h' in sys.argv:
-        return qs_default_console.print(qs_info_string, "Usage: qs wallhaven [-open_url <url>] [-one] [-save]")
-
-    if '-open_url' in sys.argv:
-        url = sys.argv[sys.argv.index('-open_url') + 1]
-        sys.argv.remove('-open_url')
+    url, oneFlag = "", False
+    
+    if "--url" in sys.argv:
+        url = sys.argv[sys.argv.index("--url") + 1]
+        sys.argv.remove("--url")
         sys.argv.remove(url)
 
-    oneFlag = '-one' in sys.argv
+    oneFlag = "-one" in sys.argv
 
     res = wallhaven(randomOne=oneFlag) if not url else wallhaven(url, randomOne=oneFlag)
     if not res:
         return
 
-    if '--save' in sys.argv:
-        from .NetTools.NormalDL import normal_dl
-        import os
-        for i in res:
-            name = i['url'].split('/')[-1]
-            if os.path.exists(name):
-                qs_default_console.print(qs_warning_string,
-                                         f'{name} is exists!' if user_lang != 'zh' else f'{name} 已存在!')
-                continue
-            qs_default_console.print(qs_info_string, f"Deal:\t{name}")
-            qs_default_console.print(qs_info_string, f'Size:\t{" × ".join([str(j) for j in i["size"]])}')
-            normal_dl(i['url'], output_error=True, failed2exit=True)
-            qs_default_console.print('-' * qs_default_console.width)
+    if "--save" in sys.argv:
+        from .NetTools.MultiSingleDL import multi_single_dl
+
+        multi_single_dl([i["url"] for i in res], qps_info=5)
     else:
         if oneFlag:
             res = res[0]
-            qs_default_console.print(qs_info_string, 'URL:\t', res['url'])
-            qs_default_console.print(qs_info_string, 'SIZE:\t', ' × '.join([str(i) for i in res['size']]))
+            qs_default_console.print(qs_info_string, "URL:\t", res["url"])
+            qs_default_console.print(
+                qs_info_string, "SIZE:\t", " × ".join([str(i) for i in res["size"]])
+            )
             from .ImageTools.ImagePreview import image_preview
 
-            with qs_default_console.status('Getting..' if user_lang != 'zh' else '获取图片中..') as st:
-                image_preview(res['url'], True, qs_console_status=st)
+            with qs_default_status("Getting.." if user_lang != "zh" else "获取图片中.."):
+                image_preview(res["url"], True)
         else:
             from .TuiTools.Table import qs_default_table
 
-            tb = qs_default_table([
-                {'header': "ID" if user_lang != 'zh' else '编号', 'justify': "center", 'style': "bold"},
-                {'header': 'URL', 'justify': "center", 'style': "bold cyan"},
-                {'header': 'Size' if user_lang != 'zh' else '尺寸', 'justify': "center"}
-            ], 'Wallhaven Anime TopList\n')
+            tb = qs_default_table(
+                [
+                    {
+                        "header": "ID" if user_lang != "zh" else "编号",
+                        "justify": "center",
+                        "style": "bold",
+                    },
+                    {"header": "URL", "justify": "center", "style": "bold cyan"},
+                    {
+                        "header": "Size" if user_lang != "zh" else "尺寸",
+                        "justify": "center",
+                    },
+                ],
+                "Wallhaven Anime TopList\n",
+            )
             for iid, item in enumerate(res):
-                tb.add_row(str(iid), item['url'], ' × '.join([str(i) for i in item['size']]))
+                tb.add_row(
+                    str(iid), item["url"], " × ".join([str(i) for i in item["size"]])
+                )
             qs_default_console.print(tb, justify="center")
 
 
 def lmgtfy():
     from .API.SimpleAPI import lmgtfy
-    pyperclip = requirePackage('pyperclip')
 
-    keyword = ' '.join(sys.argv[2:])
+    pyperclip = requirePackage("pyperclip")
+
+    keyword = " ".join(sys.argv[2:])
     res = lmgtfy(keyword)
     try:
         pyperclip.copy(res)
         qs_default_console.print(
             qs_info_string,
-            'The generated link has been copied for you, and teach your friends how to use Google! (Can also Copy '
-            'Following link'
-            if user_lang != 'zh' else '已经为您复制生成的链接，快教朋友如何使用Google吧! (也可以复制下面的链接)'
+            "The generated link has been copied for you, and teach your friends how to use Google! (Can also Copy "
+            "Following link"
+            if user_lang != "zh"
+            else "已经为您复制生成的链接，快教朋友如何使用Google吧! (也可以复制下面的链接)",
         )
     except:
         qs_default_console.print(
             qs_warning_string,
-            'Failed to use clipboard, you can copy the flowing link:'
-            if user_lang != 'zh' else '调用剪切板失败，你可以复制下面的链接:'
+            "Failed to use clipboard, you can copy the flowing link:"
+            if user_lang != "zh"
+            else "调用剪切板失败，你可以复制下面的链接:",
         )
     qs_default_console.print(qs_info_string, res)
 
 
 def daily60s():
     from .API.alapi import daily60s
 
@@ -870,48 +919,59 @@
 
     from rich.padding import Padding
     import signal
     import time
 
     cur_index = 0
 
-    with qs_default_console.status('showing' if user_lang != 'zh' else '展示中') as st:
+    with qs_default_status("showing" if user_lang != "zh" else "展示中"):
+
         def dealSignal(*argv):
-            for index in range(cur_index + 1, len(res['news'])):
-                qs_default_console.print(Padding(res['news'][index], (0, int(0.2 * qs_default_console.width))))
+            for index in range(cur_index + 1, len(res["news"])):
+                qs_default_console.print(
+                    Padding(
+                        res["news"][index], (0, int(0.2 * qs_default_console.width))
+                    )
+                )
                 qs_default_console.print()
-            qs_default_console.print('-' * qs_default_console.width)
-            qs_default_console.print(res['weiyu'] + '\n', justify='center')
+            qs_default_console.print("-" * qs_default_console.width)
+            qs_default_console.print(res["weiyu"] + "\n", justify="center")
 
-            if '--save' in sys.argv:
+            if "--save" in sys.argv:
                 import os
                 from .NetTools.NormalDL import normal_dl
 
-                st.stop()
-                name = normal_dl(res['image'], set_name='news.png')
-                st.start()
-                if system == 'darwin':
-                    qs_default_console.print('Preview' if user_lang != 'zh' else '预览', justify='center')
-                    from .ImageTools.ImagePreview import image_preview
+                name = normal_dl(res["image"], set_name="news.png")
+                qs_default_console.print(
+                    "Preview" if user_lang != "zh" else "预览", justify="center"
+                )
+                from .ImageTools.ImagePreview import image_preview
 
-                    st.update(status='loading image..' if user_lang != 'zh' else '加载图片中..')
-                    image_preview(open(name), qs_console_status=st)
+                qs_default_status.update(
+                    status="loading image.." if user_lang != "zh" else "加载图片中.."
+                )
+                image_preview(open(name))
             exit(0)
 
         signal.signal(signal.SIGINT, dealSignal)
-        qs_default_console.print('[bold magenta underline]每天60秒读懂世界[/bold magenta underline]', justify='center')
-        qs_default_console.print(res['date'], justify='center')
-        qs_default_console.print('-' * qs_default_console.width)
-        len_ls = [len(i) for i in res['news']]
+        qs_default_console.print(
+            "[bold magenta underline]每天60秒读懂世界[/bold magenta underline]",
+            justify="center",
+        )
+        qs_default_console.print(res["date"], justify="center")
+        qs_default_console.print("-" * qs_default_console.width)
+        len_ls = [len(i) for i in res["news"]]
         total_len = sum(len_ls)
         len_ls = [i / total_len * 60 for i in len_ls]
         len_ls[-1] = 0
 
-        for index, item in enumerate(res['news']):
-            qs_default_console.print(Padding(item, (0, int(0.2 * qs_default_console.width))))
+        for index, item in enumerate(res["news"]):
+            qs_default_console.print(
+                Padding(item, (0, int(0.2 * qs_default_console.width)))
+            )
             qs_default_console.print()
             cur_index = index
             time.sleep(len_ls[index])
     dealSignal()
 
 
 def m2t():
@@ -919,76 +979,279 @@
     磁力链接转种子文件
 
     Magnet link to Torrent file
     :return:
     """
     import re
 
-    if '-f' in sys.argv:
-        file_path = sys.argv[sys.argv.index('-f') + 1]
-        with open(file_path, 'r') as f:
+    if "-f" in sys.argv:
+        file_path = sys.argv[sys.argv.index("-f") + 1]
+        with open(file_path, "r") as f:
             contents = f.read()
-    elif '-u' in sys.argv:
-        contents = sys.argv[sys.argv.index('-u') + 1]
+    elif "-u" in sys.argv:
+        contents = sys.argv[sys.argv.index("-u") + 1]
     else:
-        contents = requirePackage('pyperclip', 'paste')()
-    urls = re.findall('magnet:\?xt=urn:btih:(.*)', contents)
+        contents = requirePackage("pyperclip", "paste")()
+    urls = re.findall("magnet:\?xt=urn:btih:(.*)", contents)
     if len(urls) > 1:
-        from PyInquirer import prompt
-        url = prompt({
-            'type': 'list',
-            'name': 'hash',
-            'message': 'Select hash code | 选择哈希码:',
-            'choices': urls
-        })['hash']
+        from . import _ask
+
+        url = _ask(
+            {
+                "type": "list",
+                "message": "Select hash code | 选择哈希码:",
+                "choices": urls,
+            }
+        )
     else:
         url = urls[0]
     from .API.Lolicon import magnet2torrent
+
     magnet2torrent(url)
 
 
 def d2m():
     """
     番号搜索并复制磁力链
 
     :return:
     """
     global url
     try:
         designation = sys.argv[2]
     except IndexError:
-        return qs_default_console.print(qs_error_string, 'qs m2u <designation>')
+        return qs_default_console.print(qs_error_string, "qs d2m <designation>")
 
-    from PyInquirer import prompt
+    from . import _ask
     from .API.SimpleAPI import Designation2magnet
 
-    copy = requirePackage('pyperclip', 'copy', not_ask=True)
-    PyperclipException = requirePackage('pyperclip', 'PyperclipException')
+    copy = requirePackage("pyperclip", "copy", not_ask=True)
+    PyperclipException = requirePackage("pyperclip", "PyperclipException")
     copied = False
 
     searcher = Designation2magnet(designation)
     infos = searcher.search_designation()
-    choices = [f'[{n + 1}] ' + i[1] + ': ' + i[-1] for n, i in enumerate(infos)]
 
+    choices = [f"[{n + 1}] " + i[1] + ": " + i[-1] for n, i in enumerate(infos)]
     try:
         url = searcher.get_magnet(
-                infos[
-                    choices.index(prompt({
-                        'type': 'list',
-                        'message': 'Select | 选择',
-                        'name': 'sub-url',
-                        'choices': choices
-                    })['sub-url'])
-                ][0]
+            infos[
+                choices.index(
+                    _ask(
+                        {
+                            "type": "list",
+                            "message": "Select | 选择",
+                            "choices": choices,
+                        }
+                    )
+                )
+            ][0]
         )
         if copy:
             copy(url)
             copied = True
         else:
             raise PyperclipException
     except KeyError:
         return
     except PyperclipException:
         qs_default_console.print(qs_info_string, url)
 
     if copied:
-        qs_default_console.print(qs_info_string, 'magnet url copied to clipboard' if user_lang != 'zh' else '磁力链接已拷贝至粘贴板')
+        qs_default_console.print(
+            qs_info_string,
+            "magnet url copied to clipboard" if user_lang != "zh" else "磁力链接已拷贝至粘贴板",
+        )
+
+
+def doutu():
+    """
+    获取关键词的随机十张表情包
+    :return:
+    """
+    try:
+        keyword = sys.argv[2]
+    except IndexError:
+        return qs_default_console.print(qs_error_string, "qs doutu <keyword>")
+
+    from .API.alapi import doutu
+    from .ImageTools.ImagePreview import image_preview
+
+    status, urls = doutu(keyword)
+    if not status:
+        qs_default_console.print(qs_error_string, urls)
+    else:
+        import random
+
+        urls = random.choices(urls, k=10)
+
+        for item in urls:
+            qs_default_console.print(qs_info_string, item)
+            image_preview(item, is_url=True)
+
+
+def joke():
+    """
+    获取段子
+    :return:
+    """
+    import re
+    from .API.alapi import joke
+    from rich.panel import Panel
+
+    status, ct = joke()
+    if not status:
+        qs_default_console.print(qs_error_string, ct)
+        return
+    content = re.sub("&(.*?);", "", ct["content"])
+    qs_default_console.print(
+        Panel(
+            content,
+            title="[b magenta]" + ct["title"],
+            title_align="center",
+            width=qs_default_console.width,
+            subtitle=ct["time"],
+        )
+    )
+
+
+def gpt():
+    """
+    ChatGPT-3.5
+    :return:
+    """
+    translate_text = "--translate" in sys.argv
+    if translate_text:
+        from commonmark.blocks import Parser
+        from commonmark.render.rst import ReStructuredTextRenderer
+
+        parser = Parser()
+        sys.argv.remove("--translate")
+
+        class TranslateRenderer(ReStructuredTextRenderer):
+            def __init__(self):
+                super().__init__()
+
+            def text(self, node, entering):
+                self.out(translate(node.literal))
+
+            def link(self, node, entering):
+                if entering:
+                    self.out("[")
+                else:
+                    self.out("](%s)" % node.destination)
+
+            def image(self, node, entering):
+                if entering:
+                    self.out("![")
+                else:
+                    self.out(f"]({node.destination})")
+
+            def code(self, node, entering):
+                self.out("`")
+                self.out(node.literal)
+                self.out("`")
+
+            def code_block(self, node, entering):
+                directive = "```"
+                language_name = None
+
+                info_words = node.info.split() if node.info else []
+                if len(info_words) > 0 and len(info_words[0]) > 0:
+                    language_name = info_words[0]
+
+                if language_name:
+                    directive += language_name
+
+                self.cr()
+                self.out(directive)
+                self.cr()
+                self.out(node.literal)
+                self.out("```")
+                self.cr()
+
+            def heading(self, node, entering):
+                if entering:
+                    self.cr()
+                    self.out("#" * node.level)
+                    self.out(" ")
+                else:
+                    self.cr()
+
+        render = TranslateRenderer()
+
+    from rich.markdown import Markdown
+    from rich.live import Live
+    from .API.ChatGPT import chatGPT, API_KEY, ALAPI
+    from . import _ask
+    from .NumbaTools import cut_string
+
+    qs_default_console.print(
+        qs_info_string, "Type 'exit' to exit" if user_lang != "zh" else "输入 'exit' 退出"
+    )
+
+    if not translate_text:
+        qs_default_console.print(
+            qs_info_string,
+            "Add '--translate' to enable auto translate"
+            if user_lang != "zh"
+            else "添加 '--translate' 以启用自动翻译",
+        )
+
+    record = ""
+
+    while (
+        prompt := _ask(
+            {
+                "type": "input",
+                "message": "Input Question" if user_lang != "zh" else "输入问题",
+            }
+        )
+    ) != "exit":
+        if translate_text:
+            prompt = translate(prompt, target_lang="en")
+            qs_default_console.print("EN:", prompt)
+
+        with qs_default_status("Thinking..." if user_lang != "zh" else "思考中..."):
+            response = chatGPT(prompt)
+
+        qs_default_console.print(
+            "[bold green]" + ("Answer" if user_lang != "zh" else "回答") + "[/]\n",
+            justify="center",
+        )
+        prefix = "" if prompt not in ["继续", "continue"] else record
+
+        with Live(
+            "",
+            console=qs_default_console,
+            auto_refresh=False,
+            vertical_overflow="visible",
+        ) as live:
+            total_res = prefix
+            for res in response:
+                if API_KEY or ALAPI:
+                    if ALAPI:  # ALAPI 优先启用
+                        total_res = prefix + res
+                    elif API_KEY:
+                        total_res += res
+                else:
+                    total_res = prefix + res["message"]
+                display = "\n".join(
+                    [
+                        " ".join(
+                            cut_string(
+                                line, qs_default_console.width, ignore_charset="`"
+                            )
+                        )
+                        for line in total_res.split("\n")
+                    ]
+                )
+                live.update(Markdown(display, justify="full"), refresh=True)
+            record = total_res
+            if (
+                translate_text
+                and requirePackage("langid", "classify")(total_res)[0] != user_lang
+            ):
+                live.update(
+                    Markdown(render.render(parser.parse(total_res)), justify="full"),
+                    refresh=True,
+                )
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/imageDeal.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,162 +11,196 @@
 
 def set_img_background():
     """替换图片颜色 | Replace color in image"""
     from .ImageTools.ColorTools import transport_back, get_color_from_str
 
     try:
         img = sys.argv[2]
-        if img == '-help':
+        if img == "-help":
             raise IndexError
         if not os.path.exists(img):
-            qs_default_console.log(qs_error_string, 'No Such File: %s' % img)
+            qs_default_console.log(qs_error_string, "No Such File: %s" % img)
             return
         to = sys.argv[3]
         try:
             frm = sys.argv[4]
         except IndexError:
-            frm = '0,0,0,0'
+            frm = "0,0,0,0"
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs stbg <picture> <to_color> [from_color: default transparency]')
+        qs_default_console.log(
+            qs_error_string,
+            "Usage: qs stbg <picture> <to_color> [from_color: default transparency]",
+        )
         return
     else:
         to = get_color_from_str(to)
         frm = get_color_from_str(frm)
         img = transport_back(img, to, frm)
-        iname = sys.argv[2].split('.')
-        iname = iname[0] + '_stbg.' + ''.join(iname[1:])
+        iname = sys.argv[2].split(".")
+        iname = iname[0] + "_stbg." + "".join(iname[1:])
         img.save(iname)
 
 
 def fmt_img_color():
     from .ImageTools.ColorTools import formatOneColor, get_color_from_str
 
     try:
         img = sys.argv[2]
-        if img == '-help':
+        if img == "-help":
             raise IndexError
         if not os.path.exists(img):
-            qs_default_console.log(qs_error_string, 'No Such File: %s' % img)
+            qs_default_console.log(qs_error_string, "No Such File: %s" % img)
             return
         to = sys.argv[3]
         try:
             exp = sys.argv[4:]
         except IndexError:
-            exp = '0,0,0,0'
+            exp = "0,0,0,0"
     except IndexError:
-        qs_default_console.log(qs_error_string,
-                               'Usage: qs fmti <picture> <to_color> [except_color: default transparency]')
+        qs_default_console.log(
+            qs_error_string,
+            "Usage: qs fmti <picture> <to_color> [except_color: default transparency]",
+        )
         return
     else:
         to = get_color_from_str(to)
         exp = [get_color_from_str(i) for i in exp]
         img = formatOneColor(img, to, exp)
-        iname = sys.argv[2].split('.')
-        iname = iname[0] + '_fmt.' + ''.join(iname[1:])
+        iname = sys.argv[2].split(".")
+        iname = iname[0] + "_fmt." + "".join(iname[1:])
         img.save(iname)
 
 
 def v2gif():
     """视频转gif | video to gif"""
     from .ImageTools.VideoTools import video_2_gif
 
     try:
         video = sys.argv[2]
         sz, fps = None, None
         if len(sys.argv) > 3:
             for i in sys.argv[3:]:
                 try:
-                    if ',' in i:
-                        sz = tuple([int(j) for j in i.split(',')])
+                    if "," in i:
+                        sz = tuple([int(j) for j in i.split(",")])
                     else:
                         fps = int(i)
                 except:
                     raise IndexError
-        sz = tuple([int(i) for i in sys.argv[3].split(',')]) if len(sys.argv) > 3 and ',' in sys.argv[3] else None
-    except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs v2gif <*.mp4> [width,height] [fps]')
+        sz = (
+            tuple([int(i) for i in sys.argv[3].split(",")])
+            if len(sys.argv) > 3 and "," in sys.argv[3]
+            else None
+        )
+    except IndexError:
+        qs_default_console.log(
+            qs_error_string, "Usage: qs v2gif <*.mp4> [width,height] [fps]"
+        )
         return
     else:
-        video_2_gif(video, sz, fps) if sz and fps else video_2_gif(video, sz) \
-            if sz else video_2_gif(video, fps=fps) if fps else video_2_gif(video)
+        video_2_gif(video, sz, fps) if sz and fps else video_2_gif(
+            video, sz
+        ) if sz else video_2_gif(video, fps=fps) if fps else video_2_gif(video)
 
 
 def remove_audio():
     """删除视频的音频 | remove audio in mp4"""
     from .ImageTools.VideoTools import rm_audio
+
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs rmaudio <video...>')
+        qs_default_console.log(qs_error_string, "Usage: qs rmaudio <video...>")
     else:
         for video in videos:
             rm_audio(video)
 
 
 def v2mp4():
     """视频转mp4 | transfer video to mp4"""
     from .ImageTools.VideoTools import tomp4
+
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs v2mp4 <video...>')
+        qs_default_console.log(qs_error_string, "Usage: qs v2mp4 <video...>")
     else:
         for video in videos:
             tomp4(video)
 
 
 def v2mp3():
     """提取视频音频为mp3 | Extract the audio from the video and save it in MP3 format"""
     from .ImageTools.VideoTools import video_2_mp3
+
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs v2mp3 <video...>')
+        qs_default_console.log(qs_error_string, "Usage: qs v2mp3 <video...>")
     else:
         for video in videos:
             video_2_mp3(video)
 
 
 def icat():
     """Mac::iTerm下预览图片 | Preview the picture under Mac::iTerm"""
     try:
         path = sys.argv[2]
-        is_url = '-open_url' in sys.argv or \
-                 (not os.path.exists(path) and (path.startswith('http://') or path.startswith('https://')))
+        is_url = "-u" in sys.argv or (
+            not os.path.exists(path)
+            and (path.startswith("http://") or path.startswith("https://"))
+        )
+        is_in_rc_file = "--rc" in sys.argv
+        if is_in_rc_file:
+            rc_width = int(sys.argv[sys.argv.index("--rc") + 1])
+        else:
+            rc_width = 0
         if not os.path.exists(path) and not is_url:
-            qs_default_console.log(qs_error_string, 'No such file:', path)
+            qs_default_console.log(qs_error_string, "No such file:", path)
             raise FileNotFoundError
     except:
-        qs_default_console.log(qs_error_string, 'Usage: qs icat <img path/url> [-open_url if is url]')
+        qs_default_console.log(
+            qs_error_string, "Usage: qs icat <img path/url> [-u if is url]"
+        )
     else:
         from .ImageTools.ImagePreview import image_preview
-        image_preview(open(path)) if not is_url else image_preview(path, is_url)
+
+        image_preview(
+            path, set_width_in_rc_file=rc_width, force_show=True
+        ) if not is_url else image_preview(
+            path, is_url, set_width_in_rc_file=rc_width, force_show=True
+        )
 
 
 def i2png():
     try:
         imgs = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs i2png <imgs...>')
+        qs_default_console.log(qs_error_string, "Usage: qs i2png <imgs...>")
     else:
         from .ImageTools.ImageTools import topng
+
         for imgPath in imgs:
             topng(imgPath)
 
 
 def i2jpg():
     try:
         imgs = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, 'Usage: qs i2jpg <imgs...>')
+        qs_default_console.log(qs_error_string, "Usage: qs i2jpg <imgs...>")
     else:
         from .ImageTools.ImageTools import tojpg
+
         for imgPath in imgs:
             tojpg(imgPath)
 
 
 def vsta():
     from .ImageTools.VideoTools import set_video_audio
+
     try:
         set_video_audio(*sys.argv[2:])
     except Exception as e:
-        qs_default_console.log(qs_error_string, f'{repr(e)}\nUsage: qs vsta <video> <audio>')
+        qs_default_console.log(
+            qs_error_string, f"{repr(e)}\nUsage: qs vsta <video> <audio>"
+        )
```

### Comparing `QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py` & `quickstart_rhy-0.7.1/QuickStart_Rhy/system.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,255 +2,309 @@
 """
 调用各种系统工具
 
 Call various system tools
 """
 import QuickStart_Rhy.Wrapper as _wrapper
 
-miss_file = ['.DS_Store']
+miss_file = [".DS_Store"]
 
 
 def __latest_filename(name):
     import os
-    from . import dir_char
 
     cur = os.getcwd()
-    rec = cur
-    while cur != dir_char:
-        if os.path.exists(name):
-            os.chdir(rec)
-            return cur + dir_char + name
-        os.chdir('..')
-        cur = os.getcwd()
-    os.chdir(rec)
-    return ''
+    while cur != os.path.dirname(cur):
+        if os.path.exists(os.path.join(cur, name)):
+            return os.path.join(cur, name)
+        cur = os.path.dirname(cur)
+    return os.path.join(cur, name) if os.path.exists(os.path.join(cur, name)) else ""
 
 
 def top():
     """
     CPU和内存监测
 
     CPU and memory monitoring
 
     :return: None
     """
-    from . import dir_char
-    if dir_char == '\\':
-        from .SystemTools.Monitor import top
-        top()
-    else:
-        import sys
-        sys.argv = ['bpytop'] + sys.argv[2:]
+    import sys
+
+    sys.argv = ["bpytop"] + sys.argv[2:]
+
+    from . import requirePackage
 
-        from . import requirePackage
-        requirePackage('bpytop', 'main')()
+    requirePackage("bpytop", "main")()
 
 
 def clear_mem():
     """
     清理系统内存
 
     Clean system memory
 
     :return: None
     """
     from .SystemTools import clear_mem
+
     clear_mem()
 
 
 def go_github():
     """
     自动识别当前文件夹.git/config中的地址，并通过浏览器打开
 
     Automatically recognize the address in the current folder .git/config and open it through a browser
     """
     import os
-    from . import qs_default_console, qs_error_string, user_lang, open_url, requirePackage
+    from . import (
+        qs_default_console,
+        qs_error_string,
+        user_lang,
+        open_url,
+        requirePackage,
+    )
 
-    config_path = __latest_filename('.git/config')
+    config_path = __latest_filename(".git/config")
     if not os.path.exists(config_path):
-        qs_default_console.print(qs_error_string, 'No a git dictionary' if user_lang != 'zh' else '不是 git 文件夹')
+        qs_default_console.print(
+            qs_error_string,
+            "No a git dictionary" if user_lang != "zh" else "不是 git 文件夹",
+        )
         return
-    config = requirePackage('configparser', 'ConfigParser')()
+    config = requirePackage("configparser", "ConfigParser")()
     config.read(filenames=config_path)
     url_ls = []
     for section in config.sections():
-        if section.startswith('remote'):
-            url_ls.append(config[section]['url'].replace('.git', ''))
+        if section.startswith("remote"):
+            url_ls.append(config[section]["url"].replace(".git", ""))
     open_url(url_ls)
 
 
-@_wrapper.mkCompressPackageWrap
-def _mktar(file_path: str = ''):
-    from .SystemTools.Compress import Tar
-    return Tar(file_path + '.tar.gz', 'w')
-
-
 def mktar():
     """
     创建tar包
 
     Create a tar packages
 
     :return: None
     """
-    return _mktar()
 
+    @_wrapper.mkCompressPackageWrap
+    def _mktar(file_path: str = ""):
+        from .SystemTools.Compress import Tar
 
-@_wrapper.unCompressPackageWrap
-def _untar(file_path: str = ''):
-    from .SystemTools.Compress import Tar
-    return Tar(file_path)
+        return Tar(file_path + ".tar.gz", "w")
+
+    return _mktar()
 
 
 def untar():
     """
     解压tar包
 
     Unpack the tar packages
 
     :return: None
     """
-    return _untar()
 
+    @_wrapper.unCompressPackageWrap
+    def _untar(file_path: str = ""):
+        from .SystemTools.Compress import Tar
 
-@_wrapper.mkCompressPackageWrap
-def _mkzip(file_path: str = ''):
-    from .SystemTools.Compress import Zip
-    return Zip(file_path + '.zip', 'w')
+        return Tar(file_path)
+
+    return _untar()
 
 
 def mkzip():
     """
     创建ZIP包
 
     Create a ZIP package
 
     :return: None
     """
-    return _mkzip()
 
+    @_wrapper.mkCompressPackageWrap
+    def _mkzip(file_path: str = ""):
+        from .SystemTools.Compress import Zip
 
-@_wrapper.unCompressPackageWrap
-def _unzip(file_path: str = ''):
-    from .SystemTools.Compress import Zip
-    return Zip(file_path, 'r')
+        return Zip(file_path + ".zip", "w")
+
+    return _mkzip()
 
 
 def unzip():
     """
     解压ZIP包
 
     Unpack the ZIP package
 
     :return: None
     """
-    return _unzip()
 
+    @_wrapper.unCompressPackageWrap
+    def _unzip(file_path: str = ""):
+        from .SystemTools.Compress import Zip
+
+        return Zip(file_path, "r")
 
-@_wrapper.unCompressPackageWrap
-def _unrar(file_path: str = ''):
-    from .SystemTools.Compress import Rar
-    return Rar(file_path)
+    return _unzip()
 
 
 def unrar():
     """
     解压RAR包
 
     Extract RAR package
 
     :return: None
     """
-    return _unrar()
 
+    @_wrapper.unCompressPackageWrap
+    def _unrar(file_path: str = ""):
+        from .SystemTools.Compress import Rar
 
-@_wrapper.mkCompressPackageWrap
-def _mk7z(file_path: str = ''):
-    from .SystemTools.Compress import SevenZip
-    return SevenZip(file_path + '.7z', 'w')
+        return Rar(file_path)
+
+    return _unrar()
 
 
 def mk7z():
     """
     创建7z包
 
     Create 7z package
 
     :return: None
     """
-    return _mk7z()
 
+    @_wrapper.mkCompressPackageWrap
+    def _mk7z(file_path: str = ""):
+        from .SystemTools.Compress import SevenZip
 
-@_wrapper.unCompressPackageWrap
-def _un7z(file_path: str = ''):
-    from .SystemTools.Compress import SevenZip
-    return SevenZip(file_path)
+        return SevenZip(file_path + ".7z", "w")
+
+    return _mk7z()
 
 
 def un7z():
     """
     解压7z包
 
     Extract 7z package
 
     :return:
     """
+
+    @_wrapper.unCompressPackageWrap
+    def _un7z(file_path: str = ""):
+        from .SystemTools.Compress import SevenZip
+
+        return SevenZip(file_path)
+
     return _un7z()
 
 
-@_wrapper.HashWrapper('md5')
+@_wrapper.HashWrapper()
 def md5():
     """
     获取文件md5值
     :return:
     """
 
 
-@_wrapper.HashWrapper('sha1')
+@_wrapper.HashWrapper()
 def sha1():
     """
     获取文件sha1值
     :return:
     """
 
 
-@_wrapper.HashWrapper('sha256')
+@_wrapper.HashWrapper()
 def sha256():
     """
     获取文件sha256值
     :return:
     """
 
 
-@_wrapper.HashWrapper('sha512')
+@_wrapper.HashWrapper()
 def sha512():
     """
     获取文件sha512值
     :return:
     """
 
 
 def diff_dir():
     """
     对比两个文件夹差异，并生成相应html对比结果
     :return:
     """
-    from . import user_lang, qs_default_console, qs_info_string
+    from . import user_lang, qs_default_console, qs_info_string, qs_default_status
     from .SystemTools.Diff import DictionaryFiles
     import sys
 
-    if '-h' in sys.argv:
-        qs_default_console.print(qs_info_string, 'Usage: qs diff <dir1> <dir2> [-x <name or regex pattern>]')
+    if "-h" in sys.argv:
+        qs_default_console.print(
+            qs_info_string, "Usage: qs diff <dir1> <dir2> [-x <name or regex pattern>]"
+        )
 
     d1, d2 = sys.argv[2:4]
-    apply_ignore = sys.argv[sys.argv.index('-x') + 1:] if '-x' in sys.argv else None
+    apply_ignore = sys.argv[sys.argv.index("-x") + 1 :] if "-x" in sys.argv else None
     d1 = DictionaryFiles(d1, apply_ignore)
     d2 = DictionaryFiles(d2, apply_ignore)
 
     if not (d1.available and d2.available):
         return
 
-    with qs_default_console.status('Generating diff result..' if user_lang != 'zh' else '生成对比结果中..'):
+    with qs_default_status(
+        "Generating diff result.." if user_lang != "zh" else "生成对比结果中.."
+    ):
         from .SystemTools.Diff import DiffFilesToStructHtml
 
         DiffFilesToStructHtml(d1, d2).generate()
+
+
+def mount_dmg():
+    """
+    挂载镜像 
+
+    :return:
+    """
+    from .SystemTools.DiskMac import DMG
+    import sys
+
+    DMG().mount(sys.argv[2])
+
+
+def unmount_dmg():
+    """
+    卸载镜像
+    """
+    from .SystemTools.DiskMac import DMG
+    from .TuiTools.Table import qs_default_table
+    from . import qs_default_console, user_lang, qs_info_string, _ask
+
+    disks = DMG()
+    _ls = disks.get_disk_list()[2:]
+    if not _ls:
+        return qs_default_console.print(
+            qs_info_string, "No DMG disk found" if user_lang != "zh" else "没有找到 dmg 磁盘"
+        )
+    table = qs_default_table(["Disk", "Type", "Size"])
+    for disk in _ls:
+        table.add_row(disk["path"], disk["type"], disk["size"])
+    qs_default_console.print(table, justify="center")
+    disk_paths = _ask(
+        {
+            "type": "checkbox",
+            "message": "Select a disk to umount" if user_lang != "zh" else "选择要卸载的磁盘",
+            "choices": [{'name': disk["path"], 'checked': True} for disk in _ls],
+        }
+    )
+    for disk_path in disk_paths:
+        disks.unmount(disk_path)
```

