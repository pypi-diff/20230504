# Comparing `tmp/bytecodemanipulation-0.2.2.tar.gz` & `tmp/bytecodemanipulation-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.2.2.tar", last modified: Sun Dec 25 10:37:22 2022, max compression
+gzip compressed data, was "bytecodemanipulation-0.2.4.tar", last modified: Thu May  4 14:18:13 2023, max compression
```

## Comparing `bytecodemanipulation-0.2.2.tar` & `bytecodemanipulation-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.594025 bytecodemanipulation-0.2.2/
--rw-rw-rw-   0        0        0     1082 2022-01-23 14:31:25.000000 bytecodemanipulation-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4852 2022-12-25 10:37:22.592885 bytecodemanipulation-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4134 2022-12-09 13:58:59.000000 bytecodemanipulation-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.539785 bytecodemanipulation-0.2.2/bytecodemanipulation/
--rw-rw-rw-   0        0        0    20382 2022-11-21 16:43:58.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/Emulator.py
--rw-rw-rw-   0        0        0    20602 2022-11-21 08:48:14.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/Mixin.py
--rw-rw-rw-   0        0        0    44361 2022-12-15 07:45:56.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/MutableFunction.py
--rw-rw-rw-   0        0        0    10374 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/MutableFunctionHelpers.py
--rw-rw-rw-   0        0        0     4677 2022-11-20 14:47:40.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/Opcodes.py
--rw-rw-rw-   0        0        0    25765 2022-12-16 18:32:55.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/Optimiser.py
--rw-rw-rw-   0        0        0     6369 2022-11-19 21:53:29.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/Specialization.py
--rw-rw-rw-   0        0        0      167 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/__init__.py
--rw-rw-rw-   0        0        0       53 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/annotated_std.py
--rw-rw-rw-   0        0        0     2532 2022-11-27 09:34:20.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/compiler.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.557462 bytecodemanipulation-0.2.2/bytecodemanipulation/data/
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.575034 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/
--rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/__init__.py
--rw-rw-rw-   0        0        0      218 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/builtins.json
--rw-rw-rw-   0        0        0     1429 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/instruction_spec.json
--rw-rw-rw-   0        0        0     2854 2022-11-20 14:49:21.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/opcodes.json
--rw-rw-rw-   0        0        0       52 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/specialize.py
--rw-rw-rw-   0        0        0      772 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_10/standard_library.json
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.578041 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_11/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:49:51.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_11/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.580319 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_12/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:50:05.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_12/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.583996 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_9/
--rw-rw-rw-   0        0        0        0 2022-11-26 17:49:58.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/3_9/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.589872 bytecodemanipulation-0.2.2/bytecodemanipulation/data/shared/
--rw-rw-rw-   0        0        0       28 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/shared/__init__.py
--rw-rw-rw-   0        0        0     7989 2022-12-16 19:47:43.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data/shared/builtin_spec.py
--rw-rw-rw-   0        0        0     2403 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/data_loader.py
--rw-rw-rw-   0        0        0     3864 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/mixin_util.py
--rw-rw-rw-   0        0        0      436 2022-11-20 13:43:30.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/optimise_self.py
--rw-rw-rw-   0        0        0    17510 2022-12-15 07:46:36.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/optimiser_util.py
--rw-rw-rw-   0        0        0      455 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.2/bytecodemanipulation/util.py
-drwxrwxrwx   0        0        0        0 2022-12-25 10:37:22.554125 bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/
--rw-rw-rw-   0        0        0     4852 2022-12-25 10:37:22.000000 bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1296 2022-12-25 10:37:22.000000 bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-25 10:37:22.000000 bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-12-25 10:37:22.000000 bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-01-27 09:48:33.000000 bytecodemanipulation-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-25 10:37:22.595047 bytecodemanipulation-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1360 2022-12-25 10:37:00.000000 bytecodemanipulation-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.448355 bytecodemanipulation-0.2.4/
+-rw-rw-rw-   0        0        0     1082 2022-01-23 14:31:25.000000 bytecodemanipulation-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5572 2023-05-04 14:18:13.446350 bytecodemanipulation-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4854 2023-05-03 20:01:14.000000 bytecodemanipulation-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.260793 bytecodemanipulation-0.2.4/bytecodemanipulation/
+-rw-rw-rw-   0        0        0    22555 2023-01-08 18:17:44.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Emulator.py
+-rw-rw-rw-   0        0        0    20982 2023-01-15 10:09:48.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Mixin.py
+-rw-rw-rw-   0        0        0    54236 2023-05-04 14:08:30.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunction.py
+-rw-rw-rw-   0        0        0    12635 2023-05-04 14:15:29.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-rw-rw-   0        0        0     5578 2023-05-02 17:20:16.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Opcodes.py
+-rw-rw-rw-   0        0        0    27090 2023-05-04 14:05:25.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Optimiser.py
+-rw-rw-rw-   0        0        0    11943 2023-05-03 20:02:56.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/Specialization.py
+-rw-rw-rw-   0        0        0      165 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/__init__.py
+-rw-rw-rw-   0        0        0       53 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/annotated_std.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.310264 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/
+-rw-rw-rw-   0        0        0    11767 2023-05-04 14:11:24.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Emitter.py
+-rw-rw-rw-   0        0        0     5543 2023-05-04 09:43:13.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Lexer.py
+-rw-rw-rw-   0        0        0    74735 2023-05-04 14:14:17.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/Parser.py
+-rw-rw-rw-   0        0        0        0 2023-01-11 16:22:00.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/__init__.py
+-rw-rw-rw-   0        0        0     1570 2023-05-02 12:53:48.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/hook.py
+-rw-rw-rw-   0        0        0     3430 2023-05-04 07:22:54.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/target.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.330884 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/
+-rw-rw-rw-   0        0        0      351 2023-01-06 18:03:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-rw-rw-   0        0        0        0 2023-01-13 11:24:36.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/__init__.py
+-rw-rw-rw-   0        0        0    11291 2023-05-04 09:24:29.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/parser.py
+-rw-rw-rw-   0        0        0     8566 2023-05-02 12:34:49.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/assembler/util/tokenizer.py
+-rw-rw-rw-   0        0        0     2530 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/compiler.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.337601 bytecodemanipulation-0.2.4/bytecodemanipulation/data/
+-rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.347132 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/
+-rw-rw-rw-   0        0        0       28 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/__init__.py
+-rw-rw-rw-   0        0        0    13614 2023-05-03 20:02:56.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/shared/builtin_spec.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.364157 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/
+-rw-rw-rw-   0        0        0        0 2022-11-18 20:41:26.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/__init__.py
+-rw-rw-rw-   0        0        0    80683 2023-05-04 14:13:06.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/assembly_instructions.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_10/specialize.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.384909 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/
+-rw-rw-rw-   0        0        0        0 2022-11-26 17:49:51.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/__init__.py
+-rw-rw-rw-   0        0        0    78725 2023-05-04 14:13:06.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/assembly_instructions.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 18:17:42.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_11/specialize.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.390895 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_12/
+-rw-rw-rw-   0        0        0        0 2022-11-26 17:50:05.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_12/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.397909 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_9/
+-rw-rw-rw-   0        0        0        0 2022-11-26 17:49:58.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data/v3_9/__init__.py
+-rw-rw-rw-   0        0        0     2940 2023-03-25 14:33:01.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/data_loader.py
+-rw-rw-rw-   0        0        0     4233 2023-01-08 18:17:43.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/mixin_util.py
+-rw-rw-rw-   0        0        0      455 2023-01-08 18:17:43.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/optimise_self.py
+-rw-rw-rw-   0        0        0    17871 2023-05-04 14:07:34.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/optimiser_util.py
+-rw-rw-rw-   0        0        0      652 2023-01-14 14:32:32.000000 bytecodemanipulation-0.2.4/bytecodemanipulation/util.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.280710 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/
+-rw-rw-rw-   0        0        0     5572 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1894 2023-05-04 14:18:13.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-04 14:18:12.000000 bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-01-27 09:48:33.000000 bytecodemanipulation-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:18:13.449354 bytecodemanipulation-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-05-04 14:17:31.000000 bytecodemanipulation-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:18:13.439986 bytecodemanipulation-0.2.4/tests/
+-rw-rw-rw-   0        0        0    46901 2023-05-04 14:06:22.000000 bytecodemanipulation-0.2.4/tests/test_Assembly.py
+-rw-rw-rw-   0        0        0     3278 2023-01-15 08:18:00.000000 bytecodemanipulation-0.2.4/tests/test_Mixin.py
+-rw-rw-rw-   0        0        0     1648 2022-11-19 21:26:32.000000 bytecodemanipulation-0.2.4/tests/test_MutableFunction.py
+-rw-rw-rw-   0        0        0      792 2023-05-04 14:06:22.000000 bytecodemanipulation-0.2.4/tests/test_MutableFunctionHelper.py
+-rw-rw-rw-   0        0        0     4932 2023-05-04 13:27:16.000000 bytecodemanipulation-0.2.4/tests/test_StandardLibrary.py
+-rw-rw-rw-   0        0        0     5944 2023-05-04 14:06:55.000000 bytecodemanipulation-0.2.4/tests/test_issues.py
+-rw-rw-rw-   0        0        0    10760 2023-05-04 14:16:08.000000 bytecodemanipulation-0.2.4/tests/test_optimiser_util.py
```

### Comparing `bytecodemanipulation-0.2.2/LICENSE` & `bytecodemanipulation-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.2/PKG-INFO` & `bytecodemanipulation-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: bytecodemanipulation
-Version: 0.2.2
-Summary: High level python bytecode manipulation
-Home-page: https://github.com/uuk0/PyBytecodeManipulator
-Author: uuk
-Author-email: uuk1301@gmail.com
-Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyBytecodeManipulator
 A high level cross-version python bytecode manipulation library build ontop 
 of 'dis' and 'inspect' 
 
 Supports code inlining, branch removing and arbitrary code injection into 
 existing functions.
 
@@ -82,30 +64,42 @@
 # Examples
 
 TODO
 
 
 # Applied Optimisations
 
-- Constant Expression inlining
+- Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
 - With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
 - During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
 - Method inlining is not working properly and needs a lot more testing
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
 
 
 ## Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
```

### Comparing `bytecodemanipulation-0.2.2/README.md` & `bytecodemanipulation-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: bytecodemanipulation
+Version: 0.2.4
+Summary: High level python bytecode manipulation
+Home-page: https://github.com/uuk0/PyBytecodeManipulator
+Author: uuk
+Author-email: uuk1301@gmail.com
+Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyBytecodeManipulator
 A high level cross-version python bytecode manipulation library build ontop 
 of 'dis' and 'inspect' 
 
 Supports code inlining, branch removing and arbitrary code injection into 
 existing functions.
 
@@ -64,30 +82,42 @@
 # Examples
 
 TODO
 
 
 # Applied Optimisations
 
-- Constant Expression inlining
+- Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
 - With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
 - During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
 - Method inlining is not working properly and needs a lot more testing
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
 
 
 ## Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/Emulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,31 +5,38 @@
 from inspect import CO_GENERATOR
 
 from bytecodemanipulation.MutableFunction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.Opcodes import Opcodes
 
 
-class UnknownOpcodeError(Exception): pass
-class FinalReturn(Exception): pass
-class YieldValue(Exception): pass
+class UnknownOpcodeError(Exception):
+    pass
+
+
+class FinalReturn(Exception):
+    pass
+
+
+class YieldValue(Exception):
+    pass
 
 
 class EmulatorGeneratorContainer:
     def __init__(self, mutable: MutableFunction, args: typing.Sized = tuple()):
         self.mutable = mutable
         self.instruction = mutable.instructions[0]
         self.args = args
 
         if len(self.args) != self.mutable.argument_count:
             raise ValueError()
 
         self.stack = []
         self.local_variables = [None] * len(self.mutable.shared_variable_names)
