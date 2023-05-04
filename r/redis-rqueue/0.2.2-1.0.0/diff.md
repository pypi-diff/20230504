# Comparing `tmp/redis-rqueue-0.2.2.tar.gz` & `tmp/redis-rqueue-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-rqueue-0.2.2.tar", last modified: Mon Jan 16 14:05:19 2023, max compression
+gzip compressed data, was "redis-rqueue-1.0.0.tar", last modified: Thu May  4 14:25:44 2023, max compression
```

## Comparing `redis-rqueue-0.2.2.tar` & `redis-rqueue-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-01-16 14:05:19.519401 redis-rqueue-0.2.2/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-01-16 14:05:19.519269 redis-rqueue-0.2.2/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)      406 2023-01-16 13:42:16.000000 redis-rqueue-0.2.2/README.md
--rw-r--r--   0 vitor      (501) staff       (20)      263 2023-01-16 14:04:11.000000 redis-rqueue-0.2.2/pyproject.toml
--rw-r--r--   0 vitor      (501) staff       (20)       38 2023-01-16 14:05:19.519439 redis-rqueue-0.2.2/setup.cfg
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-01-16 14:05:19.517733 redis-rqueue-0.2.2/src/
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-01-16 14:05:19.518861 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-01-16 14:05:19.000000 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)      246 2023-01-16 14:05:19.000000 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/SOURCES.txt
--rw-r--r--   0 vitor      (501) staff       (20)        1 2023-01-16 14:05:19.000000 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/dependency_links.txt
--rw-r--r--   0 vitor      (501) staff       (20)       13 2023-01-16 14:05:19.000000 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/requires.txt
--rw-r--r--   0 vitor      (501) staff       (20)        7 2023-01-16 14:05:19.000000 redis-rqueue-0.2.2/src/redis_rqueue.egg-info/top_level.txt
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-01-16 14:05:19.518987 redis-rqueue-0.2.2/src/rqueue/
--rw-r--r--   0 vitor      (501) staff       (20)     3466 2023-01-16 13:53:18.000000 redis-rqueue-0.2.2/src/rqueue/__init__.py
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 14:25:44.821952 redis-rqueue-1.0.0/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-04 14:25:44.821811 redis-rqueue-1.0.0/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)       15 2023-05-04 14:20:49.000000 redis-rqueue-1.0.0/README.md
+-rw-r--r--   0 vitor      (501) staff       (20)      263 2023-05-04 14:20:35.000000 redis-rqueue-1.0.0/pyproject.toml
+-rw-r--r--   0 vitor      (501) staff       (20)       10 2023-04-27 18:10:37.000000 redis-rqueue-1.0.0/requirements.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       38 2023-05-04 14:25:44.821996 redis-rqueue-1.0.0/setup.cfg
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 14:25:44.820152 redis-rqueue-1.0.0/src/
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 14:25:44.821403 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-04 14:25:44.000000 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)      292 2023-05-04 14:25:44.000000 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        1 2023-05-04 14:25:44.000000 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       11 2023-05-04 14:25:44.000000 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/requires.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        7 2023-05-04 14:25:44.000000 redis-rqueue-1.0.0/src/redis_rqueue.egg-info/top_level.txt
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-04 14:25:44.821644 redis-rqueue-1.0.0/src/rqueue/
+-rw-r--r--   0 vitor      (501) staff       (20)       67 2023-05-04 13:16:59.000000 redis-rqueue-1.0.0/src/rqueue/__init__.py
+-rw-r--r--   0 vitor      (501) staff       (20)     2837 2023-05-04 13:59:12.000000 redis-rqueue-1.0.0/src/rqueue/queue_executor.py
```

### Comparing `redis-rqueue-0.2.2/src/rqueue/__init__.py` & `redis-rqueue-1.0.0/src/rqueue/queue_executor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,71 @@
-from redis import Redis
-from collections.abc import Callable
-from typing import Any, List
 import logging
 import time
-from threading import Thread
-import csv
-import glob
+from collections.abc import Callable
+
+import redis
+
+logging.basicConfig(
+    format='%(asctime)s | %(levelname)s | %(message)s', level=logging.INFO)
 
-logging.basicConfig(format='%(asctime)s | %(levelname)s | %(message)s', level=logging.INFO)
 
