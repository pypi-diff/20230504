# Comparing `tmp/david-test-datadog-sma-0.0.6.tar.gz` & `tmp/david-test-datadog-sma-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-test-datadog-sma-0.0.6.tar", last modified: Thu May  4 21:31:58 2023, max compression
+gzip compressed data, was "david-test-datadog-sma-0.0.7.tar", last modified: Thu May  4 21:38:07 2023, max compression
```

## Comparing `david-test-datadog-sma-0.0.6.tar` & `david-test-datadog-sma-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:58.183940 david-test-datadog-sma-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:31:58.183940 david-test-datadog-sma-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 21:31:46.000000 david-test-datadog-sma-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:31:58.183940 david-test-datadog-sma-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:58.175940 david-test-datadog-sma-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:35.000000 david-test-datadog-sma-0.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:58.179940 david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-linux-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   980596 2023-05-04 21:31:46.000000 david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:58.179940 david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-windows-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-04 21:31:46.000000 david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:31:58.183940 david-test-datadog-sma-0.0.6/src/david_test_datadog_sma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:31:58.000000 david-test-datadog-sma-0.0.6/src/david_test_datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 21:31:58.000000 david-test-datadog-sma-0.0.6/src/david_test_datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:31:58.000000 david-test-datadog-sma-0.0.6/src/david_test_datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 21:31:58.000000 david-test-datadog-sma-0.0.6/src/david_test_datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:38:07.544681 david-test-datadog-sma-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:38:07.544681 david-test-datadog-sma-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 21:37:58.000000 david-test-datadog-sma-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:38:07.544681 david-test-datadog-sma-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:38:07.540681 david-test-datadog-sma-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:37:48.000000 david-test-datadog-sma-0.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:38:07.540681 david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-linux-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   980596 2023-05-04 21:37:58.000000 david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:38:07.540681 david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-windows-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-04 21:37:58.000000 david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:38:07.544681 david-test-datadog-sma-0.0.7/src/david_test_datadog_sma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:38:07.000000 david-test-datadog-sma-0.0.7/src/david_test_datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 21:38:07.000000 david-test-datadog-sma-0.0.7/src/david_test_datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:38:07.000000 david-test-datadog-sma-0.0.7/src/david_test_datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 21:38:07.000000 david-test-datadog-sma-0.0.7/src/david_test_datadog_sma.egg-info/top_level.txt
```

### Comparing `david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent` & `david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent`

 * *Files identical despite different names*

### Comparing `david-test-datadog-sma-0.0.6/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe` & `david-test-datadog-sma-0.0.7/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe`

 * *Files identical despite different names*