-        self.local_variables[:len(self.args)] = self.args
+        self.local_variables[: len(self.args)] = self.args
         self.free_vars = [None] * len(mutable.free_variables)
         self.exception_handle_stack = []
 
         self.instruction = self.mutable.instructions[0]
         self.continue_stack = []
 
         if not isinstance(self.mutable, MutableFunction):
@@ -44,15 +51,23 @@
             # print(self.local_variables)
             target = OPCODE_FUNCS[self.instruction.opcode]
 
             if target is None:
                 raise UnknownOpcodeError(self.instruction)
 
             try:
-                self.instruction, self.mutable = target(self.mutable, self.instruction, self.stack, self.local_variables, self.free_vars, self.continue_stack, self.exception_handle_stack)
+                self.instruction, self.mutable = target(
+                    self.mutable,
+                    self.instruction,
+                    self.stack,
+                    self.local_variables,
+                    self.free_vars,
+                    self.continue_stack,
+                    self.exception_handle_stack,
+                )
             except FinalReturn as e:
                 raise StopIteration
             except YieldValue as e:
                 if len(e.args) > 1:
                     self.instruction, self.mutable = e.args[1:]
 
                 return e.args[0]
@@ -71,139 +86,256 @@
         mutable = MutableFunction(mutable)
 
     if len(args) != mutable.argument_count:
         raise ValueError()
 
     stack = []
     local_variables = [None] * len(mutable.shared_variable_names)
-    local_variables[:len(args)] = args
+    local_variables[: len(args)] = args
     free_vars = [None] * len(mutable.free_variables)
     exception_handle_stack = []
 
     instruction = mutable.instructions[0]
     continue_stack = []
 
     while True:
         # print(instruction)
         target = OPCODE_FUNCS[instruction.opcode]
 
         if target is None:
             raise UnknownOpcodeError(instruction)
 
         try:
-            instruction, mutable = target(mutable, instruction, stack, local_variables, free_vars, continue_stack, exception_handle_stack)
+            instruction, mutable = target(
+                mutable,
+                instruction,
+                stack,
+                local_variables,
+                free_vars,
+                continue_stack,
+                exception_handle_stack,
+            )
         except FinalReturn as e:
             if len(e.args) > 1:
                 instruction, mutable = e.args[1:]
 
             return e.args[0]
         except YieldValue:
             raise RuntimeError("YIELD outside GENERATOR")
 
 
 OPCODE_FUNCS: typing.List[typing.Callable | None] = [None] * 256
 
 
 def execution(opcode: int):
-    def target(func: typing.Callable[[MutableFunction, Instruction, list, list, list, list, list], typing.Tuple[Instruction, MutableFunction]]):
+    def target(
+        func: typing.Callable[
+            [MutableFunction, Instruction, list, list, list, list, list],
+            typing.Tuple[Instruction, MutableFunction],
+        ]
+    ):
         OPCODE_FUNCS[opcode] = func
         return func
 
     return target
 
 
 @execution(Opcodes.NOP)
 @execution(Opcodes.GEN_START)
