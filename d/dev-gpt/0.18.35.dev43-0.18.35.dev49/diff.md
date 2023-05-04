# Comparing `tmp/dev-gpt-0.18.35.dev43.tar.gz` & `tmp/dev-gpt-0.18.35.dev49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.35.dev43.tar", last modified: Thu May  4 15:53:23 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.35.dev49.tar", last modified: Thu May  4 18:47:47 2023, max compression
```

## Comparing `dev-gpt-0.18.35.dev43.tar` & `dev-gpt-0.18.35.dev49.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.199991 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:53:23.000000 dev-gpt-0.18.35.dev43/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/gptdeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 15:53:22.000000 dev-gpt-0.18.35.dev43/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29645 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.199991 dev-gpt-0.18.35.dev43/src/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.203992 dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/src/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/src/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:23.207991 dev-gpt-0.18.35.dev43/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 15:53:15.000000 dev-gpt-0.18.35.dev43/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.543457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.35.dev43/LICENSE` & `dev-gpt-0.18.35.dev49/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/PKG-INFO` & `dev-gpt-0.18.35.dev49/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,465 +1,446 @@
-Metadata-Version: 2.1
-Name: dev-gpt
-Version: 0.18.35.dev43
-Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
-Home-page: https://github.com/jina-ai/gptdeploy
-Author: Florian Hönicke
-Author-email: florian.hoenicke@jina.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
-GPT Deploy: One line to generate them all 🧙🚀
+Dev GPT : One line to generate them all 🧙🚀
 </h1>
 
 <p align="center">
-<img src="res/gpt-deploy-logo.png" alt="Jina NOW logo" width="150px">
+<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
 </p>
 <p align="center">
 Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
 <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/fastapi" target="_blank">
     <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/fastapi.svg" alt="Coverage">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/gptdeploy?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/v/dev-gpt?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/gptdeploy.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/dev-gpt.svg?color=%2334D058" alt="Supported Python versions">
 </a>
