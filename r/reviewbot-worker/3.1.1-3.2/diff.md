# Comparing `tmp/reviewbot-worker-3.1.1.tar.gz` & `tmp/reviewbot-worker-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviewbot-worker-3.1.1.tar", last modified: Wed Jul 27 03:04:51 2022, max compression
+gzip compressed data, was "reviewbot-worker-3.2.tar", last modified: Thu May  4 02:36:51 2023, max compression
```

## Comparing `reviewbot-worker-3.1.1.tar` & `reviewbot-worker-3.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.585445 reviewbot-worker-3.1.1/
--rw-r--r--   0 chipx86    (501) staff       (20)      208 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/MANIFEST.in
--rw-r--r--   0 chipx86    (501) staff       (20)     6211 2022-07-27 03:04:51.585525 reviewbot-worker-3.1.1/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     5046 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/README.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      218 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/dev-requirements.txt
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.575442 reviewbot-worker-3.1.1/reviewbot/
--rw-r--r--   0 chipx86    (501) staff       (20)     1953 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14568 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/celery.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8098 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/config.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2303 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/deprecation.py
--rw-r--r--   0 chipx86    (501) staff       (20)      575 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6379 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/main.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.575652 reviewbot-worker-3.1.1/reviewbot/processing/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/processing/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    25707 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/processing/review.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.576044 reviewbot-worker-3.1.1/reviewbot/processing/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/processing/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    38792 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/processing/tests/test_file.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2805 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/processing/tests/test_review.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10044 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/repositories.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10631 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tasks.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.576457 reviewbot-worker-3.1.1/reviewbot/testing/
--rw-r--r--   0 chipx86    (501) staff       (20)      247 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/testing/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    28908 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/testing/testcases.py
--rw-r--r--   0 chipx86    (501) staff       (20)      654 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/testing/utils.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.577189 reviewbot-worker-3.1.1/reviewbot/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4458 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tests/test_celery.py
--rw-r--r--   0 chipx86    (501) staff       (20)    23126 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tests/test_config.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11309 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tests/test_repositories.py
--rw-r--r--   0 chipx86    (501) staff       (20)    20641 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tests/test_tasks.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.579541 reviewbot-worker-3.1.1/reviewbot/tools/
--rw-r--r--   0 chipx86    (501) staff       (20)     3466 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.579986 reviewbot-worker-3.1.1/reviewbot/tools/base/
--rw-r--r--   0 chipx86    (501) staff       (20)      585 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/base/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8570 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/base/mixins.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3253 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/base/registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11995 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/base/tool.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10578 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/cargotool.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3615 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/checkstyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5726 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/clang.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5498 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/cppcheck.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4459 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/cpplint.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3080 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/doc8.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10998 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/fbinfer.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3241 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/flake8.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2174 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/gofmt.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7793 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/gotool.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4667 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/jshint.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6953 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/pmd.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3322 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/pycodestyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2700 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/pydocstyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4277 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/pyflakes.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10774 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/rbsecretscanner.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4161 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/rubocop.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2265 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/rustfmt.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8838 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/shellcheck.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.573192 reviewbot-worker-3.1.1/reviewbot/tools/support/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.580099 reviewbot-worker-3.1.1/reviewbot/tools/support/js/
--rw-r--r--   0 chipx86    (501) staff       (20)      358 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/support/js/jshint_reporter.js
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.580430 reviewbot-worker-3.1.1/reviewbot/tools/testing/
--rw-r--r--   0 chipx86    (501) staff       (20)      482 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/testing/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1212 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/testing/decorators.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12202 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/testing/testcases.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.583202 reviewbot-worker-3.1.1/reviewbot/tools/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8135 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_base_tool.py
--rw-r--r--   0 chipx86    (501) staff       (20)    30196 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cargotool.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14145 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_checkstyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18239 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_clang.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10975 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cppcheck.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10403 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cpplint.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6959 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_doc8.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14421 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_fbinfer.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4392 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_file_patterns_from_setting_mixin.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9260 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_flake8.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4167 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_gofmt.py
--rw-r--r--   0 chipx86    (501) staff       (20)    20264 2022-07-27 03:04:49.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_gotool.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6016 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_java_tool_mixin.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4740 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_jshint.py
--rw-r--r--   0 chipx86    (501) staff       (20)    19734 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pmd.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4518 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pycodestyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7145 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pydocstyle.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5001 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pyflakes.py
--rw-r--r--   0 chipx86    (501) staff       (20)    25832 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rbsecretscanner.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4313 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18853 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rubocop.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4795 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rustfmt.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18533 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/tests/test_shellcheck.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.583422 reviewbot-worker-3.1.1/reviewbot/tools/utils/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/utils/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1042 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/tools/utils/codeclimate.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.584060 reviewbot-worker-3.1.1/reviewbot/utils/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1332 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/api.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7057 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/filesystem.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1447 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/log.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5463 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/process.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.584545 reviewbot-worker-3.1.1/reviewbot/utils/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12567 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/tests/test_filesystem.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2171 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/tests/test_process.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1658 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/tests/test_text.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1128 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/reviewbot/utils/text.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.585231 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     6211 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     3089 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      966 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/entry_points.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      446 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       10 2022-07-27 03:04:51.000000 reviewbot-worker-3.1.1/reviewbot_worker.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      196 2022-07-27 03:04:51.585820 reviewbot-worker-3.1.1/setup.cfg
--rwxr-xr-x   0 chipx86    (501) staff       (20)     4080 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/setup.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.573757 reviewbot-worker-3.1.1/tests/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-07-27 03:04:51.585339 reviewbot-worker-3.1.1/tests/deps/
--rw-r--r--   0 chipx86    (501) staff       (20)      246 2022-07-27 03:04:50.000000 reviewbot-worker-3.1.1/tests/deps/README.md
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.246602 reviewbot-worker-3.2/
+-rw-r--r--   0 chipx86    (501) staff       (20)      208 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/MANIFEST.in
+-rw-r--r--   0 chipx86    (501) staff       (20)     6209 2023-05-04 02:36:51.246664 reviewbot-worker-3.2/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     5046 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/README.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      218 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/dev-requirements.txt
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.236948 reviewbot-worker-3.2/reviewbot/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1953 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14568 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/celery.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8098 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/config.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2303 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/deprecation.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      575 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6379 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/main.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.237146 reviewbot-worker-3.2/reviewbot/processing/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/processing/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    26578 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/processing/review.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.237526 reviewbot-worker-3.2/reviewbot/processing/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/processing/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    39406 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/processing/tests/test_file.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2805 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/processing/tests/test_review.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10044 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/repositories.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10631 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tasks.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.237872 reviewbot-worker-3.2/reviewbot/testing/
+-rw-r--r--   0 chipx86    (501) staff       (20)      247 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/testing/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    28908 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/testing/testcases.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      654 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/testing/utils.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.238383 reviewbot-worker-3.2/reviewbot/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4458 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tests/test_celery.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    23126 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tests/test_config.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11309 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tests/test_repositories.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    20641 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tests/test_tasks.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.240604 reviewbot-worker-3.2/reviewbot/tools/
+-rw-r--r--   0 chipx86    (501) staff       (20)     3466 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.241059 reviewbot-worker-3.2/reviewbot/tools/base/
+-rw-r--r--   0 chipx86    (501) staff       (20)      585 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/base/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8570 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/base/mixins.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3253 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/base/registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11995 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/base/tool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10578 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/cargotool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3615 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/checkstyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5726 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/clang.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5498 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/cppcheck.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4459 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/cpplint.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3080 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/doc8.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10998 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/fbinfer.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3241 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/flake8.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2174 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/gofmt.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7793 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/gotool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4667 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/jshint.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7004 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/pmd.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3322 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/pycodestyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2700 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/pydocstyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4277 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/pyflakes.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12305 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/rbsecretscanner.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4161 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/rubocop.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2265 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/rustfmt.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8811 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/shellcheck.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.235034 reviewbot-worker-3.2/reviewbot/tools/support/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.241173 reviewbot-worker-3.2/reviewbot/tools/support/js/
+-rw-r--r--   0 chipx86    (501) staff       (20)      358 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/support/js/jshint_reporter.js
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.241510 reviewbot-worker-3.2/reviewbot/tools/testing/
+-rw-r--r--   0 chipx86    (501) staff       (20)      482 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/testing/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1212 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/testing/decorators.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13756 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/testing/testcases.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.244241 reviewbot-worker-3.2/reviewbot/tools/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8135 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_base_tool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    30277 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_cargotool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14145 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_checkstyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18239 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_clang.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10975 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_cppcheck.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10403 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_cpplint.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7004 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_doc8.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14421 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_fbinfer.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4392 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_file_patterns_from_setting_mixin.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9365 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_flake8.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4167 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_gofmt.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    20290 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_gotool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6016 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_java_tool_mixin.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4740 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_jshint.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    19734 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_pmd.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4436 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_pycodestyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7145 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_pydocstyle.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5001 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_pyflakes.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    31413 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_rbsecretscanner.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4313 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18853 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_rubocop.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4795 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_rustfmt.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18533 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/tests/test_shellcheck.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.244465 reviewbot-worker-3.2/reviewbot/tools/utils/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/utils/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1042 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/tools/utils/codeclimate.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.245152 reviewbot-worker-3.2/reviewbot/utils/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1332 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/api.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7057 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/filesystem.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1447 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/log.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5463 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/process.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.245616 reviewbot-worker-3.2/reviewbot/utils/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12567 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/tests/test_filesystem.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2171 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/tests/test_process.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1658 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/tests/test_text.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1128 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/reviewbot/utils/text.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.246317 reviewbot-worker-3.2/reviewbot_worker.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     6209 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     3089 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      966 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/entry_points.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      446 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       10 2023-05-04 02:36:51.000000 reviewbot-worker-3.2/reviewbot_worker.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      196 2023-05-04 02:36:51.246895 reviewbot-worker-3.2/setup.cfg
+-rwxr-xr-x   0 chipx86    (501) staff       (20)     4080 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/setup.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.235502 reviewbot-worker-3.2/tests/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-04 02:36:51.246442 reviewbot-worker-3.2/tests/deps/
+-rw-r--r--   0 chipx86    (501) staff       (20)      246 2023-05-04 02:36:50.000000 reviewbot-worker-3.2/tests/deps/README.md
```

### Comparing `reviewbot-worker-3.1.1/PKG-INFO` & `reviewbot-worker-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviewbot-worker
-Version: 3.1.1
+Version: 3.2
 Summary: Review Bot, the automated code reviewer (worker)
 Author: Beanbag, Inc.
 Author-email: support@beanbaginc.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: support@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reviewbot-worker-3.1.1/README.rst` & `reviewbot-worker-3.2/README.rst`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/__init__.py` & `reviewbot-worker-3.2/reviewbot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 #: The version of Review Bot.
 #:
 #: This is in the format of:
 #:
 #: (Major, Minor, Micro, Patch, alpha/beta/rc/final, Release Number, Released)
 #:
-VERSION = (3, 1, 1, 0, 'final', 0, True)
+VERSION = (3, 2, 0, 0, 'final', 0, True)
 
 
 def get_version_string():
     """Return the version of Review Bot.
 
     Returns:
         unicode:
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/celery.py` & `reviewbot-worker-3.2/reviewbot/celery.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/config.py` & `reviewbot-worker-3.2/reviewbot/config.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/deprecation.py` & `reviewbot-worker-3.2/reviewbot/deprecation.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/errors.py` & `reviewbot-worker-3.2/reviewbot/errors.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/main.py` & `reviewbot-worker-3.2/reviewbot/main.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/processing/review.py` & `reviewbot-worker-3.2/reviewbot/processing/review.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import division, unicode_literals
 
 import json
 import os
 from enum import Enum
 from itertools import islice
 
+import six
 from rbtools.api.errors import APIError
 
 from reviewbot.utils.filesystem import (ensure_dirs_exist,
                                         make_tempdir,
                                         make_tempfile,
                                         normalize_platform_path)
 from reviewbot.utils.log import get_logger
@@ -62,14 +63,20 @@
     Information about the file can be retreived through this class,
     including retrieving the actual body of the original or patched
     file.
 
     Allows comments to be made to the file in the review.
     """
 
+    #: The maximum number of lines allowed for a comment.
+    #:
+    #: If a comment exceeds this count, it will be capped and a line range
+    #: will be provided in the comment.
+    COMMENT_MAX_LINES = 10
+
     def __init__(self, review, api_filediff):
         """Initialize the File.
 
         Args:
             review (Review):
                 The review object.
 
@@ -103,15 +110,20 @@
             The contents of the patched file.
         """
         if (self.status == ReviewFileStatus.DELETED or
             not hasattr(self._api_filediff, 'get_patched_file')):
             return None
 
         try:
-            return self._api_filediff.get_patched_file().data
+            contents = self._api_filediff.get_patched_file().data
+
+            if isinstance(contents, six.text_type):
+                contents = contents.encode('utf-8')
+
+            return contents
         except APIError as e:
             if e.http_status == 404:
                 # This was a deleted file, a deleted FileDiff entry,
                 # or something has gone wrong with the setup.
                 return None
             elif e.http_status == 500:
                 # There was an issue with the patch server-side. Likely,
@@ -133,15 +145,20 @@
             The contents of the original file.
         """
         if (self.status == ReviewFileStatus.CREATED or
             not hasattr(self._api_filediff, 'get_original_file')):
             return None
 
         try:
-            return self._api_filediff.get_original_file().data
+            contents = self._api_filediff.get_original_file().data
+
+            if isinstance(contents, six.text_type):
+                contents = contents.encode('utf-8')
+
+            return contents
         except APIError as e:
             if e.http_status == 404:
                 # This was a deleted FileDiff entry, or something has gone
                 # wrong with the setup.
                 return None
             elif e.http_status == 500:
                 # There was probably an issue with accessing the repository
@@ -238,23 +255,27 @@
             empty if the lines could not be found.
         """
         if original:
             code_index = 2
         else:
             code_index = 5
 
-        return list(islice(
+        result = list(islice(
             (
                 # result[1] is the row information.
                 result[1][code_index]
                 for result in self._iter_lines(first_line=first_line,
                                                original=original)
             ),
             num_lines))
 
+        assert not result or isinstance(result[0], six.text_type)
+
+        return result
+
     def apply_patch(self, root_target_dir):
         """Apply the patch for this file to the filesystem.
 
         The file will be written relative to the current directory.
 
         Version Added:
             3.0
@@ -297,15 +318,15 @@
                 except Exception as e:
                     # We'll log and then continue, just creating the new file.
                     logger.warning('Unable to move source file "%s" to '
                                    'to "%s" for FileDiff ID=%s',
                                    source_file, dest_file, self.id)
 
             with open(dest_file, 'wb') as fp:
-                fp.write(self.patched_file_contents)
+                fp.write(self.patched_file_contents or b'')
 
         self.patched_file_path = self.dest_file
 
     def comment(self, text, first_line, num_lines=1, start_column=None,
                 error_code=None, issue=None, rich_text=False, original=False,
                 text_extra=None, severity=None):
         """Make a comment on the file.
@@ -361,26 +382,32 @@
             first_line = 1
             modified = True
         else:
             modified = (self.review.settings['comment_unmodified'] or
                         self._is_modified(first_line, num_lines))
 
         if modified:
+            extra = []
             real_line = self._translate_line_num(first_line)
 
             if num_lines != 1:
+                if num_lines > self.COMMENT_MAX_LINES:
+                    extra.append((
+                        'Lines',
+                        '%s-%s' % (first_line, first_line + num_lines - 1),
+                    ))
+                    num_lines = self.COMMENT_MAX_LINES
+
                 last_line = first_line + num_lines - 1
                 real_last_line = self._translate_line_num(last_line)
                 num_lines = real_last_line - real_line + 1
 
             if issue is None:
                 issue = self.review.settings['open_issues']
 
-            extra = []
-
             if start_column:
                 extra.append(('Column', start_column))
 
             if severity:
                 extra.append(('Severity', severity))
 
             if error_code:
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/processing/tests/test_file.py` & `reviewbot-worker-3.2/reviewbot/processing/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,33 @@
             'first_line': 12,
             'issue_opened': True,
             'num_lines': 2,
             'text': 'This is a comment',
             'rich_text': False,
         }])
 
+    def test_comment_with_line_range_exceeds_cap(self):
+        """Testing File.comment with line range > 10 lines"""
+        self.review_file.comment('This is a comment',
+                                 first_line=12,
+                                 num_lines=11)
+
+        self.assertEqual(self.review.comments, [{
+            'filediff_id': 42,
+            'first_line': 12,
+            'issue_opened': True,
+            'num_lines': 10,
+            'text': (
+                'This is a comment\n'
+                '\n'
+                'Lines: 12-22'
+            ),
+            'rich_text': False,
+        }])
+
     def test_comment_with_first_line_0(self):
         """Testing File.comment with first_line=0"""
         self.review_file.comment('This is a comment',
                                  first_line=0)
 
         self.assertEqual(self.review.comments, [{
             'filediff_id': 42,
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/processing/tests/test_review.py` & `reviewbot-worker-3.2/reviewbot/processing/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/repositories.py` & `reviewbot-worker-3.2/reviewbot/repositories.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tasks.py` & `reviewbot-worker-3.2/reviewbot/tasks.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/testing/testcases.py` & `reviewbot-worker-3.2/reviewbot/testing/testcases.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/testing/utils.py` & `reviewbot-worker-3.2/reviewbot/testing/utils.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tests/test_celery.py` & `reviewbot-worker-3.2/reviewbot/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tests/test_config.py` & `reviewbot-worker-3.2/reviewbot/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tests/test_repositories.py` & `reviewbot-worker-3.2/reviewbot/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tests/test_tasks.py` & `reviewbot-worker-3.2/reviewbot/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/__init__.py` & `reviewbot-worker-3.2/reviewbot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/base/__init__.py` & `reviewbot-worker-3.2/reviewbot/tools/base/__init__.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/base/mixins.py` & `reviewbot-worker-3.2/reviewbot/tools/base/mixins.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/base/registry.py` & `reviewbot-worker-3.2/reviewbot/tools/base/registry.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/base/tool.py` & `reviewbot-worker-3.2/reviewbot/tools/base/tool.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/cargotool.py` & `reviewbot-worker-3.2/reviewbot/tools/cargotool.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/checkstyle.py` & `reviewbot-worker-3.2/reviewbot/tools/checkstyle.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/clang.py` & `reviewbot-worker-3.2/reviewbot/tools/clang.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/cppcheck.py` & `reviewbot-worker-3.2/reviewbot/tools/cppcheck.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/cpplint.py` & `reviewbot-worker-3.2/reviewbot/tools/cpplint.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/doc8.py` & `reviewbot-worker-3.2/reviewbot/tools/doc8.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/fbinfer.py` & `reviewbot-worker-3.2/reviewbot/tools/fbinfer.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/flake8.py` & `reviewbot-worker-3.2/reviewbot/tools/flake8.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/gofmt.py` & `reviewbot-worker-3.2/reviewbot/tools/gofmt.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/gotool.py` & `reviewbot-worker-3.2/reviewbot/tools/gotool.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/jshint.py` & `reviewbot-worker-3.2/reviewbot/tools/jshint.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/pmd.py` & `reviewbot-worker-3.2/reviewbot/tools/pmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,22 @@
                           '\n'
                           'Check the file locally for more information.'
                           % error,
                           first_line=None)
 
             return
 
-        # Make sure there's only a single file. If not, something went wrong,
-        # but there isn't really anything the user can do about it. The
+        # Make sure there's only a single file, at most. If not, something went
+        # wrong, but there isn't really anything the user can do about it. The
         # administrator will need to look into it.
         files = report.get('files', [])
 
+        if not files:
+            return
+
         if len(files) != 1:
             self.logger.error('Expected 1 file in PMD output. Got %s: %r',
                               len(files), files)
             return
 
         # Report all errors found by PMD.
         for violation in files[0].get('violations', []):
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/pycodestyle.py` & `reviewbot-worker-3.2/reviewbot/tools/pycodestyle.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/pydocstyle.py` & `reviewbot-worker-3.2/reviewbot/tools/pydocstyle.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/pyflakes.py` & `reviewbot-worker-3.2/reviewbot/tools/pyflakes.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/rbsecretscanner.py` & `reviewbot-worker-3.2/reviewbot/tools/rbsecretscanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,14 +130,20 @@
             # NOTE: Erring on the low side for a length. Generated keys seem
             #       to be 190+ (but it's variable).
             #
             # Rule updated: April 7, 2021
             (pypi[-:][A-Za-z0-9_]{128,})
             |
 
+            # Review Board 5+ API Token
+            #
+            # Rule updated: October 31, 2022
+            (?P<reviewboard_api_token>rbp_[A-Za-z0-9]{251})
+            |
+
             # RSA Private Key
             #
             # Rule updated: April 7, 2021
             (----BEGIN\sRSA\sPRIVATE\sKEY----)
             |
 
             # SSH(DSA) Private Key
@@ -356,7 +362,40 @@
         try:
             header = json.loads(base64.b64decode(header).decode('utf-8'))
 
             return header['typ'] == 'JWT'
         except Exception:
             # This isn't a JSON web token.
             return False
+
+    def _is_reviewboard_api_token_valid(self, token, m):
+        """Return whether a Review Board API Token is valid.
+
+        Review Board API tokens (which were revamped in October 2022) are 255
+        characters long, prefixed with a ``rbp_`` prefix and contain a
+        Base62-encoded CRC32 checksum of the token data that follows, stored
+        as the last 6 characters of the token.
+
+        Args:
+            token (bytes):
+                The full token to validate.
+
+            m (object, unused):
+                The regex match data for the token.
+
+        Returns:
+            bool:
+            ``True`` if the token is valid. ``False`` if it is not.
+        """
+        checksum = base62_encode(crc32(token[4:-6]) & 0xFFFFFFFF).zfill(6)
+        checksum = checksum.decode('utf-8')
+        token = token.decode('utf-8')
+        token_checksum = token[-6:]
+
+        # Review Board 5.0 generated token checksums using an incorrect
+        # base62-encoding, which resulted in capital and lowercase letters
+        # being swapped. We check against checksum.swapcase() to catch those.
+        return (len(token) == 255 and
+                token.startswith('rbp') and
+                re.match(r'^_[0-9A-Za-z]+$', token[3:]) is not None and
+                (token_checksum == checksum or
+                 token_checksum == checksum.swapcase()))
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/rubocop.py` & `reviewbot-worker-3.2/reviewbot/tools/rubocop.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/rustfmt.py` & `reviewbot-worker-3.2/reviewbot/tools/rustfmt.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/shellcheck.py` & `reviewbot-worker-3.2/reviewbot/tools/shellcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         Returns:
             bool:
             ``True`` if the file can be handled. ``False`` if it cannot.
         """
         return (
             super(ShellCheckTool, self).get_can_handle_file(review_file,
                                                             **kwargs) or
-            self.SHELL_RE.match(review_file.patched_file_contents)
+            self.SHELL_RE.match(review_file.patched_file_contents or b'')
         )
 
     def build_base_command(self, **kwargs):
         """Build the base command line used to review files.
 
         Args:
             **kwargs (dict, unused):
@@ -211,27 +211,27 @@
                     replacement_start_column = replacement['column']
                     replacement_end_column = replacement['endColumn']
                     replacement_text = replacement['replacement']
                     replacement_line = \
                         replacement_lines[replacement_norm_linenum]
 
                     replacement_lines[replacement_norm_linenum] = (
-                        b'%s%s%s'
+                        '%s%s%s'
                         % (replacement_line[:replacement_start_column - 1],
-                           replacement_text.encode('utf-8'),
+                           replacement_text,
                            replacement_line[replacement_end_column - 1:]))
 
             if replacement_lines:
                 comment_text = (
                     '%s\n'
                     '\n'
                     'Suggested replacement:\n'
                     '```%s```'
                     % (comment_text,
-                       b'\n'.join(replacement_lines).decode('utf-8').strip())
+                       '\n'.join(replacement_lines).strip())
                 )
 
             f.comment(text=comment_text,
                       first_line=first_line,
                       num_lines=num_lines,
                       start_column=comment.get('column'),
                       severity=comment.get('level'),
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/testing/decorators.py` & `reviewbot-worker-3.2/reviewbot/tools/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/testing/testcases.py` & `reviewbot-worker-3.2/reviewbot/tools/testing/testcases.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,59 +223,85 @@
     #: :py:attr:`tool_exe_path`.
     #:
     #: Type:
     #:     dict
     tool_extra_exe_paths = {}
 
     def run_get_can_handle_file(self, filename, file_contents=b'',
-                                tool_settings={}):
+                                tool_settings={},
+                                file_contents_encoding='utf-8'):
         """Run get_can_handle_file with the given file and settings.
 
         This will create the review objects, set up a repository (if needed
         by the tool), apply any configuration, and run
         :py:meth:`~reviewbot.tools.base.BaseTool.get_can_handle_file`.
 
+        Version Changed:
+            3.1.2:
+            Added the ``file_contents_encoding`` argument.
+
         Args:
             filename (unicode):
                 The filename of the file being reviewed.
 
             file_contents (bytes, optional):
                 File content to review.
 
             tool_settings (dict, optional):
                 The settings to pass to the tool constructor.
 
+            file_contents_encoding (unicode, optional):
+                The encoding used for the provided file contents (both in
+                ``file_contents`` and ``other_contents``).
+
+                If not provided, this will be ``utf-8``.
+
+                Version Added:
+                    3.1.2
+
         Returns:
             bool:
             ``True`` if the file can be handled. ``False`` if it cannot.
         """
+        assert self.tool_class is not None
+        assert isinstance(file_contents, bytes)
+
         review = self.create_review()
         review_file = self.create_review_file(
             review,
             source_file=filename,
             dest_file=filename,
             diff_data=self.create_diff_data(chunks=[{
                 'change': 'insert',
-                'lines': file_contents.splitlines(),
+                'lines': (
+                    file_contents
+                    .decode(file_contents_encoding)
+                    .splitlines()
+                ),
                 'new_linenum': 1,
             }]),
             patched_content=file_contents)
 
         tool = self.tool_class(settings=tool_settings)
 
         return tool.get_can_handle_file(review_file)
 
     def run_tool_execute(self, filename, file_contents, checkout_dir=None,
-                         tool_settings={}, other_files={}):
+                         tool_settings={}, other_files={},
+                         file_contents_encoding='utf-8'):
         """Run execute with the given file and settings.
 
         This will create the review objects, set up a repository (if needed
         by the tool), apply any configuration, and run
         :py:meth:`~reviewbot.tools.base.BaseTool.execute`.
 
+        Version Changed:
+            3.1.2:
+            Added the ``file_contents_encoding`` argument.
+
         Args:
             filename (unicode):
                 The filename of the file being reviewed.
 
             file_contents (bytes):
                 File content to review.
 
@@ -289,27 +315,39 @@
             other_files (dict, optional):
                 Other files to write to the tree. Each will result in a new
                 file added to the review.
 
                 The dictionary is a map of file paths (relative to the
                 checkout directory) to byte strings.
 
+            file_contents_encoding (unicode, optional):
+                The encoding used for the provided file contents (both in
+                ``file_contents`` and ``other_contents``).
+
+                If not provided, this will be ``utf-8``.
+
+                Version Added:
+                    3.1.2
+
         Returns:
             tuple:
             A 2-tuple containing:
 
             1. The review (:py:class:`reviewbot.processing.review.Review)`
             2. The file entry corresponding to ``filename``
                (:py:class:`reviewbot.processing.review.File`)
 
             If ``other_files`` is specified, the second tuple item will
             instead be a dictionary of keys from ``other_files`` (along with
             ``filename``) to :py:class:`reviewbot.processing.review.File`
             instances.
         """
+        assert self.tool_class is not None
+        assert isinstance(file_contents, bytes)
+
         if self.tool_class.working_directory_required:
             repository = GitRepository(name='MyRepo',
                                        clone_path='git://example.com/repo')
             self.spy_on(repository.sync, call_original=False)
 
             @self.spy_for(repository.checkout)
             def _checkout(_self, *args, **kwargs):
@@ -320,32 +358,42 @@
         review = self.create_review()
         review_file = self.create_review_file(
             review,
             source_file=filename,
             dest_file=filename,
             diff_data=self.create_diff_data(chunks=[{
                 'change': 'insert',
-                'lines': file_contents.splitlines(),
+                'lines': (
+                    file_contents
+                    .decode(file_contents_encoding)
+                    .splitlines()
+                ),
                 'new_linenum': 1,
             }]),
             patched_content=file_contents)
 
         review_files = {}
 
         if other_files:
             review_files[filename] = review_file
 
             for other_filename, other_contents in six.iteritems(other_files):
+                assert isinstance(other_contents, bytes)
+
                 review_files[other_filename] = self.create_review_file(
                     review,
                     source_file=other_filename,
                     dest_file=other_filename,
                     diff_data=self.create_diff_data(chunks=[{
                         'change': 'insert',
-                        'lines': other_contents.splitlines(),
+                        'lines': (
+                            other_contents
+                            .decode(file_contents_encoding)
+                            .splitlines()
+                        ),
                         'new_linenum': 1,
                     }]),
                     patched_content=other_contents)
 
         worker_config = deepcopy(self.config)
         exe_paths = worker_config.setdefault('exe_paths', {})
         exe_paths.update({
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_base_tool.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_base_tool.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cargotool.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_cargotool.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,15 +335,16 @@
         " 0 filtered out; finished in 0.00s\n",
         "\n",
         "running 1 tests\n",
         "FF\n",
         "failures:\n",
         "\n",
         "---- tests::test1 stdout ----\n",
-        "thread 'main' panicked at 'assertion failed: `(left == right)`\n",
+        "thread 'tests::test1' panicked at 'assertion failed:"
+        " `(left == right)`\n",
         "  left: `1`,\n",
         " right: `2`', tests/test.rs:4:9\n",
         "note: run with `RUST_BACKTRACE=1` environment variable to display"
         " a backtrace\n",
         "\n",
         "\n",
         "failures:\n",
@@ -374,15 +375,15 @@
                 'issue_opened': True,
                 'rich_text': True,
                 'text': (
                     "1 test failed:\n"
                     "\n"
                     "```"
                     "---- tests::test1 stdout ----\n"
