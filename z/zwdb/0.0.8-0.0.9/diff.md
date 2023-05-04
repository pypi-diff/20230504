# Comparing `tmp/zwdb-0.0.8.tar.gz` & `tmp/zwdb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zwdb-0.0.8.tar", last modified: Sat Apr 18 03:36:51 2020, max compression
+gzip compressed data, was "dist/zwdb-0.0.9.tar", last modified: Sun Apr 19 12:16:12 2020, max compression
```

## Comparing `zwdb-0.0.8.tar` & `zwdb-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-18 03:36:51.000000 zwdb-0.0.8/
--rw-r--r--   0 yew        (501) staff       (20)     1050 2020-03-04 14:09:07.000000 zwdb-0.0.8/LICENSE
--rw-r--r--   0 yew        (501) staff       (20)       71 2020-03-04 17:32:18.000000 zwdb-0.0.8/MANIFEST.in
--rw-r--r--   0 yew        (501) staff       (20)      468 2020-04-18 03:36:51.000000 zwdb-0.0.8/PKG-INFO
--rw-r--r--   0 yew        (501) staff       (20)       27 2020-03-04 14:04:08.000000 zwdb-0.0.8/README.md
--rw-r--r--   0 yew        (501) staff       (20)       36 2020-04-15 15:13:54.000000 zwdb-0.0.8/requirements.txt
--rw-r--r--   0 yew        (501) staff       (20)       38 2020-04-18 03:36:51.000000 zwdb-0.0.8/setup.cfg
--rw-r--r--   0 yew        (501) staff       (20)     1344 2020-04-18 03:29:59.000000 zwdb-0.0.8/setup.py
-drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-18 03:36:51.000000 zwdb-0.0.8/tests/
--rw-r--r--   0 yew        (501) staff       (20)        0 2020-03-14 15:34:26.000000 zwdb-0.0.8/tests/__init__.py
--rw-r--r--   0 yew        (501) staff       (20)       14 2020-03-09 07:12:25.000000 zwdb-0.0.8/tests/conftest.py
--rw-r--r--   0 yew        (501) staff       (20)     3058 2020-03-19 18:17:03.000000 zwdb-0.0.8/tests/test_mongo.py
--rw-r--r--   0 yew        (501) staff       (20)     4286 2020-04-14 16:08:41.000000 zwdb-0.0.8/tests/test_mysql.py
--rw-r--r--   0 yew        (501) staff       (20)     2119 2020-04-18 03:25:47.000000 zwdb-0.0.8/tests/test_redis.py
--rw-r--r--   0 yew        (501) staff       (20)      591 2020-03-07 14:20:49.000000 zwdb-0.0.8/tests/test_utils.py
-drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb/
--rw-r--r--   0 yew        (501) staff       (20)        0 2020-03-07 16:31:50.000000 zwdb-0.0.8/zwdb/__init__.py
--rw-r--r--   0 yew        (501) staff       (20)      259 2020-04-18 03:26:14.000000 zwdb-0.0.8/zwdb/__version__.py
--rw-r--r--   0 yew        (501) staff       (20)     6496 2020-04-14 16:09:15.000000 zwdb-0.0.8/zwdb/records.py
--rw-r--r--   0 yew        (501) staff       (20)     1094 2020-04-15 15:55:45.000000 zwdb-0.0.8/zwdb/utils.py
--rw-r--r--   0 yew        (501) staff       (20)     6794 2020-03-19 18:19:37.000000 zwdb-0.0.8/zwdb/zwmongo.py
--rw-r--r--   0 yew        (501) staff       (20)     8283 2020-04-14 15:40:31.000000 zwdb-0.0.8/zwdb/zwmysql.py
--rw-r--r--   0 yew        (501) staff       (20)     5861 2020-04-18 03:22:39.000000 zwdb-0.0.8/zwdb/zwredis.py
-drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/
--rw-r--r--   0 yew        (501) staff       (20)      468 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/PKG-INFO
--rw-r--r--   0 yew        (501) staff       (20)      425 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/SOURCES.txt
--rw-r--r--   0 yew        (501) staff       (20)        1 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/dependency_links.txt
--rw-r--r--   0 yew        (501) staff       (20)       37 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/requires.txt
--rw-r--r--   0 yew        (501) staff       (20)        5 2020-04-18 03:36:51.000000 zwdb-0.0.8/zwdb.egg-info/top_level.txt
+drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-19 12:16:12.000000 zwdb-0.0.9/
+-rw-r--r--   0 yew        (501) staff       (20)     1050 2020-03-04 14:09:07.000000 zwdb-0.0.9/LICENSE
+-rw-r--r--   0 yew        (501) staff       (20)       71 2020-03-04 17:32:18.000000 zwdb-0.0.9/MANIFEST.in
+-rw-r--r--   0 yew        (501) staff       (20)      468 2020-04-19 12:16:12.000000 zwdb-0.0.9/PKG-INFO
+-rw-r--r--   0 yew        (501) staff       (20)       27 2020-03-04 14:04:08.000000 zwdb-0.0.9/README.md
+-rw-r--r--   0 yew        (501) staff       (20)       36 2020-04-15 15:13:54.000000 zwdb-0.0.9/requirements.txt
+-rw-r--r--   0 yew        (501) staff       (20)       38 2020-04-19 12:16:12.000000 zwdb-0.0.9/setup.cfg
+-rw-r--r--   0 yew        (501) staff       (20)     1349 2020-04-18 15:31:58.000000 zwdb-0.0.9/setup.py
+drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-19 12:16:12.000000 zwdb-0.0.9/tests/
+-rw-r--r--   0 yew        (501) staff       (20)        0 2020-03-14 15:34:26.000000 zwdb-0.0.9/tests/__init__.py
+-rw-r--r--   0 yew        (501) staff       (20)       14 2020-03-09 07:12:25.000000 zwdb-0.0.9/tests/conftest.py
+-rw-r--r--   0 yew        (501) staff       (20)     3058 2020-03-19 18:17:03.000000 zwdb-0.0.9/tests/test_mongo.py
+-rw-r--r--   0 yew        (501) staff       (20)     4540 2020-04-19 12:14:58.000000 zwdb-0.0.9/tests/test_mysql.py
+-rw-r--r--   0 yew        (501) staff       (20)     2119 2020-04-18 03:25:47.000000 zwdb-0.0.9/tests/test_redis.py
+-rw-r--r--   0 yew        (501) staff       (20)      591 2020-03-07 14:20:49.000000 zwdb-0.0.9/tests/test_utils.py
+drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb/
+-rw-r--r--   0 yew        (501) staff       (20)        0 2020-03-07 16:31:50.000000 zwdb-0.0.9/zwdb/__init__.py
+-rw-r--r--   0 yew        (501) staff       (20)      259 2020-04-19 12:15:27.000000 zwdb-0.0.9/zwdb/__version__.py
+-rw-r--r--   0 yew        (501) staff       (20)     6496 2020-04-14 16:09:15.000000 zwdb-0.0.9/zwdb/records.py
+-rw-r--r--   0 yew        (501) staff       (20)     1094 2020-04-15 15:55:45.000000 zwdb-0.0.9/zwdb/utils.py
+-rw-r--r--   0 yew        (501) staff       (20)     6794 2020-03-19 18:19:37.000000 zwdb-0.0.9/zwdb/zwmongo.py
+-rw-r--r--   0 yew        (501) staff       (20)     8974 2020-04-19 12:12:28.000000 zwdb-0.0.9/zwdb/zwmysql.py
+-rw-r--r--   0 yew        (501) staff       (20)     5861 2020-04-18 03:22:39.000000 zwdb-0.0.9/zwdb/zwredis.py
+drwxr-xr-x   0 yew        (501) staff       (20)        0 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/
+-rw-r--r--   0 yew        (501) staff       (20)      468 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/PKG-INFO
+-rw-r--r--   0 yew        (501) staff       (20)      425 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/SOURCES.txt
+-rw-r--r--   0 yew        (501) staff       (20)        1 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/dependency_links.txt
+-rw-r--r--   0 yew        (501) staff       (20)       37 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/requires.txt
+-rw-r--r--   0 yew        (501) staff       (20)       11 2020-04-19 12:16:12.000000 zwdb-0.0.9/zwdb.egg-info/top_level.txt
```

### Comparing `zwdb-0.0.8/LICENSE` & `zwdb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/setup.py` & `zwdb-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 from setuptools import setup, find_packages
 from codecs import open
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 pkg_name = 'zwdb'
-packages = [pkg_name]
+packages = find_packages()
 
 requires = [s.strip() for s in open('requirements.txt').readlines()]
 test_requirements = [s.strip() for s in open('requirements_dev.txt').readlines()][4:]
 
 shutil.rmtree('dist', ignore_errors=True)
 about = {}
 with open(os.path.join(here, pkg_name, '__version__.py'), 'r', 'utf-8') as f:
