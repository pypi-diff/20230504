# Comparing `tmp/david-test-datadog-sma-0.0.9.tar.gz` & `tmp/david-test-datadog-sma-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-test-datadog-sma-0.0.9.tar", last modified: Thu May  4 21:41:36 2023, max compression
+gzip compressed data, was "david-test-datadog-sma-0.1.0.tar", last modified: Thu May  4 21:43:27 2023, max compression
```

## Comparing `david-test-datadog-sma-0.0.9.tar` & `david-test-datadog-sma-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:36.875063 david-test-datadog-sma-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:41:36.875063 david-test-datadog-sma-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 21:41:27.000000 david-test-datadog-sma-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:41:36.875063 david-test-datadog-sma-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:36.871063 david-test-datadog-sma-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:18.000000 david-test-datadog-sma-0.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:36.871063 david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-linux-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   980596 2023-05-04 21:41:27.000000 david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:36.871063 david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-windows-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-04 21:41:27.000000 david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:36.875063 david-test-datadog-sma-0.0.9/src/david_test_datadog_sma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:41:36.000000 david-test-datadog-sma-0.0.9/src/david_test_datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 21:41:36.000000 david-test-datadog-sma-0.0.9/src/david_test_datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:41:36.000000 david-test-datadog-sma-0.0.9/src/david_test_datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 21:41:36.000000 david-test-datadog-sma-0.0.9/src/david_test_datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:27.690630 david-test-datadog-sma-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:43:27.690630 david-test-datadog-sma-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 21:43:19.000000 david-test-datadog-sma-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:43:27.690630 david-test-datadog-sma-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:27.686630 david-test-datadog-sma-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:05.000000 david-test-datadog-sma-0.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:27.686630 david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-linux-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   980596 2023-05-04 21:43:19.000000 david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:27.690630 david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-windows-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-04 21:43:19.000000 david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:27.690630 david-test-datadog-sma-0.1.0/src/david_test_datadog_sma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:43:27.000000 david-test-datadog-sma-0.1.0/src/david_test_datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 21:43:27.000000 david-test-datadog-sma-0.1.0/src/david_test_datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:43:27.000000 david-test-datadog-sma-0.1.0/src/david_test_datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 21:43:27.000000 david-test-datadog-sma-0.1.0/src/david_test_datadog_sma.egg-info/top_level.txt
```

### Comparing `david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent` & `david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent`

 * *Files identical despite different names*

### Comparing `david-test-datadog-sma-0.0.9/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe` & `david-test-datadog-sma-0.1.0/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe`

 * *Files identical despite different names*

