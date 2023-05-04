# Comparing `tmp/asytest-0.1.3.tar.gz` & `tmp/asytest-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asytest-0.1.3.tar", last modified: Mon May  1 18:02:40 2023, max compression
+gzip compressed data, was "asytest-0.1.4.tar", last modified: Thu May  4 13:26:35 2023, max compression
```

## Comparing `asytest-0.1.3.tar` & `asytest-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.065968 asytest-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 18:02:22.000000 asytest-0.1.3/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 18:02:22.000000 asytest-0.1.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 18:02:22.000000 asytest-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 18:02:22.000000 asytest-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 18:02:40.073968 asytest-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 18:02:22.000000 asytest-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 18:02:22.000000 asytest-0.1.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/example_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 18:02:22.000000 asytest-0.1.3/example_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-01 18:02:22.000000 asytest-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 18:02:22.000000 asytest-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:02:40.073968 asytest-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.069968 asytest-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/src/asytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 18:02:39.000000 asytest-0.1.3/src/asytest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-01 18:02:22.000000 asytest-0.1.3/src/asytest/asytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/src/asytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 18:02:40.000000 asytest-0.1.3/src/asytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:02:40.073968 asytest-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 18:02:22.000000 asytest-0.1.3/tests/test_asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.173889 asytest-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-04 13:26:20.000000 asytest-0.1.4/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 13:26:20.000000 asytest-0.1.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-04 13:26:20.000000 asytest-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 13:26:20.000000 asytest-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 13:26:35.181889 asytest-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 13:26:20.000000 asytest-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-04 13:26:20.000000 asytest-0.1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/example_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 13:26:20.000000 asytest-0.1.4/example_tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 13:26:20.000000 asytest-0.1.4/example_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 13:26:20.000000 asytest-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 13:26:20.000000 asytest-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:26:35.181889 asytest-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.173889 asytest-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.177889 asytest-0.1.4/src/asytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-04 13:26:20.000000 asytest-0.1.4/src/asytest/asytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/src/asytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 13:26:35.000000 asytest-0.1.4/src/asytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:26:35.181889 asytest-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-04 13:26:20.000000 asytest-0.1.4/tests/test_asytest.py
```

### Comparing `asytest-0.1.3/.github/workflows/build.yaml` & `asytest-0.1.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.3/.github/workflows/release.yaml` & `asytest-0.1.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.3/LICENSE` & `asytest-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asytest-0.1.3/PKG-INFO` & `asytest-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asytest-0.1.3/dev-requirements.txt` & `asytest-0.1.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `asytest-0.1.3/example_tests/test_dummy.py` & `asytest-0.1.4/example_tests/test_concurrent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 import asyncio
 
-async def util_function():
-    print("util")
-
 async def test_http_call_1():
     print("start 1")
     await asyncio.sleep(1)
     print("end 1")
 
 async def test_http_call_2():
     print("start 2")
     await asyncio.sleep(1)
-    x = []
-    print(x.length)
+    print("end 2")
 
-async def test_with_a_very_long_name_http_call_3():
+async def test_http_call_3():
     print("start 3")
     await asyncio.sleep(1)
-    assert False
+    print("end 3")
 
 async def test_http_call_4():
     print("start 4")
     await asyncio.sleep(1)
     print("end 4")
 
 async def test_http_call_5():
     print("start 5")
     await asyncio.sleep(1)
-    print("end 5")
+    print("end 5")
+
+async def test_http_call_6():
+    print("start 6")
+    await asyncio.sleep(1)
+    print("end 6")
+
+async def test_http_call_7():
+    print("start 7")
+    await asyncio.sleep(1)
+    print("end 7")
+
+async def test_http_call_8():
+    print("start 8")
+    await asyncio.sleep(1)
+    print("end 8")
```

### Comparing `asytest-0.1.3/pyproject.toml` & `asytest-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asytest-0.1.3/src/asytest/asytest.py` & `asytest-0.1.4/src/asytest/asytest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 from enum import Enum
 from functools import wraps
 import os
 import time
 import asyncio
 from importlib.util import spec_from_file_location, module_from_spec
 import inspect
@@ -44,14 +45,15 @@
         raise ValueError(f"Test function {func_name} is not async")
 
 class TestStatus(Enum):
     SUCCESS = "SUCCESS"
     ERROR = "ERROR"
     FAILED = "FAILED"
 
+
 class TestResult:
     """
     A class representing the result of a test.
     """
     def __init__(self, 
                  exec_time: int, 
                  name: str, 
@@ -60,19 +62,43 @@
                  error: Optional[BaseException] = None):
         self.exec_time = exec_time
         self.module = module
         self.name = name
         self.status = status
         self.error = error
 
-
     def __repr__(self):
         return f"TestResult(execution_time={self.exec_time}, name='{self.name}', status={self.status})"
 
 
+class TestSuiteResult:
+    """
+    A class representing the result of running a test set.
+    """
+    def __init__(self, test_results: List[TestResult], exec_time: int) -> None:
+        self.test_results = test_results
+        self.exec_time = exec_time
+
+    def get_total_tests(self):
+        return len(self.test_results)
+    
+    def count_num_passed(self):
+        return sum(1 for r in self.test_results if r.status == TestStatus.SUCCESS)
+
+    def count_num_failed(self):
+        return sum(1 for r in self.test_results if r.status in [TestStatus.FAILED, TestStatus.ERROR])
+
+    def __repr__(self):
+        return (
+            f"TestSuiteResult(execution_time={self.exec_time}, "
+            f"failed={self.count_num_failed()}, "
+            f"success={self.count_num_passed()})"
+        )
+
+
 def wrap_test_func(file_location, func_name, test_func):
 
     @wraps(test_func)
     async def test_func_wrapper(*args, **kwargs):
         start = time.time()
         try:
             await test_func(*args, **kwargs)
