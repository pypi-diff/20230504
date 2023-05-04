# Comparing `tmp/gdb_plus-6.1.1.tar.gz` & `tmp/gdb_plus-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.1.1.tar", last modified: Fri Apr 28 13:00:13 2023, max compression
+gzip compressed data, was "gdb_plus-6.1.2.tar", last modified: Thu May  4 11:33:59 2023, max compression
```

## Comparing `gdb_plus-6.1.1.tar` & `gdb_plus-6.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.963025 gdb_plus-6.1.1/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.1/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11478 2023-04-28 13:00:13.961928 gdb_plus-6.1.1/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11238 2023-04-28 10:24:27.000000 gdb_plus-6.1.1/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.913379 gdb_plus-6.1.1/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11017 2023-04-28 08:59:52.000000 gdb_plus-6.1.1/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-04-28 08:06:22.000000 gdb_plus-6.1.1/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    76108 2023-04-28 12:59:02.000000 gdb_plus-6.1.1/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-04-28 08:06:22.000000 gdb_plus-6.1.1/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.942245 gdb_plus-6.1.1/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11478 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-04-28 09:25:00.000000 gdb_plus-6.1.1/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-04-28 13:00:13.963378 gdb_plus-6.1.1/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.944657 gdb_plus-6.1.1/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    17641 2023-04-28 10:40:32.000000 gdb_plus-6.1.1/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.265838 gdb_plus-6.1.2/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.2/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11532 2023-05-04 11:33:59.264915 gdb_plus-6.1.2/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11293 2023-05-04 10:56:05.000000 gdb_plus-6.1.2/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.243924 gdb_plus-6.1.2/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11017 2023-05-04 10:40:58.000000 gdb_plus-6.1.2/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-05-04 10:40:57.000000 gdb_plus-6.1.2/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    76260 2023-05-04 10:49:43.000000 gdb_plus-6.1.2/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-05-04 10:40:58.000000 gdb_plus-6.1.2/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.259086 gdb_plus-6.1.2/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11532 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-05-04 11:30:52.000000 gdb_plus-6.1.2/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-05-04 11:33:59.266155 gdb_plus-6.1.2/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.261759 gdb_plus-6.1.2/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    17663 2023-05-04 11:33:14.000000 gdb_plus-6.1.2/tests/test.py
```

### Comparing `gdb_plus-6.1.1/LICENSE` & `gdb_plus-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.1/PKG-INFO` & `gdb_plus-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.1.1
+Version: 6.1.2
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -262,7 +262,8 @@
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
+* Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.1/README.md` & `gdb_plus-6.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,8 +247,9 @@
 
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
-* Improve ptrace emulation
+* Improve ptrace emulation
+* Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.1/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.1.2/gdb_plus/Inner_Debugger.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.1/gdb_plus/gdb_plus.py` & `gdb_plus-6.1.2/gdb_plus/gdb_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from functools import partial
 from capstone import Cs, CS_ARCH_X86
 from threading import Thread, Event
 from queue import Queue
 from gdb_plus.utils import Arguments, user_regs_struct, context, MyEvent, Breakpoint
 
 RET = b"\xc3"
+DEBUG_OFF = "Debug is off, commands won't be executed"
 
 class Debugger:
     # If possible patch the rpath (spwn and pwninit do it automatically) instead of using env to load the correct libc. This will let you get a shell not having problems trying to preload bash too
     def __init__(self, target: [int, process, str, list], env={}, aslr:bool=True, script:str="", from_start:bool=True, binary:str=None, debug_from: int=None, timeout: int=0.5):
         log.debug(f"debugging {target if binary is None else binary} using arch: {context.arch} [{context.bits}bits]")
 
         self._capstone = None #To decompile assembly for next_inst
@@ -214,15 +215,15 @@
                         self.debug_from_done.set()
                         break
                     else:
                         log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
 
             Thread(target=action).start()
         else:
