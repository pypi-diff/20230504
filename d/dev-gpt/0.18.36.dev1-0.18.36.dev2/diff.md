# Comparing `tmp/dev-gpt-0.18.36.dev1.tar.gz` & `tmp/dev-gpt-0.18.36.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.36.dev1.tar", last modified: Thu May  4 19:06:26 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.36.dev2.tar", last modified: Thu May  4 19:11:43 2023, max compression
```

## Comparing `dev-gpt-0.18.36.dev1.tar` & `dev-gpt-0.18.36.dev2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.784942 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 19:06:26.000000 dev-gpt-0.18.36.dev1/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/dev_gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:26.788942 dev-gpt-0.18.36.dev1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 19:06:22.000000 dev-gpt-0.18.36.dev1/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.817221 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 19:11:43.000000 dev-gpt-0.18.36.dev2/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/dev_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:43.821221 dev-gpt-0.18.36.dev2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 19:11:39.000000 dev-gpt-0.18.36.dev2/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.36.dev1/LICENSE` & `dev-gpt-0.18.36.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/PKG-INFO` & `dev-gpt-0.18.36.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.36.dev1
+Version: 0.18.36.dev2
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -15,22 +15,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-Dev GPT : One line to generate them all 🧙🚀
+Dev GPT: Your Automated Development Team
 </h1>
 
+<div align="center">
+<table>
+  <tr>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/product.png" alt="Product Manager" width="130" /><br>
+      <em>Product Manager</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/engineer.png" alt="Developer" width="130" /><br>
+      <em>Developer</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/dev-ops.png" alt="DevOps" width="130" /><br>
+      <em>DevOps</em>
+    </td>
+  </tr>
+</table>
+</div>
+
 <p align="center">