-                    "thread 'main' panicked at 'assertion failed: "
+                    "thread 'tests::test1' panicked at 'assertion failed: "
                     "`(left == right)`\n"
                     "  left: `1`,\n"
                     " right: `2`', tests/test.rs:4:9\n"
                     "\n"
                     "\n"
                     "failures:\n"
                     "    tests::test1"
@@ -416,22 +417,24 @@
         " 0 filtered out; finished in 0.00s\n",
         "\n",
         "running 2 tests\n",
         "FF\n",
         "failures:\n",
         "\n",
         "---- tests::test1 stdout ----\n",
-        "thread 'main' panicked at 'assertion failed: `(left == right)`\n",
+        "thread 'tests::test1' panicked at 'assertion failed:"
+        " `(left == right)`\n",
         "  left: `1`,\n",
         " right: `2`', tests/test.rs:4:9\n",
         "note: run with `RUST_BACKTRACE=1` environment variable to display"
         " a backtrace\n",
         "\n",
         "---- tests::test2 stdout ----\n",
-        "thread 'main' panicked at 'assertion failed: `(left == right)`\n",
+        "thread 'tests::test2' panicked at 'assertion failed:"
+        " `(left == right)`\n",
         "  left: `3`,\n",
         " right: `4`', tests/test.rs:9:9\n",
         "note: run with `RUST_BACKTRACE=1` environment variable to display"
         " a backtrace\n",
         "\n",
         "\n",
         "failures:\n",
