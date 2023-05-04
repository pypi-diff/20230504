# Comparing `tmp/appeal-0.5.7.tar.gz` & `tmp/appeal-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.7.tar", last modified: Wed May  3 18:44:38 2023, max compression
+gzip compressed data, was "appeal-0.5.8.tar", last modified: Thu May  4 07:00:10 2023, max compression
```

## Comparing `appeal-0.5.7.tar` & `appeal-0.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.7/.gitignore
--rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.7/LICENSE
--rw-r--r--   0        0        0    67303 2023-05-03 18:37:18.618814 appeal-0.5.7/README.md
--rw-r--r--   0        0        0   173042 2023-05-03 18:37:47.599733 appeal-0.5.7/appeal/__init__.py
--rw-r--r--   0        0        0    23346 2023-05-02 08:25:22.602769 appeal-0.5.7/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.7/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.7/appeal/text.py
--rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.7/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/links.txt
--rw-r--r--   0        0        0    65199 2023-05-03 18:16:25.747049 appeal-0.5.7/tests/run_tests.py
--rw-r--r--   0        0        0    67797 1970-01-01 00:00:00.000000 appeal-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.8/LICENSE
+-rw-r--r--   0        0        0    68258 2023-05-04 06:59:09.308913 appeal-0.5.8/README.md
+-rw-r--r--   0        0        0   174135 2023-05-04 06:53:52.222431 appeal-0.5.8/appeal/__init__.py
+-rw-r--r--   0        0        0    23346 2023-05-02 08:25:22.602769 appeal-0.5.8/appeal/argument_grouping.py
+-rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.8/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.8/appeal/text.py
+-rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/links.txt
+-rw-r--r--   0        0        0    67934 2023-05-04 06:53:04.228844 appeal-0.5.8/tests/run_tests.py
+-rw-r--r--   0        0        0    68752 1970-01-01 00:00:00.000000 appeal-0.5.8/PKG-INFO
```

### Comparing `appeal-0.5.7/LICENSE` & `appeal-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/README.md` & `appeal-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1965,22 +1965,42 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.8**
+
+* Fixed up the "name" of the program for options.  We used to take
+  the name of the command, add all the option strings, and join it
+  together with commas, as in `'command, -o, --option'`.  Now it
+  looks like `'command -o | --option'`.
+* Fixed presentation bug: if you didn't have enough positional
+  arguments for your command function, but you ever invoked an
+  option on the command-line, the usage text would contain the
+  name of the last option invoked (aka the last Charm program run).
+  Added a regression test for this.
+* Cleaned up implementation a little: instead of using mystery
+  lists on the `CharmInterpreter` stack and context_stack, I now
+  use instances of bespoke `CharmStackEntry` and
+  `CharmContextStackEntry` classes.
+
 **0.5.7**
 
 * Rewrite the technology behind `accumulator[...]` and
   `mapping[...]`.  It previously used `exec()`, which was
   limiting; for example, you couldn't use your own types
   or converters.  The new implementation should be much
   more robust; it now manually defines an explicit signature
   for the `option()` method of the subclass it creates.
+* This fixed a regression, where you couldn't use a locally-defined
+  class (e.g. `IntFloat`) as one of the types in the square
+  brackets for `accumulator` and `mapping`.  Added a test
+  for this.
 
 **0.5.6**
 
 * Fix formatting for usage when you have a
   global command *and* subcommands.
 
 **0.5.5**
```

### Comparing `appeal-0.5.7/appeal/__init__.py` & `appeal-0.5.8/appeal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.7"
+__version__ = "0.5.8"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -1253,17 +1253,19 @@
         if want_prints:
             indent = "  " * depth
             print(f"[cc] {indent}compile_options options={options} key={key} parameter={parameter} parameter.kind={parameter.kind}")
 
         cls = self.appeal.root.map_to_converter(parameter)
 
         assert options
-        strings = [f"{parent_callable.__name__}"]
-        strings.extend(denormalize_option(o) for o in options)
-        program_name = ", ".join(strings)
+        name = parent_callable.__name__
+        option_names = [denormalize_option(o) for o in options]
+        assert option_names
+        option_names = " | ".join(option_names)
+        program_name = f"{name} {option_names}"
         if cls is SimpleTypeConverterStr:
             if want_prints:
                 print(f"[cc] {indent}(hand-coded str option)")
             program = CharmProgram(name=program_name, minimum=1, maximum=1)
             a = CharmAssembler(self)
             a.push_context()
             a.set_group(1, 1, optional=False)
@@ -1773,14 +1775,36 @@
         self.ip = address
 
     def jump_relative(self, delta):
         self.ip += delta
 
 
 
