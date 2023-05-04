# Comparing `tmp/quenouille-1.7.1.tar.gz` & `tmp/quenouille-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quenouille-1.7.1.tar", last modified: Wed Mar  8 19:39:15 2023, max compression
+gzip compressed data, was "dist/quenouille-1.8.0.tar", last modified: Thu May  4 13:48:23 2023, max compression
```

## Comparing `quenouille-1.7.1.tar` & `quenouille-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-08 19:39:15.000000 quenouille-1.7.1/
--rw-r--r--   0 Yomgui     (501) staff       (20)    19045 2023-03-08 19:39:15.000000 quenouille-1.7.1/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)    16163 2023-03-08 14:22:34.000000 quenouille-1.7.1/README.md
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille/
--rw-r--r--   0 Yomgui     (501) staff       (20)      183 2023-02-22 19:41:55.000000 quenouille-1.7.1/quenouille/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      469 2021-05-25 17:09:07.000000 quenouille-1.7.1/quenouille/constants.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      471 2021-04-21 13:43:46.000000 quenouille-1.7.1/quenouille/exceptions.py
--rw-r--r--   0 Yomgui     (501) staff       (20)    40103 2023-03-08 19:36:44.000000 quenouille-1.7.1/quenouille/imap.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     3603 2023-03-08 14:37:32.000000 quenouille-1.7.1/quenouille/utils.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)    19045 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)      327 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/dependency_links.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       43 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       11 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-03-08 19:39:15.000000 quenouille-1.7.1/quenouille.egg-info/zip-safe
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-03-08 19:39:15.000000 quenouille-1.7.1/setup.cfg
--rw-r--r--   0 Yomgui     (501) staff       (20)      708 2023-03-08 19:38:53.000000 quenouille-1.7.1/setup.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    19392 2023-05-04 13:48:23.000000 quenouille-1.8.0/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)    16510 2023-05-04 13:34:27.000000 quenouille-1.8.0/README.md
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      183 2023-02-22 19:41:55.000000 quenouille-1.8.0/quenouille/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      469 2021-05-25 17:09:07.000000 quenouille-1.8.0/quenouille/constants.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      548 2023-05-03 18:05:41.000000 quenouille-1.8.0/quenouille/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    42481 2023-05-04 12:24:18.000000 quenouille-1.8.0/quenouille/imap.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4128 2023-05-04 12:24:05.000000 quenouille-1.8.0/quenouille/utils.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    19392 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)      327 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/SOURCES.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/dependency_links.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       43 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/requires.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       11 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/top_level.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-05-04 13:48:23.000000 quenouille-1.8.0/quenouille.egg-info/zip-safe
+-rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-05-04 13:48:23.000000 quenouille-1.8.0/setup.cfg
+-rw-r--r--   0 Yomgui     (501) staff       (20)      708 2023-05-04 13:47:32.000000 quenouille-1.8.0/setup.py
```

### Comparing `quenouille-1.7.1/PKG-INFO` & `quenouille-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quenouille
-Version: 1.7.1
+Version: 1.8.0
 Summary: A library of multithreaded iterator workflows.
 Home-page: http://github.com/medialab/quenouille
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/quenouille/workflows/Tests/badge.svg)](https://github.com/medialab/quenouille/actions)
         
@@ -103,15 +103,15 @@
           print(html)
         ```
         
         *Arguments*
         
         * **iterable** *(iterable)*: Any python iterable.
         * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
         * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
         * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
         * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
         * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
         * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
         * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
         * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
@@ -177,15 +177,15 @@
         executor.shutdown(wait=False)
         ```
         
         Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
         
         *Arguments*
         
-        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
         * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
         * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
         * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
         * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
         <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
         
@@ -259,15 +259,15 @@
           return 5 + (2 * random())
         ```
         
         #### Caveats regarding exception raising
         
         *Deferred generator usage exception deadlocks*
         
-        If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you will get end up in a deadlock if you raise an exception.
+        If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
         
         This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
         
         ```python
         # Safe
         for item in imap(...):
           raise RuntimeError
```

### Comparing `quenouille-1.7.1/README.md` & `quenouille-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
   print(html)
 ```
 
 *Arguments*
 
 * **iterable** *(iterable)*: Any python iterable.
 * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-* **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+* **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
 * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
 * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
 * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
 * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
 * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
 * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
 * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
@@ -169,15 +169,15 @@
 executor.shutdown(wait=False)
 ```
 
 Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
 
 *Arguments*
 
-* **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+* **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
 * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
 * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
 * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
 * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
 
 <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
 
@@ -251,15 +251,15 @@
   return 5 + (2 * random())
 ```
 
 #### Caveats regarding exception raising
 
 *Deferred generator usage exception deadlocks*
 
-If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you will get end up in a deadlock if you raise an exception.
+If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
 
 This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
 
 ```python
 # Safe
 for item in imap(...):
   raise RuntimeError
```

### Comparing `quenouille-1.7.1/quenouille/imap.py` & `quenouille-1.8.0/quenouille/imap.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Generic,
     TypeVar,
     Optional,
     Hashable,
     Callable,
     Dict,
     List,
-    Tuple,
     Any,
     Iterator,
     Iterable,
     Union,
 )
 
 import sys
