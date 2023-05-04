# Comparing `tmp/cc1101-2.7.3rc0.tar.gz` & `tmp/cc1101-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc1101-2.7.3rc0.tar", last modified: Tue Apr 20 14:49:23 2021, max compression
+gzip compressed data, was "cc1101-3.0.0.tar", last modified: Thu May  4 07:37:06 2023, max compression
```

## Comparing `cc1101-2.7.3rc0.tar` & `cc1101-3.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.062183 cc1101-2.7.3rc0/.github/
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      550 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/.github/dependabot.yml
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.062183 cc1101-2.7.3rc0/.github/workflows/
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2619 2021-04-20 12:36:19.000000 cc1101-2.7.3rc0/.github/workflows/python.yml
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)       56 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/.gitignore
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      171 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/.pylintrc
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     4849 2021-04-20 14:08:14.000000 cc1101-2.7.3rc0/CHANGELOG.md
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)    35149 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/COPYING
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     5014 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/PKG-INFO
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2004 2021-04-20 12:36:19.000000 cc1101-2.7.3rc0/Pipfile
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)    24107 2021-04-20 12:36:19.000000 cc1101-2.7.3rc0/Pipfile.lock
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3237 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/README.md
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.062183 cc1101-2.7.3rc0/cc1101/
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)    38800 2021-04-20 14:44:02.000000 cc1101-2.7.3rc0/cc1101/__init__.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     6141 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/cc1101/_cli.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2474 2021-04-20 14:13:32.000000 cc1101-2.7.3rc0/cc1101/_gpio.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3837 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/cc1101/addresses.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1951 2021-04-20 14:38:08.000000 cc1101-2.7.3rc0/cc1101/options.py
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/cc1101.egg-info/
--rw-r--r--   0 fabianpeter  (1000) fabianpeter  (1000)     5014 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/PKG-INFO
--rw-r--r--   0 fabianpeter  (1000) fabianpeter  (1000)     1152 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/SOURCES.txt
--rw-r--r--   0 fabianpeter  (1000) fabianpeter  (1000)        1 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/dependency_links.txt
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      109 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/entry_points.txt
--rw-r--r--   0 fabianpeter  (1000) fabianpeter  (1000)       13 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/requires.txt
--rw-r--r--   0 fabianpeter  (1000) fabianpeter  (1000)        7 2021-04-20 14:49:22.000000 cc1101-2.7.3rc0/cc1101.egg-info/top_level.txt
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/examples/
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      768 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/examples/asynchronous_gpio_transmit.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      253 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/examples/show_config.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      565 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/examples/transmit_fixed_length.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1454 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/examples/transmit_variable_length.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)       37 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/mypy.ini
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)       38 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/setup.cfg
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2786 2021-04-20 12:36:19.000000 cc1101-2.7.3rc0/setup.py
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/tests/
-drwxr-s---   0 fabianpeter  (1000) fabianpeter  (1000)        0 2021-04-20 14:49:23.066183 cc1101-2.7.3rc0/tests/config/
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      199 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/__init__.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1656 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x04_0x05_sync1_sync0.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1633 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x06_pktlen.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3318 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x08_pktctrl0.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3443 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x10_mdmcfg4.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1504 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x11_mdmcfg3.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     5372 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x12_mdmcfg2.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2658 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x13_mdmcfg1.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2343 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x22_frend0.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1994 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/config/test_0x3e_patable.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      166 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/conftest.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     5221 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_cli_export_config.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     7610 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_cli_transmit.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     6984 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_config.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     4325 2021-04-20 14:14:35.000000 cc1101-2.7.3rc0/tests/test_gpio.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     6445 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_lock.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3738 2021-04-20 14:49:03.000000 cc1101-2.7.3rc0/tests/test_receive.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)      784 2021-04-20 14:44:02.000000 cc1101-2.7.3rc0/tests/test_received_packet.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     7175 2021-04-20 14:11:18.000000 cc1101-2.7.3rc0/tests/test_spi.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     1438 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_state.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     2139 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_str.py
--rw-r-----   0 fabianpeter  (1000) fabianpeter  (1000)     3869 2021-02-26 13:05:50.000000 cc1101-2.7.3rc0/tests/test_transmit.py
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/.github/
+-rw-r-----   0 persona   (1000) persona   (1000)      720 2022-06-17 15:36:31.000000 cc1101-3.0.0/.github/dependabot.yml
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/.github/workflows/
+-rw-r-----   0 persona   (1000) persona   (1000)     2587 2023-04-29 08:07:14.000000 cc1101-3.0.0/.github/workflows/python.yml
+-rw-r-----   0 persona   (1000) persona   (1000)       56 2022-06-17 15:36:31.000000 cc1101-3.0.0/.gitignore
+-rw-r-----   0 persona   (1000) persona   (1000)     1025 2022-06-17 15:36:31.000000 cc1101-3.0.0/.pylintrc
+-rw-r-----   0 persona   (1000) persona   (1000)     5463 2023-05-04 07:31:55.000000 cc1101-3.0.0/CHANGELOG.md
+-rw-r-----   0 persona   (1000) persona   (1000)    35149 2022-06-17 15:36:31.000000 cc1101-3.0.0/COPYING
+-rw-r-----   0 persona   (1000) persona   (1000)     5031 2023-05-04 07:37:06.870005 cc1101-3.0.0/PKG-INFO
+-rw-r-----   0 persona   (1000) persona   (1000)     2135 2023-02-03 10:27:47.000000 cc1101-3.0.0/Pipfile
+-rw-r-----   0 persona   (1000) persona   (1000)    39446 2023-05-04 07:26:56.000000 cc1101-3.0.0/Pipfile.lock
+-rw-r-----   0 persona   (1000) persona   (1000)     3237 2023-04-29 07:52:26.000000 cc1101-3.0.0/README.md
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/cc1101/
+-rw-r-----   0 persona   (1000) persona   (1000)    38139 2023-05-04 07:27:05.000000 cc1101-3.0.0/cc1101/__init__.py
+-rw-r-----   0 persona   (1000) persona   (1000)     6118 2022-06-17 15:36:31.000000 cc1101-3.0.0/cc1101/_cli.py
+-rw-r-----   0 persona   (1000) persona   (1000)     4842 2022-06-17 15:36:31.000000 cc1101-3.0.0/cc1101/_gpio.py
+-rw-r-----   0 persona   (1000) persona   (1000)     3837 2022-06-17 15:36:31.000000 cc1101-3.0.0/cc1101/addresses.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1951 2022-06-17 15:36:31.000000 cc1101-3.0.0/cc1101/options.py
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/cc1101.egg-info/
+-rw-r--r--   0 persona   (1000) persona   (1000)     5031 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/PKG-INFO
+-rw-r--r--   0 persona   (1000) persona   (1000)     1152 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/SOURCES.txt
+-rw-r--r--   0 persona   (1000) persona   (1000)        1 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/dependency_links.txt
+-rw-r--r--   0 persona   (1000) persona   (1000)      109 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/entry_points.txt
+-rw-r--r--   0 persona   (1000) persona   (1000)        7 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/requires.txt
+-rw-r--r--   0 persona   (1000) persona   (1000)        7 2023-05-04 07:37:06.000000 cc1101-3.0.0/cc1101.egg-info/top_level.txt
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/examples/
+-rw-r-----   0 persona   (1000) persona   (1000)      768 2022-06-17 15:36:31.000000 cc1101-3.0.0/examples/asynchronous_gpio_transmit.py
+-rw-r-----   0 persona   (1000) persona   (1000)      253 2022-06-17 15:36:31.000000 cc1101-3.0.0/examples/show_config.py
+-rw-r-----   0 persona   (1000) persona   (1000)      565 2022-06-17 15:36:31.000000 cc1101-3.0.0/examples/transmit_fixed_length.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1454 2022-06-17 15:36:31.000000 cc1101-3.0.0/examples/transmit_variable_length.py
+-rw-r-----   0 persona   (1000) persona   (1000)       37 2022-06-17 15:36:31.000000 cc1101-3.0.0/mypy.ini
+-rw-r-----   0 persona   (1000) persona   (1000)       38 2023-05-04 07:37:06.870005 cc1101-3.0.0/setup.cfg
+-rw-r-----   0 persona   (1000) persona   (1000)     2777 2022-12-19 08:12:50.000000 cc1101-3.0.0/setup.py
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/tests/
+drwxr-x---   0 persona   (1000) persona   (1000)        0 2023-05-04 07:37:06.870005 cc1101-3.0.0/tests/config/
+-rw-r-----   0 persona   (1000) persona   (1000)      199 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/__init__.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1656 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x04_0x05_sync1_sync0.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1633 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x06_pktlen.py
+-rw-r-----   0 persona   (1000) persona   (1000)     3318 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x08_pktctrl0.py
+-rw-r-----   0 persona   (1000) persona   (1000)     3443 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x10_mdmcfg4.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1504 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x11_mdmcfg3.py
+-rw-r-----   0 persona   (1000) persona   (1000)     5372 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x12_mdmcfg2.py
+-rw-r-----   0 persona   (1000) persona   (1000)     2658 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x13_mdmcfg1.py
+-rw-r-----   0 persona   (1000) persona   (1000)     2343 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x22_frend0.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1994 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/config/test_0x3e_patable.py
+-rw-r-----   0 persona   (1000) persona   (1000)      377 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/conftest.py
+-rw-r-----   0 persona   (1000) persona   (1000)     5354 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_cli_export_config.py
+-rw-r-----   0 persona   (1000) persona   (1000)     7595 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_cli_transmit.py
+-rw-r-----   0 persona   (1000) persona   (1000)     6982 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_config.py
+-rw-r-----   0 persona   (1000) persona   (1000)     4762 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_gpio.py
+-rw-r-----   0 persona   (1000) persona   (1000)     6435 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_lock.py
+-rw-r-----   0 persona   (1000) persona   (1000)     3459 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_receive.py
+-rw-r-----   0 persona   (1000) persona   (1000)      784 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_received_packet.py
+-rw-r-----   0 persona   (1000) persona   (1000)     7840 2023-05-04 07:27:05.000000 cc1101-3.0.0/tests/test_spi.py
+-rw-r-----   0 persona   (1000) persona   (1000)     1438 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_state.py
+-rw-r-----   0 persona   (1000) persona   (1000)     2139 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_str.py
+-rw-r-----   0 persona   (1000) persona   (1000)     3904 2022-06-17 15:36:31.000000 cc1101-3.0.0/tests/test_transmit.py
```

### Comparing `cc1101-2.7.3rc0/.github/dependabot.yml` & `cc1101-3.0.0/.github/dependabot.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 version: 2
 
 updates:
 - # > Dependabot also supports the following package managers: [...]
   # > - pipenv, pip-compile, and poetry (specify pip)
   package-ecosystem: pip
   directory: /