-            #log.warn_once(FEATURE_SKIPPED)
+            log.warn_once(DEBUG_OFF)
             self.debug_from_done.set()
         return self
 
     # Use as : dbg = Debugger("file").remote(IP, PORT)
     def remote(self, host: str, port: int):
         """
         Define the connection to use when the script is called with argument REMOTE
@@ -252,15 +253,15 @@
     def execute(self, code: str):
         """ 
         Execute a command that does NOT require a wait later
         """
         if self.debugging:
             return self.gdb.execute(code, to_string=True)
         else:
-            log.warn_once("Debug is off, commands won't be executed")
+            log.warn_once(DEBUG_OFF)
 
     # I want a function to restart the process without closing and opening a new one
     # Not working properly
     def reset(self, argv=None, reload_elf=False):
         ...
 
     # Since reset doesn't work
@@ -364,18 +365,21 @@
    ########################## CONTROL FLOW ##########################
 
     # For commands that will make the process run and should handle priority
     def execute_action(self, command, sender=None):
         """
         Wrapper around execute to handle commands that will require a wait
         """
-        self.priority += 1
-        self.__clear_stop(sender if sender is not None else command)
-        self.execute(command)
-
+        if self.debugging:
+            self.priority += 1
+            self.__clear_stop(sender if sender is not None else command)
+            self.execute(command)
+        else:
+            log.warn_once(DEBUG_OFF)
+            
     # TODO make the option to have "until" be non blocking with an event when we reach the address [28/04/23] In other words migrate wait=False to wait=Event()
     def c(self, wait=False, force = False, until = None):
         """
         Continue execution of the process
 
         Arguments:
             wait: Should block your script until the next interruption ?
@@ -414,15 +418,18 @@
         if legacy:
             self.gdb.myStopped.wait(timeout)
         else:
             self.priority_wait()
 
     # This should only be used under the hood, but how do we let the other one to the user without generating problems ? [14/04/23]
     def priority_wait(self):
-        self.gdb.myStopped.priority_wait()
+        if self.debugging:
+            self.gdb.myStopped.priority_wait()
+        else:
+            log.warn_once(DEBUG_OFF)
 
     # problems when I haven't executed anything
     @property
     def running(self):
         return not self.gdb.myStopped.is_set()
 
     @property
@@ -483,15 +490,15 @@
     def interrupt(self):
         """
         Stop the process as you would with ctrl+C in gdb
 
         Warning: can not YET be put inside a callback
         """
         if not self.debugging:
-            #log.warn_once(FEATURE_SKIPPED)
+            log.warn_once(DEBUG_OFF)
             return
         
         # TODO check that self.running is valid and then use execute_action and priority_wait
         if self.running == self.running:
             self.interrupted = True
             self.gdb.myStopped.clear()
             kill(self.inferiors[self._inferior].pid, signal.SIGINT)
@@ -636,15 +643,14 @@
         self.b(address, temporary=True)
         self.execute_action(f"jump *{hex(address)}", sender="jump")
         log.debug("Waiting for jump to conclude")
         self.priority_wait()
 
     # Now can return from anywhere in the function
     # Works only for standard functions (push rbp; mov rbp, rsp; ...; leave; ret;). May crash if used in the libc
-    # Can't I use __saved_ip now ? [28/04/23]
     def ret(self, value: int = None):
         """
         Exit from current function without executing it. 
 
         Warning: Experimental and depends on the stack frame
         """
         log.warn_once(f"ret is still at an experimental stage and may not work properly")
```

### Comparing `gdb_plus-6.1.1/gdb_plus/utils.py` & `gdb_plus-6.1.2/gdb_plus/utils.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.1/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.1.2/gdb_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.1.1
+Version: 6.1.2
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -262,7 +262,8 @@
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
+* Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.1/pyproject.toml` & `gdb_plus-6.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools",
     "wheel",
 ]
 
 [project]
 name = "gdb_plus"
 description = "Python library to automate gdb debugging"
-version = "6.1.1"
+version = "6.1.2"
 authors = [{name = "Edoardo"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "pwntools>=4.5.0",
     "capstone"
 ]
```

### Comparing `gdb_plus-6.1.1/tests/test.py` & `gdb_plus-6.1.2/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		for dbg in self.debuggers:
 			try:
 				dbg.close()
 			except:
 				pass
 		pass
 
-	#@unittest.skip
+	@unittest.skip
 	def test_file_standard(self):
 		print("\ntest_file_standard: ", end="")
 		with context.local(arch="i386", bits=32):
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
 			dbg.c()
 			self.assertEqual(dbg.recv(), b"Let's start the CTF:")
@@ -36,18 +36,20 @@
 	#@unittest.skip
 	def test_noptrace(self):
 		print("\ntest_noptrace: ", end="")
 		with context.local(noptrace = True, arch="i386", bits=32):
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.recv(), b"Let's start the CTF:")
+			dbg.c(wait=False)
+			dbg.c(wait=True)
 			self.assertFalse(dbg.gdb) 
 			dbg.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_remote(self):
 		print("\ntest_remote: ", end="")
 		with context.local(arch="i386", bits=32):
 			args.REMOTE = True
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
 			shellcode = b"\x6a\x0b\x58\x68\x2f\x73\x68\x00\x68\x2f\x62\x69\x6e\x89\xe3\x31\xC9\x31\xD2\xcd\x80"
