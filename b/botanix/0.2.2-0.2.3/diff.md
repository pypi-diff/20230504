# Comparing `tmp/botanix-0.2.2.tar.gz` & `tmp/botanix-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botanix-0.2.2.tar", last modified: Wed May  3 21:59:52 2023, max compression
+gzip compressed data, was "botanix-0.2.3.tar", last modified: Thu May  4 09:19:32 2023, max compression
```

## Comparing `botanix-0.2.2.tar` & `botanix-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.097531 botanix-0.2.2/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.2.2/LICENSE
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 21:59:52.097678 botanix-0.2.2/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8991 2023-05-01 07:52:10.000000 botanix-0.2.2/README.md
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.094570 botanix-0.2.2/botanix/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.2.2/botanix/__init__.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.2.2/botanix/conversion_helper.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8392 2023-05-03 19:15:01.000000 botanix-0.2.2/botanix/handling.py
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.097225 botanix-0.2.2/botanix.egg-info/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-05-03 21:59:52.000000 botanix-0.2.2/botanix.egg-info/SOURCES.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/dependency_links.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/requires.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/top_level.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-05-03 21:59:52.098250 botanix-0.2.2/setup.cfg
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      383 2023-05-03 21:59:43.000000 botanix-0.2.2/setup.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-04 09:19:32.286116 botanix-0.2.3/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.2.3/LICENSE
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-04 09:19:32.286219 botanix-0.2.3/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8991 2023-05-01 07:52:10.000000 botanix-0.2.3/README.md
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-04 09:19:32.284281 botanix-0.2.3/botanix/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.2.3/botanix/__init__.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.2.3/botanix/conversion_helper.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8371 2023-05-04 09:18:13.000000 botanix-0.2.3/botanix/handling.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-04 09:19:32.285874 botanix-0.2.3/botanix.egg-info/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-04 09:19:32.000000 botanix-0.2.3/botanix.egg-info/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-05-04 09:19:32.000000 botanix-0.2.3/botanix.egg-info/SOURCES.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-05-04 09:19:32.000000 botanix-0.2.3/botanix.egg-info/dependency_links.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-05-04 09:19:32.000000 botanix-0.2.3/botanix.egg-info/requires.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-05-04 09:19:32.000000 botanix-0.2.3/botanix.egg-info/top_level.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-05-04 09:19:32.286646 botanix-0.2.3/setup.cfg
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      383 2023-05-04 09:10:20.000000 botanix-0.2.3/setup.py
```

### Comparing `botanix-0.2.2/LICENSE` & `botanix-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botanix-0.2.2/README.md` & `botanix-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `botanix-0.2.2/botanix/conversion_helper.py` & `botanix-0.2.3/botanix/conversion_helper.py`

 * *Files identical despite different names*

### Comparing `botanix-0.2.2/botanix/handling.py` & `botanix-0.2.3/botanix/handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
   def override_step(self, step:int):
     self.step = step
 
   def get_custom(self, key:str):
     return self.custom[key]
 
-  def to_string(self) -> str:
+  def to_json_string(self) -> str:
     cop = self.__dict__.copy()
     decimal_to_int_for_shallow_graph(cop)
     return json.dumps(cop)
 
   @staticmethod
-  def from_string(json_s:str):
+  def from_json_string(json_s:str):
     dic = json.loads(json_s)
     ctx = HandlingContext(123, 'dummy')
     ctx.__dict__ = dic
     ctx.timestamp = Decimal(ctx.timestamp)
     return ctx
 
 
@@ -183,18 +183,17 @@
     Creates, stores and returns a new context
     :param uid:
     :param track_nam:
     :return:
     """
     pass
 
-  def put_context(self, uid: int, context: HandlingContext) -> None:
+  def put_context(self, context: HandlingContext) -> None:
     """
     Updates the stored context
-    :param uid:
     :param context:
     :return:
     """
     pass
 
   def clear_context(self, uid: int):
     """
@@ -241,12 +240,12 @@
   async def _do_handle(self, uid: int, command: str, update: Update, context: HandlingContext, class_command: str) -> HandlingResult:
     result = await self.handlers[class_command].handle( command, update, context)
     if result.handled and not result.is_terminal:
       if result.step_override is None:
         context.move_to_next()  # increase the step
       else:
         context.override_step(result.step_override)  # change the step
-      self.store.put_context(uid, context)
+      self.store.put_context(context)
     if result.is_terminal:
       self.store.clear_context(uid)
     return result
```

