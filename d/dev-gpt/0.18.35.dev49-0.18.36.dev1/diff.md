# Comparing `tmp/dev-gpt-0.18.35.dev49.tar.gz` & `tmp/dev-gpt-0.18.36.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.35.dev49.tar", last modified: Thu May  4 18:47:47 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.36.dev1.tar", last modified: Thu May  4 19:06:26 2023, max compression
```

## Comparing `dev-gpt-0.18.35.dev49.tar` & `dev-gpt-0.18.36.dev1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.543457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 18:47:47.000000 dev-gpt-0.18.35.dev49/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/dev_gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.547457 dev-gpt-0.18.35.dev49/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:47.551457 dev-gpt-0.18.35.dev49/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 18:47:42.000000 dev-gpt-0.18.35.dev49/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.35.dev49/LICENSE` & `dev-gpt-0.18.36.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/PKG-INFO` & `dev-gpt-0.18.36.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.35.dev49
+Version: 0.18.36.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev49 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.35.dev49/README.md` & `dev-gpt-0.18.36.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.36.dev1/dev_gpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.36.dev1/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.36.dev1/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/cli.py` & `dev-gpt-0.18.36.dev1/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/constants.py` & `dev-gpt-0.18.36.dev1/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/__init__.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/utils/io.py` & `dev-gpt-0.18.36.dev1/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.36.dev1/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.36.dev1/dev_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.35.dev49
+Version: 0.18.36.dev1
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.35.dev49 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev1 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.35.dev49/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.36.dev1/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/setup.py` & `dev-gpt-0.18.36.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/test/integration/test_generator.py` & `dev-gpt-0.18.36.dev1/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/test/unit/test_api.py` & `dev-gpt-0.18.36.dev1/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.35.dev49/test/unit/test_response_parsing.py` & `dev-gpt-0.18.36.dev1/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