+class CharmStackEntry:
+    def __init__(self, i, program, context_count=0):
+        self.i = i
+        self.program = program
+        self.context_count = context_count
+
+    def __repr__(self):
+        return f"<CharmStackEntry i={self.i} program={self.program.name!r} context_count={self.context_count}>"
+
+
+class CharmContextStackEntry:
+    def __init__(self, converter, group, o, option, total):
+        self.converter = converter
+        self.group = group
+        self.o = o
+        self.option = option
+        self.total = total
+
+    def __repr__(self):
+        return f"<CharmContextStackEntry converter={self.converter} group={self.group} o={self.o} option={self.option} total={self.total}>"
+
+
 class CharmInterpreter:
     def __init__(self, program, *, name=''):
         self.name = name
         self.stack = []
         self.context_stack = []
 
         assert program
@@ -1788,14 +1812,15 @@
         # registers
         self.converter = None
         self.o = None
         self.option = None
         self.total = None
         self.group = None
         self.converters = {}
+        self.program = program
 
         self.op = None
 
         # ip register actually lives inside the iterator
         self.i = CharmProgramIterator(program)
 
     def repr_ip(self):
@@ -1834,44 +1859,51 @@
                     print("()>", op)
                 return op
             except StopIteration as e:
                 self.finish()
                 continue
 
     def __bool__(self):
-        return bool(self.i) or any(bool(i) for i in self.stack)
+        return bool(self.i) or any(bool(cse.i) for cse in self.stack)
 
     def rewind(self):
         if self.i is None:
             raise StopIteration
         self.i.jump_relative(-1)
 
     def call(self, program):
-        self.stack.append([self.i, 0])
+        self.stack.append(CharmStackEntry(self.i, self.program))
+        self.program = program
         self.i = CharmProgramIterator(program)
 
     def push_context(self):
-        context = [self.converter, self.o, self.option, self.total, self.group]
+        context = CharmContextStackEntry(self.converter, self.group, self.o, self.option, self.total)
         self.context_stack.append(context)
         if self.stack:
-            self.stack[-1][-1] += 1
+            self.stack[-1].context_count += 1
 
     def _pop_context(self):
         context = self.context_stack.pop()
-        self.converter, self.o, self.option, self.total, self.group = context
+        self.converter = context.converter
+        self.group = context.group
+        self.o = context.o
+        self.option = context.option
+        self.total = context.total
 
     def pop_context(self):
         self._pop_context()
         if self.stack:
-            self.stack[-1][-1] -= 1
+            self.stack[-1].context_count -= 1
 
     def finish(self):
         if self.stack:
-            self.i, context_pops = self.stack.pop()
-            for i in range(context_pops):
+            cse = self.stack.pop()
+            self.i = cse.i
+            self.program = cse.program
+            for i in range(cse.context_count):
                 self._pop_context()
         else:
             self.i = None
 
     def abort(self):
         self.i = None
         self.stack.clear()
@@ -2496,14 +2528,15 @@
             which = "total"
             ag = ci.total
         if ag.minimum == ag.maximum:
             plural = "" if ag.minimum == 1 else "s"
             middle = f"{ag.minimum} argument{plural}"
         else:
             middle = f"at least {ag.minimum} arguments but no more than {ag.maximum} arguments"
+        program = ci.program
         message = f"{program.name} requires {middle} {which}."
 
         raise AppealUsageError(message)
 
     if want_prints:
         print(f"##")
         print(f"## ending parse.")
```

### Comparing `appeal-0.5.7/appeal/argument_grouping.py` & `appeal-0.5.8/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/appeal/cpp.py` & `appeal-0.5.8/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/appeal/text.py` & `appeal-0.5.8/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/pyproject.toml` & `appeal-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/resources/images/appeal.logo.png` & `appeal-0.5.8/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/resources/images/give.your.program.appeal.png` & `appeal-0.5.8/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.7/tests/run_tests.py` & `appeal-0.5.8/tests/run_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,26 @@
 
 def five_a(*, d:five_d=None, e=False, f=False):
     return (five_a, d, e, f)
 
 def five_level_stack(*, a:five_a=None, b=False, c=False):
     return (five_level_stack, a, b, c)
 