@@ -101,29 +127,28 @@
         name = result.name
         module = result.module
         status = result.status.value
         color = "\033[92m" if status == "SUCCESS" else "\033[91m"
         print(f"{module}::{name} {color}{status:<10}\033[0m [{exec_time_formatted}s]")
     print()
 
-def print_summary(results: List[TestResult], total_exec_time) -> None:
+def print_summary(result: TestSuiteResult) -> None:
     """
-    Prints a summary of the test results to stdout.
+    Prints a summary of the test suite result to stdout.
 
     Args:
-        results: List of TestResult objects.
+        result: TestSuiteResult objects.
     """
-    num_tests = len(results)
-    num_passed = sum(1 for r in results if r.status == TestStatus.SUCCESS)
-    num_failed = num_tests - num_passed
-    total_time_formatted = str(timedelta(seconds=round(total_exec_time)))
+    total_time_formatted = str(timedelta(seconds=round(result.exec_time)))
     status_line = " "
+    num_failed = result.count_num_failed()
+    num_passed = result.count_num_passed()
     if num_failed > 0:
         status_line += f"\033[31m{num_failed} failed\033[0m, "
-    status_line += f"\033[32m{num_passed} passed\033[0m in {total_exec_time:.1f}s ({total_time_formatted}) "
+    status_line += f"\033[32m{num_passed} passed\033[0m in {result.exec_time:.1f}s ({total_time_formatted}) "
     print(format_line(" SUMMARY "))
     print(status_line)
 
 def print_errors(test_results: List[TestResult]) -> None:
     """
     Print the errors for a list of test results.
     """
@@ -141,24 +166,52 @@
     else:
         padding = line_size - len(line)
         left_padding = padding // 2
         right_padding = padding - left_padding
         return f"{'='*left_padding}{line}{'='*right_padding}"
 
 def load_test_functions(module: ModuleType) -> List[Callable[..., Any]]:
-            # Get all functions from the module
+        # Get all functions from the module
         module_functions = inspect.getmembers(module, inspect.isfunction)
         # Filter the functions to only include those that start with "test_"
         test_functions = [func for func in module_functions if func[0].startswith("test_")]
         for func_name, func in test_functions:
             validate_function_async(func_name, func)
         return test_functions
 
-async def run_tests_async(tests_path: str) -> List[TestResult]:
-    print(f"Runnint tests for {tests_path}")
+async def run_tests_concurrently(test_functions, max_concurrent) -> List[TestResult]:
+    results = []
+    tasks = []
+
+    # Start running coroutines
+    for tf in test_functions:
+        # Add new coroutine to the tasks list
+        tasks.append(asyncio.create_task(tf()))
+        # Check if the maximum number of concurrent coroutines has been reached
+        if len(tasks) == max_concurrent:
+            # Wait for any of the current coroutines to finish
+            done, _ = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+            # Collect the results from the finished coroutines
+            for finished_task in done:
+                result = await finished_task
+                results.append(result)
+            # Remove the finished tasks from the tasks list
+            tasks = [t for t in tasks if not t.done()]
+
+    # Wait for all remaining coroutines to finish
+    done, _ = await asyncio.wait(tasks) if tasks else ([],[])
+    for finished_task in done:
+        result = await finished_task
+        results.append(result)
+
+    return results
+
+
+async def run_tests_async(tests_path: str, max_concurrent: int) -> TestSuiteResult:
+    print(f"Runnint tests for {tests_path} with {max_concurrent} max concurrent tests.")
 
     all_test_functions = []
     for file_location in get_python_files(tests_path):
         module = load_script_from_location(file_location)
         test_functions = load_test_functions(module)
         # Call each test function
         for func_name, func in test_functions:
@@ -166,16 +219,34 @@
             all_test_functions.append(wrap_test_func(
                 file_location=file_location, 
                 func_name=func_name, 
                 test_func=func
             ))
 
     start = time.time()
-    test_results = await asyncio.gather(*[tf() for tf in all_test_functions])
-    exec_time = time.time() - start
+    test_results = await run_tests_concurrently(all_test_functions, max_concurrent)
+    test_suite_result = TestSuiteResult(test_results, time.time() - start)
     print_test_results(test_results)
     print_errors(test_results)
-    print_summary(results=test_results, total_exec_time=exec_time)
-    return test_results
+    print_summary(test_suite_result)
+    return test_suite_result
+
+def run_tests(tests_path: str, max_concurrent: int) -> TestSuiteResult:
+    return asyncio.run(run_tests_async(tests_path, max_concurrent))
 
-def run_tests(tests_path: str) -> List[TestResult]:
-    return asyncio.run(run_tests_async(tests_path))
+def parse_args():
+    """Parse the command-line arguments."""
+    parser = argparse.ArgumentParser(
+        description="Run tests in parallel using asyncio"
+    )
+    parser.add_argument(
+        "resource", 
+        help="Path to the test resource. Can be a file or a folder."
+    )
+    parser.add_argument(
+        "-n",
+        "--max-concurrent",
+        type=int,
+        default=10,
+        help="Maximum number of tests to run concurrently",
+    )
+    return parser.parse_args()
```

### Comparing `asytest-0.1.3/src/asytest.egg-info/PKG-INFO` & `asytest-0.1.4/src/asytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asytest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tiny async test framework for python 
 Author: Pavel Rabetski
 Project-URL: Homepage, https://github.com/pavradev/asytest
 Project-URL: Bug Tracker, https://github.com/pavradev/asytest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