@@ -463,21 +466,21 @@
                 'issue_opened': True,
                 'rich_text': True,
                 'text': (
                     "2 tests failed:\n"
                     "\n"
                     "```"
                     "---- tests::test1 stdout ----\n"
-                    "thread 'main' panicked at 'assertion failed: "
+                    "thread 'tests::test1' panicked at 'assertion failed: "
                     "`(left == right)`\n"
                     "  left: `1`,\n"
                     " right: `2`', tests/test.rs:4:9\n"
                     "\n"
                     "---- tests::test2 stdout ----\n"
-                    "thread 'main' panicked at 'assertion failed: "
+                    "thread 'tests::test2' panicked at 'assertion failed: "
                     "`(left == right)`\n"
                     "  left: `3`,\n"
                     " right: `4`', tests/test.rs:9:9\n"
                     "\n"
                     "\n"
                     "failures:\n"
                     "    tests::test1\n"
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_checkstyle.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_checkstyle.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_clang.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_clang.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cppcheck.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_cppcheck.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_cpplint.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_cpplint.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_doc8.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_doc8.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         """Testing Doc8Tool.execute with encoding setting"""
         review, review_file = self.run_tool_execute(
             filename='test.rst',
             file_contents=(
                 # This is: "*hi 🍎"
                 b'\xff\xfe*\x00h\x00i\x00 \x00<\xd8N\xdf'
             ),
+            file_contents_encoding='utf-16',
             tool_settings={
                 'encoding': 'utf-16',
                 'max_line_length': 79,
             })
 
         self.assertEqual(review.comments, [
             {
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_fbinfer.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_fbinfer.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_file_patterns_from_setting_mixin.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_file_patterns_from_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_flake8.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_flake8.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,20 +243,22 @@
 
         self.assertEqual(len(review.comments), 1)
         comment = review.comments[0]
 
         # Depending on the version of flake8, column indexes may be offset.
         # For wide version compatibility (given current support for Python 2
         # and compatible versions of flake8), this test needs to check both.
+        #
+        # We also may get an older "invalid syntax" or a newer "expected '('.
         self.assertRegex(
             comment.pop('text'),
-            'SyntaxError: invalid syntax\n'
-            '\n'
-            'Column: (9|10)\n'
-            'Error code: E999')
+            "SyntaxError: (invalid syntax|expected '\\(')\n"
+            "\n"
+            "Column: (9|10)\n"
+            "Error code: E999")
 
         self.assertEqual(comment, {
             'filediff_id': review_file.id,
             'first_line': 1,
             'num_lines': 1,
             'issue_opened': True,
             'rich_text': False,
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_gofmt.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_gofmt.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_gotool.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_gotool.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,28 +139,29 @@
             checkout_dir=self.checkout_dir,
             filename='mypackage/main.go',
             file_contents=self.SAMPLE_GO_CODE,
             tool_settings={
                 'test': True,
             })
 
-        self.assertEqual(review.general_comments, [
-            {
-                'text': (
-                    'TestThingie failed in the example.com/myrepo/mypackage '
-                    'package:\n'
-                    '\n'
-                    '```=== RUN   TestThingie\n'
-                    '    test_test.go:8: Fail!%!(EXTRA int=123)\n'
-                    '--- FAIL: TestThingie (0.00s)```'
-                ),
-                'issue_opened': True,
-                'rich_text': True,
-            },
-        ])
+        comments = review.general_comments
+        self.assertEqual(len(comments), 1)
+
+        comment = comments[0]
+        self.assertTrue(comment['issue_opened'])
+        self.assertTrue(comment['rich_text'])
+        self.assertRegex(
+            comment['text'],
+            'TestThingie failed in the example.com/myrepo/mypackage '
+            'package:\n'
+            '\n'
+            '```=== RUN   TestThingie\n'
+            '    test_test.go:8: Fail!%!\\(EXTRA int=123\\)\n'
+            '--- FAIL: TestThingie \\(\\d+\\.\\d+s\\)```')
+
         self.assertEqual(review.comments, [])
 
         self.assertSpyCalledWith(
             execute,
             [
                 self.tool_exe_path,
                 'test',
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_java_tool_mixin.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_java_tool_mixin.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_jshint.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_jshint.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pmd.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_pmd.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pycodestyle.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_rustfmt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,161 @@
-"""Unit tests for reviewbot.tools.pycodestyle."""
+"""Unit tests for reviewbot.tools.rustfmt."""
 
 from __future__ import unicode_literals
 
 import os
 
 import kgb
 import six
 
-from reviewbot.tools.pycodestyle import PycodestyleTool
+from reviewbot.tools.rustfmt import RustfmtTool
 from reviewbot.tools.testing import (BaseToolTestCase,
                                      ToolTestCaseMetaclass,
                                      integration_test,
                                      simulation_test)
 from reviewbot.utils.filesystem import tmpdirs
 from reviewbot.utils.process import execute
 
 
 @six.add_metaclass(ToolTestCaseMetaclass)
-class BasePycodestyleToolTests(BaseToolTestCase):
-    """Unit tests for reviewbot.tools.pycodestyle.PycodestyleTool."""
+class RustfmtToolTests(BaseToolTestCase):
+    """Unit tests for reviewbot.tools.rustfmt.RustfmtTool."""
 
-    tool_class = PycodestyleTool
-    tool_exe_config_key = 'pycodestyle'
-    tool_exe_path = '/path/to/pycodestyle'
+    tool_class = RustfmtTool
+    tool_exe_config_key = 'rustfmt'
+    tool_exe_path = '/path/to/rustfmt'
 
     @integration_test()
-    @simulation_test(output_payload=[
-        "E722:3:1:do not use bare 'except'",
-        "W601:6:5:.has_key() is deprecated, use 'in'",
-    ])
+    @simulation_test(stdout=(
+        'Diff in /test.rs at line 1:\n'
+        ' fn main() {\n'
+        '-println!("Hi")\n'
+        '+    println!("Hi")\n'
+        '}\n'
+    ))
     def test_execute(self):
-        """Testing PycodestyleTool.execute"""
+        """Testing RustfmtTool.execute"""
         review, review_file = self.run_tool_execute(
-            filename='test.py',
+            filename='test.rs',
             file_contents=(
-                b'try:\n'
-                b'    func()\n'
-                b'except:\n'
-                b'    pass\n'
-                b'\n'
-                b'if d.has_key():\n'
-                b'    pass\n'
-            ),
-            tool_settings={
-                'max_line_length': 79,
-            })
+                b'fn main() {\n'
+                b'println!("Hi")\n'
+                b'}\n'
+            ))
 
         self.assertEqual(review.comments, [
             {
                 'filediff_id': review_file.id,
-                'first_line': 3,
+                'first_line': 1,
                 'num_lines': 1,
                 'text': (
-                    "do not use bare 'except'\n"
-                    "\n"
-                    "Column: 1\n"
-                    "Error code: E722"
+                    'This file contains formatting errors and should be run '
+                    'through `rustfmt`.'
                 ),
                 'issue_opened': True,
-                'rich_text': False,
-            },
-            {
-                'filediff_id': review_file.id,
-                'first_line': 6,
-                'num_lines': 1,
-                'text': (
-                    ".has_key() is deprecated, use 'in'\n"
-                    "\n"
-                    "Column: 5\n"
-                    "Error code: W601"
-                ),
-                'issue_opened': True,
-                'rich_text': False,
+                'rich_text': True,
             },
         ])
 
         self.assertSpyCalledWith(
             execute,
             [
                 self.tool_exe_path,
-                '--max-line-length=79',
-                '--format=%(code)s:%(row)d:%(col)d:%(text)s',
-                os.path.join(tmpdirs[-1], 'test.py'),
+                '-q',
+                '--check',
+                '--color=never',
+                os.path.join(tmpdirs[-1], 'test.rs'),
             ],
-            ignore_errors=True)
+            ignore_errors=True,
+            return_errors=True)
 
     @integration_test()
-    @simulation_test(output_payload=[
-        "W601:6:5:.has_key() is deprecated, use 'in'",
-    ])
-    def test_execute_with_ignore(self):
-        """Testing PycodestyleTool.execute with ignore"""
+    @simulation_test(stderr=(
+        'error: this file contains an unclosed delimiter\n'
+        ' --> /test.rs:2:27\n'
+        '  |\n'
+        '1 | afn main() {\n'
+        '               - unclosed delimiter\n'
+        '2 | println!("Hello world!");\n'
+        '  |                           ^\n'
+        '\n'
+        'error: expected one of `!` or `::`, found `main`\n'
+        ' --> /test.rs:1:6\n'
+        '  |\n'
+        '1 | afn main() {\n'
+        '  |     ^^^^ expected one of `!` or `::`\n'
+    ))
+    def test_execute_with_syntax_error(self):
+        """Testing RustfmtTool.execute with syntax error"""
         review, review_file = self.run_tool_execute(
-            filename='test.py',
+            filename='test.rs',
             file_contents=(
-                b'try:\n'
-                b'    func()\n'
-                b'except:\n'
-                b'    pass\n'
-                b'\n'
-                b'if d.has_key():\n'
-                b'    pass\n'
-            ),
-            tool_settings={
-                'max_line_length': 79,
-                'ignore': 'W123,E722',
-            })
+                b'func main() {}\n'
+            ))
 
         self.assertEqual(review.comments, [
             {
                 'filediff_id': review_file.id,
-                'first_line': 6,
+                'first_line': 1,
                 'num_lines': 1,
                 'text': (
-                    ".has_key() is deprecated, use 'in'\n"
-                    "\n"
-                    "Column: 5\n"
-                    "Error code: W601"
+                    'expected one of `!` or `::`, found `main`\n'
+                    '\n'
+                    'Column: 6'
                 ),
                 'issue_opened': True,
                 'rich_text': False,
             },
         ])
 
         self.assertSpyCalledWith(
             execute,
             [
                 self.tool_exe_path,
-                '--max-line-length=79',
-                '--format=%(code)s:%(row)d:%(col)d:%(text)s',
-                '--ignore=W123,E722',
-                os.path.join(tmpdirs[-1], 'test.py'),
+                '-q',
+                '--check',
+                '--color=never',
+                os.path.join(tmpdirs[-1], 'test.rs'),
             ],
-            ignore_errors=True)
+            ignore_errors=True,
+            return_errors=True)
 