-<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
-</p>
-<p align="center">
-Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
+Tell your AI team what microservice you want to build, and they will do it for you.
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
@@ -49,21 +65,21 @@
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
+</p>
+
+Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 [//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
-</p>
-This project streamlines the creation and deployment of AI-powered microservices. 
-Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-You get guidance from our three agents:
+
 
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev1 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev2 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE
-        ****** Dev GPT : One line to generate them all ð§ð ******
-                                [Jina NOW logo]
-  Turn your natural language descriptions into fully functional, deployed AI-
-  powered microservices with a single command! Your imagination is the limit!
+            ****** Dev GPT: Your Automated Development Team ******
+                    [Product Manager] [Developer] [DevOps]
+                     Product Manager   Developer   DevOps
+Tell your AI team what microservice you want to build, and they will do it for
+                      you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
- thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
-                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
-This project streamlines the creation and deployment of AI-powered
-microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. You get guidance from
-our three agents: ## Quickstart ### Requirements - OpenAI key with access to
-GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
---key  ``` If you set the environment variable `OPENAI_API_KEY`, the
-configuration step can be skipped. Your api key must have access to gpt-4 to
-use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
-Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
+                     platforms] [Downloads] [Discord_Chat]
+Welcome to Dev GPT, where we bring your ideas to life with the power of
+advanced artificial intelligence! Our automated development team is designed to
+create microservices tailored to your specific needs, making your software
+development process seamless and efficient. Comprised of a virtual Product
+Manager, Developer, and DevOps, our AI team ensures that every aspect of your
+project is covered, from concept to deployment. [//]: # ([![Watch the video]
+(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
+231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
+Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
+```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+Your api key must have access to gpt-4 to use this tool. We are working on a
+way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
+generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.36.dev1/README.md` & `dev-gpt-0.18.36.dev2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 <h1 align="center">
-Dev GPT : One line to generate them all 🧙🚀
+Dev GPT: Your Automated Development Team
 </h1>
 
+<div align="center">
+<table>
+  <tr>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/product.png" alt="Product Manager" width="130" /><br>
+      <em>Product Manager</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/engineer.png" alt="Developer" width="130" /><br>
+      <em>Developer</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/dev-ops.png" alt="DevOps" width="130" /><br>
+      <em>DevOps</em>
+    </td>
+  </tr>
+</table>
+</div>
+
 <p align="center">
-<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
-</p>
-<p align="center">
-Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
+Tell your AI team what microservice you want to build, and they will do it for you.
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
@@ -29,21 +45,21 @@
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
+</p>
+
+Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 [//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
-</p>
-This project streamlines the creation and deployment of AI-powered microservices. 
-Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-You get guidance from our three agents:
+
 
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
-        ****** Dev GPT : One line to generate them all ð§ð ******
-                                [Jina NOW logo]
-  Turn your natural language descriptions into fully functional, deployed AI-
-  powered microservices with a single command! Your imagination is the limit!
+            ****** Dev GPT: Your Automated Development Team ******
+                    [Product Manager] [Developer] [DevOps]
+                     Product Manager   Developer   DevOps
+Tell your AI team what microservice you want to build, and they will do it for
+                      you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
- thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
-                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
-This project streamlines the creation and deployment of AI-powered
-microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. You get guidance from
-our three agents: ## Quickstart ### Requirements - OpenAI key with access to
-GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
---key  ``` If you set the environment variable `OPENAI_API_KEY`, the
-configuration step can be skipped. Your api key must have access to gpt-4 to
-use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
-Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
+                     platforms] [Downloads] [Discord_Chat]
+Welcome to Dev GPT, where we bring your ideas to life with the power of
+advanced artificial intelligence! Our automated development team is designed to
+create microservices tailored to your specific needs, making your software
+development process seamless and efficient. Comprised of a virtual Product
+Manager, Developer, and DevOps, our AI team ensures that every aspect of your
+project is covered, from concept to deployment. [//]: # ([![Watch the video]
+(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
+231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
+Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
+```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+Your api key must have access to gpt-4 to use this tool. We are working on a
+way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
+generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.36.dev2/dev_gpt/apis/gpt.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.36.dev2/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.36.dev2/dev_gpt/apis/pypi.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/cli.py` & `dev-gpt-0.18.36.dev2/dev_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/constants.py` & `dev-gpt-0.18.36.dev2/dev_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/__init__.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/templates_user.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.36.dev2/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/utils/io.py` & `dev-gpt-0.18.36.dev2/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.36.dev2/dev_gpt/utils/string_tools.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.36.dev2/dev_gpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.36.dev1
+Version: 0.18.36.dev2
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -15,22 +15,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
-Dev GPT : One line to generate them all 🧙🚀
+Dev GPT: Your Automated Development Team
 </h1>
 
+<div align="center">
+<table>
+  <tr>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/product.png" alt="Product Manager" width="130" /><br>
+      <em>Product Manager</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/engineer.png" alt="Developer" width="130" /><br>
+      <em>Developer</em>
+    </td>
+    <td align="center" style="padding: 0 10px;">
+      <img src="res/team/dev-ops.png" alt="DevOps" width="130" /><br>
+      <em>DevOps</em>
+    </td>
+  </tr>
+</table>
+</div>
+
 <p align="center">
-<img src="res/dev-gpt-logo.png" alt="Jina NOW logo" width="150px">
-</p>
-<p align="center">
-Turn your natural language descriptions into fully functional, deployed AI-powered microservices with a single command!
+Tell your AI team what microservice you want to build, and they will do it for you.
 Your imagination is the limit!
 </p>
 
 <p align="center">
 <a href="https://github.com/tiangolo/fastapi/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
     <img src="https://github.com/tiangolo/fastapi/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
 </a>
@@ -49,21 +65,21 @@
 <a href="https://pypistats.org/packages/dev-gpt" target="_blank">
     <img src="https://img.shields.io/pypi/dm/dev-gpt?color=%2334D058&label=pypi%20downloads" alt="Downloads">
 </a>
 <a href="https://discord.gg/ESn8ED6Fyn" target="_blank">
     <img src="https://img.shields.io/badge/chat_on-Discord-7289DA?logo=discord&logoColor=white" alt="Discord Chat">
 </a>
 
+</p>
+
+Welcome to Dev GPT, where we bring your ideas to life with the power of advanced artificial intelligence! Our automated development team is designed to create microservices tailored to your specific needs, making your software development process seamless and efficient. Comprised of a virtual Product Manager, Developer, and DevOps, our AI team ensures that every aspect of your project is covered, from concept to deployment.
 
 [//]: # ([![Watch the video]&#40;res/thumbnail.png&#41;]&#40;https://user-images.githubusercontent.com/11627845/231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4&#41;)
 
-</p>
-This project streamlines the creation and deployment of AI-powered microservices. 
-Simply describe your task using natural language, and the system will automatically build and deploy your microservice. 
-You get guidance from our three agents:
+
 
 
 ## Quickstart
 ### Requirements
 - OpenAI key with access to GPT-3.5 or GPT-4 
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev1 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.36.dev2 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE
-        ****** Dev GPT : One line to generate them all ð§ð ******
-                                [Jina NOW logo]
-  Turn your natural language descriptions into fully functional, deployed AI-
-  powered microservices with a single command! Your imagination is the limit!
+            ****** Dev GPT: Your Automated Development Team ******
+                    [Product Manager] [Developer] [DevOps]
+                     Product Manager   Developer   DevOps
+Tell your AI team what microservice you want to build, and they will do it for
+                      you. Your imagination is the limit!
   [Test] [Coverage] [Package_version] [Supported_Python_versions] [Supported
-    platforms] [Downloads] [Discord_Chat] [//]: # ([![Watch the video](res/
- thumbnail.png)](https://user-images.githubusercontent.com/11627845/231530421-
-                  272a66aa-4260-4e17-ab7a-ba66adca754c.mp4))
-This project streamlines the creation and deployment of AI-powered
-microservices. Simply describe your task using natural language, and the system
-will automatically build and deploy your microservice. You get guidance from
-our three agents: ## Quickstart ### Requirements - OpenAI key with access to
-GPT-3.5 or GPT-4 ### Installation ```bash pip install dev-gpt dev-gpt configure
---key  ``` If you set the environment variable `OPENAI_API_KEY`, the
-configuration step can be skipped. Your api key must have access to gpt-4 to
-use this tool. We are working on a way to use gpt-3.5-turbo as well. ###
-Generate Microservice ```bash dev-gpt generate \ --description "" \ --model
+                     platforms] [Downloads] [Discord_Chat]
+Welcome to Dev GPT, where we bring your ideas to life with the power of
+advanced artificial intelligence! Our automated development team is designed to
+create microservices tailored to your specific needs, making your software
+development process seamless and efficient. Comprised of a virtual Product
+Manager, Developer, and DevOps, our AI team ensures that every aspect of your
+project is covered, from concept to deployment. [//]: # ([![Watch the video]
+(res/thumbnail.png)](https://user-images.githubusercontent.com/11627845/
+231530421-272a66aa-4260-4e17-ab7a-ba66adca754c.mp4)) ## Quickstart ###
+Requirements - OpenAI key with access to GPT-3.5 or GPT-4 ### Installation
+```bash pip install dev-gpt dev-gpt configure --key  ``` If you set the
+environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+Your api key must have access to gpt-4 to use this tool. We are working on a
+way to use gpt-3.5-turbo as well. ### Generate Microservice ```bash dev-gpt
+generate \ --description "" \ --model
 5 or gpt-4> \ --path
 o/local/folder> ``` To generate your personal microservice two things are
 required: - A `description` of the task you want to accomplish. (optional) -
 The `model` you want to use - either `gpt-3.5` or `gpt-4`. `gpt-3.5` is ~10x
 cheaper, but will not be able to generate as complex microservices. (default:
 largest you have access to) - A `path` on the local drive where the
 microservice will be generated. (default: ./microservice) The creation process
```

### Comparing `dev-gpt-0.18.36.dev1/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.36.dev2/dev_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/setup.py` & `dev-gpt-0.18.36.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/test/integration/test_generator.py` & `dev-gpt-0.18.36.dev2/test/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/test/unit/test_api.py` & `dev-gpt-0.18.36.dev2/test/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.36.dev1/test/unit/test_response_parsing.py` & `dev-gpt-0.18.36.dev2/test/unit/test_response_parsing.py`

 * *Files identical despite different names*

