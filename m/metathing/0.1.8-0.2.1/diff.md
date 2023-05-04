# Comparing `tmp/metathing-0.1.8.tar.gz` & `tmp/metathing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metathing-0.1.8.tar", last modified: Wed Apr 13 07:21:13 2022, max compression
+gzip compressed data, was "metathing-0.2.1.tar", last modified: Thu May  4 13:59:40 2023, max compression
```

## Comparing `metathing-0.1.8.tar` & `metathing-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-28 11:35:16.000000 metathing-0.1.8/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:21:13.000000 metathing-0.1.8/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)       86 2021-11-28 11:35:16.000000 metathing-0.1.8/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-13 18:23:50.000000 metathing-0.1.8/metathing/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      290 2021-11-13 18:23:51.000000 metathing-0.1.8/metathing/config.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13705 2022-04-13 07:20:57.000000 metathing-0.1.8/metathing/device.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10829 2021-12-17 09:00:21.000000 metathing-0.1.8/metathing/http.py
--rw-r--r--   0 debian    (1000) debian    (1000)      377 2021-12-15 04:04:47.000000 metathing-0.1.8/metathing/metathing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1787 2021-12-13 14:16:16.000000 metathing-0.1.8/metathing/mqtt.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3797 2022-03-29 00:32:33.000000 metathing-0.1.8/metathing/service.py
--rw-r--r--   0 debian    (1000) debian    (1000)      793 2021-12-13 21:44:36.000000 metathing-0.1.8/metathing/sql.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      354 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       10 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2022-04-13 07:21:13.000000 metathing-0.1.8/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)      235 2022-04-13 07:21:09.000000 metathing-0.1.8/setup.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/test/
--rw-r--r--   0 debian    (1000) debian    (1000)      812 2021-11-28 11:35:16.000000 metathing-0.1.8/test/test_basic.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1211 2021-11-28 11:35:16.000000 metathing-0.1.8/test/test_mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.185782 metathing-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 13:59:40.182449 metathing-0.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.172449 metathing-0.2.1/metathing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-25 13:42:49.000000 metathing-0.2.1/metathing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-03-31 12:28:23.000000 metathing-0.2.1/metathing/alarmer.py
+-rw-r--r--   0 root         (0) root         (0)     9007 2023-05-04 13:48:06.000000 metathing-0.2.1/metathing/application.py
+-rw-r--r--   0 root         (0) root         (0)      290 2023-02-25 13:42:49.000000 metathing-0.2.1/metathing/config.py
+-rw-r--r--   0 root         (0) root         (0)    20090 2023-04-22 14:51:16.000000 metathing-0.2.1/metathing/device.py
+-rw-r--r--   0 root         (0) root         (0)    16266 2023-03-31 01:10:23.000000 metathing-0.2.1/metathing/http.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-11 23:36:40.000000 metathing-0.2.1/metathing/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-05-04 13:56:53.000000 metathing-0.2.1/metathing/metathing.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-04-13 16:58:53.000000 metathing-0.2.1/metathing/mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-03-28 12:54:26.000000 metathing-0.2.1/metathing/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.182449 metathing-0.2.1/metathing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 13:59:40.185782 metathing-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-04 13:59:19.000000 metathing-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metathing-0.1.8/metathing/service.py` & `metathing-0.2.1/metathing/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from .config import Config
-from .http import Http
-from .mqtt import Mqtt
-from .sql import Entry, Flow
 import json
-
-from sqlalchemy.sql.expression import true
-from sqlalchemy import create_engine, Integer
-from sqlalchemy.orm import sessionmaker
-
 from pdb import set_trace as stop
 
 
+from .config import Config
+from .http import Http
+from .mqtt import Mqtt
+
 class Service():
     default_config = {
-            "ADDR": "127.0.0.1",
-            "PORT": "10100",
-            "WORKDIR": ".",
-            "MQTT_ADDR": "localhost",
-            "MQTT_PORT": 1883
-        }
+        "ADDR": "127.0.0.1",
+        "PORT": "10100",
+        "WORKDIR": ".",
+        "MQTT_ADDR": "localhost",
+        "MQTT_PORT": 1883
+    }
 
     def __init__(self, cfg: object, srv_name: str):
         self.config = Config(self.default_config)
         self.config.from_object(cfg)
         self.srv_name = srv_name
-        
+
         # print('sqlite:///{0}/dm.db?charset=utf8'.format(self.config["WORKDIR"]))
