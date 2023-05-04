# Comparing `tmp/sentenai-1.6.4.6.tar.gz` & `tmp/sentenai-1.6.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentenai-1.6.4.6.tar", last modified: Sat Apr 29 11:29:13 2023, max compression
+gzip compressed data, was "dist/sentenai-1.6.4.7.tar", last modified: Thu May  4 20:21:49 2023, max compression
```

## Comparing `sentenai-1.6.4.6.tar` & `sentenai-1.6.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.593172 sentenai-1.6.4.6/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.6/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-29 11:29:13.593247 sentenai-1.6.4.6/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.6/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.591657 sentenai-1.6.4.6/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9068 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.593016 sentenai-1.6.4.6/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       53 2022-10-04 21:43:28.000000 sentenai-1.6.4.6/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.6/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.6/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24627 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-04-29 11:29:13.592201 sentenai-1.6.4.6/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-04-29 11:29:13.000000 sentenai-1.6.4.6/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-04-29 11:29:13.593482 sentenai-1.6.4.6/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-04-29 11:28:45.000000 sentenai-1.6.4.6/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.7/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.7/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     8918 2023-04-30 01:51:32.000000 sentenai-1.6.4.7/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.7/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.4.7/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.7/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.7/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    19914 2023-05-04 20:20:46.000000 sentenai-1.6.4.7/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-05-04 20:21:49.000000 sentenai-1.6.4.7/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-05-04 20:21:23.000000 sentenai-1.6.4.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sentenai-1.6.4.6/LICENSE` & `sentenai-1.6.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.6/PKG-INFO` & `sentenai-1.6.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.6
+Version: 1.6.4.7
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.6/README.md` & `sentenai-1.6.4.7/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.6/sentenai/__init__.py` & `sentenai-1.6.4.7/sentenai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,19 +148,15 @@
             return {'start': dt64(self._info['start']), 'end': dt64(self._info['end'])}
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
             return self.range
 
     @property
     def origin(self):
-        if self._info:
-            return dt64(self._info.get('origin'))
-        else:
-            self._info = self._post("range", json=self._tspl['value']).json()
-            return self.origin
+        return dt64(self.explain()['origin'])
 
     @property
     def type(self):
         if self._info:
             return self._info.get('type')
         else:
             self._info = self._post("range", json=self._tspl['value']).json()
```

### Comparing `sentenai-1.6.4.6/sentenai/api.py` & `sentenai-1.6.4.7/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.6/sentenai/stream/events.py` & `sentenai-1.6.4.7/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.6/sentenai/stream/metadata.py` & `sentenai-1.6.4.7/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.6/sentenai/stream/streams.py` & `sentenai-1.6.4.7/sentenai/stream/streams.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,162 +56,14 @@
         else:
             if resp.status_code > 204:
                 resp.close()
                 raise Exception(f"failed on row {i}, column {k}")
             resp.close()
             break
 