@@ -30,22 +29,27 @@
 import time
 from queue import Queue, Empty
 from threading import Thread, Event, Lock, Condition, Barrier, BrokenBarrierError
 from collections import OrderedDict
 from collections.abc import Sized
 from itertools import count
 
-from quenouille.exceptions import BrokenThreadPool
+from quenouille.exceptions import (
+    BrokenThreadPool,
+    InvalidThrottleParallelismCombination,
+)
 from quenouille.utils import (
     clear,
     flush,
     smash,
+    queue_iter,
     is_usable_queue,
     get_default_maxworkers,
     SmartTimer,
+    TimedHeapSet,
 )
 from quenouille.constants import THE_END_IS_NIGH, DEFAULT_BUFFER_SIZE, TIMER_EPSILON
 
 ItemType = TypeVar("ItemType", covariant=True)
 
 
 class QuenouilleQueueProtocol(Protocol[ItemType]):
@@ -89,22 +93,19 @@
         except BaseException:
             # We catch the exception before flushing downstream to be
             # sure the job can be passed down the line but it might not be
             # the best thing to do. Time will tell...
             self.exc_info = sys.exc_info()
 
     def __repr__(self):
-        return (
-            "<{name} id={id!r} index={index!r} group={group!r} item={item!r}>".format(
-                name=self.__class__.__name__,
-                index=self.index,
-                group=self.group,
-                item=self.item,
-                id=id(self),
-            )
+        return "<{name} index={index!r} group={group!r} item={item!r}>".format(
+            name=self.__class__.__name__,
+            index=self.index,
+            group=self.group,
+            item=self.item,
         )
 
 
 class IterationState(object):
     """
     Class representing an executor imap iteration state. It keeps tracks of
     counts of jobs started and finished, and is used to declare the end of
@@ -177,15 +178,15 @@
         self,
         output_queue: Queue,
         throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
     ):
         # Properties
         self.output_queue = output_queue  # type: Queue
         self.throttle = throttle  # type: ThrottleType[GroupType, ItemType, ResultType]
-        self.identity = None  # type: Optional[int]
+        self.identity = None  # type: Optional[Any]
 
         # Containers
         self.groups = {}  # type: Dict[GroupType, float]
 
         # Threading
         self.timer = None  # type: Optional[SmartTimer]
         self.__registered_calback = None  # type: Optional[Callable[[int], None]]
@@ -205,20 +206,18 @@
         self.__registered_calback = None
 
     def update(
         self, key, throttle: ThrottleType[GroupType, ItemType, ResultType]
     ) -> None:
         assert key is None or callable(key)
 
-        new_identity = id(key)
-
-        if new_identity != self.identity:
+        if key is not self.identity:
             self.__reset()
 
-        self.identity = new_identity
+        self.identity = key
         self.throttle = throttle
 
         assert isinstance(self.throttle, (int, float)) or callable(self.throttle)
 
     def add(self, job: Job[ItemType, GroupType, ResultType]) -> None:
         throttle_time = self.throttle
 
@@ -229,15 +228,19 @@
                 throttle_time = 0
 
             if not isinstance(throttle_time, (int, float)) or throttle_time < 0:
                 raise TypeError('callable "throttle" must return numbers >= 0')
 
         if throttle_time != 0:
             group = cast(GroupType, job.group)
-            assert group not in self
+
+            if group in self:
+                raise InvalidThrottleParallelismCombination(
+                    "throttle cannot be > 0 for a group with parallelism > 1"
+                )
 
             self.groups[group] = time.time() + throttle_time  # type: ignore
             self.__spawn_timer(throttle_time)  # type: ignore
 
     def __cancel_timer(self) -> None:
         if self.timer is None:
             return
@@ -434,28 +437,28 @@
 
         return None
 
     def put(self, job: Job[ItemType, GroupType, ResultType]) -> None:
         with self.lock:
             assert not self.__full()
 
-            self.items[id(job)] = job
+            self.items[job.index] = job
 
     def get(self) -> Optional[Job[ItemType, GroupType, ResultType]]:
         while not self.teardown_event.is_set():
             self.lock.acquire()
 
             if len(self.items) == 0:
                 self.lock.release()
                 return None
 
             job = self.__find_suitable_job()
 
             if job is not None:
-                del self.items[id(job)]
+                del self.items[job.index]
                 self.lock.release()
                 return job
 
             if self.__full():
                 self.lock.release()
 
                 with self.condition:
@@ -508,51 +511,51 @@
 
     Note that this requires to buffer values into memory until the next valid
     item has been processed by a worker thread.
     """
 
     def __init__(self):
         self.last_index = 0  # type: int
-        self.items = {}  # type: Dict[int, Job[ItemType, GroupType, ResultType]]
+        self.items = {}  # type: Dict[int, ResultType]
 
     def is_clean(self) -> bool:
         """
         This function is only used after an imap is over to ensure no
         dangling resource could be found.
         """
         return len(self.items) == 0
 
     def flush(self) -> Iterator[ResultType]:
         while self.last_index in self.items:
-            yield self.items.pop(self.last_index).result  # type: ignore
+            yield self.items.pop(self.last_index)
             self.last_index += 1
 
     def output(self, job: Job[ItemType, GroupType, ResultType]) -> Iterator[ResultType]:
         if job.index == self.last_index:
             self.last_index += 1
             yield job.result  # type: ignore
             yield from self.flush()
         else:
-            self.items[job.index] = job
+            self.items[job.index] = job.result  # type: ignore
 
 
 def validate_threadpool_kwargs(
     name,
     max_workers=None,
     initializer=None,
     initargs=None,
     wait=None,
     daemonic=None,
     excepthook=None,
 ) -> None:
     if max_workers is None:
         return
 
-    if not isinstance(max_workers, int) or max_workers < 1:
-        raise TypeError('"%s" should be an integer > 0' % name)
+    if not isinstance(max_workers, int) or max_workers < 0:
+        raise TypeError('"%s" should be an integer >= 0' % name)
 
     if initializer is not None and not callable(initializer):
         raise TypeError('"initializer" is not callable')
 
     if initargs is not None and not isinstance(initargs, Iterable):
         raise TypeError('"initargs" is not iterable')
 
@@ -563,15 +566,15 @@
         raise TypeError('"daemonic" should be boolean')
 
     if not isinstance(excepthook, bool):
         raise TypeError('"excepthook" should be boolean')
 
 
 def validate_imap_kwargs(
-    iterable, func, *, max_workers, key, parallelism, buffer_size, throttle
+    iterable, func, *, key, parallelism, buffer_size, throttle
 ) -> None:
     if not isinstance(iterable, Iterable) and not is_usable_queue(iterable):
         raise TypeError("target is not iterable nor a queue")
 
     if not callable(func):
         raise TypeError("worker function is not callable")
 
@@ -580,33 +583,34 @@
 
     if not isinstance(parallelism, (int, float)) and not callable(parallelism):
         raise TypeError('"parallelism" is not a number nor callable')
 
     if isinstance(parallelism, int) and parallelism < 0:
         raise TypeError('"parallelism" is not a positive integer')
 
-    # if parallelism > max_workers:
-    #     raise TypeError('"parallelism" cannot be greater than the number of workers')
-
-    if not isinstance(buffer_size, int) or buffer_size < 1:
-        raise TypeError('"buffer_size" is not an integer > 0')
+    if not isinstance(buffer_size, int) or buffer_size < 0:
+        raise TypeError('"buffer_size" is not an integer >= 0')
 
     if not isinstance(throttle, (int, float)) and not callable(throttle):
         raise TypeError('"throttle" is not a number nor callable')
 
     if isinstance(throttle, (int, float)) and throttle < 0:
         raise TypeError('"throttle" cannot be negative')
 
 
 class ThreadPoolExecutor(object):
     """
     Quenouille custom ThreadPoolExecutor able to lazily pull items to process
     from iterated streams, all while bounding used memory and respecting
     group parallelism and throttling.
 
+    Note that if given max_workers=0, this pool will still work, but without
+    relying on threads whatsoever. This can be useful in some scenarios where
+    you want to avoid duplicating code.
+
     Args:
         max_workers (int, optional): Number of threads to use.
             Defaults to min(32, os.cpu_count() + 1).
         initializer (callable, optional): Function that will be run when starting
             each worker thread. Can be useful to setup a threading local context
             for instance.
         initargs (iterable, optional): Arguments to pass to the thread initializer
@@ -617,15 +621,15 @@
             Defaults to False.
     """
 
     def __init__(
         self,
         max_workers: Optional[int] = None,
         initializer: Optional[Callable[..., None]] = None,
-        initargs: Tuple[Any, ...] = tuple(),
+        initargs: Iterable[Any] = tuple(),
         wait: bool = True,
         daemonic: bool = False,
         excepthook: bool = False,
     ):
         # Validation and defaults
         validate_threadpool_kwargs(
             "max_workers",
@@ -638,14 +642,15 @@
         )
 
         if max_workers is None:
             max_workers = get_default_maxworkers()
 
         # Properties
         self.max_workers = max_workers  # type: int
+        self.dummy = max_workers == 0  # type: bool
         self.wait = wait  # type: bool
         self.daemonic = daemonic  # type: bool
 
         # Init
         self.initializer = initializer
         self.initargs = list(initargs)
 
@@ -665,14 +670,20 @@
 
         # State
         self.patching_excepthook = excepthook
         self.original_excepthook = None
         self.cleanup = None
         self.closed = False  # type: bool
 
+        if self.dummy:
+            # If pool is dummy, we run the initializer synchronously
+            if self.initializer is not None:
+                self.initializer(*self.initargs)
+            return
+
         # Thread pool
         self.threads = [
             Thread(
                 name="Thread-quenouille-%i-%i" % (id(self), n),
                 target=self.__worker,
                 daemon=self.daemonic,
             )
@@ -690,15 +701,23 @@
 
         try:
             self.boot_barrier.wait()
         except BrokenBarrierError:
             self.shutdown(wait=self.wait)
             raise BrokenThreadPool
 
+    @property
+    def is_actually_multithreaded(self) -> bool:
+        return self.dummy
+
     def __enter__(self):
+        # NOTE: nothing needs to happens if the executor is not multithreaded
+        if self.dummy:
+            return self
+
         if self.closed:
             raise RuntimeError("cannot re-enter a closed executor")
 
         if not self.patching_excepthook:
             return self
 
         self.original_excepthook = sys.excepthook
@@ -720,21 +739,29 @@
             self.original_excepthook(exc_type, exc_value, exc_traceback)  # type: ignore
 
         sys.excepthook = executor_excepthook
 
         return self
 
     def __exit__(self, *args) -> Optional[bool]:
+        # NOTE: nothing needs to happens if the executor is not multithreaded
+        if self.dummy:
+            return
+
         if self.patching_excepthook:
             sys.excepthook = self.original_excepthook
             self.original_excepthook = None
 
         self.shutdown(wait=self.wait)
 
     def shutdown(self, wait=True) -> None:
+        # NOTE: shutdown is a noop if the executor is not multithreaded
+        if self.dummy:
+            return
+
         if self.closed:
             return
 
         with self.teardown_lock:
             self.teardown_event.set()
 
             # Killing workers (cancel jobs and flushing end messages)
@@ -797,25 +824,66 @@
 
                 assert self.output_queue is not None
                 self.output_queue.put(job)
 
         except BaseException as e:
             smash(self.output_queue, e)
 
+    def __imap_sync(
+        self,
+        iterable: ImapTarget[ItemType],
+        func: Callable[[ItemType], ResultType],
+        *,
+        key: Optional[Callable[[ItemType], GroupType]] = None,
+        throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
+    ) -> Iterator[ResultType]:
+        if is_usable_queue(iterable):
+            items = queue_iter(iterable)  # type: ignore
+        else:
+            items = iterable
+
+        items = cast(Iterator[ItemType], items)
+
+        # TODO: make throttling work per group
+        timers = TimedHeapSet()  # type: TimedHeapSet[GroupType]
+
+        for item in items:
+            group = None if key is None else key(item)
+
+            if group is not None:
+                # NOTE: wait_for also perform cleanup for us
+                timers.wait_for(group)
+
+            result = func(item)
+
+            if group is not None and throttle is not None:
+                if callable(throttle):
+                    duration = throttle(group, item, result)
+                else:
+                    duration = throttle
+
+                if duration > 0:
+                    timers.add(group, duration)
+
+            yield result
+
     def __imap(
         self,
         iterable: ImapTarget[ItemType],
         func: Callable[[ItemType], ResultType],
         *,
         ordered: bool = False,
         key: Optional[Callable[[ItemType], GroupType]] = None,
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
         throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
     ) -> Iterator[ResultType]:
+        if self.dummy:
+            return self.__imap_sync(iterable, func, key=key, throttle=throttle)
+
         # Cannot run in multiple threads
         if self.imap_lock.locked():
             raise RuntimeError(
                 "cannot run multiple executor methods concurrently from different threads"
             )
 
         # Cannot run if already closed
@@ -849,19 +917,20 @@
             "Queue[Union[Job[ItemType, GroupType, ResultType], object]]", self.job_queue
         )
         self.output_queue = cast(
             "Queue[Union[BaseException, Job[ItemType, GroupType, ResultType], object]]",
             self.output_queue,
         )
 
+        # NOTE: currently buffer_size=0 does not work with throttle nor group parallelism
         def enqueue():
             try:
                 while not end_event.is_set():
                     # First we check to see if there is a suitable buffered job
-                    job = buffer.get()
+                    job = None if buffer_size == 0 else buffer.get()
 
                     if job is None:
                         # Else we consume the iterator to find one
                         try:
                             if not iterable_is_queue:
                                 item = next(iterator)  # type: ignore
                             else:
@@ -889,16 +958,17 @@
                         group = None
 
                         if key is not None:
                             group = key(item)
 
                         job = Job(func, item=item, index=next(job_counter), group=group)
 
-                        buffer.put(job)
-                        continue
+                        if buffer_size > 0:
+                            buffer.put(job)
+                            continue
 
                     # Registering the job
                     buffer.register_job(job)
                     state.start_task()
                     self.job_queue.put(job)
 
             except BaseException as e:
@@ -973,14 +1043,17 @@
                     # NOTE: this was moved after yielding items so that the
                     # generator body may enqueue new jobs. It is possible that
                     # this has a slight perf hit if the body performs heavy work?
                     state.finish_task()
 
                     # Cleanup memory and avoid keeping references attached to
                     # ease up garbage collection
+                    # NOTE: the ordered output buffer does not store any reference
+                    # to jobs but only keep their results. This is therefore
+                    # the last remaining reference to a job there.
                     del job
 
             except:
                 raised = True
                 raise
 
             finally:
@@ -1007,15 +1080,14 @@
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
         throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
     ) -> Iterator[ResultType]:
         validate_imap_kwargs(
             iterable=iterable,
             func=func,
-            max_workers=self.max_workers,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
         )
 
         return self.__imap(
@@ -1037,15 +1109,14 @@
         parallelism: ParallelismType[GroupType] = 1,
         buffer_size: int = DEFAULT_BUFFER_SIZE,
         throttle: ThrottleType[GroupType, ItemType, ResultType] = 0
     ) -> Iterator[ResultType]:
         validate_imap_kwargs(
             iterable=iterable,
             func=func,
-            max_workers=self.max_workers,
             key=key,
             parallelism=parallelism,
             buffer_size=buffer_size,
             throttle=throttle,
         )
 
         return self.__imap(
@@ -1065,15 +1136,15 @@
     threads: Optional[int] = None,
     *,
     key: Optional[Callable[[ItemType], GroupType]] = None,
     parallelism: ParallelismType[GroupType] = 1,
     buffer_size: int = DEFAULT_BUFFER_SIZE,
     throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
     initializer: Optional[Callable[..., None]] = None,
-    initargs: Tuple[Any, ...] = tuple(),
+    initargs: Iterable[Any] = tuple(),
     wait: bool = True,
     daemonic: bool = False,
     excepthook: bool = False
 ) -> Iterator[ResultType]:
     validate_threadpool_kwargs(
         "threads",
         threads,
@@ -1082,15 +1153,14 @@
         wait=wait,
         daemonic=daemonic,
         excepthook=excepthook,
     )
     validate_imap_kwargs(
         iterable=iterable,
         func=func,
-        max_workers=threads,
         key=key,
         parallelism=parallelism,
         buffer_size=buffer_size,
         throttle=throttle,
     )
 
     # If we know the size of the iterable, and this size is less than the
