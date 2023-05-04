# Comparing `tmp/pitricks-0.1.3a3.tar.gz` & `tmp/pitricks-0.1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitricks-0.1.3a3.tar", last modified: Tue Apr  4 04:37:18 2023, max compression
+gzip compressed data, was "pitricks-0.1.4a1.tar", last modified: Thu May  4 07:21:12 2023, max compression
```

## Comparing `pitricks-0.1.3a3.tar` & `pitricks-0.1.4a1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.170634 pitricks-0.1.3a3/
--rw-rw-rw-   0        0        0    35823 2023-01-19 08:44:48.000000 pitricks-0.1.3a3/LICENSE
--rw-rw-rw-   0        0        0      219 2023-04-04 04:37:18.168632 pitricks-0.1.3a3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.048139 pitricks-0.1.3a3/pitricks/
--rw-rw-rw-   0        0        0      121 2023-04-01 07:52:08.000000 pitricks-0.1.3a3/pitricks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.072135 pitricks-0.1.3a3/pitricks/odd_tools/
--rw-rw-rw-   0        0        0        0 2023-01-20 04:15:03.000000 pitricks-0.1.3a3/pitricks/odd_tools/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-01 07:39:29.000000 pitricks-0.1.3a3/pitricks/odd_tools/file_batch_replace.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.081136 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/
--rw-rw-rw-   0        0        0       41 2023-01-25 11:00:42.000000 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/__init__.py
--rw-rw-rw-   0        0        0     4496 2023-04-01 07:54:45.000000 pitricks-0.1.3a3/pitricks/odd_tools/method_chain/main.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.089137 pitricks-0.1.3a3/pitricks/operations/
--rw-rw-rw-   0        0        0        0 2023-01-19 02:49:31.000000 pitricks-0.1.3a3/pitricks/operations/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-03-28 13:56:40.000000 pitricks-0.1.3a3/pitricks/operations/ops.py
--rw-rw-rw-   0        0        0      125 2023-04-01 07:48:40.000000 pitricks-0.1.3a3/pitricks/path.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.094154 pitricks-0.1.3a3/pitricks/tmp/
--rw-rw-rw-   0        0        0       34 2023-01-24 15:08:53.000000 pitricks-0.1.3a3/pitricks/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.104136 pitricks-0.1.3a3/pitricks/tmp/classes/
--rw-rw-rw-   0        0        0       86 2023-01-25 01:34:13.000000 pitricks-0.1.3a3/pitricks/tmp/classes/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-01-25 02:00:15.000000 pitricks-0.1.3a3/pitricks/tmp/classes/chain.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.162632 pitricks-0.1.3a3/pitricks/utils/
--rw-rw-rw-   0        0        0      369 2023-04-03 03:52:19.000000 pitricks-0.1.3a3/pitricks/utils/__init__.py
--rw-rw-rw-   0        0        0     1108 2023-01-25 00:49:09.000000 pitricks-0.1.3a3/pitricks/utils/code_generater.py
--rw-rw-rw-   0        0        0        0 2023-02-16 06:58:34.000000 pitricks-0.1.3a3/pitricks/utils/daemon.py
--rw-rw-rw-   0        0        0     2304 2023-04-03 09:46:38.000000 pitricks-0.1.3a3/pitricks/utils/handle_exp.py
--rw-rw-rw-   0        0        0        0 2023-02-22 13:22:41.000000 pitricks-0.1.3a3/pitricks/utils/lock.py
--rw-rw-rw-   0        0        0     1088 2023-04-03 08:01:37.000000 pitricks-0.1.3a3/pitricks/utils/log.py
--rw-rw-rw-   0        0        0     4613 2023-04-01 07:37:12.000000 pitricks-0.1.3a3/pitricks/utils/mp_workflow.py
--rw-rw-rw-   0        0        0     1930 2023-04-01 07:37:28.000000 pitricks-0.1.3a3/pitricks/utils/reflect.py
--rw-rw-rw-   0        0        0      956 2023-03-28 13:50:09.000000 pitricks-0.1.3a3/pitricks/utils/relative_import_everywhere.py
--rw-rw-rw-   0        0        0     4368 2023-04-03 08:54:39.000000 pitricks-0.1.3a3/pitricks/utils/retry.py
--rw-rw-rw-   0        0        0      602 2023-01-24 13:34:04.000000 pitricks-0.1.3a3/pitricks/utils/sync.py
--rw-rw-rw-   0        0        0      860 2023-01-23 10:37:27.000000 pitricks-0.1.3a3/pitricks/utils/test.py
--rw-rw-rw-   0        0        0      528 2023-04-01 07:51:06.000000 pitricks-0.1.3a3/pitricks/utils/types.py
--rw-rw-rw-   0        0        0     2167 2023-04-03 07:37:13.000000 pitricks-0.1.3a3/pitricks/utils/use_pool.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:37:18.065136 pitricks-0.1.3a3/pitricks.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 04:37:17.000000 pitricks-0.1.3a3/pitricks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 04:37:18.171633 pitricks-0.1.3a3/setup.cfg
--rw-rw-rw-   0        0        0      263 2023-04-03 09:48:36.000000 pitricks-0.1.3a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.549218 pitricks-0.1.4a1/
+-rw-rw-rw-   0        0        0    35823 2023-01-19 08:44:48.000000 pitricks-0.1.4a1/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-05-04 07:21:12.548220 pitricks-0.1.4a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.484218 pitricks-0.1.4a1/pitricks/
+-rw-rw-rw-   0        0        0      121 2023-04-01 07:52:08.000000 pitricks-0.1.4a1/pitricks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.500218 pitricks-0.1.4a1/pitricks/odd_tools/
+-rw-rw-rw-   0        0        0        0 2023-01-20 04:15:03.000000 pitricks-0.1.4a1/pitricks/odd_tools/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 07:39:29.000000 pitricks-0.1.4a1/pitricks/odd_tools/file_batch_replace.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.504219 pitricks-0.1.4a1/pitricks/odd_tools/method_chain/
+-rw-rw-rw-   0        0        0       41 2023-01-25 11:00:42.000000 pitricks-0.1.4a1/pitricks/odd_tools/method_chain/__init__.py
+-rw-rw-rw-   0        0        0     4496 2023-04-01 07:54:45.000000 pitricks-0.1.4a1/pitricks/odd_tools/method_chain/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.507217 pitricks-0.1.4a1/pitricks/operations/
+-rw-rw-rw-   0        0        0        0 2023-01-19 02:49:31.000000 pitricks-0.1.4a1/pitricks/operations/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-03-28 13:56:40.000000 pitricks-0.1.4a1/pitricks/operations/ops.py
+-rw-rw-rw-   0        0        0      125 2023-04-01 07:48:40.000000 pitricks-0.1.4a1/pitricks/path.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.509217 pitricks-0.1.4a1/pitricks/tmp/
+-rw-rw-rw-   0        0        0       34 2023-01-24 15:08:53.000000 pitricks-0.1.4a1/pitricks/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.513218 pitricks-0.1.4a1/pitricks/tmp/classes/
+-rw-rw-rw-   0        0        0       86 2023-01-25 01:34:13.000000 pitricks-0.1.4a1/pitricks/tmp/classes/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-01-25 02:00:15.000000 pitricks-0.1.4a1/pitricks/tmp/classes/chain.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.544218 pitricks-0.1.4a1/pitricks/utils/
+-rw-rw-rw-   0        0        0      396 2023-05-04 07:19:19.000000 pitricks-0.1.4a1/pitricks/utils/__init__.py
+-rw-rw-rw-   0        0        0     1108 2023-01-25 00:49:09.000000 pitricks-0.1.4a1/pitricks/utils/code_generater.py
+-rw-rw-rw-   0        0        0        0 2023-02-16 06:58:34.000000 pitricks-0.1.4a1/pitricks/utils/daemon.py
+-rw-rw-rw-   0        0        0     2304 2023-04-03 09:46:38.000000 pitricks-0.1.4a1/pitricks/utils/handle_exp.py
+-rw-rw-rw-   0        0        0        0 2023-02-22 13:22:41.000000 pitricks-0.1.4a1/pitricks/utils/lock.py
+-rw-rw-rw-   0        0        0     1088 2023-05-02 14:11:40.000000 pitricks-0.1.4a1/pitricks/utils/log.py
+-rw-rw-rw-   0        0        0     4613 2023-04-01 07:37:12.000000 pitricks-0.1.4a1/pitricks/utils/mp_workflow.py
+-rw-rw-rw-   0        0        0      161 2023-05-04 07:18:47.000000 pitricks-0.1.4a1/pitricks/utils/path_ops.py
+-rw-rw-rw-   0        0        0     1930 2023-04-01 07:37:28.000000 pitricks-0.1.4a1/pitricks/utils/reflect.py
+-rw-rw-rw-   0        0        0      956 2023-03-28 13:50:09.000000 pitricks-0.1.4a1/pitricks/utils/relative_import_everywhere.py
+-rw-rw-rw-   0        0        0     4375 2023-05-04 06:40:51.000000 pitricks-0.1.4a1/pitricks/utils/retry.py
+-rw-rw-rw-   0        0        0      602 2023-01-24 13:34:04.000000 pitricks-0.1.4a1/pitricks/utils/sync.py
+-rw-rw-rw-   0        0        0      860 2023-01-23 10:37:27.000000 pitricks-0.1.4a1/pitricks/utils/test.py
+-rw-rw-rw-   0        0        0      572 2023-05-04 06:40:30.000000 pitricks-0.1.4a1/pitricks/utils/types.py
+-rw-rw-rw-   0        0        0     2167 2023-04-03 07:37:13.000000 pitricks-0.1.4a1/pitricks/utils/use_pool.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:21:12.496218 pitricks-0.1.4a1/pitricks.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-04 07:21:12.000000 pitricks-0.1.4a1/pitricks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2023-05-04 07:21:12.000000 pitricks-0.1.4a1/pitricks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:21:12.000000 pitricks-0.1.4a1/pitricks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 07:21:12.000000 pitricks-0.1.4a1/pitricks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 07:21:12.000000 pitricks-0.1.4a1/pitricks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:21:12.549218 pitricks-0.1.4a1/setup.cfg
+-rw-rw-rw-   0        0        0      271 2023-05-04 07:19:39.000000 pitricks-0.1.4a1/setup.py
```

### Comparing `pitricks-0.1.3a3/LICENSE` & `pitricks-0.1.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/odd_tools/method_chain/main.py` & `pitricks-0.1.4a1/pitricks/odd_tools/method_chain/main.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/operations/ops.py` & `pitricks-0.1.4a1/pitricks/operations/ops.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/tmp/classes/chain.py` & `pitricks-0.1.4a1/pitricks/tmp/classes/chain.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/code_generater.py` & `pitricks-0.1.4a1/pitricks/utils/code_generater.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/handle_exp.py` & `pitricks-0.1.4a1/pitricks/utils/handle_exp.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/log.py` & `pitricks-0.1.4a1/pitricks/utils/log.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/mp_workflow.py` & `pitricks-0.1.4a1/pitricks/utils/mp_workflow.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/reflect.py` & `pitricks-0.1.4a1/pitricks/utils/reflect.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/relative_import_everywhere.py` & `pitricks-0.1.4a1/pitricks/utils/relative_import_everywhere.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/retry.py` & `pitricks-0.1.4a1/pitricks/utils/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   """重试, 可以用于装饰器, 也可以用于函数;
   _times: 重试时间, -1为无限重试; 
   _interval: 重试间隔, 可以是一个数字, 也可以是元组(最小间隔, 最大间隔, 乘数), 也可以自定义从上一个间隔计算下一个的函数; 
   _exp: 重试的异常, 可以是一个异常类, 也可以是一个异常类的元组; 
   _regex: 重试的异常信息的正则表达式, 默认为".*", 与retry_exp是`与`的关系 """
   if not isinstance(_exp, tuple):
     _exp = (_exp, )
