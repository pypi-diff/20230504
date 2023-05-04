# Comparing `tmp/krutils-0.20230411.1644.tar.gz` & `tmp/krutils-0.20230504.1600.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1644.tar", last modified: Tue Apr 11 07:44:07 2023, max compression
+gzip compressed data, was "krutils-0.20230504.1600.tar", last modified: Thu May  4 07:00:14 2023, max compression
```

## Comparing `krutils-0.20230411.1644.tar` & `krutils-0.20230504.1600.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.288281 krutils-0.20230411.1644/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:44:07.283490 krutils-0.20230411.1644/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1644/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.134510 krutils-0.20230411.1644/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1644/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230411.1644/krutils/CONST.py
--rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230411.1644/krutils/__init__.py
--rw-rw-rw-   0        0        0     5528 2023-04-11 07:31:01.000000 krutils-0.20230411.1644/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0    33519 2023-04-11 07:31:30.000000 krutils-0.20230411.1644/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.278313 krutils-0.20230411.1644/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:44:07.288281 krutils-0.20230411.1644/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-04-11 07:44:05.000000 krutils-0.20230411.1644/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:00:14.493073 krutils-0.20230504.1600/
+-rw-rw-rw-   0        0        0      526 2023-05-04 07:00:14.488692 krutils-0.20230504.1600/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230504.1600/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 07:00:14.286692 krutils-0.20230504.1600/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230504.1600/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230504.1600/krutils/CONST.py
+-rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230504.1600/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230504.1600/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    33617 2023-05-04 06:39:56.000000 krutils-0.20230504.1600/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:00:14.482198 krutils-0.20230504.1600/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-04 07:00:13.000000 krutils-0.20230504.1600/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-04 07:00:13.000000 krutils-0.20230504.1600/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:00:13.000000 krutils-0.20230504.1600/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 07:00:13.000000 krutils-0.20230504.1600/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 07:00:13.000000 krutils-0.20230504.1600/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:00:14.493073 krutils-0.20230504.1600/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-04 07:00:11.000000 krutils-0.20230504.1600/setup.py
```

### Comparing `krutils-0.20230411.1644/krutils/CONST.py` & `krutils-0.20230504.1600/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1644/krutils/_dbmgr.py` & `krutils-0.20230504.1600/krutils/_dbmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 import os
 import pymysql
 from pymysql import Connection
 import utils
 
-print (utils.__file__)
-logger = utils.logger(__file__)
 
 
 
 # SQL PARAM 형식
 SQL_PARAM_PATTERN = "#\\{\\D[\\w]*\\}";
 
 # SELECT 기본 MAX 건수 : 500 (DBIO 조회 기본값)
```

### Comparing `krutils-0.20230411.1644/krutils/utils.py` & `krutils-0.20230504.1600/krutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,18 +522,20 @@
 
 
 
 ##########################################
 ##      FILE, DIRECTORIES
 ##########################################
 
-def find_first_file_to_root(file_name: str) -> str:
+def get_file_path_fr(file_name: str) -> str:
     '''
-    file_name을 최상위 디렉토리까지 올라가며 찾는다.
-    첫번째 확인된 경로를 리턴한다.
+    ```config_file_path = get_file_path_ftr('config.json')```
+    > get file path following through root
+    > file_name을 최상위 디렉토리까지 올라가며 찾는다.
+    > 첫번째 확인된 경로를 리턴한다.
     '''
     if is_empty(file_name):
         raise Exception('찾고자하는 파일명을 입력해 주세요')
 
     import os
 
     curr_dir = os.path.dirname(__file__)
@@ -583,26 +585,26 @@
 
 ##########################################
 ##      JSON
 ##########################################
 
 
 
-def get_json_as_dic(file_path=None) -> dict():
+def get_json_as_dic(file_path=None) -> dict:
     '''
        "xxx.json"  file을 읽어 dict형태로 반환한다.
 
        ex> get_json_file("./config/setting.json")
     '''
 
     # do something
     pass
 
 
-def is_connectable_internet() -> bool():
+def is_connectable_internet() -> bool:
 
     if (checkInternetHttplib() == True or
             checkInternetSocket() == True):
         return True
 
     else:
         return False
@@ -634,15 +636,15 @@
         return True
 
     except socket.error as ex:
         # print(ex)
         return False
 
 
-def get_katis_env() -> dict():
+def get_katis_env() -> dict:
 
     # 실행환경 설정 파일 읽기
     katis_file_path = get_katis_config_file_path()
 
     if (len(katis_file_path) == 0):
         return False
```