@@ -1125,15 +1195,15 @@
     threads: Optional[int] = None,
     *,
     key: Optional[Callable[[ItemType], GroupType]] = None,
     parallelism: ParallelismType[GroupType] = 1,
     buffer_size: int = DEFAULT_BUFFER_SIZE,
     throttle: ThrottleType[GroupType, ItemType, ResultType] = 0,
     initializer: Optional[Callable[..., None]] = None,
-    initargs: Tuple[Any, ...] = tuple(),
+    initargs: Iterable[Any] = tuple(),
     wait: bool = True,
     daemonic: bool = False,
     excepthook: bool = False
 ) -> Iterator[ResultType]:
     validate_threadpool_kwargs(
         "threads",
         threads,
@@ -1142,15 +1212,14 @@
         wait=wait,
         daemonic=daemonic,
         excepthook=excepthook,
     )
     validate_imap_kwargs(
         iterable=iterable,
         func=func,
-        max_workers=threads,
         key=key,
         parallelism=parallelism,
         buffer_size=buffer_size,
         throttle=throttle,
     )
 
     # If we know the size of the iterable, and this size is less than the
```

### Comparing `quenouille-1.7.1/quenouille/utils.py` & `quenouille-1.8.0/quenouille/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # =============================================================================
 # Quenouille Various Utils
 # =============================================================================
 #
 # Miscellaneous utility functions.
 #
