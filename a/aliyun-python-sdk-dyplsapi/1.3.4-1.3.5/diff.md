# Comparing `tmp/aliyun-python-sdk-dyplsapi-1.3.4.tar.gz` & `tmp/aliyun-python-sdk-dyplsapi-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dyplsapi-1.3.4.tar", last modified: Fri Feb 24 09:21:35 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dyplsapi-1.3.5.tar", last modified: Thu May  4 02:41:29 2023, max compression
```

## Comparing `aliyun-python-sdk-dyplsapi-1.3.4.tar` & `aliyun-python-sdk-dyplsapi-1.3.5.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2153 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/
--rw-r--r--   0 root         (0) root         (0)     2601 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/AddAxnTrackNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/AddSecretBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     4967 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxbRequest.py
--rw-r--r--   0 root         (0) root         (0)     4750 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxgRequest.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxnExtensionRequest.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxnRequest.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BuySecretNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CancelPickUpWaybillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreateAxgGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2701 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillPreQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     4745 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillRequest.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/DeleteSecretBlacklistRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/GetSecretAsrDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/GetTotalPublicUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/LockSecretNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/OperateAxgGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/OperateBlackNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QueryPhoneNoAByTrackNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2651 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QueryRecordFileDownloadUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoRemainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySubsIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySubscriptionDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/ReleaseSecretNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2635 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UnbindSubscriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UnlockSecretNoRequest.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UpdateSubscriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-02-24 09:21:35.000000 aliyun-python-sdk-dyplsapi-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/AddAxnTrackNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/AddSecretBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4967 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxgRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxnExtensionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxnRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindBatchAxgRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BuySecretNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CancelPickUpWaybillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreateAxgGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillPreQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4745 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/DeleteAxgGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/DeleteSecretBlacklistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/GetSecretAsrDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/GetTotalPublicUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/LockSecretNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/OperateAxgGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/OperateBlackNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QueryPhoneNoAByTrackNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QueryRecordFileDownloadUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoRemainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySubsIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySubscriptionDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/ReleaseSecretNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UnbindSubscriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UnlockSecretNoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UpdateSubscriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-04 02:41:29.000000 aliyun-python-sdk-dyplsapi-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-04 02:41:28.000000 aliyun-python-sdk-dyplsapi-1.3.5/setup.py
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/LICENSE` & `aliyun-python-sdk-dyplsapi-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/PKG-INFO` & `aliyun-python-sdk-dyplsapi-1.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dyplsapi
-Version: 1.3.4
+Version: 1.3.5
 Summary: The dyplsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dyplsapi
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/README.rst` & `aliyun-python-sdk-dyplsapi-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/PKG-INFO` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dyplsapi
-Version: 1.3.4
+Version: 1.3.5
 Summary: The dyplsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dyplsapi
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyun_python_sdk_dyplsapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyun_python_sdk_dyplsapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 aliyunsdkdyplsapi/request/__init__.py
 aliyunsdkdyplsapi/request/v20170525/AddAxnTrackNoRequest.py
 aliyunsdkdyplsapi/request/v20170525/AddSecretBlacklistRequest.py
 aliyunsdkdyplsapi/request/v20170525/BindAxbRequest.py
 aliyunsdkdyplsapi/request/v20170525/BindAxgRequest.py
 aliyunsdkdyplsapi/request/v20170525/BindAxnExtensionRequest.py
 aliyunsdkdyplsapi/request/v20170525/BindAxnRequest.py
+aliyunsdkdyplsapi/request/v20170525/BindBatchAxgRequest.py
 aliyunsdkdyplsapi/request/v20170525/BuySecretNoRequest.py
 aliyunsdkdyplsapi/request/v20170525/CancelPickUpWaybillRequest.py
 aliyunsdkdyplsapi/request/v20170525/CreateAxgGroupRequest.py
 aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillPreQueryRequest.py
 aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillRequest.py
+aliyunsdkdyplsapi/request/v20170525/DeleteAxgGroupRequest.py
 aliyunsdkdyplsapi/request/v20170525/DeleteSecretBlacklistRequest.py
 aliyunsdkdyplsapi/request/v20170525/GetSecretAsrDetailRequest.py
 aliyunsdkdyplsapi/request/v20170525/GetTotalPublicUrlRequest.py
 aliyunsdkdyplsapi/request/v20170525/LockSecretNoRequest.py
 aliyunsdkdyplsapi/request/v20170525/OperateAxgGroupRequest.py
 aliyunsdkdyplsapi/request/v20170525/OperateBlackNoRequest.py
 aliyunsdkdyplsapi/request/v20170525/QueryPhoneNoAByTrackNoRequest.py
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/endpoint.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/AddAxnTrackNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/AddAxnTrackNoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/AddSecretBlacklistRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/AddSecretBlacklistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxbRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxgRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxgRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxnExtensionRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxnExtensionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BindAxnRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BindAxnRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/BuySecretNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/BuySecretNoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CancelPickUpWaybillRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CancelPickUpWaybillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreateAxgGroupRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreateAxgGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillPreQueryRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillPreQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/CreatePickUpWaybillRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/DeleteSecretBlacklistRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/DeleteSecretBlacklistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/GetSecretAsrDetailRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/GetSecretAsrDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/GetTotalPublicUrlRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/GetTotalPublicUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/LockSecretNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/LockSecretNoRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_SecretNo(self): # String
+		return self.get_query_params().get('SecretNo')
+
+	def set_SecretNo(self, SecretNo):  # String
+		self.add_query_param('SecretNo', SecretNo)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
@@ -47,12 +52,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_PoolKey(self): # String
 		return self.get_query_params().get('PoolKey')
 
 	def set_PoolKey(self, PoolKey):  # String
 		self.add_query_param('PoolKey', PoolKey)
-	def get_SecretNo(self): # String
-		return self.get_query_params().get('SecretNo')
-
-	def set_SecretNo(self, SecretNo):  # String
-		self.add_query_param('SecretNo', SecretNo)
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/OperateAxgGroupRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/OperateAxgGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/OperateBlackNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/OperateBlackNoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QueryPhoneNoAByTrackNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QueryPhoneNoAByTrackNoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QueryRecordFileDownloadUrlRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QueryRecordFileDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoDetailRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoRemainRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySecretNoRemainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySubsIdRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySubsIdRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_PhoneNoX(self): # String
+		return self.get_query_params().get('PhoneNoX')
+
+	def set_PhoneNoX(self, PhoneNoX):  # String
+		self.add_query_param('PhoneNoX', PhoneNoX)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
@@ -47,12 +52,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_PoolKey(self): # String
 		return self.get_query_params().get('PoolKey')
 
 	def set_PoolKey(self, PoolKey):  # String
 		self.add_query_param('PoolKey', PoolKey)
-	def get_PhoneNoX(self): # String
-		return self.get_query_params().get('PhoneNoX')
-
-	def set_PhoneNoX(self, PhoneNoX):  # String
-		self.add_query_param('PhoneNoX', PhoneNoX)
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/QuerySubscriptionDetailRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/QuerySubscriptionDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/ReleaseSecretNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/ReleaseSecretNoRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_SecretNo(self): # String
+		return self.get_query_params().get('SecretNo')
+
+	def set_SecretNo(self, SecretNo):  # String
+		self.add_query_param('SecretNo', SecretNo)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
@@ -47,12 +52,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_PoolKey(self): # String
 		return self.get_query_params().get('PoolKey')
 
 	def set_PoolKey(self, PoolKey):  # String
 		self.add_query_param('PoolKey', PoolKey)
-	def get_SecretNo(self): # String
-		return self.get_query_params().get('SecretNo')
-
-	def set_SecretNo(self, SecretNo):  # String
-		self.add_query_param('SecretNo', SecretNo)
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UnbindSubscriptionRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UnbindSubscriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UnlockSecretNoRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UnlockSecretNoRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_SecretNo(self): # String
+		return self.get_query_params().get('SecretNo')
+
+	def set_SecretNo(self, SecretNo):  # String
+		self.add_query_param('SecretNo', SecretNo)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
@@ -47,12 +52,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_PoolKey(self): # String
 		return self.get_query_params().get('PoolKey')
 
 	def set_PoolKey(self, PoolKey):  # String
 		self.add_query_param('PoolKey', PoolKey)
-	def get_SecretNo(self): # String
-		return self.get_query_params().get('SecretNo')
-
-	def set_SecretNo(self, SecretNo):  # String
-		self.add_query_param('SecretNo', SecretNo)
```

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/aliyunsdkdyplsapi/request/v20170525/UpdateSubscriptionRequest.py` & `aliyun-python-sdk-dyplsapi-1.3.5/aliyunsdkdyplsapi/request/v20170525/UpdateSubscriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dyplsapi-1.3.4/setup.py` & `aliyun-python-sdk-dyplsapi-1.3.5/setup.py`

 * *Files identical despite different names*