-    def setup_simulation_test(self, output_payload):
-        """Set up the simulation test for pycodestyle.
+    @integration_test()
+    @simulation_test()
+    def test_execute_with_success(self):
+        """Testing RustfmtTool.execute with no errors"""
+        review, review_file = self.run_tool_execute(
+            filename='test.rs',
+            file_contents=(
+                b'fn main() {\n'
+                b'    println!("Hello world!");\n'
+                b'}\n'
+            ))
+
+        self.assertEqual(review.comments, [])
+
+        self.assertSpyCalledWith(
+            execute,
+            [
+                self.tool_exe_path,
+                '-q',
+                '--check',
+                '--color=never',
+                os.path.join(tmpdirs[-1], 'test.rs'),
+            ],
+            ignore_errors=True,
+            return_errors=True)
+
+    def setup_simulation_test(self, stdout='', stderr=''):
+        """Set up the simulation test for rustfmt.
 
         This will spy on :py:func:`~reviewbot.utils.process.execute`, making
-        it return the provided payload.
+        it return the provided stdout and stderr results.
 
         Args:
-            output_payload (dict):
-                The outputted payload.
+            stdout (unicode, optional):
+                The outputted stdout.
+
+            stderr (unicode, optional):
+                The outputted stderr.
         """
-        self.spy_on(execute, op=kgb.SpyOpReturn(output_payload))
+        self.spy_on(execute, op=kgb.SpyOpReturn((stdout, stderr)))
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pydocstyle.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_pydocstyle.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_pyflakes.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_pyflakes.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rbsecretscanner.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_rbsecretscanner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Unit tests for reviewbot.tools.rbsecretscanner."""
 
 from __future__ import unicode_literals
 