-  # avoid changes in Pipfile breaking python3.5 compatibility
+  # avoid changes in Pipfile breaking constraints for compatibility with older python versions
   versioning-strategy: lockfile-only
   schedule:
     interval: weekly
     day: friday
+- package-ecosystem: github-actions
+  directory: /
+  # > YAML aliases are not supported
+  schedule:
+    interval: weekly
+    day: friday
 
 # https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/configuration-options-for-dependency-updates
```

### Comparing `cc1101-2.7.3rc0/.github/workflows/python.yml` & `cc1101-3.0.0/.github/workflows/python.yml`

 * *Files 26% similar despite different names*

```diff
@@ -10,63 +10,68 @@
   push:
   pull_request:
   schedule:
   - cron: '0 20 * * 5'
 
 jobs:
   code-format:
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version:
-        - 3.8
+        python-version: ['3.9']
     steps:
-    - uses: actions/checkout@v1
-    - uses: actions/setup-python@v1
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - run: pip install --upgrade pipenv==2020.8.13
     - run: pipenv install --python "$PYTHON_VERSION" --deploy --dev
       env:
         PYTHON_VERSION: ${{ matrix.python-version }}
     - run: pipenv graph
     - run: pipenv run black --check .
   tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version:
-        - 3.5
-        - 3.6
-        - 3.7
-        - 3.8
-        - 3.9
+        - '3.7'
+        - '3.8'
+        - '3.9'
+        - '3.10'
+        - '3.11'
       fail-fast: false
     steps:
-    - uses: actions/checkout@v1
-    - uses: actions/setup-python@v1
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    - run: sudo apt-get update
-    # https://github.com/hhk7734/python3-gpiod/blob/v1.2.1/py_src/gpiod/libgpiod/__init__.py#L54
-    - run: sudo apt-get install --yes --no-install-recommends libgpiod2
     - run: pip install --upgrade pipenv==2020.8.13
+    # by default pipenv picks the latest version in PATH
     - run: pipenv install --python "$PYTHON_VERSION" --deploy --dev
       env:
         PYTHON_VERSION: ${{ matrix.python-version }}
     - run: pipenv graph
     - run: pipenv run pytest --cov="$(cat *.egg-info/top_level.txt)" --cov-report=term-missing --cov-fail-under=94
