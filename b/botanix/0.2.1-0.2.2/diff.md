# Comparing `tmp/botanix-0.2.1.tar.gz` & `tmp/botanix-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botanix-0.2.1.tar", last modified: Wed May  3 18:52:41 2023, max compression
+gzip compressed data, was "botanix-0.2.2.tar", last modified: Wed May  3 21:59:52 2023, max compression
```

## Comparing `botanix-0.2.1.tar` & `botanix-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 18:52:41.931179 botanix-0.2.1/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.2.1/LICENSE
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 18:52:41.931299 botanix-0.2.1/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8991 2023-05-01 07:52:10.000000 botanix-0.2.1/README.md
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 18:52:41.928248 botanix-0.2.1/botanix/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.2.1/botanix/__init__.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.2.1/botanix/conversion_helper.py
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8396 2023-05-03 17:56:28.000000 botanix-0.2.1/botanix/handling.py
-drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 18:52:41.930913 botanix-0.2.1/botanix.egg-info/
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 18:52:41.000000 botanix-0.2.1/botanix.egg-info/PKG-INFO
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-05-03 18:52:41.000000 botanix-0.2.1/botanix.egg-info/SOURCES.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-05-03 18:52:41.000000 botanix-0.2.1/botanix.egg-info/dependency_links.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-05-03 18:52:41.000000 botanix-0.2.1/botanix.egg-info/requires.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-05-03 18:52:41.000000 botanix-0.2.1/botanix.egg-info/top_level.txt
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-05-03 18:52:41.931781 botanix-0.2.1/setup.cfg
--rw-r--r--   0 alikheyrollahi   (501) staff       (20)      383 2023-05-03 18:52:37.000000 botanix-0.2.1/setup.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.097531 botanix-0.2.2/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     1072 2023-01-17 08:12:09.000000 botanix-0.2.2/LICENSE
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 21:59:52.097678 botanix-0.2.2/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8991 2023-05-01 07:52:10.000000 botanix-0.2.2/README.md
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.094570 botanix-0.2.2/botanix/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        0 2023-01-19 20:24:06.000000 botanix-0.2.2/botanix/__init__.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      569 2023-01-19 19:54:23.000000 botanix-0.2.2/botanix/conversion_helper.py
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)     8392 2023-05-03 19:15:01.000000 botanix-0.2.2/botanix/handling.py
+drwxr-xr-x   0 alikheyrollahi   (501) staff       (20)        0 2023-05-03 21:59:52.097225 botanix-0.2.2/botanix.egg-info/
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      213 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/PKG-INFO
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      259 2023-05-03 21:59:52.000000 botanix-0.2.2/botanix.egg-info/SOURCES.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        1 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/dependency_links.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)       20 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/requires.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)        8 2023-05-03 21:59:51.000000 botanix-0.2.2/botanix.egg-info/top_level.txt
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      103 2023-05-03 21:59:52.098250 botanix-0.2.2/setup.cfg
+-rw-r--r--   0 alikheyrollahi   (501) staff       (20)      383 2023-05-03 21:59:43.000000 botanix-0.2.2/setup.py
```

### Comparing `botanix-0.2.1/LICENSE` & `botanix-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botanix-0.2.1/README.md` & `botanix-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `botanix-0.2.1/botanix/conversion_helper.py` & `botanix-0.2.2/botanix/conversion_helper.py`

 * *Files identical despite different names*

### Comparing `botanix-0.2.1/botanix/handling.py` & `botanix-0.2.2/botanix/handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
       if class_command in MainHandler.generic_handler_names:
         ctx = HandlingContext(uid, track_nam=class_command) # create a dummy context and not store since they do not have follow up
       else:
         ctx = self.store.new_context(uid, class_command)  # renew context
       return await self._do_handle(uid, message_text, update, ctx, class_command)
 
   async def _do_handle(self, uid: int, command: str, update: Update, context: HandlingContext, class_command: str) -> HandlingResult:
-    result = await self.handlers[class_command].handle(uid, command, update, context)
+    result = await self.handlers[class_command].handle( command, update, context)
     if result.handled and not result.is_terminal:
       if result.step_override is None:
         context.move_to_next()  # increase the step
       else:
         context.override_step(result.step_override)  # change the step
       self.store.put_context(uid, context)
     if result.is_terminal:
```