+import kgb
 import six
 
 from reviewbot.tools.rbsecretscanner import SecretScannerTool
 from reviewbot.tools.testing import (BaseToolTestCase,
                                      ToolTestCaseMetaclass,
                                      integration_test)
 from reviewbot.utils.process import execute
 
 
 @six.add_metaclass(ToolTestCaseMetaclass)
-class SecretScannerToolTests(BaseToolTestCase):
+class SecretScannerToolTests(BaseToolTestCase, kgb.SpyAgency):
     """Unit tests for SecretScannerTool."""
 
     tool_class = SecretScannerTool
 
     def test_get_can_handle_file(self):
         """Testing SecretScannerTool.get_can_handle_file"""
         self.assertTrue(self.run_get_can_handle_file(filename='test.txt'))
@@ -206,14 +207,16 @@
         # Upper bounds of length.
         self._run_token_test(
             'GITHUB_TOKEN=1234567890ABCDEFGabcdefg12345XYZxyz12345')
 
     @integration_test()
     def test_execute_with_github_oauth_token_gho(self):
         """Testing SecretScannerTool.execute with GitHub token (gho...)"""
+        self.spy_on(self.tool_class._is_github_modern_token_valid)
+
         # Lower bounds of length.
         self._run_token_test(
             'gho_1234567890ABCDEFGabcdefg1234508vKGb')
 
         # Upper bounds of length.
         self._run_token_test(
             'gho_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
@@ -230,17 +233,32 @@
         self._run_token_test(
             'Zgho_1234567890ABCDEFGabcdefg1234508vKGb',
             match=False)
         self._run_token_test(
             'gho_1234567890ABCDEFGabcdefg1234508vKGbZ',
             match=False)
 
+        # No match because checksum does not match.
+        self._run_token_test(
+            'gho_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
+            'bcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890'
+            'abcdef1234567890abcdef1234567890abcdef1234567890abcdef123456789'
+            '0abcdef1234567890abcdef1234567890abcdef1234567890abcdef123451X8'
+            '8Ax',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_github_modern_token_valid,
+            5)
+
     @integration_test()
     def test_execute_with_github_oauth_token_ghp(self):
         """Testing SecretScannerTool.execute with GitHub token (ghp...)"""
+        self.spy_on(self.tool_class._is_github_modern_token_valid)
+
         # Lower bounds of length.
         self._run_token_test(
             'ghp_1234567890ABCDEFGabcdefg1234508vKGb')
 
         # Upper bounds of length.
         self._run_token_test(
             'ghp_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
@@ -257,17 +275,32 @@
         self._run_token_test(
             'Zghp_1234567890ABCDEFGabcdefg1234508vKGb',
             match=False)
         self._run_token_test(
             'ghp_1234567890ABCDEFGabcdefg1234508vKGbZ',
             match=False)
 
+        # No match because checksum does not match.
+        self._run_token_test(
+            'ghp_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
+            'bcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890'
+            'abcdef1234567890abcdef1234567890abcdef1234567890abcdef123456789'
+            '0abcdef1234567890abcdef1234567890abcdef1234567890abcdef123451X8'
+            '8Ax',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_github_modern_token_valid,
+            5)
+
     @integration_test()
     def test_execute_with_github_oauth_token_ghr(self):
         """Testing SecretScannerTool.execute with GitHub token (ghr...)"""
+        self.spy_on(self.tool_class._is_github_modern_token_valid)
+
         # Lower bounds of length.
         self._run_token_test(
             'ghr_1234567890ABCDEFGabcdefg1234508vKGb')
 
         # Upper bounds of length.
         self._run_token_test(
             'ghr_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
@@ -284,17 +317,32 @@
         self._run_token_test(
             'Zghr_1234567890ABCDEFGabcdefg1234508vKGb',
             match=False)
         self._run_token_test(
             'ghr_1234567890ABCDEFGabcdefg1234508vKGbZ',
             match=False)
 
+        # No match because checksum does not match.
+        self._run_token_test(
+            'ghr_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
+            'bcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890'
+            'abcdef1234567890abcdef1234567890abcdef1234567890abcdef123456789'
+            '0abcdef1234567890abcdef1234567890abcdef1234567890abcdef123451X8'
+            '8Ax',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_github_modern_token_valid,
+            5)
+
     @integration_test()
     def test_execute_with_github_oauth_token_ghs(self):
         """Testing SecretScannerTool.execute with GitHub token (ghs...)"""
+        self.spy_on(self.tool_class._is_github_modern_token_valid)
+
         # Lower bounds of length.
         self._run_token_test(
             'ghs_1234567890ABCDEFGabcdefg1234508vKGb')
 
         # Upper bounds of length.
         self._run_token_test(
             'ghs_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
@@ -311,17 +359,32 @@
         self._run_token_test(
             'Zghs_1234567890ABCDEFGabcdefg1234508vKGb',
             match=False)
         self._run_token_test(
             'ghs_1234567890ABCDEFGabcdefg1234508vKGbZ',
             match=False)
 
+        # No match because checksum does not match.
+        self._run_token_test(
+            'ghs_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
+            'bcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890'
+            'abcdef1234567890abcdef1234567890abcdef1234567890abcdef123456789'
+            '0abcdef1234567890abcdef1234567890abcdef1234567890abcdef123451X8'
+            '8Ax',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_github_modern_token_valid,
+            5)
+
     @integration_test()
     def test_execute_with_github_oauth_token_ghu(self):
         """Testing SecretScannerTool.execute with GitHub token (ghu...)"""
+        self.spy_on(self.tool_class._is_github_modern_token_valid)
+
         # Lower bounds of length.
         self._run_token_test(
             'ghu_1234567890ABCDEFGabcdefg1234508vKGb')
 
         # Upper bounds of length.
         self._run_token_test(
             'ghu_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
@@ -338,14 +401,27 @@
         self._run_token_test(
             'Zghu_1234567890ABCDEFGabcdefg1234508vKGb',
             match=False)
         self._run_token_test(
             'ghu_1234567890ABCDEFGabcdefg1234508vKGbZ',
             match=False)
 
+        # No match because checksum does not match.
+        self._run_token_test(
+            'ghu_1234567890abcdef1234567890abcdef1234567890abcdef1234567890a'
+            'bcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890'
+            'abcdef1234567890abcdef1234567890abcdef1234567890abcdef123456789'
+            '0abcdef1234567890abcdef1234567890abcdef1234567890abcdef123451X8'
+            '8Ax',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_github_modern_token_valid,
+            5)
+
     @integration_test()
     def test_execute_with_google_gcp_api_key(self):
         """Testing SecretScannerTool.execute with Google GCP API Key"""
         self._run_token_test('ABCDEFGabcdefg123456789ZYXWzywxSTUVstuv')
         self._run_token_test('ZABCDEFGabcdefg123456789ZYXWzywxSTUVstuv',
                              match=False)
         self._run_token_test('ABCDEFGabcdefg123456789ZYXWzywxSTUVstuvZ',
@@ -379,14 +455,16 @@
         """Testing SecretScannerTool.execute with Heroku API Key"""
         self._run_token_test(
             'HEROKU_API_KEY=1234abcd-12ab-34cd-56ef-123456abcdef')
 
     @integration_test()
     def test_execute_with_json_web_token(self):
         """Testing SecretScannerTool.execute with JSON Web Token"""
+        self.spy_on(self.tool_class._is_json_web_token_valid)
+
         self._run_token_test(
             'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJrZXkiOiJ2YWx1ZSJ9.'
             '5pps1XMxciBCpOhezqTk9XuGny-4_HZ9aEKp3AqgekA')
         self._run_token_test(
             'W10K.eyJrZXkiOiJ2YWx1ZSJ9.8nUniKZ63ZQLtj401tAGgVLo0Fm1LAOe'
             'M5vPSBY3-os',
             match=False)
@@ -394,14 +472,18 @@
             'eyJ0eXAiOiAib3RoZXIifQo=.eyJrZXkiOiJ2YWx1ZSJ9.'
             '8nUniKZ63ZQLtj401tAGgVLo0Fm1LAOeM5vPSBY3-os',
             match=False)
         self._run_token_test(
             'foo.bar.baz',
             match=False)
 
+        self.assert_spy_call_count(
+            self.tool_class._is_json_web_token_valid,
+            4)
+
     @integration_test()
     def test_execute_with_mailchimp_api_key(self):
         """Testing SecretScannerTool.execute with Mailchimp API key"""
         self._run_token_test('abcdef1234567890abcdef1234567890-us1')
         self._run_token_test('abcdef1234567890abcdef1234567890-us12')
         self._run_token_test('Zabcdef1234567890abcdef1234567890-us12',
                              match=False)
@@ -440,14 +522,58 @@
             'UVWXYZ_0123456789_abcdefghijklmnopqrstuvwxyz')
         self._run_token_test(
             'pypi:abcdefghijklmnopqrstuvwxyz_ABCDEFGHIJKLMNOPQRSTUVWXYZ_'
             '0123456789_abcdefghijklmnopqrstuvwxyz_ABCDEFGHIJKLMNOPQRST'
             'UVWXYZ_0123456789_abcdefghijklmnopqrstuvwxyz')
 
     @integration_test()
+    def test_execute_with_reviewboard_api_token(self):
+        """Testing SecretScannerTool.execute with Review Board API Token"""
+        self.spy_on(self.tool_class._is_reviewboard_api_token_valid)
+
+        self._run_token_test(
+            'rbp_eVZF8sv33KEWtMuupDJeipmW566fRZHveuAC7MchaktaJNTBQ4eNqhBQJKIv'
+            '6iKQJL64s8yMWfzp1Buc8p9m9ItCnkvNKTVuMJM299H7zffcrUJ0PQaSVSG0aUhg'
+            'zzwIZ0MtK9spxYTLtu8bBVoQEiAsbDSfYICdKx23PfphGGqHyTwZRvYaebe1gGbv'
+            'KgZ3PT8HqNQRAnAbUsDjwm4oiXXlmNOSM84a1uACZ2DCm9frU9z32pzHs4Ss9cI')
+
+        # A Review Board 5.0.0 token whose checksum has the incorrect
+        # base62-encoding.
+        self._run_token_test(
+            'rbp_eVZF8sv33KEWtMuupDJeipmW566fRZHveuAC7MchaktaJNTBQ4eNqhBQJKIv'
+            '6iKQJL64s8yMWfzp1Buc8p9m9ItCnkvNKTVuMJM299H7zffcrUJ0PQaSVSG0aUhg'
+            'zzwIZ0MtK9spxYTLtu8bBVoQEiAsbDSfYICdKx23PfphGGqHyTwZRvYaebe1gGbv'
+            'KgZ3PT8HqNQRAnAbUsDjwm4oiXXlmNOSM84a1uACZ2DCm9frU9z32pzHs4sS9Ci')
+
+        self._run_token_test(
+            '!rbp_eVZF8sv33KEWtMuupDJeipmW566fRZHveuAC7MchaktaJNTBQ4eNqhBQJKI'
+            '6iKQJL64s8yMWfzp1Buc8p9m9ItCnkvNKTVuMJM299H7zffcrUJ0PQaSVSG0aUhg'
+            'zzwIZ0MtK9spxYTLtu8bBVoQEiAsbDSfYICdKx23PfphGGqHyTwZRvYaebe1gGbv'
+            'KgZ3PT8HqNQRAnAbUsDjwm4oiXXlmNOSM84a1uACZ2DCm9frU9z32pzHs4sS9Ci',
+            match=False)
+        self._run_token_test(
+            'rbp_eVZF8sv33KEWtMuupDJeipmW566fRZHveuAC7MchaktaJNTBQ4eNqhBQJKIv'
+            '6iKQJL64s8yMWfzp1Buc8p9m9ItCnkvNKTVuMJM299H7zffcrUJ0PQaSVSG0aUhg'
+            'zzwIZ0MtK9spxYTLtu8bBVoQEiAsbDSfYICdKx23PfphGGqHyTwZRvYaebe1gGbv'
+            'KgZ3PT8HqNQRAnAbUsDjwm4oiXXlmNOSM84a1uACZ2DCm9frU9z32pzHs4sS9C!',
+            match=False)
+
+        # No match because checksum does not match.
+        self._run_token_test(
+            'rbp_eVZF8sv33KEWtMuupDJeipmW566fRZHveuAC7MchaktaJNTBQ4eNqhBQJKIv'
+            '6iKQJL64s8yMWfzp1Buc8p9m9ItCnkvNKTVuMJM299H7zffcrUJ0PQaSVSG0aUhg'
+            'zzwIZ0MtK9spxYTLtu8bBVoQEiAsbDSfYICdKx23PfphGGqHyTwZRvYaebe1gGbv'
+            'KgZ3PT8HqNQRAnAbUsDjwm4oiXXlmNOSM84a1uACZ2DCm9frU9z32pzHs4sS9Cb',
+            match=False)
+
+        self.assert_spy_call_count(
+            self.tool_class._is_reviewboard_api_token_valid,
+            3)
+
+    @integration_test()
     def test_execute_with_rsa_private_key(self):
         """Testing SecretScannerTool.execute with RSA Private Key"""
         self._run_token_test('----BEGIN RSA PRIVATE KEY----')
 
     @integration_test()
     def test_execute_with_ssh_dsa_private_key(self):
         """Testing SecretScannerTool.execute with SSH (DSA) Private Key"""
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_registry.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rubocop.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_rubocop.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_rustfmt.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_pycodestyle.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,145 @@
-"""Unit tests for reviewbot.tools.rustfmt."""
+"""Unit tests for reviewbot.tools.pycodestyle."""
 
 from __future__ import unicode_literals
 
 import os
 
 import kgb
 import six
 
-from reviewbot.tools.rustfmt import RustfmtTool
+from reviewbot.tools.pycodestyle import PycodestyleTool
 from reviewbot.tools.testing import (BaseToolTestCase,
                                      ToolTestCaseMetaclass,
                                      integration_test,
                                      simulation_test)
 from reviewbot.utils.filesystem import tmpdirs
 from reviewbot.utils.process import execute
 
 
 @six.add_metaclass(ToolTestCaseMetaclass)
-class RustfmtToolTests(BaseToolTestCase):
-    """Unit tests for reviewbot.tools.rustfmt.RustfmtTool."""
+class BasePycodestyleToolTests(BaseToolTestCase):
+    """Unit tests for reviewbot.tools.pycodestyle.PycodestyleTool."""
 
-    tool_class = RustfmtTool
-    tool_exe_config_key = 'rustfmt'
-    tool_exe_path = '/path/to/rustfmt'
+    tool_class = PycodestyleTool
+    tool_exe_config_key = 'pycodestyle'
+    tool_exe_path = '/path/to/pycodestyle'
 
     @integration_test()
-    @simulation_test(stdout=(
-        'Diff in /test.rs at line 1:\n'
-        ' fn main() {\n'
-        '-println!("Hi")\n'
-        '+    println!("Hi")\n'
-        '}\n'
-    ))
+    @simulation_test(output_payload=[
+        "E401:1:10:multiple imports on one line",
+        "E722:5:1:do not use bare 'except'",
+    ])
     def test_execute(self):
-        """Testing RustfmtTool.execute"""
+        """Testing PycodestyleTool.execute"""
         review, review_file = self.run_tool_execute(
-            filename='test.rs',
+            filename='test.py',
             file_contents=(
-                b'fn main() {\n'
-                b'println!("Hi")\n'
-                b'}\n'
-            ))
+                b'import os, sys\n'
+                b'\n'
+                b'try:\n'
+                b'    func()\n'
+                b'except:\n'
+                b'    pass\n'
+            ),
+            tool_settings={
+                'max_line_length': 79,
+            })
 
         self.assertEqual(review.comments, [
             {
                 'filediff_id': review_file.id,
                 'first_line': 1,
                 'num_lines': 1,
                 'text': (
-                    'This file contains formatting errors and should be run '
-                    'through `rustfmt`.'
+                    'multiple imports on one line\n'
+                    '\n'
+                    'Column: 10\n'
+                    'Error code: E401'
                 ),
                 'issue_opened': True,
-                'rich_text': True,
+                'rich_text': False,
+            },
+            {
+                'filediff_id': review_file.id,
+                'first_line': 5,
+                'num_lines': 1,
+                'text': (
+                    "do not use bare 'except'\n"
+                    "\n"
+                    "Column: 1\n"
+                    "Error code: E722"
+                ),
+                'issue_opened': True,
+                'rich_text': False,
             },
         ])
 
         self.assertSpyCalledWith(
             execute,
             [
                 self.tool_exe_path,
-                '-q',
-                '--check',
-                '--color=never',
-                os.path.join(tmpdirs[-1], 'test.rs'),
+                '--max-line-length=79',
+                '--format=%(code)s:%(row)d:%(col)d:%(text)s',
+                os.path.join(tmpdirs[-1], 'test.py'),
             ],
-            ignore_errors=True,
-            return_errors=True)
+            ignore_errors=True)
 
     @integration_test()
-    @simulation_test(stderr=(
-        'error: this file contains an unclosed delimiter\n'
-        ' --> /test.rs:2:27\n'
-        '  |\n'
-        '1 | afn main() {\n'
-        '               - unclosed delimiter\n'
-        '2 | println!("Hello world!");\n'
-        '  |                           ^\n'
-        '\n'
-        'error: expected one of `!` or `::`, found `main`\n'
-        ' --> /test.rs:1:6\n'
-        '  |\n'
-        '1 | afn main() {\n'
-        '  |     ^^^^ expected one of `!` or `::`\n'
-    ))
-    def test_execute_with_syntax_error(self):
-        """Testing RustfmtTool.execute with syntax error"""
+    @simulation_test(output_payload=[
+        "E401:1:10:multiple imports on one line",
+    ])
+    def test_execute_with_ignore(self):
+        """Testing PycodestyleTool.execute with ignore"""
         review, review_file = self.run_tool_execute(
-            filename='test.rs',
+            filename='test.py',
             file_contents=(
-                b'func main() {}\n'
-            ))
+                b'import os, sys\n'
+                b'\n'
+                b'try:\n'
+                b'    func()\n'
+                b'except:\n'
+                b'    pass\n'
+            ),
+            tool_settings={
+                'max_line_length': 79,
+                'ignore': 'W123,E722',
+            })
 
         self.assertEqual(review.comments, [
             {
                 'filediff_id': review_file.id,
                 'first_line': 1,
                 'num_lines': 1,
                 'text': (
-                    'expected one of `!` or `::`, found `main`\n'
+                    'multiple imports on one line\n'
                     '\n'
-                    'Column: 6'
+                    'Column: 10\n'
+                    'Error code: E401'
                 ),
                 'issue_opened': True,
                 'rich_text': False,
             },
         ])
 
         self.assertSpyCalledWith(
             execute,
             [
                 self.tool_exe_path,
-                '-q',
-                '--check',
-                '--color=never',
-                os.path.join(tmpdirs[-1], 'test.rs'),
-            ],
-            ignore_errors=True,
-            return_errors=True)
-
-    @integration_test()
-    @simulation_test()
-    def test_execute_with_success(self):
-        """Testing RustfmtTool.execute with no errors"""
-        review, review_file = self.run_tool_execute(
-            filename='test.rs',
-            file_contents=(
-                b'fn main() {\n'
-                b'    println!("Hello world!");\n'
-                b'}\n'
-            ))
-
-        self.assertEqual(review.comments, [])
-
-        self.assertSpyCalledWith(
-            execute,
-            [
-                self.tool_exe_path,
-                '-q',
-                '--check',
-                '--color=never',
-                os.path.join(tmpdirs[-1], 'test.rs'),
+                '--max-line-length=79',
+                '--format=%(code)s:%(row)d:%(col)d:%(text)s',
+                '--ignore=W123,E722',
+                os.path.join(tmpdirs[-1], 'test.py'),
             ],
-            ignore_errors=True,
-            return_errors=True)
+            ignore_errors=True)
 