-        engine = create_engine('sqlite:///{0}/dm.db'.format(self.config["WORKDIR"]))
-        Entry.__table__.create(engine, checkfirst=True)
-        Flow.__table__.create(engine, checkfirst=True)
-        self.sql = sessionmaker(bind=engine)()
+        # engine = create_engine(
+        #     'sqlite:///{0}/dm.db'.format(self.config["WORKDIR"]))
+        # Entry.__table__.create(engine, checkfirst=True)
+        # Flow.__table__.create(engine, checkfirst=True)
+        # self.sql = sessionmaker(bind=engine)() 【弃用SQLITE】
 
-        self.http = Http(self.config, self.srv_name, sql=self.sql)
+        self.http = Http(self.config, self.srv_name)
         self.http.srv = self
-        
+
         self.mqtt = Mqtt(self.config['MQTT_ADDR'], self.config['MQTT_PORT'])
         self.mqtt.srv = self
 
         self.devmodels = {}
+        self.gcbs = {}  # 【弃用】 global callback set, 叠加回调针对单输入多输出的情况
 
     def Bind(self, app):
         self.app = app
         self.app.srv = self
         self.devs = self.app.devs
         self.http.Build()
 
     def AddDev(self, model):
         try:
             return self.app.AddDev(model)
         except Exception as e:
             return e
-    
+
     def UpdateDev(self, model):
         try:
             return self.app.UpdateDev(model)
         except Exception as e:
             return e
-    
+
     def DeleteDev(self, id):
         try:
             return self.app.DeleteDev(id)
         except Exception as e:
             return e
-    
+
     def InitDev(self, model):
         try:
             return self.app.InitDev(model)
         except Exception as e:
             print(e)
             return str(e)
 
     def InitAllDevs(self):
-        models = self.sql.query(Entry).all()
-        flows = self.sql.query(Flow).all()
-        try:
-            for m in models:
-                model = json.loads(m.content)
-                self.InitDev(model)
-                if len(flows) > 0:
-                    for fs in flows:
-                        flowModels = json.loads(fs.content)
-                        for f in flowModels:
-                            if f['dev_id'] == m.id:
-                                self.devs[f['dev_id']].flow('add', srv_name=f['srv_name'], sub_topic=f['sub_topic'], pub_topic=f['pub_topic'], qos=f['qos'] )
-        except Exception as e:
-            print("[InitAllDevs error]:" + e)
-            pass
+        return
+        # models = self.sql.query(Entry).all()
+        # flows = self.sql.query(Flow).all()
+        # try:
+        #     for m in models:
+        #         model = json.loads(m.content)
+        #         self.InitDev(model)
+        #         if len(flows) > 0:
+        #             for fs in flows:
+        #                 flowModels = json.loads(fs.content)
+        #                 for f in flowModels:
+        #                     if f['_dev_id'] == m.id:
+        #                         self.devs[f['_dev_id']].flow(
+        #                             'add', srv_name=f['srv_name'], sub_topic=f['sub_topic'], pub_topic=f['pub_topic'], qos=f['qos'])
+        # except Exception as e:
+        #     print("[InitAllDevs error]")
+        #     print(e)
+        #     pass
 
     # def parse(self, model_str: str) -> object:
-
+    # 以下均弃用
     def ReadProperty(self, key: str, content):
         print("Read property: " + key)
-        try: # Service mode
+        try:  # Service mode
             return getattr(self.app, key)
-        except: # Protocol mode (need implementation)
-            return self.app.ReadProperty(key, content) 
-        
-    def WriteProperty(self, key:str, content):
+        except:  # Protocol mode (need implementation)
+            return self.app.ReadProperty(key, content)
+
+    def WriteProperty(self, key: str, content):
         print("Write property: " + key)
-        print(content)
-        try: # Service
+        # print(content)
+        try:  # Service
             setattr(self.app, key, content)
-        except: # Protocol
+        except:  # Protocol
             return self.app.WriteProperty(key, content)
 
-    def Execute(self, func_name:str, content = None):
+    def Execute(self, func_name: str, content=None):
         print("Execute function: " + func_name)
         if (content == None):
             return getattr(self.app, func_name)()
         else:
-            print(content)
+            # print(content)
             if isinstance(content, str):
                 return getattr(self.app, func_name)(**(json.loads(content)))
             elif isinstance(content, dict):
                 return getattr(self.app, func_name)(**content)
             else:
-                return "Content type is not supported"
+                return "Content type is not supported"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