```

### Comparing `zwdb-0.0.8/tests/test_mongo.py` & `zwdb-0.0.9/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/tests/test_mysql.py` & `zwdb-0.0.9/tests/test_mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             fs = ','.join(ks)
             vs = ','.join(['%({})s'.format(s) for s in ks])
             stmt = 'INSERT INTO tbl ({}) VALUES({})'.format(fs, vs)
             conn.executemany(stmt, fetchall=False, commit=True, paramslist=recs_insert)
         yield dbobj
         # clean
         with dbobj.get_connection() as conn:
-            tbls = ['tbl', 'tbl_insert']
+            tbls = ['tbl', 'tbl_insert', 'tbl_create']
             for t in tbls:
                 conn.execute('DROP TABLE IF EXISTS %s'%t, commit=True)
 
 class TestMysql:
     def test_list(self, db):
         assert len(db.lists())>0
     
@@ -116,8 +116,14 @@
             ([{'id':1},{'id':3}], ['id']),
         )
     )
     def test_delete(self, db, recs, keyflds):
         tbl = 'tbl_insert'
         c = db.delete('tbl_insert', recs, keyflds=keyflds)
         total_recs = db.find(tbl, fetchall=True)
-        assert c == 2 and 1 == len(total_recs)
+        assert c == 2 and 1 == len(total_recs)
+    
+    def test_exec_script(self, db):
+        r = db.exec_script('data/tbl_create.sql')
+        with db.get_connection() as conn:
+            rs = conn.execute("show tables like 'tbl_create';", fetchall=True)
+        assert len(rs) == 1
```

### Comparing `zwdb-0.0.8/tests/test_redis.py` & `zwdb-0.0.9/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/tests/test_utils.py` & `zwdb-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/zwdb/records.py` & `zwdb-0.0.9/zwdb/records.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/zwdb/utils.py` & `zwdb-0.0.9/zwdb/utils.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/zwdb/zwmongo.py` & `zwdb-0.0.9/zwdb/zwmongo.py`

 * *Files identical despite different names*

### Comparing `zwdb-0.0.8/zwdb/zwmysql.py` & `zwdb-0.0.9/zwdb/zwmysql.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,28 +82,43 @@
             rtn = conn.upsert(tbl, recs, keyflds)
         return rtn
 
     def delete(self, tbl, recs, keyflds):
         with self.get_connection() as conn:
             rtn = conn.delete(tbl, recs, keyflds)
         return rtn