-class WQueue(Queue):
-    def write(self, data):
-        if data:
-            j = {}
-            if data.id:
-                j['id'] = id
-            if not data.start:
-                j['ts'] = dt64(datetime.utcnow())
-            else:
-                j['ts'] = dt64(data.start)
-            if data.end:
-                j['duration'] = int((dt64(data.end) - dt64(j['ts'])).astype('timedelta64[ns]'))
-            j['event'] = data.data
-            self.put((JSON.dumps(j, ignore_nan=True, cls=SentenaiEncoder) + "\n").encode('utf-8'))
-
-    def __iter__(self):
-        return iter(self.get, None)
-
-    def gen(self):
-        while True:
-            x = self.get()
-            if x is None:
-                break
-            else:
-                yield x
-
-    def close(self):
-        self.put(None)
-
-class Logger(Thread):
-
-    def join(self, timeout=None):
-        super(Logger, self).join(timeout)
-        if self._exc: raise self._exc
-
-    def run(self):
-        self._exc = None
-        try:
-            self.ret = self._target(*self._args, **self._kwargs)
-        except BaseException as e:
-            self._exc = e
-
-class Log(object):
-    def __init__(self, parent):
-        self._queue = WQueue(1000)
-        self._parent = parent
-        self._thread = Logger(target=self._post)
-        self._thread.start()
-        self._exc = None
-
-    def _post(self):
-        self._parent._post(json=self._queue.gen())
-
-
-    def __setitem__(self, item, data):
-        if isinstance(item, slice):
-            if item.start is None:
-                raise ValueError("start time must be specified")
-            elif item.stop and item.start >= item.stop:
-                raise ValueError("end time must be after start time")
-            else:
-                self._queue.write(Update(start=item.start, end=item.stop, id=item.step, data=data))
-        else:
-            raise ValueError("Must be a slice of the form `start : end* : id*`, where `*` indicates optional)")
-
-
-
-
-class Updates(API):
-    def __init__(self, parent):
-        API.__init__(self, parent._credentials, *parent._prefix, "events")
-        self._log = None
-        self._parent = parent
-
-    def __setitem__(self, item, data):
-        hdrs = {'content-type': 'application/json'}
-        if isinstance(item, slice):
-            if item.start is None:
-                raise ValueError("start time must be specified")
-            elif item.stop and item.start >= item.stop:
-                raise ValueError("end time must be after start time")
-            else:
-                if item.start is not None and item.stop is None:
-                    hdrs["timestamp"] = iso8601(item.start)
-                elif item.stop is not None:
-                    hdrs['start'] = iso8601(item.start)
-                    hdrs["end"] = iso8601(item.stop)
-                if item.step is None:
-                    r = self._post(headers=hdrs, json=data)
-                else:
-                    r = self._put(item.step, headers=hdrs, json=data)
-                if 300 > r.status_code >= 200:
-                    return None
-                else:
-                    raise Exception(r.status_code)
-        else:
-            raise ValueError("Must be a slice of the form `start : end* : id*`, where `*` indicates optional)")
-
-    def __enter__(self):
-        self._log = Log(self._parent)
-        return self._log
-
-    def __exit__(self, x, y, z):
-        self._log._queue.close()
-        self._log._thread.join()
-        self._log = None
-
-    def __delitem__(self, item):
-        if isinstance(item, slice):
-            raise TypeError("slice not supported for deleting updates.")
-        else:
-            r = self._delete(item)
-            if r.status_code == 204:
-                return None
-            else:
-                raise Exception(r.status_code)
-
-
-    def __getitem__(self, item):
-        if isinstance(item, slice):
-            params = {}
-            if item.start is not None:
-                params['start'] = iso8601(item.start)
-            if item.stop is not None:
-                params['end'] = iso8601(item.stop)
-            if item.step is not None:
-                params['limit'] = abs(item.step)
-                if item.step < 0:
-                    params['sort'] = 'desc'
-            r = self._get(params=params)
-            if r.status_code == 200:
-                data = []
-                for line in r.json():
-                    data.append({
-                        'start': dt64(line['ts']),
-                        'end': dt64(line['ts']) + td64(line['duration']) if line['duration'] else None,
-                        'data': line['event'],
-                    })
-                return data
-            else:
-                raise Exception(r.json())
-        else:
-            r = self._get(item)
-            if r.status_code == 404:
-                raise KeyError(f"Update with id `{item}` not found.")
-            else:
-                return r.json()
-
 
 class Database(API):
     def __init__(self, parent, name, origin):
         self._parent = parent
         self._name = name
         self._origin = origin
         API.__init__(self, parent._credentials, *parent._prefix, "db", name)
@@ -446,14 +298,23 @@
     def origin(self):
         return self._origin
 
     @property
     def name(self):
         return self._name
 
+class Node(API):
+    def __init__(self, db, node):
+        self._node = node
+        API.__init__(self, db._credentials, *db._prefix, "nodes", self._node)
+
+    @property
+    def meta(self):
+        return Metadata(self)
+
 class Stream(API):
     def __init__(self, parent, *path):
         self._parent = parent
         self._path = path
         r = self._parent._get('paths', *path)
         if r.status_code == 404:
             raise KeyError("path does not exist")
```

### Comparing `sentenai-1.6.4.6/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.7/sentenai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.6
+Version: 1.6.4.7
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.6/setup.py` & `sentenai-1.6.4.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.6',
+    version='1.6.4.7',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