+
+class IntFloat:
+    def __init__(self, integer:int, real:float):
+        self.i = integer
+        self.f = real
+
+    def __repr__(self):
+        return f"<IntFloat i={self.i!r} f={self.f!r}>"
+
+def str_i_f(value, i_f:IntFloat=None, *, option=None, verbose=False):
+    return (str_i_f, value, i_f, option, verbose)
+
 class SmokeTests(unittest.TestCase):
     def setUp(self):
         global app
         global command
         global process
         app = appeal.Appeal(
             usage_max_columns=80,
@@ -324,16 +336,22 @@
             return app.process(args)
         process = my_process
 
     def assert_process(self, cmdline, result):
         self.assertEqual(process(shlex.split(cmdline)), result)
 
     def assert_process_raises(self, cmdline, exception):
+        e = None
         with self.assertRaises(exception):
-            process(shlex.split(cmdline))
+            try:
+                process(shlex.split(cmdline))
+            except exception as e2:
+                e = e2
+                raise e2
+        return e
 
     def tearDown(self):
         global app
         global command
         app = command = None
 
     def test_test_usage(self):
@@ -1254,14 +1272,77 @@
         command(five_level_stack)
         self.maxDiff=None
         self.assert_process(
             "five_level_stack -a -d -g -j -m -behknp",
             (five_level_stack, (five_a, (five_d, (five_g, (five_j, (five_m, True, False, False), True, False), True, False), True, False), True, False), True, False),
             )
 
+    def test_str_i_f_1(self):
+        command(str_i_f)
+        e = self.assert_process_raises(
+            "str_i_f abc 1",
+            appeal.AppealUsageError,
+            )
+        self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
+
+        # regression test:
+        # when printing usage, we used to print the name of the last program
+        # we'd called, regardless of whether or not it was currently running.
+        # so this error used to read
+        #   str_i_f, -v, --verbose requires 2 arguments in this argument group.
+        e = self.assert_process_raises(
+            "str_i_f abc 1 --verbose",
+            appeal.AppealUsageError,
+            )
+        self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
+
+        e = self.assert_process_raises(
+            "str_i_f abc 1 --option x",
+            appeal.AppealUsageError,
+            )
+        self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
+
+        e = self.assert_process_raises(
+            "str_i_f abc 1 --option",
+            appeal.AppealUsageError,
+            )
+        self.assertEqual(str(e), "str_i_f -o | --option requires 1 argument in this argument group.")
+
+
+    def test_app_class(self):
+        app = appeal.Appeal()
+        app_class, command_method = app.app_class()
+
+        instances = []
+        @app_class()
+        class MyApp:
+            def __init__(self, *, verbose=False):
+                self.verbose = verbose
+                self.pattern = None
+                self.filename = None
+                self.context = None
+                instances.append(self)
+
+            @command_method()
+            def fgrep(self, pattern, filename, *, context=0):
+                self.pattern = pattern
+                self.filename = filename
+                self.context = context
+
+            def dump(self):
+                return self.verbose, self.pattern, self.filename, self.context
+
+        result = app.process(shlex.split("-v fgrep patt -c 33 file"))
+        self.assertEqual(result, None)
+        self.assertEqual(len(instances), 1)
+        instance = instances.pop()
+        self.assertIsInstance(instance, MyApp)
+        self.assertEqual(instance.dump(), (True, 'patt', 'file', 33))
+
+
 
 ##
 ## I got tired of the examples in README.md not working
 ## or being out of sync with the implementation.
 ## So now I ensure the examples in README.md are always
 ## working--because I run them.
 ##
```

### Comparing `appeal-0.5.7/PKG-INFO` & `appeal-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.7
+Version: 0.5.8
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -1978,22 +1978,42 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.8**
+
+* Fixed up the "name" of the program for options.  We used to take
+  the name of the command, add all the option strings, and join it
+  together with commas, as in `'command, -o, --option'`.  Now it
+  looks like `'command -o | --option'`.
+* Fixed presentation bug: if you didn't have enough positional
+  arguments for your command function, but you ever invoked an
+  option on the command-line, the usage text would contain the
+  name of the last option invoked (aka the last Charm program run).
+  Added a regression test for this.
+* Cleaned up implementation a little: instead of using mystery
+  lists on the `CharmInterpreter` stack and context_stack, I now
+  use instances of bespoke `CharmStackEntry` and
+  `CharmContextStackEntry` classes.
+
 **0.5.7**
 
 * Rewrite the technology behind `accumulator[...]` and
   `mapping[...]`.  It previously used `exec()`, which was
   limiting; for example, you couldn't use your own types
   or converters.  The new implementation should be much
   more robust; it now manually defines an explicit signature
   for the `option()` method of the subclass it creates.
+* This fixed a regression, where you couldn't use a locally-defined
+  class (e.g. `IntFloat`) as one of the types in the square
+  brackets for `accumulator` and `mapping`.  Added a test
+  for this.
 
 **0.5.6**
 
 * Fix formatting for usage when you have a
   global command *and* subcommands.
 
 **0.5.5**
```