-    # https://github.com/PyCQA/pylint/issues/3882
-    - run: python3 -c 'import sys; sys.exit(sys.version_info < (3, 9))'
-        || pipenv run pylint --load-plugins=pylint_import_requirements "$(cat *.egg-info/top_level.txt)"
+    - run: pipenv run pylint --load-plugins=pylint_import_requirements "$(cat *.egg-info/top_level.txt)"
     # https://github.com/PyCQA/pylint/issues/352
     - run: pipenv run pylint tests/*
     - run: pipenv run mypy "$(cat *.egg-info/top_level.txt)" tests
-    # >=2.1.0 to support GITHUB_TOKEN
-    # COVERALLS_REPO_TOKEN required manual configuration of secret
-    # https://github.com/TheKevJames/coveralls-python/commit/f597109b62fadaf900af79d4f08a7debee5229e2
-    - run: pip install 'coveralls>=2.1.0,<4'
-    - run: coveralls
+    - uses: coverallsapp/github-action@v2
+  check-links:
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        python-version: ['3.9']
+    steps:
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: ${{ matrix.python-version }}
+    - run: pip install --upgrade pipenv==2020.8.13
+    - run: pipenv install --python "$PYTHON_VERSION" --deploy --dev
       env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        # https://github.com/TheKevJames/coveralls-python/issues/240#issuecomment-758336355
-        COVERALLS_SERVICE_NAME: github
+        PYTHON_VERSION: ${{ matrix.python-version }}
+    - run: pipenv graph
+    # `--include '*.md'` fails for https://securipi.co.uk/cc1101.pdf (HTTP403).
+    # `--include '*.py'` identifies `logging.INFO` as an url.
+    - run: pipenv run blinkcheck --include CHANGELOG.md
```

### Comparing `cc1101-2.7.3rc0/CHANGELOG.md` & `cc1101-3.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+
+## [3.0.0] - 2023-05-04
+### Added
+- declare compatibility with `python3.11`
+- allow parametrization of `spi_max_speed_hz` during `C1101` class instantiation
+  to solve [issue-128]
+
+### Changed
+- `CC1101.transmit`: raise `RuntimeError` instead of `Exception` when
+  attempting to transmit in non-idle state
+
+### Removed
+- compatibility with `python3.5` & `python3.6`
+
+## [2.7.3] - 2021-04-20
 ### Fixed
 - change `IOCFG0.GDO0_CFG` as recommended in docs to "optimize RF performance"
 
 ## [2.7.2] - 2021-03-12
 ### Fixed
 - recommend to check wiring & bus selection when receiving chip version `0`
 
@@ -102,22 +117,25 @@
   - `get_configuration_register_values()` to read all configuration registers
 - OOK modulation
 - configurable symbol rate & sync mode
 - optional manchester encoding
 - disabled data whitening
 - automatic calibration
 
-[Unreleased]: https://github.com/fphammerle/python-cc1101/compare/v2.7.2...HEAD
+[Unreleased]: https://github.com/fphammerle/python-cc1101/compare/v3.0.0...HEAD
+[3.0.0]: https://github.com/fphammerle/python-cc1101/compare/v2.7.3...v3.0.0
+[2.7.3]: https://github.com/fphammerle/python-cc1101/compare/v2.7.2...v2.7.3
 [2.7.2]: https://github.com/fphammerle/python-cc1101/compare/v2.7.1...v2.7.2
 [2.7.1]: https://github.com/fphammerle/python-cc1101/compare/v2.7.0...v2.7.1
 [2.7.0]: https://github.com/fphammerle/python-cc1101/compare/v2.6.1...v2.7.0
 [2.6.1]: https://github.com/fphammerle/python-cc1101/compare/v2.6.0...v2.6.1
 [2.6.0]: https://github.com/fphammerle/python-cc1101/compare/v2.5.0...v2.6.0
 [2.5.0]: https://github.com/fphammerle/python-cc1101/compare/v2.4.0...v2.5.0
 [2.4.0]: https://github.com/fphammerle/python-cc1101/compare/v2.3.0...v2.4.0
 [2.3.0]: https://github.com/fphammerle/python-cc1101/compare/v2.2.0...v2.3.0
 [2.2.0]: https://github.com/fphammerle/python-cc1101/compare/v2.1.0...v2.2.0
 [2.1.0]: https://github.com/fphammerle/python-cc1101/compare/v2.0.0...v2.1.0
 [2.0.0]: https://github.com/fphammerle/python-cc1101/compare/v1.2.0...v2.0.0
 [1.2.0]: https://github.com/fphammerle/python-cc1101/compare/v1.1.0...v1.2.0
 [1.1.0]: https://github.com/fphammerle/python-cc1101/compare/v1.0.0...v1.1.0
 [1.0.0]: https://github.com/fphammerle/python-cc1101/releases/tag/v1.0.0
+[issue-128]: https://github.com/fphammerle/python-cc1101/issues/128
```

### Comparing `cc1101-2.7.3rc0/COPYING` & `cc1101-3.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/PKG-INFO` & `cc1101-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc1101
-Version: 2.7.3rc0
+Version: 3.0.0
 Summary: Python Library & Command Line Tool to Transmit RF Signals via C1101 Transceivers
 Home-page: https://github.com/fphammerle/python-cc1101
 Author: Fabian Peter Hammerle
 Author-email: fabian+python-cc1101@hammerle.me
 License: GPLv3+
 Project-URL: Changelog, https://github.com/fphammerle/python-cc1101/blob/master/CHANGELOG.md
 Description: # python-cc1101
@@ -91,19 +91,20 @@
         followed by a re-login.
         
         Consult CC1101's offical docs for an in-depth explanation of all options:
         https://www.ti.com/lit/ds/symlink/cc1101.pdf
         
 Keywords: ISM,SPI,automation,radio-frequency,raspberry-pi,transceiver,transmission,wireless
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Communications
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cc1101-2.7.3rc0/README.md` & `cc1101-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/cc1101/__init__.py` & `cc1101-3.0.0/cc1101/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,42 +11,43 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import contextlib
 import datetime
 import enum
 import fcntl
 import logging
 import math
 import typing
 import warnings
 
 import spidev
 
 import cc1101._gpio
 from cc1101.addresses import (
-    StrobeAddress,
     ConfigurationRegisterAddress,
-    StatusRegisterAddress,
-    PatableAddress,
     FIFORegisterAddress,
+    PatableAddress,
+    StatusRegisterAddress,
+    StrobeAddress,
 )
 from cc1101.options import (
     GDOSignalSelection,
     ModulationFormat,
     PacketLengthMode,
     SyncMode,
     _TransceiveMode,
 )
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class Pin(enum.Enum):
     GDO0 = "GDO0"
 
 
@@ -64,21 +65,20 @@
     RX = 0x0D
     RXFIFO_OVERFLOW = 0x11
     TX = 0x13
     # TXFIFO_UNDERFLOW = 0x16
 
 
 class _ReceivedPacket:  # unstable
-
     # "Table 31: Typical RSSI_offset Values"
     _RSSI_OFFSET_dB = 74
 
     def __init__(
         self,
-        # *,
+        *,
         payload: bytes,
         rssi_index: int,  # byte
         checksum_valid: bool,
         link_quality_indicator: int,  # 7bit
     ):
         self.payload = payload
         self._rssi_index = rssi_index
@@ -95,31 +95,28 @@
         see section "17.3 RSSI"
         """
         if self._rssi_index >= 128:
             return (self._rssi_index - 256) / 2 - self._RSSI_OFFSET_dB
         return self._rssi_index / 2 - self._RSSI_OFFSET_dB
 
     def __str__(self) -> str:
-        return "{}(RSSI {:.0f}dBm, 0x{})".format(
-            type(self).__name__, self.rssi_dbm, self.payload.hex()
-        )
+        return f"{type(self).__name__}(RSSI {self.rssi_dbm:.0f}dBm, 0x{self.payload.hex()})"
 
 
 def _format_patable(settings: typing.Iterable[int], insert_spaces: bool) -> str:
     # "Table 39: Optimum PATABLE Settings" uses hexadecimal digits
     # "0" for brevity
-    settings_hex = tuple(map(lambda s: "0" if s == 0 else "0x{:x}".format(s), settings))
+    settings_hex = tuple(map(lambda s: "0" if s == 0 else f"0x{s:x}", settings))
     if len(settings_hex) == 1:
-        return "({},)".format(settings_hex[0])
+        return f"({settings_hex[0]},)"
     delimiter = ", " if insert_spaces else ","
-    return "({})".format(delimiter.join(settings_hex))
+    return f"({delimiter.join(settings_hex)})"
 
 
 class CC1101:
-
     # pylint: disable=too-many-public-methods
 
     # > All transfers on the SPI interface are done
     # > most significant bit first.
     # > All transactions on the SPI interface start with
     # > a header byte containing a R/W bit, a access bit (B),
     # > and a 6-bit address (A5 - A0).
@@ -144,26 +141,30 @@
         0x04,  #  https://github.com/fphammerle/python-cc1101/issues/15
         0x14,
     ]
 
     _CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ = 26e6
     # see "21 Frequency Programming"
     # > f_carrier = f_XOSC / 2**16 * (FREQ + CHAN * ((256 + CHANSPC_M) * 2**CHANSPC_E-2))
-    _FREQUENCY_CONTROL_WORD_HERTZ_FACTOR = _CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ / 2 ** 16
+    _FREQUENCY_CONTROL_WORD_HERTZ_FACTOR = _CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ / 2**16
 
     # roughly estimated / tested with SDR receiver, docs specify:
     # > can [...] be programmed for operation at other frequencies
     # > in the 300-348 MHz, 387-464 MHz and 779-928 MHz bands.
     _TRANSMIT_MIN_FREQUENCY_HERTZ = 281.7e6
 
     # > The PATABLE is an 8-byte table that defines the PA control settings [...]
     _PATABLE_LENGTH_BYTES = 8
 
     def __init__(
-        self, spi_bus: int = 0, spi_chip_select: int = 0, lock_spi_device: bool = False
+        self,
+        spi_bus: int = 0,
+        spi_chip_select: int = 0,
+        lock_spi_device: bool = False,
+        spi_max_speed_hz: int = 55700,
     ) -> None:
         """
         lock_spi_device:
             When True, an advisory, exclusive lock will be set on the SPI device file
             non-blockingly via flock upon entering the context.
             If the SPI device file is already locked (e.g., by a different process),
             a BlockingIOError will be raised.
@@ -176,28 +177,29 @@
             >>> # lock removed
             >>> with transceiver:
             >>>     # locked
             >>>     transceiver.unlock_spi_device()
             >>>     # lock removed
         """
         self._spi = spidev.SpiDev()
+        self._spi_max_speed_hz = spi_max_speed_hz
         self._spi_bus = int(spi_bus)
         # > The BCM2835 core common to all Raspberry Pi devices has 3 SPI Controllers:
         # > SPI0, with two hardware chip selects, [...]
         # > SPI1, with three hardware chip selects, [...]
         # > SPI2, also with three hardware chip selects, is only usable on a Compute Module [...]
         # https://github.com/raspberrypi/documentation/blob/d41d69f8efa3667b1a8b01a669238b8bd113edc1/hardware/raspberrypi/spi/README.md#hardware
         # https://www.raspberrypi.org/documentation/hardware/raspberrypi/spi/README.md
         self._spi_chip_select = int(spi_chip_select)
         self._lock_spi_device = lock_spi_device
 
     @property
     def _spi_device_path(self) -> str:
         # https://github.com/doceme/py-spidev/blob/v3.4/spidev_module.c#L1286
-        return "/dev/spidev{}.{}".format(self._spi_bus, self._spi_chip_select)
+        return f"/dev/spidev{self._spi_bus}.{self._spi_chip_select}"
 
     @staticmethod
     def _log_chip_status_byte(chip_status: int) -> None:
         # see "10.1 Chip Status Byte" & "Table 23: Status Byte Summary"
         # > The command strobe registers are accessed by transferring
         # > a single header byte [...]. That is, only the R/W̄ bit,
         # > the burst access bit (set to 0), and the six address bits [...]
@@ -268,21 +270,21 @@
         assert all(v == response[0] for v in response[1:]), response
 
     def _reset(self) -> None:
         self._command_strobe(StrobeAddress.SRES)
 
     @classmethod
     def _filter_bandwidth_floating_point_to_real(
-        cls, mantissa: int, exponent: int
+        cls, *, mantissa: int, exponent: int
     ) -> float:
         """
         See "13 Receiver Channel Filter Bandwidth"
         """
         return cls._CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ / (
-            8 * (4 + mantissa) * (2 ** exponent)
+            8 * (4 + mantissa) * (2**exponent)
         )
 
     def _get_filter_bandwidth_hertz(self) -> float:
         """
         MDMCFG4.CHANBW_E & MDMCFG4.CHANBW_M
 
         > [...] decimation ratio for the delta-sigma ADC input stream
@@ -332,39 +334,41 @@
 
     def _set_symbol_rate_mantissa(self, mantissa: int) -> None:
         self._write_burst(
             start_register=ConfigurationRegisterAddress.MDMCFG3, values=[mantissa]
         )
 
     @classmethod
-    def _symbol_rate_floating_point_to_real(cls, mantissa: int, exponent: int) -> float:
+    def _symbol_rate_floating_point_to_real(
+        cls, *, mantissa: int, exponent: int
+    ) -> float:
         # see "12 Data Rate Programming"
         return (
             (256 + mantissa)
-            * (2 ** exponent)
+            * (2**exponent)
             * cls._CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ
-            / (2 ** 28)
+            / (2**28)
         )
 
     @classmethod
     def _symbol_rate_real_to_floating_point(cls, real: float) -> typing.Tuple[int, int]:
         # see "12 Data Rate Programming"
         assert real > 0, real
         exponent = math.floor(
             math.log2(real / cls._CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ) + 20
         )
         mantissa = round(
-            real * 2 ** 28 / cls._CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ / 2 ** exponent
+            real * 2**28 / cls._CRYSTAL_OSCILLATOR_FREQUENCY_HERTZ / 2**exponent
             - 256
         )
         if mantissa == 256:
             exponent += 1
             mantissa = 0
-        assert 0 < exponent <= 2 ** 4, exponent
-        assert mantissa <= 2 ** 8, mantissa
+        assert 0 < exponent <= 2**4, exponent
+        assert mantissa <= 2**8, mantissa
         return mantissa, exponent
 
     def get_symbol_rate_baud(self) -> float:
         return self._symbol_rate_floating_point_to_real(
             mantissa=self._get_symbol_rate_mantissa(),
             exponent=self._get_symbol_rate_exponent(),
         )
@@ -400,15 +404,15 @@
         mdmcfg2 = self._read_single_byte(ConfigurationRegisterAddress.MDMCFG2)
         return SyncMode(mdmcfg2 & 0b11)
 
     def set_sync_mode(
         self,
         mode: SyncMode,
         *,
-        _carrier_sense_threshold_enabled: typing.Optional[bool] = None  # unstable
+        _carrier_sense_threshold_enabled: typing.Optional[bool] = None,  # unstable
     ) -> None:
         """
         MDMCFG2.SYNC_MODE
 
         see "14.3 Byte Synchronization"
 
         Carrier Sense (CS) Threshold (when receiving packets, API unstable):
@@ -451,26 +455,26 @@
 
     def set_preamble_length_bytes(self, length: int) -> None:
         """
         see .get_preamble_length_bytes()
         """
         if length < 1:
             raise ValueError(
-                "invalid preamble length {} given".format(length)
-                + "\ncall .set_sync_mode(cc1101.SyncMode.NO_PREAMBLE_AND_SYNC_WORD)"
-                + " to disable preamble"
+                f"invalid preamble length {length} given"
+                "\ncall .set_sync_mode(cc1101.SyncMode.NO_PREAMBLE_AND_SYNC_WORD)"
+                " to disable preamble"
             )
-        if length % 3 == 0:
+        if length % 3 == 0:  # pylint: disable=consider-ternary-expression
             index = math.log2(length / 3) * 2 + 1
         else:
             index = math.log2(length / 2) * 2
         if not index.is_integer() or index < 0 or index > 0b111:
             raise ValueError(
-                "unsupported preamble length: {} bytes".format(length)
-                + "\nsee MDMCFG1.NUM_PREAMBLE in cc1101 docs"
+                f"unsupported preamble length: {length} bytes"
+                "\nsee MDMCFG1.NUM_PREAMBLE in cc1101 docs"
             )
         self._set_preamble_length_index(int(index))
 
     def _get_power_amplifier_setting_index(self) -> int:
         """
         see ._set_power_amplifier_setting_index
         """
@@ -500,24 +504,23 @@
         frend0 |= setting_index
         self._write_burst(ConfigurationRegisterAddress.FREND0, [frend0])
 
     def _verify_chip(self) -> None:
         partnum = self._read_status_register(StatusRegisterAddress.PARTNUM)
         if partnum != self._SUPPORTED_PARTNUM:
             raise ValueError(
-                "unexpected chip part number {} (expected: {})".format(
-                    partnum, self._SUPPORTED_PARTNUM
-                )
+                f"unexpected chip part number {partnum} (expected: {self._SUPPORTED_PARTNUM})"
             )
         version = self._read_status_register(StatusRegisterAddress.VERSION)
         if version not in self._SUPPORTED_VERSIONS:
-            msg = "Unsupported chip version 0x{:02x} (expected one of [{}])".format(
-                version,
-                ", ".join("0x{:02x}".format(v) for v in self._SUPPORTED_VERSIONS),
+            msg = f"Unsupported chip version 0x{version:02x}"
+            supported_versions = ", ".join(
+                f"0x{v:02x}" for v in self._SUPPORTED_VERSIONS
             )
+            msg += f" (expected one of [{supported_versions}])"
             if version == 0:
                 msg += (
                     "\n\nPlease verify that all required pins are connected"
                     " (see https://github.com/fphammerle/python-cc1101#wiring-raspberry-pi)"
                     " and that you selected the correct SPI bus and chip/slave select line."
                 )
             raise ValueError(msg)
@@ -539,40 +542,38 @@
         # > in order to optimize RF performance.
         self._write_burst(
             ConfigurationRegisterAddress.IOCFG0,
             # required for _wait_for_packet()
             [GDOSignalSelection.RX_FIFO_AT_OR_ABOVE_THRESHOLD_OR_PACKET_END_REACHED],
         )
 
-    def __enter__(self) -> "CC1101":
+    def __enter__(self) -> CC1101:
         # https://docs.python.org/3/reference/datamodel.html#object.__enter__
         try:
             self._spi.open(self._spi_bus, self._spi_chip_select)
         except PermissionError as exc:
             raise PermissionError(
-                "Could not access {}".format(self._spi_device_path)
-                + "\nVerify that the current user has both read and write access."
-                + "\nOn some systems, like Raspberry Pi OS / Raspbian,"
-                + "\n\tsudo usermod -a -G spi $USER"
-                + "\nfollowed by a re-login grants sufficient permissions."
+                f"Could not access {self._spi_device_path}"
+                "\nVerify that the current user has both read and write access."
+                "\nOn some systems, like Raspberry Pi OS / Raspbian,"
+                "\n\tsudo usermod -a -G spi $USER"
+                "\nfollowed by a re-login grants sufficient permissions."
             ) from exc
         if self._lock_spi_device:
             # advisory, exclusive, non-blocking
             # lock removed in __exit__ by SpiDev.close()
             fcntl.flock(self._spi.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
         try:
-            self._spi.max_speed_hz = 55700  # empirical
+            self._spi.max_speed_hz = self._spi_max_speed_hz
             self._reset()
             self._verify_chip()
             self._configure_defaults()
             marcstate = self.get_main_radio_control_state_machine_state()
             if marcstate != MainRadioControlStateMachineState.IDLE:
-                raise ValueError(
-                    "expected marcstate idle (actual: {})".format(marcstate.name)
-                )
+                raise ValueError(f"expected marcstate idle (actual: {marcstate.name})")
         except:
             self._spi.close()
             raise
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):  # -> typing.Literal[False]
         # https://docs.python.org/3/reference/datamodel.html#object.__exit__
@@ -651,50 +652,45 @@
         if freq < (self._TRANSMIT_MIN_FREQUENCY_HERTZ - 50e3):
             # > [use] warnings.warn() in library code if the issue is avoidable
             # > and the client application should be modified to eliminate the warning[.]
             # > [use] logging.warning() if there is nothing the client application
             # > can do about the situation, but the event should still be noted.
             # https://docs.python.org/3/howto/logging.html#when-to-use-logging
             warnings.warn(
-                "CC1101 is unable to transmit at frequencies below {:.1f} MHz".format(
-                    self._TRANSMIT_MIN_FREQUENCY_HERTZ / 1e6
-                )
+                "CC1101 is unable to transmit at frequencies"
+                f" below {(self._TRANSMIT_MIN_FREQUENCY_HERTZ / 1e6):.1f} MHz"
             )
         self._set_base_frequency_control_word(
             self._hertz_to_frequency_control_word(freq)
         )
 
     def __str__(self) -> str:
         sync_mode = self.get_sync_mode()
         attrs = (
-            "marcstate={}".format(
-                self.get_main_radio_control_state_machine_state().name.lower()
-            ),
-            "base_frequency={:.2f}MHz".format(
-                self.get_base_frequency_hertz() / 10 ** 6
-            ),
-            "symbol_rate={:.2f}kBaud".format(self.get_symbol_rate_baud() / 1000),
-            "modulation_format={}".format(self.get_modulation_format().name),
-            "sync_mode={}".format(sync_mode.name),
-            "preamble_length={}B".format(self.get_preamble_length_bytes())
+            f"marcstate={self.get_main_radio_control_state_machine_state().name.lower()}",
+            f"base_frequency={(self.get_base_frequency_hertz() / 1e6):.2f}MHz",
+            f"symbol_rate={(self.get_symbol_rate_baud() / 1000):.2f}kBaud",
+            f"modulation_format={self.get_modulation_format().name}",
+            f"sync_mode={sync_mode.name}",
+            f"preamble_length={self.get_preamble_length_bytes()}B"
             if sync_mode != SyncMode.NO_PREAMBLE_AND_SYNC_WORD
             else None,
-            "sync_word=0x{}".format(self.get_sync_word().hex())
+            f"sync_word=0x{self.get_sync_word().hex()}"
             if sync_mode != SyncMode.NO_PREAMBLE_AND_SYNC_WORD
             else None,
-            "packet_length{}{}B".format(
+            "packet_length{}{}B".format(  # pylint: disable=consider-using-f-string
                 "≤"
                 if self.get_packet_length_mode() == PacketLengthMode.VARIABLE
                 else "=",
                 self.get_packet_length_bytes(),
             ),
-            "output_power={}".format(
-                _format_patable(self.get_output_power(), insert_spaces=False)
-            ),
+            "output_power="
+            + _format_patable(self.get_output_power(), insert_spaces=False),
         )
+        # pylint: disable=consider-using-f-string
         return "CC1101({})".format(", ".join(filter(None, attrs)))
 
     def get_configuration_register_values(
         self,
         start_register: ConfigurationRegisterAddress = min(
             ConfigurationRegisterAddress
         ),
@@ -724,15 +720,15 @@
         )
 
     def set_sync_word(self, sync_word: bytes) -> None:
         """
         See .set_sync_word()
         """
         if len(sync_word) != 2:
-            raise ValueError("expected two bytes, got {!r}".format(sync_word))
+            raise ValueError(f"expected two bytes, got {sync_word!r}")
         self._write_burst(
             start_register=ConfigurationRegisterAddress.SYNC1, values=list(sync_word)
         )
 
     def get_packet_length_bytes(self) -> int:
         """
         PKTLEN
@@ -746,17 +742,15 @@
         """
         return self._read_single_byte(ConfigurationRegisterAddress.PKTLEN)
 
     def set_packet_length_bytes(self, packet_length: int) -> None:
         """
         see get_packet_length_bytes()
         """
-        assert 1 <= packet_length <= 255, "unsupported packet length {}".format(
-            packet_length
-        )
+        assert 1 <= packet_length <= 255, f"unsupported packet length {packet_length}"
         self._write_burst(
             start_register=ConfigurationRegisterAddress.PKTLEN, values=[packet_length]
         )
 
     def _disable_data_whitening(self):
         """
         PKTCTRL0.WHITE_DATA
@@ -887,41 +881,35 @@
         # see "15.2 Packet Format"
         # > In variable packet length mode, [...]
         # > The first byte written to the TXFIFO must be different from 0.
         packet_length_mode = self.get_packet_length_mode()
         packet_length = self.get_packet_length_bytes()
         if packet_length_mode == PacketLengthMode.VARIABLE:
             if not payload:
-                raise ValueError("empty payload {!r}".format(payload))
+                raise ValueError(f"empty payload {payload!r}")
             if len(payload) > packet_length:
                 raise ValueError(
-                    "payload exceeds maximum payload length of {} bytes".format(
-                        packet_length
-                    )
-                    + "\nsee .get_packet_length_bytes()"
-                    + "\npayload: {!r}".format(payload)
+                    f"payload exceeds maximum payload length of {packet_length} bytes"
+                    "\nsee .get_packet_length_bytes()"
+                    f"\npayload: {payload!r}"
                 )
             payload = int.to_bytes(len(payload), length=1, byteorder="big") + payload
         elif (
             packet_length_mode == PacketLengthMode.FIXED
             and len(payload) != packet_length
         ):
             raise ValueError(
-                "expected payload length of {} bytes, got {}".format(
-                    packet_length, len(payload)
-                )
+                f"expected payload length of {packet_length} bytes, got {len(payload)}"
                 + "\nsee .set_packet_length_mode() and .get_packet_length_bytes()"
-                + "\npayload: {!r}".format(payload)
+                + f"\npayload: {payload!r}"
             )
         marcstate = self.get_main_radio_control_state_machine_state()
         if marcstate != MainRadioControlStateMachineState.IDLE:
-            raise Exception(
-                "device must be idle before transmission (current marcstate: {})".format(
-                    marcstate.name
-                )
+            raise RuntimeError(
+                f"device must be idle before transmission (current marcstate: {marcstate.name})"
             )
         self._flush_tx_fifo_buffer()
         self._write_burst(FIFORegisterAddress.TX, list(payload))
         _LOGGER.info("transmitting 0x%s (%r)", payload.hex(), payload)
         self._command_strobe(StrobeAddress.STX)
 
     @contextlib.contextmanager
@@ -966,31 +954,23 @@
             checksum_valid=bool(buffer[-1] >> 7),
             link_quality_indicator=buffer[-1] & 0b0111111,
         )
 
     def _wait_for_packet(  # unstable
         self,
         timeout: datetime.timedelta,
-        # https://github.com/hhk7734/python3-gpiod/blob/v1.5.0/py_src/gpiod/libgpiodcxx/__init__.py#L83
-        gdo0_chip: cc1101._gpio.ChipSelector = 0,
-        gdo0_line_name: str = "GPIO24",  # recommended in README.md
+        gdo0_gpio_line_name: bytes = b"GPIO24",  # recommended in README.md
     ) -> typing.Optional[_ReceivedPacket]:
         """
         depends on IOCFG0 == 0b00000001 (see _configure_defaults)
         """
         # pylint: disable=protected-access
-        gdo0_line = cc1101._gpio.get_line(
-            chip_selector=gdo0_chip, line_name=gdo0_line_name
-        )
-        import gpiod  # pylint: disable=import-outside-toplevel; see get_line()
-
-        # https://github.com/hhk7734/python3-gpiod/blob/v1.2.1/py_src/gpiod/test/button.py#L33
-        gdo0_line_request = gpiod.line_request()
-        gdo0_line_request.consumer = "python cc1101 {}".format(
-            self._wait_for_packet.__name__
-        )
-        gdo0_line_request.request_type = gpiod.line_request.EVENT_RISING_EDGE
-        gdo0_line.request(gdo0_line_request)
+        gdo0 = cc1101._gpio.GPIOLine.find(name=gdo0_gpio_line_name)
         self._enable_receive_mode()
-        if not gdo0_line.event_wait(timeout=timeout):
+        if not gdo0.wait_for_rising_edge(consumer=b"CC1101:GDO0", timeout=timeout):
+            self._command_strobe(StrobeAddress.SIDLE)
+            _LOGGER.debug(
+                "reached timeout of %.02f seconds while waiting for packet",
+                timeout.total_seconds(),
+            )
             return None  # timeout
         return self._get_received_packet()
```

### Comparing `cc1101-2.7.3rc0/cc1101/_cli.py` & `cc1101-3.0.0/cc1101/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         if args.debug
         else "%(message)s",
         datefmt="%Y-%m-%dT%H:%M:%S%z",
     )
 
 
 def _configure_via_args(
+    *,
     transceiver: cc1101.CC1101,
     args: argparse.Namespace,
     packet_length_if_fixed: typing.Optional[int],
 ) -> None:
     if args.base_frequency_hertz:
         transceiver.set_base_frequency_hertz(args.base_frequency_hertz)
     if args.symbol_rate_baud:
@@ -130,18 +131,17 @@
             print(
                 "0b{value:08b}, # 0x{value:02x} {register_name}".format(
                     value=value, register_name=register.name
                 )
             )
         print("]")
         print(
-            "# PATABLE = {}".format(
-                # pylint: disable=protected-access; internal function & method
-                cc1101._format_patable(transceiver._get_patable(), insert_spaces=True)
-            )
+            # pylint: disable=protected-access; internal function & method
+            "# PATABLE = "
+            + cc1101._format_patable(transceiver._get_patable(), insert_spaces=True)
         )
 
 
 def _transmit():
     argparser = argparse.ArgumentParser(
         description="Transmits the payload provided via standard input (stdin)"
         " ASK/OOK-modulated in big-endian bit order.",
```

### Comparing `cc1101-2.7.3rc0/cc1101/addresses.py` & `cc1101-3.0.0/cc1101/addresses.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/cc1101/options.py` & `cc1101-3.0.0/cc1101/options.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/cc1101.egg-info/PKG-INFO` & `cc1101-3.0.0/cc1101.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc1101
-Version: 2.7.3rc0
+Version: 3.0.0
 Summary: Python Library & Command Line Tool to Transmit RF Signals via C1101 Transceivers
 Home-page: https://github.com/fphammerle/python-cc1101
 Author: Fabian Peter Hammerle
 Author-email: fabian+python-cc1101@hammerle.me
 License: GPLv3+
 Project-URL: Changelog, https://github.com/fphammerle/python-cc1101/blob/master/CHANGELOG.md
 Description: # python-cc1101
@@ -91,19 +91,20 @@
         followed by a re-login.
         
         Consult CC1101's offical docs for an in-depth explanation of all options:
         https://www.ti.com/lit/ds/symlink/cc1101.pdf
         
 Keywords: ISM,SPI,automation,radio-frequency,raspberry-pi,transceiver,transmission,wireless
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Communications
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cc1101-2.7.3rc0/cc1101.egg-info/SOURCES.txt` & `cc1101-3.0.0/cc1101.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/examples/asynchronous_gpio_transmit.py` & `cc1101-3.0.0/examples/asynchronous_gpio_transmit.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/examples/transmit_fixed_length.py` & `cc1101-3.0.0/examples/transmit_fixed_length.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/examples/transmit_variable_length.py` & `cc1101-3.0.0/examples/transmit_variable_length.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/setup.py` & `cc1101-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,37 +41,37 @@
         "raspberry-pi",
         "transceiver",
         "transmission",
         "wireless",
     ],
     classifiers=[
         # https://pypi.org/classifiers/
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: POSIX :: Linux",
         # .github/workflows/python.yml
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Home Automation",
         "Topic :: Communications",
     ],
     entry_points={
         "console_scripts": [
             "cc1101-export-config = cc1101._cli:_export_config",
             "cc1101-transmit = cc1101._cli:_transmit",
         ]
     },
+    # >=3.6 f-strings, variable type hints, force kwargs with *
+    # >=3.7 postponed evaluation of type annotations (PEP563)
+    python_requires=">=3.7",
     install_requires=[
-        # potential alternative: https://salsa.debian.org/debian/libgpiod (python3-libgpiod)
-        # https://github.com/hhk7734/python3-gpiod
-        "gpiod",
         # apt install python3-spidev
         # https://github.com/doceme/py-spidev
         "spidev",
     ],
     setup_requires=["setuptools_scm"],
     tests_require=["pytest"],
 )
```

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x04_0x05_sync1_sync0.py` & `cc1101-3.0.0/tests/config/test_0x04_0x05_sync1_sync0.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x06_pktlen.py` & `cc1101-3.0.0/tests/config/test_0x06_pktlen.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x08_pktctrl0.py` & `cc1101-3.0.0/tests/config/test_0x08_pktctrl0.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x10_mdmcfg4.py` & `cc1101-3.0.0/tests/config/test_0x10_mdmcfg4.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x11_mdmcfg3.py` & `cc1101-3.0.0/tests/config/test_0x11_mdmcfg3.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x12_mdmcfg2.py` & `cc1101-3.0.0/tests/config/test_0x12_mdmcfg2.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x13_mdmcfg1.py` & `cc1101-3.0.0/tests/config/test_0x13_mdmcfg1.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x22_frend0.py` & `cc1101-3.0.0/tests/config/test_0x22_frend0.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/config/test_0x3e_patable.py` & `cc1101-3.0.0/tests/config/test_0x3e_patable.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/test_cli_export_config.py` & `cc1101-3.0.0/tests/test_cli_export_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 )
 def test_configure_device(args, packet_length_mode, checksum_disabled):
     # pylint: disable=too-many-arguments
     with unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock:
         with unittest.mock.patch("sys.argv", args):
             cc1101._cli._export_config()
     transceiver_class_mock.assert_called_once_with(lock_spi_device=True)
-    transceiver_mock = transceiver_class_mock().__enter__()
+    with transceiver_class_mock() as transceiver_mock:
+        pass
     if packet_length_mode is None:
-        transceiver_mock.__enter__().set_packet_length_mode.assert_not_called()
+        transceiver_mock.set_packet_length_mode.assert_not_called()
     else:
         transceiver_mock.set_packet_length_mode.assert_called_once_with(
             packet_length_mode
         )
     transceiver_mock.set_packet_length_bytes.assert_not_called()
-    if checksum_disabled:
+    if checksum_disabled:  # pylint: disable=duplicate-code
         transceiver_mock.disable_checksum.assert_called_once_with()
     else:
         transceiver_mock.disable_checksum.assert_not_called()
 
 
 @pytest.mark.parametrize(
     ("args", "output_power_settings"),
@@ -64,38 +65,38 @@
         (
             ["", "-p", "3", "15", "30", "39", "80", "129", "203", "194"],
             [3, 15, 30, 39, 80, 129, 203, 194],
         ),
     ),
 )
 def test_configure_device_output_power_settings(args, output_power_settings):
-    with unittest.mock.patch("cc1101.CC1101") as transceiver_mock:
+    with unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock:
         with unittest.mock.patch("sys.argv", args):
             cc1101._cli._export_config()
+    with transceiver_class_mock() as transceiver_mock:
+        pass
     if output_power_settings is None:
-        transceiver_mock().__enter__().set_output_power.assert_not_called()
+        transceiver_mock.set_output_power.assert_not_called()
     else:
-        transceiver_mock().__enter__().set_output_power.assert_called_with(
-            output_power_settings
-        )
+        transceiver_mock.set_output_power.assert_called_with(output_power_settings)
 
 
 def test_export_python_list(capsys, caplog):
-    with unittest.mock.patch("cc1101.CC1101") as transceiver_mock:
-        transceiver_mock().__enter__().get_configuration_register_values.return_value = {
+    with unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock:
+        with transceiver_class_mock() as transceiver_mock:
+            pass
+        transceiver_mock.get_configuration_register_values.return_value = {
             cc1101.addresses.ConfigurationRegisterAddress.IOCFG2: 0x29,
             cc1101.addresses.ConfigurationRegisterAddress.IOCFG1: 0x2E,
         }
-        transceiver_mock().__enter__()._get_patable.return_value = [0xC6] + [0] * 7
+        transceiver_mock._get_patable.return_value = [0xC6] + [0] * 7
         with unittest.mock.patch("sys.argv", [""]):
             with caplog.at_level(logging.INFO):
                 cc1101._cli._export_config()
-    assert caplog.record_tuples == [
-        ("cc1101._cli", 20, str(transceiver_mock().__enter__()))
-    ]
+    assert caplog.record_tuples == [("cc1101._cli", 20, str(transceiver_mock))]
     out, err = capsys.readouterr()
     assert not err
     assert (
         out
         == "[\n0b00101001, # 0x29 IOCFG2\n0b00101110, # 0x2e IOCFG1\n]\n"
         + "# PATABLE = (0xc6, 0, 0, 0, 0, 0, 0, 0)\n"
     )
@@ -113,24 +114,25 @@
     ),
 )
 def test_root_log_level(args, root_log_level, log_format):
     with unittest.mock.patch("cc1101.CC1101"), unittest.mock.patch(
         "sys.argv", [""] + args
     ), unittest.mock.patch("logging.basicConfig") as logging_basic_config_mock:
         cc1101._cli._export_config()
-    assert logging_basic_config_mock.call_count == 1
+    logging_basic_config_mock.assert_called_once()
     assert logging_basic_config_mock.call_args[1]["level"] == root_log_level
     assert logging_basic_config_mock.call_args[1]["format"] == log_format
 
 
 def test_logging(caplog):
     with unittest.mock.patch("sys.argv", [""]), unittest.mock.patch(
         "cc1101.CC1101"
-    ) as transceiver_mock, caplog.at_level(logging.DEBUG):
-        transceiver_mock().__enter__().__str__.return_value = "dummystr"
+    ) as transceiver_class_mock, caplog.at_level(logging.DEBUG):
+        with transceiver_class_mock() as transceiver_mock:
+            transceiver_mock.__str__.return_value = "dummystr"
         cc1101._cli._export_config()
     assert len(caplog.records) == 2
     assert caplog.records[0].levelno == logging.DEBUG
     assert caplog.records[0].name == "cc1101._cli"
     assert caplog.records[0].message.startswith(
         "args=Namespace(base_frequency_hertz=None, "
     )
```

### Comparing `cc1101-2.7.3rc0/tests/test_cli_transmit.py` & `cc1101-3.0.0/tests/test_cli_transmit.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,53 +100,51 @@
     symbol_rate_baud,
     sync_mode,
     packet_length_mode,
     checksum_disabled,
     payload,
 ):
     # pylint: disable=too-many-arguments
-    with unittest.mock.patch("cc1101.CC1101") as transceiver_mock:
+    with unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock:
         stdin_mock = unittest.mock.MagicMock()
         stdin_mock.buffer = io.BytesIO(payload)
         with unittest.mock.patch("sys.stdin", stdin_mock):
             with unittest.mock.patch("sys.argv", args):
                 cc1101._cli._transmit()
-    transceiver_mock.assert_called_once_with(lock_spi_device=True)
+    transceiver_class_mock.assert_called_once_with(lock_spi_device=True)
+    with transceiver_class_mock() as transceiver_mock:
+        pass
     if base_frequency_hertz is None:
-        transceiver_mock().__enter__().set_base_frequency_hertz.assert_not_called()
+        transceiver_mock.set_base_frequency_hertz.assert_not_called()
     else:
-        transceiver_mock().__enter__().set_base_frequency_hertz.assert_called_once_with(
+        transceiver_mock.set_base_frequency_hertz.assert_called_once_with(
             base_frequency_hertz
         )
     if symbol_rate_baud is None:
-        transceiver_mock().__enter__().set_symbol_rate_baud.assert_not_called()
+        transceiver_mock.set_symbol_rate_baud.assert_not_called()
     else:
-        transceiver_mock().__enter__().set_symbol_rate_baud.assert_called_once_with(
-            symbol_rate_baud
-        )
+        transceiver_mock.set_symbol_rate_baud.assert_called_once_with(symbol_rate_baud)
     if sync_mode is None:
-        transceiver_mock().__enter__().set_sync_mode.assert_not_called()
+        transceiver_mock.set_sync_mode.assert_not_called()
     else:
-        transceiver_mock().__enter__().set_sync_mode.assert_called_once_with(sync_mode)
-    if packet_length_mode is None:
-        transceiver_mock().__enter__().set_packet_length_mode.assert_not_called()
+        transceiver_mock.set_sync_mode.assert_called_once_with(sync_mode)
+    if packet_length_mode is None:  # pylint: disable=duplicate-code
+        transceiver_mock.set_packet_length_mode.assert_not_called()
     else:
-        transceiver_mock().__enter__().set_packet_length_mode.assert_called_once_with(
+        transceiver_mock.set_packet_length_mode.assert_called_once_with(
             packet_length_mode
         )
     if packet_length_mode == PacketLengthMode.FIXED:
-        transceiver_mock().__enter__().set_packet_length_bytes.assert_called_with(
-            len(payload)
-        )
+        transceiver_mock.set_packet_length_bytes.assert_called_with(len(payload))
     else:
-        transceiver_mock().__enter__().set_packet_length_bytes.assert_not_called()
+        transceiver_mock.set_packet_length_bytes.assert_not_called()
     if checksum_disabled:
-        transceiver_mock().__enter__().disable_checksum.assert_called_once_with()
+        transceiver_mock.disable_checksum.assert_called_once_with()
     else:
-        transceiver_mock().__enter__().disable_checksum.assert_not_called()
+        transceiver_mock.disable_checksum.assert_not_called()
 
 
 @pytest.mark.parametrize(
     ("args", "output_power_settings"),
     (
         ([""], None),
         (["", "-p", "198"], [198]),  # default
@@ -155,27 +153,27 @@
         (
             ["", "-p", "18", "14", "29", "52", "96", "132", "200", "192"],
             [18, 14, 29, 52, 96, 132, 200, 192],
         ),
     ),
 )
 def test_configure_device_output_power(args, output_power_settings):
-    with unittest.mock.patch("cc1101.CC1101") as transceiver_mock:
+    with unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock:
         stdin_mock = unittest.mock.MagicMock()
         stdin_mock.buffer = io.BytesIO(b"message")
         with unittest.mock.patch("sys.stdin", stdin_mock):
             with unittest.mock.patch("sys.argv", args):
                 cc1101._cli._transmit()
-    transceiver_mock.assert_called_once_with(lock_spi_device=True)
+    transceiver_class_mock.assert_called_once_with(lock_spi_device=True)
+    with transceiver_class_mock() as transceiver_mock:
+        pass
     if output_power_settings:
-        transceiver_mock().__enter__().set_output_power.assert_called_with(
-            output_power_settings
-        )
+        transceiver_mock.set_output_power.assert_called_with(output_power_settings)
     else:
-        transceiver_mock().__enter__().set_output_power.assert_not_called()
+        transceiver_mock.set_output_power.assert_not_called()
 
 
 @pytest.mark.parametrize(
     ("args", "root_log_level", "log_format"),
     (
         ([""], logging.INFO, "%(message)s"),
         (
@@ -190,30 +188,31 @@
     stdin_mock.buffer = io.BytesIO(b"")
     with unittest.mock.patch("cc1101.CC1101"), unittest.mock.patch(
         "sys.stdin", stdin_mock
     ), unittest.mock.patch("sys.argv", args), unittest.mock.patch(
         "logging.basicConfig"
     ) as logging_basic_config_mock:
         cc1101._cli._transmit()
-    assert logging_basic_config_mock.call_count == 1
+    logging_basic_config_mock.assert_called_once()
     assert logging_basic_config_mock.call_args[1]["level"] == root_log_level
     assert logging_basic_config_mock.call_args[1]["format"] == log_format
 
 
 @pytest.mark.parametrize("payload", (b"", b"message"))
 def test_logging(caplog, payload):
     # pylint: disable=too-many-arguments
     stdin_mock = unittest.mock.MagicMock()
     stdin_mock.buffer = io.BytesIO(payload)
     with unittest.mock.patch("sys.stdin", stdin_mock), unittest.mock.patch(
         "sys.argv", [""]
-    ), unittest.mock.patch("cc1101.CC1101") as transceiver_mock, caplog.at_level(
+    ), unittest.mock.patch("cc1101.CC1101") as transceiver_class_mock, caplog.at_level(
         logging.DEBUG
     ):
-        transceiver_mock().__enter__().__str__.return_value = "dummy"
+        with transceiver_class_mock() as transceiver_mock:
+            transceiver_mock.__str__.return_value = "dummy"
         cc1101._cli._transmit()
     assert len(caplog.records) == 2
     assert caplog.records[0].name == "cc1101._cli"
     assert caplog.records[0].levelno == logging.DEBUG
     assert caplog.records[0].message.startswith(
         "args=Namespace(base_frequency_hertz=None, "
     )
```

### Comparing `cc1101-2.7.3rc0/tests/test_config.py` & `cc1101-3.0.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 )
 def test_set_base_frequency_hertz_low_warning(transceiver, freq_hz, warn):
     with unittest.mock.patch.object(
         transceiver, "_set_base_frequency_control_word"
     ) as set_control_word_mock:
         with warnings.catch_warnings(record=True) as caught_warnings:
             transceiver.set_base_frequency_hertz(freq_hz)
-    assert set_control_word_mock.call_count == 1
+    set_control_word_mock.assert_called_once()
     if warn:
         assert len(caught_warnings) == 1
         assert (
             str(caught_warnings[0].message)
             == "CC1101 is unable to transmit at frequencies below 281.7 MHz"
         )
     else:
```

### Comparing `cc1101-2.7.3rc0/tests/test_lock.py` & `cc1101-3.0.0/tests/test_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @pytest.fixture(scope="function")
 def spidev_mock(tmp_path):
     class _SpiDevMock:
         def __init__(self):
             self._file = None
 
         def open(self, bus, select):
-            path = tmp_path.joinpath("spidev{}.{}~".format(bus, select))
+            path = tmp_path.joinpath(f"spidev{bus}.{select}~")
             self._file = path.open("w+")
 
         def fileno(self):
             # mimic behaviour of spidev.SpiDev.fileno()
             return self._file.fileno() if self._file else -1
 
         def close(self):
```

### Comparing `cc1101-2.7.3rc0/tests/test_receive.py` & `cc1101-3.0.0/tests/test_receive.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import datetime
 import unittest.mock
 
-import gpiod
 import pytest
 
 # pylint: disable=protected-access
 
 
 def test__enable_receive_mode(transceiver):
     transceiver._spi.xfer.return_value = [15]
@@ -41,53 +40,43 @@
         received_packet = transceiver._get_received_packet()
     read_status_register.assert_called_once_with(0x3B)
     read_burst_mock.assert_called_once_with(
         start_register=0x3F, length=len(fifo_buffer)
     )
     assert received_packet.payload == payload
     assert received_packet._rssi_index == 128
-    # assert received_packet.checksum_valid
+    assert received_packet.checksum_valid
     assert received_packet.link_quality_indicator == 42
 
 
-@pytest.mark.parametrize("gdo0_chip_selector", (0, "/dev/gpiochip1"))
-@pytest.mark.parametrize("gdo0_line_name", ("GPIO24", "GPIO25"))
+@pytest.mark.parametrize("gdo0_gpio_line_name", (b"GPIO24", b"GPIO25"))
 @pytest.mark.parametrize("reached_timeout", (True, False))
-@pytest.mark.parametrize("timeout", (datetime.timedelta(seconds=1),))
-def test__wait_for_packet(
-    transceiver, gdo0_chip_selector, gdo0_line_name, timeout, reached_timeout
-):
+@pytest.mark.parametrize("timeout", (datetime.timedelta(seconds=4),))
+def test__wait_for_packet(transceiver, gdo0_gpio_line_name, timeout, reached_timeout):
     line_mock = unittest.mock.MagicMock()
-    line_mock.event_wait.return_value = not reached_timeout
+    line_mock.wait_for_rising_edge.return_value = not reached_timeout
     with unittest.mock.patch(
-        "cc1101._gpio.get_line"
-    ) as get_line_mock, unittest.mock.patch.object(
-        transceiver, "_get_received_packet"
+        "cc1101._gpio.GPIOLine.find", return_value=line_mock
+    ) as find_line_mock, unittest.mock.patch.object(
+        transceiver, "_get_received_packet", return_value="packet-dummy"
     ) as get_received_packet_mock, unittest.mock.patch.object(
         transceiver, "_enable_receive_mode"
-    ) as enable_receive_mode_mock:
-        get_line_mock.return_value = line_mock
-        get_received_packet_mock.return_value = "packet-dummy"
+    ) as enable_receive_mode_mock, unittest.mock.patch.object(
+        transceiver, "_command_strobe"
+    ) as command_strobe_mock:
         packet = transceiver._wait_for_packet(
             timeout=timeout,
-            gdo0_chip=gdo0_chip_selector,
-            gdo0_line_name=gdo0_line_name,
+            gdo0_gpio_line_name=gdo0_gpio_line_name,
         )
-    get_line_mock.assert_called_once_with(
-        chip_selector=gdo0_chip_selector, line_name=gdo0_line_name
-    )
-    assert line_mock.request.call_count == 1
-    (line_request,) = line_mock.request.call_args[0]
-    assert vars(line_request) == {
-        "consumer": "python cc1101 _wait_for_packet",
-        "flags": 0,
-        "request_type": gpiod.line_request.EVENT_RISING_EDGE,
-    }
-    assert not line_mock.request.call_args[1]
+    find_line_mock.assert_called_once_with(name=gdo0_gpio_line_name)
     enable_receive_mode_mock.assert_called_once_with()
-    line_mock.event_wait.assert_called_once_with(timeout=timeout)
+    line_mock.wait_for_rising_edge.assert_called_once_with(
+        consumer=b"CC1101:GDO0", timeout=timeout
+    )
     if reached_timeout:
         assert packet is None
+        command_strobe_mock.assert_called_once_with(0x36)  # SIDLE
         get_received_packet_mock.assert_not_called()
     else:
+        command_strobe_mock.assert_not_called()
         get_received_packet_mock.assert_called_once_with()
         assert packet == "packet-dummy"
```

### Comparing `cc1101-2.7.3rc0/tests/test_received_packet.py` & `cc1101-3.0.0/tests/test_received_packet.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/test_spi.py` & `cc1101-3.0.0/tests/test_spi.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 @pytest.mark.parametrize("bus", [0, 1])
 @pytest.mark.parametrize("chip_select", [0, 2])
 def test___init__select_device(bus, chip_select):
     with unittest.mock.patch("spidev.SpiDev"):
         transceiver = cc1101.CC1101(spi_bus=bus, spi_chip_select=chip_select)
     assert transceiver._spi_bus == bus
     assert transceiver._spi_chip_select == chip_select
-    assert transceiver._spi_device_path == "/dev/spidev{}.{}".format(bus, chip_select)
+    assert transceiver._spi_device_path == f"/dev/spidev{bus}.{chip_select}"
+    assert transceiver._spi_max_speed_hz == 55700
     transceiver._spi.open.side_effect = SystemExit
     with pytest.raises(SystemExit):
         with transceiver:
             pass
     transceiver._spi.open.assert_called_once_with(bus, chip_select)
 
 
@@ -83,26 +84,40 @@
             cc1101.addresses.StatusRegisterAddress.PARTNUM: 0,
             cc1101.addresses.StatusRegisterAddress.VERSION: chip_version,
         }[r]
         with transceiver as transceiver_context:
             assert transceiver == transceiver_context
             transceiver._spi.open.assert_called_once_with(0, 0)
             assert transceiver._spi.max_speed_hz == 55700
+            assert transceiver._spi.max_speed_hz == transceiver._spi_max_speed_hz
             reset_mock.assert_called_once_with()
             set_modulation_format_mock.assert_called_once_with(
                 cc1101.options.ModulationFormat.ASK_OOK
             )
             set_pa_setting_mock.assert_called_once_with(1)
             disable_whitening_mock.assert_called_once_with()
             assert write_burst_mock.call_args_list == [
                 unittest.mock.call(0x18, [0b010100]),
                 unittest.mock.call(0x02, [0b000001]),
             ]
 
 
+@pytest.mark.parametrize("spi_max_speed_hz", [55700, 500000])
+def test___enter__spi_max_speed(spi_max_speed_hz):
+    with unittest.mock.patch("spidev.SpiDev"):
+        transceiver = cc1101.CC1101(spi_max_speed_hz=spi_max_speed_hz)
+    assert transceiver._spi_max_speed_hz == spi_max_speed_hz
+    with unittest.mock.patch.object(
+        transceiver, "_reset", side_effect=SystemExit
+    ), pytest.raises(SystemExit):
+        with transceiver:
+            pass
+    assert transceiver._spi.max_speed_hz == spi_max_speed_hz
+
+
 def test___enter___unsupported_partnum(transceiver):
     with unittest.mock.patch.object(
         transceiver, "_read_status_register"
     ) as read_status_register_mock, unittest.mock.patch.object(transceiver, "_reset"):
         read_status_register_mock.side_effect = lambda r: {
             cc1101.addresses.StatusRegisterAddress.PARTNUM: 21
         }[r]
@@ -117,15 +132,15 @@
     ) as read_status_register_mock, unittest.mock.patch.object(transceiver, "_reset"):
         read_status_register_mock.side_effect = lambda r: {
             cc1101.addresses.StatusRegisterAddress.PARTNUM: 0,
             cc1101.addresses.StatusRegisterAddress.VERSION: 0x15,
         }[r]
         with pytest.raises(
             ValueError,
-            match=r"^{}$".format(
+            match=r"^{}$".format(  # pylint: disable=consider-using-f-string
                 re.escape(
                     "Unsupported chip version 0x15 (expected one of [0x04, 0x14])"
                 )
             ),
         ):
             with transceiver:
                 pass
@@ -152,17 +167,15 @@
 
 @pytest.mark.parametrize("bus", [0, 1])
 @pytest.mark.parametrize("chip_select", [0, 2])
 def test___enter__permission_error(transceiver, bus, chip_select):
     transceiver._spi.open.side_effect = PermissionError("[Errno 13] Permission denied")
     transceiver._spi_bus = bus
     transceiver._spi_chip_select = chip_select
-    with pytest.raises(
-        PermissionError, match=r"\s/dev/spidev{}.{}\s".format(bus, chip_select)
-    ):
+    with pytest.raises(PermissionError, match=f"\\s/dev/spidev{bus}.{chip_select}\\s"):
         with transceiver:
             pass
 
 
 def test___enter__non_idle(transceiver):
     with unittest.mock.patch.object(
         transceiver,
```

### Comparing `cc1101-2.7.3rc0/tests/test_state.py` & `cc1101-3.0.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/test_str.py` & `cc1101-3.0.0/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `cc1101-2.7.3rc0/tests/test_transmit.py` & `cc1101-3.0.0/tests/test_transmit.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         unittest.mock.call([0x3F | 0x40] + list(payload)),
         unittest.mock.call([0x35]),  # start transmission
     ]
     assert caplog.record_tuples == [
         (
             "cc1101",
             20,
-            "transmitting 0x{} ({!r})".format(
-                "".join("{:02x}".format(b) for b in payload), payload
+            "transmitting 0x{} ({!r})".format(  # pylint: disable=consider-using-f-string
+                "".join(f"{b:02x}" for b in payload), payload
             ),
         )
     ]
 
 
 @pytest.mark.parametrize(
     "payload", (b"\x01\0", b"\x03\xaa\xbb\xcc", b"\x10" + bytes(range(16)))
```