-    def setup_simulation_test(self, stdout='', stderr=''):
-        """Set up the simulation test for rustfmt.
+    def setup_simulation_test(self, output_payload):
+        """Set up the simulation test for pycodestyle.
 
         This will spy on :py:func:`~reviewbot.utils.process.execute`, making
-        it return the provided stdout and stderr results.
+        it return the provided payload.
 
         Args:
-            stdout (unicode, optional):
-                The outputted stdout.
-
-            stderr (unicode, optional):
-                The outputted stderr.
+            output_payload (dict):
+                The outputted payload.
         """
-        self.spy_on(execute, op=kgb.SpyOpReturn((stdout, stderr)))
+        self.spy_on(execute, op=kgb.SpyOpReturn(output_payload))
```

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/tests/test_shellcheck.py` & `reviewbot-worker-3.2/reviewbot/tools/tests/test_shellcheck.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/tools/utils/codeclimate.py` & `reviewbot-worker-3.2/reviewbot/tools/utils/codeclimate.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/api.py` & `reviewbot-worker-3.2/reviewbot/utils/api.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/filesystem.py` & `reviewbot-worker-3.2/reviewbot/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/log.py` & `reviewbot-worker-3.2/reviewbot/utils/log.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/process.py` & `reviewbot-worker-3.2/reviewbot/utils/process.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/tests/test_filesystem.py` & `reviewbot-worker-3.2/reviewbot/utils/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/tests/test_process.py` & `reviewbot-worker-3.2/reviewbot/utils/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/tests/test_text.py` & `reviewbot-worker-3.2/reviewbot/utils/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot/utils/text.py` & `reviewbot-worker-3.2/reviewbot/utils/text.py`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot_worker.egg-info/PKG-INFO` & `reviewbot-worker-3.2/reviewbot_worker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviewbot-worker
-Version: 3.1.1
+Version: 3.2
 Summary: Review Bot, the automated code reviewer (worker)
 Author: Beanbag, Inc.
 Author-email: support@beanbaginc.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: support@beanbaginc.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reviewbot-worker-3.1.1/reviewbot_worker.egg-info/SOURCES.txt` & `reviewbot-worker-3.2/reviewbot_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/reviewbot_worker.egg-info/entry_points.txt` & `reviewbot-worker-3.2/reviewbot_worker.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `reviewbot-worker-3.1.1/setup.py` & `reviewbot-worker-3.2/setup.py`

 * *Files identical despite different names*