-  interval = _interval if isinstance(_interval, float) else _interval[0]
+  interval = _interval if isinstance(_interval, (int, float)) else _interval[0]
   
   if func is None:
     # 用于装饰器
     assert not args and not kwargs, "retry can't be used as wrapper with args or kwargs"
     
     if iscoroutinefunction(func):
       # async函数
```

### Comparing `pitricks-0.1.3a3/pitricks/utils/sync.py` & `pitricks-0.1.4a1/pitricks/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/test.py` & `pitricks-0.1.4a1/pitricks/utils/test.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks/utils/use_pool.py` & `pitricks-0.1.4a1/pitricks/utils/use_pool.py`

 * *Files identical despite different names*

### Comparing `pitricks-0.1.3a3/pitricks.egg-info/SOURCES.txt` & `pitricks-0.1.4a1/pitricks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 setup.py
 pitricks/__init__.py
 pitricks/path.py
 pitricks.egg-info/PKG-INFO
 pitricks.egg-info/SOURCES.txt
 pitricks.egg-info/dependency_links.txt
+pitricks.egg-info/requires.txt
 pitricks.egg-info/top_level.txt
 pitricks/odd_tools/__init__.py
 pitricks/odd_tools/file_batch_replace.py
 pitricks/odd_tools/method_chain/__init__.py
 pitricks/odd_tools/method_chain/main.py
 pitricks/operations/__init__.py
 pitricks/operations/ops.py
@@ -18,14 +19,15 @@
 pitricks/utils/__init__.py
 pitricks/utils/code_generater.py
 pitricks/utils/daemon.py
 pitricks/utils/handle_exp.py
 pitricks/utils/lock.py
 pitricks/utils/log.py
 pitricks/utils/mp_workflow.py
+pitricks/utils/path_ops.py
 pitricks/utils/reflect.py
 pitricks/utils/relative_import_everywhere.py
 pitricks/utils/retry.py
 pitricks/utils/sync.py
 pitricks/utils/test.py
 pitricks/utils/types.py
 pitricks/utils/use_pool.py
```