-<a href="https://github.com/tiangolo/gptdeploy/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
+<a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
-<a href="https://pypistats.org/packages/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/dm/gptdeploy?color=%2334D058&label=pypi%20downloads" alt="Downloads">
+<a href="https://pypistats.org/packages/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 
-[![Watch the video](res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)
+[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
 </p>
 This project streamlines the creation and deployment of AI-powered microservices. 
 Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-To ensure the microservice accurately aligns with your intended task a test scenario is required.
+You get guidance from our three agents:
+
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
 ```bash
-pip install gptdeploy
-gptdeploy configure --key <your openai api key>
+pip install dev-gpt
+dev-gpt configure --key <your openai api key>
 ```
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ### Generate Microservice
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
 To generate your personal microservice two things are required:
 - A `description` of the task you want to accomplish. (optional)
 - The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x cheaper, 
 but will not be able to generate as complex microservices. (default: largest you have access to)
 - A `path` on the local drive where the microservice will be generated. (default: ./microservice)
 
 The creation process should take between 5 and 15 minutes.
 During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
 
-Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice (using GPT-4).
+Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo.
 
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
-gptdeploy run --path <path to microservice>
+dev-gpt run --path <path to microservice>
 ```
 
 
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
-gptdeploy deploy --microservice_path <path to microservice>
+dev-gpt deploy --microservice_path <path to microservice>
 ```
 
 
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
 ## Examples
-In this section you can get a feeling for the kind of microservices that can be generated with GPT Deploy.
+In this section you can get a feeling for the kind of microservices that can be generated with Dev-GPT.
 
 ### Compliment Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
 
 ### Extract and summarize news articles given a URL
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
 
 ### Chemical Formula Visualization
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert a chemical formula into a 2D chemical structure diagram. Example inputs: C=C, CN=C=O, CCC(=O)O" \
 --model gpt-4
 ```
 <img src="res/chemical_formula_example.png" alt="Chemical Formula Visualization" width="400" />
 
 ### 2d rendering of 3d model
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "create a 2d rendering of a whole 3d object and x,y,z object rotation using trimesh and pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https://graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \
 --model gpt-4
 ```
 <img src="res/obj_render_example.gif" alt="2D Rendering of 3D Model" width="400" />
 
 ### Product Recommendation
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate personalized product recommendations based on user product browsing history and the product categories fashion, electronics and sport. Example: Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \
 --model gpt-4
 ```
 <img src="res/recommendation_example.png" alt="Product Recommendation" width="400" />
 
 ### Hacker News Search
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a search query, find articles on hacker news using the hacker news api and return a list of (title, author, website_link, first_image_on_the_website)" \
 --model gpt-4
 ````
 <img src="res/hacker_news_example.png" alt="Hacker News Search" width="400" />
 
 ### Animal Detector
 ```bash
 
-gptdeploy generate \
+dev-gpt generate \
 --description "Given an image, return the image with bounding boxes of all animals (https://pjreddie.com/media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \
 --model gpt-4
 ```
 <img src="res/animal_detector_example.png" alt="Animal Detector" width="400" />
 
 ### Meme Generator
 ```bash
-gptdeploy generate \
---description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \
+dev-gpt generate \
+--description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \
 --model gpt-4
 ```
 <img src="res/meme_example.png" alt="Meme Generator" width="400" />
 
 ### Rhyme Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a word, return a list of rhyming words using the datamuse api" \
 --model gpt-4
 ```
 <img src="res/rhyme_generator_example.png" alt="Rhyme Generator" width="400" />
 
 ### Word Cloud Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate a word cloud from a given text" \
 --model gpt-4
 ```
 <img src="res/word_cloud_example.png" alt="Word Cloud Generator" width="400" />
 
 ### 3d model info
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a 3d object, return vertex count and face count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj" \
 --model gpt-4
 ```
 <img src="res/obj_info_example.png" alt="3D Model Info" width="400" />
 
 ### Table extraction
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a URL, extract all tables as csv. Example: http://www.ins.tn/statistiques/90" \
 --model gpt-4
 ```
 <img src="res/table_extraction_example.png" alt="Table Extraction" width="400" />
 
 ### Audio to mel spectrogram
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create mel spectrogram from audio file. Example: https://cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \
 --model gpt-4
 ```
 <img src="res/audio_to_mel_example.png" alt="Audio to Mel Spectrogram" width="400" />
 
 ### Text to speech
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert text to speech" \
 --model gpt-4
 ```
 <a href=res/text_to_speech_example.wav><img src="res/text_to_speech_example.png" alt="Text to Speech" width="400" /></a>
 
 <audio controls>
   <source src="res/text_to_speech_example.wav" type="audio/mpeg">
   Your browser does not support the audio element.
 </audio>
 
 ### Heatmap Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create a heatmap from an image and a list of relative coordinates. Example input: https://images.unsplash.com/photo-1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1], [0.7, 0.2], [0.4, 0.2]]" \
 --model gpt-4
 ```
 <img src="res/heatmap_example.png" alt="Heatmap Generator" width="400" />
 
 ### QR Code Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate QR code from URL. Example input: https://www.example.com" \
 --model gpt-4 
 ```
 <img src="res/qr_example.png" alt="QR Code Generator" width="400" />
 
 ### Mandelbrot Set Visualizer
 
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Visualize the Mandelbrot set with custom parameters. Example input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \
 --model gpt-4
 ```
 <img src="res/mandelbrot_example.png" alt="Mandelbrot Set Visualizer" width="400" />
 
 
 ### Markdown to HTML Converter
 
 ```bash
-gptdeploy generate --description "Convert markdown to HTML"
+dev-gpt generate --description "Convert markdown to HTML"
 ```
 
 <img src="res/markdown_to_html_example.png" alt="Markdown to HTML Converter" width="400" />
 
 
 
 [//]: # (## TO BE TESTED)
 
 
 [//]: # (### Password Strength Checker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
+[//]: # (dev-gpt generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
 
 [//]: # (```)
 
 [//]: # (### Morse Code Translator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert text to morse code" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Convert text to morse code" --test "Hello, welcome to GPT Dev!")
 
 [//]: # (```)
 
 [//]: # (### IP Geolocation)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
+[//]: # (dev-gpt generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
 
 [//]: # (```)
 
 [//]: # (### Currency Converter)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Converts any currency into any other" --test "1 usd to eur")
+[//]: # (dev-gpt generate --description "Converts any currency into any other" --test "1 usd to eur")
 
 [//]: # (```)
 
 [//]: # (### Image Resizer)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (### Weather API)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a city, return the current weather" --test "Berlin")
+[//]: # (dev-gpt generate --description "Given a city, return the current weather" --test "Berlin")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Sudoku Solver)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
+[//]: # (dev-gpt generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Carbon Footprint Calculator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
+[//]: # (dev-gpt generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Real Estate Valuation Estimator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
+[//]: # (dev-gpt generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gene Sequence Alignment)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
+[//]: # (dev-gpt generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Barcode Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a barcode from a string" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Generate a barcode from a string" --test "Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Compression)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Watermarking Images)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Add a watermark &#40;GPT Deploy&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Add a watermark &#40;Dev-GPT&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Metadata Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Video Thumbnail Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
+[//]: # (dev-gpt generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gif Maker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
+[//]: # (dev-gpt generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
 
 [//]: # (```)
 
 [//]: # ()
 
 [//]: # ()
 
 [//]: # (### Sound Visualizer)
 
 [//]: # ()
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
+[//]: # (dev-gpt generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
 
 [//]: # (```)
 
 [//]: # (## Upcoming Challenges)
 
 [//]: # (### Color Palette Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
+[//]: # (dev-gpt generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Depth Map Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
+[//]: # (dev-gpt generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
 
 [//]: # (```)
 
 [//]: # ()
 
 
 
 [//]: # (### ASCII Art Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (generate --description "Get a png as input and return a vectorized version as svg." --test "Make sure when you convert the image back, it looks similar." --path microservice --verbose)
 
 ## Technical Insights
 The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
@@ -494,22 +475,22 @@
 
     deploy --> streamlit[generate streamlit playground]
 
     streamlit --> user_run[user tests microservice]
 
 ```
 
-1. GPT Deploy identifies several strategies to implement your task.
+1. Dev-GPT identifies several strategies to implement your task.
 2. It tests each strategy until it finds one that works.
 3. For each strategy, it generates the following files:
 - microservice.py: This is the main implementation of the microservice.
 - test_microservice.py: These are test cases to ensure the microservice works as expected.
 - requirements.txt: This file lists the packages needed by the microservice and its tests.
 - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
-4. GPT Deploy attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
+4. Dev-GPT attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
 5. Once it finds a successful strategy, it:
 - Pushes the Docker image to the registry.
 - Deploys the microservice.
 - Generates a Streamlit playground where you can test the microservice.
 6. If it fails 10 times in a row, it moves on to the next approach.
 
 
@@ -525,15 +506,15 @@
 - [ ] add video to README.md
 - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
 - [ ] new user has free credits but should be told to verify account
 
 
 Nice to have:
 - [ ] smooth rendering animation of  the responses
-- [ ] if the user runs gptdeploy without any arguments, show the help message
+- [ ] if the user runs dev-gpt without any arguments, show the help message
 - [ ] don't show this message: 
 🔐 You are logged in to Jina AI as florian.hoenicke (username:auth0-unified-448f11965ce142b6). 
 To log out, use jina auth logout.
 - [ ] put the playground into the custom gateway (without rebuilding the custom gateway)
 - [ ] hide prompts in normal mode and show them in verbose mode
 - [ ] tests
 - [ ] clean up duplicate code
@@ -544,22 +525,20 @@
 - [ ] support multiple endpoints - example: todolist microservice with endpoints for adding, deleting, and listing todos
 - [ ] support stateful microservices
 - [ ] The playground is currently printed twice even if it did not change. 
 Make sure it is only printed twice in case it changed.
 - [ ] allow to update your microservice by providing feedback
 - [ ] support for other large language models like Open Assistent
 - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
-- [ ] use gptdeploy list to show all deployments
-- [ ] gptdeploy delete to delete a deployment
-- [ ] gptdeploy update to update a deployment
+- [ ] use dev-gpt list to show all deployments
+- [ ] dev-gpt delete to delete a deployment
+- [ ] dev-gpt update to update a deployment
 - [ ] test param optional - in case the test param is not there first ask gpt if more information is required to write a test - like access to pdf data
 - [ ] section for microservices built by the community
 - [ ] test feedback for playground generation (could be part of the debugging)
 - [ ] should we send everything via json in the text attribute for simplicity?
 - [ ] fix release workflow
 - [ ] after the user specified the task, ask them questions back if the task is not clear enough or something is missing
 
 Proposal:
 - [ ] just generate the non-jina related code and insert it into an executor template
 - [ ] think about strategies after the first approach failed?
-
-
```

#### html2text {}

```diff
@@ -1,180 +1,168 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev43 Summary: Use natural
-language interface to generate, deploy and update your microservice
-infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
-HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
-File: LICENSE
-       ****** GPT Deploy: One line to generate them all ð§ð ******
+        ****** Dev GPT : One line to generate them all ð§ð ******
                                 [Jina NOW logo]
   Turn your natural language descriptions into fully functional, deployed AI-
   powered microservices with a single command! Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
- platforms] [Downloads] [Discord_Chat] [![Watch the video](res/thumbnail.png)]
- (https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-
-                          4e17-ab7a-ba66adca754c.mp4)
+    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
+ thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
+                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
 This project streamlines the creation and deployment of AI-powered
 microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. To ensure the
-microservice accurately aligns with your intended task a test scenario is
-required. ## Quickstart ### Requirements - OpenAI key with access to GPT-3.5 or
-GPT-4 ### Installation ```bash pip install gptdeploy gptdeploy configure --key
-``` If you set the environment variable `OPENAI_API_KEY`, the configuration
-step can be skipped. Your api key must have access to gpt-4 to use this tool.
-We are working on a way to use gpt-3.5-turbo as well. ### Generate Microservice
-```bash gptdeploy generate \ --description "" \ --model
+will automatically build and deploy your microservice. You get guidance from
+our three agents: ## Quickstart ### Requirements - OpenAI key with access to
+GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
+--key  ``` If you set the environment variable `OPENAI_API_KEY`, the
+configuration step can be skipped. Your api key must have access to gpt-4 to
+use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
+Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
 should take between 5 and 15 minutes. During this time, GPT iteratively builds
 your microservice until it finds a strategy that make your test scenario pass.
 Be aware that the costs you have to pay for openai vary between $0.50 and $3.00
-per microservice (using GPT-4). ### Run Microservice Run the microservice
-locally in docker. In case docker is not running on your machine, it will try
-to run it without docker. With this command a playground opens in your browser
-where you can test the microservice. ```bash gptdeploy run --path  ``` ###
-Deploy Microservice If you want to deploy your microservice to the cloud a
-[Jina account](https://cloud.jina.ai/) is required. When creating a Jina
-account, you get some free credits, which you can use to deploy your
-microservice ($0.025/hour). If you run out of credits, you can purchase more.
-```bash gptdeploy deploy --microservice_path  ``` ### Delete Microservice To
-save credits you can delete your microservice via the following commands:
-```bash jc list # get the microservice id jc delete  ``` ## Examples In this
-section you can get a feeling for the kind of microservices that can be
-generated with GPT Deploy. ### Compliment Generator ```bash gptdeploy generate
-\ --description "The user writes something and gets a related deep compliment."
-\ --model gpt-4 ``` [Compliment Generator] ### Extract and summarize news
-articles given a URL ```bash gptdeploy generate \ --description "Extract text
-from a news article URL using Newspaper3k library and generate a summary using
-gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-
-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example] ### Chemical
-Formula Visualization ```bash gptdeploy generate \ --description "Convert a
-chemical formula into a 2D chemical structure diagram. Example inputs: C=C,
-CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula Visualization] ### 2d
-rendering of 3d model ```bash gptdeploy generate \ --description "create a 2d
-rendering of a whole 3d object and x,y,z object rotation using trimesh and
-pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and
-freeglut3-dev library - example input: https://graphics.stanford.edu/courses/
-cs148-10-summer/as3/code/as3/teapot.obj" \ --model gpt-4 ``` [2D Rendering of
-3D Model] ### Product Recommendation ```bash gptdeploy generate \ --description
-"Generate personalized product recommendations based on user product browsing
-history and the product categories fashion, electronics and sport. Example:
-Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion),
-output: p4(fashion)" \ --model gpt-4 ``` [Product Recommendation] ### Hacker
-News Search ```bash gptdeploy generate \ --description "Given a search query,
-find articles on hacker news using the hacker news api and return a list of
-(title, author, website_link, first_image_on_the_website)" \ --model gpt-4 ````
-[Hacker News Search] ### Animal Detector ```bash gptdeploy generate \ --
-description "Given an image, return the image with bounding boxes of all
-animals (https://pjreddie.com/media/files/yolov3.weights, https://
-raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example
-input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \ --model
-gpt-4 ``` [Animal Detector] ### Meme Generator ```bash gptdeploy generate \ --
-description "Generate a meme from an image and a caption. Example input: https:
-//media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
-Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \ --model
-gpt-4 ``` [Meme Generator] ### Rhyme Generator ```bash gptdeploy generate \ --
+per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo. ### Run
+Microservice Run the microservice locally in docker. In case docker is not
+running on your machine, it will try to run it without docker. With this
+command a playground opens in your browser where you can test the microservice.
+```bash dev-gpt run --path  ``` ### Deploy Microservice If you want to deploy
+your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is
+required. When creating a Jina account, you get some free credits, which you
+can use to deploy your microservice ($0.025/hour). If you run out of credits,
+you can purchase more. ```bash dev-gpt deploy --microservice_path  ``` ###
+Delete Microservice To save credits you can delete your microservice via the
+following commands: ```bash jc list # get the microservice id jc delete  ``` ##
+Examples In this section you can get a feeling for the kind of microservices
+that can be generated with Dev-GPT. ### Compliment Generator ```bash dev-gpt
+generate \ --description "The user writes something and gets a related deep
+compliment." \ --model gpt-4 ``` [Compliment Generator] ### Extract and
+summarize news articles given a URL ```bash dev-gpt generate \ --description
+"Extract text from a news article URL using Newspaper3k library and generate a
+summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-
+laws-obamacare-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example]
+### Chemical Formula Visualization ```bash dev-gpt generate \ --description
+"Convert a chemical formula into a 2D chemical structure diagram. Example
+inputs: C=C, CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula
+Visualization] ### 2d rendering of 3d model ```bash dev-gpt generate \ --
+description "create a 2d rendering of a whole 3d object and x,y,z object
+rotation using trimesh and pyrender.OffscreenRenderer with os.environ
+['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https:
+//graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \ --
+model gpt-4 ``` [2D Rendering of 3D Model] ### Product Recommendation ```bash
+dev-gpt generate \ --description "Generate personalized product recommendations
+based on user product browsing history and the product categories fashion,
+electronics and sport. Example: Input: browsing history: prod1
+(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \ --model
+gpt-4 ``` [Product Recommendation] ### Hacker News Search ```bash dev-gpt
+generate \ --description "Given a search query, find articles on hacker news
+using the hacker news api and return a list of (title, author, website_link,
+first_image_on_the_website)" \ --model gpt-4 ```` [Hacker News Search] ###
+Animal Detector ```bash dev-gpt generate \ --description "Given an image,
+return the image with bounding boxes of all animals (https://pjreddie.com/
+media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/
+master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-
+1444212477490-ca407925329e" \ --model gpt-4 ``` [Animal Detector] ### Meme
+Generator ```bash dev-gpt generate \ --description "Generate a meme from an
+image and a caption. Example input: https://media.wired.com/photos/
+5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
+Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \ --model gpt-
+4 ``` [Meme Generator] ### Rhyme Generator ```bash dev-gpt generate \ --
 description "Given a word, return a list of rhyming words using the datamuse
 api" \ --model gpt-4 ``` [Rhyme Generator] ### Word Cloud Generator ```bash
-gptdeploy generate \ --description "Generate a word cloud from a given text" \
---model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash gptdeploy
+dev-gpt generate \ --description "Generate a word cloud from a given text" \ --
+model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash dev-gpt
 generate \ --description "Given a 3d object, return vertex count and face
 count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/
 master/models/wolf.obj" \ --model gpt-4 ``` [3D Model Info] ### Table
-extraction ```bash gptdeploy generate \ --description "Given a URL, extract all
+extraction ```bash dev-gpt generate \ --description "Given a URL, extract all
 tables as csv. Example: http://www.ins.tn/statistiques/90" \ --model gpt-4 ```
-[Table Extraction] ### Audio to mel spectrogram ```bash gptdeploy generate \ --
+[Table Extraction] ### Audio to mel spectrogram ```bash dev-gpt generate \ --
 description "Create mel spectrogram from audio file. Example: https://
 cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \ --model gpt-
-4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash gptdeploy generate
-\ --description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
+4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash dev-gpt generate \
+--description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
 Your browser does not support the audio element.  ### Heatmap Generator ```bash
-gptdeploy generate \ --description "Create a heatmap from an image and a list
-of relative coordinates. Example input: https://images.unsplash.com/photo-
+dev-gpt generate \ --description "Create a heatmap from an image and a list of
+relative coordinates. Example input: https://images.unsplash.com/photo-
 1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1],
 [0.7, 0.2], [0.4, 0.2]]" \ --model gpt-4 ``` [Heatmap Generator] ### QR Code
-Generator ```bash gptdeploy generate \ --description "Generate QR code from
-URL. Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code
-Generator] ### Mandelbrot Set Visualizer ```bash gptdeploy generate \ --
-description "Visualize the Mandelbrot set with custom parameters. Example
-input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-
-4 ``` [Mandelbrot Set Visualizer] ### Markdown to HTML Converter ```bash
-gptdeploy generate --description "Convert markdown to HTML" ``` [Markdown to
-HTML Converter] [//]: # (## TO BE TESTED) [//]: # (### Password Strength
-Checker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Given a
-password, return a score from 1 to 10 indicating the strength of the password"
---test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (###
-Morse Code Translator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Convert text to morse code" --test "Hello, welcome to GPT
-Deploy!") [//]: # (```) [//]: # (### IP Geolocation) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given an IP address, return the geolocation
-information" --test "142.251.46.174") [//]: # (```) [//]: # (### Currency
-Converter) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Converts any currency into any other" --test "1 usd to eur") [//]: # (```) [//
-]: # (### Image Resizer) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given an image, resize it to a specified width and height" --test
-"https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```)
-[//]: # (### Weather API) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given a city, return the current weather" --test "Berlin") [//]: #
-(```) [//]: # () [//]: # (### Sudoku Solver) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given a sudoku puzzle, return the solution"
---test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0,
-0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0,
-4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0,
-3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]: # () [//]: # (### Carbon
-Footprint Calculator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Estimate a company's carbon footprint based on factors like
-transportation, electricity usage, waste production etc..." --test "Jina AI")
-[//]: # (```) [//]: # () [//]: # (### Real Estate Valuation Estimator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Create a microservice that
-estimates the value of a property based on factors like location, property
-type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100mÂ², 10
-years old") [//]: # (```) [//]: # () [//]: # (### Gene Sequence Alignment) [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Align two DNA or RNA
-sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA") [//]: #
-(```) [//]: # () [//]: # (### Barcode Generator) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Generate a barcode from a string" --test
-"Hello, welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### File
-Compression) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Compress a file using the gzip algorithm" --test "content of the file: Hello,
-welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### Watermarking
-Images) [//]: # (```bash) [//]: # (gptdeploy generate --description "Add a
-watermark (GPT Deploy) to an image" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### File
-Metadata Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Extract metadata from a file" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### Video
-Thumbnail Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Extract a thumbnail from a video" --test "http://techslides.com/
-demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: # (### Gif
-Maker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Create a
-gif from a list of images" --test "https://images.unsplash.com/photo-
+Generator ```bash dev-gpt generate \ --description "Generate QR code from URL.
+Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code Generator]
+### Mandelbrot Set Visualizer ```bash dev-gpt generate \ --description
+"Visualize the Mandelbrot set with custom parameters. Example input: center=-
+0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-4 ``` [Mandelbrot
+Set Visualizer] ### Markdown to HTML Converter ```bash dev-gpt generate --
+description "Convert markdown to HTML" ``` [Markdown to HTML Converter] [//]: #
+(## TO BE TESTED) [//]: # (### Password Strength Checker) [//]: # (```bash) [//
+]: # (dev-gpt generate --description "Given a password, return a score from 1
+to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5,
+!Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (### Morse Code Translator) [//]:
+# (```bash) [//]: # (dev-gpt generate --description "Convert text to morse
+code" --test "Hello, welcome to GPT Dev!") [//]: # (```) [//]: # (### IP
+Geolocation) [//]: # (```bash) [//]: # (dev-gpt generate --description "Given
+an IP address, return the geolocation information" --test "142.251.46.174") [//
+]: # (```) [//]: # (### Currency Converter) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Converts any currency into any other" --test "1 usd to
+eur") [//]: # (```) [//]: # (### Image Resizer) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Given an image, resize it to a specified width and
+height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (```) [//]: # (### Weather API) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Given a city, return the current weather" --test
+"Berlin") [//]: # (```) [//]: # () [//]: # (### Sudoku Solver) [//]: #
+(```bash) [//]: # (dev-gpt generate --description "Given a sudoku puzzle,
+return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4,
+0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0,
+0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2],
+[0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]:
+# () [//]: # (### Carbon Footprint Calculator) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Estimate a company's carbon footprint based on
+factors like transportation, electricity usage, waste production etc..." --test
+"Jina AI") [//]: # (```) [//]: # () [//]: # (### Real Estate Valuation
+Estimator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Create a
+microservice that estimates the value of a property based on factors like
+location, property type, age, and square footage." --test "Berlin
+Friedrichshain, Flat, 100mÂ², 10 years old") [//]: # (```) [//]: # () [//]: #
+(### Gene Sequence Alignment) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Align two DNA or RNA sequences using the Needleman-Wunsch
+algorithm" --test "AGTC, GTCA") [//]: # (```) [//]: # () [//]: # (### Barcode
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Generate
+a barcode from a string" --test "Hello, welcome to Dev-GPT!") [//]: # (```) [//
+]: # () [//]: # (### File Compression) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Compress a file using the gzip algorithm" --test
+"content of the file: Hello, welcome to Dev-GPT!") [//]: # (```) [//]: # () [//
+]: # (### Watermarking Images) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Add a watermark (Dev-GPT) to an image" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### File Metadata Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract metadata from a file" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### Video Thumbnail Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract a thumbnail from a video" --test "http://
+techslides.com/demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: #
+(### Gif Maker) [//]: # (```bash) [//]: # (dev-gpt generate --description
+"Create a gif from a list of images" --test "https://images.unsplash.com/photo-
 1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-
 bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68") [/
 /]: # (```) [//]: # () [//]: # () [//]: # (### Sound Visualizer) [//]: # () [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Visualize a sound
-file and output the visualization as video combined with the sound" --test
-"some/mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: #
-(### Color Palette Generator) [//]: # (```bash) [//]: # (gptdeploy generate --
+]: # (```bash) [//]: # (dev-gpt generate --description "Visualize a sound file
+and output the visualization as video combined with the sound" --test "some/
+mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: # (###
+Color Palette Generator) [//]: # (```bash) [//]: # (dev-gpt generate --
 description "creates aesthetically pleasing color palettes based on a seed
 color, using color theory principles like complementary or analogous colors" --
 test "red") [//]: # (```) [//]: # () [//]: # (### Depth Map Generator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Generate a depth map from
-a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
+(```bash) [//]: # (dev-gpt generate --description "Generate a depth map from a
+3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### ASCII Art
-Generator) [//]: # (```bash) [//]: # (gptdeploy generate --description "Convert
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Convert
 image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-
 51ab2ae6c4ff") [//]: # (```) [//]: # (generate --description "Get a png as
 input and return a vectorized version as svg." --test "Make sure when you
 convert the image back, it looks similar." --path microservice --verbose) ##
 Technical Insights The graphic below illustrates the process of creating a
 microservice and deploying it to the cloud elaboration two different
 implementation strategies. ```mermaid graph TB description[description:
@@ -183,54 +171,54 @@
 [implement strategy 1] implement1 --> build1{build image} build1 -->|error
 message| implement1 build1 -->|failed 10 times| implement2[implement strategy
 2] build1 -->|success| registry[push docker image to registry] implement2 --
 > build2{build image} build2 -->|error message| implement2 build2 -->|failed 10
 times| all_failed[all strategies failed] build2 -->|success| registry[push
 docker image to registry] registry --> deploy[deploy microservice] deploy --
 > streamlit[generate streamlit playground] streamlit --> user_run[user tests
-microservice] ``` 1. GPT Deploy identifies several strategies to implement your
+microservice] ``` 1. Dev-GPT identifies several strategies to implement your
 task. 2. It tests each strategy until it finds one that works. 3. For each
 strategy, it generates the following files: - microservice.py: This is the main
 implementation of the microservice. - test_microservice.py: These are test
 cases to ensure the microservice works as expected. - requirements.txt: This
 file lists the packages needed by the microservice and its tests. - Dockerfile:
 This file is used to run the microservice in a container and also runs the
-tests when building the image. 4. GPT Deploy attempts to build the image. If
-the build fails, it uses the error message to apply a fix and tries again to
-build the image. 5. Once it finds a successful strategy, it: - Pushes the
-Docker image to the registry. - Deploys the microservice. - Generates a
-Streamlit playground where you can test the microservice. 6. If it fails 10
-times in a row, it moves on to the next approach. ## ð® vision Use natural
-language interface to generate, deploy and update your microservice
-infrastructure. ## â¨ Contributors If you want to contribute to this project,
-feel free to open a PR or an issue. In the following, you can find a list of
-things that need to be done. next steps: - [ ] check if windows and linux
-support works - [ ] add video to README.md - [ ] bug: it can happen that the
-code generation is hanging forever - in this case aboard and redo the
-generation - [ ] new user has free credits but should be told to verify account
-Nice to have: - [ ] smooth rendering animation of the responses - [ ] if the
-user runs gptdeploy without any arguments, show the help message - [ ] don't
-show this message: ð You are logged in to Jina AI as florian.hoenicke
-(username:auth0-unified-448f11965ce142b6). To log out, use jina auth logout. -
-[ ] put the playground into the custom gateway (without rebuilding the custom
-gateway) - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] add more examples to README.md - [ ]
-support multiple endpoints - example: todolist microservice with endpoints for
-adding, deleting, and listing todos - [ ] support stateful microservices - [ ]
-The playground is currently printed twice even if it did not change. Make sure
-it is only printed twice in case it changed. - [ ] allow to update your
-microservice by providing feedback - [ ] support for other large language
-models like Open Assistent - [ ] for cost savings, it should be possible to
-insert less context during the code generation of the main functionality - no
-jina knowledge is required - [ ] use gptdeploy list to show all deployments -
-[ ] gptdeploy delete to delete a deployment - [ ] gptdeploy update to update a
-deployment - [ ] test param optional - in case the test param is not there
-first ask gpt if more information is required to write a test - like access to
-pdf data - [ ] section for microservices built by the community - [ ] test
-feedback for playground generation (could be part of the debugging) - [ ]
-should we send everything via json in the text attribute for simplicity? - [ ]
-fix release workflow - [ ] after the user specified the task, ask them
-questions back if the task is not clear enough or something is missing
-Proposal: - [ ] just generate the non-jina related code and insert it into an
-executor template - [ ] think about strategies after the first approach failed?
+tests when building the image. 4. Dev-GPT attempts to build the image. If the
+build fails, it uses the error message to apply a fix and tries again to build
+the image. 5. Once it finds a successful strategy, it: - Pushes the Docker
+image to the registry. - Deploys the microservice. - Generates a Streamlit
+playground where you can test the microservice. 6. If it fails 10 times in a
+row, it moves on to the next approach. ## ð® vision Use natural language
+interface to generate, deploy and update your microservice infrastructure. ##
+â¨ Contributors If you want to contribute to this project, feel free to open a
+PR or an issue. In the following, you can find a list of things that need to be
+done. next steps: - [ ] check if windows and linux support works - [ ] add
+video to README.md - [ ] bug: it can happen that the code generation is hanging
+forever - in this case aboard and redo the generation - [ ] new user has free
+credits but should be told to verify account Nice to have: - [ ] smooth
+rendering animation of the responses - [ ] if the user runs dev-gpt without any
+arguments, show the help message - [ ] don't show this message: ð You are
+logged in to Jina AI as florian.hoenicke (username:auth0-unified-
+448f11965ce142b6). To log out, use jina auth logout. - [ ] put the playground
+into the custom gateway (without rebuilding the custom gateway) - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] support for other large language models like Open Assistent -
+[ ] for cost savings, it should be possible to insert less context during the
+code generation of the main functionality - no jina knowledge is required - [ ]
+use dev-gpt list to show all deployments - [ ] dev-gpt delete to delete a
+deployment - [ ] dev-gpt update to update a deployment - [ ] test param
+optional - in case the test param is not there first ask gpt if more
+information is required to write a test - like access to pdf data - [ ] section
+for microservices built by the community - [ ] test feedback for playground
+generation (could be part of the debugging) - [ ] should we send everything via
+json in the text attribute for simplicity? - [ ] fix release workflow - [ ]
+after the user specified the task, ask them questions back if the task is not
+clear enough or something is missing Proposal: - [ ] just generate the non-jina
+related code and insert it into an executor template - [ ] think about
+strategies after the first approach failed?
```

### Comparing `dev-gpt-0.18.35.dev43/README.md` & `dev-gpt-0.18.35.dev49/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,445 +1,466 @@
+Metadata-Version: 2.1
+Name: dev-gpt
+Version: 0.18.35.dev49
+Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
+Home-page: https://github.com/jina-ai/dev-gpt
+Author: Florian Hönicke
+Author-email: florian.hoenicke@jina.ai
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">
-GPT Deploy: One line to generate them all 🧙🚀
+Dev GPT : One line to generate them all 🧙🚀
 </h1>
 
 <p align="center">
-<img src="res/gpt-deploy-logo.png" alt="Jina NOW logo" width="150px">
+<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
 </p>
 <p align="center">
 Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
 <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/fastapi" target="_blank">
     <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/fastapi.svg" alt="Coverage">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/gptdeploy?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/v/dev-gpt?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/gptdeploy.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/dev-gpt.svg?color=%2334D058" alt="Supported Python versions">
 </a>
-<a href="https://github.com/tiangolo/gptdeploy/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
+<a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
-<a href="https://pypistats.org/packages/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/dm/gptdeploy?color=%2334D058&label=pypi%20downloads" alt="Downloads">
+<a href="https://pypistats.org/packages/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 
-[![Watch the video](res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)
+[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
 </p>
 This project streamlines the creation and deployment of AI-powered microservices. 
 Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-To ensure the microservice accurately aligns with your intended task a test scenario is required.
+You get guidance from our three agents:
+
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
 ```bash
-pip install gptdeploy
-gptdeploy configure --key <your openai api key>
+pip install dev-gpt
+dev-gpt configure --key <your openai api key>
 ```
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ### Generate Microservice
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
 To generate your personal microservice two things are required:
 - A `description` of the task you want to accomplish. (optional)
 - The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x cheaper, 
 but will not be able to generate as complex microservices. (default: largest you have access to)
 - A `path` on the local drive where the microservice will be generated. (default: ./microservice)
 
 The creation process should take between 5 and 15 minutes.
 During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
 
-Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice (using GPT-4).
+Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo.
 
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
-gptdeploy run --path <path to microservice>
+dev-gpt run --path <path to microservice>
 ```
 
 
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
-gptdeploy deploy --microservice_path <path to microservice>
+dev-gpt deploy --microservice_path <path to microservice>
 ```
 
 
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
 ## Examples
-In this section you can get a feeling for the kind of microservices that can be generated with GPT Deploy.
+In this section you can get a feeling for the kind of microservices that can be generated with Dev-GPT.
 
 ### Compliment Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
 
 ### Extract and summarize news articles given a URL
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
 
 ### Chemical Formula Visualization
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert a chemical formula into a 2D chemical structure diagram. Example inputs: C=C, CN=C=O, CCC(=O)O" \
 --model gpt-4
 ```
 <img src="res/chemical_formula_example.png" alt="Chemical Formula Visualization" width="400" />
 
 ### 2d rendering of 3d model
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "create a 2d rendering of a whole 3d object and x,y,z object rotation using trimesh and pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https://graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \
 --model gpt-4
 ```
 <img src="res/obj_render_example.gif" alt="2D Rendering of 3D Model" width="400" />
 
 ### Product Recommendation
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate personalized product recommendations based on user product browsing history and the product categories fashion, electronics and sport. Example: Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \
 --model gpt-4
 ```
 <img src="res/recommendation_example.png" alt="Product Recommendation" width="400" />
 
 ### Hacker News Search
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a search query, find articles on hacker news using the hacker news api and return a list of (title, author, website_link, first_image_on_the_website)" \
 --model gpt-4
 ````
 <img src="res/hacker_news_example.png" alt="Hacker News Search" width="400" />
 
 ### Animal Detector
 ```bash
 
-gptdeploy generate \
+dev-gpt generate \
 --description "Given an image, return the image with bounding boxes of all animals (https://pjreddie.com/media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \
 --model gpt-4
 ```
 <img src="res/animal_detector_example.png" alt="Animal Detector" width="400" />
 
 ### Meme Generator
 ```bash
-gptdeploy generate \
---description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \
+dev-gpt generate \
+--description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \
 --model gpt-4
 ```
 <img src="res/meme_example.png" alt="Meme Generator" width="400" />
 
 ### Rhyme Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a word, return a list of rhyming words using the datamuse api" \
 --model gpt-4
 ```
 <img src="res/rhyme_generator_example.png" alt="Rhyme Generator" width="400" />
 
 ### Word Cloud Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate a word cloud from a given text" \
 --model gpt-4
 ```
 <img src="res/word_cloud_example.png" alt="Word Cloud Generator" width="400" />
 
 ### 3d model info
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a 3d object, return vertex count and face count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj" \
 --model gpt-4
 ```
 <img src="res/obj_info_example.png" alt="3D Model Info" width="400" />
 
 ### Table extraction
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a URL, extract all tables as csv. Example: http://www.ins.tn/statistiques/90" \
 --model gpt-4
 ```
 <img src="res/table_extraction_example.png" alt="Table Extraction" width="400" />
 
 ### Audio to mel spectrogram
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create mel spectrogram from audio file. Example: https://cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \
 --model gpt-4
 ```
 <img src="res/audio_to_mel_example.png" alt="Audio to Mel Spectrogram" width="400" />
 
 ### Text to speech
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert text to speech" \
 --model gpt-4
 ```
 <a href=res/text_to_speech_example.wav><img src="res/text_to_speech_example.png" alt="Text to Speech" width="400" /></a>
 
 <audio controls>
   <source src="res/text_to_speech_example.wav" type="audio/mpeg">
   Your browser does not support the audio element.
 </audio>
 
 ### Heatmap Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create a heatmap from an image and a list of relative coordinates. Example input: https://images.unsplash.com/photo-1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1], [0.7, 0.2], [0.4, 0.2]]" \
 --model gpt-4
 ```
 <img src="res/heatmap_example.png" alt="Heatmap Generator" width="400" />
 
 ### QR Code Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate QR code from URL. Example input: https://www.example.com" \
 --model gpt-4 
 ```
 <img src="res/qr_example.png" alt="QR Code Generator" width="400" />
 
 ### Mandelbrot Set Visualizer
 
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Visualize the Mandelbrot set with custom parameters. Example input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \
 --model gpt-4
 ```
 <img src="res/mandelbrot_example.png" alt="Mandelbrot Set Visualizer" width="400" />
 
 
 ### Markdown to HTML Converter
 
 ```bash
-gptdeploy generate --description "Convert markdown to HTML"
+dev-gpt generate --description "Convert markdown to HTML"
 ```
 
 <img src="res/markdown_to_html_example.png" alt="Markdown to HTML Converter" width="400" />
 
 
 
 [//]: # (## TO BE TESTED)
 
 
 [//]: # (### Password Strength Checker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
+[//]: # (dev-gpt generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
 
 [//]: # (```)
 
 [//]: # (### Morse Code Translator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert text to morse code" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Convert text to morse code" --test "Hello, welcome to GPT Dev!")
 
 [//]: # (```)
 
 [//]: # (### IP Geolocation)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
+[//]: # (dev-gpt generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
 
 [//]: # (```)
 
 [//]: # (### Currency Converter)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Converts any currency into any other" --test "1 usd to eur")
+[//]: # (dev-gpt generate --description "Converts any currency into any other" --test "1 usd to eur")
 
 [//]: # (```)
 
 [//]: # (### Image Resizer)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (### Weather API)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a city, return the current weather" --test "Berlin")
+[//]: # (dev-gpt generate --description "Given a city, return the current weather" --test "Berlin")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Sudoku Solver)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
+[//]: # (dev-gpt generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Carbon Footprint Calculator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
+[//]: # (dev-gpt generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Real Estate Valuation Estimator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
+[//]: # (dev-gpt generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gene Sequence Alignment)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
+[//]: # (dev-gpt generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Barcode Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a barcode from a string" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Generate a barcode from a string" --test "Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Compression)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Watermarking Images)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Add a watermark &#40;GPT Deploy&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Add a watermark &#40;Dev-GPT&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Metadata Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Video Thumbnail Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
+[//]: # (dev-gpt generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gif Maker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
+[//]: # (dev-gpt generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
 
 [//]: # (```)
 
 [//]: # ()
 
 [//]: # ()
 
 [//]: # (### Sound Visualizer)
 
 [//]: # ()
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
+[//]: # (dev-gpt generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
 
 [//]: # (```)
 
 [//]: # (## Upcoming Challenges)
 
 [//]: # (### Color Palette Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
+[//]: # (dev-gpt generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Depth Map Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
+[//]: # (dev-gpt generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
 
 [//]: # (```)
 
 [//]: # ()
 
 
 
 [//]: # (### ASCII Art Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (generate --description "Get a png as input and return a vectorized version as svg." --test "Make sure when you convert the image back, it looks similar." --path microservice --verbose)
 
 ## Technical Insights
 The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
@@ -474,22 +495,22 @@
 
     deploy --> streamlit[generate streamlit playground]
 
     streamlit --> user_run[user tests microservice]
 
 ```
 
-1. GPT Deploy identifies several strategies to implement your task.
+1. Dev-GPT identifies several strategies to implement your task.
 2. It tests each strategy until it finds one that works.
 3. For each strategy, it generates the following files:
 - microservice.py: This is the main implementation of the microservice.
 - test_microservice.py: These are test cases to ensure the microservice works as expected.
 - requirements.txt: This file lists the packages needed by the microservice and its tests.
 - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
-4. GPT Deploy attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
+4. Dev-GPT attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
 5. Once it finds a successful strategy, it:
 - Pushes the Docker image to the registry.
 - Deploys the microservice.
 - Generates a Streamlit playground where you can test the microservice.
 6. If it fails 10 times in a row, it moves on to the next approach.
 
 
@@ -505,15 +526,15 @@
 - [ ] add video to README.md
 - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
 - [ ] new user has free credits but should be told to verify account
 
 
 Nice to have:
 - [ ] smooth rendering animation of  the responses
-- [ ] if the user runs gptdeploy without any arguments, show the help message
+- [ ] if the user runs dev-gpt without any arguments, show the help message
 - [ ] don't show this message: 
 🔐 You are logged in to Jina AI as florian.hoenicke (username:auth0-unified-448f11965ce142b6). 
 To log out, use jina auth logout.
 - [ ] put the playground into the custom gateway (without rebuilding the custom gateway)
 - [ ] hide prompts in normal mode and show them in verbose mode
 - [ ] tests
 - [ ] clean up duplicate code
@@ -524,20 +545,22 @@
 - [ ] support multiple endpoints - example: todolist microservice with endpoints for adding, deleting, and listing todos
 - [ ] support stateful microservices
 - [ ] The playground is currently printed twice even if it did not change. 
 Make sure it is only printed twice in case it changed.
 - [ ] allow to update your microservice by providing feedback
 - [ ] support for other large language models like Open Assistent
 - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
-- [ ] use gptdeploy list to show all deployments
-- [ ] gptdeploy delete to delete a deployment
-- [ ] gptdeploy update to update a deployment
+- [ ] use dev-gpt list to show all deployments
+- [ ] dev-gpt delete to delete a deployment
+- [ ] dev-gpt update to update a deployment
 - [ ] test param optional - in case the test param is not there first ask gpt if more information is required to write a test - like access to pdf data
 - [ ] section for microservices built by the community
 - [ ] test feedback for playground generation (could be part of the debugging)
 - [ ] should we send everything via json in the text attribute for simplicity?
 - [ ] fix release workflow
 - [ ] after the user specified the task, ask them questions back if the task is not clear enough or something is missing
 
 Proposal:
 - [ ] just generate the non-jina related code and insert it into an executor template
 - [ ] think about strategies after the first approach failed?
+
+
```

#### html2text {}

```diff
@@ -1,169 +1,179 @@
-       ****** GPT Deploy: One line to generate them all ð§ð ******
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev49 Summary: Use natural
+language interface to generate, deploy and update your microservice
+infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
+HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
+UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
+File: LICENSE
+        ****** Dev GPT : One line to generate them all ð§ð ******
                                 [Jina NOW logo]
   Turn your natural language descriptions into fully functional, deployed AI-
   powered microservices with a single command! Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
- platforms] [Downloads] [Discord_Chat] [![Watch the video](res/thumbnail.png)]
- (https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-
-                          4e17-ab7a-ba66adca754c.mp4)
+    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
+ thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
+                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
 This project streamlines the creation and deployment of AI-powered
 microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. To ensure the
-microservice accurately aligns with your intended task a test scenario is
-required. ## Quickstart ### Requirements - OpenAI key with access to GPT-3.5 or
-GPT-4 ### Installation ```bash pip install gptdeploy gptdeploy configure --key
-``` If you set the environment variable `OPENAI_API_KEY`, the configuration
-step can be skipped. Your api key must have access to gpt-4 to use this tool.
-We are working on a way to use gpt-3.5-turbo as well. ### Generate Microservice
-```bash gptdeploy generate \ --description "" \ --model
+will automatically build and deploy your microservice. You get guidance from
+our three agents: ## Quickstart ### Requirements - OpenAI key with access to
+GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
+--key  ``` If you set the environment variable `OPENAI_API_KEY`, the
+configuration step can be skipped. Your api key must have access to gpt-4 to
+use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
+Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
 should take between 5 and 15 minutes. During this time, GPT iteratively builds
 your microservice until it finds a strategy that make your test scenario pass.
 Be aware that the costs you have to pay for openai vary between $0.50 and $3.00
-per microservice (using GPT-4). ### Run Microservice Run the microservice
-locally in docker. In case docker is not running on your machine, it will try
-to run it without docker. With this command a playground opens in your browser
-where you can test the microservice. ```bash gptdeploy run --path  ``` ###
-Deploy Microservice If you want to deploy your microservice to the cloud a
-[Jina account](https://cloud.jina.ai/) is required. When creating a Jina
-account, you get some free credits, which you can use to deploy your
-microservice ($0.025/hour). If you run out of credits, you can purchase more.
-```bash gptdeploy deploy --microservice_path  ``` ### Delete Microservice To
-save credits you can delete your microservice via the following commands:
-```bash jc list # get the microservice id jc delete  ``` ## Examples In this
-section you can get a feeling for the kind of microservices that can be
-generated with GPT Deploy. ### Compliment Generator ```bash gptdeploy generate
-\ --description "The user writes something and gets a related deep compliment."
-\ --model gpt-4 ``` [Compliment Generator] ### Extract and summarize news
-articles given a URL ```bash gptdeploy generate \ --description "Extract text
-from a news article URL using Newspaper3k library and generate a summary using
-gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-
-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example] ### Chemical
-Formula Visualization ```bash gptdeploy generate \ --description "Convert a
-chemical formula into a 2D chemical structure diagram. Example inputs: C=C,
-CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula Visualization] ### 2d
-rendering of 3d model ```bash gptdeploy generate \ --description "create a 2d
-rendering of a whole 3d object and x,y,z object rotation using trimesh and
-pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and
-freeglut3-dev library - example input: https://graphics.stanford.edu/courses/
-cs148-10-summer/as3/code/as3/teapot.obj" \ --model gpt-4 ``` [2D Rendering of
-3D Model] ### Product Recommendation ```bash gptdeploy generate \ --description
-"Generate personalized product recommendations based on user product browsing
-history and the product categories fashion, electronics and sport. Example:
-Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion),
-output: p4(fashion)" \ --model gpt-4 ``` [Product Recommendation] ### Hacker
-News Search ```bash gptdeploy generate \ --description "Given a search query,
-find articles on hacker news using the hacker news api and return a list of
-(title, author, website_link, first_image_on_the_website)" \ --model gpt-4 ````
-[Hacker News Search] ### Animal Detector ```bash gptdeploy generate \ --
-description "Given an image, return the image with bounding boxes of all
-animals (https://pjreddie.com/media/files/yolov3.weights, https://
-raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example
-input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \ --model
-gpt-4 ``` [Animal Detector] ### Meme Generator ```bash gptdeploy generate \ --
-description "Generate a meme from an image and a caption. Example input: https:
-//media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
-Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \ --model
-gpt-4 ``` [Meme Generator] ### Rhyme Generator ```bash gptdeploy generate \ --
+per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo. ### Run
+Microservice Run the microservice locally in docker. In case docker is not
+running on your machine, it will try to run it without docker. With this
+command a playground opens in your browser where you can test the microservice.
+```bash dev-gpt run --path  ``` ### Deploy Microservice If you want to deploy
+your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is
+required. When creating a Jina account, you get some free credits, which you
+can use to deploy your microservice ($0.025/hour). If you run out of credits,
+you can purchase more. ```bash dev-gpt deploy --microservice_path  ``` ###
+Delete Microservice To save credits you can delete your microservice via the
+following commands: ```bash jc list # get the microservice id jc delete  ``` ##
+Examples In this section you can get a feeling for the kind of microservices
+that can be generated with Dev-GPT. ### Compliment Generator ```bash dev-gpt
+generate \ --description "The user writes something and gets a related deep
+compliment." \ --model gpt-4 ``` [Compliment Generator] ### Extract and
+summarize news articles given a URL ```bash dev-gpt generate \ --description
+"Extract text from a news article URL using Newspaper3k library and generate a
+summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-
+laws-obamacare-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example]
+### Chemical Formula Visualization ```bash dev-gpt generate \ --description
+"Convert a chemical formula into a 2D chemical structure diagram. Example
+inputs: C=C, CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula
+Visualization] ### 2d rendering of 3d model ```bash dev-gpt generate \ --
+description "create a 2d rendering of a whole 3d object and x,y,z object
+rotation using trimesh and pyrender.OffscreenRenderer with os.environ
+['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https:
+//graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \ --
+model gpt-4 ``` [2D Rendering of 3D Model] ### Product Recommendation ```bash
+dev-gpt generate \ --description "Generate personalized product recommendations
+based on user product browsing history and the product categories fashion,
+electronics and sport. Example: Input: browsing history: prod1
+(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \ --model
+gpt-4 ``` [Product Recommendation] ### Hacker News Search ```bash dev-gpt
+generate \ --description "Given a search query, find articles on hacker news
+using the hacker news api and return a list of (title, author, website_link,
+first_image_on_the_website)" \ --model gpt-4 ```` [Hacker News Search] ###
+Animal Detector ```bash dev-gpt generate \ --description "Given an image,
+return the image with bounding boxes of all animals (https://pjreddie.com/
+media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/
+master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-
+1444212477490-ca407925329e" \ --model gpt-4 ``` [Animal Detector] ### Meme
+Generator ```bash dev-gpt generate \ --description "Generate a meme from an
+image and a caption. Example input: https://media.wired.com/photos/
+5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
+Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \ --model gpt-
+4 ``` [Meme Generator] ### Rhyme Generator ```bash dev-gpt generate \ --
 description "Given a word, return a list of rhyming words using the datamuse
 api" \ --model gpt-4 ``` [Rhyme Generator] ### Word Cloud Generator ```bash
-gptdeploy generate \ --description "Generate a word cloud from a given text" \
---model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash gptdeploy
+dev-gpt generate \ --description "Generate a word cloud from a given text" \ --
+model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash dev-gpt
 generate \ --description "Given a 3d object, return vertex count and face
 count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/
 master/models/wolf.obj" \ --model gpt-4 ``` [3D Model Info] ### Table
-extraction ```bash gptdeploy generate \ --description "Given a URL, extract all
+extraction ```bash dev-gpt generate \ --description "Given a URL, extract all
 tables as csv. Example: http://www.ins.tn/statistiques/90" \ --model gpt-4 ```
-[Table Extraction] ### Audio to mel spectrogram ```bash gptdeploy generate \ --
+[Table Extraction] ### Audio to mel spectrogram ```bash dev-gpt generate \ --
 description "Create mel spectrogram from audio file. Example: https://
 cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \ --model gpt-
-4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash gptdeploy generate
-\ --description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
+4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash dev-gpt generate \
+--description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
 Your browser does not support the audio element.  ### Heatmap Generator ```bash
-gptdeploy generate \ --description "Create a heatmap from an image and a list
-of relative coordinates. Example input: https://images.unsplash.com/photo-
+dev-gpt generate \ --description "Create a heatmap from an image and a list of
+relative coordinates. Example input: https://images.unsplash.com/photo-
 1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1],
 [0.7, 0.2], [0.4, 0.2]]" \ --model gpt-4 ``` [Heatmap Generator] ### QR Code
-Generator ```bash gptdeploy generate \ --description "Generate QR code from
-URL. Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code
-Generator] ### Mandelbrot Set Visualizer ```bash gptdeploy generate \ --
-description "Visualize the Mandelbrot set with custom parameters. Example
-input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-
-4 ``` [Mandelbrot Set Visualizer] ### Markdown to HTML Converter ```bash
-gptdeploy generate --description "Convert markdown to HTML" ``` [Markdown to
-HTML Converter] [//]: # (## TO BE TESTED) [//]: # (### Password Strength
-Checker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Given a
-password, return a score from 1 to 10 indicating the strength of the password"
---test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (###
-Morse Code Translator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Convert text to morse code" --test "Hello, welcome to GPT
-Deploy!") [//]: # (```) [//]: # (### IP Geolocation) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given an IP address, return the geolocation
-information" --test "142.251.46.174") [//]: # (```) [//]: # (### Currency
-Converter) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Converts any currency into any other" --test "1 usd to eur") [//]: # (```) [//
-]: # (### Image Resizer) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given an image, resize it to a specified width and height" --test
-"https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```)
-[//]: # (### Weather API) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given a city, return the current weather" --test "Berlin") [//]: #
-(```) [//]: # () [//]: # (### Sudoku Solver) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given a sudoku puzzle, return the solution"
---test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0,
-0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0,
-4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0,
-3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]: # () [//]: # (### Carbon
-Footprint Calculator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Estimate a company's carbon footprint based on factors like
-transportation, electricity usage, waste production etc..." --test "Jina AI")
-[//]: # (```) [//]: # () [//]: # (### Real Estate Valuation Estimator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Create a microservice that
-estimates the value of a property based on factors like location, property
-type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100mÂ², 10
-years old") [//]: # (```) [//]: # () [//]: # (### Gene Sequence Alignment) [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Align two DNA or RNA
-sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA") [//]: #
-(```) [//]: # () [//]: # (### Barcode Generator) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Generate a barcode from a string" --test
-"Hello, welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### File
-Compression) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Compress a file using the gzip algorithm" --test "content of the file: Hello,
-welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### Watermarking
-Images) [//]: # (```bash) [//]: # (gptdeploy generate --description "Add a
-watermark (GPT Deploy) to an image" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### File
-Metadata Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Extract metadata from a file" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### Video
-Thumbnail Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Extract a thumbnail from a video" --test "http://techslides.com/
-demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: # (### Gif
-Maker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Create a
-gif from a list of images" --test "https://images.unsplash.com/photo-
+Generator ```bash dev-gpt generate \ --description "Generate QR code from URL.
+Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code Generator]
+### Mandelbrot Set Visualizer ```bash dev-gpt generate \ --description
+"Visualize the Mandelbrot set with custom parameters. Example input: center=-
+0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-4 ``` [Mandelbrot
+Set Visualizer] ### Markdown to HTML Converter ```bash dev-gpt generate --
+description "Convert markdown to HTML" ``` [Markdown to HTML Converter] [//]: #
+(## TO BE TESTED) [//]: # (### Password Strength Checker) [//]: # (```bash) [//
+]: # (dev-gpt generate --description "Given a password, return a score from 1
+to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5,
+!Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (### Morse Code Translator) [//]:
+# (```bash) [//]: # (dev-gpt generate --description "Convert text to morse
+code" --test "Hello, welcome to GPT Dev!") [//]: # (```) [//]: # (### IP
+Geolocation) [//]: # (```bash) [//]: # (dev-gpt generate --description "Given
+an IP address, return the geolocation information" --test "142.251.46.174") [//
+]: # (```) [//]: # (### Currency Converter) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Converts any currency into any other" --test "1 usd to
+eur") [//]: # (```) [//]: # (### Image Resizer) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Given an image, resize it to a specified width and
+height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (```) [//]: # (### Weather API) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Given a city, return the current weather" --test
+"Berlin") [//]: # (```) [//]: # () [//]: # (### Sudoku Solver) [//]: #
+(```bash) [//]: # (dev-gpt generate --description "Given a sudoku puzzle,
+return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4,
+0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0,
+0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2],
+[0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]:
+# () [//]: # (### Carbon Footprint Calculator) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Estimate a company's carbon footprint based on
+factors like transportation, electricity usage, waste production etc..." --test
+"Jina AI") [//]: # (```) [//]: # () [//]: # (### Real Estate Valuation
+Estimator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Create a
+microservice that estimates the value of a property based on factors like
+location, property type, age, and square footage." --test "Berlin
+Friedrichshain, Flat, 100mÂ², 10 years old") [//]: # (```) [//]: # () [//]: #
+(### Gene Sequence Alignment) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Align two DNA or RNA sequences using the Needleman-Wunsch
+algorithm" --test "AGTC, GTCA") [//]: # (```) [//]: # () [//]: # (### Barcode
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Generate
+a barcode from a string" --test "Hello, welcome to Dev-GPT!") [//]: # (```) [//
+]: # () [//]: # (### File Compression) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Compress a file using the gzip algorithm" --test
+"content of the file: Hello, welcome to Dev-GPT!") [//]: # (```) [//]: # () [//
+]: # (### Watermarking Images) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Add a watermark (Dev-GPT) to an image" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### File Metadata Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract metadata from a file" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### Video Thumbnail Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract a thumbnail from a video" --test "http://
+techslides.com/demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: #
+(### Gif Maker) [//]: # (```bash) [//]: # (dev-gpt generate --description
+"Create a gif from a list of images" --test "https://images.unsplash.com/photo-
 1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-
 bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68") [/
 /]: # (```) [//]: # () [//]: # () [//]: # (### Sound Visualizer) [//]: # () [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Visualize a sound
-file and output the visualization as video combined with the sound" --test
-"some/mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: #
-(### Color Palette Generator) [//]: # (```bash) [//]: # (gptdeploy generate --
+]: # (```bash) [//]: # (dev-gpt generate --description "Visualize a sound file
+and output the visualization as video combined with the sound" --test "some/
+mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: # (###
+Color Palette Generator) [//]: # (```bash) [//]: # (dev-gpt generate --
 description "creates aesthetically pleasing color palettes based on a seed
 color, using color theory principles like complementary or analogous colors" --
 test "red") [//]: # (```) [//]: # () [//]: # (### Depth Map Generator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Generate a depth map from
-a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
+(```bash) [//]: # (dev-gpt generate --description "Generate a depth map from a
+3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### ASCII Art
-Generator) [//]: # (```bash) [//]: # (gptdeploy generate --description "Convert
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Convert
 image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-
 51ab2ae6c4ff") [//]: # (```) [//]: # (generate --description "Get a png as
 input and return a vectorized version as svg." --test "Make sure when you
 convert the image back, it looks similar." --path microservice --verbose) ##
 Technical Insights The graphic below illustrates the process of creating a
 microservice and deploying it to the cloud elaboration two different
 implementation strategies. ```mermaid graph TB description[description:
@@ -172,54 +182,54 @@
 [implement strategy 1] implement1 --> build1{build image} build1 -->|error
 message| implement1 build1 -->|failed 10 times| implement2[implement strategy
 2] build1 -->|success| registry[push docker image to registry] implement2 --
 > build2{build image} build2 -->|error message| implement2 build2 -->|failed 10
 times| all_failed[all strategies failed] build2 -->|success| registry[push
 docker image to registry] registry --> deploy[deploy microservice] deploy --
 > streamlit[generate streamlit playground] streamlit --> user_run[user tests
-microservice] ``` 1. GPT Deploy identifies several strategies to implement your
+microservice] ``` 1. Dev-GPT identifies several strategies to implement your
 task. 2. It tests each strategy until it finds one that works. 3. For each
 strategy, it generates the following files: - microservice.py: This is the main
 implementation of the microservice. - test_microservice.py: These are test
 cases to ensure the microservice works as expected. - requirements.txt: This
 file lists the packages needed by the microservice and its tests. - Dockerfile:
 This file is used to run the microservice in a container and also runs the
-tests when building the image. 4. GPT Deploy attempts to build the image. If
-the build fails, it uses the error message to apply a fix and tries again to
-build the image. 5. Once it finds a successful strategy, it: - Pushes the
-Docker image to the registry. - Deploys the microservice. - Generates a
-Streamlit playground where you can test the microservice. 6. If it fails 10
-times in a row, it moves on to the next approach. ## ð® vision Use natural
-language interface to generate, deploy and update your microservice
-infrastructure. ## â¨ Contributors If you want to contribute to this project,
-feel free to open a PR or an issue. In the following, you can find a list of
-things that need to be done. next steps: - [ ] check if windows and linux
-support works - [ ] add video to README.md - [ ] bug: it can happen that the
-code generation is hanging forever - in this case aboard and redo the
-generation - [ ] new user has free credits but should be told to verify account
-Nice to have: - [ ] smooth rendering animation of the responses - [ ] if the
-user runs gptdeploy without any arguments, show the help message - [ ] don't
-show this message: ð You are logged in to Jina AI as florian.hoenicke
-(username:auth0-unified-448f11965ce142b6). To log out, use jina auth logout. -
-[ ] put the playground into the custom gateway (without rebuilding the custom
-gateway) - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] add more examples to README.md - [ ]
-support multiple endpoints - example: todolist microservice with endpoints for
-adding, deleting, and listing todos - [ ] support stateful microservices - [ ]
-The playground is currently printed twice even if it did not change. Make sure
-it is only printed twice in case it changed. - [ ] allow to update your
-microservice by providing feedback - [ ] support for other large language
-models like Open Assistent - [ ] for cost savings, it should be possible to
-insert less context during the code generation of the main functionality - no
-jina knowledge is required - [ ] use gptdeploy list to show all deployments -
-[ ] gptdeploy delete to delete a deployment - [ ] gptdeploy update to update a
-deployment - [ ] test param optional - in case the test param is not there
-first ask gpt if more information is required to write a test - like access to
-pdf data - [ ] section for microservices built by the community - [ ] test
-feedback for playground generation (could be part of the debugging) - [ ]
-should we send everything via json in the text attribute for simplicity? - [ ]
-fix release workflow - [ ] after the user specified the task, ask them
-questions back if the task is not clear enough or something is missing
-Proposal: - [ ] just generate the non-jina related code and insert it into an
-executor template - [ ] think about strategies after the first approach failed?
+tests when building the image. 4. Dev-GPT attempts to build the image. If the
+build fails, it uses the error message to apply a fix and tries again to build
+the image. 5. Once it finds a successful strategy, it: - Pushes the Docker
+image to the registry. - Deploys the microservice. - Generates a Streamlit
+playground where you can test the microservice. 6. If it fails 10 times in a
+row, it moves on to the next approach. ## ð® vision Use natural language
+interface to generate, deploy and update your microservice infrastructure. ##
+â¨ Contributors If you want to contribute to this project, feel free to open a
+PR or an issue. In the following, you can find a list of things that need to be
+done. next steps: - [ ] check if windows and linux support works - [ ] add
+video to README.md - [ ] bug: it can happen that the code generation is hanging
+forever - in this case aboard and redo the generation - [ ] new user has free
+credits but should be told to verify account Nice to have: - [ ] smooth
+rendering animation of the responses - [ ] if the user runs dev-gpt without any
+arguments, show the help message - [ ] don't show this message: ð You are
+logged in to Jina AI as florian.hoenicke (username:auth0-unified-
+448f11965ce142b6). To log out, use jina auth logout. - [ ] put the playground
+into the custom gateway (without rebuilding the custom gateway) - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] support for other large language models like Open Assistent -
+[ ] for cost savings, it should be possible to insert less context during the
+code generation of the main functionality - no jina knowledge is required - [ ]
+use dev-gpt list to show all deployments - [ ] dev-gpt delete to delete a
+deployment - [ ] dev-gpt update to update a deployment - [ ] test param
+optional - in case the test param is not there first ask gpt if more
+information is required to write a test - like access to pdf data - [ ] section
+for microservices built by the community - [ ] test feedback for playground
+generation (could be part of the debugging) - [ ] should we send everything via
+json in the text attribute for simplicity? - [ ] fix release workflow - [ ]
+after the user specified the task, ask them questions back if the task is not
+clear enough or something is missing Proposal: - [ ] just generate the non-jina
+related code and insert it into an executor template - [ ] think about
+strategies after the first approach failed?
```

### Comparing `dev-gpt-0.18.35.dev43/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.35.dev49/dev_gpt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.35.dev43
+Version: 0.18.35.dev49
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
-Home-page: https://github.com/jina-ai/gptdeploy
+Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,451 +15,452 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-GPT Deploy: One line to generate them all 🧙🚀
+Dev GPT : One line to generate them all 🧙🚀
 </h1>
 
 <p align="center">
-<img src="res/gpt-deploy-logo.png" alt="Jina NOW logo" width="150px">
+<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
 </p>
 <p align="center">
 Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
 <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/fastapi" target="_blank">
     <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/fastapi.svg" alt="Coverage">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/v/gptdeploy?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/v/dev-gpt?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/gptdeploy.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/dev-gpt.svg?color=%2334D058" alt="Supported Python versions">
 </a>
-<a href="https://github.com/tiangolo/gptdeploy/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
+<a href="https://github.com/tiangolo/dev-gpt/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://img.shields.io/badge/platform-mac%20%7C%20linux%20%7C%20windows-blue" alt="Supported platforms">
 </a>
-<a href="https://pypistats.org/packages/gptdeploy" target="_blank">
-    <img src="https://img.shields.io/pypi/dm/gptdeploy?color=%2334D058&label=pypi%20downloads" alt="Downloads">
+<a href="https://pypistats.org/packages/dev-gpt" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
 
-[![Watch the video](res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)
+[//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
 </p>
 This project streamlines the creation and deployment of AI-powered microservices. 
 Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-To ensure the microservice accurately aligns with your intended task a test scenario is required.
+You get guidance from our three agents:
+
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
 ```bash
-pip install gptdeploy
-gptdeploy configure --key <your openai api key>
+pip install dev-gpt
+dev-gpt configure --key <your openai api key>
 ```
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
 Your api key must have access to gpt-4 to use this tool. 
 We are working on a way to use gpt-3.5-turbo as well.
 
 ### Generate Microservice
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "<description of the microservice>" \
 --model <gpt-3.5 or gpt-4> \
 --path </path/to/local/folder>
 ```
 To generate your personal microservice two things are required:
 - A `description` of the task you want to accomplish. (optional)
 - The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x cheaper, 
 but will not be able to generate as complex microservices. (default: largest you have access to)
 - A `path` on the local drive where the microservice will be generated. (default: ./microservice)
 
 The creation process should take between 5 and 15 minutes.
 During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
 
-Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice (using GPT-4).
+Be aware that the costs you have to pay for openai vary between $0.50 and $3.00 per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo.
 
 ### Run Microservice
 Run the microservice locally in docker. In case docker is not running on your machine, it will try to run it without docker.
 With this command a playground opens in your browser where you can test the microservice.
 ```bash
-gptdeploy run --path <path to microservice>
+dev-gpt run --path <path to microservice>
 ```
 
 
 ### Deploy Microservice
 If you want to deploy your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is required.
 When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
 If you run out of credits, you can purchase more.
 ```bash
-gptdeploy deploy --microservice_path <path to microservice>
+dev-gpt deploy --microservice_path <path to microservice>
 ```
 
 
 ### Delete Microservice
 To save credits you can delete your microservice via the following commands:
 ```bash
 jc list # get the microservice id
 jc delete <microservice id>
 ```
 
 ## Examples
-In this section you can get a feeling for the kind of microservices that can be generated with GPT Deploy.
+In this section you can get a feeling for the kind of microservices that can be generated with Dev-GPT.
 
 ### Compliment Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "The user writes something and gets a related deep compliment." \
 --model gpt-4
 ```
 <img src="res/compliment_example.png" alt="Compliment Generator" width="400" />
 
 
 ### Extract and summarize news articles given a URL
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Extract text from a news article URL using Newspaper3k library and generate a summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/" \
 --model gpt-4
 ```
 <img src="res/news_article_example.png" alt="News Article Example" width="400" />
 
 ### Chemical Formula Visualization
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert a chemical formula into a 2D chemical structure diagram. Example inputs: C=C, CN=C=O, CCC(=O)O" \
 --model gpt-4
 ```
 <img src="res/chemical_formula_example.png" alt="Chemical Formula Visualization" width="400" />
 
 ### 2d rendering of 3d model
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "create a 2d rendering of a whole 3d object and x,y,z object rotation using trimesh and pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https://graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \
 --model gpt-4
 ```
 <img src="res/obj_render_example.gif" alt="2D Rendering of 3D Model" width="400" />
 
 ### Product Recommendation
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate personalized product recommendations based on user product browsing history and the product categories fashion, electronics and sport. Example: Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \
 --model gpt-4
 ```
 <img src="res/recommendation_example.png" alt="Product Recommendation" width="400" />
 
 ### Hacker News Search
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a search query, find articles on hacker news using the hacker news api and return a list of (title, author, website_link, first_image_on_the_website)" \
 --model gpt-4
 ````
 <img src="res/hacker_news_example.png" alt="Hacker News Search" width="400" />
 
 ### Animal Detector
 ```bash
 
-gptdeploy generate \
+dev-gpt generate \
 --description "Given an image, return the image with bounding boxes of all animals (https://pjreddie.com/media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \
 --model gpt-4
 ```
 <img src="res/animal_detector_example.png" alt="Animal Detector" width="400" />
 
 ### Meme Generator
 ```bash
-gptdeploy generate \
---description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \
+dev-gpt generate \
+--description "Generate a meme from an image and a caption. Example input: https://media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \
 --model gpt-4
 ```
 <img src="res/meme_example.png" alt="Meme Generator" width="400" />
 
 ### Rhyme Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a word, return a list of rhyming words using the datamuse api" \
 --model gpt-4
 ```
 <img src="res/rhyme_generator_example.png" alt="Rhyme Generator" width="400" />
 
 ### Word Cloud Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate a word cloud from a given text" \
 --model gpt-4
 ```
 <img src="res/word_cloud_example.png" alt="Word Cloud Generator" width="400" />
 
 ### 3d model info
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a 3d object, return vertex count and face count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj" \
 --model gpt-4
 ```
 <img src="res/obj_info_example.png" alt="3D Model Info" width="400" />
 
 ### Table extraction
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Given a URL, extract all tables as csv. Example: http://www.ins.tn/statistiques/90" \
 --model gpt-4
 ```
 <img src="res/table_extraction_example.png" alt="Table Extraction" width="400" />
 
 ### Audio to mel spectrogram
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create mel spectrogram from audio file. Example: https://cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \
 --model gpt-4
 ```
 <img src="res/audio_to_mel_example.png" alt="Audio to Mel Spectrogram" width="400" />
 
 ### Text to speech
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Convert text to speech" \
 --model gpt-4
 ```
 <a href=res/text_to_speech_example.wav><img src="res/text_to_speech_example.png" alt="Text to Speech" width="400" /></a>
 
 <audio controls>
   <source src="res/text_to_speech_example.wav" type="audio/mpeg">
   Your browser does not support the audio element.
 </audio>
 
 ### Heatmap Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Create a heatmap from an image and a list of relative coordinates. Example input: https://images.unsplash.com/photo-1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1], [0.7, 0.2], [0.4, 0.2]]" \
 --model gpt-4
 ```
 <img src="res/heatmap_example.png" alt="Heatmap Generator" width="400" />
 
 ### QR Code Generator
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Generate QR code from URL. Example input: https://www.example.com" \
 --model gpt-4 
 ```
 <img src="res/qr_example.png" alt="QR Code Generator" width="400" />
 
 ### Mandelbrot Set Visualizer
 
 ```bash
-gptdeploy generate \
+dev-gpt generate \
 --description "Visualize the Mandelbrot set with custom parameters. Example input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \
 --model gpt-4
 ```
 <img src="res/mandelbrot_example.png" alt="Mandelbrot Set Visualizer" width="400" />
 
 
 ### Markdown to HTML Converter
 
 ```bash
-gptdeploy generate --description "Convert markdown to HTML"
+dev-gpt generate --description "Convert markdown to HTML"
 ```
 
 <img src="res/markdown_to_html_example.png" alt="Markdown to HTML Converter" width="400" />
 
 
 
 [//]: # (## TO BE TESTED)
 
 
 [//]: # (### Password Strength Checker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
+[//]: # (dev-gpt generate --description "Given a password, return a score from 1 to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5")
 
 [//]: # (```)
 
 [//]: # (### Morse Code Translator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert text to morse code" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Convert text to morse code" --test "Hello, welcome to GPT Dev!")
 
 [//]: # (```)
 
 [//]: # (### IP Geolocation)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
+[//]: # (dev-gpt generate --description "Given an IP address, return the geolocation information" --test "142.251.46.174")
 
 [//]: # (```)
 
 [//]: # (### Currency Converter)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Converts any currency into any other" --test "1 usd to eur")
+[//]: # (dev-gpt generate --description "Converts any currency into any other" --test "1 usd to eur")
 
 [//]: # (```)
 
 [//]: # (### Image Resizer)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Given an image, resize it to a specified width and height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (### Weather API)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a city, return the current weather" --test "Berlin")
+[//]: # (dev-gpt generate --description "Given a city, return the current weather" --test "Berlin")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Sudoku Solver)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
+[//]: # (dev-gpt generate --description "Given a sudoku puzzle, return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Carbon Footprint Calculator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
+[//]: # (dev-gpt generate --description "Estimate a company's carbon footprint based on factors like transportation, electricity usage, waste production etc..." --test "Jina AI")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Real Estate Valuation Estimator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
+[//]: # (dev-gpt generate --description "Create a microservice that estimates the value of a property based on factors like location, property type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100m², 10 years old")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gene Sequence Alignment)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
+[//]: # (dev-gpt generate --description "Align two DNA or RNA sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Barcode Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a barcode from a string" --test "Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Generate a barcode from a string" --test "Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Compression)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to GPT Deploy!")
+[//]: # (dev-gpt generate --description "Compress a file using the gzip algorithm" --test "content of the file: Hello, welcome to Dev-GPT!")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Watermarking Images)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Add a watermark &#40;GPT Deploy&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Add a watermark &#40;Dev-GPT&#41; to an image" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### File Metadata Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Extract metadata from a file" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Video Thumbnail Extractor)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
+[//]: # (dev-gpt generate --description "Extract a thumbnail from a video" --test "http://techslides.com/demos/sample-videos/small.mp4")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Gif Maker)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
+[//]: # (dev-gpt generate --description "Create a gif from a list of images" --test "https://images.unsplash.com/photo-1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68")
 
 [//]: # (```)
 
 [//]: # ()
 
 [//]: # ()
 
 [//]: # (### Sound Visualizer)
 
 [//]: # ()
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
+[//]: # (dev-gpt generate --description "Visualize a sound file and output the visualization as video combined with the sound" --test "some/mp3/file.mp3")
 
 [//]: # (```)
 
 [//]: # (## Upcoming Challenges)
 
 [//]: # (### Color Palette Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
+[//]: # (dev-gpt generate --description "creates aesthetically pleasing color palettes based on a seed color, using color theory principles like complementary or analogous colors" --test "red")
 
 [//]: # (```)
 
 [//]: # ()
 [//]: # (### Depth Map Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
+[//]: # (dev-gpt generate --description "Generate a depth map from a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-assets/master/models/wolf.obj")
 
 [//]: # (```)
 
 [//]: # ()
 
 
 
 [//]: # (### ASCII Art Generator)
 
 [//]: # (```bash)
 
-[//]: # (gptdeploy generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (dev-gpt generate --description "Convert image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
 
 [//]: # (```)
 
 [//]: # (generate --description "Get a png as input and return a vectorized version as svg." --test "Make sure when you convert the image back, it looks similar." --path microservice --verbose)
 
 ## Technical Insights
 The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
@@ -494,22 +495,22 @@
 
     deploy --> streamlit[generate streamlit playground]
 
     streamlit --> user_run[user tests microservice]
 
 ```
 
-1. GPT Deploy identifies several strategies to implement your task.
+1. Dev-GPT identifies several strategies to implement your task.
 2. It tests each strategy until it finds one that works.
 3. For each strategy, it generates the following files:
 - microservice.py: This is the main implementation of the microservice.
 - test_microservice.py: These are test cases to ensure the microservice works as expected.
 - requirements.txt: This file lists the packages needed by the microservice and its tests.
 - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
-4. GPT Deploy attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
+4. Dev-GPT attempts to build the image. If the build fails, it uses the error message to apply a fix and tries again to build the image.
 5. Once it finds a successful strategy, it:
 - Pushes the Docker image to the registry.
 - Deploys the microservice.
 - Generates a Streamlit playground where you can test the microservice.
 6. If it fails 10 times in a row, it moves on to the next approach.
 
 
@@ -525,15 +526,15 @@
 - [ ] add video to README.md
 - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
 - [ ] new user has free credits but should be told to verify account
 
 
 Nice to have:
 - [ ] smooth rendering animation of  the responses
-- [ ] if the user runs gptdeploy without any arguments, show the help message
+- [ ] if the user runs dev-gpt without any arguments, show the help message
 - [ ] don't show this message: 
 🔐 You are logged in to Jina AI as florian.hoenicke (username:auth0-unified-448f11965ce142b6). 
 To log out, use jina auth logout.
 - [ ] put the playground into the custom gateway (without rebuilding the custom gateway)
 - [ ] hide prompts in normal mode and show them in verbose mode
 - [ ] tests
 - [ ] clean up duplicate code
@@ -544,17 +545,17 @@
 - [ ] support multiple endpoints - example: todolist microservice with endpoints for adding, deleting, and listing todos
 - [ ] support stateful microservices
 - [ ] The playground is currently printed twice even if it did not change. 
 Make sure it is only printed twice in case it changed.
 - [ ] allow to update your microservice by providing feedback
 - [ ] support for other large language models like Open Assistent
 - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
-- [ ] use gptdeploy list to show all deployments
-- [ ] gptdeploy delete to delete a deployment
-- [ ] gptdeploy update to update a deployment
+- [ ] use dev-gpt list to show all deployments
+- [ ] dev-gpt delete to delete a deployment
+- [ ] dev-gpt update to update a deployment
 - [ ] test param optional - in case the test param is not there first ask gpt if more information is required to write a test - like access to pdf data
 - [ ] section for microservices built by the community
 - [ ] test feedback for playground generation (could be part of the debugging)
 - [ ] should we send everything via json in the text attribute for simplicity?
 - [ ] fix release workflow
 - [ ] after the user specified the task, ask them questions back if the task is not clear enough or something is missing
```

#### html2text {}

```diff
@@ -1,180 +1,179 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev43 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev49 Summary: Use natural
 language interface to generate, deploy and update your microservice
-infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
+infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE
-       ****** GPT Deploy: One line to generate them all ð§ð ******
+        ****** Dev GPT : One line to generate them all ð§ð ******
                                 [Jina NOW logo]
   Turn your natural language descriptions into fully functional, deployed AI-
   powered microservices with a single command! Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
- platforms] [Downloads] [Discord_Chat] [![Watch the video](res/thumbnail.png)]
- (https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-
-                          4e17-ab7a-ba66adca754c.mp4)
+    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
+ thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
+                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
 This project streamlines the creation and deployment of AI-powered
 microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. To ensure the
-microservice accurately aligns with your intended task a test scenario is
-required. ## Quickstart ### Requirements - OpenAI key with access to GPT-3.5 or
-GPT-4 ### Installation ```bash pip install gptdeploy gptdeploy configure --key
-``` If you set the environment variable `OPENAI_API_KEY`, the configuration
-step can be skipped. Your api key must have access to gpt-4 to use this tool.
-We are working on a way to use gpt-3.5-turbo as well. ### Generate Microservice
-```bash gptdeploy generate \ --description "" \ --model
+will automatically build and deploy your microservice. You get guidance from
+our three agents: ## Quickstart ### Requirements - OpenAI key with access to
+GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
+--key  ``` If you set the environment variable `OPENAI_API_KEY`, the
+configuration step can be skipped. Your api key must have access to gpt-4 to
+use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
+Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
 should take between 5 and 15 minutes. During this time, GPT iteratively builds
 your microservice until it finds a strategy that make your test scenario pass.
 Be aware that the costs you have to pay for openai vary between $0.50 and $3.00
-per microservice (using GPT-4). ### Run Microservice Run the microservice
-locally in docker. In case docker is not running on your machine, it will try
-to run it without docker. With this command a playground opens in your browser
-where you can test the microservice. ```bash gptdeploy run --path  ``` ###
-Deploy Microservice If you want to deploy your microservice to the cloud a
-[Jina account](https://cloud.jina.ai/) is required. When creating a Jina
-account, you get some free credits, which you can use to deploy your
-microservice ($0.025/hour). If you run out of credits, you can purchase more.
-```bash gptdeploy deploy --microservice_path  ``` ### Delete Microservice To
-save credits you can delete your microservice via the following commands:
-```bash jc list # get the microservice id jc delete  ``` ## Examples In this
-section you can get a feeling for the kind of microservices that can be
-generated with GPT Deploy. ### Compliment Generator ```bash gptdeploy generate
-\ --description "The user writes something and gets a related deep compliment."
-\ --model gpt-4 ``` [Compliment Generator] ### Extract and summarize news
-articles given a URL ```bash gptdeploy generate \ --description "Extract text
-from a news article URL using Newspaper3k library and generate a summary using
-gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-
-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example] ### Chemical
-Formula Visualization ```bash gptdeploy generate \ --description "Convert a
-chemical formula into a 2D chemical structure diagram. Example inputs: C=C,
-CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula Visualization] ### 2d
-rendering of 3d model ```bash gptdeploy generate \ --description "create a 2d
-rendering of a whole 3d object and x,y,z object rotation using trimesh and
-pyrender.OffscreenRenderer with os.environ['PYOPENGL_PLATFORM'] = 'egl' and
-freeglut3-dev library - example input: https://graphics.stanford.edu/courses/
-cs148-10-summer/as3/code/as3/teapot.obj" \ --model gpt-4 ``` [2D Rendering of
-3D Model] ### Product Recommendation ```bash gptdeploy generate \ --description
-"Generate personalized product recommendations based on user product browsing
-history and the product categories fashion, electronics and sport. Example:
-Input: browsing history: prod1(electronics),prod2(fashion),prod3(fashion),
-output: p4(fashion)" \ --model gpt-4 ``` [Product Recommendation] ### Hacker
-News Search ```bash gptdeploy generate \ --description "Given a search query,
-find articles on hacker news using the hacker news api and return a list of
-(title, author, website_link, first_image_on_the_website)" \ --model gpt-4 ````
-[Hacker News Search] ### Animal Detector ```bash gptdeploy generate \ --
-description "Given an image, return the image with bounding boxes of all
-animals (https://pjreddie.com/media/files/yolov3.weights, https://
-raw.githubusercontent.com/pjreddie/darknet/master/cfg/yolov3.cfg), Example
-input: https://images.unsplash.com/photo-1444212477490-ca407925329e" \ --model
-gpt-4 ``` [Animal Detector] ### Meme Generator ```bash gptdeploy generate \ --
-description "Generate a meme from an image and a caption. Example input: https:
-//media.wired.com/photos/5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
-Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPTDeploy" \ --model
-gpt-4 ``` [Meme Generator] ### Rhyme Generator ```bash gptdeploy generate \ --
+per microservice using GPT-4 or $0.05 to $0.30 for GPT-3.5-Trubo. ### Run
+Microservice Run the microservice locally in docker. In case docker is not
+running on your machine, it will try to run it without docker. With this
+command a playground opens in your browser where you can test the microservice.
+```bash dev-gpt run --path  ``` ### Deploy Microservice If you want to deploy
+your microservice to the cloud a [Jina account](https://cloud.jina.ai/) is
+required. When creating a Jina account, you get some free credits, which you
+can use to deploy your microservice ($0.025/hour). If you run out of credits,
+you can purchase more. ```bash dev-gpt deploy --microservice_path  ``` ###
+Delete Microservice To save credits you can delete your microservice via the
+following commands: ```bash jc list # get the microservice id jc delete  ``` ##
+Examples In this section you can get a feeling for the kind of microservices
+that can be generated with Dev-GPT. ### Compliment Generator ```bash dev-gpt
+generate \ --description "The user writes something and gets a related deep
+compliment." \ --model gpt-4 ``` [Compliment Generator] ### Extract and
+summarize news articles given a URL ```bash dev-gpt generate \ --description
+"Extract text from a news article URL using Newspaper3k library and generate a
+summary using gpt. Example input: http://fox13now.com/2013/12/30/new-year-new-
+laws-obamacare-pot-guns-and-drones/" \ --model gpt-4 ``` [News Article Example]
+### Chemical Formula Visualization ```bash dev-gpt generate \ --description
+"Convert a chemical formula into a 2D chemical structure diagram. Example
+inputs: C=C, CN=C=O, CCC(=O)O" \ --model gpt-4 ``` [Chemical Formula
+Visualization] ### 2d rendering of 3d model ```bash dev-gpt generate \ --
+description "create a 2d rendering of a whole 3d object and x,y,z object
+rotation using trimesh and pyrender.OffscreenRenderer with os.environ
+['PYOPENGL_PLATFORM'] = 'egl' and freeglut3-dev library - example input: https:
+//graphics.stanford.edu/courses/cs148-10-summer/as3/code/as3/teapot.obj" \ --
+model gpt-4 ``` [2D Rendering of 3D Model] ### Product Recommendation ```bash
+dev-gpt generate \ --description "Generate personalized product recommendations
+based on user product browsing history and the product categories fashion,
+electronics and sport. Example: Input: browsing history: prod1
+(electronics),prod2(fashion),prod3(fashion), output: p4(fashion)" \ --model
+gpt-4 ``` [Product Recommendation] ### Hacker News Search ```bash dev-gpt
+generate \ --description "Given a search query, find articles on hacker news
+using the hacker news api and return a list of (title, author, website_link,
+first_image_on_the_website)" \ --model gpt-4 ```` [Hacker News Search] ###
+Animal Detector ```bash dev-gpt generate \ --description "Given an image,
+return the image with bounding boxes of all animals (https://pjreddie.com/
+media/files/yolov3.weights, https://raw.githubusercontent.com/pjreddie/darknet/
+master/cfg/yolov3.cfg), Example input: https://images.unsplash.com/photo-
+1444212477490-ca407925329e" \ --model gpt-4 ``` [Animal Detector] ### Meme
+Generator ```bash dev-gpt generate \ --description "Generate a meme from an
+image and a caption. Example input: https://media.wired.com/photos/
+5f87340d114b38fa1f8339f9/master/w_1600%2Cc_limit/
+Ideas_Surprised_Pikachu_HD.jpg, TOP:When you discovered GPT Dev" \ --model gpt-
+4 ``` [Meme Generator] ### Rhyme Generator ```bash dev-gpt generate \ --
 description "Given a word, return a list of rhyming words using the datamuse
 api" \ --model gpt-4 ``` [Rhyme Generator] ### Word Cloud Generator ```bash
-gptdeploy generate \ --description "Generate a word cloud from a given text" \
---model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash gptdeploy
+dev-gpt generate \ --description "Generate a word cloud from a given text" \ --
+model gpt-4 ``` [Word Cloud Generator] ### 3d model info ```bash dev-gpt
 generate \ --description "Given a 3d object, return vertex count and face
 count. Example: https://raw.githubusercontent.com/polygonjs/polygonjs-assets/
 master/models/wolf.obj" \ --model gpt-4 ``` [3D Model Info] ### Table
-extraction ```bash gptdeploy generate \ --description "Given a URL, extract all
+extraction ```bash dev-gpt generate \ --description "Given a URL, extract all
 tables as csv. Example: http://www.ins.tn/statistiques/90" \ --model gpt-4 ```
-[Table Extraction] ### Audio to mel spectrogram ```bash gptdeploy generate \ --
+[Table Extraction] ### Audio to mel spectrogram ```bash dev-gpt generate \ --
 description "Create mel spectrogram from audio file. Example: https://
 cdn.pixabay.com/download/audio/2023/02/28/audio_550d815fa5.mp3" \ --model gpt-
-4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash gptdeploy generate
-\ --description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
+4 ``` [Audio to Mel Spectrogram] ### Text to speech ```bash dev-gpt generate \
+--description "Convert text to speech" \ --model gpt-4 ``` [Text_to_Speech]
 Your browser does not support the audio element.  ### Heatmap Generator ```bash
-gptdeploy generate \ --description "Create a heatmap from an image and a list
-of relative coordinates. Example input: https://images.unsplash.com/photo-
+dev-gpt generate \ --description "Create a heatmap from an image and a list of
+relative coordinates. Example input: https://images.unsplash.com/photo-
 1574786198875-49f5d09fe2d2, [[0.1, 0.2], [0.3, 0.4], [0.5, 0.6], [0.2, 0.1],
 [0.7, 0.2], [0.4, 0.2]]" \ --model gpt-4 ``` [Heatmap Generator] ### QR Code
-Generator ```bash gptdeploy generate \ --description "Generate QR code from
-URL. Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code
-Generator] ### Mandelbrot Set Visualizer ```bash gptdeploy generate \ --
-description "Visualize the Mandelbrot set with custom parameters. Example
-input: center=-0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-
-4 ``` [Mandelbrot Set Visualizer] ### Markdown to HTML Converter ```bash
-gptdeploy generate --description "Convert markdown to HTML" ``` [Markdown to
-HTML Converter] [//]: # (## TO BE TESTED) [//]: # (### Password Strength
-Checker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Given a
-password, return a score from 1 to 10 indicating the strength of the password"
---test "Pa$$w0rd => 1/5, !Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (###
-Morse Code Translator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Convert text to morse code" --test "Hello, welcome to GPT
-Deploy!") [//]: # (```) [//]: # (### IP Geolocation) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given an IP address, return the geolocation
-information" --test "142.251.46.174") [//]: # (```) [//]: # (### Currency
-Converter) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Converts any currency into any other" --test "1 usd to eur") [//]: # (```) [//
-]: # (### Image Resizer) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given an image, resize it to a specified width and height" --test
-"https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```)
-[//]: # (### Weather API) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Given a city, return the current weather" --test "Berlin") [//]: #
-(```) [//]: # () [//]: # (### Sudoku Solver) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Given a sudoku puzzle, return the solution"
---test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4, 0, 0, 0], [4, 0, 7, 0,
-0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0, 0, 9, 8, 1, 0, 0], [0,
-4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2], [0, 7, 0, 0, 0, 0, 0, 0,
-3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]: # () [//]: # (### Carbon
-Footprint Calculator) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Estimate a company's carbon footprint based on factors like
-transportation, electricity usage, waste production etc..." --test "Jina AI")
-[//]: # (```) [//]: # () [//]: # (### Real Estate Valuation Estimator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Create a microservice that
-estimates the value of a property based on factors like location, property
-type, age, and square footage." --test "Berlin Friedrichshain, Flat, 100mÂ², 10
-years old") [//]: # (```) [//]: # () [//]: # (### Gene Sequence Alignment) [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Align two DNA or RNA
-sequences using the Needleman-Wunsch algorithm" --test "AGTC, GTCA") [//]: #
-(```) [//]: # () [//]: # (### Barcode Generator) [//]: # (```bash) [//]: #
-(gptdeploy generate --description "Generate a barcode from a string" --test
-"Hello, welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### File
-Compression) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Compress a file using the gzip algorithm" --test "content of the file: Hello,
-welcome to GPT Deploy!") [//]: # (```) [//]: # () [//]: # (### Watermarking
-Images) [//]: # (```bash) [//]: # (gptdeploy generate --description "Add a
-watermark (GPT Deploy) to an image" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### File
-Metadata Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --description
-"Extract metadata from a file" --test "https://images.unsplash.com/photo-
-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # () [//]: # (### Video
-Thumbnail Extractor) [//]: # (```bash) [//]: # (gptdeploy generate --
-description "Extract a thumbnail from a video" --test "http://techslides.com/
-demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: # (### Gif
-Maker) [//]: # (```bash) [//]: # (gptdeploy generate --description "Create a
-gif from a list of images" --test "https://images.unsplash.com/photo-
+Generator ```bash dev-gpt generate \ --description "Generate QR code from URL.
+Example input: https://www.example.com" \ --model gpt-4 ``` [QR Code Generator]
+### Mandelbrot Set Visualizer ```bash dev-gpt generate \ --description
+"Visualize the Mandelbrot set with custom parameters. Example input: center=-
+0+1i, zoom=1.0, size=800x800, iterations=1000" \ --model gpt-4 ``` [Mandelbrot
+Set Visualizer] ### Markdown to HTML Converter ```bash dev-gpt generate --
+description "Convert markdown to HTML" ``` [Markdown to HTML Converter] [//]: #
+(## TO BE TESTED) [//]: # (### Password Strength Checker) [//]: # (```bash) [//
+]: # (dev-gpt generate --description "Given a password, return a score from 1
+to 10 indicating the strength of the password" --test "Pa$$w0rd => 1/5,
+!Akfdh%.ytRadf => 5/5") [//]: # (```) [//]: # (### Morse Code Translator) [//]:
+# (```bash) [//]: # (dev-gpt generate --description "Convert text to morse
+code" --test "Hello, welcome to GPT Dev!") [//]: # (```) [//]: # (### IP
+Geolocation) [//]: # (```bash) [//]: # (dev-gpt generate --description "Given
+an IP address, return the geolocation information" --test "142.251.46.174") [//
+]: # (```) [//]: # (### Currency Converter) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Converts any currency into any other" --test "1 usd to
+eur") [//]: # (```) [//]: # (### Image Resizer) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Given an image, resize it to a specified width and
+height" --test "https://images.unsplash.com/photo-1602738328654-51ab2ae6c4ff")
+[//]: # (```) [//]: # (### Weather API) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Given a city, return the current weather" --test
+"Berlin") [//]: # (```) [//]: # () [//]: # (### Sudoku Solver) [//]: #
+(```bash) [//]: # (dev-gpt generate --description "Given a sudoku puzzle,
+return the solution" --test "[[2, 5, 0, 0, 3, 0, 9, 0, 1], [0, 1, 0, 0, 0, 4,
+0, 0, 0], [4, 0, 7, 0, 0, 0, 2, 0, 8], [0, 0, 5, 2, 0, 0, 0, 0, 0], [0, 0, 0,
+0, 9, 8, 1, 0, 0], [0, 4, 0, 0, 0, 3, 0, 0, 0], [0, 0, 0, 3, 6, 0, 0, 7, 2],
+[0, 7, 0, 0, 0, 0, 0, 0, 3], [9, 0, 3, 0, 0, 0, 6, 0, 4]]") [//]: # (```) [//]:
+# () [//]: # (### Carbon Footprint Calculator) [//]: # (```bash) [//]: # (dev-
+gpt generate --description "Estimate a company's carbon footprint based on
+factors like transportation, electricity usage, waste production etc..." --test
+"Jina AI") [//]: # (```) [//]: # () [//]: # (### Real Estate Valuation
+Estimator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Create a
+microservice that estimates the value of a property based on factors like
+location, property type, age, and square footage." --test "Berlin
+Friedrichshain, Flat, 100mÂ², 10 years old") [//]: # (```) [//]: # () [//]: #
+(### Gene Sequence Alignment) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Align two DNA or RNA sequences using the Needleman-Wunsch
+algorithm" --test "AGTC, GTCA") [//]: # (```) [//]: # () [//]: # (### Barcode
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Generate
+a barcode from a string" --test "Hello, welcome to Dev-GPT!") [//]: # (```) [//
+]: # () [//]: # (### File Compression) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Compress a file using the gzip algorithm" --test
+"content of the file: Hello, welcome to Dev-GPT!") [//]: # (```) [//]: # () [//
+]: # (### Watermarking Images) [//]: # (```bash) [//]: # (dev-gpt generate --
+description "Add a watermark (Dev-GPT) to an image" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### File Metadata Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract metadata from a file" --test "https://
+images.unsplash.com/photo-1602738328654-51ab2ae6c4ff") [//]: # (```) [//]: # ()
+[//]: # (### Video Thumbnail Extractor) [//]: # (```bash) [//]: # (dev-gpt
+generate --description "Extract a thumbnail from a video" --test "http://
+techslides.com/demos/sample-videos/small.mp4") [//]: # (```) [//]: # () [//]: #
+(### Gif Maker) [//]: # (```bash) [//]: # (dev-gpt generate --description
+"Create a gif from a list of images" --test "https://images.unsplash.com/photo-
 1564725075388-cc8338732289, https://images.unsplash.com/photo-1584555684040-
 bad07f46a21f, https://images.unsplash.com/photo-1584555613497-9ecf9dd06f68") [/
 /]: # (```) [//]: # () [//]: # () [//]: # (### Sound Visualizer) [//]: # () [//
-]: # (```bash) [//]: # (gptdeploy generate --description "Visualize a sound
-file and output the visualization as video combined with the sound" --test
-"some/mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: #
-(### Color Palette Generator) [//]: # (```bash) [//]: # (gptdeploy generate --
+]: # (```bash) [//]: # (dev-gpt generate --description "Visualize a sound file
+and output the visualization as video combined with the sound" --test "some/
+mp3/file.mp3") [//]: # (```) [//]: # (## Upcoming Challenges) [//]: # (###
+Color Palette Generator) [//]: # (```bash) [//]: # (dev-gpt generate --
 description "creates aesthetically pleasing color palettes based on a seed
 color, using color theory principles like complementary or analogous colors" --
 test "red") [//]: # (```) [//]: # () [//]: # (### Depth Map Generator) [//]: #
-(```bash) [//]: # (gptdeploy generate --description "Generate a depth map from
-a 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
+(```bash) [//]: # (dev-gpt generate --description "Generate a depth map from a
+3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### ASCII Art
-Generator) [//]: # (```bash) [//]: # (gptdeploy generate --description "Convert
+Generator) [//]: # (```bash) [//]: # (dev-gpt generate --description "Convert
 image to ASCII art" --test "https://images.unsplash.com/photo-1602738328654-
 51ab2ae6c4ff") [//]: # (```) [//]: # (generate --description "Get a png as
 input and return a vectorized version as svg." --test "Make sure when you
 convert the image back, it looks similar." --path microservice --verbose) ##
 Technical Insights The graphic below illustrates the process of creating a
 microservice and deploying it to the cloud elaboration two different
 implementation strategies. ```mermaid graph TB description[description:
@@ -183,54 +182,54 @@
 [implement strategy 1] implement1 --> build1{build image} build1 -->|error
 message| implement1 build1 -->|failed 10 times| implement2[implement strategy
 2] build1 -->|success| registry[push docker image to registry] implement2 --
 > build2{build image} build2 -->|error message| implement2 build2 -->|failed 10
 times| all_failed[all strategies failed] build2 -->|success| registry[push
 docker image to registry] registry --> deploy[deploy microservice] deploy --
 > streamlit[generate streamlit playground] streamlit --> user_run[user tests
-microservice] ``` 1. GPT Deploy identifies several strategies to implement your
+microservice] ``` 1. Dev-GPT identifies several strategies to implement your
 task. 2. It tests each strategy until it finds one that works. 3. For each
 strategy, it generates the following files: - microservice.py: This is the main
 implementation of the microservice. - test_microservice.py: These are test
 cases to ensure the microservice works as expected. - requirements.txt: This
 file lists the packages needed by the microservice and its tests. - Dockerfile:
 This file is used to run the microservice in a container and also runs the
-tests when building the image. 4. GPT Deploy attempts to build the image. If
-the build fails, it uses the error message to apply a fix and tries again to
-build the image. 5. Once it finds a successful strategy, it: - Pushes the
-Docker image to the registry. - Deploys the microservice. - Generates a
-Streamlit playground where you can test the microservice. 6. If it fails 10
-times in a row, it moves on to the next approach. ## ð® vision Use natural
-language interface to generate, deploy and update your microservice
-infrastructure. ## â¨ Contributors If you want to contribute to this project,
-feel free to open a PR or an issue. In the following, you can find a list of
-things that need to be done. next steps: - [ ] check if windows and linux
-support works - [ ] add video to README.md - [ ] bug: it can happen that the
-code generation is hanging forever - in this case aboard and redo the
-generation - [ ] new user has free credits but should be told to verify account
-Nice to have: - [ ] smooth rendering animation of the responses - [ ] if the
-user runs gptdeploy without any arguments, show the help message - [ ] don't
-show this message: ð You are logged in to Jina AI as florian.hoenicke
-(username:auth0-unified-448f11965ce142b6). To log out, use jina auth logout. -
-[ ] put the playground into the custom gateway (without rebuilding the custom
-gateway) - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] add more examples to README.md - [ ]
-support multiple endpoints - example: todolist microservice with endpoints for
-adding, deleting, and listing todos - [ ] support stateful microservices - [ ]
-The playground is currently printed twice even if it did not change. Make sure
-it is only printed twice in case it changed. - [ ] allow to update your
-microservice by providing feedback - [ ] support for other large language
-models like Open Assistent - [ ] for cost savings, it should be possible to
-insert less context during the code generation of the main functionality - no
-jina knowledge is required - [ ] use gptdeploy list to show all deployments -
-[ ] gptdeploy delete to delete a deployment - [ ] gptdeploy update to update a
-deployment - [ ] test param optional - in case the test param is not there
-first ask gpt if more information is required to write a test - like access to
-pdf data - [ ] section for microservices built by the community - [ ] test
-feedback for playground generation (could be part of the debugging) - [ ]
-should we send everything via json in the text attribute for simplicity? - [ ]
-fix release workflow - [ ] after the user specified the task, ask them
-questions back if the task is not clear enough or something is missing
-Proposal: - [ ] just generate the non-jina related code and insert it into an
-executor template - [ ] think about strategies after the first approach failed?
+tests when building the image. 4. Dev-GPT attempts to build the image. If the
+build fails, it uses the error message to apply a fix and tries again to build
+the image. 5. Once it finds a successful strategy, it: - Pushes the Docker
+image to the registry. - Deploys the microservice. - Generates a Streamlit
+playground where you can test the microservice. 6. If it fails 10 times in a
+row, it moves on to the next approach. ## ð® vision Use natural language
+interface to generate, deploy and update your microservice infrastructure. ##
+â¨ Contributors If you want to contribute to this project, feel free to open a
+PR or an issue. In the following, you can find a list of things that need to be
+done. next steps: - [ ] check if windows and linux support works - [ ] add
+video to README.md - [ ] bug: it can happen that the code generation is hanging
+forever - in this case aboard and redo the generation - [ ] new user has free
+credits but should be told to verify account Nice to have: - [ ] smooth
+rendering animation of the responses - [ ] if the user runs dev-gpt without any
+arguments, show the help message - [ ] don't show this message: ð You are
+logged in to Jina AI as florian.hoenicke (username:auth0-unified-
+448f11965ce142b6). To log out, use jina auth logout. - [ ] put the playground
+into the custom gateway (without rebuilding the custom gateway) - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] support for other large language models like Open Assistent -
+[ ] for cost savings, it should be possible to insert less context during the
+code generation of the main functionality - no jina knowledge is required - [ ]
+use dev-gpt list to show all deployments - [ ] dev-gpt delete to delete a
+deployment - [ ] dev-gpt update to update a deployment - [ ] test param
+optional - in case the test param is not there first ask gpt if more
+information is required to write a test - like access to pdf data - [ ] section
+for microservices built by the community - [ ] test feedback for playground
+generation (could be part of the debugging) - [ ] should we send everything via
+json in the text attribute for simplicity? - [ ] fix release workflow - [ ]
+after the user specified the task, ask them questions back if the task is not
+clear enough or something is missing Proposal: - [ ] just generate the non-jina
+related code and insert it into an executor template - [ ] think about
+strategies after the first approach failed?
```

### Comparing `dev-gpt-0.18.35.dev43/setup.py` & `dev-gpt-0.18.35.dev49/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 try:
-    libinfo_py = path.join('src', '__init__.py')
+    libinfo_py = path.join('dev_gpt', '__init__.py')
     libinfo_content = open(libinfo_py, 'r', encoding='utf8').readlines()
     version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][
         0
     ]
     exec(version_line)  # gives __version__
 except FileNotFoundError:
     __version__ = '0.0.0'
@@ -22,22 +22,22 @@
     name='dev-gpt',
     version=__version__,
     description='Use natural language interface to generate, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
-    url='https://github.com/jina-ai/gptdeploy',
+    url='https://github.com/jina-ai/dev-gpt',
     packages=find_packages(),
     include_package_data=True,
     install_requires=read_requirements(),
-    scripts=['gptdeploy.py'],
+    scripts=['dev_gpt.py'],
     entry_points={
         'console_scripts': [
-            'gptdeploy = src:main',
+            'dev-gpt = dev_gpt:main',
         ],
     },
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dev-gpt-0.18.35.dev43/src/apis/gpt.py` & `dev-gpt-0.18.35.dev49/dev_gpt/apis/gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from langchain.chat_models import ChatOpenAI
 from openai.error import RateLimitError
 from langchain.schema import HumanMessage, SystemMessage, BaseMessage, AIMessage
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from requests.exceptions import ConnectionError, ChunkedEncodingError
 from urllib3.exceptions import InvalidChunkLength
 
-from src.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
+from dev_gpt.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
     PRICING_GPT3_5_TURBO_GENERATION, CHARS_PER_TOKEN
-from src.options.generate.templates_system import template_system_message_base
-from src.utils.string_tools import print_colored
+from dev_gpt.options.generate.templates_system import template_system_message_base
+from dev_gpt.utils.string_tools import print_colored
 
 
 def configure_openai_api_key():
     if 'OPENAI_API_KEY' not in os.environ:
         print_colored('You need to set OPENAI_API_KEY in your environment.', '''
 Run:
-gptdeploy configure --key <your_openai_api_key>
+dev-gpt configure --key <your_openai_api_key>
 
 If you have updated it already, please restart your terminal.
 ''', 'red')
         exit(1)
     openai.api_key = os.environ['OPENAI_API_KEY']
 
 class GPTSession:
```

### Comparing `dev-gpt-0.18.35.dev43/src/apis/jina_cloud.py` & `dev-gpt-0.18.35.dev49/dev_gpt/apis/jina_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import click
 import hubble
 import requests
 from hubble.executor.helper import upload_file, archive_package, get_full_version
 from jcloud.flow import CloudFlow
 from jina import Flow
 
-from src.constants import DEMO_TOKEN
-from src.utils.io import suppress_stdout, is_docker_running
-from src.utils.string_tools import print_colored
+from dev_gpt.constants import DEMO_TOKEN
+from dev_gpt.utils.io import suppress_stdout, is_docker_running
+from dev_gpt.utils.string_tools import print_colored
 
 
 def wait_until_app_is_ready(url):
     is_app_ready = False
     while not is_app_ready:
         try:
             response = requests.get(url)
@@ -38,28 +38,28 @@
     url = f"{host}/playground"
     wait_until_app_is_ready(url)
     webbrowser.open(url, new=2)
 
 
 def redirect_callback(href):
     print(
-        f'You need login to Jina first to use GPTDeploy\n'
+        f'You need login to Jina first to use Dev GPT\n'
         f'Please open this link if it does not open automatically in your browser: {href}'
     )
     webbrowser.open(href, new=0, autoraise=True)
 
 
 def jina_auth_login():
     try:
         hubble.Client(jsonify=True).get_user_info(log_error=False)
     except hubble.AuthenticationRequiredError:
-        print('You need login to Jina first to use GPTDeploy')
+        print('You need login to Jina first to use dev-gpt')
         print_colored('', '''
 If you just created an account, it can happen that the login callback is not working.
-In this case, please cancel this run, rerun your gptdeploy command and login into your account again. 
+In this case, please cancel this run, rerun your dev-gpt command and login into your account again. 
 ''', 'green'
                       )
         hubble.login(prompt='login', redirect_callback=redirect_callback)
 
 
 def push_executor(dir_path):
     for i in range(3):
@@ -162,17 +162,17 @@
         except Exception as e:
             print(f'Could not deploy on Jina Cloud. Trying again in 5 seconds. Error: {e}')
             time.sleep(5)
         except SystemExit as e:
             raise SystemExit(f'''
 Looks like you either ran out of credits or something went wrong in the generation and we didn't catch it.
 To check if you ran out of credits, please go to https://cloud.jina.ai.
-If you have credits left, please create an issue here https://github.com/jina-ai/gptdeploy/issues/new/choose
+If you have credits left, please create an issue here https://github.com/jina-ai/dev-gpt/issues/new/choose
 and add details on the microservice you are trying to create.
-In that case, you can upgrade your GPT Deploy version, if not using latest, and try again.
+In that case, you can upgrade your Dev-GPT version, if not using latest, and try again.
 ''') from e
     if i == 2:
         raise Exception('''
 Could not deploy on Jina Cloud. 
 This can happen when the microservice is buggy, if it requires too much memory or if the Jina Cloud is overloaded. 
 Please try again later.
 '''
@@ -196,15 +196,15 @@
     else:
         click.echo('''
 Docker daemon doesn\'t seem to be running (possible reasons: incorrect docker installation, docker command isn\'t in system path, insufficient permissions, docker is running but unrespnsive).
 It might be important to run your microservice within a docker container.
 Your machine might not have all the dependencies installed.
 You have 3 options:
 a) start the docker daemon
-b) run gptdeploy deploy... to deploy your microservice on Jina Cloud. All dependencies will be installed there.
+b) run dev-gpt deploy... to deploy your microservice on Jina Cloud. All dependencies will be installed there.
 c) try to run your microservice locally without docker. It is worth a try but might fail.
 '''
                    )
         user_input = click.prompt('Do you want to run your microservice locally without docker? (Y/n)', type=str, default='y')
         if user_input.lower() != 'y':
             exit(1)
         use_docker = False
```

### Comparing `dev-gpt-0.18.35.dev43/src/apis/pypi.py` & `dev-gpt-0.18.35.dev49/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/cli.py` & `dev-gpt-0.18.35.dev49/dev_gpt/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from src import env  # noqa: F401 to make sure certain environment variables are set
+from dev_gpt import env  # noqa: F401 to make sure certain environment variables are set
 import functools
 import os
 
 import click
 
-from src.apis.gpt import configure_openai_api_key
-from src.apis.jina_cloud import jina_auth_login
-from src.options.configure.key_handling import set_api_key
+from dev_gpt.apis.gpt import configure_openai_api_key
+from dev_gpt.apis.jina_cloud import jina_auth_login
+from dev_gpt.options.configure.key_handling import set_api_key
 
 def openai_api_key_needed(func):
     def wrapper(*args, **kwargs):
         configure_openai_api_key()
         return func(*args, **kwargs)
     return wrapper
 
@@ -21,15 +21,15 @@
             return func(*args, **kwargs)
         except Exception as e:
             raise type(e)(f'''
 {str(e)}
 
 😱😱😱 Sorry for this experience. 
 Could you please report an issue about this on our github repo? We'll try to fix it asap.
-https://github.com/jina-ai/gptdeploy/issues/new
+https://github.com/jina-ai/dev-gpt/issues/new
 ''') from e
     return wrapper
 
 def path_param(func):
     @click.option('--path', default='microservice', help='Path to the generated microservice.')
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
@@ -64,33 +64,33 @@
     path = os.path.expanduser(path)
     path = os.path.abspath(path)
     if os.path.exists(path):
         if os.listdir(path):
             click.echo(f"Error: The path {path} you provided via --path is not empty. Please choose a directory that does not exist or is empty.")
             return
 
-    from src.options.generate.generator import Generator
+    from dev_gpt.options.generate.generator import Generator
     generator = Generator(description, path=path, model=model)
     generator.generate()
 
 @openai_api_key_needed
 @main.command()
 @path_param
 def run(path):
-    from src.options.run import Runner
+    from dev_gpt.options.run import Runner
     path = os.path.expanduser(path)
     path = os.path.abspath(path)
     Runner().run(path)
 
 @openai_api_key_needed
 @main.command()
 @path_param
 def deploy(path):
     jina_auth_login()
-    from src.options.deploy.deployer import Deployer
+    from dev_gpt.options.deploy.deployer import Deployer
     path = os.path.expanduser(path)
     path = os.path.abspath(path)
     Deployer().deploy(path)
 
 @main.command()
 @click.option('--key', required=True, help='Your OpenAI API key.')
 def configure(key):
```

### Comparing `dev-gpt-0.18.35.dev43/src/constants.py` & `dev-gpt-0.18.35.dev49/dev_gpt/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DOCKER_BASE_IMAGE_VERSION = '0.0.4'
+DOCKER_BASE_IMAGE_VERSION = '0.0.6'
 
 EXECUTOR_FILE_NAME = '__init__.py'
 IMPLEMENTATION_FILE_NAME = 'microservice.py'
 TEST_EXECUTOR_FILE_NAME = 'test_microservice.py'
 REQUIREMENTS_FILE_NAME = 'requirements.txt'
 DOCKER_FILE_NAME = 'Dockerfile'
 CLIENT_FILE_NAME = 'client.py'
```

### Comparing `dev-gpt-0.18.35.dev43/src/options/__init__.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from src.constants import REQUIREMENTS_FILE_NAME, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, TEST_EXECUTOR_FILE_NAME
+from dev_gpt.constants import REQUIREMENTS_FILE_NAME, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, TEST_EXECUTOR_FILE_NAME
 
 
 def list_dirs_no_hidden(path):
     """
     List all non-hidden directories in the specified path.
 
     :param path: str, optional (default is '.')
@@ -37,15 +37,15 @@
 
 def validate_folder_is_correct(microservice_path):
     if not os.path.exists(microservice_path):
         raise ValueError(f'Path {microservice_path} does not exist')
     if not os.path.isdir(microservice_path):
         raise ValueError(f'Path {microservice_path} is not a directory')
     if len(list_dirs_no_hidden(microservice_path)) == 0:
-        raise ValueError(f'Path {microservice_path} is empty. Please generate a microservice first. Type `gptdeploy generate` for further instructions.')
+        raise ValueError(f'Path {microservice_path} is empty. Please generate a microservice first. Type `dev-gpt generate` for further instructions.')
     if len(list_dirs_no_hidden(microservice_path)) > 1:
         raise ValueError(f'Path {microservice_path} needs to contain only one folder. Please make sure that you only have one microservice in this folder.')
     latest_version_path = get_latest_version_path(microservice_path)
     required_files = [
         'gateway/app.py',
         REQUIREMENTS_FILE_NAME,
         DOCKER_FILE_NAME,
```

### Comparing `dev-gpt-0.18.35.dev43/src/options/configure/key_handling.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/generator.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 from typing import Callable
 from typing import List, Text, Optional
 
 from langchain import PromptTemplate
 from langchain.schema import SystemMessage, HumanMessage, AIMessage
 from pydantic.dataclasses import dataclass
 
-from src.apis import gpt
-from src.apis.gpt import _GPTConversation
-from src.apis.jina_cloud import process_error_message, push_executor, is_executor_in_hub
-from src.apis.pypi import is_package_on_pypi, get_latest_package_version, clean_requirements_txt
-from src.constants import FILE_AND_TAG_PAIRS, NUM_IMPLEMENTATION_STRATEGIES, MAX_DEBUGGING_ITERATIONS, \
+from dev_gpt.apis import gpt
+from dev_gpt.apis.gpt import _GPTConversation
+from dev_gpt.apis.jina_cloud import process_error_message, push_executor, is_executor_in_hub
+from dev_gpt.apis.pypi import is_package_on_pypi, get_latest_package_version, clean_requirements_txt
+from dev_gpt.constants import FILE_AND_TAG_PAIRS, NUM_IMPLEMENTATION_STRATEGIES, MAX_DEBUGGING_ITERATIONS, \
     BLACKLISTED_PACKAGES, EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_TAG, \
     REQUIREMENTS_FILE_NAME, REQUIREMENTS_FILE_TAG, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, \
     IMPLEMENTATION_FILE_TAG, LANGUAGE_PACKAGES, UNNECESSARY_PACKAGES, DOCKER_BASE_IMAGE_VERSION
-from src.options.generate.templates_system import system_task_iteration, system_task_introduction, system_test_iteration
-from src.options.generate.templates_user import template_generate_microservice_name, \
+from dev_gpt.options.generate.templates_system import system_task_iteration, system_task_introduction, system_test_iteration
+from dev_gpt.options.generate.templates_user import template_generate_microservice_name, \
     template_generate_possible_packages, \
     template_solve_code_issue, \
     template_solve_pip_dependency_issue, template_is_dependency_issue, template_generate_playground, \
     template_generate_function, template_generate_test, template_generate_requirements, \
     template_chain_of_thought, template_summarize_error, \
     template_solve_apt_get_dependency_issue, template_pm_task_iteration, \
     template_pm_test_iteration
-from src.options.generate.ui import get_random_employee
-from src.utils.io import persist_file, get_all_microservice_files_with_content, get_microservice_path
-from src.utils.string_tools import print_colored
+from dev_gpt.options.generate.ui import get_random_employee
+from dev_gpt.utils.io import persist_file, get_all_microservice_files_with_content, get_microservice_path
+from dev_gpt.utils.string_tools import print_colored
 
 
 @dataclass
 class TaskSpecification:
     task: Optional[Text]
     test: Optional[Text]
 
@@ -144,15 +144,15 @@
     ):
         MICROSERVICE_FOLDER_v1 = get_microservice_path(self.microservice_root_path, microservice_name, packages,
                                                        num_approach, 1)
         os.makedirs(MICROSERVICE_FOLDER_v1)
 
         with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'jina_wrapper.py'), 'r', encoding='utf-8') as f:
             microservice_executor_boilerplate = f.read()
-        microservice_executor_code = microservice_executor_boilerplate.replace('class GPTDeployExecutor(Executor):',
+        microservice_executor_code = microservice_executor_boilerplate.replace('class DevGPTExecutor(Executor):',
                                                                                f'class {microservice_name}(Executor):')
         persist_file(microservice_executor_code, os.path.join(MICROSERVICE_FOLDER_v1, EXECUTOR_FILE_NAME))
 
         with open(os.path.join(os.path.dirname(__file__), 'static_files', 'microservice', 'apis.py'), 'r', encoding='utf-8') as f:
             persist_file(f.read(), os.path.join(MICROSERVICE_FOLDER_v1, 'apis.py'))
 
         microservice_content = self.generate_and_persist_file(
@@ -190,15 +190,15 @@
             }),
             file_name_purpose=REQUIREMENTS_FILE_NAME,
             file_name_s=[REQUIREMENTS_FILE_NAME],
             parse_result_fn=self.parse_result_fn_requirements,
             tag_name=REQUIREMENTS_FILE_TAG,
         )[REQUIREMENTS_FILE_NAME]
 
-        # I deactivated this because 3.5-turbo was halucinating packages that were not needed
+        # I deactivated this because 3.5-turbo was hallucinating packages that were not needed
         # now, in the first iteration the default dockerfile is used
         # self.generate_and_persist_file(
         #     section_title='Generate Dockerfile',
         #     template=template_generate_apt_get_install,
         #     destination_folder=MICROSERVICE_FOLDER_v1,
         #     file_name_s=None,
         #     parse_result_fn=self.parse_result_fn_dockerfile,
@@ -445,16 +445,16 @@
                     print_colored('',
                                   f'Could not debug the Microservice with any of the approaches: {packages} giving up.',
                                   'red')
                     return -1
                 continue
             print(f'''
 You can now run or deploy your microservice:
-gptdeploy run --path {self.microservice_root_path}
-gptdeploy deploy --path {self.microservice_root_path}
+dev-gpt run --path {self.microservice_root_path}
+dev-gpt deploy --path {self.microservice_root_path}
 '''
                   )
             return 0
 
     def summarize_error(self, error):
         conversation = self.gpt_session.get_conversation()
         error_summary = conversation.chat(template_summarize_error.format(error=error))
```

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/templates_system.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.options.generate.templates_user import not_allowed_docker_string, not_allowed_function_string
+from dev_gpt.options.generate.templates_user import not_allowed_docker_string, not_allowed_function_string
 
 
 template_system_message_base = f'''It is September 2021. 
 You are a principal engineer working at Jina - an open source company.
 You accurately satisfy all of the user's requirements.
 To be more specific, you help the user to build a microservice with the following requirements:
 ```
```

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/templates_user.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from langchain import PromptTemplate
 
-from src.constants import IMPLEMENTATION_FILE_NAME
+from dev_gpt.constants import IMPLEMENTATION_FILE_NAME
 
 general_guidelines_string = '''The code you write is production ready. Every file starts with comments describing what the code is doing before the first import. Comments can only be written within code blocks.
 Then all imports are listed.
 
 Start from top-level and then fully implement all methods.'''
 
 
@@ -341,29 +341,29 @@
 {code_files_wrapped}
 
 Create a playground for the executor {microservice_name} using streamlit.
 The playground must look like it was made by a professional designer.
 All the ui elements are well thought out to make them visually appealing and easy to use.
 Don't mention the word Playground in the title.
 The playground contains many emojis that fit the theme of the playground and has an emoji as favicon.
-The playground encourages the user to deploy their own microservice by clicking on this link: https://github.com/jina-ai/gptdeploy
+The playground encourages the user to deploy their own microservice by clicking on this link: https://github.com/jina-ai/dev-gpt
 The playground uses the following code to send a request to the microservice:
 ```
 from jina import Client, Document, DocumentArray
 client = Client(host='http://localhost:8080')
 d = Document(text=json.dumps(INPUT_DICTIONARY)) # fill-in dictionary which takes input
 response = client.post('/', inputs=DocumentArray([d])) # always use '/'
 print(response[0].text) # can also be blob in case of image/audio..., this should be visualized in the streamlit app
 ```
 Note that the response will always be in response[0].text
 The playground displays a code block containing the microservice specific curl code that can be used to send the request to the microservice.
 While the exact payload in the curl might change, the host and deployment ID always stay the same. Example: 
 ```
 deployment_id = os.environ.get("K8S_NAMESPACE_NAME", "")
-host = f'https://gptdeploy-{{deployment_id.split("-")[1]}}.wolf.jina.ai/post' if deployment_id else "http://localhost:8080/post"
+host = f'https://dev-gpt-{{deployment_id.split("-")[1]}}.wolf.jina.ai/post' if deployment_id else "http://localhost:8080/post"
 with st.expander("See curl command"):
     st.code(
         f'curl -X \\'POST\\' \\'host\\' -H \\'accept: application/json\\' -H \\'Content-Type: application/json\\' -d \\'{{{{"data": [{{{{"text": "hello, world!"}}}}]}}}}\\'',
         language='bash'
     )
 ```
 You must provide the complete app.py file using the following syntax to wrap the code:
```

### Comparing `dev-gpt-0.18.35.dev43/src/options/generate/ui.py` & `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/utils/io.py` & `dev-gpt-0.18.35.dev49/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/src/utils/string_tools.py` & `dev-gpt-0.18.35.dev49/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev43/test/integration/test_generator.py` & `dev-gpt-0.18.35.dev49/test/integration/test_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import pytest
 
-from src.options.generate.generator import Generator
+from dev_gpt.options.generate.generator import Generator
 
 
 # The cognitive difficulty level is determined by the number of requirements the microservice has.
 
 def test_generation_level_0(tmpdir):
     """
     Requirements:
```

### Comparing `dev-gpt-0.18.35.dev43/test/unit/test_api.py` & `dev-gpt-0.18.35.dev49/test/unit/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
-from src.apis.jina_cloud import is_executor_in_hub
-from src.apis.pypi import is_package_on_pypi, clean_requirements_txt
-from src.options.generate.generator import Generator
+from dev_gpt.apis.jina_cloud import is_executor_in_hub
+from dev_gpt.apis.pypi import is_package_on_pypi, clean_requirements_txt
+from dev_gpt.options.generate.generator import Generator
 
 
 def test_is_microservice_in_hub():
     assert is_executor_in_hub('reoihoflsnvoiawejeruhvflsfk') is False
     assert is_executor_in_hub('CLIPImageEncoder') is True
```

### Comparing `dev-gpt-0.18.35.dev43/test/unit/test_response_parsing.py` & `dev-gpt-0.18.35.dev49/test/unit/test_response_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from src.options.generate.generator import Generator
+from dev_gpt.options.generate.generator import Generator
 
 def create_code_block(with_backticks, asterisks, with_highlight_info, file_name, start_inline, content):
     code_block = f'''
 {{
     "content": "{content}",
 }}
 '''
```