@@ -60,86 +62,86 @@
 			dbg.p.recv()
 			dbg.p.send(shellcode.ljust(0x2c, b'\x90') + p32(stack))
 			dbg.p.sendline(b"cat /home/start/flag")
 			self.assertEqual(dbg.p.recv().strip(), b"FLAG{Pwn4bl3_tW_1s_y0ur_st4rt}")
 			dbg.close()
 			args.REMOTE = ""
 
-	#@unittest.skip
+	@unittest.skip
 	def test_process(self):
 		print("\ntest_process: ", end="")
 		with context.local(arch="i386", bits=32):
 			p = process("./start")
 			dbg = Debugger(p)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.p.recv(), b"Let's start the CTF:")
 			dbg.close()
 			p.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_pid(self):
 		print("\ntest_pid: ", end="")
 		with context.local(arch="i386", bits=32):
 			p = process("./start")
 			self.assertEqual(type(p.pid), int)
 			dbg = Debugger(p.pid, binary="./start")
 			self.debuggers.append(dbg)
 			dbg.close()
 			p.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_debug_from(self):
 		print("\ntest_debug_from: ", end="")
 		with context.local(arch="amd64", bits=64):
 			dbg = Debugger("./traps_withSymbols", aslr=False, debug_from=0x0401590, timeout=0.4)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.rip, 0x0401590)
 			dbg.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_nonblocking_debug_from(self):
 		print("\ntest_nonblocking_debug_from: ", end="")
 
 		with context.local(arch="i386", bits=32):
 			interaction_finished = Event()
 			dbg = Debugger("./start", aslr=False).debug_from(0x804809d, event=interaction_finished, timeout=0.01)
 			dbg.p.sendline(b"ciao")
 			interaction_finished.set()
 			dbg.debug_from_done.wait()
 			self.assertEqual(dbg.eip, 0x804809d)
 