-class Queue:
+class QueueExecutor:
     def __init__(
         self,
-        queue_name:str,
-        success_queue:str|List[str] = None,
-        error_queue:str|List[str] = None,
-        redis_host:str = 'localhost',
-        redis_port:int = 6379,
-        redis_db:int = 0
-        ) -> None:
-
-        self.queue_name = queue_name
-        self.redis_client = Redis(host=redis_host, port=redis_port, db=redis_db, decode_responses=True)
-
-        if success_queue:
-            self.success_queue = [success_queue] if type(success_queue) == str else success_queue
-        else:
-            self.success_queue = [f'{self.queue_name}:success']
-
-        if error_queue:
-            self.error_queue = [error_queue] if type(error_queue) == str else error_queue
-        else:
-            self.error_queue = [f'{self.queue_name}:error']
+        redis_client: redis.Redis,
+        user_function: Callable[[str], None],
+        queue: str,
+        doing_queue: str,
+        success_queue: str,
+        error_queue: str,
+        maximum_attempts: int,
+        sleep_time: int
+    ) -> None:
+
+        self.redis_client = redis_client
+        self.user_function = user_function
+        self.queue = queue
+        self.doing_queue = doing_queue
+        self.success_queue = success_queue
+        self.error_queue = error_queue
+        self.maximum_attempts = maximum_attempts
+        self.sleep_time = sleep_time
 
+        self.redis_client.connection_pool.connection_kwargs['decode_responses'] = True
         self.redis_client.ping()
-        logging.info('Successfully connected to Redis.')
 
-    def _run_user_function(self, function:Callable, parameter:Any) -> None:
-        try:
-            function(parameter)
-            for queue in self.success_queue:
-                self.redis_client.rpush(queue, parameter)
-            logging.info(f'User function successfully executed with parameter "{parameter}"')
-        except Exception as e:
-            for queue in self.error_queue:
-                self.redis_client.rpush(queue, parameter)
-            logging.error(f'Failed to execute user function with parameter "{parameter}". {e}')
-
-    def _run_user_function_threading(self, function:Callable, parameters:list) -> None:
-        threads = []
-        for parameter in parameters:
-            thread = Thread(target=self._run_user_function, args=(function, parameter))
-            threads.append(thread)
-            thread.start()
-        for thread in threads:
-            thread.join()
-
-    def fill_from_list(self, elements:list, flush:bool=True) -> None:
-        if flush:
-            self.redis_client.delete(self.queue_name)
-            logging.info(f'The Redis queue "{self.queue_name}" was deleted.')
-        self.redis_client.rpush(self.queue_name, *elements)
-        logging.info(f'The Redis queue "{self.queue_name}" was filled with {len(elements)} elements.')
-
-    def fill_from_csv(self, csv_path:str, flush:bool=True) -> None:
-        with open(csv_path) as f:
-            elements = [element[0] for element in list(csv.reader(f))]
-        self.fill_from_list(elements, flush=flush)
-
-    def fill_from_folder(self, folder:str, suffix:str='', flush:bool=True):
-        elements = [i.removeprefix(f'{folder}/').removesuffix(f'{suffix}') for i in glob.glob(f'{folder}/*{suffix}')]
-        self.fill_from_list(elements, flush=flush)
-
-    def execute(self, function:Callable, threadings:int=2, retry:bool=True, sleep_time:int=30) -> None:
-        if retry:
-            self.error_queue = [self.queue_name]
+        self.attempt = 1
+        self.current_queue = queue
 
+    def execute(self):
         while True:
-            parameters = self.redis_client.lpop(self.queue_name, count=threadings) or []
-            if parameters:
-                self._run_user_function_threading(function, parameters)
+            if parameter := self.redis_client.lpop(self.current_queue):
+                self.redis_client.rpush(self.doing_queue, parameter)
+                try:
+                    self.user_function(parameter)
+                    self.redis_client.lrem(self.doing_queue, 0, parameter)
+                    self.redis_client.rpush(self.success_queue, parameter)
+                    logging.info(
+                        f'User function successfully executed with parameter "{parameter}". (attempt {self.attempt}).')
+                except Exception as e:
+                    self.redis_client.lrem(self.doing_queue, 0, parameter)
+                    if self.attempt >= self.maximum_attempts:
+                        self.redis_client.rpush(self.error_queue, parameter)
+                    else:
+                        self.redis_client.rpush(
+                            f'{self.queue}:attempt:{self.attempt + 1}', parameter)
+                    logging.error(
+                        f'Failed to execute user function with parameter "{parameter}". (attempt {self.attempt}). {e}')
+            elif self.attempt < self.maximum_attempts:
+                current_queue = self.current_queue
+                self.attempt += 1
+                self.current_queue = f'{self.queue}:attempt:{self.attempt}'
+                logging.info(
+                    f'The Redis queue "{current_queue}" is empty, changing to queue "{self.current_queue}".')
             else:
-                logging.info(f'The Redis queue "{self.queue_name}" is empty, sleeping for {sleep_time} second(s).')
-                time.sleep(sleep_time)
+                current_queue = self.current_queue
+                self.attempt = 1
+                self.current_queue = self.queue
+                logging.info(
+                    f'The Redis queue "{current_queue}" is empty, restarting.')
+                logging.info(f'Waiting {self.sleep_time} seconds.')
+                time.sleep(self.sleep_time)
```