-def nop(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def nop(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     return instr.next_instruction, func
 
 
 @execution(Opcodes.POP_TOP)
-def pop_top(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def pop_top(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.JUMP_ABSOLUTE)
 @execution(Opcodes.JUMP_FORWARD)
-def jump_unconditional(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def jump_unconditional(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     return instr.arg_value, func
 
 
 @execution(Opcodes.LOAD_GLOBAL)
-def load_global(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_global(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     try:
         stack.append(func.target.__globals__[instr.arg_value])
     except KeyError:
         stack.append(getattr(builtins, instr.arg_value))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.STORE_GLOBAL)
-def store_global(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def store_global(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     func.target.__globals__[instr.arg_value] = stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.LOAD_METHOD)
 @execution(Opcodes.LOAD_ATTR)
-def load_attr(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_attr(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     obj = stack.pop(-1)
     try:
         stack.append(getattr(obj, instr.arg_value))
     except AttributeError:
         print(obj, instr)
         raise
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.STORE_ATTR)
-def load_attr(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_attr(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     setattr(stack.pop(-1), instr.arg_value, stack.pop(-1))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.LOAD_FAST)
-def load_fast(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_fast(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(local[instr.arg])
     return instr.next_instruction, func
 
 
 @execution(Opcodes.STORE_FAST)
-def store_fast(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def store_fast(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     local[instr.arg] = stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.LOAD_CONST)
-def load_const(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_const(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(instr.arg_value)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.LOAD_DEREF)
 @execution(Opcodes.LOAD_CLOSURE)
-def load_deref(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def load_deref(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(free_vars[instr.arg])
     return instr.next_instruction, func
 
 
 @execution(Opcodes.STORE_DEREF)
-def store_deref(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def store_deref(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     free_vars += [None] * (instr.arg + 1 - len(free_vars))
     free_vars[instr.arg] = stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.CALL_METHOD)
 @execution(Opcodes.CALL_FUNCTION)
-def call_method(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def call_method(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     args = list(reversed([stack.pop(-1) for _ in range(instr.arg)]))
     target = stack.pop(-1)
 
     if hasattr(target, "__self__") and hasattr(target, "__code__"):
         args.insert(0, target.__self__)
 
     try:
@@ -212,58 +344,98 @@
         stack.append(target(*args))
         return instr.next_instruction, func
 
     if mutable.code_flags & CO_GENERATOR:
         stack.append(EmulatorGeneratorContainer(mutable, args))
         return instr.next_instruction, func
 
-    call_stack.append((func, stack[:], local[:], instr.next_instruction, exception_handle_stack[:], free_vars[:]))
+    call_stack.append(
+        (
+            func,
+            stack[:],
+            local[:],
+            instr.next_instruction,
+            exception_handle_stack[:],
+            free_vars[:],
+        )
+    )
 
     free_vars.clear()
 
     free_vars[:] = [None] * len(mutable.free_variables)
 
     if hasattr(target, "_CELL_SPACE"):
-        free_vars[:len(target._CELL_SPACE)] = target._CELL_SPACE
+        free_vars[: len(target._CELL_SPACE)] = target._CELL_SPACE
 
     stack.clear()
     local[:] = [None] * len(mutable.shared_variable_names)
-    local[:len(args)] = args
+    local[: len(args)] = args
 
     print("calling", mutable)
 
     return mutable.instructions[0], mutable
 
 
 @execution(Opcodes.RETURN_VALUE)
-def return_value(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def return_value(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     return_obj = stack.pop(-1)
 
     print("returning", func)
     print(return_obj)
 
     if len(call_stack) == 0:
         raise FinalReturn(return_obj)
 
-    func, stack[:], local[:], next_instr, exception_handle_stack[:], free_vars[:] = call_stack.pop(-1)
+    (
+        func,
+        stack[:],
+        local[:],
+        next_instr,
+        exception_handle_stack[:],
+        free_vars[:],
+    ) = call_stack.pop(-1)
 
     stack.append(return_obj)
 
     return next_instr, func
 
 
 @execution(Opcodes.YIELD_VALUE)
-def yield_value(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list):
+def yield_value(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+):
     value = stack.pop(-1)
     stack.append(None)
     raise YieldValue(value, instr.next_instruction, func)
 
 
 @execution(Opcodes.YIELD_FROM)
-def yield_from(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def yield_from(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     null = stack.pop(-1)
 
     if null is not None:
         raise RuntimeError("expected None, got " + repr(null))
 
     tos = stack[-1]
 
@@ -272,210 +444,410 @@
     except StopIteration:
         stack.pop(-1)
         stack.append(None)
         return instr.next_instruction, func
 
 
 @execution(Opcodes.POP_JUMP_IF_TRUE)
-def pop_jump_if_true(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def pop_jump_if_true(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     case = stack.pop(-1)
 
     if case:
         return instr.arg_value, func
     return instr.next_instruction, func
 
 
 @execution(Opcodes.JUMP_IF_TRUE_OR_POP)
-def jump_if_true_or_pop(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def jump_if_true_or_pop(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     case = stack[-1]
 
     if case:
         return instr.arg_value, func
 
     stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.POP_JUMP_IF_FALSE)
-def pop_jump_if_false(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def pop_jump_if_false(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     case = stack.pop(-1)
 
     if not case:
         return instr.arg_value, func
     return instr.next_instruction, func
 
 
 @execution(Opcodes.CONTAINS_OP)
-def contains_op(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def contains_op(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     state = stack.pop(-2) in stack.pop(-1)
 
     if instr.arg:
         state = not state
 
     stack.append(state)
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.IS_OP)
-def is_op(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def is_op(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     state = stack.pop(-2) is stack.pop(-1)
 
     if instr.arg:
         state = not state
 
     stack.append(state)
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.COMPARE_OP)
-def compare_op(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
-    op = ('<', '<=', '==', '!=', '>', '>=')[instr.arg]
+def compare_op(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    op = ("<", "<=", "==", "!=", ">", ">=")[instr.arg]
     a, b = stack.pop(-2), stack.pop(-1)
 
     stack.append(eval(f"a {op} b", {"a": a, "b": b}))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BINARY_SUBSCR)
-def binary_subscr(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subscr(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(stack.pop(-2)[stack.pop(-1)])
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BINARY_ADD)
-def binary_add(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_add(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(stack.pop(-2) + stack.pop(-1))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.INPLACE_ADD)
-def binary_subtract(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     a, b = stack.pop(-2), stack.pop(-1)
     a += b
     stack.append(a)
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BINARY_SUBTRACT)
-def binary_subtract(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(stack.pop(-2) - stack.pop(-1))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.INPLACE_SUBTRACT)
-def binary_subtract(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     a, b = stack.pop(-2), stack.pop(-1)
     a -= b
     stack.append(a)
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BINARY_MULTIPLY)
-def binary_subtract(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(stack.pop(-2) * stack.pop(-1))
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.INPLACE_MULTIPLY)
-def binary_subtract(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     a, b = stack.pop(-2), stack.pop(-1)
     a *= b
     stack.append(a)
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.SETUP_FINALLY)
-def setup_finally(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def setup_finally(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     exception_handle_stack.append(instr.arg_value)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.POP_BLOCK)
-def pop_block(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def pop_block(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     exception_handle_stack.pop(-1)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.IMPORT_NAME)
-def import_name(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def import_name(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(importlib.import_module(instr.arg_value))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.IMPORT_FROM)
-def import_name(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def import_name(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(getattr(stack.pop(-1), instr.arg_value))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.GET_ITER)
 @execution(Opcodes.GET_YIELD_FROM_ITER)
-def get_iter(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def get_iter(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(iter(stack.pop(-1)))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.FOR_ITER)
-def for_iter(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def for_iter(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
 
     iterator = stack[-1]
 
     try:
         stack.append(next(iterator))
     except StopIteration:
         stack.pop(-1)
         return instr.arg_value, func
 
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BUILD_TUPLE)
-def build_tuple(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def build_tuple(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(tuple(reversed([stack.pop(-1) for _ in range(instr.arg)])))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BUILD_LIST)
-def build_tuple(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def build_tuple(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(list(reversed([stack.pop(-1) for _ in range(instr.arg)])))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BUILD_SET)
-def build_set(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def build_set(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack.append(set([stack.pop(-1) for _ in range(instr.arg)]))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.UNPACK_SEQUENCE)
-def unpack_sequence(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def unpack_sequence(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     stack += reversed(stack.pop(-1))
     return instr.next_instruction, func
 
 
 @execution(Opcodes.LIST_EXTEND)
-def list_extend(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
-    l = stack[-instr.arg-1]
+def list_extend(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    l = stack[-instr.arg - 1]
     obj = stack.pop(-1)
     l.extend(obj)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.MAKE_FUNCTION)
-def make_function(func: MutableFunction, instr: Instruction, stack: list, local: list, free_vars: list, call_stack: list, exception_handle_stack: list) -> typing.Tuple[Instruction, MutableFunction]:
+def make_function(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
     flags = instr.arg
 
     add_args = []
     add_kwargs = {}
     parameter_annotations = []
     cells = []
 
@@ -490,15 +862,15 @@
 
     if flags & 0x02:  # keyword-args
         add_kwargs.update(stack.pop(-1))
 
     if flags & 0x01:  # default arg tuple
         add_args += stack.pop(-1)
 
-    cell_names = string.ascii_lowercase[:len(cells)]
+    cell_names = string.ascii_lowercase[: len(cells)]
 
     if cell_names:
         create = f"""
 
 def init():
     {', '.join(cell_names)} = {", ".join(["None"] * len(cell_names))}
     
@@ -508,18 +880,21 @@
     return target
 """
 
         space = {}
         exec(create, space)
         target = space["init"]()
     else:
+
         def target():
             pass
 
     target._CELL_SPACE = cells[:]
 
     target.__code__ = code_obj
     target.__name__ = qualified_name
 
-    stack.append(lambda *args, **kwargs: target(*add_args, *args, **add_kwargs, **kwargs))
+    stack.append(
+        lambda *args, **kwargs: target(*add_args, *args, **add_kwargs, **kwargs)
+    )
 
     return instr.next_instruction, func
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/Mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,25 @@
 
             try:
                 state = os.environ["DEBUG_MIXINS"]
             except KeyError:
                 state = False
 
             if state:
+                print("DEBUGGING MIXINS!")
+
+            if state:
                 target = MutableFunction(self.target)
                 override_target = MutableFunction(_invoke_emulator)
-                override_target.constants[override_target.constants.index(100)] = mutable
+                override_target.constants[
+                    override_target.constants.index(100)
+                ] = mutable
                 target.copy_from(override_target)
                 target.reassign_to_function()
+                target.target._debug_wrapper = mutable
             else:
                 mutable.reassign_to_function()
 
         def reset(self):
             pass
 
         def run_optimiser(self):
@@ -367,17 +373,15 @@
 
     def annotation(target):
         return target
 
     return annotation
 
 
-_PREPARED_ANNOTATIONS: typing.Dict[
-    str, typing.List["Mixin._MixinHandle"]
-] = {}
+_PREPARED_ANNOTATIONS: typing.Dict[str, typing.List["Mixin._MixinHandle"]] = {}
 
 
 class Mixin:
     """
     Mixin class providing an abstract interface for bytecode manipulation
 
     Example use:
@@ -410,27 +414,31 @@
         @Mixin-annotated classes MUST implement this so the neat helper functions can be used
         """
 
         MIXIN_CONTAINER: _MixinContainer = None
 
         @classmethod
         def resolve_local(cls, name: str) -> object:
-            raise MixinInjectionNotSupportedException("Not implemented, should not happen!")
+            raise MixinInjectionNotSupportedException(
+                "Not implemented, should not happen!"
+            )
 
         @classmethod
         def resolve_exception_instance(cls) -> Exception:
             raise MixinInjectionNotSupportedException("Not implemented!")
 
         @classmethod
         def resolve_prepared_parameter(cls, index: int) -> object:
             raise MixinInjectionNotSupportedException("Not implemented!")
 
         @classmethod
         def resolve_cell_variable(cls, name: str) -> object:
-            raise MixinInjectionNotSupportedException("Not implemented, should not happen!")
+            raise MixinInjectionNotSupportedException(
+                "Not implemented, should not happen!"
+            )
 
         @classmethod
         def return_outer(cls, value=None):
             raise MixinInjectionNotSupportedException("Not implemented!")
 
         @classmethod
         def jump_to(cls, position: InjectionPosition.AbstractInjectionPosition):
@@ -457,15 +465,19 @@
 
         def apply_on(self, mutable: MutableFunction):
             resolve_accesses(mutable, self.override_with)
 
             mutable.copy_from(self.override_with)
 
     class _InjectAtHandle(_MixinHandle):
-        def __init__(self, at: InjectionPosition.AbstractInjectionPosition, inject: MutableFunction):
+        def __init__(
+            self,
+            at: InjectionPosition.AbstractInjectionPosition,
+            inject: MutableFunction,
+        ):
             self.at = at
             self.inject = inject
 
         def apply_on(self, mutable: MutableFunction):
             protected_locals = resolve_accesses(mutable, self.inject)
 
             if self.inject.shared_variable_names[0] in ("cls", "self"):
@@ -473,15 +485,20 @@
 
             tree = MutableFunctionWithTree(mutable)
 
             for position_instr in self.at.get_positions(mutable.instructions[0])[:]:
                 if position_instr not in mutable.instructions:
                     continue
 
-                insert_method_into(tree, position_instr.offset, self.inject, protected_locals=protected_locals)
+                insert_method_into(
+                    tree,
+                    position_instr.offset - 1,
+                    self.inject,
+                    protected_locals=protected_locals,
+                )
 
                 mutable.assemble_instructions_from_tree(tree.root)
 
     def __init__(
         self,
         target_class: str | typing.Type | typing.Callable[[], typing.Type],
         priority=0,
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/MutableFunction.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import copy
 import dis
+import sys
 import types
 import typing
 import simplejson
 
+import bytecodemanipulation.assembler.util.tokenizer
 from bytecodemanipulation.Opcodes import HAS_CELL_VARIABLE
 from bytecodemanipulation.Opcodes import HAS_JUMP_BACKWARDS
 from bytecodemanipulation.Opcodes import (
     Opcodes,
     END_CONTROL_FLOW,
     OPCODE2NAME,
     OPNAME2CODE,
@@ -39,42 +41,60 @@
         "offset",
         "opcode",
         "opname",
         "arg_value",
         "arg",
         "_next_instruction",
         "previous_instructions",
+        "source_location",
     )
 
     @classmethod
     def create(cls, *args, **kwargs):
         return cls(None, -1, *args, **kwargs)
 
+    @classmethod
+    def create_with_token(
+        cls,
+        token: bytecodemanipulation.assembler.util.tokenizer.AbstractToken,
+        function: typing.Optional["MutableFunction"],
+        offset: int | None,
+        opcode_or_name: int | str,
+        arg_value: object = None,
+        arg: int = None,
+        _decode_next=True,
+    ) -> "Instruction":
+        raise NotImplementedError("not bound!")
+
     def __init__(
         self,
         function: typing.Optional["MutableFunction"],
         offset: int | None,
         opcode_or_name: int | str,
         arg_value: object = None,
         arg: int = None,
         _decode_next=True,
+        pos_info=None,
     ):
         self.function = function
         self.offset = offset
         self.opcode, self.opname = self._pair_instruction(opcode_or_name)
         self.arg_value = arg_value
         self.arg = arg
+        self.source_location = pos_info
 
         if (
             self.arg is not None
             and self.arg_value is None
             and (_decode_next or not self.has_jump())
         ):
             self.change_arg(self.arg)
-        elif self.arg_value is not None and self.arg is None:
+        elif (
+            self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST
+        ) and self.arg is None:
             self.change_arg_value(self.arg_value)
 
         # Reference to the next instruction
         # Will raise an exception if changed and not using assemble_instructions_from_tree()
         self._next_instruction: typing.Optional[Instruction] = (
             None
             if function is None
@@ -82,32 +102,83 @@
             or self.opcode in END_CONTROL_FLOW
             or not _decode_next
             else function.instructions[offset + 1]
         )
 
         self.previous_instructions: typing.List["Instruction"] | None = None
 
+    def copy(self, owner: "MutableFunction" = None) -> "Instruction":
+        instance = type(self)(
+            self.function,
+            self.offset,
+            self.opcode,
+            self.arg_value if self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST else self.arg,
+        )
+
+        if owner:
+            instance.update_owner(owner, -1, force_change_arg_index=True)
+
+        return instance
+
     def apply_visitor(
         self,
         visitor: AbstractInstructionWalker,
         visited: typing.Set["Instruction"] = None,
     ):
         if visited is None:
             visited = set()
 
+        if self in visited:
+            return
+
+        visited.add(self)
+
         visitor.visit(self)
 
         if self.has_stop_flow():
             return
 
-        self.next_instruction.apply_visitor(visitor, visited)
+        if self.next_instruction is not None and self.next_instruction != self:
+            self.next_instruction.apply_visitor(visitor, visited)
 
-        if self.has_jump():
+        if self.has_jump() and isinstance(self.arg_value, Instruction):
             typing.cast(Instruction, self.arg_value).apply_visitor(visitor, visited)
 
+    def apply_value_visitor(
+        self,
+        callback: typing.Callable[
+            ["Instruction", typing.Any | None, typing.Any | None], typing.Any
+        ],
+        visited: typing.Dict["Instruction", typing.Any] = None,
+    ) -> typing.Any:
+        if visited is None:
+            visited = {}
+
+        elif self in visited:
+            return visited[self]
+
+        visited[self] = None
+
+        if self.has_stop_flow():
+            return callback(self, None, None)
+
+        if self.has_jump() and isinstance(self.arg_value, Instruction):
+            return callback(
+                self,
+                self.next_instruction.apply_value_visitor(callback, visited),
+                self.arg_value.apply_value_visitor(callback, visited),
+            )
+
+        if self.next_instruction is not None:
+            return callback(
+                self, self.next_instruction.apply_value_visitor(callback, visited), None
+            )
+
+        return callback(self, None, None)
+
     def add_previous_instruction(self, instruction: "Instruction"):
         if self.previous_instructions is None:
             self.previous_instructions = [instruction]
         elif instruction not in self.previous_instructions:
             self.previous_instructions.append(instruction)
 
     def remove_previous_instruction(self, instruction: "Instruction"):
@@ -165,42 +236,50 @@
 
     def __eq__(self, other):
         if not isinstance(other, Instruction):
             return False
 
         return (
             self.opcode == other.opcode
-            and (self.offset == other.offset or self.offset is None or other.offset is None)
             and (
-                (self.arg_value == other.arg_value) if not isinstance(self.arg_value, Instruction) else (id(self.arg_value) == id(other.arg_value))
+                self.offset == other.offset
+                or self.offset is None
+                or other.offset is None
+            )
+            and (
+                (self.arg_value == other.arg_value)
+                if not isinstance(self.arg_value, Instruction)
+                else (id(self.arg_value) == id(other.arg_value))
                 if self.arg_value is not None and other.arg_value is not None
                 else True
             )
         )
 
-    def lossy_eq(self, other):
+    def lossy_eq(self, other: "Instruction") -> bool:
         if not isinstance(other, Instruction):
             return False
 
-        return (
-            self.opcode == other.opcode
-            and (
-                (self.arg_value == other.arg_value) if not isinstance(self.arg_value, Instruction) else self.arg_value.lossy_eq(other.arg_value)
-                if self.arg_value is not None and other.arg_value is not None
-                else True
+        return self.opcode == other.opcode and (
+            (
+                (self.arg_value == other.arg_value)
+                if not isinstance(self.arg_value, Instruction)
+                else self.arg_value.lossy_eq(other.arg_value)
             )
+            if (self.arg_value is not None and other.arg_value is not None)
+            or self.opcode == Opcodes.LOAD_CONST
+            else True
         )
 
     def __hash__(self):
         return id(self)
 
     def get_arg(self):
         return 0 if self.arg is None else self.arg
 
-    def change_opcode(self, opcode: int | str):
+    def change_opcode(self, opcode: int | str, arg_value=None):
         self.opcode, self.opname = self._pair_instruction(opcode)
         # todo: what happens with the arg?
 
         self.next_instruction = (
             None
             if self.function is None
             or self.offset is None
@@ -209,57 +288,81 @@
             else self.function.instructions[self.offset + 1]
         )
 
         if self.opcode < dis.HAVE_ARGUMENT:
             self.arg = 0
             self.arg_value = None
 
+        if arg_value:
+            self.change_arg_value(arg_value)
+
+        return self
+
     def change_arg_value(self, value: object):
         self.arg_value = value
 
         if self.function is not None:
             if self.opcode in HAS_NAME:
                 assert isinstance(value, str)
                 self.arg = self.function.allocate_shared_name(value)
+            elif self.opcode in HAS_CELL_VARIABLE:
+                assert isinstance(value, str)
+                self.arg = self.function.allocate_shared_cell(value)
             elif self.opcode in HAS_CONST:
                 self.arg = self.function.allocate_shared_constant(value)
             elif self.opcode in HAS_LOCAL:
                 assert isinstance(value, str), (value, self.opname)
                 self.arg = self.function.allocate_shared_variable_name(value)
             elif self.opcode in HAS_JUMP_ABSOLUTE:
-                assert isinstance(value, Instruction), value
-                self.arg = value.offset
+                if isinstance(value, Instruction):
+                    self.arg = value.offset
             elif self.opcode == Opcodes.FOR_ITER:
                 assert isinstance(value, Instruction), value
                 self.arg = value.offset - self.offset
             elif self.opcode in HAS_JUMP_FORWARD:
                 assert isinstance(value, Instruction), value
                 self.arg = value.offset - self.offset
         else:
             self.arg = None
 
     def change_arg(self, arg: int):
         self.arg = arg
 
         if self.function is not None:
             try:
-                if self.opcode in HAS_NAME:
+                flag = False
+                if sys.version_info.minor >= 11:
+                    if self.opcode == Opcodes.LOAD_GLOBAL:
+                        self.arg_value = self.function.shared_names[arg >> 1]
+                        flag = True
+
+                if flag:
+                    pass
+                elif self.opcode in HAS_NAME:
                     self.arg_value = self.function.shared_names[arg]
+                elif self.opcode in HAS_CELL_VARIABLE:
+                    self.arg_value = self.function.cell_variables[arg]
                 elif self.opcode in HAS_CONST:
                     self.arg_value = self.function.constants[arg]
                 elif self.opcode in HAS_LOCAL:
                     self.arg_value = self.function.shared_variable_names[arg]
                 elif self.opcode in HAS_JUMP_ABSOLUTE:
                     self.arg_value = self.function.instructions[arg]
                 elif self.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
                     self.arg_value = self.function.instructions[arg + self.offset]
                 elif self.opcode in HAS_JUMP_FORWARD and self.offset is not None:
                     self.arg_value = self.function.instructions[arg + self.offset]
             except:
-                print(self.opname, arg, self.function.shared_names, self.function.constants, self.function.shared_variable_names)
+                print(
+                    self.opname,
+                    arg,
+                    self.function.shared_names,
+                    self.function.constants,
+                    self.function.shared_variable_names,
+                )
                 raise
         else:
             self.arg_value = None
 
     def has_name(self):
         return self.opcode in HAS_NAME
 
@@ -291,27 +394,37 @@
     def has_unconditional_jump(self):
         return self.opcode in UNCONDITIONAL_JUMPS
 
     def has_stop_flow(self):
         return self.opcode in END_CONTROL_FLOW
 
     def update_owner(
-        self, function: "MutableFunction", offset: int, update_following=True
+        self,
+        function: "MutableFunction",
+        offset: int,
+        update_following=True,
+        force_change_arg_index=False,
     ):
         previous_function = self.function
 
         self.function = function
         self.offset = offset
 
         # If previously the ownership was unset, and we have not fully referenced args, do it now!
         # todo: when previous owner was set, and arg is not None, we might need to de-ref the value
         #    and re-ref afterwards, so the value lives in the new owner
-        if self.arg is not None and self.arg_value is None:
+        if (
+            self.arg is not None
+            and self.arg_value is None
+            and (not force_change_arg_index or self.opcode != Opcodes.LOAD_CONST)
+        ):
             self.change_arg(self.arg)
-        elif self.arg_value is not None and self.arg is None:
+        elif (self.arg_value is not None or self.opcode == Opcodes.LOAD_CONST) and (
+            self.arg is None or force_change_arg_index
+        ):
             self.change_arg_value(self.arg_value)
 
         if update_following:
             self.next_instruction = (
                 (None if previous_function != function else self.next_instruction)
                 if function is None
                 or offset is None
@@ -334,35 +447,35 @@
 
         if self.has_unconditional_jump():
             return self.arg_value.optimise_tree(visited)
 
         if visited is None:
             visited = set()
 
-        if self.opcode == Opcodes.NOP and self.next_instruction is not None:
-            return self.next_instruction.optimise_tree(visited)
-
         if self in visited:
             return self
 
+        visited.add(self)
+
+        if self.opcode == Opcodes.NOP and self.next_instruction is not None:
+            return self.next_instruction.optimise_tree(visited)
+
         while self.next_instruction is not None:
             assert isinstance(self.next_instruction, Instruction)
 
             if self.next_instruction.opname == "NOP":
                 self.next_instruction = self.next_instruction.next_instruction
                 continue
 
             if self.next_instruction.opname in ("JUMP_ABSOLUTE", "JUMP_FORWARD"):
                 self.next_instruction = self.next_instruction.arg_value
                 continue
 
             break
 
-        visited.add(self)
-
         if (
             self.next_instruction is not None
             and not self.has_stop_flow()
             and not self.has_unconditional_jump()
         ):
             self.next_instruction = self.next_instruction.optimise_tree(visited)
 
@@ -372,15 +485,17 @@
             or self.has_jump_backward()
         ) and self.arg_value is not None:
             assert isinstance(self.arg_value, Instruction)
             self.change_arg_value(self.arg_value.optimise_tree(visited))
 
         return self
 
-    def trace_variable_set(self, name: str, visited: typing.Set[str] = None) -> typing.Iterator["Instruction"]:
+    def trace_variable_set(
+        self, name: str, visited: typing.Set[str] = None
+    ) -> typing.Iterator["Instruction"]:
         if visited and self in visited:
             return
 
         if self.opcode == Opcodes.STORE_FAST and self.arg_value == name:
             yield self
             return
 
@@ -399,47 +514,63 @@
     def trace_stack_position(
         self, stack_position: int
     ) -> typing.Iterator["Instruction"]:
         for instr in self.get_priorities_previous():
             yield from instr._trace_stack_position(stack_position, set(), self)
 
     def get_priorities_previous(self) -> typing.List["Instruction"]:
-        if not self.previous_instructions: return []
+        if not self.previous_instructions:
+            return []
 
-        real_previous = [instr for instr in self.previous_instructions if instr.next_instruction == self]
-        unreal_previous = [instr for instr in self.previous_instructions if instr.next_instruction != self]
+        real_previous = [
+            instr
+            for instr in self.previous_instructions
+            if instr.next_instruction == self
+        ]
+        unreal_previous = [
+            instr
+            for instr in self.previous_instructions
+            if instr.next_instruction != self
+        ]
         highest = None
 
         for e in real_previous:
             if e.offset == self.offset - 1 or e.opcode == Opcodes.SETUP_FINALLY:
                 highest = e
 
         if not highest:
             return real_previous + unreal_previous
 
         return [highest] + [e for e in real_previous if e != highest] + unreal_previous
 
-    def trace_normalized_stack_position(self, stack_position: int) -> typing.Optional["Instruction"]:
+    def trace_normalized_stack_position(
+        self, stack_position: int
+    ) -> typing.Optional["Instruction"]:
         target = next(self.trace_stack_position(stack_position))
 
         if target.opcode == Opcodes.DUP_TOP:
             return target.trace_normalized_stack_position(0)
 
         if target.opcode == Opcodes.LOAD_FAST:
             try:
-                variable_set = next(target.trace_variable_set(typing.cast(str, target.arg_value)))
+                variable_set = next(
+                    target.trace_variable_set(typing.cast(str, target.arg_value))
+                )
             except StopIteration:
                 return target
 
             return variable_set.trace_normalized_stack_position(0)
 
         return target
 
     def _trace_stack_position(
-        self, stack_position: int, yielded: typing.Set["Instruction"], previous_instr: "Instruction" = None
+        self,
+        stack_position: int,
+        yielded: typing.Set["Instruction"],
+        previous_instr: "Instruction" = None,
     ) -> typing.Iterator["Instruction"]:
         assert stack_position >= 0
 
         if self in yielded:
             return
 
         if self.has_unconditional_jump():
@@ -463,15 +594,17 @@
             yielded.add(self)
             # print("hit")
             yield self
             # print("cont")
 
             if additional_pos:
                 for instr in self.get_priorities_previous():
-                    yield from instr._trace_stack_position(additional_pos, yielded, self)
+                    yield from instr._trace_stack_position(
+                        additional_pos, yielded, self
+                    )
 
             return
 
         stack_position -= pushed
         stack_position += popped
 
         yielded.add(self)
@@ -486,21 +619,25 @@
         if additional_pos:
             for instr in self.get_priorities_previous():
                 yield from instr._trace_stack_position(additional_pos, yielded, self)
 
     def trace_stack_position_use(
         self, stack_position: int
     ) -> typing.Iterator["Instruction"]:
-        print(self, 0)
+        # print(self, 0)
 
         if not self.has_stop_flow():
-            yield from self.next_instruction._trace_stack_position_use(stack_position, set())
+            yield from self.next_instruction._trace_stack_position_use(
+                stack_position, set()
+            )
 
         if self.has_jump():
-            yield from typing.cast(Instruction, self.arg_value)._trace_stack_position_use(stack_position, set())
+            yield from typing.cast(
+                Instruction, self.arg_value
+            )._trace_stack_position_use(stack_position, set())
 
     def _trace_stack_position_use(
         self, stack_position: int, yielded: typing.Set["Instruction"]
     ) -> typing.Iterator["Instruction"]:
         assert stack_position >= 0
 
         if self in yielded:
@@ -511,79 +648,94 @@
         pushed, popped, additional_pos = self.get_stack_affect()
 
         if popped > stack_position:
             yielded.add(self)
             yield self
 
             if additional_pos:
-                yield from self.next_instruction._trace_stack_position_use(additional_pos, yielded)
+                yield from self.next_instruction._trace_stack_position_use(
+                    additional_pos, yielded
+                )
 
             return
 
         stack_position -= popped
         stack_position += pushed
 
         if not self.has_stop_flow():
-            yield from self.next_instruction._trace_stack_position_use(stack_position, yielded)
+            yield from self.next_instruction._trace_stack_position_use(
+                stack_position, yielded
+            )
 
         if self.has_jump():
-            yield from typing.cast(Instruction, self.arg_value)._trace_stack_position_use(stack_position, yielded)
+            yield from typing.cast(
+                Instruction, self.arg_value
+            )._trace_stack_position_use(stack_position, yielded)
 
         if additional_pos:
-            yield from self.next_instruction._trace_stack_position_use(additional_pos, yielded)
+            yield from self.next_instruction._trace_stack_position_use(
+                additional_pos, yielded
+            )
 
     def get_stack_affect(self) -> typing.Tuple[int, int, int | None]:
         # pushed, popped, additional
-        if self.opcode in (Opcodes.NOP, Opcodes.POP_BLOCK, Opcodes.POP_EXCEPT, Opcodes.SETUP_FINALLY, Opcodes.GEN_START, Opcodes.JUMP_ABSOLUTE):
+        if self.opcode in (
+            Opcodes.NOP,
+            Opcodes.POP_BLOCK,
+            Opcodes.POP_EXCEPT,
+            Opcodes.SETUP_FINALLY,
+            Opcodes.GEN_START,
+            Opcodes.JUMP_ABSOLUTE,
+            Opcodes.BYTECODE_LABEL,
+            Opcodes.CACHE,
+            Opcodes.PRECALL,
+            Opcodes.RESUME,
+        ):
             return 0, 0, None
 
         if self.opcode == Opcodes.DUP_TOP:
             return 2, 1, None
 
         if self.opcode in (Opcodes.GET_ITER, Opcodes.FOR_ITER):
             return 1, 0, None
 
         if self.opcode in (
             Opcodes.LOAD_CONST,
             Opcodes.LOAD_GLOBAL,
             Opcodes.LOAD_FAST,
             Opcodes.LOAD_DEREF,
             Opcodes.LOAD_CLOSURE,
+            Opcodes.LOAD_BUILD_CLASS,
         ):
             return 1, 0, None
 
         if self.opcode in (
             Opcodes.BUILD_TUPLE,
             Opcodes.BUILD_LIST,
             Opcodes.BUILD_SET,
             Opcodes.BUILD_SLICE,
             Opcodes.BUILD_STRING,
         ):
             return 1, self.arg, None
 
-        if self.opcode in (
-            Opcodes.ROT_TWO,
-        ):
+        if self.opcode in (Opcodes.ROT_TWO,):
             return 2, 2, None
 
-        if self.opcode in (
-            Opcodes.FORMAT_VALUE,
-        ):
+        if self.opcode in (Opcodes.FORMAT_VALUE,):
             return 1, (2 if (self.arg & 0x04) == 0x04 else 1), None
 
         if self.opcode in (
             Opcodes.CALL_FUNCTION,
             Opcodes.CALL_METHOD,
             Opcodes.CALL_FUNCTION_KW,
+            Opcodes.CALL,
         ):
             return 1, self.arg + 1, None
 
-        if self.opcode in (
-            Opcodes.CALL_FUNCTION_EX,
-        ):
+        if self.opcode in (Opcodes.CALL_FUNCTION_EX,):
             count = 2
 
             if self.arg & 0x01:
                 count += 1
 
             return 1, count, None
 
@@ -610,64 +762,80 @@
             Opcodes.BINARY_MODULO,
             Opcodes.BINARY_XOR,
             Opcodes.BINARY_AND,
             Opcodes.BINARY_OR,
             Opcodes.BINARY_POWER,
             Opcodes.INPLACE_SUBTRACT,
             Opcodes.IMPORT_NAME,
+            Opcodes.YIELD_FROM,
         ):
             return 1, 2, None
 
         if self.opcode in (
             Opcodes.LOAD_ATTR,
             Opcodes.LOAD_METHOD,
             Opcodes.GET_AWAITABLE,
             Opcodes.LIST_TO_TUPLE,
             Opcodes.IMPORT_FROM,
             Opcodes.UNARY_NEGATIVE,
+            Opcodes.YIELD_VALUE,
+            Opcodes.GET_YIELD_FROM_ITER,
+            Opcodes.UNARY_NOT,
+            Opcodes.UNARY_NEGATIVE,
+            Opcodes.UNARY_INVERT,
+            Opcodes.UNARY_POSITIVE,
+            Opcodes.STATIC_ATTRIBUTE_ACCESS,
         ):
             return 1, 1, None
 
-        if self.opcode in (
-            Opcodes.STORE_ATTR,
-        ):
+        if self.opcode in (Opcodes.STORE_ATTR,):
             return 2, 0, None
 
         if self.opcode in (
             Opcodes.POP_TOP,
             Opcodes.POP_JUMP_IF_TRUE,
             Opcodes.POP_JUMP_IF_FALSE,
             Opcodes.STORE_FAST,
+            Opcodes.STORE_NAME,
             Opcodes.STORE_DEREF,
-            Opcodes.YIELD_VALUE,
-            Opcodes.YIELD_FROM,
+            Opcodes.STORE_GLOBAL,
             Opcodes.RETURN_VALUE,
         ):
             return 0, 1, None
 
         if self.opcode == Opcodes.UNPACK_SEQUENCE:
             return self.arg, 1, None
 
         if self.opcode == Opcodes.JUMP_IF_NOT_EXC_MATCH:
             return 0, 2, None
 
         if self.opcode == Opcodes.MAKE_FUNCTION:
             return 1, 2 + self.arg.bit_count(), None
 
+        if self.opcode == Opcodes.RAISE_VARARGS:
+            return 0, self.arg, None
+
+        if self.opcode == Opcodes.DUP_TOP_TWO:
+            return 2, 4, None
+
         raise RuntimeError(self)
 
     def insert_after(self, *instructions: "Instruction" | typing.List["Instruction"]):
-        if not instructions: return self
+        if not instructions:
+            return self
 
         if isinstance(instructions[0], (list, tuple)):
             if len(instructions) > 1:
                 raise ValueError
 
             instructions = instructions[0]
 
+        if len(instructions) == 0:
+            return self
+
         instructions[0].next_instruction = self.next_instruction
         self.next_instruction = instructions[0]
 
         if len(instructions) > 1:
             instructions[0].insert_after(instructions[1:])
 
         return self
@@ -683,33 +851,68 @@
         return cls(target)
 
     def __init__(self, target: types.FunctionType | types.MethodType):
         self.target = target
 
         self.code_object: types.CodeType = target.__code__
 
-        self.argument_count = self.code_object.co_argcount
-        self.cell_variables = list(self.code_object.co_cellvars)
-        self.__raw_code = bytearray(self.code_object.co_code)
-        self.constants = list(self.code_object.co_consts)
-        self.filename = self.code_object.co_filename
-        self.first_line_number = self.code_object.co_firstlineno
-        self.code_flags = self.code_object.co_flags
-        self.free_variables = list(self.code_object.co_freevars)
-        self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
-        self.line_table = self.code_object.co_linetable
-        self.lnotab = bytearray(self.code_object.co_lnotab)
-        self.function_name = self.code_object.co_name
-        self.shared_names = list(self.code_object.co_names)
-        # Local variable count is implied by co_varnames
-        self.positional_only_argument_count = self.code_object.co_posonlyargcount
-        self.stack_size = self.code_object.co_stacksize
-        self.shared_variable_names = list(self.code_object.co_varnames)
+        self._load_from_code_object(self.code_object)
+
+    if sys.version_info.major == 3 and sys.version_info.minor == 10:
+
+        def _load_from_code_object(self, obj: types.CodeType):
+            self.argument_count = self.code_object.co_argcount
+            self.cell_variables = list(self.code_object.co_cellvars)
+            self.__raw_code = bytearray(self.code_object.co_code)
+            self.constants = list(self.code_object.co_consts)
+            self.filename = self.code_object.co_filename
+            self.first_line_number = self.code_object.co_firstlineno
+            self.code_flags = self.code_object.co_flags
+            self.free_variables = list(self.code_object.co_freevars)
+            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
+            self.line_table = self.code_object.co_linetable
+            self.lnotab = bytearray(self.code_object.co_lnotab)
+
+            self.function_name = self.code_object.co_name
+            self.shared_names = list(self.code_object.co_names)
+            # Local variable count is implied by co_varnames
+            self.positional_only_argument_count = self.code_object.co_posonlyargcount
+            self.stack_size = self.code_object.co_stacksize
+            self.shared_variable_names = list(self.code_object.co_varnames)
+
+            self.__instructions: typing.Optional[typing.List[Instruction]] = None
+
+    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
+
+        def _load_from_code_object(self, obj: types.CodeType):
+            self.argument_count = self.code_object.co_argcount
+            self.cell_variables = list(self.code_object.co_cellvars)
+            self.__raw_code = bytearray(self.code_object.co_code)
+            self.constants = list(self.code_object.co_consts)
+            self.filename = self.code_object.co_filename
+            self.first_line_number = self.code_object.co_firstlineno
+            self.code_flags = self.code_object.co_flags
+            self.free_variables = list(self.code_object.co_freevars)
+            self.keyword_only_argument_count = self.code_object.co_kwonlyargcount
+            self.line_table = self.code_object.co_linetable
+            self.lnotab = bytearray(self.code_object.co_lnotab)
+
+            self.function_name = self.code_object.co_name
+            self.shared_names = list(self.code_object.co_names)
+            # Local variable count is implied by co_varnames
+            self.positional_only_argument_count = self.code_object.co_posonlyargcount
+            self.stack_size = self.code_object.co_stacksize
+            self.shared_variable_names = list(self.code_object.co_varnames)
 
-        self.__instructions: typing.Optional[typing.List[Instruction]] = None
+            self.exception_table = bytearray(self.code_object.co_exceptiontable)
+
+            self.__instructions: typing.Optional[typing.List[Instruction]] = None
+
+    else:
+        raise RuntimeError(sys.version_info)
 
     def __repr__(self):
         return f"MutableFunction({self.target})"
 
     def copy(self):
         def _():
             pass
@@ -738,68 +941,138 @@
         self.shared_names = mutable.shared_names.copy()
         self.positional_only_argument_count = mutable.positional_only_argument_count
         self.stack_size = mutable.stack_size
         self.shared_variable_names = mutable.shared_variable_names.copy()
 
         self.__instructions = None
 
-    def create_code_obj(self) -> types.CodeType:
-        if self.__instructions is None:
-            self.get_instructions()
+    if sys.version_info.major == 3 and sys.version_info.minor == 10:
 
-        self.assemble_fast(self.__instructions)
+        def create_code_obj(self) -> types.CodeType:
+            if self.__instructions is None:
+                self.get_instructions()
+
+            self.assemble_fast(self.__instructions)
+
+            return types.CodeType(
+                self.argument_count,
+                self.positional_only_argument_count,
+                self.keyword_only_argument_count,
+                len(self.shared_variable_names),
+                self.stack_size,
+                self.code_flags,
+                bytes(self.raw_code),
+                tuple(self.constants),
+                tuple(self.shared_names),
+                tuple(self.shared_variable_names),
+                self.filename,
+                self.function_name,
+                self.first_line_number,
+                self.get_lnotab(),
+                tuple(self.free_variables),
+                tuple(self.cell_variables),
+            )
 
-        return types.CodeType(
-            self.argument_count,
-            self.positional_only_argument_count,
-            self.keyword_only_argument_count,
-            len(self.shared_variable_names),
-            self.stack_size,
-            self.code_flags,
-            bytes(self.raw_code),
-            tuple(self.constants),
-            tuple(self.shared_names),
-            tuple(self.shared_variable_names),
-            self.filename,
-            self.function_name,
-            self.first_line_number,
-            bytes(self.lnotab),
-            tuple(self.free_variables),
-            tuple(self.cell_variables),
-        )
+    elif sys.version_info.major == 3 and sys.version_info.minor == 11:
+
+        def create_code_obj(self) -> types.CodeType:
+            if self.__instructions is None:
+                self.get_instructions()
+
+            self.assemble_fast(self.__instructions)
+
+            return types.CodeType(
+                self.argument_count,
+                self.positional_only_argument_count,
+                self.keyword_only_argument_count,
+                len(self.shared_variable_names),
+                self.stack_size,
+                self.code_flags,
+                bytes(self.raw_code),
+                tuple(self.constants),
+                tuple(self.shared_names),
+                tuple(self.shared_variable_names),
+                self.filename,
+                self.function_name,
+                self.function_name,
+                self.first_line_number,
+                self.get_lnotab(),
+                bytes(self.exception_table),
+                tuple(self.free_variables),
+                tuple(self.cell_variables),
+            )
+
+    def get_lnotab(self) -> bytes:
+        items = []
+
+        prev_line = self.first_line_number
+        count_since_previous = 0
+
+        for instr in self.__instructions:
+            count_since_previous += 1
+
+            if instr.source_location is None or instr.source_location[0] == prev_line:
+                continue
+
+            offset = instr.source_location[0] - prev_line
+
+            if offset > 127:
+                return bytes()
+
+            if offset < 0:
+                return bytes()
+
+            items.append(count_since_previous)
+            items.append(offset)
+            count_since_previous = 0
+
+        return bytes(items)
 
     def reassign_to_function(self):
         self.target.__code__ = self.create_code_obj()
 
     def decode_instructions(self):
         if self.__instructions is not None:
             self.__instructions.clear()
         else:
             self.__instructions = []
 
+        line = self.first_line_number
+        lnotab = list(self.lnotab)
+
         extra: int = 0
         for i in range(0, len(self.__raw_code), 2):
             opcode, arg = self.__raw_code[i : i + 2]
 
             if opcode == Opcodes.EXTENDED_ARG:
                 extra = extra * 256 + arg
-                self.__instructions.append(
-                    Instruction(self, i // 2, "NOP", _decode_next=False)
-                )
+                instr = Instruction(self, i // 2, "NOP", _decode_next=False)
 
             else:
                 arg += extra * 256
                 extra = 0
 
                 if opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
                     arg += 1
 
-                self.__instructions.append(
-                    Instruction(self, i // 2, opcode, arg=arg, _decode_next=False)
-                )
+                instr = Instruction(self, i // 2, opcode, arg=arg, _decode_next=False)
+
+            if lnotab:
+                lnotab[0] -= 1
+
+                if lnotab[0] == 0:
+                    line_incr = lnotab[1]
+                    del lnotab[:2]
+
+                    line += line_incr
+
+            instr.source_location = (line, None, None)
+
+            self.__instructions.append(instr)
+            # print(instr, instr.source_location)
 
         for i, instruction in enumerate(self.instructions):
             instruction.update_owner(self, i)
 
         self.prepare_previous_instructions()
 
     def prepare_previous_instructions(self):
@@ -861,14 +1134,15 @@
                     instruction.next_instruction = None
                 except:
                     print(instruction)
                     print(instruction.next_instruction)
                     raise
 
         self.assemble_fast(instructions)
+        self.update_instruction_offsets(self.instructions)
         # We do not re-decode, as that would invalidate the instruction instances here
 
     def update_instruction_offsets(self, instructions):
         # Update instruction positions
         for i, instruction in enumerate(instructions):
             instruction.offset = i
 
@@ -893,15 +1167,15 @@
         for i, instruction in enumerate(instructions):
             arg = instruction.arg
 
             if arg is None:
                 if instruction.opcode < dis.HAVE_ARGUMENT:
                     arg = 0
                 else:
-                    print(instruction)
+                    print("error", instruction)
 
             if arg >= 256**3:
                 count = 3
             elif arg >= 256**2:
                 count = 2
             elif arg >= 256:
                 count = 1
@@ -966,20 +1240,31 @@
         pending_instructions = [root]
         visited: typing.Set[Instruction] = set()
         instructions: typing.List[Instruction] = []
 
         while pending_instructions:
             instruction = pending_instructions.pop()
 
+            if not isinstance(instruction, Instruction):
+                print(f"Invalid task instruction: {instruction}")
+                continue
+
+            if not isinstance(instruction, Instruction):
+                raise ValueError(instruction)
+
             # If we visited it, we can skip
             if instruction in visited:
                 continue
 
             # Walk over the instructions as long as we have not met them
             while instruction not in visited:
+                if not isinstance(instruction, Instruction):
+                    print(f"Invalid task instruction: {instruction}")
+                    break
+
                 # If it branches off, it needs to be visited later on
                 if instruction.has_jump():
                     if instruction.arg_value is None:
                         instruction.update_owner(self, instruction.offset)
 
                     assert instruction.arg_value is not None, instruction
 
@@ -995,28 +1280,34 @@
                 ):
                     break
 
                 if instruction.next_instruction is None:
                     instruction.update_owner(self, instruction.offset)
 
                 # The next instruction MUST be set if it does NOT end the control flow
-                assert instruction.next_instruction is not None, instruction
+                if instruction.next_instruction is None:
+                    print("---- start dump")
+                    for instr in instructions:
+                        print(instr)
+                    print("---- end dump")
+                    raise RuntimeError(f"next instruction is None: {instruction}")
 
                 instruction = instruction.next_instruction
 
         return instructions
 
     def assemble_instructions(self):
 
         # Check for linearity violations
         for i, instruction in enumerate(self.__instructions):
             if (
                 instruction.next_instruction is not None
                 and instruction.offset + 1 != instruction.next_instruction.offset
                 and not instruction.has_unconditional_jump()
+                and not instruction.has_stop_flow()
             ):
                 # todo: do we want to dynamic use assemble_instructions_from_tree()?
                 raise LinearCodeConstraintViolationException(
                     f"Failed between instruction {instruction} and {instruction.next_instruction}, use assemble_instructions_from_tree(...) to assemble from an non-normal tree"
                 )
 
         needs_tree_assemble = False
@@ -1054,20 +1345,22 @@
                             self,
                             0,
                             "NOP",
                         )
                         root.next_instruction = instruction
                         missing -= 1
 
-                    # And now, insert the "NOP"'s required after the previous for the things
-                    for delta in range(missing):
-                        nop = Instruction(self, previous.offset + delta + 1, "NOP")
-                        nop.next_instruction = instruction
-                        previous.next_instruction = nop
-                        previous = nop
+                    previous.insert_after(
+                        [
+                            Instruction(self, previous.offset + i + 1, Opcodes.NOP)
+                            for i in range(missing)
+                        ]
+                    )
+
+                nop_count = 0
 
             previous = instruction
 
         if needs_tree_assemble:
             self.assemble_instructions_from_tree(root)
             return
 
@@ -1108,14 +1401,17 @@
         self.__instructions = [
             instruction.update_owner(self, i, update_following=False)
             for i, instruction in enumerate(instructions)
         ]
 
         self.__raw_code.clear()
         for i, instruction in enumerate(self.__instructions):
+            if instruction.opcode > 255:
+                raise ValueError(f"invalid instruction at result level: {instruction}")
+
             arg = instruction.get_arg()
 
             if arg > 255:
                 extend = arg // 256
                 arg %= 256
 
                 offset = 1
@@ -1182,14 +1478,20 @@
 
     def allocate_shared_variable_name(self, variable_name: str) -> int:
         if variable_name in self.shared_variable_names:
             return self.shared_variable_names.index(variable_name)
         self.shared_variable_names.append(variable_name)
         return len(self.shared_variable_names) - 1
 
+    def allocate_shared_cell(self, name: str):
+        if name in self.cell_variables:
+            return self.cell_variables.index(name)
+        self.cell_variables.append(name)
+        return len(self.cell_variables) - 1
+
     def dump_info(self, file: str):
         data = {
             "instructions": [
                 {
                     "opcode": instr.opcode,
                     "opname": instr.opname,
                     "arg": instr.arg,
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,78 @@
 import typing
 
 from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
 from bytecodemanipulation.Opcodes import Opcodes, HAS_GLOBAL
 from bytecodemanipulation.Opcodes import UNCONDITIONAL_JUMPS
 
 
+class Guarantees:
+    class AbstractGuarantee:
+        pass
+
+    RESULT_IS_CONSTANT = AbstractGuarantee()
+    NO_DISCARD = AbstractGuarantee()
+
+    class ArgIsNotMutated(AbstractGuarantee):
+        def __init__(self, arg_index: int, arg_name: str):
+            self.arg_index = arg_index
+            self.arg_name = arg_name
+
+    class ReturnType(AbstractGuarantee):
+        def __init__(self, data_type: type, may_subclass=False):
+            self.data_type = data_type
+            self.may_subclass = may_subclass
+
+
+class MethodInvocationInfo:
+    def __init__(self, call_instruction: Instruction):
+        self.call_instruction = call_instruction
+
+        if call_instruction.opcode == Opcodes.CALL_FUNCTION:
+            self.arg_loads = [
+                next(call_instruction.trace_stack_position(i))
+                for i in range(call_instruction.arg - 1, -1, -1)
+            ]
+            self.function_load = call_instruction.trace_normalized_stack_position(
+                call_instruction.arg
+            )
+        else:
+            raise NotImplementedError(call_instruction)
+
+        self._guarantees: typing.List[Guarantees.AbstractGuarantee] = None
+
+    def get_guarantees(self) -> typing.List[Guarantees.AbstractGuarantee]:
+        if self._guarantees:
+            return self._guarantees
+
+        if self.function_load.opcode != Opcodes.LOAD_CONST:
+            return []
+
+        from bytecodemanipulation.Optimiser import _OptimisationContainer
+
+        function_target = self.function_load.arg_value
+        optimisation_container = _OptimisationContainer.get_for_target(function_target)
+
+        self._guarantees = []
+        if optimisation_container.guarantees:
+            self._guarantees += optimisation_container.guarantees
+
+        return self._guarantees
+
+    def is_argument_mutated(self, name_or_index: str | int) -> bool:
+        for guarantee in self.get_guarantees():
+            if isinstance(guarantee, Guarantees.ArgIsNotMutated) and (
+                guarantee.arg_index == name_or_index
+                or guarantee.arg_name == name_or_index
+            ):
+                return False
+
+        return True
+
+
 class MutableFunctionWithTree:
     def __init__(self, mutable: MutableFunction, root: Instruction = None):
         self.mutable = mutable
         self.root = root or mutable.instructions[0]
 
     def visitor(
         self, visitor: typing.Callable[[Instruction, typing.List[Instruction]], None]
@@ -64,21 +128,26 @@
         self.print_recursive(root.next_instruction, visited, level)
 
         if root.has_jump():
             self.print_recursive(root.arg_value, visited, level + 1)
 
 
 def prefix_all_locals_with(
-    mutable: MutableFunction | MutableFunctionWithTree, prefix: str, protected_locals: typing.List[str] = tuple(),
+    mutable: MutableFunction | MutableFunctionWithTree,
+    prefix: str,
+    protected_locals: typing.List[str] = tuple(),
 ):
     if isinstance(mutable, MutableFunctionWithTree):
         mutable.mutable.assemble_instructions_from_tree(mutable.root)
         mutable = mutable.mutable
 
-    mutable.shared_variable_names = [prefix + e if e not in protected_locals else e for e in mutable.shared_variable_names]
+    mutable.shared_variable_names = [
+        prefix + e if e not in protected_locals else e
+        for e in mutable.shared_variable_names
+    ]
 
     print(mutable.shared_variable_names)
 
     for instruction in mutable.instructions:
         if instruction.has_local():
             instruction.update_owner(mutable, instruction.offset)
 
@@ -227,15 +296,15 @@
     prefix_all_locals_with(to_insert, to_insert.function_name + ":", protected_locals)
     replace_opcode_with_other(
         to_insert, Opcodes.RETURN_VALUE, Opcodes.INTERMEDIATE_INNER_RETURN
     )
     inline_access_to_global(to_insert, "capture_local", capture_local)
     inline_access_to_global(to_insert, "outer_return", outer_return)
 
-    MutableFunctionWithTree(to_insert).print_recursive()
+    # MutableFunctionWithTree(to_insert).print_recursive()
 
     instr = None
     previous = None
     for instr in to_insert.instructions:
         if previous is not None:
             previous.next_instruction = instr
 
@@ -256,36 +325,36 @@
         to_insert.instructions[0],
         breaks_flow=(
             Instruction.create(
                 Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
             ),
         ),
     )
-    MutableFunctionWithTree(to_insert).print_recursive()
+    # MutableFunctionWithTree(to_insert).print_recursive()
     # to_insert.decode_instructions()
 
     for instr in to_insert.instructions:
         instr.update_owner(body.mutable, -1, False)
 
     to_insert_tree = MutableFunctionWithTree(to_insert)
-    to_insert_tree.print_recursive()
+    # to_insert_tree.print_recursive()
     replace_const_func_call_with_opcode(
         to_insert_tree,
         capture_local,
         Opcodes.LOAD_FAST,
         _inline_capture_local,
     )
-    to_insert_tree.print_recursive()
+    # to_insert_tree.print_recursive()
     replace_const_func_call_with_opcode(
         to_insert_tree,
         outer_return,
         Opcodes.RETURN_VALUE,
         _inline_outer_return,
     )
-    to_insert_tree.print_recursive()
+    # to_insert_tree.print_recursive()
 
     def visit(instruction: Instruction, path):
         if instruction is None:
             print(path)
             raise
 
         instruction.function = body.mutable
@@ -302,12 +371,12 @@
             instruction.arg = body.mutable.allocate_shared_variable_name(
                 instruction.arg_value
             )
 
     HEAD_INSTRUCTION.next_instruction = to_insert_tree.root
     body.visitor(visit)
 
-    body.print_recursive()
+    # body.print_recursive()
 
     body.mutable.assemble_instructions_from_tree(body.root)
 
-    body.print_recursive()
+    # body.print_recursive()
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/Opcodes.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/Opcodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -146,17 +146,51 @@
     LOAD_METHOD = 160
     CALL_METHOD = 161
     LIST_EXTEND = 162
     SET_UPDATE = 163
     DICT_MERGE = 164
     DICT_UPDATE = 165
 
+    # Since python 3.11
+    CACHE = 166
+    PUSH_NULL = 167
+    PUSH_EXC_INFO = 168
+    CHECK_EXC_MATCH = 169
+    CHECK_EG_MATCH = 170
+    BEFORE_WITH = 171
+    RETURN_GENERATOR = 172
+    ASYNC_GEN_WRAP = 173
+    PREP_RERAISE_STAR = 174
+    SWAP = 175
+    POP_JUMP_FORWARD_IF_FALSE = 176
+    POP_JUMP_FORWARD_IF_TRUE = 177
+    COPY = 178
+    BINARY_OP = 179
+    SEND = 180
+    POP_JUMP_FORWARD_IF_NOT_NONE = 181
+    POP_JUMP_FORWARD_IF_NONE = 182
+    JUMP_BACKWARD_NO_INTERRUPT = 183
+    MAKE_CELL = 184
+    JUMP_BACKWARD = 185
+    COPY_FREE_VARS = 186
+    RESUME = 187
+    PRECALL = 188
+    CALL = 189
+    KW_NAMES = 190
+    POP_JUMP_BACKWARD_IF_NOT_NONE = 191
+    POP_JUMP_BACKWARD_IF_NONE = 192
+    POP_JUMP_BACKWARD_IF_FALSE = 193
+    POP_JUMP_BACKWARD_IF_TRUE = 194
+
     INTERMEDIATE_INNER_RETURN = 256
     INTERMEDIATE_OUTER_RETURN = 257
     INTERMEDIATE_LOAD_FAST = 258
+    BYTECODE_LABEL = 259
+    MACRO_PARAMETER_EXPANSION = 260
+    STATIC_ATTRIBUTE_ACCESS = 261
 
 
 OPCODE2NAME = {}
 OPNAME2CODE = {}
 
 
 def init_maps():
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/Optimiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import dis
 import inspect
 import math
 import os
+import re
+import string
+import struct
 import types
 import typing
 import builtins
+import random
 
+from bytecodemanipulation.MutableFunctionHelpers import Guarantees
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.Opcodes import Opcodes
 from bytecodemanipulation.optimiser_util import inline_const_value_pop_pairs
 from bytecodemanipulation.optimiser_util import inline_constant_binary_ops
 from bytecodemanipulation.optimiser_util import inline_constant_method_invokes
 from bytecodemanipulation.optimiser_util import inline_static_attribute_access
 from bytecodemanipulation.optimiser_util import remove_branch_on_constant
@@ -41,34 +46,40 @@
 
     @classmethod
     def apply_all(cls):
         for target in cls._CONTAINERS:
             target.run_optimisers(False)
 
     @classmethod
-    def get_for_target(cls, target):
+    def get_for_target(
+        cls,
+        target: types.FunctionType | types.MethodType | typing.Type | types.ModuleType,
+    ):
 
         if hasattr(target, "_OPTIMISER_CONTAINER"):
             return target._OPTIMISER_CONTAINER
 
         if target in cls._CUSTOM_TARGETS:
             return cls._CUSTOM_TARGETS[target]
 
         container = cls(target)
 
         cls._CONTAINERS.append(container)
 
         try:
             target._OPTIMISER_CONTAINER = container
-        except (AttributeError,  TypeError):
+        except (AttributeError, TypeError):
             cls._CUSTOM_TARGETS[target] = container
 
         return container
 
-    def __init__(self, target: types.FunctionType | types.MethodType | typing.Type):
+    def __init__(
+        self,
+        target: types.FunctionType | types.MethodType | typing.Type | types.ModuleType,
+    ):
         self.target = target
         self.parents: typing.List["_OptimisationContainer"] = []
         self.children: typing.List["_OptimisationContainer"] = []
         self.optimisations: typing.List[AbstractOptimisationWalker] = []
 
         # Global names that are constant (e.g. imports)
         self.lazy_global_name_cache: typing.Dict[str, typing.Callable[[], object]] = {}
@@ -122,30 +133,52 @@
         self.static_attributes: typing.Set[str] = set()
 
         # Exceptions that can be raised from here
         self.may_raise_exceptions: typing.Set[
             typing.Type[Exception] | Exception
         ] | None = None
 
-        self.specializations: typing.List[typing.Callable[[SpecializationContainer], None]] = []
+        self.specializations: typing.List[
+            typing.Callable[[SpecializationContainer], None]
+        ] = []
 
         self.is_optimized = False
 
         # Add the children to self
         if isinstance(self.target, type):
             for key, e in self.target.__dict__.items():
-                if isinstance(e, (type(guarantee_builtin_names_are_protected), staticmethod, classmethod, type)):
+                if isinstance(
+                    e,
+                    (
+                        type(guarantee_builtin_names_are_protected),
+                        staticmethod,
+                        classmethod,
+                        type,
+                    ),
+                ):
                     if isinstance(e, (staticmethod, classmethod)):
                         func = e.__func__
                     else:
                         func = e
 
-                    if func.__qualname__.startswith(self.target.__qualname__+".") and func.__module__ == self.target.__module__:
+                    if (
+                        func.__qualname__.startswith(self.target.__qualname__ + ".")
+                        and func.__module__ == self.target.__module__
+                    ):
                         self.children.append(self.get_for_target(e))
 
+        self.guarantees: typing.List[Guarantees.AbstractGuarantee] | None = None
+
+    def add_guarantee(self, guarantee: Guarantees.AbstractGuarantee):
+        if self.guarantees is None:
+            self.guarantees = []
+
+        self.guarantees.append(guarantee)
+        return self
+
     def is_attribute_static(self, name: str):
         return self.is_static or name in self.static_attributes
 
     def _walk_children_and_copy_attributes(self):
         for value in self.target.__dict__.values():
             if (
                 isinstance(value, type)
@@ -192,27 +225,29 @@
             return
 
         self.is_optimized = True
 
         if DISABLE_OPTIMISATION_APPLY:
             return
 
-        print("opt", self.target)
+        # print("opt", self.target)
         from bytecodemanipulation.optimiser_util import apply_specializations
 
         if self.children:
             self._walk_children_and_copy_attributes()
 
             for child in self.children:
                 child.run_optimisers()
 
         # resolve the lazy types
         self._resolve_lazy_references()
 
-        if not hasattr(self.target, "__code__") and not isinstance(self.target, (classmethod, staticmethod)):
+        if not hasattr(self.target, "__code__") and not isinstance(
+            self.target, (classmethod, staticmethod)
+        ):
             return
 
         # Create mutable wrapper around the target
         mutable = MutableFunction.create(self.target)
         mutable.prepare_previous_instructions()
 
         # Walk over the code and resolve cached globals
@@ -285,15 +320,18 @@
                 if key not in self.dereference_local_var_type:
                     self.dereference_local_var_type[key] = lazy()
 
             for key, lazy in self.lazy_local_var_attr_type.items():
                 if key not in self.dereference_local_var_attr_type:
                     self.dereference_local_var_attr_type[key] = lazy()
 
-            if self.dereference_return_type is None and self.lazy_return_type is not None:
+            if (
+                self.dereference_return_type is None
+                and self.lazy_return_type is not None
+            ):
                 self.dereference_return_type = self.lazy_return_type()
 
             for key, lazy in self.lazy_return_attr_type.items():
                 if key not in self.dereference_return_attr_type:
                     self.dereference_return_attr_type[key] = lazy()
 
             for key, lazy in self.lazy_attribute_type.items():
@@ -355,14 +393,18 @@
                     source.change_opcode(Opcodes.NOP)
                     dirty = True
 
         return dirty
 
 
 _OptimisationContainer.get_for_target(typing).is_static = True
+_OptimisationContainer.get_for_target(random).is_static = True
+_OptimisationContainer.get_for_target(string).is_static = True
+_OptimisationContainer.get_for_target(re).is_static = True
+_OptimisationContainer.get_for_target(struct).is_static = True
 _OptimisationContainer.get_for_target(math).is_static = True
 _OptimisationContainer.get_for_target(os).is_static = True
 
 
 class AbstractOptimisationWalker:
     """
     Optimisation walker for classes and functions, constructed by the optimiser annotations
@@ -537,14 +579,15 @@
         raise ValueError("Both data_type and lazy_data_type are provided!")
 
     def annotate(target):
         container = _OptimisationContainer.get_for_target(target)
         container.lazy_return_type = (
             lazy_data_type if lazy_data_type is not None else lambda: data_type
         )
+        container.add_guarantee(Guarantees.ReturnType(data_type or lazy_data_type))
 
         return target
 
     return annotate
 
 
 def guarantee_exact_return_attribute_type(
@@ -636,14 +679,15 @@
     Guarantees that this function will return the same value if invoked with the same args
     Implies that the function does NOT modify the args again if seen again.
     """
 
     def annotate(target):
         container = _OptimisationContainer.get_for_target(target)
         container.is_constant_op = True
+        container.add_guarantee(Guarantees.RESULT_IS_CONSTANT)
 
         return target
 
     return annotate
 
 
 def guarantee_side_effect_free_call():
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/compiler.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """
     Parses a 'file' (path) as a 'module_name'
     and returns the resulting ModuleType
 
     @bytecode:guarantee_not_empty[file]
     @bytecode:guarantee_not_empty[module_name]
     """
-    with open(file, 'rb') as f:
+    with open(file, "rb") as f:
         data = f.read()
 
         f.seek(0)
 
         tokens = list(tokenize.tokenize(f.readline))
 
     ast_tree = ast.parse(data, file)
@@ -92,8 +92,7 @@
             break
 
     return module
 
 
 if __name__ == "__main__":
     parse(__file__, "__main__")
-
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/data_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from bytecodemanipulation import Opcodes as OpcodesM
 from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
 
 
 local = os.path.dirname(__file__)
 
 version = f"{sys.version_info.major}_{sys.version_info.minor}"
-folder = local + "/data/" + version
+folder = local + "/data/v" + version
+sys.path.append(os.path.dirname(local))
+
+
+INIT_ASSEMBLY = True
 
 
 def load_opcode_data():
     opcode_data: dict = json.load(open(folder + "/opcodes.json"))
 
     valid_opcode_names = [
         key
@@ -49,15 +53,15 @@
     builtin_spec = json.load(open(folder + "/builtins.json"))
 
     CONSTANT_BUILTINS[:] = [getattr(builtins, key) for key in builtin_spec["constant"]]
     CONSTANT_BUILTIN_TYPES[:] = [
         getattr(builtins, key) for key in builtin_spec["const_builtin_types"]
     ]
 
-    importlib.import_module("bytecodemanipulation.data."+version+".specialize")
+    importlib.import_module("bytecodemanipulation.data.v" + version + ".specialize")
 
 
 def load_standard_library_annotations():
     import importlib
 
     std_annot = json.load(open(folder + "/standard_library.json"))
 
@@ -68,13 +72,29 @@
             attr = module
             for e in name.split("."):
                 attr = getattr(attr, e)
 
             CONSTANT_BUILTINS.append(attr)
 
 
+ASSEMBLY_MODULE = {}
+
+
+def load_assembly_instructions():
+    if os.path.exists(folder + "/assembly_instructions.py"):
+        # exec(open(folder + "/assembly_instructions.py").read(), ASSEMBLY_MODULE)
+        ASSEMBLY_MODULE.update(
+            importlib.import_module(
+                "bytecodemanipulation.data.v" + version + ".assembly_instructions"
+            ).__dict__
+        )
+
+
 def init():
     load_opcode_data()
     init_maps()
     load_instruction_spec()
     load_builtin_spec()
     load_standard_library_annotations()
+
+    if INIT_ASSEMBLY:
+        load_assembly_instructions()
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/mixin_util.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/mixin_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 import typing
 
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.Opcodes import Opcodes
 
 
-def resolve_accesses(inject_target: MutableFunction, injected: MutableFunction) -> typing.List[str]:
+def resolve_accesses(
+    inject_target: MutableFunction, injected: MutableFunction
+) -> typing.List[str]:
     BOUND_LOCALS = {}
     BOUND_CELL_VARIABLES = {}
 
     for instruction in injected.instructions:
         if instruction.has_local():
-            instruction.change_arg_value(injected.function_name + "::" + instruction.arg_value)
+            instruction.change_arg_value(
+                injected.function_name + "::" + instruction.arg_value
+            )
 
     for instruction in injected.instructions:
-        if instruction.opcode in (Opcodes.CALL_METHOD, Opcodes.CALL_FUNCTION) and instruction.arg <= 1:
+        if (
+            instruction.opcode in (Opcodes.CALL_METHOD, Opcodes.CALL_FUNCTION)
+            and instruction.arg <= 1
+        ):
             source = next(instruction.trace_stack_position(instruction.arg))
 
             if source.opcode == Opcodes.LOAD_CONST:
                 target = source.arg_value
 
-                if not isinstance(target, classmethod): continue
+                if not isinstance(target, classmethod):
+                    continue
 
                 func_name = target.__name__
                 is_const = True
                 source_source = None
             elif source.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
                 source_source = next(source.trace_stack_position(0))
 
-                if source_source.opcode == Opcodes.LOAD_FAST and source_source.arg_value in ("self", "cls"):
+                if (
+                    source_source.opcode == Opcodes.LOAD_FAST
+                    and source_source.arg_value in ("self", "cls")
+                ):
                     func_name = source.arg_value
                     is_const = False
                 else:
                     continue
             else:
                 continue
 
             if func_name == "resolve_local":
-                assert instruction.arg == 1, f"resolve_local() must be invoked with exactly one arg, got {instruction.arg}"
+                assert (
+                    instruction.arg == 1
+                ), f"resolve_local() must be invoked with exactly one arg, got {instruction.arg}"
 
                 variable_name = next(instruction.trace_stack_position(0))
 
-                assert variable_name.opcode == Opcodes.LOAD_CONST, f"resolve_local(<xy>) MUST be invoked with a constant, got {instruction}"
+                assert (
+                    variable_name.opcode == Opcodes.LOAD_CONST
+                ), f"resolve_local(<xy>) MUST be invoked with a constant, got {instruction}"
 
                 target = next(instruction.trace_stack_position_use(0))
 
                 if target.opcode == Opcodes.STORE_FAST:
                     BOUND_LOCALS[target.arg_value] = variable_name.arg_value
                 else:
                     instruction.change_opcode(Opcodes.LOAD_FAST)
                     instruction.change_arg_value(variable_name.arg_value)
                     source.change_opcode(Opcodes.NOP)
 
                     if not is_const:
                         source_source.change_opcode(Opcodes.NOP)
 
             elif func_name == "resolve_cell_variable":
-                assert instruction.arg == 1, f"resolve_cell_variable() must be invoked with exactly one arg, got {instruction.arg}"
+                assert (
+                    instruction.arg == 1
+                ), f"resolve_cell_variable() must be invoked with exactly one arg, got {instruction.arg}"
 
                 variable_name = next(instruction.trace_stack_position(0))
 
-                assert variable_name.opcode == Opcodes.LOAD_CONST, f"resolve_cell_variable(<xy>) MUST be invoked with a constant, got {instruction}"
+                assert (
+                    variable_name.opcode == Opcodes.LOAD_CONST
+                ), f"resolve_cell_variable(<xy>) MUST be invoked with a constant, got {instruction}"
 
                 target = next(instruction.trace_stack_position_use(0))
 
                 if target.opcode == Opcodes.STORE_FAST:
                     BOUND_CELL_VARIABLES[target.arg_value] = variable_name
                 else:
                     instruction.change_opcode(Opcodes.LOAD_DEREF)
@@ -76,11 +95,12 @@
                         source_source.change_opcode(Opcodes.NOP)
 
         elif instruction.has_local():
             if instruction.arg_value in BOUND_LOCALS:
                 instruction.change_arg_value(BOUND_LOCALS[instruction.arg_value])
             elif instruction.arg_value in BOUND_CELL_VARIABLES:
                 instruction.change_opcode(instruction.opname.replace("FAST", "DEREF"))
-                instruction.change_arg_value(BOUND_CELL_VARIABLES[instruction.arg_value])
+                instruction.change_arg_value(
+                    BOUND_CELL_VARIABLES[instruction.arg_value]
+                )
 
     return list(BOUND_LOCALS.keys())
-
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.2.4/bytecodemanipulation/optimiser_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                     and getattr(function, "_OPTIMISER_CONTAINER").is_constant_op
                 ):
                     args = [
                         next(instr.trace_stack_position(i))
                         for i in range(instr.arg - 1, -1, -1)
                     ]
 
-                    if all(instr.opcode == Opcodes.LOAD_CONST for instr in args):
+                    if all(ins.opcode == Opcodes.LOAD_CONST for ins in args):
                         result = function(*(e.arg_value for e in args))
 
                         instr.change_opcode(Opcodes.LOAD_CONST)
                         instr.change_arg_value(result)
                         target.change_opcode(Opcodes.NOP)
 
                         for arg in args:
@@ -341,17 +341,24 @@
     return dirty
 
 
 def remove_branch_on_constant(mutable: MutableFunction) -> bool:
     dirty = False
 
     for instruction in mutable.instructions:
-        if instruction.has_jump() and not instruction.has_unconditional_jump() and instruction.opcode not in (Opcodes.SETUP_FINALLY, Opcodes.SETUP_WITH):
+        if (
+            instruction.has_jump()
+            and not instruction.has_unconditional_jump()
+            and instruction.opcode not in (Opcodes.SETUP_FINALLY, Opcodes.SETUP_WITH)
+        ):
             if instruction.previous_instructions is None:
-                if instruction.offset == 0 and instruction.opcode == Opcodes.SETUP_FINALLY:
+                if (
+                    instruction.offset == 0
+                    and instruction.opcode == Opcodes.SETUP_FINALLY
+                ):
                     continue
 
                 raise RuntimeError
 
             source = next(instruction.trace_stack_position(0))
 
             if source.opcode == Opcodes.LOAD_CONST:
@@ -411,15 +418,15 @@
                     instruction.arg_value
                 ):
                     attr_name = instruction.arg_value
                     source_instr.change_opcode(Opcodes.NOP)
                     instruction.change_opcode(Opcodes.LOAD_CONST)
                     instruction.change_arg_value(getattr(source, attr_name))
 
-                    print(instruction)
+                    # print(instruction)
 
                     use = next(instruction.trace_stack_position_use(0))
 
                     if use.opcode == Opcodes.CALL_METHOD:
                         use.change_opcode(Opcodes.CALL_FUNCTION)
 
                     dirty = True
@@ -443,20 +450,29 @@
 
                 if not container.specializations:
                     continue
 
                 target_func = source.arg_value
 
                 spec = SpecializationContainer()
+                spec.target = mutable
                 spec.underlying_function = target_func
-                spec.method_call_descriptor = MethodCallDescriptor(safe_source, instruction)
-                spec.set_arg_descriptors([
-                    ArgDescriptor(next(instruction.trace_stack_position(arg_id)), instruction.trace_normalized_stack_position(arg_id), arg_id)
-                    for arg_id in range(instruction.arg-1, -1, -1)
-                ])
+                spec.method_call_descriptor = MethodCallDescriptor(
+                    safe_source, instruction
+                )
+                spec.set_arg_descriptors(
+                    [
+                        ArgDescriptor(
+                            next(instruction.trace_stack_position(arg_id)),
+                            instruction.trace_normalized_stack_position(arg_id),
+                            arg_id,
+                        )
+                        for arg_id in range(instruction.arg - 1, -1, -1)
+                    ]
+                )
 
                 for special in container.specializations:
                     special(spec)
 
                     if spec.no_special:
                         continue
```

### Comparing `bytecodemanipulation-0.2.2/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.2.4/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.2.2
+Version: 0.2.4
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -82,30 +82,42 @@
 # Examples
 
 TODO
 
 
 # Applied Optimisations
 
-- Constant Expression inlining
+- Constant Expression inlining (can be declared for custom functions to be constant)
 - LOAD_GLOBAL for builtins (if enabled)
 - standard library inlining (if enabled)
 - specialization of methods based on arguments, e.g. constant arguments (when already resolved before, requires one of above options)
-- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time)
+- branch elimination when jumping on a constant (TODO: also if condition can be inferred ahead-of-time, see specialization)
+- local variable elimination
 
 
 # Currently Limitations
 
 - Line Numbers get mixed up, we need some way to assign meaningful line numbers
 - With python 3.11 (?), exception table exists, and this breaks our current concept of one big flow diagram,
   as exception handling code might exist outside the default flow
 - During optimization, a lot of stuff is being recomputed each optimisation pass, we need to cache that drastically
 - Method inlining is not working properly and needs a lot more testing
 - If the exact type is known at optimisation time (e.g. object creation via class call, or type annotation), we can try to
   inline method accesses for further optimisation
+- Python 3.12 will likely break how certain operations are stored in instructions, combing opcodes-without-args into a single
+  parent instruction, using the arg to switch between modes
+
+
+# Assembly Code
+
+- The library provides also a way to use some "python-assembly" for writing code
+- This is only python bytecode, so no fancy stuff can be done
+- See ASSEMBLY.md for more information on instructions
+- We provide an import system hook for importing .pyasm files via bytecodemanipulation.assembler.hook
+- You may use the functions from bytecodemanipulation.assembler.target for creating inline-assembly
 
 
 ## Code Formatting
 
 We use the python formatting library "black" on our code
 
 # TODO's
```

### Comparing `bytecodemanipulation-0.2.2/setup.py` & `bytecodemanipulation-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.2.2",
+    version="0.2.4",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