-#@unittest.skip
+@unittest.skip
 class Debugger_actions(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		with context.local(arch="amd64", bits=64):
 			self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
 
 	# Fail, ho fatto next a mano e ho perso il controllo
-	#@unittest.skip
+	@unittest.skip
 	def test_continue_until(self):
 		print("\ntest_continue_until: ", end="")
 		self.dbg.b(0x403ad7, temporary=True)
 		print("\nPlay with gdb once we hit address 0x403ad7 and then send continue")
 		self.dbg.c(until=0x403adb)
 		self.assertEqual(self.dbg.instruction_pointer, 0x403adb)
 
-#@unittest.skip
+@unittest.skip
 class Debugger_callbacks(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_read_memory(self):
 		print("\ntest_read_memory: ", end="")
 		
 		data = []
 
 		def callback(dbg):
 			dbg.push(dbg.rsi)
@@ -148,15 +150,15 @@
 			return True
 			
 		self.dbg.b(0x400786, callback=callback, temporary=True)
 		self.dbg.c(wait=True)
 
 		self.assertFalse(sum(data))
 
-	#@unittest.skip
+	@unittest.skip
 	def test_no_stop(self):
 		print("\ntest_no_stop: ", end="")
 		def callback(dbg):
 			dbg.b(0x403ad9, temporary=True)
 			return False
 
 		self.dbg.b(0x403ad0, callback=callback, temporary=True)
@@ -165,30 +167,30 @@
 		#self.dbg.b(0x403ad9, temporary=True)
 
 		self.dbg.c(wait=True)
 		#self.dbg.interactive()
 		self.assertEqual(self.dbg.rip, 0x403ad9)
 		self.assertFalse(len(self.dbg.breakpoints))
 
-	#@unittest.skip
+	@unittest.skip
 	def test_step(self):
 		print("\ntest_step: ", end="")
 
 		def callback(dbg):
 			dbg.step()
 			return True
 
 		self.dbg.b(0x403ad0, callback=callback, temporary=True)
 		self.dbg.c(wait=True)
 		self.assertEqual(self.dbg.rip, 0x403ad2)
 
 	# Ricordati di testare anche finish con callback
 
 
-#@unittest.skip
+@unittest.skip
 class Debugger_memory(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.dbg = Debugger("./cube")
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
@@ -221,15 +223,15 @@
 		self.dbg.dealloc(pointer)
 		pointer = self.dbg.alloc(16, heap=False)
 		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 		self.dbg.dealloc(pointer, len=16, heap=False)
 		# remember dealloc in the bss will only delete the last chunk... 
 		self.dbg.close()
 		
-#@unittest.skip
+@unittest.skip
 class Debbuger_fork(unittest.TestCase):
 	from base64 import b64encode
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		warnings.simplefilter("ignore", ImportWarning)
 
 	def tearDown(self):
@@ -244,15 +246,15 @@
 		request.append(b"authorization: Basic " + auth) 
 		if keepAlive:
 			request.append(b"Connection: keep-alive")
 		else:
 			request.append(b"Connection: close")
 		return LINE_TERMINATOR.join(request + [b""])
 
-	#@unittest.skip
+	@unittest.skip
 	def test_continuous_follow(self):
 		print("\ntest_continuous_follow: ", end="")
 		gdbscript = """
 		set detach-on-fork off
 		set follow-fork-mode child
 		"""
 		self.dbg = Debugger("./httpd", aslr=False, script=gdbscript)
@@ -271,15 +273,15 @@
 		self.dbg.execute("inferior 1") # We can't go back while the child is running
 		self.dbg.c()
 		self.dbg.p.sendline(self.http_request(keepAlive=True))
 		self.dbg.wait()
 		self.assertEqual(self.dbg.rip, 0x5555555566d5)
 		self.dbg.close()
 	
-	#@unittest.skip
+	@unittest.skip
 	def test_split(self):
 		print("\ntest_split: ", end="")
 		with context.local(arch = "amd64", bits = 64):
 			CALL_TO_B64DECODE = 0x26d5
 			gdbscript = """
 			set detach-on-fork off
 			continue
@@ -301,15 +303,15 @@
 			#dbg.c()
 			#dbg.wait()
 			dbg.c(wait=True)
 			self.assertEqual(dbg.rip, 0x5555555566d5)
 			dbg.close()
 			child.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_my_split(self):
 		print("\ntest_my_split: ", end="")
 		with context.local(arch = 'amd64'):
 			SYSCALL_RET = 0x04133f6
 			dbg = Debugger("./traps_withSymbols", aslr=False).set_split_on_fork()
 			dbg.elf.symbols["_syscall"] = SYSCALL_RET
 			dbg.c()
@@ -317,15 +319,15 @@
 			pid = dbg.wait_split() # and then for the child to split out
 			child = dbg.children[pid]
 			self.assertEqual(dbg.instruction_pointer, 0x4327a7) # Will continue without interuptions. Get's there waiting for the PTRACE from the child
 			self.assertEqual(child.instruction_pointer, 0x432d37)
 			dbg.close()
 			child.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_ptrace_emulation(self):
 		print("\ntest_ptrace_emulation: ", end="")
 		with context.local(arch = 'amd64'):
 			SYSCALL_RET = 0x04133f6
 			ANTI_DEBUG_TEST_FINISHED = 0x0401590
 			RWX_SECTION = 0x7ffff7ff8000
 			END_UNPACK  = RWX_SECTION + 0x80
@@ -443,15 +445,15 @@
 #			else:
 #				output.append(ni.toString())
 #		self.dbg.step_until_ret(callback)
 #		with open("dump_ExceptionalChecking") as fp:
 #			self.assertEqual(output, fp.read().split("\n"))
 	
 	# Commented out to not slow down too much the tests
-	#@unittest.skip
+	@unittest.skip
 	def test_signal_handler(self):
 		print("\ntest_signal_handler: ", end="")
 		from queue import Queue
 		HANDLER_RET = 0x04011ff
 		CHECK_CALL = 0x0401341
 		self.dbg.p.sendline(b"serial_a_caso")
 		self.dbg.cont(until=CHECK_CALL)
@@ -470,24 +472,24 @@
 				self.dbg.write(self.dbg.instruction_pointer, b"\x90") #Just to avoid problems
 			else:
 				output.append(ni.toString())
 		self.dbg.step_until_ret(callback)
 		with open("dump_ExceptionalChecking") as fp:
 			self.assertEqual(output, fp.read().split("\n"))
 
-#@unittest.skip
+@unittest.skip
 class Debugger_calls(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
 			self.dbg.close()
 
-	#@unittest.skip
+	@unittest.skip
 	def test_call(self):
 		print("\ntest_call: ", end="")
 		out = []
 		self.dbg = Debugger("./cube", from_start=False, aslr=False) # You must wait for the libc to be loaded to call malloc
 		for mossa in [0x00003175, 0x00003e74, 0x000038d9, 0x00001885]:
 			# Create blank cube
 			pointer = self.dbg.alloc(54*8)
```