-from typing import TypeVar, Generic, List, Set, Tuple, Hashable
+from typing import TypeVar, Generic, List, Dict, Tuple, Hashable, Iterator
 
 import os
 import time
 import heapq
 from threading import Lock, Timer
 from weakref import WeakValueDictionary
 from queue import Empty, Full, Queue
@@ -35,14 +35,22 @@
 
 
 def smash(q: "Queue[ItemType]", v: ItemType) -> None:
     clear(q)
     q.put_nowait(v)
 
 
+def queue_iter(q: "Queue[ItemType]") -> Iterator[ItemType]:
+    while True:
+        try:
+            yield q.get_nowait()
+        except Empty:
+            break
+
+
 def is_usable_queue(v) -> bool:
     # NOTE: get_nowait is the only method used by quenouille when working
     # on a queue given by the user, as of now.
     return hasattr(v, "get_nowait") and callable(v.get_nowait)
 
 
 # As per: https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor
@@ -108,25 +116,38 @@
 
 class TimedHeapSet(Generic[HeapSetItemType]):
     def __init__(self):
         self.clear()
 
     def clear(self) -> None:
         self.heap = []  # type: List[Tuple[float, HeapSetItemType]]
-        self.set = set()  # type: Set[HeapSetItemType]
+        self.map = {}  # type: Dict[HeapSetItemType, float]
 
     def __len__(self) -> int:
         return len(self.heap)
 
     def __contains__(self, item: HeapSetItemType) -> bool:
-        return item in self.set
+        return item in self.map
 
     def add(self, item: HeapSetItemType, duration: float) -> None:
-        self.set.add(item)
-        heapq.heappush(self.heap, (time.time() + duration, item))
+        next_time = time.time() + duration
+        self.map[item] = next_time
+        heapq.heappush(self.heap, (next_time, item))
+
+    def wait_for(self, item: HeapSetItemType) -> None:
+        # NOTE: we cleanup before just in case
+        self.cleanup()
+
+        next_time = self.map.get(item)
+
+        if next_time is None:
+            return
+
+        time.sleep(max((next_time - time.time()), 0) + TIMER_EPSILON)
+        self.cleanup()
 
     def cleanup(self) -> None:
         current_time = time.time()
 
         while self.heap and current_time >= self.heap[0][0] - TIMER_EPSILON:
-            self.set.remove(self.heap[0][1])
+            del self.map[self.heap[0][1]]
             heapq.heappop(self.heap)
```

### Comparing `quenouille-1.7.1/quenouille.egg-info/PKG-INFO` & `quenouille-1.8.0/quenouille.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quenouille
-Version: 1.7.1
+Version: 1.8.0
 Summary: A library of multithreaded iterator workflows.
 Home-page: http://github.com/medialab/quenouille
 Author: Guillaume Plique
 Author-email: kropotkinepiotr@gmail.com
 License: MIT
 Description: [![Build Status](https://github.com/medialab/quenouille/workflows/Tests/badge.svg)](https://github.com/medialab/quenouille/actions)
         
@@ -103,15 +103,15 @@
           print(html)
         ```
         
         *Arguments*
         
         * **iterable** *(iterable)*: Any python iterable.
         * **func** *(callable)*: Function used to perform the desired tasks. The function takes an item yielded by the given iterable as single argument. Note that since this function will be dispatched in worker threads, so you should ensure it is thread-safe.
-        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+        * **threads** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
         * **key** *(callable, optional)*: Function returning to which "group" a given item is supposed to belong. This will be used to ensure maximum parallelism is respected.
         * **parallelism** *(int or callable, optional)* [`1`]: Number of threads allowed to work on a same group at once. Can also be a function taking a group and returning its parallelism.
         * **buffer_size** *(int, optional)* [`1024`]: Maximum number of items the function will buffer into memory while attempting to find an item that can be passed to a worker immediately, all while respecting throttling and group parallelism.
         * **throttle** *(int or float or callable, optional)*: Optional throttle time, in seconds, to wait before processing the next item of a given group. Can also be a function taking last group, item and result and returning next throttle time for this group.
         * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
         * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
         * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when shutting down the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
@@ -177,15 +177,15 @@
         executor.shutdown(wait=False)
         ```
         
         Note that your throttling state is kept between multiple `imap` and `imap_unordered` calls so you don't end up perform some tasks too soon. But keep in mind this state is tied to the `key` function you provide to remain consistent, so if you change the used `key`, the throttling state will be reset.
         
         *Arguments*
         
-        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`.
+        * **max_workers** *(int, optional)*: Maximum number of threads to use. Defaults to `min(32, os.cpu_count() + 1)`. Note that it can be `0`, in which case no threads will be used and everything will run synchronously (this can be useful for debugging or to avoid duplicating code sometimes).
         * **initializer** *(callable, optional)*: Function to run at the start of each thread worker. Can be useful to setup [thread-local data](https://docs.python.org/3/library/threading.html#thread-local-data), for instance. Remember this function must be threadsafe and should not block because the thread pool will wait for each thread to be correctly booted before being able to proceed. If one of the function calls fails, the thread pool will raise a `quenouille.exceptions.BrokenThreadPool` error and terminate immediately.
         * **initargs** *(iterable, optional)*: Arguments to pass to the `initializer` function.
         * **wait** *(bool, optional)* [`True`]: Whether to join worker threads, i.e. wait for them to end, when closing the executor. Set this to `False` if you need to go on quickly without waiting for your worker threads to end when cleaning up the executor's resources. Just note that if you spawn other thread-intensive tasks or other executors afterwards in rapid succession, you might start too many threads at once.
         * **daemonic** *(bool, optional)* [`False`]: whether to spawn daemonic worker. If your worker are daemonic, the interpreter will not wait for them to end when exiting. This can be useful, combined to `wait=False`, for instance, if you want your program to exit as soon as hitting ctrl+C (you might want to avoid this if your threads need to cleanup things on exit as they will be abruptly shut down).
         
         <h4 id="executor-imap">#.imap, #.imap_unordered</h4>
         
@@ -259,15 +259,15 @@
           return 5 + (2 * random())
         ```
         
         #### Caveats regarding exception raising
         
         *Deferred generator usage exception deadlocks*
         
-        If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you will get end up in a deadlock if you raise an exception.
+        If you consume a generator returned by `imap/imap_unordered` somewhere else than where you created it, you may end up in a deadlock if you raise an exception.
         
         This is not important when using `daemonic=True` but you might stumble upon segfaults on exit because of python reasons beyond my control.
         
         ```python
         # Safe
         for item in imap(...):
           raise RuntimeError
```

### Comparing `quenouille-1.7.1/setup.py` & `quenouille-1.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="quenouille",
-    version="1.7.1",
+    version="1.8.0",
     description="A library of multithreaded iterator workflows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/medialab/quenouille",
     license="MIT",
     author="Guillaume Plique",
     author_email="kropotkinepiotr@gmail.com",
```