+    
+    def exec_script(self, fp):
+        with self.get_connection() as conn:
+            cursor = conn._conn.cursor()
+            statement = ''
+            for line in open(fp):
+                if line.strip().startswith('--'):  # ignore sql comment lines
+                    continue
+                if not line.strip().endswith(';'):  # keep appending lines that don't end in ';'
+                    statement = statement + line
+                else:  # when you get a line ending in ';' then exec statement and reset for next statement
+                    statement = statement + line
+                    cursor.execute(statement)
+                    statement = ''
+        return True
 
     @contextmanager
     def transaction(self):
         """A context manager for executing a transaction on this Database."""
-        pass
-        # conn = self.get_connection()
-        # tx = conn.transaction()
-        # try:
-        #     yield conn
-        #     tx.commit()
-        # except:
-        #     tx.rollback()
-        # finally:
-        #     conn.close()
+        conn = self.get_connection()
+        _conn = conn._conn
+        tx = _conn.transaction()
+        try:
+            yield conn
+            tx.commit()
+        except:
+            tx.rollback()
+        finally:
+            _conn.close()
 
     def __repr__(self):
         return '<Database host={}:{}>'.format(self.dbcfg['host'], self.dbcfg['port'])
 
     def __enter__(self):
         return self
```

### Comparing `zwdb-0.0.8/zwdb/zwredis.py` & `zwdb-0.0.9/zwdb/zwredis.py`

 * *Files identical despite different names*

