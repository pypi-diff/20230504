# Comparing `tmp/grizzly-loadtester-2.6.3.tar.gz` & `tmp/grizzly-loadtester-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-2.6.3.tar", last modified: Fri Apr 21 06:49:19 2023, max compression
+gzip compressed data, was "grizzly-loadtester-2.6.4.tar", last modified: Thu May  4 07:58:47 2023, max compression
```

## Comparing `grizzly-loadtester-2.6.3.tar` & `grizzly-loadtester-2.6.4.tar`

### file list

```diff
@@ -1,325 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.010635 grizzly-loadtester-2.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.github/workflows/code-quality.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.pytest_tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.pytest_tmp/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/build.novella
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/content/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/assets/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_1024.png
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_16.png
--rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_256.png
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_48.png
--rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_512.png
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_64.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/command-line-interface/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/editor-support/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/vscode.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/licenses.md
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/example.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.014634 grizzly-loadtester-2.6.3/docs/content/framework/usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/environment-configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/templating.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/mkdocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/environments/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/example.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.014634 grizzly-loadtester-2.6.3/example/features/requests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/requests/books/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/requests/books/books.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/steps/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/steps/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26780 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/locust.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/scenarios/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.038634 grizzly-loadtester-2.6.3/grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    35217 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/async_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/until.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/types/
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/locust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/dummy_pymqi.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-21 06:49:19.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate-changelog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate-licenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate.bash
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    41596 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_iteration_pace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/test_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test__helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_async_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    32204 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_locust.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    44377 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_sb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.946077 grizzly-loadtester-2.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.github/workflows/code-quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.pytest_tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.pytest_tmp/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/build.novella
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.958078 grizzly-loadtester-2.6.4/docs/content/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_1024.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/command-line-interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.962078 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/editor-support/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/editors/vscode.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/editor-support/licenses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/example.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.946077 grizzly-loadtester-2.6.4/docs/content/framework/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/environment-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/templating.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/content/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/docs/mkdocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/environments/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/example.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.950078 grizzly-loadtester-2.6.4/example/features/requests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/requests/books/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/requests/books/books.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.966078 grizzly-loadtester-2.6.4/example/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/steps/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/features/steps/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/example/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/auth/aad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/listeners/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26965 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.970078 grizzly-loadtester-2.6.4/grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/scenarios/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/background/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.974078 grizzly-loadtester-2.6.4/grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35217 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/scenario/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/steps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.978078 grizzly-loadtester-2.6.4/grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/async_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.982078 grizzly-loadtester-2.6.4/grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/clients/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/tasks/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.982078 grizzly-loadtester-2.6.4/grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/types/locust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.986078 grizzly-loadtester-2.6.4/grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/base/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/users/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.990078 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26029 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/async_message/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/dummy_pymqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/grizzly_extras/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 07:58:46.000000 grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate-changelog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate-licenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/script/docs-generate.bash
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.994078 grizzly-loadtester-2.6.4/tests/e2e/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/e2e/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/steps/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_iteration_pace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/e2e/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38536 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:46.998078 grizzly-loadtester-2.6.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33819 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/auth/test_aad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/test_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.002078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.006078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test__helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_async_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32204 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.010078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.014078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.014078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:47.018078 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-04 07:57:37.000000 grizzly-loadtester-2.6.4/tests/webserver.py
```

### Comparing `grizzly-loadtester-2.6.3/.devcontainer/Dockerfile` & `grizzly-loadtester-2.6.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/.devcontainer/devcontainer.json` & `grizzly-loadtester-2.6.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/.github/workflows/code-quality.yaml` & `grizzly-loadtester-2.6.4/.github/workflows/code-quality.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
       run: python -m pip install -e .[dev]
 
     - name: install docker-compose
       id: install-docker-compose
       if: matrix.run_mode == 'dist'
       uses: KengoTODA/actions-setup-docker-compose@main
       with:
-        version: '1.29.2'
+        version: '2.17.2'
 
     - name: ssh agent
       id: ssh-agent
       run: |
         ssh-agent -a /tmp/ssh_auth_sock
 
     - name: 'pytest (e2e ${{ matrix.run_mode }})'
```

### Comparing `grizzly-loadtester-2.6.3/.github/workflows/release.yaml` & `grizzly-loadtester-2.6.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/.vscode/launch.json` & `grizzly-loadtester-2.6.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/LICENSE.md` & `grizzly-loadtester-2.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/PKG-INFO` & `grizzly-loadtester-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.3
+Version: 2.6.4
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.3/README.md` & `grizzly-loadtester-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/build.novella` & `grizzly-loadtester-2.6.4/docs/build.novella`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/favicon.ico` & `grizzly-loadtester-2.6.4/docs/content/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown.svg` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange.svg` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo.svg` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_1024.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_1024.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_128.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_128.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_16.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_16.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_256.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_256.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_32.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_32.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_48.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_48.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_512.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_512.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_64.png` & `grizzly-loadtester-2.6.4/docs/content/assets/logo/grizzly_logo_64.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/metadata.md` & `grizzly-loadtester-2.6.4/docs/content/command-line-interface/usage/metadata.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/editor-support/index.md` & `grizzly-loadtester-2.6.4/docs/content/editor-support/index.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/example.md` & `grizzly-loadtester-2.6.4/docs/content/example.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/environment-configuration.md` & `grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/environment-configuration.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/templating.md` & `grizzly-loadtester-2.6.4/docs/content/framework/usage/variables/templating.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/docs/mkdocs.yaml` & `grizzly-loadtester-2.6.4/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/example/features/environment.py` & `grizzly-loadtester-2.6.4/example/features/environment.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/example/features/example.feature` & `grizzly-loadtester-2.6.4/example/features/example.feature`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/example/features/steps/custom.py` & `grizzly-loadtester-2.6.4/example/features/steps/custom.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/example/features/steps/steps.py` & `grizzly-loadtester-2.6.4/example/features/steps/steps.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/behave.py` & `grizzly-loadtester-2.6.4/grizzly/behave.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from os import environ
 from typing import Any, Dict, Tuple, List, cast
 from time import perf_counter as time
 from datetime import datetime
 from pathlib import Path
 from json import loads as jsonloads
 
@@ -11,23 +13,22 @@
 from grizzly.types.behave import Context, Feature, Step, Scenario, Status
 
 from .context import GrizzlyContext
 from .testdata.variables import destroy_variables
 from .locust import run as locustrun, on_worker
 from .utils import catch, check_mq_client_logs, fail_direct, in_correct_section
 
+logger = logging.getLogger(__name__)
+
 try:
     import pymqi  # pylint: disable=unused-import
 except ModuleNotFoundError:
     from grizzly_extras import dummy_pymqi as pymqi
 
 
-last_task_count: Dict[str, int] = {}
-
-
 def before_feature(context: Context, feature: Feature, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
     # identify as grizzly, instead of behave
     proc.setproctitle('grizzly')
 
     environ['GRIZZLY_CONTEXT_ROOT'] = context.config.base_dir
     environ['GRIZZLY_FEATURE_FILE'] = feature.filename
 
@@ -45,19 +46,21 @@
 
     if persistent_file.exists():
         grizzly.state.persistent = jsonloads(persistent_file.read_text())
 
     context.grizzly = grizzly
     context.start = time()
     context.started = datetime.now().astimezone()
+    context.last_task_count = {}
 
 
 @catch(KeyboardInterrupt)
 def after_feature(context: Context, feature: Feature, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
     return_code: int
+    cause: str
 
     # all scenarios has been processed, let's run locust
     if feature.status == Status.passed:
         return_code = locustrun(context)
 
         if return_code != 0:
             feature.set_status(Status.failed)
@@ -67,33 +70,32 @@
             stats = grizzly.state.locust.environment.stats
 
             for behave_scenario in cast(List[Scenario], feature.scenarios):
                 grizzly_scenario = grizzly.scenarios.find_by_description(behave_scenario.name)
                 if grizzly_scenario is None:
                     continue
 
+                total_errors = 0
+                for error in stats.errors.values():
+                    if error.name.startswith(grizzly_scenario.identifier):
+                        total_errors += 1
+
                 scenario_stat = stats.get(grizzly_scenario.locust_name, RequestType.SCENARIO())
 
-                if scenario_stat.num_failures > 0 or scenario_stat.num_requests != grizzly_scenario.iterations:
+                if scenario_stat.num_failures > 0 or scenario_stat.num_requests != grizzly_scenario.iterations or total_errors > 0:
                     behave_scenario.set_status(Status.failed)
+                    return_code = 1
 
-                rindex = -1
+        if pymqi.__name__ != 'grizzly_extras.dummy_pymqi' and not on_worker(context):
+            check_mq_client_logs(context)
 
-                for stat in stats.entries.values():
-                    if stat.method == RequestType.SCENARIO() or not stat.name.startswith(f'{grizzly_scenario.identifier} '):
-                        continue
-
-                    if stat.num_failures > 0:
-                        rindex -= 1
-                        behave_step = cast(Step, behave_scenario.steps[rindex])
-                        behave_step.status = Status.failed
-
-            if pymqi.__name__ != 'grizzly_extras.dummy_pymqi' and not on_worker(context):
-                check_mq_client_logs(context)
+        if return_code != 0:
+            cause = 'locust test failed'
     else:
+        cause = 'failed to prepare locust test'
         return_code = 1
 
     if not on_worker(context):
         # show start and stop date time
         stopped = datetime.now().astimezone()
 
         print('')
@@ -104,14 +106,17 @@
         try:
             duration = int(time() - context.start)
 
             feature.scenarios[-1].steps[-1].duration = duration
         except Exception:
             pass
 
+        if return_code != 0:
+            raise RuntimeError(cause)
+
 
 def before_scenario(context: Context, scenario: Scenario, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
     grizzly = cast(GrizzlyContext, context.grizzly)
 
     if grizzly.state.background_section_done:
         scenario.background = None
     else:
@@ -135,16 +140,16 @@
 
         if not in_correct_section(matched_step.func, ['grizzly.steps.scenario', 'grizzly.steps']):
             # to get a nicer error message, the step should fail before it's executed, see before_step hook
             setattr(step, 'location_status', 'incorrect')
 
     grizzly.scenarios.create(scenario)
 
-    if grizzly.scenario.identifier not in last_task_count:
-        last_task_count[grizzly.scenario.identifier] = 0
+    if grizzly.scenario.identifier not in context.last_task_count:
+        context.last_task_count[grizzly.scenario.identifier] = 0
 
 
 def after_scenario(context: Context, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
     grizzly = cast(GrizzlyContext, context.grizzly)
 
     # first scenario is done, do not process background for any (possible) other scenarios
     if not grizzly.state.background_section_done:
@@ -169,12 +174,13 @@
 def after_step(context: Context, step: Step, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
     # grizzly does not have any functionality that should run after every step, but added for
     # clarity of what can be overloaded
     grizzly = cast(GrizzlyContext, context.grizzly)
 
     if len(grizzly.scenario.tasks._tmp.__stack__) == 0:
         task_index = len(grizzly.scenario.tasks)
+        last_task_index = context.last_task_count.get(grizzly.scenario.identifier, None)
 
-        if task_index > last_task_count[grizzly.scenario.identifier]:
-            last_task_count[grizzly.scenario.identifier] = task_index
-            # GrizzlyIterator offset by one, since it has an interal task
+        if last_task_index is not None and task_index > last_task_index:
+            context.last_task_count[grizzly.scenario.identifier] = task_index
+            # GrizzlyIterator offset by one, since it has an interal task which is not represented by a step
             grizzly.scenario.tasks.behave_steps.update({task_index + 1: f'{step.keyword} {step.name}'})
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/clients.py` & `grizzly-loadtester-2.6.4/grizzly/clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/context.py` & `grizzly-loadtester-2.6.4/grizzly/context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/exceptions.py` & `grizzly-loadtester-2.6.4/grizzly/exceptions.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/listeners/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/listeners/appinsights.py` & `grizzly-loadtester-2.6.4/grizzly/listeners/appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/listeners/influxdb.py` & `grizzly-loadtester-2.6.4/grizzly/listeners/influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/locust.py` & `grizzly-loadtester-2.6.4/grizzly/locust.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,17 +239,22 @@
     for scenario in grizzly.scenarios():
         stat = stats.get(scenario.locust_name, RequestType.SCENARIO())
         max_length_description = max(len(scenario.description or 'unknown'), max_length_description)
         max_length_iterations = max(len(f'{stat.num_requests}/{scenario.iterations or 0}'), max_length_iterations)
         max_length_status = max(len(Status.undefined.name) if stat.num_requests < 1 else len(Status.passed.name), max_length_status)
 
     for scenario in grizzly.scenarios():
+        total_errors = 0
+        for error in stats.errors.values():
+            if error.name.startswith(scenario.identifier):
+                total_errors += 1
+
         stat = stats.get(scenario.locust_name, RequestType.SCENARIO())
         if stat.num_requests > 0:
-            if stat.num_failures == 0 and stat.num_requests == scenario.iterations:
+            if stat.num_failures == 0 and stat.num_requests == scenario.iterations and total_errors == 0:
                 status = Status.passed
             else:
                 status = Status.failed
         else:
             status = Status.undefined
 
         description = scenario.description or 'unknown'
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/scenarios/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/scenarios/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,18 @@
         for task in self.tasks:
             if isinstance(task, grizzlytask):
                 task.on_start(self)
 
     def on_stop(self) -> None:
         for task in self.tasks:
             if isinstance(task, grizzlytask):
-                task.on_stop(self)
+                try:
+                    task.on_stop(self)
+                except Exception as e:
+                    self.logger.error(f'on_stop: {str(e)}', exc_info=True)
 
         self.consumer.stop()
         self.user.scenario_state = ScenarioState.STOPPED
 
 
 from .iterator import IteratorScenario
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/scenarios/iterator.py` & `grizzly-loadtester-2.6.4/grizzly/scenarios/iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from grizzly.types import RequestType, ScenarioState
 from grizzly.types.locust import StopUser
 from grizzly.exceptions import RestartScenario, StopScenario
 
 from . import GrizzlyScenario
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.users.base import GrizzlyUser
 
 
 class IteratorScenario(GrizzlyScenario):
     user: 'GrizzlyUser'
 
     start: Optional[float]
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/_helpers.py` & `grizzly-loadtester-2.6.4/grizzly/steps/_helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/background/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/steps/background/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/background/setup.py` & `grizzly-loadtester-2.6.4/grizzly/steps/background/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/background/shapes.py` & `grizzly-loadtester-2.6.4/grizzly/steps/background/shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/scenario/response.py` & `grizzly-loadtester-2.6.4/grizzly/steps/scenario/response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/scenario/results.py` & `grizzly-loadtester-2.6.4/grizzly/steps/scenario/results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/scenario/setup.py` & `grizzly-loadtester-2.6.4/grizzly/steps/scenario/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from grizzly.types.locust import StopUser
 from grizzly.types.behave import Context, given, then, register_type
 from grizzly.context import GrizzlyContext
 from grizzly.testdata.utils import create_context_variable, resolve_variable
 from grizzly.utils import merge_dicts
 from grizzly.exceptions import RestartScenario
 from grizzly.tasks import RequestTask, GrizzlyTask
+from grizzly.auth import GrizzlyHttpAuthClient
 from grizzly.steps._helpers import is_template
 
 
 @parse.with_pattern(r'(iteration[s]?)')
 @permutation(vector=(False, True,))
 def parse_iteration_gramatical_number(text: str) -> str:
     return text.strip()
@@ -207,36 +208,48 @@
 
 
 @then(u'metadata "{key}" is "{value}"')
 @given(u'metadata "{key}" is "{value}"')
 def step_setup_metadata(context: Context, key: str, value: str) -> None:
     '''Set a metadata (header) value to be used by the user when sending requests.
 
+    When step expression is used before any tasks has been added in the scenario the metadata will
+    be used for all requests the specified loadtesting user executes in the scenario.
+
+    If used after a {@pylink grizzly.tasks.request} task, the metadata will be added and only used
+    for that request.
+
+    If used after a task that implements `grizzly.auth.GrizzlyHttpAuthClient` (e.g. {@pylink grizzly.tasks.clients.http}),
+    the metadata will be added and only used when that task executes.
+
     Example:
 
     ``` gherkin
     And metadata "Content-Type" is "application/xml"
     And metadata "Ocp-Apim-Subscription-Key" is "9asdf00asdf00adsf034"
     ```
 
     Or, for use in one request only, specify metadata after the request:
     ``` gherkin
     Then post request ...
     And metadata "x-header" is "{{ value }}"
+
+    Then get "https://{{ client_url }}" with name "client-http" and save response payload in "payload"
+    And metadata "Ocp-Apim-Subscription-Key" is "deadbeefb00f"
     ```
     '''
 
     grizzly = cast(GrizzlyContext, context.grizzly)
     casted_value = resolve_variable(grizzly, value)
 
     previous_task: Optional[GrizzlyTask] = None
     tasks = grizzly.scenario.tasks()
     if len(tasks) > 0:
         previous_task = tasks[-1]
 
-    if isinstance(previous_task, RequestTask):
+    if isinstance(previous_task, (RequestTask, GrizzlyHttpAuthClient,)):
         previous_task.add_metadata(key, value)
     else:
         if grizzly.scenario.context.get('metadata', None) is None:
             grizzly.scenario.context['metadata'] = {}
 
         grizzly.scenario.context['metadata'].update({key: casted_value})
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/scenario/tasks.py` & `grizzly-loadtester-2.6.4/grizzly/steps/scenario/tasks.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/scenario/user.py` & `grizzly-loadtester-2.6.4/grizzly/steps/scenario/user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/steps/setup.py` & `grizzly-loadtester-2.6.4/grizzly/steps/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     def __init__(self, scenario: Optional['GrizzlyContextScenario'] = None) -> None:
         self._context_root = environ.get('GRIZZLY_CONTEXT_ROOT', '.')
         if scenario is not None:
             self.scenario = scenario
 
     @abstractmethod
     def __call__(self) -> grizzlytask:
-        raise NotImplementedError(f'{self.__class__.__name__} has not been implemented')
+        raise NotImplementedError(f'{self.__class__.__name__} has not been implemented')  # pragma: no cover
 
     def get_templates(self) -> List[str]:
         def is_template(value: str) -> bool:
             return '{{' in value and '}}' in value
 
         def _get_value_templates(value: Any) -> Set[str]:
             templates: Set[str] = set()
@@ -200,27 +200,33 @@
 
 class GrizzlyMetaRequestTask(GrizzlyTask, metaclass=ABCMeta):
     content_type: TransformerContentType
     name: Optional[str]
     endpoint: str
 
     def execute(self, parent: 'GrizzlyScenario') -> 'GrizzlyResponse':
-        raise NotImplementedError(f'{self.__class__.name} has not implemented "execute"')
+        raise NotImplementedError(f'{self.__class__.name} has not implemented "execute"')  # pragma: no cover
+
+    def on_start(self, parent: 'GrizzlyScenario') -> None:
+        pass
+
+    def on_stop(self, parent: 'GrizzlyScenario') -> None:
+        pass
 
 
 class GrizzlyTaskWrapper(GrizzlyTask, metaclass=ABCMeta):
     name: str
 
     @abstractmethod
     def add(self, task: GrizzlyTask) -> None:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented add')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented add')  # pragma: no cover
 
     @abstractmethod
     def peek(self) -> List[GrizzlyTask]:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented peek')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented peek')  # pragma: no cover
 
 
 class template:
     attributes: List[str]
 
     def __init__(self, attribute: str, *additional_attributes: str) -> None:
         self.attributes = [attribute]
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/async_group.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/async_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def peek(self) -> List[GrizzlyTask]:
         return self.tasks
 
     def __call__(self) -> grizzlytask:
         @grizzlytask
         def task(parent: 'GrizzlyScenario') -> Any:
             if not isinstance(parent.user, AsyncRequests):
-                raise NotImplementedError(f'{parent.user.__class__.__name__} does not inherit AsyncRequests')
+                raise NotImplementedError(f'{parent.user.__class__.__name__} does not inherit AsyncRequests')  # pragma: no cover
 
             exception: Optional[Exception] = None
             response_length = 0
 
             def trace_green(event: str, args: Tuple[gevent.Greenlet, gevent.Greenlet]) -> None:  # pragma: no cover
                 src, target = args
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/clients/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/clients/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     _scheme: str
     _short_name: str
     _direction_arrow: Dict[RequestDirection, str] = {
         RequestDirection.FROM: '<-',
         RequestDirection.TO: '->',
     }
 
+    host: str
     grizzly: GrizzlyContext
     direction: RequestDirection
     endpoint: str
     name: Optional[str]
     payload_variable: Optional[str]
     metadata_variable: Optional[str]
     source: Optional[str]
@@ -116,14 +117,15 @@
         self.direction = direction
         self.endpoint = endpoint
         self.name = name
         self.payload_variable = payload_variable
         self.metadata_variable = metadata_variable
         self.source = source
         self.destination = destination
+        self.host = endpoint
 
         if self.payload_variable is not None and self.direction != RequestDirection.FROM:
             raise AttributeError(f'{self.__class__.__name__}: variable argument is not applicable for direction {self.direction.name}')
 
         if self.source is not None and self.direction != RequestDirection.TO:
             raise AttributeError(f'{self.__class__.__name__}: source argument is not applicable for direction {self.direction.name}')
 
@@ -153,15 +155,15 @@
         pass
 
     # SOW: see https://github.com/python/mypy/issues/5936#issuecomment-1429175144
     def text_fget(self) -> Optional[str]:
         return self._text
 
     def text_fset(self, value: str) -> None:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented support for step text')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented support for step text')  # pragma: no cover
 
     text = property(text_fget, text_fset)
     # EOW
 
     @property
     def variable_template(self) -> Optional[str]:
         if self.payload_variable is None or ('{{' in self.payload_variable and '}}' in self.payload_variable):
@@ -194,31 +196,32 @@
         return task
 
     def execute(self, parent: GrizzlyScenario) -> GrizzlyResponse:
         return self.get(parent)
 
     @abstractmethod
     def get(self, parent: GrizzlyScenario) -> GrizzlyResponse:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented GET')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented GET')  # pragma: no cover
 
     @abstractmethod
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented PUT')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented PUT')  # pragma: no cover
 
     @contextmanager
     def action(self, parent: GrizzlyScenario, action: Optional[str] = None, suppress: bool = False) -> Generator[Dict[str, Any], None, None]:
         exception: Optional[Exception] = None
         response_length = 0
         start_time = time()
         meta: Dict[str, Any] = {}
 
         try:
             # get metadata back from actual implementation
             yield meta
         except Exception as e:
+            parent.logger.error(str(e), exc_info=True)
             exception = e
         finally:
             if self.name is None:
                 action = action or meta.get('action', self.payload_variable)
                 name = f'{parent.user._scenario.identifier} {self._short_name}{meta.get("direction", self._direction_arrow[self.direction])}{action}'
             else:
                 rendered_name = parent.render(self.name)
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/clients/blobstorage.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/clients/blobstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         self.service_client = BlobServiceClient.from_connection_string(conn_str=self.connection_string)
 
     @property
     def connection_string(self) -> str:
         return f'DefaultEndpointsProtocol={self._endpoints_protocol};AccountName={self.account_name};AccountKey={self.account_key};EndpointSuffix=core.windows.net'
 
     def get(self, parent: GrizzlyScenario) -> GrizzlyResponse:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented GET')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented GET')  # pragma: no cover
 
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
         source = parent.render(cast(str, self.source))
 
         if self.destination is not None:
             destination = parent.render(self.destination)
         else:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/clients/messagequeue.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/clients/messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/clients/servicebus.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/clients/servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/conditional.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/conditional.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/date.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,15 @@
                 offset_rendered = parent.render(offset)
                 offset_params = cast(Any, parse_timespan(offset_rendered))
                 date_value += relativedelta(**offset_params)
 
             timezone_argument = self.arguments.get('timezone', None)
             timezone: Optional[ZoneInfo] = None  # None in asttimezone == local time zone
             if timezone_argument is not None:
+                timezone_argument = parent.render(timezone_argument)
                 try:
                     timezone = ZoneInfo(timezone_argument)
                 except ZoneInfoNotFoundError as e:
                     raise ValueError(f'"{timezone_argument}" is not a valid time zone') from e
 
             date_format = cast(str, self.arguments.get('format', '%Y-%m-%d %H:%M:%S'))
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/log_message.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/loop.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/loop.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/request.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/set_variable.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/set_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import TYPE_CHECKING, Any, Optional, MutableMapping, Type, cast
 
 from grizzly.testdata import GrizzlyVariables
 from grizzly.testdata.variables import AtomicVariable
 
 from . import GrizzlyTask, template, grizzlytask
 
-if TYPE_CHECKING:  # pragma: no coverage
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContextScenario
     from grizzly.scenarios import GrizzlyScenario
 
 
 @template('variable_template', 'value')
 class SetVariableTask(GrizzlyTask):
     variable: str
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/task_wait.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/timer.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/transformer.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/until.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/until.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 from jinja2 import Template
 from gevent import sleep as gsleep
 from grizzly_extras.transformer import Transformer, TransformerContentType, TransformerError, transformer
 from grizzly_extras.arguments import get_unsupported_arguments, parse_arguments, split_value
 
 from grizzly.types import RequestType
+from grizzly.utils import safe_del
 
 from . import GrizzlyTask, GrizzlyMetaRequestTask, template, grizzlytask
 
 if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContextScenario, GrizzlyContext
     from grizzly.scenarios import GrizzlyScenario
 
@@ -132,14 +133,16 @@
             retry = 0
             exception: Optional[Exception] = None
             response_length = 0
 
             start = perf_counter()
 
             try:
+                error_count_before = len(parent.user.environment.stats.errors.keys())
+
                 while retry < self.retries:
                     number_of_matches = 0
 
                     try:
                         gsleep(self.wait)
 
                         _, payload = self.request.execute(parent)
@@ -159,14 +162,25 @@
                             exception = e
                         number_of_matches = 0
                     finally:
                         if number_of_matches == self.expected_matches:
                             break
                         else:
                             retry += 1
+
+                # remove any errors produced during until loop
+                error_count_after = len(parent.user.environment.stats.errors.keys())
+                if error_count_after > error_count_before:
+                    error_keys: List[str] = []
+                    for error_key, error in parent.user.environment.stats.errors.items():
+                        if error.name == f'{parent.user._scenario.identifier} {self.request.name}':
+                            error_keys.append(error_key)
+
+                    for error_key in error_keys:
+                        safe_del(parent.user.environment.stats.errors, error_key)
             except Exception as e:
                 parent.logger.error(f'{task_name}: error retry={retry}', exc_info=True)
                 if exception is None:
                     exception = e
             finally:
                 response_time = int((perf_counter() - start) * 1000)
 
@@ -192,8 +206,16 @@
                     context=parent.user._context,
                     exception=exception,
                 )
 
                 if exception is not None and self.scenario.failure_exception is not None:
                     raise self.scenario.failure_exception()
 
+        @task.on_start
+        def on_start(parent: 'GrizzlyScenario') -> None:
+            self.request.on_start(parent)
+
+        @task.on_stop
+        def on_stop(parent: 'GrizzlyScenario') -> None:
+            self.request.on_stop(parent)
+
         return task
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/tasks/wait.py` & `grizzly-loadtester-2.6.4/grizzly/tasks/wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Type, Any, Optional, Callable, List, Tuple, Set, Dict, cast
 from importlib import import_module
 
 from grizzly.types import GrizzlyVariableType
 from grizzly.types.locust import MessageHandler
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContext
     from .variables import AtomicVariable
 
 
 __all__ = [
     'GrizzlyVariableType',
 ]
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/ast.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from jinja2 import Environment as Jinja2Environment, FileSystemLoader as Jinja2FileSystemLoader
 from jinja2 import nodes as j2
 
 from grizzly.tasks import GrizzlyTask
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContextScenario
 
 logger = logging.getLogger(__name__)
 
 
 def get_template_variables(tasks: List[GrizzlyTask]) -> Dict[str, Set[str]]:
     templates: Dict['GrizzlyContextScenario', Set[str]] = {}
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/communication.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/communication.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from grizzly.types.locust import Environment, StopUser
 
 from .utils import transform
 from .variables import AtomicVariablePersist
 from . import GrizzlyVariables
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContext
     from grizzly.scenarios import GrizzlyScenario
 
 
 class TestdataConsumer:
     # need so pytest doesn't raise PytestCollectionWarning
     __test__: bool = False
@@ -244,19 +244,19 @@
 
                                             if value is None and scenario_name not in self.scenarios_iteration:
                                                 message['action'] = 'stop'
                                                 self.logger.warning(f'{key} does not have a value and iterations is not set for {scenario_name}, stop test')
                                                 data = {}
                                                 break
                                             else:
+                                                data['variables'][key] = value
+
                                                 if key in self.grizzly.state.alias:
                                                     key = self.grizzly.state.alias[key]
                                                     data[key] = value
-                                                else:
-                                                    data['variables'][key] = value
 
                                         message['data'] = data
 
                                     if scenario_name in self.scenarios_iteration:
                                         self.scenarios_iteration[scenario_name] += 1
                                         self.logger.debug(f'{consumer_identifier}/{scenario_name}: iteration={self.scenarios_iteration[scenario_name]}')
                         except TypeError:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/utils.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 import logging
 import re
 
-from typing import TYPE_CHECKING, Optional, List, Dict, Any, Tuple, Set
+from typing import TYPE_CHECKING, Optional, List, Dict, Any, Tuple, Set, cast
 from collections import namedtuple
 from os import environ
 from time import perf_counter as time
 
 from jinja2 import Template, Environment
 from jinja2.meta import find_undeclared_variables
 
@@ -15,15 +15,15 @@
 from grizzly.testdata.ast import get_template_variables
 from grizzly.tasks import GrizzlyTask
 from grizzly.utils import merge_dicts
 
 from . import GrizzlyVariables
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContext, GrizzlyContextScenario
 
 
 logger = logging.getLogger(__name__)
 
 
 def initialize_testdata(grizzly: 'GrizzlyContext', tasks: List[GrizzlyTask]) -> Tuple[TestdataType, Set[str], Dict[str, MessageHandler]]:
@@ -153,18 +153,29 @@
 
 
 def create_context_variable(grizzly: 'GrizzlyContext', variable: str, value: str) -> Dict[str, Any]:
     if '{{' in value and '}}' in value:
         grizzly.scenario.orphan_templates.append(value)
 
     casted_value = resolve_variable(grizzly, value)
+    casted_variable = cast(str, resolve_variable(grizzly, variable))
 
-    variable = variable.lower().replace(' ', '_').replace('/', '.')
+    prefix: Optional[str] = None
 
-    return transform(grizzly, {variable: casted_value}, objectify=False)
+    if casted_variable.count('/') == 1 and casted_variable.count('.') > 0:
+        prefix, casted_variable = casted_variable.split('/', 1)
+
+    casted_variable = casted_variable.lower().replace(' ', '_').replace('/', '.')
+
+    transformed = transform(grizzly, {casted_variable: casted_value}, objectify=False)
+
+    if prefix is not None:
+        transformed = {prefix: transformed}
+
+    return transformed
 
 
 def resolve_variable(grizzly: 'GrizzlyContext', value: str, guess_datatype: Optional[bool] = True, only_grizzly: bool = False) -> GrizzlyVariableType:
     if len(value) < 1:
         return value
 
     quote_char: Optional[str] = None
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         return cls._semaphore if not outer else DummySemaphore()
 
     def __getitem__(self, variable: str) -> Optional[T]:
         with self.semaphore():
             return self._get_value(variable)
 
     def __setitem__(self, variable: str, value: Optional[T]) -> None:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented "__setitem__"')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented "__setitem__"')  # pragma: no cover
 
     def __delitem__(self, variable: str) -> None:
         try:
             del self._values[variable]
         except KeyError:
             pass
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_reader.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_writer.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/csv_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         variables = list(instance._settings.keys())
 
         for variable in variables:
             del instance._settings[variable]
             del instance._buffer[variable]
 
     def __getitem__(self, variable: str) -> Optional[str]:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented "__getitem__"')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented "__getitem__"')  # pragma: no cover
 
     def __setitem__(self, variable: str, value: Optional[str]) -> None:
         if value is None or isinstance(self.grizzly.state.locust, MasterRunner):
             return
 
         if variable.count('.') < 1:
             raise ValueError(f'{self.__class__.__name__}.{variable} is not a valid reference')
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/date.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/directory_contents.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/integer_incrementer.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_integer.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_string.py` & `grizzly-loadtester-2.6.4/grizzly/testdata/variables/random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/types/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,18 @@
 
     @property
     def direction(self) -> RequestDirection:
         return self.value
 
 
 class RequestType(Enum, AdvancedEnum, metaclass=MixedEnumMeta, init='alias _weight'):
-    SCENARIO = ('SCEN', 0,)
-    TESTDATA = ('TSTD', 1,)
-    PACE = ('PACE', 2,)
+    AUTH = ('AUTH', 0,)
+    SCENARIO = ('SCEN', 1,)
+    TESTDATA = ('TSTD', 2,)
+    PACE = ('PACE', 3,)
     UNTIL = ('UNTL', None,)
     VARIABLE = ('VAR', None,)
     ASYNC_GROUP = ('ASYNC', None,)
     CLIENT_TASK = ('CLTSK', None,)
     HELLO = ('HELO', None,)
     RECEIVE = ('RECV', None,)
     CONNECT = ('CONN', None,)
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/types/locust.py` & `grizzly-loadtester-2.6.4/grizzly/types/locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/users/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/base/__init__.py` & `grizzly-loadtester-2.6.4/grizzly/users/base/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.types import GrizzlyResponse
     from grizzly.tasks import RequestTask
 
 
 class FileRequests:
     pass
 
@@ -14,15 +14,15 @@
 class HttpRequests:
     pass
 
 
 class AsyncRequests:
     @abstractmethod
     def async_request(self, request: 'RequestTask') -> 'GrizzlyResponse':
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented async_request')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented async_request')  # pragma: no cover
 
 
 from .response_event import ResponseEvent
 from .request_logger import RequestLogger
 from .response_handler import ResponseHandler
 from .grizzly_user import GrizzlyUser
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/base/grizzly_user.py` & `grizzly-loadtester-2.6.4/grizzly/users/base/grizzly_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 from grizzly.types.locust import Environment, StopUser
 from grizzly.tasks import RequestTask
 from grizzly.utils import merge_dicts
 
 from . import FileRequests
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContextScenario
 
 
 class GrizzlyUser(User):
+    __dependencies__: Set[str] = set()
+
     _context_root: str
     _context: Dict[str, Any] = {
         'variables': {},
     }
     _scenario: 'GrizzlyContextScenario'
 
     _scenario_state: Optional[ScenarioState]
 
-    __dependencies__: Set[str] = set()
-
     logger: Logger
 
     weight: int = 1
     host: str
 
     def __init__(self, environment: Environment, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
         super().__init__(environment, *args, **kwargs)
@@ -66,15 +66,15 @@
             self._state = LOCUST_STATE_RUNNING
             return False
         else:
             return cast(bool, super().stop(force=force))
 
     @abstractmethod
     def request(self, request: RequestTask) -> GrizzlyResponse:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented request')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented request')  # pragma: no cover
 
     def render(self, request: RequestTask) -> Tuple[str, str, Optional[str], Optional[Dict[str, str]], Optional[Dict[str, str]]]:
         scenario_name = f'{request.scenario.identifier} {request.name}'
 
         try:
             payload: Optional[str] = None
             name = Template(request.name).render(**self.context_variables)
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/base/request_logger.py` & `grizzly-loadtester-2.6.4/grizzly/users/base/request_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 'metadata': response_headers,
                 'payload': response_body,
                 'status': response.status_code,
             },
         }
 
     def request(self, request: RequestTask) -> GrizzlyResponse:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented request')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented request')  # pragma: no cover
 
     def request_logger(
         self,
         name: str,
         context: HandlerContextType,
         request: RequestTask,
         user: GrizzlyUser,
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/base/response_event.py` & `grizzly-loadtester-2.6.4/grizzly/users/base/response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/base/response_handler.py` & `grizzly-loadtester-2.6.4/grizzly/users/base/response_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @abstractmethod
     def __call__(
         self,
         input_context: Tuple[TransformerContentType, Any],
         user: GrizzlyUser,
         response: Optional[GrizzlyResponseContextManager] = None,
     ) -> None:
-        raise NotImplementedError(f'{self.__class__.__name__} has not implemented __call__')
+        raise NotImplementedError(f'{self.__class__.__name__} has not implemented __call__')  # pragma: no cover
 
     def get_match(
         self,
         input_context: Tuple[TransformerContentType, Any],
         user: GrizzlyUser,
         condition: bool = False
     ) -> Tuple[Optional[str], str, str]:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/blobstorage.py` & `grizzly-loadtester-2.6.4/grizzly/users/blobstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         response_length = 0
 
         try:
             with self.client.get_blob_client(container=endpoint, blob=os.path.basename(request_name)) as blob_client:
                 if request.method in [RequestMethod.SEND, RequestMethod.PUT]:
                     blob_client.upload_blob(payload)
                     response_length = len(payload or '')
-                else:
+                else:  # pragma: no cover
                     raise NotImplementedError(f'{self.__class__.__name__} has not implemented {request.method.name}')
         except Exception as e:
             exception = e
         finally:
             total_time = int((time() - start_time) * 1000)
             self.environment.events.request.fire(
                 request_type=RequestType.from_method(request.method),
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/dummy.py` & `grizzly-loadtester-2.6.4/grizzly/users/dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/iothub.py` & `grizzly-loadtester-2.6.4/grizzly/users/iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/messagequeue.py` & `grizzly-loadtester-2.6.4/grizzly/users/messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/restapi.py` & `grizzly-loadtester-2.6.4/grizzly/auth/aad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,219 +1,82 @@
-# pylint: disable=line-too-long
-'''Communicates with HTTP and HTTPS, with built-in support for Azure authenticated endpoints.
-
-## Request methods
-
-Supports the following request methods:
-
-* get
-* put
-* post
-
-## Format
-
-Format of `host` is the following:
-
-``` plain
-http[s]://<hostname>
-```
-
-## Examples
-
-Example on how to use it in a scenario:
-
-``` gherkin
-Given a user of type "RestApi" load testing "https://api.example.com"
-Then post request "test/request.j2.json" to endpoint "/api/test"
-Then get request from endpoint "/api/test"
-```
-
-To change how often the token should be refreshed, default is 3000 seconds:
-``` gherkin
-And set context variable "auth.refresh_time" to "3500"
-```
-
-### Authentication
-
-#### Client secret
-
-``` gherkin
-Given a user of type "RestApi" load testing "https://api.example.com"
-And set context variable "auth.provider" to "<provider>"
-And set context variable "auth.client.id" to "<client id>"
-And set context variable "auth.client.secret" to "<client secret>"
-And set context variable "auth.client.resource" to "<resource url/guid>"
-```
-
-#### Username and password
-
-`auth.user.redirect_uri` needs to correspond to the endpoint that the client secret is registrered for.
-
-``` gherkin
-Given a user of type "RestApi" load testing "https://api.example.com"
-And set context variable "auth.provider" to "<provider>"
-And set context variable "auth.client.id" to "<client id>"
-And set context variable "auth.user.username" to "alice@example.onmicrosoft.com"
-And set context variable "auth.user.password" to "HemL1gaArn3!"
-And set context variable "auth.user.redirect_uri" to "/app-registrered-redirect-uri"
-```
-
-#### Multipart/form-data
-
-RestApi supports posting of multipart/form-data content-type, and in that case additional arguments needs to be passed with the request:
-
-* `multipart_form_data_name` _str_ - the name of the input form
-
-* `multipart_form_data_filename` _str_ - the filename
-
-Example:
-
-``` gherkin
-Then post request "path/my_template.j2.xml" with name "FormPost" to endpoint "example.url.com | content_type=multipart/form-data, multipart_form_data_filename=my_filename, multipart_form_data_name=form_name"
-```
-'''  # noqa: E501
-import json
 import re
+import json
+import logging
 
-from typing import Dict, Optional, Any, Tuple, List, Union, cast
-from time import time, perf_counter as time_perf_counter
-from functools import wraps
-from enum import Enum
+from typing import Dict, Any, Tuple, Optional, List, cast
 from urllib.parse import parse_qs, urlparse
 from uuid import uuid4
 from secrets import token_urlsafe
 from hashlib import sha256
 from base64 import urlsafe_b64encode
-
-from locust.contrib.fasthttp import FastHttpSession
+from time import perf_counter as time_perf_counter
+from html.parser import HTMLParser
 
 import requests
 
-from grizzly_extras.transformer import TransformerContentType
-
-from grizzly.types import GrizzlyResponse, RequestType, RequestMethod, WrappedFunc, GrizzlyResponseContextManager
-from grizzly.types.locust import Environment, StopUser
-from grizzly.utils import merge_dicts, safe_del
-from grizzly.tasks import RequestTask
-from grizzly.clients import ResponseEventSession
-
-from .base import RequestLogger, ResponseHandler, GrizzlyUser, HttpRequests, AsyncRequests
-from . import logger
-
-from urllib3 import disable_warnings as urllib3_disable_warnings
-urllib3_disable_warnings()
-
-
-class AuthMethod(Enum):
-    NONE = 1
-    CLIENT = 2
-    USER = 3
-
-
-class refresh_token:
-    def __call__(self, func: WrappedFunc) -> WrappedFunc:
-        @wraps(func)
-        def refresh_token(cls: 'RestApiUser', *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> Any:
-            auth_context = cls._context['auth']
-
-            use_auth_client = (
-                auth_context.get('client', {}).get('id', None) is not None
-                and auth_context.get('client', {}).get('secret', None) is not None
-                and auth_context.get('provider', None) is not None
-            )
-            use_auth_user = (
-                auth_context.get('client', {}).get('id', None) is not None
-                and auth_context.get('user', {}).get('username', None) is not None
-                and auth_context.get('user', {}).get('password', None) is not None
-                and auth_context.get('user', {}).get('redirect_uri', None) is not None
-                and auth_context.get('provider', None) is not None
-            )
-
-            if use_auth_client:
-                auth_method = AuthMethod.CLIENT
-            elif use_auth_user:
-                auth_method = AuthMethod.USER
-            else:
-                auth_method = AuthMethod.NONE
-
-            if auth_method is not AuthMethod.NONE and cls.session_started is not None:
-                session_now = time()
-                session_duration = session_now - cls.session_started
-
-                # refresh token if session has been alive for at least refresh_time
-                if session_duration >= auth_context.get('refresh_time', 3000) or cls.headers.get('Authorization', None) is None:
-                    cls.get_token(auth_method)
-            else:
-                safe_del(cls.headers, 'Authorization')
-
-            return func(cls, *args, **kwargs)
-
-        return cast(WrappedFunc, refresh_token)
-
-
-class RestApiUser(ResponseHandler, RequestLogger, GrizzlyUser, HttpRequests, AsyncRequests):
-    session_started: Optional[float]
-    headers: Dict[str, Optional[str]]
-    environment: Environment
-
-    _context: Dict[str, Any] = {
-        'verify_certificates': True,
-        'auth': {
-            'refresh_time': 3000,
-            'provider': None,
-            'client': {
-                'id': None,
-                'secret': None,
-                'resource': None,
-            },
-            'user': {
-                'username': None,
-                'password': None,
-                'redirect_uri': None,
-            },
-        },
-        'metadata': None,
-    }
-
-    def __init__(self, environment: Environment, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
-        super().__init__(environment, *args, **kwargs)
-
-        self.headers = {
-            'Authorization': None,
-            'Content-Type': 'application/json',
-            'x-grizzly-user': self.__class__.__name__,
+from grizzly.utils import safe_del
+from grizzly.types.locust import StopUser
+from . import RefreshToken, GrizzlyHttpAuthClient, AuthType
+
+
+logger = logging.getLogger(__name__)
+
+
+class FormPostParser(HTMLParser):
+    action: Optional[str]
+    id_token: Optional[str]
+    client_info: Optional[str]
+    state: Optional[str]
+    session_state: Optional[str]
+
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.action = None
+        self.id_token = None
+        self.client_info = None
+        self.state = None
+        self.session_state = None
+
+    @property
+    def payload(self) -> Dict[str, str]:
+        assert self.id_token is not None, 'could not find id_token in response'
+        assert self.client_info is not None, 'could not find client_info in response'
+        assert self.state is not None, 'could not find state in response'
+        assert self.session_state is not None, 'could not find session_state in response'
+
+        return {
+            'id_token': self.id_token,
+            'client_info': self.client_info,
+            'state': self.state,
+            'session_state': self.session_state,
         }
 
-        self.session_started = None
-        self._context = merge_dicts(
-            super().context(),
-            # this is needed since we create a new class with this class as sub class, context will be messed up otherwise
-            # in other words, don't use RestApiUser._context. This should only be used in classes which are direct created
-            # in grizzly
-            self.__class__._context,
-        )
-
-        headers = self._context.get('metadata', None)
-        if headers is not None:
-            self.headers.update(headers)
-
-    def on_start(self) -> None:
-        super().on_start()
-
-        self.session_started = time()
-
-    def get_token(self, auth_method: AuthMethod) -> None:
-        if auth_method == AuthMethod.CLIENT:
-            self.get_oauth_token()
-        elif auth_method == AuthMethod.USER:
-            self.get_oauth_authorization()
-        else:
-            pass
-
-    def get_oauth_authorization(self) -> None:
+    def handle_starttag(self, tag: str, attrs: List[Tuple[str, Optional[str]]]) -> None:
+        if tag == 'form':
+            for attr, value in attrs:
+                if attr == 'action':
+                    self.action = value
+        elif tag == 'input':
+            prop_name: Optional[str] = None
+            prop_value: Optional[str] = None
+
+            for attr, value in attrs:
+                if attr == 'name':
+                    prop_name = value
+                elif attr == 'value':
+                    prop_value = value
+
+            if prop_name is not None and prop_value is not None:
+                setattr(self, prop_name, prop_value)
+
+
+class AAD(RefreshToken):
+    @classmethod
+    def get_oauth_authorization(cls, client: GrizzlyHttpAuthClient) -> Tuple[AuthType, str]:
         def _parse_response_config(response: requests.Response) -> Dict[str, Any]:
             match = re.search(r'Config={(.*?)};', response.text, re.MULTILINE)
 
             if not match:
                 raise ValueError(f'no config found in response from {response.url}')
 
             return cast(Dict[str, Any], json.loads(f'{{{match.group(1)}}}'))
@@ -251,28 +114,44 @@
 
             return code_verifier.decode('ascii'), code_challenge
 
         headers_ua: Dict[str, str] = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:88.0) Gecko/20100101 Firefox/88.0'
         }
 
-        auth_user_context = self._context['auth']['user']
+        auth_context = client._context.get('auth', None)
+        assert auth_context is not None, 'context variable auth is not set'
+        auth_user_context = auth_context.get('user', None)
+        assert auth_user_context is not None, 'context variable auth.user is not set'
+
+        initialize_uri = auth_user_context.get('initialize_uri', None)
+        redirect_uri = auth_user_context.get('redirect_uri', None)
+
+        assert initialize_uri is None or redirect_uri is None, 'both auth.user.initialize_uri and auth.user.redirect_uri is set'
+
+        is_token_v2_0: Optional[bool] = None
+        if initialize_uri is None:
+            redirect_uri = cast(str, redirect_uri)
+            auth_client_context = auth_context.get('client', None)
+            assert auth_client_context is not None, 'context variable auth.client is not set'
+            provider_url = auth_context.get('provider', None)
+            assert provider_url is not None, 'context variable auth.provider is not set'
+            auth_provider_parsed = urlparse(provider_url)
+            is_token_v2_0 = 'v2.0' in provider_url
+
         start_time = time_perf_counter()
         total_response_length = 0
         exception: Optional[Exception] = None
-        provider_url = self._context['auth'].get('provider', None)
-        assert provider_url is not None, 'context variable auth.provider is not set'
-        auth_provider_parsed = urlparse(provider_url)
-        is_token_v2_0 = 'v2.0' in provider_url
+        verify = client._context.get('verify_certificates', True)
+        username_lowercase = cast(str, auth_user_context['username']).lower()
 
         try:
-
             total_response_length = 0
 
-            with requests.Session() as client:
+            with requests.Session() as session:
                 headers: Dict[str, str]
                 payload: Dict[str, Any]
                 data: Dict[str, Any]
                 state: Dict[str, str] = {
                     'hpgact': '',
                     'hpgid': '',
                     'sFT': '',
@@ -282,87 +161,103 @@
                     'correlationId': '',
                     'sessionId': '',
                     'x-ms-request-id': '',
                     'country': '',
                 }
 
                 # <!-- request 1
-                client_id = self._context['auth']['client']['id']
-                client_request_id = generate_uuid()
-                username_lowercase = auth_user_context['username'].lower()
-
-                redirect_uri_parsed = urlparse(auth_user_context['redirect_uri'])
-                redirect_uri = auth_user_context['redirect_uri']
-
-                if len(redirect_uri_parsed.netloc) == 0:
-                    redirect_uri = f"{self._context['host']}{redirect_uri}"
-
-                url = f'{provider_url}/authorize'
-
-                params: Dict[str, List[str]] = {
-                    'response_type': ['id_token'],
-                    'client_id': [client_id],
-                    'redirect_uri': [redirect_uri],
-                    'state': [generate_uuid()],
-                    'client-request-id': [client_request_id],
-                    'x-client-SKU': ['Js'],
-                    'x-client-Ver': ['1.0.18'],
-                    'nonce': [generate_uuid()],
-                }
+                if initialize_uri is None:
+                    # <!-- dummy stuff, done earlier
+                    assert auth_client_context is not None
+                    assert redirect_uri is not None
+                    # // -->
+                    client_id = cast(str, auth_client_context['id'])
+                    client_request_id = generate_uuid()
+
+                    redirect_uri_parsed = urlparse(redirect_uri)
+
+                    if len(redirect_uri_parsed.netloc) == 0:
+                        redirect_uri = f"{client.host}{redirect_uri}"
+
+                    url = f'{provider_url}/authorize'
+
+                    params: Dict[str, List[str]] = {
+                        'response_type': ['id_token'],
+                        'client_id': [client_id],
+                        'redirect_uri': [redirect_uri],
+                        'state': [generate_uuid()],
+                        'client-request-id': [client_request_id],
+                        'x-client-SKU': ['Js'],
+                        'x-client-Ver': ['1.0.18'],
+                        'nonce': [generate_uuid()],
+                    }
+
+                    code_verifier: Optional[str] = None
+                    code_challenge: Optional[str] = None
+
+                    if is_token_v2_0:
+                        params.update({
+                            'response_mode': ['fragment'],
+                        })
+
+                        code_verifier, code_challenge = generate_pkcs()
+                        params.update({
+                            'response_type': ['code'],
+                            'code_challenge_method': ['S256'],
+                            'code_challenge': [code_challenge],
+                            'scope': ['openid profile offline_access'],
+                        })
+
+                    headers = {
+                        'Host': auth_provider_parsed.netloc,
+                        **headers_ua,
+                    }
 
-                code_verifier: Optional[str] = None
-                code_challenge: Optional[str] = None
+                    response = session.get(url, headers=headers, params=params, allow_redirects=False)
+                else:
+                    initialize_uri_parsed = urlparse(initialize_uri)
+                    if len(initialize_uri_parsed.netloc) < 1:
+                        initialize_uri = f'{client.host}{initialize_uri}'
 
-                if is_token_v2_0:
-                    code_verifier, code_challenge = generate_pkcs()
-                    params.update({
-                        'response_type': ['code'],
-                        'response_mode': ['fragment'],
-                        'scope': ['openid profile offline_access'],
-                        'code_challenge_method': ['S256'],
-                        'code_challenge': [code_challenge],
-                    })
+                    initialize_uri_parsed = urlparse(initialize_uri)
 
-                headers = {
-                    'Host': str(auth_provider_parsed.netloc),
-                    **headers_ua,
-                }
+                    response = session.get(initialize_uri, verify=verify)
+
+                    is_token_v2_0 = 'v2.0' in response.url
 
-                response = client.get(url, headers=headers, params=params)
                 logger.debug(f'user auth request 1: {response.url} ({response.status_code})')
                 total_response_length += int(response.headers.get('content-length', '0'))
 
                 if response.status_code != 200:
                     raise RuntimeError(f'user auth request 1: {response.url} had unexpected status code {response.status_code}')
 
                 referer = response.url
 
-                config = _parse_response_config(response)
+                config = update_state(state, response)
 
                 exception_message = config.get('strServiceExceptionMessage', None)
 
                 if exception_message is not None and len(exception_message.strip()) > 0:
                     raise RuntimeError(exception_message)
-
-                config = update_state(state, response)
                 # // request 1 -->
 
                 # <!-- request 2
                 url_parsed = urlparse(config['urlGetCredentialType'])
                 params = parse_qs(url_parsed.query)
 
                 url = f'{url_parsed.scheme}://{url_parsed.netloc}{url_parsed.path}'
+                host = url_parsed.netloc
                 params['mkt'] = ['sv-SE']
 
                 headers = {
                     'Accept': 'application/json',
-                    'Host': str(auth_provider_parsed.netloc),
+                    'Host': host,
                     'ContentType': 'application/json; charset=UTF-8',
                     'canary': state['apiCanary'],
-                    'client-request-id': client_request_id,
+                    'client-request-id': state['correlationId'],
                     'hpgact': state['hpgact'],
                     'hpgid': state['hpgid'],
                     'hpgrequestid': state['sessionId'],
                     **headers_ua,
                 }
 
                 payload = {
@@ -379,15 +274,15 @@
                     'isRemoteConnectSupported': False,
                     'federationFlags': 0,
                     'isSignup': False,
                     'flowToken': state['sFT'],
                     'isAccessPassSupported': True,
                 }
 
-                response = client.post(url, headers=headers, params=params, json=payload)
+                response = session.post(url, headers=headers, params=params, json=payload, allow_redirects=False)
                 total_response_length += int(response.headers.get('content-length', '0'))
 
                 logger.debug(f'user auth request 2: {response.url} ({response.status_code})')
 
                 if response.status_code != 200:
                     raise RuntimeError(f'user auth request 2: {response.url} had unexpected status code {response.status_code}')
 
@@ -397,21 +292,25 @@
                     raise RuntimeError(f'error response from {url}: code={error["code"]}, message={error["message"]}')
 
                 state['apiCanary'] = data['apiCanary']
                 assert state['sFT'] == data['FlowToken'], 'flow token between user auth request 1 and 2 differed'
                 # // request 2 -->
 
                 # <!-- request 3
-                assert config['urlPost'].startswith('https://'), f"response from {response.url} contained unexpected value '{config['urlPost']}'"
-                url = config['urlPost']
+                if initialize_uri is None:
+                    assert config['urlPost'].startswith('https://'), f"response from {response.url} contained unexpected value '{config['urlPost']}'"
+                    url = config['urlPost']
+                else:
+                    assert not config['urlPost'].startswith('https://'), f"response from {response.url} contained unexpected value '{config['urlPost']}'"
+                    url = f'{url_parsed.scheme}://{host}{config["urlPost"]}'
 
                 headers = {
                     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                     'Content-Type': 'application/x-www-form-urlencoded',
-                    'Host': str(auth_provider_parsed.netloc),
+                    'Host': host,
                     'Referer': referer,
                     **headers_ua,
                 }
 
                 payload = {
                     'i13': '0',
                     'login': username_lowercase,
@@ -438,50 +337,46 @@
                     'i21': '0',  # wasLearnMoreShown
                     'CookieDisclosure': '0',
                     'IsFidoSupported': '1',
                     'isSignupPost': '0',
                     'i19': '16369',  # time on page
                 }
 
-                response = client.post(url, headers=headers, data=payload)
+                response = session.post(url, headers=headers, data=payload)
                 total_response_length += int(response.headers.get('content-length', '0'))
 
                 logger.debug(f'user auth request 3: {response.url} ({response.status_code})')
 
                 if response.status_code != 200:
                     raise RuntimeError(f'user auth request 3: {response.url} had unexpected status code {response.status_code}')
 
-                config = _parse_response_config(response)
+                config = update_state(state, response)
 
                 exception_message = config.get('strServiceExceptionMessage', None)
 
                 if exception_message is not None and len(exception_message.strip()) > 0:
                     raise RuntimeError(exception_message)
 
                 user_proofs = config.get('arrUserProofs', [])
 
                 if len(user_proofs) > 0:
                     user_proof = user_proofs[0]
                     error_message = f'{username_lowercase} requires MFA for login: {user_proof["authMethodId"]} = {user_proof["display"]}'
                     logger.error(error_message)
                     raise RuntimeError(error_message)
-
-                # update state
-                state['sessionId'] = config['sessionId']
-                state['sFT'] = config['sFT']
                 # // request 3 -->
 
                 #  <!-- request 4
                 assert not config['urlPost'].startswith('https://'), f"unexpected response from {response.url}, incorrect username and/or password?"
-                url = f'{str(auth_provider_parsed.scheme)}://{str(auth_provider_parsed.netloc)}{config["urlPost"]}'
+                url = f'https://{host}{config["urlPost"]}'
 
                 headers = {
                     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                     'Content-Type': 'application/x-www-form-urlencoded',
-                    'Host': str(auth_provider_parsed.netloc),
+                    'Host': host,
                     'Referer': referer,
                     **headers_ua,
                 }
 
                 payload = {
                     'LoginOptions': '3',
                     'type': '28',
@@ -496,298 +391,236 @@
                 if not is_token_v2_0:
                     payload.update({
                         'i2': '',
                         'i17': '',
                         'i18': '',
                     })
 
-                response = client.post(url, headers=headers, data=payload, allow_redirects=False)
+                response = session.post(url, headers=headers, data=payload, allow_redirects=False)
                 total_response_length += int(response.headers.get('content-length', '0'))
 
                 logger.debug(f'user auth request 4: {response.url} ({response.status_code})')
 
-                if response.status_code != 302:
-                    try:
-                        config = _parse_response_config(response)
-                        exception_message = config.get('strServiceExceptionMessage', None)
-
-                        if exception_message is not None and len(exception_message.strip()) > 0:
-                            raise RuntimeError(exception_message)
-                    except ValueError:
-                        pass
-
-                    raise RuntimeError(f'user auth request 4: {response.url} had unexpected status code {response.status_code}')
-
-                assert 'Location' in response.headers, f'Location header was not found in response from {response.url}'
-
-                token_url = response.headers['Location']
-                assert token_url.startswith(f'{redirect_uri}'), f'unexpected redirect URI, got {token_url} but expected {redirect_uri}'
-                # // request 4 -->
-
-                token_url_parsed = urlparse(token_url)
-                fragments = parse_qs(token_url_parsed.fragment)
-
-                # exchange received with with a token
-                if is_token_v2_0:
-                    assert code_verifier is not None, 'no code verifier has been generated!'
-                    assert 'code' in fragments, f'could not find code in {token_url}'
-                    code = fragments['code'][0]
-                    self.get_oauth_token((code, code_verifier,))
+                if initialize_uri is None:
+                    if response.status_code != 302:
+                        try:
+                            config = _parse_response_config(response)
+                            exception_message = config.get('strServiceExceptionMessage', None)
+
+                            if exception_message is not None and len(exception_message.strip()) > 0:
+                                raise RuntimeError(exception_message)
+                        except ValueError:
+                            pass
+
+                        raise RuntimeError(f'user auth request 4: {response.url} had unexpected status code {response.status_code}')
+
+                    assert 'Location' in response.headers, f'Location header was not found in response from {response.url}'
+
+                    token_url = response.headers['Location']
+                    assert token_url.startswith(f'{redirect_uri}'), f'unexpected redirect URI, got {token_url} but expected {redirect_uri}'
+                    # // request 4 -->
+
+                    token_url_parsed = urlparse(token_url)
+                    fragments = parse_qs(token_url_parsed.fragment)
+
+                    # exchange received with with a token
+                    if is_token_v2_0:
+                        assert code_verifier is not None, 'no code verifier has been generated!'
+                        assert 'code' in fragments, f'could not find code in {token_url}'
+                        code = fragments['code'][0]
+                        return cls.get_oauth_token(client, (code, code_verifier,))
+                    else:
+                        assert 'id_token' in fragments, f'could not find id_token in {token_url}'
+                        token = fragments['id_token'][0]
+                        return (AuthType.HEADER, token,)
                 else:
-                    assert 'id_token' in fragments, f'could not find id_token in {token_url}'
-                    token = fragments['id_token'][0]
-                    self.headers['Authorization'] = f'Bearer {token}'
-                    self.session_started = time()
+                    parser = FormPostParser()
+                    parser.feed(response.text)
+
+                    if response.status_code != 200 or parser.action is None:
+                        try:
+                            config = _parse_response_config(response)
+                            exception_message = config.get('strServiceExceptionMessage', None)
+
+                            if exception_message is not None and len(exception_message.strip()) > 0:
+                                raise RuntimeError(exception_message)
+                        except ValueError:
+                            pass
+
+                        raise RuntimeError(f'user auth request 4: {response.url} had unexpected status code {response.status_code}')
+
+                    origin = f'https://{host}'
+
+                    headers.update({
+                        'Origin': origin,
+                        'Referer': origin,
+                    })
+
+                    safe_del(headers, 'Host')
+
+                    response = session.post(parser.action, headers=headers, data=parser.payload, allow_redirects=True, verify=verify)
+
+                    if response.status_code != 200:
+                        raise RuntimeError(f'user auth request 5: {response.url} had unexpected status code {response.status_code}')
+
+                    for cookie in session.cookies:
+                        domain = cookie.domain[1:] if cookie.domain_initial_dot else cookie.domain
+
+                        if domain in initialize_uri:
+                            return AuthType.COOKIE, f'{cookie.name}={cookie.value}'
+
+                    raise RuntimeError('did not find AAD cookie in authorization flow response session')
         except Exception as e:
             exception = e
-            self.logger.error(str(e), exc_info=True)
+            logger.error(str(e), exc_info=True)
         finally:
-            name = self.__class__.__name__.rsplit('_', 1)[-1]
+            name = client.__class__.__name__.rsplit('_', 1)[-1]
 
-            version = 'v1.0' if not is_token_v2_0 else 'v2.0'
+            if is_token_v2_0 is None:
+                version = ''
+            else:
+                version = 'v1.0' if not is_token_v2_0 else 'v2.0'
 
             request_meta = {
-                'request_type': 'GET',
+                'request_type': 'AUTH',
                 'response_time': int((time_perf_counter() - start_time) * 1000),
-                'name': f'{name} OAuth2 user token {version}',
-                'context': self._context,
+                'name': f'{name} {cls.__name__} OAuth2 user token {version}',
+                'context': client._context,
                 'response': None,
                 'exception': exception,
                 'response_length': total_response_length,
             }
 
-            self.environment.events.request.fire(**request_meta)
+            client.environment.events.request.fire(**request_meta)
 
             if exception is not None:
                 raise StopUser()
 
-    def get_oauth_token(self, pkcs: Optional[Tuple[str, str]] = None) -> None:
-        name = self.__class__.__name__.rsplit('_', 1)[-1]
-
-        provider_url = self._context['auth'].get('provider', None)
+    @classmethod
+    def get_oauth_token(cls, client: GrizzlyHttpAuthClient, pkcs: Optional[Tuple[str, str]] = None) -> Tuple[AuthType, str]:
+        auth_context = client._context.get('auth', None)
+        assert auth_context is not None, 'context variable auth is not set'
+        provider_url = auth_context.get('provider', None)
         assert provider_url is not None, 'context variable auth.provider is not set'
 
-        auth_client_context = self._context['auth']['client']
-        resource = auth_client_context.get('resource', self.host)
+        auth_client_context = auth_context.get('client', None)
+        assert auth_client_context is not None, 'context variable auth.client is not set'
+        resource = auth_client_context.get('resource', client.host)
+
+        auth_user_context = auth_context.get('user', None)
+
+        is_token_v2_0 = 'v2.0' in provider_url
 
         url = f'{provider_url}/token'
 
-        if pkcs is not None:
+        if is_token_v2_0:
             version = 'v2.0'
         else:
             version = 'v1.0'
 
         # parameters valid for both versions
         parameters: Dict[str, Any] = {
             'data': {
                 'grant_type': None,
                 'client_id': auth_client_context['id'],
             },
-            'verify': self._context.get('verify_certificates', True),
+            'verify': True,
         }
 
         # build generic header values, but remove stuff that shouldn't be part
         # of authentication flow
-        headers = {**self.headers}
+        headers = {**client.headers}
         safe_del(headers, 'Authorization')
         safe_del(headers, 'Content-Type')
         safe_del(headers, 'Ocp-Apim-Subscription-Key')
 
-        if pkcs is None:  # token v1.0
-            parameters['data'].update({
-                'grant_type': 'client_credentials',
-                'client_secret': auth_client_context['secret'],
-                'resource': resource,
-            })
-        else:  # token v2.0
+        start_time = time_perf_counter()
+
+        if pkcs is not None:  # token v2.0, authorization_code
+            assert auth_user_context is not None, 'context variable auth.user is not set'
             code, code_verifier = pkcs
 
-            auth_user_context = self._context['auth']['user']
             redirect_uri = auth_user_context['redirect_uri']
+            assert redirect_uri is not None, 'context variable auth.user.redirect_uri is not set'
             redirect_uri_parsed = urlparse(redirect_uri)
 
             if len(redirect_uri_parsed.netloc) == 0:
-                redirect_uri = f"{self._context['host']}{redirect_uri}"
+                redirect_uri = f"{client.host}{redirect_uri}"
+                redirect_uri_parsed = urlparse(redirect_uri)
 
             origin = f'{redirect_uri_parsed.scheme}://{redirect_uri_parsed.netloc}'
 
             headers.update({
                 'Origin': origin,
                 'Referer': origin,
             })
 
             parameters['data'].update({
                 'grant_type': 'authorization_code',
                 'redirect_uri': redirect_uri,
                 'code': code,
                 'code_verifier': code_verifier,
             })
-            parameters.update({'allow_redirects': False})
-
-        parameters.update({'headers': headers})
-
-        with self.client.request(
-            'POST',
-            url,
-            name=f'{name} OAuth2 client token {version}',
-            request=None,
-            catch_response=True,
-            **parameters,
-        ) as response:
-            if response.status_code == 200:
-                payload = json.loads(response.text)
-
-                if pkcs is None:
-                    token = str(payload['access_token'])
-                else:
-                    token = str(payload['id_token'])
+        elif not is_token_v2_0:  # token v1.0
+            parameters['data'].update({
+                'grant_type': 'client_credentials',
+                'client_secret': auth_client_context['secret'],
+                'resource': resource,
+            })
+        elif is_token_v2_0:  # token v2.0
+            tenant = auth_context.get('tenant', None)
+            if tenant is None:
+                provider_url_parsed = urlparse(provider_url)
+                tenant, _ = provider_url_parsed.path[1:].split('/', 1)
 
-                self.headers['Authorization'] = f'Bearer {token}'
-                self.session_started = time()
+            parameters['data'].update({
+                'grant_type': 'client_credentials',
+                'client_secret': auth_client_context['secret'],
+                'scope': resource,
+                'tenant': tenant,
+            })
 
-                response.success()
-            else:
-                message = self.get_error_message(response)
-                message = f'{message} ({response.status_code})'
+        parameters.update({'headers': headers, 'allow_redirects': (pkcs is None)})
 
-                self.logger.error(message)
-                response.failure(message)
+        exception: Optional[Exception] = None
 
-                raise StopUser()
+        response_length: int = 0
 
-    def get_error_message(self, response: GrizzlyResponseContextManager) -> str:
-        if response.text is None:
-            return f'unknown response {type(response)}'
-
-        if len(response.text) < 1:
-            if response.status_code == 401:
-                message = 'unauthorized'
-            elif response.status_code == 403:
-                message = 'forbidden'
-            elif response.status_code == 404:
-                message = 'not found'
-            else:
-                message = 'unknown'
-        else:
-            try:
+        try:
+            with requests.Session() as session:
+                response = session.post(url, **parameters)
+                response_length = len(response.text.encode())
                 payload = json.loads(response.text)
 
-                # special handling for dynamics error messages
-                if 'Message' in payload:
-                    message = payload['Message'].split('\\n', 1)[0].replace('\n', ' ')
-                elif 'error_description' in payload:
-                    message = payload['error_description'].split('\r\n')[0]
-                else:
-                    message = response.text
-            except json.decoder.JSONDecodeError:
-                message = response.text
-
-        return message
-
-    def async_request(self, request: RequestTask) -> GrizzlyResponse:
-        client = FastHttpSession(
-            environment=self.environment,
-            base_url=self.host,
-            user=self,
-            insecure=not self._context.get('verify_certificates', True),
-            max_retries=1,
-            connection_timeout=60.0,
-            network_timeout=60.0,
-        )
-
-        return self._request(client, request)
-
-    def request(self, request: RequestTask) -> GrizzlyResponse:
-        return self._request(self.client, request)
-
-    @refresh_token()
-    def _request(self, client: Union[FastHttpSession, ResponseEventSession], request: RequestTask) -> GrizzlyResponse:
-        if request.method not in [RequestMethod.GET, RequestMethod.PUT, RequestMethod.POST]:
-            raise NotImplementedError(f'{request.method.name} is not implemented for {self.__class__.__name__}')
-
-        if request.response.content_type == TransformerContentType.UNDEFINED:
-            request.response.content_type = TransformerContentType.JSON
-        elif request.response.content_type == TransformerContentType.XML:
-            self.headers['Content-Type'] = 'application/xml'
-        elif request.response.content_type == TransformerContentType.MULTIPART_FORM_DATA:
-            if 'Content-Type' in self.headers:
-                del self.headers['Content-Type']
-
-        request_name, endpoint, payload, arguments, metadata = self.render(request)
-
-        if metadata is not None:
-            self.headers.update(metadata)
-
-        parameters: Dict[str, Any] = {'headers': self.headers}
-
-        url = f'{self.host}{endpoint}'
-
-        # only render endpoint once, so needs to be done here
-        if isinstance(client, ResponseEventSession):
-            parameters.update({
-                'request': request,
-                'verify': self._context.get('verify_certificates', True),
-            })
-
-        name = f'{request.scenario.identifier} {request_name}'
-
-        if payload is not None:
-            if request.response.content_type == TransformerContentType.JSON:
-                try:
-                    parameters['json'] = json.loads(payload)
-                except json.decoder.JSONDecodeError as exception:
-                    # so that locust treats it as a failure
-                    self.environment.events.request.fire(
-                        request_type=RequestType.from_method(request.method),
-                        name=name,
-                        response_time=0,
-                        response_length=0,
-                        context=self._context,
-                        exception=exception,
-                    )
-                    logger.error(f'{url}: failed to decode: {payload=}')
-
-                    # this is a fundemental error, so we'll always stop the user
-                    raise StopUser()
-            elif request.response.content_type == TransformerContentType.MULTIPART_FORM_DATA and arguments:
-                parameters['files'] = {arguments['multipart_form_data_name']: (arguments['multipart_form_data_filename'], payload)}
-            else:
-                parameters['data'] = bytes(payload, 'UTF-8')
+                if response.status_code != 200:
+                    raise RuntimeError(payload['error_description'])
 
-        with client.request(
-            method=request.method.name,
-            name=name,
-            url=url,
-            catch_response=True,
-            **parameters,
-        ) as response:
-            if not isinstance(client, ResponseEventSession):
-                # monkey patch in request body... not available otherwise
-                setattr(response, 'request_body', payload)
-
-                self.response_event.fire(
-                    name=name,
-                    request=request,
-                    context=response,
-                    user=self,
-                )
-
-            if response._manual_result is None:
-                if response.status_code in request.response.status_codes:
-                    response.success()
+                if pkcs is None:
+                    token = str(payload['access_token'])
                 else:
-                    message = self.get_error_message(response)
-                    response.failure(f'{response.status_code} not in {request.response.status_codes}: {message}')
-
-            if response._manual_result is not True and request.scenario.failure_exception is not None:
-                raise request.scenario.failure_exception()
+                    token = str(payload['id_token'])
 
-            headers = dict(response.headers.items()) if response.headers not in [None, {}] else None
+                return (AuthType.HEADER, token,)
+        except Exception as e:
+            exception = e
+            logger.error(str(e), exc_info=True)
+        finally:
+            if client.parent is not None:
+                scenario_index = client.parent.user._scenario.identifier
+            else:
+                scenario_index = client.__class__.__name__.rsplit('_', 1)[-1]
 
-            return headers, response.text
+            request_meta = {
+                'request_type': 'AUTH',
+                'response_time': int((time_perf_counter() - start_time) * 1000),
+                'name': f'{scenario_index} {cls.__name__} OAuth2 user token {version}',
+                'context': client._context,
+                'response': None,
+                'exception': exception,
+                'response_length': response_length,
+            }
 
-    def add_context(self, context: Dict[str, Any]) -> None:
-        # something change in auth context, we need to re-authenticate
-        if context.get('auth', {}).get('user', {}).get('username', None) is not None:
-            self.headers['Authorization'] = None
+            if pkcs is None:
+                client.environment.events.request.fire(**request_meta)
 
-        super().add_context(context)
+            if exception is not None:
+                raise StopUser()
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/servicebus.py` & `grizzly-loadtester-2.6.4/grizzly/users/servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly/users/sftp.py` & `grizzly-loadtester-2.6.4/grizzly/users/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     }
 
     _auth_context: Dict[str, Any]
 
     _context_root: str
     _payload_root: str
 
+    host: str
+    port: int
+
     sftp_client: SftpClientSession
     session: SFTPClient
 
     def __init__(self, environment: Environment, *args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> None:
         super().__init__(environment, *args, **kwargs)
 
         self._context = merge_dicts(super().context(), self.__class__._context)
@@ -89,28 +92,29 @@
         if self._context['auth']['key_file'] is not None:
             raise NotImplementedError(f'{self.__class__.__name__}: key authentication is not implemented')
 
         host = parsed.netloc
         if ':' in host:
             [host, _] = host.split(':', 1)
 
-        port = int(parsed.port) if parsed.port is not None else 22
+        self.host = host
+        self.port = int(parsed.port) if parsed.port is not None else 22
         username = self._context['auth']['username']
         password = self._context['auth']['password']
         key_file = self._context['auth']['key_file']
 
         if username is None:
             raise ValueError(f'{self.__class__.__name__}: "auth.username" context variable is not set')
 
         if password is None and key_file is None:
             raise ValueError(f'{self.__class__.__name__}: "auth.password" or "auth.key" context variable must be set')
-        self.sftp_client = SftpClientSession(host, port)
 
     def on_start(self) -> None:
         super().on_start()
+        self.sftp_client = SftpClientSession(self.host, self.port)
         self.session = self.sftp_client.session(**self._context['auth']).__enter__()
 
     def on_stop(self) -> None:
         self.session.__exit__(None, None, None)
         super().on_stop()
 
     def request(self, request: RequestTask) -> GrizzlyResponse:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly/utils.py` & `grizzly-loadtester-2.6.4/grizzly/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/arguments.py` & `grizzly-loadtester-2.6.4/grizzly_extras/arguments.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/async_message/__init__.py` & `grizzly-loadtester-2.6.4/grizzly_extras/async_message/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,19 +132,19 @@
 
         # silence uamqp loggers
         for uamqp_logger_name in ['uamqp', 'uamqp.c_uamqp']:
             logging.getLogger(uamqp_logger_name).setLevel(logging.ERROR)
 
     @abstractmethod
     def get_handler(self, action: str) -> Optional['AsyncMessageRequestHandler']:
-        raise NotImplementedError(f'{self.__class__.__name__}: get_handler is not implemented')
+        raise NotImplementedError(f'{self.__class__.__name__}: get_handler is not implemented')  # pragma: no cover
 
     @abstractmethod
     def close(self) -> None:
-        raise NotImplementedError(f'{self.__class__.__name__}: close is not implemented')
+        raise NotImplementedError(f'{self.__class__.__name__}: close is not implemented')  # pragma: no cover
 
     @final
     def handle(self, request: AsyncMessageRequest) -> AsyncMessageResponse:
         start_time = time()
 
         try:
             action = request.get('action', None)
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/async_message/daemon.py` & `grizzly-loadtester-2.6.4/grizzly_extras/async_message/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,55 +196,42 @@
 
         response: Optional[AsyncMessageResponse] = None
 
         try:
             if request['worker'] != identity:
                 raise RuntimeError(f'got {request["worker"]}, expected {identity}')
 
-            action = request.get('action', None)
-
             if integration is None:
-                if action not in ['DISCONNECT', 'DISC']:
-                    integration_url = request.get('context', {}).get('url', None)
-                    if integration_url is None:
-                        raise RuntimeError('no url found in request context')
-
-                    parsed = urlparse(integration_url)
-
-                    if parsed.scheme in ['mq', 'mqs']:
-                        from .mq import AsyncMessageQueueHandler
-                        integration = AsyncMessageQueueHandler(identity)
-                    elif parsed.scheme == 'sb':
-                        from .sb import AsyncServiceBusHandler
-                        integration = AsyncServiceBusHandler(identity)
-                    else:
-                        raise RuntimeError(f'integration for {str(parsed.scheme)}:// is not implemented')
+                integration_url = request.get('context', {}).get('url', None)
+                if integration_url is None:
+                    raise RuntimeError('no url found in request context')
+
+                parsed = urlparse(integration_url)
+
+                if parsed.scheme in ['mq', 'mqs']:
+                    from .mq import AsyncMessageQueueHandler
+                    integration = AsyncMessageQueueHandler(identity)
+                elif parsed.scheme == 'sb':
+                    from .sb import AsyncServiceBusHandler
+                    integration = AsyncServiceBusHandler(identity)
                 else:
-                    response = {
-                        'worker': identity,
-                        'response_time': 0,
-                        'success': True,
-                        'message': f'already handled {action}',
-                    }
+                    raise RuntimeError(f'integration for {str(parsed.scheme)}:// is not implemented')
         except Exception as e:
             response = {
                 'worker': identity,
                 'response_time': 0,
                 'success': False,
                 'message': str(e),
             }
 
         if response is None and integration is not None:
             logger.debug('send request to handler')
             response = integration.handle(request)
             logger.debug('got response from handler')
 
-            if action in ['DISCONNECT', 'DISC']:
-                integration = None
-
         response_proto = [
             request_proto[0],
             SPLITTER_FRAME,
             jsondumps(response, cls=JsonBytesEncoder).encode(),
         ]
 
         worker.send_multipart(response_proto)
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/__init__.py` & `grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/rfh2.py` & `grizzly-loadtester-2.6.4/grizzly_extras/async_message/mq/rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/async_message/sb.py` & `grizzly-loadtester-2.6.4/grizzly_extras/async_message/sb.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,29 +57,32 @@
 
         return self._client
 
     @client.setter
     def client(self, value: ServiceBusClient) -> None:
         self._client = value
 
-    def close(self) -> None:
-        for key, sender in self._sender_cache.items():
-            self.logger.debug(f'closing sender {key}')
-            sender.close()
-
-        self._sender_cache.clear()
-
-        for key, receiver in self._receiver_cache.items():
-            self.logger.debug(f'closing receiver {key}')
-            receiver.close()
+    def close(self, soft: bool = False) -> None:
+        self.logger.debug(f'close: {soft=}')
+        if not soft:
+            for key, sender in self._sender_cache.items():
+                self.logger.debug(f'closing sender {key}')
+                sender.close()
+
+            self._sender_cache.clear()
+
+            for key, receiver in self._receiver_cache.items():
+                self.logger.debug(f'closing receiver {key}')
+                receiver.close()
 
-        self._receiver_cache.clear()
+            self._receiver_cache.clear()
 
         if len(self._sender_cache) + len(self._receiver_cache) == 0:
-            if self.client is not None:
+            self.logger.debug('no senders or receivers left, close ServiceBus clients')
+            if self._client is not None:
                 self.logger.debug('closing client')
                 self.client.close()
 
             if self.mgmt_client is not None:
                 self.logger.debug('closing management client')
                 self.mgmt_client.close()
 
@@ -246,15 +249,15 @@
                     pass
 
             try:
                 del cache[cache_endpoint]
             except:  # pragma: no cover
                 pass
 
-        self.close()
+            self.close(soft=True)
 
         return {
             'message': 'thanks for all the fish',
         }
 
     @register(handlers, 'SUBSCRIBE')
     def subscribe(self, request: AsyncMessageRequest) -> AsyncMessageResponse:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/text.py` & `grizzly-loadtester-2.6.4/grizzly_extras/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,8 +134,8 @@
     @classmethod
     def get_vector(cls) -> Optional[Tuple[bool, bool]]:
         return getattr(cls, '__vector__', None)
 
     @classmethod
     @abstractmethod
     def from_string(cls, value: str) -> Enum:
-        raise NotImplementedError(f'{cls.__name__} has not implemented `from_string`')
+        raise NotImplementedError(f'{cls.__name__} has not implemented `from_string`')  # pragma: no cover
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_extras/transformer.py` & `grizzly-loadtester-2.6.4/grizzly_extras/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,23 @@
         else:
             raise ValueError(f'"{value}" is an unknown response content type')
 
 
 class Transformer(ABCMeta):
     @classmethod
     def transform(cls, raw: str) -> Any:
-        raise NotImplementedError(f'{cls.__name__} has not implemented transform')
+        raise NotImplementedError(f'{cls.__name__} has not implemented transform')  # pragma: no cover
 
     @classmethod
     def validate(cls, expression: str) -> bool:
-        raise NotImplementedError(f'{cls.__name__} has not implemented validate')
+        raise NotImplementedError(f'{cls.__name__} has not implemented validate')  # pragma: no cover
 
     @classmethod
     def parser(cls, expression: str) -> Callable[[Any], List[str]]:
-        raise NotImplementedError(f'{cls.__name__} has not implemented parse')
+        raise NotImplementedError(f'{cls.__name__} has not implemented parse')  # pragma: no cover
 
 
 class transformer:
     content_type: TransformerContentType
     available: Dict[TransformerContentType, Type[Transformer]] = {}
 
     def __init__(self, content_type: TransformerContentType) -> None:
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/PKG-INFO` & `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.3
+Version: 2.6.4
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/SOURCES.txt` & `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 grizzly/behave.py
 grizzly/clients.py
 grizzly/context.py
 grizzly/exceptions.py
 grizzly/locust.py
 grizzly/py.typed
 grizzly/utils.py
+grizzly/auth/__init__.py
+grizzly/auth/aad.py
 grizzly/listeners/__init__.py
 grizzly/listeners/appinsights.py
 grizzly/listeners/influxdb.py
 grizzly/scenarios/__init__.py
 grizzly/scenarios/iterator.py
 grizzly/steps/__init__.py
 grizzly/steps/_helpers.py
@@ -154,14 +156,15 @@
 script/docs-generate.bash
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
 tests/helpers.py
 tests/webserver.py
 tests/e2e/__init__.py
+tests/e2e/test_auth.py
 tests/e2e/test_example.py
 tests/e2e/test_failure.py
 tests/e2e/test_iteration_pace.py
 tests/e2e/test_persistence.py
 tests/e2e/test_until.py
 tests/e2e/test_variables.py
 tests/e2e/steps/__init__.py
@@ -180,14 +183,17 @@
 tests/unit/test_grizzly/__init__.py
 tests/unit/test_grizzly/test_behave.py
 tests/unit/test_grizzly/test_clients.py
 tests/unit/test_grizzly/test_context.py
 tests/unit/test_grizzly/test_locust.py
 tests/unit/test_grizzly/test_types.py
 tests/unit/test_grizzly/test_utils.py
+tests/unit/test_grizzly/auth/__init__.py
+tests/unit/test_grizzly/auth/test___init__.py
+tests/unit/test_grizzly/auth/test_aad.py
 tests/unit/test_grizzly/listeners/__init__.py
 tests/unit/test_grizzly/listeners/test___init__.py
 tests/unit/test_grizzly/listeners/test_appinsights.py
 tests/unit/test_grizzly/listeners/test_influxdb.py
 tests/unit/test_grizzly/scenarios/__init__.py
 tests/unit/test_grizzly/scenarios/test_iterator.py
 tests/unit/test_grizzly/steps/__init__.py
```

### Comparing `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/requires.txt` & `grizzly-loadtester-2.6.4/grizzly_loadtester.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/pyproject.toml` & `grizzly-loadtester-2.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -262,9 +262,10 @@
     "--cov=.",
     "--cov-report=",
     "--no-cov-on-fail"
 ]
 timeout = 10
 filterwarnings = [
     "ignore:setDaemon\\(\\) is deprecated.*:DeprecationWarning",
-    "ignore:.*pkg_resources.*:DeprecationWarning"
+    "ignore:.*pkg_resources.*:DeprecationWarning",
+    "error:.*:gevent.monkey.MonkeyPatchWarning"
 ]
```

### Comparing `grizzly-loadtester-2.6.3/script/docs-generate-changelog.py` & `grizzly-loadtester-2.6.4/script/docs-generate-changelog.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/script/docs-generate-licenses.py` & `grizzly-loadtester-2.6.4/script/docs-generate-licenses.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/script/docs-generate.bash` & `grizzly-loadtester-2.6.4/script/docs-generate.bash`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/conftest.py` & `grizzly-loadtester-2.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_setup.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,222 +1,286 @@
 from typing import cast, Dict, List
 from itertools import product
 
-import pytest
-
 from grizzly.types.behave import Context
 from grizzly.context import GrizzlyContext
 from grizzly.types import ResponseTarget
+from grizzly.types.behave import Feature
 
 from tests.fixtures import End2EndFixture
 
 
-@pytest.mark.parametrize('target', [target for target in ResponseTarget])
-def test_e2e_step_response_save_matches(e2e_fixture: End2EndFixture, target: ResponseTarget) -> None:
+def test_e2e_step_response_save_matches(e2e_fixture: End2EndFixture) -> None:
+    targets = [target for target in ResponseTarget]
+
     def validator(context: Context) -> None:
         from grizzly.tasks import RequestTask
         from grizzly.users.base.response_handler import SaveHandlerAction
 
         grizzly = cast(GrizzlyContext, context.grizzly)
-
-        data = list(context.table)[0].as_dict()
-        handler_type = data['target']
-
         grizzly.scenario.tasks().pop()  # latest task is a dummy task
 
-        assert len(grizzly.scenario.orphan_templates) == 1, 'unexpected number of orphan templates'
-        assert grizzly.scenario.orphan_templates[0] == '{{ expression }}', f'{grizzly.scenario.orphan_templates[0]} != {{ expression }}'
+        rows = list(context.table)
+        assert len(grizzly.scenario.orphan_templates) == len(rows)
 
-        request = grizzly.scenario.tasks()[-2]
-
-        assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+        for row in rows:
+            data = row.as_dict()
+            handler_type = data['target']
+            index = int(data['index'])
+            attr_name = data['attr_name']
+
+            request = grizzly.scenario.tasks()[index]
+
+            assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+
+            handlers = getattr(request.response.handlers, handler_type)
+
+            assert f'{{{{ expression_{index} }}}}' in grizzly.scenario.orphan_templates, f'{{{{ expression_{index} }}}} not in {grizzly.scenario.orphan_templates}'
+            assert grizzly.state.variables.get(f'expression_{index}', None) == f'$.`this`.{attr_name}', f'variable expression_{index} is not $.`this`.{attr_name}'
+            assert len(handlers) == 1, f'unexpected number of {target} handlers'
+            handler = handlers[0]
+            assert isinstance(handler, SaveHandlerAction), f'{handler.__class__.__name__} != SaveHandlerAction'
+            assert handler.variable == f'tmp_{index}', f'{handler.variable} != tmp_{index}'
+            assert handler.expression == f'{{{{ expression_{index} }}}}', f'{handler.expression} != {{{{ expression_{index} }}}}'
+            assert handler.match_with == 'foo.*$', f'{handler.match_with} != foo.*$'
+            assert handler.expected_matches == 1, f'{handler.expected_matches} != 1'
+
+    table: List[Dict[str, str]] = []
+    scenario: List[str] = []
+
+    index = 0
+    for target in targets:
+        if target == ResponseTarget.METADATA:
+            attr_name = 'Foobar'
+        else:
+            attr_name = 'foobar'
 
-        handlers = getattr(request.response.handlers, handler_type)
+        table.append({'target': target.name.lower(), 'index': str(index), 'attr_name': attr_name})
 
-        assert len(handlers) == 1, f'unexpected number of {target} handlers'
-        handler = handlers[0]
-        assert isinstance(handler, SaveHandlerAction), f'{handler.__class__.__name__} != SaveHandlerAction'
-        assert handler.variable == 'tmp', f'{handler.variable} != tmp'
-        assert handler.expression == '{{ expression }}', f'{handler.expression} != {{{{ expression }}}}'
-        assert handler.match_with == 'foo[bar]?', f'{handler.match_with} != foo[bar]?'
-        assert handler.expected_matches == 10, f'{handler.expected_matches} != 10'
-
-    table: List[Dict[str, str]] = [{
-        'target': target.name.lower(),
-    }]
+        scenario += [
+            f'Given value for variable "expression_{index}" is "$.`this`.{attr_name}"',
+            f'Given value for variable "tmp_{index}" is "none"',
+            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/echo?foobar=foo | content_type=json"',
+            'And metadata "foobar" is "foobar"',
+            f'Then save response {target.name.lower()} "{{{{ expression_{index} }}}} | expected_matches=1" that matches "foo.*$" in variable "tmp_{index}"',
+            f'Then log message "tmp_{index}={{{{ tmp_{index} }}}}"',
+        ]
+        index += 2
 
     e2e_fixture.add_validator(
         validator,
         table=table,
     )
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            'And value for variable "tmp" is "none"',
-            'And value for variable "expression" is "$.hello.world"',
-            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/test | content_type=json"',
-            f'Then save response {target.name.lower()} "{{{{ expression }}}} | expected_matches=10" that matches "foo[bar]?" in variable "tmp"',
-            'Then log message "tmp={{ tmp }}"',
-        ],
-        identifier=target.name,
+        scenario=scenario,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
 
-@pytest.mark.parametrize('target', [target for target in ResponseTarget])
-def test_e2e_step_response_save(e2e_fixture: End2EndFixture, target: ResponseTarget) -> None:
+def test_e2e_step_response_save(e2e_fixture: End2EndFixture) -> None:
+    targets = [target for target in ResponseTarget]
+
     def validator(context: Context) -> None:
         from grizzly.tasks import RequestTask
         from grizzly.users.base.response_handler import SaveHandlerAction
 
         grizzly = cast(GrizzlyContext, context.grizzly)
+        grizzly.scenario.tasks().pop()  # latest task is a dummy task
 
-        data = list(context.table)[0].as_dict()
-        handler_type = data['target']
+        rows = list(context.table)
 
-        grizzly.scenario.tasks().pop()  # latest task is a dummy task
+        for row in rows:
+            data = row.as_dict()
+            handler_type = data['target']
+            index = int(data['index'])
+            attr_name = data['attr_name']
 
-        assert len(grizzly.scenario.orphan_templates) == 0, 'unexpected number of orphan templates'
+            assert len(grizzly.scenario.orphan_templates) == 0, 'unexpected number of orphan templates'
 
-        request = grizzly.scenario.tasks()[-2]
+            request = grizzly.scenario.tasks()[index]
 
-        assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+            assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+
+            handlers = getattr(request.response.handlers, handler_type)
 
-        handlers = getattr(request.response.handlers, handler_type)
+            assert len(handlers) == 1, f'unexpected number of {target} handlers'
+            handler = handlers[0]
+            assert isinstance(handler, SaveHandlerAction), f'{handler.__class__.__name__} != SaveHandlerAction'
+            assert handler.variable == f'tmp_{index}', f'{handler.variable} != tmp_{index}'
+            assert handler.expression == f'$.`this`.{attr_name}', f'{handler.expression} != $.`this`.{attr_name}'
+            assert handler.match_with == '.*', f'{handler.match_with} != .*'
+            assert handler.expected_matches == 1, f'{handler.expected_matches} != 1'
 
-        assert len(handlers) == 1, f'unexpected number of {target} handlers'
-        handler = handlers[0]
-        assert isinstance(handler, SaveHandlerAction), f'{handler.__class__.__name__} != SaveHandlerAction'
-        assert handler.variable == 'foobar', f'{handler.variable} != foobar'
-        assert handler.expression == '$.hello.world', f'{handler.expression} != $.hello.world'
-        assert handler.match_with == '.*', f'{handler.match_with} != .*'
-        assert handler.expected_matches == 1, f'{handler.expected_matches} != 1'
-
-    table: List[Dict[str, str]] = [{
-        'target': target.name.lower(),
-    }]
+    table: List[Dict[str, str]] = []
+    scenario: List[str] = []
+
+    index = 0
+    for target in targets:
+        if target == ResponseTarget.METADATA:
+            attr_name = 'Foobar'
+        else:
+            attr_name = 'foobar'
+        table.append({'target': target.name.lower(), 'index': str(index), 'attr_name': attr_name})
+
+        scenario += [
+            f'Given value for variable "tmp_{index}" is "none"',
+            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/echo?foobar=foo | content_type=json"',
+            'And metadata "foobar" is "foobar"',
+            f'Then save response {target.name.lower()} "$.`this`.{attr_name} | expected_matches=1" in variable "tmp_{index}"',
+            f'Then log message "tmp_{index}={{{{ tmp_{index} }}}}"',
+        ]
+
+        index += 2
 
     e2e_fixture.add_validator(
         validator,
         table=table,
     )
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            'And value for variable "foobar" is "none"',
-            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/test | content_type=json"',
-            f'Then save response {target.name.lower()} "$.hello.world" in variable "foobar"',
-            'Then log message "foobar={{ foobar }}"',
-        ],
-        identifier=target.name,
+        scenario=scenario,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
 
-@pytest.mark.parametrize('target,condition', list(product(ResponseTarget, ['is', 'is not'])))
-def test_e2e_step_response_validate(e2e_fixture: End2EndFixture, target: ResponseTarget, condition: str) -> None:
+def test_e2e_step_response_validate(e2e_fixture: End2EndFixture) -> None:
+    parameterize = list(product(ResponseTarget, ['is', 'is not']))
+
+    def after_feature(context: Context, feature: Feature) -> None:
+        from grizzly.locust import on_master
+
+        if on_master(context):
+            return
+
+        grizzly = cast(GrizzlyContext, context.grizzly)
+        stats = grizzly.state.locust.environment.stats
+
+        expectations = [
+            ('GET', '001 metadata-handler', 2, 1,),
+            ('GET', '001 payload-handler', 2, 1,),
+        ]
+
+        for method, name, expected_num_requests, expected_num_failures in expectations:
+            stat = stats.get(name, method)
+            assert stat.num_failures == expected_num_failures, f'{stat.method}:{stat.name}.num_failures: {stat.num_failures} != {expected_num_failures}'
+            assert stat.num_requests == expected_num_requests, f'{stat.method}:{stat.name}.num_requests: {stat.num_requests} != {expected_num_requests}'
+
+    e2e_fixture.add_after_feature(after_feature)
+
     def validator(context: Context) -> None:
         from grizzly.tasks import RequestTask
         from grizzly.users.base.response_handler import ValidationHandlerAction
 
         grizzly = cast(GrizzlyContext, context.grizzly)
+        grizzly.scenario.tasks().pop()  # latest task is a dummy task
 
-        data = list(context.table)[0].as_dict()
-        handler_type = data['target']
-        textual_condition = data['condition']
+        rows = list(context.table)
 
-        grizzly.scenario.tasks().pop()  # latest task is a dummy task
+        for index, row in enumerate(rows):
+            data = row.as_dict()
+            handler_type = data['target']
+            textual_condition = data['condition']
 
-        assert len(grizzly.scenario.orphan_templates) == 0, 'unexpected number of orphan templates'
+            assert len(grizzly.scenario.orphan_templates) == 0, 'unexpected number of orphan templates'
 
-        assert grizzly.scenario.failure_exception is None
+            assert grizzly.scenario.failure_exception is None
 
-        request = grizzly.scenario.tasks()[-1]
+            request = grizzly.scenario.tasks()[index]
 
-        assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+            assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
 
-        handlers = getattr(request.response.handlers, handler_type)
+            handlers = getattr(request.response.handlers, handler_type)
 
-        assert len(handlers) == 1, f'unexpected number of {target} handlers'
-        handler = handlers[0]
-        assert isinstance(handler, ValidationHandlerAction), f'{handler.__class__.__name__} != ValidationHandlerAction'
-        if textual_condition == 'is not':
-            assert not handler.condition
-        else:
-            assert handler.condition
+            assert len(handlers) == 1, f'unexpected number of {target} handlers'
+            handler = handlers[0]
+            assert isinstance(handler, ValidationHandlerAction), f'{handler.__class__.__name__} != ValidationHandlerAction'
+            if textual_condition == 'is not':
+                assert not handler.condition
+            else:
+                assert handler.condition
+
+            assert handler.expression == '$.hello.world', f'{handler.expression} != $.hello.world'
+            assert handler.match_with == 'foo[bar]?', f'{handler.match_with} != foo[bar]?'
+            assert handler.expected_matches == 1, f'{handler.expected_matches} != 1'
 
-        assert handler.expression == '$.hello.world', f'{handler.expression} != $.hello.world'
-        assert handler.match_with == 'foo[bar]?', f'{handler.match_with} != foo[bar]?'
-        assert handler.expected_matches == 1, f'{handler.expected_matches} != 1'
-
-    table: List[Dict[str, str]] = [{
-        'target': target.name.lower(),
-        'condition': condition,
-    }]
+    table: List[Dict[str, str]] = []
+    scenario: List[str] = []
+
+    for target, condition in parameterize:
+        table.append({
+            'target': target.name.lower(),
+            'condition': condition,
+        })
+
+        scenario += [
+            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/echo | content_type=json"',
+            f'When response {target.name.lower()} "$.hello.world" {condition} "foo[bar]?" fail request',
+        ]
 
     e2e_fixture.add_validator(
         validator,
         table=table,
     )
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            f'Then get request with name "{target.name.lower()}-handler" from endpoint "/api/test | content_type=json"',
-            f'When response {target.name.lower()} "$.hello.world" {condition} "foo[bar]?" fail request',
-        ],
-        identifier=target.name,
+        scenario=scenario,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    assert rc == 1
+
 
+def test_e2e_step_allow_status_codes(e2e_fixture: End2EndFixture) -> None:
+    status_codes = ['200,301', '-200,500']
 
-@pytest.mark.parametrize('status_codes', [
-    '200,302',
-    '-200,404',
-])
-def test_e2e_step_allow_status_codes(e2e_fixture: End2EndFixture, status_codes: str) -> None:
     def validator(context: Context) -> None:
         from grizzly.tasks import RequestTask
 
         grizzly = cast(GrizzlyContext, context.grizzly)
+        grizzly.scenario.tasks().pop()  # latest task is a dummy task
 
-        data = list(context.table)[0].as_dict()
-        status_codes = [int(status_code.strip()) for status_code in data['status_codes'].split(',') if status_code.strip() != '-200']
+        rows = list(context.table)
 
-        grizzly.scenario.tasks().pop()  # latest task is a dummy task
+        for index, row in enumerate(rows):
+            data = row.as_dict()
+            status_codes = [int(status_code.strip()) for status_code in data['status_codes'].split(',') if status_code.strip() != '-200']
 
-        request = grizzly.scenario.tasks()[-1]
+            request = grizzly.scenario.tasks()[index]
+
+            assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+            assert request.response.status_codes == status_codes
 
-        assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
-        assert request.response.status_codes == status_codes
         assert len(grizzly.scenario.orphan_templates) == 0, 'unexpected number of orphan templates'
 
-    table: List[Dict[str, str]] = [{
-        'status_codes': status_codes,
-    }]
+    table: List[Dict[str, str]] = []
+    scenario: List[str] = []
+
+    for status_code in status_codes:
+        table.append({'status_codes': status_code})
+        _, s = status_code.split(',', 1)
+        scenario += [
+            f'Then get request with name "test-allow-status-codes" from endpoint "/api/statuscode/{s}"',
+            f'And allow response status codes "{status_code}"',
+        ]
 
     e2e_fixture.add_validator(
         validator,
         table=table,
     )
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            'Then get request with name "test-allow-status-codes" from endpoint "/api/test"',
-            f'And allow response status codes "{status_codes}"',
-        ],
-        identifier=status_codes,
+        scenario=scenario,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
     assert rc == 0
 
 
 def test_e2e_step_allow_status_codes_table(e2e_fixture: End2EndFixture) -> None:
@@ -239,58 +303,67 @@
 
     e2e_fixture.add_validator(
         validator,
     )
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
-            'Then get request with name "test-get-1" from endpoint "/api/test"',
-            'Then get request with name "test-get-2" from endpoint "/api/test"',
+            'Then get request with name "test-get-1" from endpoint "/api/statuscode/302"',
+            'Then get request with name "test-get-2" from endpoint "/api/statuscode/404"',
             '''And allow response status codes
       | status   |
       | 200, 302 |
       | -200,404 |
 ''',
         ],
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
     assert rc == 0
 
 
-@pytest.mark.parametrize('content_type', [
-    'json', 'application/json',
-    'xml', 'application/xml',
-    'plain', 'text/plain',
-])
-def test_e2e_step_response_content_type(e2e_fixture: End2EndFixture, content_type: str) -> None:
+def test_e2e_step_response_content_type(e2e_fixture: End2EndFixture) -> None:
+    content_types = [
+        'json', 'application/json',
+        'xml', 'application/xml',
+        'plain', 'text/plain',
+    ]
+
     def validator(context: Context) -> None:
         from grizzly.tasks import RequestTask
         from grizzly_extras.transformer import TransformerContentType
 
         grizzly = cast(GrizzlyContext, context.grizzly)
-        data = list(context.table)[0].as_dict()
+        grizzly.scenario.tasks.pop()
 
-        request = grizzly.scenario.tasks()[-2]
-        assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
-        assert request.name == 'test-get-1', f'{request.name} != test-get-1'
-        assert request.response.content_type == TransformerContentType.from_string(data['content_type'])
+        rows = list(context.table)
 
-    table: List[Dict[str, str]] = [{
-        'content_type': content_type,
-    }]
+        for index, row in enumerate(rows):
+            data = row.as_dict()
+
+            request = grizzly.scenario.tasks()[index]
+            assert isinstance(request, RequestTask), f'{request.__class__.__name__} != RequestTask'
+            assert request.name == f'test-get-{index}', f'{request.name} != test-get-{index}'
+            assert request.response.content_type == TransformerContentType.from_string(data['content_type'])
+
+    table: List[Dict[str, str]] = []
+    scenario: List[str] = []
+
+    for index, content_type in enumerate(content_types):
+        table.append({'content_type': content_type})
+
+        scenario += [
+            f'Then get request with name "test-get-{index}" from endpoint "/api/echo?foo=bar"',
+            f'And set response content type to "{content_type}"',
+        ]
 
     e2e_fixture.add_validator(
         validator,
         table=table,
     )
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            'Then get request with name "test-get-1" from endpoint "/api/test"',
-            f'And set response content type to "{content_type}"',
-        ],
-        identifier=content_type,
+        scenario=scenario,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
     assert rc == 0
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,83 @@
 import textwrap
 
-from typing import cast, List, Dict
+from typing import cast, List, Dict, Any
 
 import pytest
 
 from grizzly.types.behave import Context, Feature
 from grizzly.context import GrizzlyContext
 
 from tests.fixtures import End2EndFixture
 
 
-@pytest.mark.parametrize('name,value,expected', [
-    ('token.url', 'http://example.com/api/auth', '{"token": {"url": "http://example.com/api/auth"}}',),
-    ('token/client id', 'aaaa-bbbb-cccc-dddd', '{"token": {"client_id": "aaaa-bbbb-cccc-dddd"}}',),
-    ('log_all_requests', 'True', '{"log_all_requests": true}',),
-    ('run_id', '13', '{"run_id": 13}',),
-])
-def test_e2e_step_setup_set_context_variable(e2e_fixture: End2EndFixture, name: str, value: str, expected: str) -> None:
+def test_e2e_step_setup_set_context_variable(e2e_fixture: End2EndFixture) -> None:
+    testdata = [
+        ('token.url', 'http://example.com/api/auth', '{"token": {"url": "http://example.com/api/auth"}}',),
+        ('token/client id', 'aaaa-bbbb-cccc-dddd', '{"token": {"client_id": "aaaa-bbbb-cccc-dddd"}}',),
+        ('log_all_requests', 'True', '{"log_all_requests": true}',),
+        ('run_id', '13', '{"run_id": 13}',),
+        ('www.example.com/auth.user.username', 'bob', '{"www.example.com": {"auth": {"user": {"username": "bob"}}}}'),
+    ]
+
     def validate_context_variable(context: Context) -> None:
         from json import loads as jsonloads
+        from grizzly.utils import merge_dicts
+
         grizzly = cast(GrizzlyContext, context.grizzly)
-        data = list(context.table)[0].as_dict()
+        expected_total: Dict[str, Any] = {}
+        first_row = list(context.table)[0].as_dict()
+        expected_host = first_row['expected']
+
+        for row in list(context.table)[1:]:
+            data = row.as_dict()
+
+            expected = jsonloads(data['expected'])
+            expected['hello'] = {'world': 'foobar'}
+
+            if 'token' not in expected:
+                expected['token'] = {'client_secret': 'something'}
+            else:
+                expected['token'].update({'client_secret': 'something'})
 
-        expected = jsonloads(data['expected'])
-        e2e_fixture_host = data['e2e_fixture.host']
-        expected['hello'] = {'world': 'foobar'}
-
-        if 'token' not in expected:
-            expected['token'] = {'client_secret': 'something'}
-        else:
-            expected['token'].update({'client_secret': 'something'})
+            expected_total = merge_dicts(expected_total, expected)
 
         actual = grizzly.scenario.context.copy()
 
         try:
             del actual['host']
         except KeyError:
             pass
 
-        assert actual == expected, f'{str(actual)} != {str(expected)}'
-        assert grizzly.scenario.context.get('host', None) == f'http://{e2e_fixture_host}'  # added by fixture
+        assert actual == expected_total, f'{str(actual)} != {str(expected)}'
+        assert grizzly.scenario.context.get('host', None) == f'http://{expected_host}'  # added by fixture
 
-    table: List[Dict[str, str]] = [{
-        'expected': expected,
-        'e2e_fixture.host': e2e_fixture.host,
-    }]
+    table: List[Dict[str, str]] = [{'expected': e2e_fixture.host}]
+    scenario: List[str] = []
+
+    for name, value, expected in testdata:
+        table.append({'expected': expected})
+        scenario.append(f'And set context variable "{name}" to "{value}"')
 
     e2e_fixture.add_validator(validate_context_variable, table=table)
 
     feature_file = e2e_fixture.test_steps(
-        scenario=[
-            f'And set context variable "{name}" to "{value}"',
+        scenario=scenario + [
             'And set context variable "hello.world" to "foobar"',
             'And set context variable "token/client_secret" to "something"',
         ],
         identifier=name,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
 
+# no easy way to rewrite without parameterize without rewriting End2EndFixture...
 @pytest.mark.parametrize('iterations', [
     '10', '1', '{{ leveranser * 0.25 }}',
 ])
 def test_e2e_step_setup_iterations(e2e_fixture: End2EndFixture, iterations: str) -> None:
     def validate_iterations(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
         data = list(context.table)[0].as_dict()
@@ -99,23 +111,27 @@
     )
 
     rc, _ = e2e_fixture.execute(feature_file, testdata={'leveranser': '100'})
 
     assert rc == 0
 
 
+# no easy way to rewrite without parameterize without rewriting End2EndFixture...
 @pytest.mark.parametrize('pace', ['2000', '{{ pace }}'])
 def test_e2e_step_setup_pace(e2e_fixture: End2EndFixture, pace: str) -> None:
     def validate_iterations(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
         data = list(context.table)[0].as_dict()
         pace = data['pace']
 
         assert grizzly.scenario.pace == pace, f'{grizzly.scenario.pace} != {pace}'
 
+        if '{{' in pace:
+            assert grizzly.scenario.orphan_templates == [pace], f'{pace} not in {grizzly.scenario.orphan_templates}'
+
     table: List[Dict[str, str]] = [{
         'pace': pace,
     }]
 
     e2e_fixture.add_validator(validate_iterations, table=table)
 
     feature_file = e2e_fixture.test_steps(
@@ -125,15 +141,15 @@
         scenario=[
             f'And set iteration time to "{pace}" milliseconds',
             'Then log message "pace={{ pace }}"',
         ],
         identifier=pace,
     )
 
-    rc, _ = e2e_fixture.execute(feature_file, testdata={'pace': pace})
+    rc, _ = e2e_fixture.execute(feature_file, testdata={'pace': '2000'})
 
     assert rc == 0
 
 
 def test_e2e_step_variable_value(e2e_fixture: End2EndFixture) -> None:
     def validate_variable_value(context: Context) -> None:
         from os import environ
@@ -214,14 +230,15 @@
     assert rc == 0
     assert 'persistent=10' in result
 
 
 def test_e2e_step_set_variable_alias(e2e_fixture: End2EndFixture) -> None:
     def validate_variable_alias(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
+        grizzly.scenario.tasks.pop()
 
         alias = grizzly.state.alias
 
         assert len(alias) == 2, 'unexpected number of aliases'
         alias_username = alias.get('AtomicCsvReader.users.username', None)
         assert alias_username == 'auth.user.username', f'{alias_username} != auth.user.username'
         alias_password = alias.get('AtomicCsvReader.users.password', None)
@@ -239,21 +256,24 @@
             'Then log message "username={{ AtomicCsvReader.users.username }}"',
             'Then log message "password={{ AtomicCsvReader.users.password }}"',
         ],
     )
 
     (e2e_fixture.root / 'features' / 'requests' / 'users.csv').write_text(textwrap.dedent(
         '''username,password
-        grizzly,secret
-        '''
+grizzly,secret'''
     ))
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
+
+    result = ''.join(output)
 
     assert rc == 0
+    assert 'username=grizzly' in result
+    assert 'password=secret' in result
 
 
 def test_e2e_step_setup_log_all_requests(e2e_fixture: End2EndFixture) -> None:
     def validate_log_all_requests(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         assert grizzly.scenario.context.get('log_all_requests', False)
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from json import dumps as jsondumps
 from typing import cast, List, Dict
 from textwrap import dedent
 
-import pytest
-
 from grizzly.context import GrizzlyContext
 from grizzly.types.behave import Context, Feature
 
 from tests.fixtures import End2EndFixture
 
 
 def test_e2e_step_task_request_text_with_name_to_endpoint(e2e_fixture: End2EndFixture) -> None:
@@ -26,35 +24,35 @@
 
         assert len(tasks) == 5, f'{len(tasks)} != 5'
 
         request = tasks[0]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.POST, f'{request.method} != RequestMethod.POST'
         assert request.name == 'test-post', f'{request.name} != test-post'
-        assert request.endpoint == '/api/test', f'{request.endpoint} != /api/test'
+        assert request.endpoint == '/api/echo', f'{request.endpoint} != /api/echo'
         assert isinstance(request.template, Template), 'request.template is not a Template'
         assert request.source is not None, 'request.source is None'
         assert jsonloads(request.source) == {'test': 'post'}, f"{request.source} != {'test': 'post'}"
         assert request.response.content_type == TransformerContentType.UNDEFINED, f'{request.response.content_type} != TransformerContentType.UNDEFINED'
 
         request = tasks[1]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.PUT
         assert request.name == 'test-put'
-        assert request.endpoint == '/api/test'
+        assert request.endpoint == '/api/echo'
         assert isinstance(request.template, Template)
         assert request.source is not None
         assert jsonloads(request.source) == {'test': 'put'}
         assert request.response.content_type == TransformerContentType.JSON
 
         request = tasks[2]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.GET
         assert request.name == 'test-get'
-        assert request.endpoint == '/api/test'
+        assert request.endpoint == '/api/echo'
         assert request.template is None
         assert request.source is None
         assert request.response.content_type == TransformerContentType.UNDEFINED
 
         request = tasks[3]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.SEND
@@ -74,43 +72,49 @@
         assert request.source is None
         assert request.response.content_type == TransformerContentType.XML
 
     e2e_fixture.add_validator(validate_requests)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
-            dedent('''Then post request with name "test-post" to endpoint "/api/test"
+            dedent('''Then post request with name "test-post" to endpoint "/api/echo"
                 """
                 {
                     "test": "post"
                 }
                 """
             '''),
-            dedent('''Then put request with name "test-put" to endpoint "/api/test | content_type=json"
+            dedent('''Then put request with name "test-put" to endpoint "/api/echo | content_type=json"
                 """
                 {
                     "test": "put"
                 }
                 """
             '''),
-            'Then get request with name "test-get" from endpoint "/api/test"',
+            'Then get request with name "test-get" from endpoint "/api/echo"',
             dedent('''Then send request with name "test-send" to endpoint "queue:receive-queue"
                 """
                 {
                     "test": "send"
                 }
                 """
             '''),
             'Then receive request with name "test-receive" from endpoint "queue:receive-queue | content_type=xml"',
         ],
     )
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    result = ''.join(output)
+
+    assert rc == 1
+
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed' in result
+    assert 'NotImplementedError: RECEIVE is not implemented for RestApiUser_001' in result
+    assert 'NotImplementedError: SEND is not implemented for RestApiUser_001' in result
 
 
 def test_e2e_step_task_request_file_with_name_endpoint(e2e_fixture: End2EndFixture) -> None:
     def validate_requests(context: Context) -> None:
         from json import loads as jsonloads
         from grizzly.tasks import RequestTask
         from grizzly.types import RequestMethod
@@ -136,26 +140,26 @@
         assert request.response.content_type == TransformerContentType.XML, f'{request.response.content_type} != TransformerContentType.XML'
         assert len(request.get_templates()) == 0
 
         request = tasks[1]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.POST
         assert request.name == 'test-post'
-        assert request.endpoint == '/api/test'
+        assert request.endpoint == '/api/echo'
         assert isinstance(request.template, Template)
         assert request.source is not None
         assert jsonloads(request.source) == {'test': 'request-{{ post }}'}
         assert request.response.content_type == TransformerContentType.JSON
         assert len(request.get_templates()) == 1
 
         request = tasks[2]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.PUT
         assert request.name == 'test-put-{{ foo }}'
-        assert request.endpoint == '/api/{{ bar }}'
+        assert request.endpoint == '/api/echo?foo={{ bar }}'
         assert isinstance(request.template, Template)
         assert request.source is not None
         assert jsonloads(request.source) == {'test': 'request-put-{{ foobar }}'}
         assert request.response.content_type == TransformerContentType.UNDEFINED
         assert len(request.get_templates()) == 3
 
     e2e_fixture.add_validator(validate_requests)
@@ -170,22 +174,26 @@
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "foo" is "bar"',
             'And value for variable "bar" is "foo"',
             'And value for variable "post" is "get"',
             'And value for variable "foobar" is "barfoo"',
             'Then send request "test/request-send.j2.json" with name "test-send" to endpoint "queue:receive-queue | content_type=xml"',
-            'Then post request "test/request-post.j2.json" with name "test-post" to endpoint "/api/test | content_type=json"',
-            'Then put request "test/request-put.j2.json" with name "test-put-{{ foo }}" to endpoint "/api/{{ bar }}"',
+            'Then post request "test/request-post.j2.json" with name "test-post" to endpoint "/api/echo | content_type=json"',
+            'Then put request "test/request-put.j2.json" with name "test-put-{{ foo }}" to endpoint "/api/echo?foo={{ bar }}"',
         ],
     )
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    result = ''.join(output)
+
+    assert rc == 1
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed' in result
+    assert 'NotImplementedError: SEND is not implemented for RestApiUser_001' in result
 
 
 def test_e2e_step_task_request_file_with_name(e2e_fixture: End2EndFixture) -> None:
     def validate_requests(context: Context) -> None:
         from json import loads as jsonloads
         from grizzly.tasks import RequestTask
         from grizzly.types import RequestMethod
@@ -200,15 +208,15 @@
 
         assert len(tasks) == 2, f'{len(tasks)} != 2'
 
         for index, request in enumerate(tasks, start=1):
             assert isinstance(request, RequestTask)
             assert request.method == RequestMethod.POST
             assert request.name == f'test-post-{index}'
-            assert request.endpoint == '/api/test'
+            assert request.endpoint == '/api/echo'
             assert isinstance(request.template, Template)
             assert request.source is not None
             assert jsonloads(request.source) == {'test': f'request-{{{{ post_{index} }}}}-{index}'}
             assert request.response.content_type == TransformerContentType.JSON
             assert len(request.get_templates()) == 1
 
     e2e_fixture.add_validator(validate_requests)
@@ -219,15 +227,15 @@
     (request_files / 'request-post-1.j2.json').write_text(jsondumps({'test': 'request-{{ post_1 }}-1'}))
     (request_files / 'request-post-2.j2.json').write_text(jsondumps({'test': 'request-{{ post_2 }}-2'}))
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "post_1" is "hello world"',
             'And value for variable "post_2" is "foobar"',
-            'Then post request "test/request-post-1.j2.json" with name "test-post-1" to endpoint "/api/test | content_type=json"',
+            'Then post request "test/request-post-1.j2.json" with name "test-post-1" to endpoint "/api/echo | content_type=json"',
             'Then post request "test/request-post-2.j2.json" with name "test-post-2"',
         ],
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
@@ -249,50 +257,50 @@
 
         assert len(tasks) == 4, f'{len(tasks)} != 4'
 
         for index, request in enumerate(tasks[:2], start=1):
             assert isinstance(request, RequestTask)
             assert request.method == RequestMethod.POST
             assert request.name == f'test-post-{index}'
-            assert request.endpoint == '/api/test'
+            assert request.endpoint == '/api/echo'
             assert isinstance(request.template, Template)
             assert request.source is not None
             assert jsonloads(request.source) == {'value': f'test-post-{index}'}
             assert request.response.content_type == TransformerContentType.JSON
             assert len(request.get_templates()) == 0
 
         for index, request in enumerate(tasks[2:], start=1):
             assert isinstance(request, RequestTask)
             assert request.method == RequestMethod.GET
             assert request.name == f'test-get-{index}'
-            assert request.endpoint == '/api/test'
+            assert request.endpoint == '/api/echo'
             assert request.template is None
             assert request.source is None
             assert request.response.content_type == TransformerContentType.XML
             assert len(request.get_templates()) == 0
 
     e2e_fixture.add_validator(validate_requests)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
-            dedent('''Then post request with name "test-post-1" to endpoint "/api/test | content_type=json"
+            dedent('''Then post request with name "test-post-1" to endpoint "/api/echo | content_type=json"
                 """
                 {
                     "value": "test-post-1"
                 }
                 """
             '''),
             dedent('''Then post request with name "test-post-2"
                 """
                 {
                     "value": "test-post-2"
                 }
                 """
             '''),
-            'Then get request with name "test-get-1" from endpoint "/api/test | content_type=\"application/xml\""',
+            'Then get request with name "test-get-1" from endpoint "/api/echo | content_type=\"application/xml\""',
             'Then get request with name "test-get-2"',
         ],
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
@@ -383,39 +391,39 @@
 
         assert len(tasks) == 4
 
         task = tasks[0]
         assert isinstance(task, TransformerTask)
         assert task.content == '{{ document }}'
         assert task.variable == 'document_id'
-        assert task.expression == '$.documents.id'
+        assert task.expression == '$.document.id'
         assert task.content_type == TransformerContentType.JSON
         assert issubclass(task._transformer, JsonTransformer)
         assert task.get_templates() == ['{{ document }}']
         assert callable(task._parser)
 
         task = tasks[1]
         assert isinstance(task, TransformerTask)
         assert task.content == '{{ document }}'
         assert task.variable == 'document_title'
-        assert task.expression == '$.documents.title'
+        assert task.expression == '$.document.title'
         assert task.content_type == TransformerContentType.JSON
         assert issubclass(task._transformer, JsonTransformer)
         assert task.get_templates() == ['{{ document }}']
         assert callable(task._parser)
 
     e2e_fixture.add_validator(validate_transform)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "document_id" is "None"',
             'And value for variable "document_title" is "None"',
             'And value for variable "document" is "{\"document\": {\"id\": \"DOCUMENT_8843-1\", \"title\": \"TPM Report 2021\"}}"',
-            'Then parse "{{ document }}" as "json" and save value of "$.documents.id" in variable "document_id"',
-            'Then parse "{{ document }}" as "json" and save value of "$.documents.title" in variable "document_title"',
+            'Then parse "{{ document }}" as "json" and save value of "$.document.id" in variable "document_id"',
+            'Then parse "{{ document }}" as "json" and save value of "$.document.title" in variable "document_title"',
             'Then log message "document_id={{ document_id }}"',
             'Then log message "document_title={{ document_title }}"',
         ]
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
@@ -436,63 +444,88 @@
         tasks.pop()
 
         assert len(tasks) == 3
 
         task = tasks[0]
         assert isinstance(task, HttpClientTask)
         assert task.direction == RequestDirection.FROM
-        assert task.endpoint == f'https://{e2e_fixture_host}/example.json'
+        assert task.endpoint == f'http://{e2e_fixture_host}/api/echo?foo=bar'
         assert task.name == 'https-get'
         assert task.payload_variable == 'example_openapi', f'{task.payload_variable} != example_openapi'
         assert task.metadata_variable is None
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         actual_templates = task.get_templates()
         assert actual_templates == ['{{ example_openapi }}'], f"{actual_templates} != ['{{{{ example_openapi }}}}']"
 
         task = tasks[1]
         assert isinstance(task, HttpClientTask)
         assert task.direction == RequestDirection.FROM
-        assert task.endpoint == '{{ endpoint }}'
+        assert task.endpoint == '{{ endpoint }}/api/echo?bar=foo', f'{task.endpoint=}'
         assert task.name == 'http-get'
         assert task.payload_variable == 'endpoint_payload'
         assert task.metadata_variable == 'endpoint_metadata'
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         actual_templates = task.get_templates()
         assert (
-            sorted(actual_templates) == sorted(['{{ endpoint }}', '{{ endpoint_payload }} {{ endpoint_metadata }}'])
+            sorted(actual_templates) == sorted(['{{ endpoint }}/api/echo?bar=foo', '{{ endpoint_payload }} {{ endpoint_metadata }}'])
         ), f"{actual_templates} != ['{{{{ endpoint }}}}', '{{{{ endpoint_payload }}}} {{{{ endpoint_metadata}}}}']"
 
     table: List[Dict[str, str]] = [{
         'e2e_fixture.host': e2e_fixture.host,
     }]
 
     e2e_fixture.add_validator(validate_client_task, table=table)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
-            'And value for variable "example_openapi" is "None"',
-            'And value for variable "endpoint_payload" is "None"',
-            'And value for variable "endpoint_metadata" is "None"',
-            f'And value for variable "endpoint" is "{e2e_fixture.host}"',
-            f'Then get "https://{e2e_fixture.host}/example.json" with name "https-get" and save response payload in "example_openapi"',
-            'Then get "http://{{ endpoint }}" with name "http-get" and save response payload in "endpoint_payload" and metadata in "endpoint_metadata"',
+            'And value for variable "example_openapi" is "none"',
+            'And value for variable "endpoint_payload" is "none"',
+            'And value for variable "endpoint_metadata" is "none"',
+            f'And value for variable "endpoint" is "http://{e2e_fixture.host}"',
+            f'Then get "http://{e2e_fixture.host}/api/echo?foo=bar" with name "https-get" and save response payload in "example_openapi"',
+            'Then get "http://{{ endpoint }}/api/echo?bar=foo" with name "http-get" and save response payload in "endpoint_payload" and metadata in "endpoint_metadata"',
             'Then log message "example_openapi={{ example_openapi }}, endpoint_payload={{ endpoint_payload }}, endpoint_metadata={{ endpoint_metadata }}"',
         ]
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
 
 def test_e2e_step_task_client_get_endpoint_until(e2e_fixture: End2EndFixture) -> None:
+    def after_feature(context: Context, feature: Feature) -> None:
+        from grizzly.locust import on_master
+
+        if on_master(context):
+            return
+
+        grizzly = cast(GrizzlyContext, context.grizzly)
+        stats = grizzly.state.locust.environment.stats
+
+        expectations = [
+            ('CLTSK', '001 http-get', 2, 1,),
+            ('UNTL', '001 http-get, w=0.11s, r=3, em=1', 1, 0,),
+            ('CLTSK', '001 http-env-get', 1, 1,),
+            ('UNTL', '001 https-env-get, w=0.1s, r=1, em=1', 1, 1,),
+            ('CLTSK', '001 https-get', 2, 1,),
+            ('UNTL', '001 https-get, w=0.12s r=1, em=1', 1, 0,),
+        ]
+
+        for method, name, expected_num_requests, expected_num_failures in expectations:
+            stat = stats.get(name, method)
+            assert stat.num_failures == expected_num_failures, f'{stat.method}:{stat.name}.num_failures: {stat.num_failures} != {expected_num_failures}'
+            assert stat.num_requests == expected_num_requests, f'{stat.method}:{stat.name}.num_requests: {stat.num_requests} != {expected_num_requests}'
+
+    e2e_fixture.add_after_feature(after_feature)
+
     def validate_client_task_until(context: Context) -> None:
         from grizzly.types import RequestDirection
         from grizzly_extras.transformer import TransformerContentType
         from grizzly.tasks.clients import HttpClientTask
         from grizzly.tasks import UntilRequestTask
 
         grizzly = cast(GrizzlyContext, context.grizzly)
@@ -504,15 +537,15 @@
         tasks.pop()  # remove dummy task added by `test_steps`
 
         assert len(tasks) == 3
 
         parent_task = tasks[0]
         assert isinstance(parent_task, UntilRequestTask)
         assert parent_task.retries == 3
-        assert parent_task.wait == 1.0
+        assert parent_task.wait == 0.11, f'{parent_task.wait=}'
         assert parent_task.expected_matches == 1
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == f'http://{e2e_fixture_host}/api/until/id?nth=2&wrong=bar&right=foo&as_array=True', f'{task.name=}, {task.endpoint=}'
@@ -523,15 +556,15 @@
         assert task.destination is None
         assert task._short_name == 'Http'
         assert task.get_templates() == []
 
         parent_task = tasks[1]
         assert isinstance(parent_task, UntilRequestTask)
         assert parent_task.retries == 3
-        assert parent_task.wait == 2.0
+        assert parent_task.wait == 0.12
         assert parent_task.expected_matches == 1
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == '{{ endpoint }}/api/until/success?nth=2&wrong=false&right=true&as_array=True', f'{task.name=}, {task.endpoint=}'
@@ -541,16 +574,16 @@
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         assert task.get_templates() == ['{{ endpoint }}/api/until/success?nth=2&wrong=false&right=true&as_array=True'], f'{task.name=}, {task.get_templates()=}'
 
         parent_task = tasks[2]
         assert isinstance(parent_task, UntilRequestTask)
-        assert parent_task.retries == 4
-        assert parent_task.wait == 1.0
+        assert parent_task.retries == 1
+        assert parent_task.wait == 0.1
         assert parent_task.expected_matches == 1
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {'verify': False}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == f'http://{e2e_fixture_host}/api/until/hello?nth=2&wrong=foobar&right=world&as_array=True', f'{task.name=}, {task.endpoint=}'
@@ -569,41 +602,60 @@
     e2e_fixture.add_validator(validate_client_task_until, table=table)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             f'And value for variable "endpoint" is "http://{e2e_fixture.host}"',
             (
                 f'Then get "http://{e2e_fixture.host}/api/until/id?nth=2&wrong=bar&right=foo&as_array=True | '
-                'content_type=json" with name "https-get" until "$.`this`[?id="foo"]"'
+                'content_type=json" with name "https-get" until "$.`this`[?id="foo"] | wait=0.11"'
             ),
             (
                 'Then get "http://{{ endpoint }}/api/until/success?nth=2&wrong=false&right=true&as_array=True | '
-                'content_type=json" with name "http-get" until "$.`this`[?success="true"] | wait=2.0"'
+                'content_type=json" with name "http-get" until "$.`this`[?success="true"] | wait=0.12"'
             ),
             (
                 'Then get "https://$conf::test.host$/api/until/hello?nth=2&wrong=foobar&right=world&as_array=True | content_type=json, verify=False" with name "https-env-get" '
-                'until "$.`this`[?hello=\"world\"] | retries=4, expected_matches=1"'
+                'until "$.`this`[?hello=\"world\"] | retries=1, expected_matches=1, wait=0.1"'
             ),
         ]
     )
 
     env_conf: Dict[str, Dict[str, Dict[str, str]]] = {
         'configuration': {
             'test': {
                 'host': f'http://{e2e_fixture.host}',
             }
         }
     }
 
-    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
+    rc, output = e2e_fixture.execute(feature_file, env_conf=env_conf)
 
-    assert rc == 0
+    result = ''.join(output)
+
+    assert rc == 1
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed' in result
 
 
 def test_e2e_step_task_client_put_endpoint_file_destination(e2e_fixture: End2EndFixture) -> None:
+    def after_feature(context: Context, feature: Feature) -> None:
+        from grizzly.locust import on_master
+
+        if on_master(context):
+            return
+
+        grizzly = cast(GrizzlyContext, context.grizzly)
+        errors = grizzly.state.locust.environment.stats.errors
+
+        assert len(errors) == 2
+
+        for error in errors.values():
+            assert isinstance(error.error, FileNotFoundError)
+
+    e2e_fixture.add_after_feature(after_feature)
+
     def validate_client_task(context: Context) -> None:
         from grizzly.types import RequestDirection
         from grizzly.tasks.clients import BlobStorageClientTask
 
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         tasks = grizzly.scenario.tasks()
@@ -650,20 +702,39 @@
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'Then put "test-file.json" to "bs://my-unsecure-storage?AccountKey=aaaabbb=&Container=my-container" with name "bs-put" as "uploaded-test-file.json"',
             'Then put "test-files.json" to "bss://my-storage?AccountKey=aaaabbb=&Container=my-container" with name "bss-put" as "uploaded-test-files.json"',
         ]
     )
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    result = ''.join(output)
+
+    assert rc == 1
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed' in result
 
 
 def test_e2e_step_task_client_put_endpoint_file(e2e_fixture: End2EndFixture) -> None:
+    def after_feature(context: Context, feature: Feature) -> None:
+        from grizzly.locust import on_master
+
+        if on_master(context):
+            return
+
+        grizzly = cast(GrizzlyContext, context.grizzly)
+        errors = grizzly.state.locust.environment.stats.errors
+
+        assert len(errors) == 2
+
+        for error in errors.values():
+            assert isinstance(error.error, FileNotFoundError)
+
+    e2e_fixture.add_after_feature(after_feature)
+
     def validate_client_task(context: Context) -> None:
         from grizzly.types import RequestDirection
         from grizzly.tasks.clients import BlobStorageClientTask
 
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         tasks = grizzly.scenario.tasks()
@@ -710,17 +781,20 @@
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'Then put "test-file.json" to "bs://my-unsecure-storage?AccountKey=aaaabbb=&Container=my-container" with name "bs-put"',
             'Then put "test-files.json" to "bss://my-storage?AccountKey=aaaabbb=&Container=my-container" with name "bss-put"',
         ]
     )
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    result = ''.join(output)
+
+    assert rc == 1
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed' in result
 
 
 def test_e2e_step_task_date(e2e_fixture: End2EndFixture) -> None:
     def validate_date_task(context: Context) -> None:
         from grizzly.tasks import DateTask
 
         grizzly = cast(GrizzlyContext, context.grizzly)
@@ -810,53 +884,53 @@
         assert task.name == 'async-group-{{ index }}'
         assert len(task.tasks) == 2
 
         request = task.tasks[0]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.POST
         assert request.name == 'async-group-{{ index }}:test-post-1'
-        assert request.endpoint == '/api/test'
+        assert request.endpoint == '/api/echo'
         assert isinstance(request.template, Template)
         assert request.source is not None
         assert jsonloads(request.source) == {'value': 'i have good news!'}
         assert request.get_templates() == ['async-group-{{ index }}:test-post-1']
 
         request = task.tasks[1]
         assert isinstance(request, RequestTask)
         assert request.method == RequestMethod.GET
         assert request.name == 'async-group-{{ index }}:test-get-1'
-        assert request.endpoint == '/api/test'
+        assert request.endpoint == '/api/echo?foo=bar'
         assert request.template is None
         assert request.source is None
         assert request.get_templates() == ['async-group-{{ index }}:test-get-1']
 
         task = tasks[1]
         assert isinstance(task, RequestTask)
         assert task.method == RequestMethod.GET
         assert task.name == 'test-get-2'
-        assert task.endpoint == '/api/test'
+        assert task.endpoint == '/api/echo?bar=foo'
         assert task.source is None
         assert task.template is None
 
     e2e_fixture.add_validator(validate_async_group)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "index" is "13"',
             'Given an async request group with name "async-group-{{ index }}"',
-            dedent('''Then post request with name "test-post-1" to endpoint "/api/test"
+            dedent('''Then post request with name "test-post-1" to endpoint "/api/echo"
                 """
                 {
                     "value": "i have good news!"
                 }
                 """
             '''),
-            'Then get request with name "test-get-1" from endpoint "/api/test"',
+            'Then get request with name "test-get-1" from endpoint "/api/echo?foo=bar"',
             'And close async request group',
-            'Then get request with name "test-get-2" from endpoint "/api/test"',
+            'Then get request with name "test-get-2" from endpoint "/api/echo?bar=foo"',
         ]
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
@@ -945,58 +1019,66 @@
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
 
-@pytest.mark.parametrize('value', [1, 6], scope='function')
-def test_e2e_step_task_conditional(e2e_fixture: End2EndFixture, value: int) -> None:
+def test_e2e_step_task_conditional(e2e_fixture: End2EndFixture) -> None:
     def validate_task_conditional(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         grizzly.scenario.tasks().pop()  # remove dummy task
 
-        assert len(grizzly.scenario.tasks()) == 1
+        assert len(grizzly.scenario.tasks()) == 2
 
     def after_feature(context: Context, feature: Feature) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         stats = grizzly.state.locust.environment.stats
 
-        suffix = 'True' if int(grizzly.state.variables['value']) > 5 else 'False'
+        conditional = stats.get('001 conditional-1: False (1)', 'COND')
 
-        conditional = stats.get(f'001 conditional-1: {suffix} (1)', 'COND')
+        assert conditional.num_requests == 1, f'{conditional.num_requests} != 1'
+        assert conditional.total_content_length == 1, f'{conditional.total_content_length} != 1'
+
+        conditional = stats.get('001 conditional-2: True (1)', 'COND')
 
         assert conditional.num_requests == 1, f'{conditional.num_requests} != 1'
         assert conditional.total_content_length == 1, f'{conditional.total_content_length} != 1'
 
     e2e_fixture.add_validator(validate_task_conditional)
     e2e_fixture.add_after_feature(after_feature)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
-            'And ask for value of variable "value"',
-            'When condition "{{ value | int > 5 }}" with name "conditional-1" is true, execute these tasks',
-            'Then log message "{{ value }} was greater than 5"',
+            'And ask for value of variable "value_1"',
+            'And ask for value of variable "value_2"',
+            'When condition "{{ value_1 | int > 5 }}" with name "conditional-1" is true, execute these tasks',
+            'Then log message "{{ value_1 }} was greater than 5"',
+            'But if condition is false, execute these tasks',
+            'Then log message "{{ value_1 }} was less than or equal to 5"',
+            'Then end condition',
+            'When condition "{{ value_2 | int > 5 }}" with name "conditional-2" is true, execute these tasks',
+            'Then log message "{{ value_2 }} was greater than 5"',
             'But if condition is false, execute these tasks',
-            'Then log message "{{ value }} was less than or equal to 5"',
+            'Then log message "{{ value_2 }} was less than or equal to 5"',
             'Then end condition',
         ],
     )
 
-    rc, output = e2e_fixture.execute(feature_file, testdata={'value': str(value)})
+    rc, output = e2e_fixture.execute(feature_file, testdata={'value_1': '1', 'value_2': '6'})
 
     assert rc == 0
     result = ''.join(output)
 
-    if value > 5:
-        assert f'{value} was greater than 5' in result
-    else:
-        assert f'{value} was less than or equal to 5' in result
+    assert '1 was greater than 5' not in result
+    assert '1 was less than or equal to 5' in result
+    assert '6 was greater than 5' in result
+    assert '6 was less than or equal to 5' not in result
 
 
 def test_e2e_step_task_loop(e2e_fixture: End2EndFixture) -> None:
     def validate_task_loop(context: Context) -> None:
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         grizzly.scenario.tasks().pop()  # remove dummy task
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/scenario/test_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,18 @@
             'And set context variable "auth.password" to "locust"',
         ],
         identifier=user_type,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    if user_type == 'Sftp':
+        assert rc == 1
+    else:
+        assert rc == 0
 
 
 @pytest.mark.parametrize('user_type,host', [
     ('RestApi', 'https://localhost/api',),
     ('MessageQueueUser', 'mq://mqm:secret@localhost/?QueueManager=QMGR01&Channel=Channel01',),
     ('ServiceBus', 'sb://localhost/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789=',),
     ('BlobStorageUser', 'DefaultEndpointsProtocol=https;EndpointSuffix=localhost;AccountName=examplestorage;AccountKey=xxxyyyyzzz==',),
@@ -102,8 +105,11 @@
             'And set context variable "auth.password" to "locust"',
         ],
         identifier=user_type,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    if user_type == 'Sftp':
+        assert rc == 1
+    else:
+        assert rc == 0
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/test_setup.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/steps/test_utils.py` & `grizzly-loadtester-2.6.4/tests/e2e/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_example.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_example.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_failure.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_failure.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
         expectations = [
             # failure exception is StopUser, abort user/scenario when there's a failure
             ('001 stop user', 'SCEN', 1, 1,),
             ('001 stop user', 'TSTD', 0, 1,),
             ('001 stop-get1', 'GET', 0, 1,),
             ('001 stop-get2', 'GET', 1, 1,),
-            ('001 stop-get3', 'GET', 0, 0,),
             # failure exception is RestartScenario, do not run steps after the failing step, restart from task 0
             ('002 restart scenario', 'SCEN', 1, 2,),
             ('002 restart scenario', 'TSTD', 0, 2,),
             ('002 restart-get1', 'GET', 0, 2,),
             ('002 restart-get2', 'GET', 1, 2,),
             ('002 restart-get3', 'GET', 0, 1,),
             # failure exception is None, just continue
@@ -78,10 +77,11 @@
         And repeat for "2" iterations
         Then get request with name "default-get1" from endpoint "/api/echo"
         Then get request with name "default-get2" from endpoint "/api/until/hello?nth=2&wrong=foobar&right=world | content_type=json"
         When response payload "$.hello" is not "world" fail request
         Then get request with name "default-get3" from endpoint "/api/echo"
     '''))
 
-    rc, _ = e2e_fixture.execute(feature_file)
+    rc, output = e2e_fixture.execute(feature_file)
 
-    assert rc == 0
+    assert rc == 1
+    assert "HOOK-ERROR in after_feature: RuntimeError: locust test failed" in ''.join(output)
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_iteration_pace.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_iteration_pace.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from grizzly.types.behave import Context, Feature
 
 from tests.fixtures import End2EndFixture
 
 
 def test_e2e_iteration_pace(e2e_fixture: End2EndFixture) -> None:
     def after_feature(context: Context, feature: Feature) -> None:
-        from grizzly.locust import on_master
-        if on_master(context):
+        from grizzly.locust import on_worker
+        if on_worker(context):
             return
 
         grizzly = cast(GrizzlyContext, context.grizzly)
 
         stats = grizzly.state.locust.environment.stats
 
         expectations = [
@@ -46,27 +46,38 @@
                 'host': f'http://{e2e_fixture.host}'
             }
         }
     }
 
     feature_file = e2e_fixture.create_feature(dedent(f'''Feature: Iteration Pace
     Background: common configuration
-        Given "1" user
+        Given "2" user
         And spawn rate is "1" user per second
         {start_webserver_step}
     Scenario: RequestTask
         Given a user of type "RestApi" load testing "http://{e2e_fixture.host}"
         And repeat for "3" iteration
         And set iteration time to "500" milliseconds
         And stop user on failure
         And value for variable "AtomicRandomInteger.sleep1" is "1..5"
         And value for variable "AtomicIntegerIncrementer.run_id" is "1"
         When condition "{{{{ AtomicIntegerIncrementer.run_id < 3 }}}}" with name "run" is true, execute these tasks
         Then get request with name "sleep-1" from endpoint "/api/sleep/{{{{ AtomicRandomInteger.sleep1 / 1000 / 2 }}}}"
         But if condition is false, execute these tasks
         Then get request with name "sleep-2" from endpoint "/api/sleep/0.6"
         Then end condition
+    Scenario: Dummy
+        Given a user of type "RestApi" load testing "http://{e2e_fixture.host}"
+        And repeat for "3" iteration
+        Then log message "dummy"
     '''))  # noqa: E501
 
-    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
+    rc, output = e2e_fixture.execute(feature_file, env_conf=env_conf)
+
+    result = ''.join(output)
 
-    assert rc == 0
+    assert rc == 1
+    assert 'HOOK-ERROR in after_feature: RuntimeError: locust test failed'
+    if e2e_fixture._distributed:
+        assert "1                  PACE 001 RequestTask: \"RuntimeError('pace falling behind')\"" in result  # ?!?!?!
+    else:
+        assert "1                  PACE 001 RequestTask: RuntimeError('pace falling behind')" in result
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_persistence.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_persistence.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_until.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_until.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             ('001 request-task, w=1.0s, r=2, em=1', 'UNTL', 0, 1,),
             ('002 HttpClientTask', 'SCEN', 0, 1,),
             ('002 HttpClientTask', 'TSTD', 0, 1,),
             ('002 http-client-task, w=1.0s, r=3, em=1', 'UNTL', 0, 1,),
             ('002 http-client-task', 'CLTSK', 1, 2,),
         ]
 
-        assert len(stats.errors) == 2, f'expected 0 logged errors, got {len(stats.errors)}'
+        assert len(stats.errors) == 0, f'expected 0 logged errors, got {len(stats.errors)}'
 
         for name, method, expected_num_failures, expected_num_requests in expectations:
             stat = stats.get(name, method)
             assert stat.num_failures == expected_num_failures, f'{stat.method}:{stat.name}.num_failures: {stat.num_failures} != {expected_num_failures}'
             assert stat.num_requests == expected_num_requests, f'{stat.method}:{stat.name}.num_requests: {stat.num_requests} != {expected_num_requests}'
 
     e2e_fixture.add_after_feature(after_feature)
```

### Comparing `grizzly-loadtester-2.6.3/tests/e2e/test_variables.py` & `grizzly-loadtester-2.6.4/tests/e2e/test_variables.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/fixtures.py` & `grizzly-loadtester-2.6.4/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1101,20 +1101,24 @@
             rc, output = run_command(
                 command,
                 cwd=str(self.root),
                 env=self._env,
             )
 
             if rc != 0:
-                print(''.join(output))
 
-                for container in ['master', 'worker'] if self._distributed else []:
-                    command = ['docker', 'container', 'logs', f'{self.root.name}-{getuser()}_{container}_1']
-                    _, output = run_command(
-                        command,
-                        cwd=str(self.root),
-                        env=self._env,
-                    )
+                if self._distributed:
+                    output = []
+
+                    for container in ['master', 'worker']:
+                        command = ['docker', 'container', 'logs', f'{self.root.name}-{getuser()}-{container}-1']
+                        _, o = run_command(
+                            command,
+                            cwd=str(self.root),
+                            env=self._env,
+                        )
 
-                    print(''.join(output))
+                        output += o
+
+                print(''.join(output))
 
             return rc, output
```

### Comparing `grizzly-loadtester-2.6.3/tests/helpers.py` & `grizzly-loadtester-2.6.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_appinsights.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_influxdb.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/listeners/test_influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/test_iterator.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/scenarios/test_iterator.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_setup.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from parse import compile
 from pytest_mock import MockerFixture
 
 from grizzly.context import GrizzlyContext
 from grizzly.steps import *  # pylint: disable=unused-wildcard-import  # noqa: F403
 from grizzly.testdata import GrizzlyVariables, GrizzlyVariableType
+from grizzly.tasks.clients import HttpClientTask
+from grizzly.types import RequestDirection, RequestMethod
 
 from tests.fixtures import BehaveFixture
 
 
 def test_parse_iteration_gramatical_number() -> None:
     p = compile(
         'run for {iteration:d} {iteration_number:IterationGramaticalNumber}',
@@ -171,14 +173,30 @@
     step_setup_set_context_variable(behave, 'url', 'HOST')
     assert grizzly.scenario.context == {
         'url': 'HOST',
         'tenant': 'example.com',
         'host': 'http://example.com',
     }
 
+    step_setup_set_context_variable(behave, 'www.example.com/auth.user.username', 'bob')
+    step_setup_set_context_variable(behave, 'www.example.com/auth.user.password', 'password')
+    assert grizzly.scenario.context == {
+        'url': 'HOST',
+        'tenant': 'example.com',
+        'host': 'http://example.com',
+        'www.example.com': {
+            'auth': {
+                'user': {
+                    'username': 'bob',
+                    'password': 'password',
+                },
+            },
+        },
+    }
+
 
 def test_step_setup_iterations(behave_fixture: BehaveFixture) -> None:
     behave = behave_fixture.context
     grizzly = cast(GrizzlyContext, behave.grizzly)
 
     assert grizzly.scenario.iterations == 1
 
@@ -317,10 +335,19 @@
     }
 
     grizzly.scenario.context['metadata'] = None
     request = RequestTask(RequestMethod.POST, endpoint='/api/test', name='request_task')
     grizzly.scenario.tasks.add(request)
     step_setup_metadata(behave, 'new_header', 'new_value')
 
-    assert grizzly.scenario.context.get('metadata', None) is None
-    assert request.metadata is not None
-    assert request.metadata.get('new_header') == 'new_value'
+    assert grizzly.scenario.context.get('metadata', {}) is None
+    assert request.metadata == {'new_header': 'new_value'}
+
+    grizzly.state.variables.update({'test_payload': 'none', 'test_metadata': 'none'})
+    task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable='test_payload', metadata_variable='test_metadata')
+
+    grizzly.scenario.tasks.add(task_factory)
+    step_setup_metadata(behave, 'x-test-header', 'foobar')
+
+    assert grizzly.scenario.context.get('metadata', {}) is None
+    assert request.metadata == {'new_header': 'new_value'}
+    assert task_factory._context['metadata'] == {'x-test-header': 'foobar'}
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_tasks.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/scenario/test_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test__helpers.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test__helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_setup.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/steps/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_http.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import cast
 from json import dumps as jsondumps, loads as jsonloads
+from unittest.mock import ANY
+from itertools import cycle
 
 import pytest
 
 from pytest_mock import MockerFixture
 from requests import Response
 from requests.structures import CaseInsensitiveDict
 
@@ -14,14 +16,40 @@
 from grizzly.types import RequestDirection
 from grizzly.types.locust import StopUser, CatchResponseError
 
 from tests.fixtures import GrizzlyFixture
 
 
 class TestHttpClientTask:
+    def test_on_start(self, grizzly_fixture: GrizzlyFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+
+        assert scenario is not None
+
+        behave = grizzly_fixture.behave
+        grizzly = cast(GrizzlyContext, behave.grizzly)
+        grizzly.state.variables.update({'test_payload': 'none', 'test_metadata': 'none'})
+
+        task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable='test_payload', metadata_variable='test_metadata')
+        task = task_factory()
+
+        task_factory.add_metadata('x-test-header', 'foobar')
+
+        assert getattr(task_factory, 'parent', None) is None
+        assert getattr(task_factory, 'environment', None) is None
+        assert getattr(task_factory, 'session_started', None) is None
+        assert task_factory.headers == {'x-grizzly-user': ANY}
+
+        task.on_start(scenario)
+
+        assert task_factory.parent is scenario
+        assert task_factory.environment is scenario.user.environment
+        assert getattr(task_factory, 'session_started', -1.0) >= 0.0
+        assert task_factory.headers == {'x-grizzly-user': ANY, 'x-test-header': 'foobar'}
+
     def test_get(self, mocker: MockerFixture, grizzly_fixture: GrizzlyFixture) -> None:
         behave = grizzly_fixture.behave
         grizzly = cast(GrizzlyContext, behave.grizzly)
 
         with pytest.raises(AttributeError) as ae:
             HttpClientTask(RequestDirection.TO, 'http://example.org', payload_variable='test')
         assert 'HttpClientTask: variable argument is not applicable for direction TO' in str(ae.value)
@@ -75,21 +103,22 @@
 
         task_factory.name = 'test-1'
         response.status_code = 400
         response.headers = CaseInsensitiveDict({'x-foo-bar': 'test'})
 
         task(scenario)
 
-        assert scenario.user._context['variables'].get('test_payload', '') == jsondumps({'hello': 'world'})
-        assert scenario.user._context['variables'].get('test_metadata', '') == jsondumps({'x-foo-bar': 'test'})
+        assert scenario.user._context['variables'].get('test_payload', None) is None
+        assert scenario.user._context['variables'].get('test_metadata', None) is None
         assert requests_get_spy.call_count == 1
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'http://example.org'
-        assert len(kwargs) == 1
+        assert len(kwargs) == 2
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
 
         assert request_fire_spy.call_count == 1
         _, kwargs = request_fire_spy.call_args_list[-1]
         assert kwargs.get('request_type', None) == 'CLTSK'
         assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} test-1'
         assert kwargs.get('response_time', None) >= 0.0
         assert kwargs.get('response_length') == len(jsondumps({'hello': 'world'}))
@@ -117,16 +146,17 @@
 
         task(scenario)
 
         assert scenario.user._context['variables'].get('test', '') is None  # not set
         assert requests_get_spy.call_count == 2
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'http://example.org'
-        assert len(kwargs) == 1
+        assert len(kwargs) == 2
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
 
         assert request_fire_spy.call_count == 2
         _, kwargs = request_fire_spy.call_args_list[-1]
         assert kwargs.get('request_type', None) == 'CLTSK'
         assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} test-2'
         assert kwargs.get('response_time', None) >= 0.0
         assert kwargs.get('response_length') == 0
@@ -146,16 +176,17 @@
         with pytest.raises(RestartScenario):
             task(scenario)
 
         assert scenario.user._context['variables'].get('test', '') is None  # not set
         assert requests_get_spy.call_count == 4
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'http://example.org'
-        assert len(kwargs) == 1
+        assert len(kwargs) == 2
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
 
         assert request_fire_spy.call_count == 4
         _, kwargs = request_fire_spy.call_args_list[-1]
         assert kwargs.get('request_type', None) == 'CLTSK'
         assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} test-4'
         assert kwargs.get('response_time', None) >= 0.0
         assert kwargs.get('response_length') == 0
@@ -172,16 +203,17 @@
 
         task(scenario)
 
         assert scenario.user._context['variables'].get('test', '') is None  # not set
         assert requests_get_spy.call_count == 5
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'http://example.org'
-        assert len(kwargs) == 1
+        assert len(kwargs) == 2
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
 
         assert request_fire_spy.call_count == 5
         _, kwargs = request_fire_spy.call_args_list[-1]
         assert kwargs.get('request_type', None) == 'CLTSK'
         assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} http-get'
         assert kwargs.get('response_time', None) >= 0.0
         assert kwargs.get('response_length') == 0
@@ -191,57 +223,72 @@
 
         grizzly.state.configuration['test.host'] = 'https://example.org'
 
         task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test', 'http-env-get', payload_variable='test')
         assert task_factory.arguments == {'verify': True}
         assert task_factory.content_type == TransformerContentType.UNDEFINED
         task = task_factory()
+        response.url = 'https://example.org/api/test'
+        requests_get_spy.side_effect = cycle([response])
 
         task(scenario)
 
         assert requests_get_spy.call_count == 6
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'https://example.org/api/test'
-        assert len(kwargs) == 2
+        assert len(kwargs) == 3
         assert kwargs.get('verify', None)
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
+
+        print(list(task_factory.log_dir.rglob('**/*')))
+
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
         task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=False, content_type=json', 'http-env-get-1', payload_variable='test')
         task = task_factory()
         assert task_factory.arguments == {'verify': False}
         assert task_factory.content_type == TransformerContentType.JSON
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
         task(scenario)
 
         assert requests_get_spy.call_count == 7
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'https://example.org/api/test'
-        assert len(kwargs) == 2
+        assert len(kwargs) == 3
         assert not kwargs.get('verify', None)
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert kwargs.get('cookies', None) == {}
         assert request_fire_spy.call_count == 7
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
         task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', payload_variable='test')
         task = task_factory()
         assert task_factory.arguments == {'verify': True}
         assert task_factory.content_type == TransformerContentType.JSON
 
         scenario.user._scenario.context['log_all_requests'] = True
+        task_factory._context['metadata'] = {'x-test-header': 'foobar'}
+
+        task.on_start(scenario)
+
+        assert task_factory.headers.get('x-test-header', None) == 'foobar'
 
         task(scenario)
 
         assert requests_get_spy.call_count == 8
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'https://example.org/api/test'
-        assert len(kwargs) == 2
+        assert len(kwargs) == 3
         assert kwargs.get('verify', None)
-        assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
+        headers = kwargs.get('headers', {})
+        assert headers.get('x-grizzly-user', None).startswith('HttpClientTask::')
+        assert headers.get('x-test-header', None) == 'foobar'
+        assert kwargs.get('cookies', None) == {}
         assert request_fire_spy.call_count == 8
         args, kwargs = request_fire_spy.call_args_list[-1]
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 6
 
         with pytest.raises(NotImplementedError) as nie:
             HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', payload_variable='test', text='foobar')
         assert str(nie.value) == 'HttpClientTask has not implemented support for step text'
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_servicebus.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/clients/test_servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_async_group.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_async_group.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_conditional.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_conditional.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_date.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_log_message.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_loop.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_loop.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_request.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_set_variable.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_set_variable.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_task_wait.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_timer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_transformer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_until.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_until.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from grizzly.types.locust import StopUser
 from grizzly.tasks import GrizzlyMetaRequestTask, UntilRequestTask, RequestTask
 from grizzly.tasks.clients import HttpClientTask
 from grizzly_extras.transformer import TransformerContentType, TransformerError, transformer
 
 from tests.fixtures import GrizzlyFixture
 
+parameterize = ('meta_request_task_type,meta_args,meta_kwargs', [
+    (RequestTask, (RequestMethod.GET,), {'name': 'test-request', 'endpoint': '/api/test | content_type=json'}),
+    (HttpClientTask, (RequestDirection.FROM, 'https://example.io/test | content_type=json', 'test-request',), {}),
+])
+
 
 class TestUntilRequestTask:
     def test___init__(self, grizzly_fixture: GrizzlyFixture) -> None:
         grizzly_fixture()
         grizzly = grizzly_fixture.grizzly
 
         request = RequestTask(RequestMethod.GET, name='test', endpoint='/api/test')
@@ -51,18 +56,15 @@
             UntilRequestTask(grizzly, request, '$.`this`[?status="ready"] | wait=0.0, retries=10')
         assert 'wait argument cannot be less than 0.1 seconds' in str(ve)
 
         with pytest.raises(ValueError) as ve:
             UntilRequestTask(grizzly, request, '$.`this`[?status="ready"] | wait=0.1, retries=0')
         assert 'retries argument cannot be less than 1' in str(ve)
 
-    @pytest.mark.parametrize('meta_request_task_type, meta_args, meta_kwargs', [
-        (RequestTask, (RequestMethod.GET,), {'name': 'test-request', 'endpoint': '/api/test | content_type=json'}),
-        (HttpClientTask, (RequestDirection.FROM, 'https://example.io/test | content_type=json', 'test-request',), {}),
-    ])
+    @pytest.mark.parametrize(*parameterize)
     def test___call__(
         self,
         grizzly_fixture: GrizzlyFixture,
         mocker: MockerFixture,
         caplog: LogCaptureFixture,
         meta_request_task_type: Type[GrizzlyMetaRequestTask],
         meta_args: Tuple[Any, ...],
@@ -423,7 +425,59 @@
 
         assert kwargs.get('request_type', None) == 'UNTL'
         assert kwargs.get('name', None) == f'{task_factory.scenario.identifier} test-request, w=4.0s, r=1, em=1'
         assert kwargs.get('response_time', None) == 111
         assert kwargs.get('response_length', None) == 0
         assert kwargs.get('context', None) == {'variables': {}}
         assert isinstance(kwargs.get('exception', ''), RuntimeError)
+
+    @pytest.mark.parametrize(*parameterize)
+    def test_on_start(
+        self,
+        grizzly_fixture: GrizzlyFixture,
+        mocker: MockerFixture,
+        meta_request_task_type: Type[GrizzlyMetaRequestTask],
+        meta_args: Tuple[Any, ...],
+        meta_kwargs: Dict[str, Any],
+    ) -> None:
+        _, _, scenario = grizzly_fixture()
+        assert scenario is not None
+
+        meta_request_task = meta_request_task_type(*meta_args, **meta_kwargs)
+
+        meta_request_task.scenario = grizzly_fixture.request_task.request.scenario
+        on_start_spy = mocker.spy(meta_request_task, 'on_start')
+
+        grizzly = grizzly_fixture.grizzly
+
+        task_factory = UntilRequestTask(grizzly, meta_request_task, "$.`this`[?status='ready'] | wait=100, retries=10", scenario=meta_request_task.scenario)
+        task = task_factory()
+
+        task.on_start(scenario)
+
+        on_start_spy.assert_called_once_with(scenario)
+
+    @pytest.mark.parametrize(*parameterize)
+    def test_on_stop(
+        self,
+        grizzly_fixture: GrizzlyFixture,
+        mocker: MockerFixture,
+        meta_request_task_type: Type[GrizzlyMetaRequestTask],
+        meta_args: Tuple[Any, ...],
+        meta_kwargs: Dict[str, Any],
+    ) -> None:
+        _, _, scenario = grizzly_fixture()
+        assert scenario is not None
+
+        meta_request_task = meta_request_task_type(*meta_args, **meta_kwargs)
+
+        meta_request_task.scenario = grizzly_fixture.request_task.request.scenario
+        on_stop_spy = mocker.spy(meta_request_task, 'on_stop')
+
+        grizzly = grizzly_fixture.grizzly
+
+        task_factory = UntilRequestTask(grizzly, meta_request_task, "$.`this`[?status='ready'] | wait=100, retries=10", scenario=meta_request_task.scenario)
+        task = task_factory()
+
+        task.on_stop(scenario)
+
+        on_stop_spy.assert_called_once_with(scenario)
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_wait.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/tasks/test_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_behave.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_behave.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import subprocess
+import sys
+
 from os import environ
 from typing import Any, Tuple, Dict, Optional, cast
 from time import perf_counter
 from json import dumps as jsondumps
 from shutil import rmtree
 from datetime import datetime
 
@@ -15,20 +18,51 @@
 
 from grizzly.types.behave import Context, Feature, Step, Status
 from grizzly.behave import before_feature, after_feature, before_scenario, after_scenario, before_step, after_step
 from grizzly.context import GrizzlyContext
 from grizzly.steps.setup import step_setup_variable_value_ask as step_both
 from grizzly.steps.background.setup import step_setup_save_statistics as step_background
 from grizzly.steps.scenario.setup import step_setup_iterations as step_scenario
-from grizzly.tasks import AsyncRequestGroupTask, TimerTask, ConditionalTask, LoopTask
+from grizzly.tasks import AsyncRequestGroupTask, TimerTask, ConditionalTask, LoopTask, LogMessageTask
+from grizzly.types import RequestType
 
-from tests.fixtures import BehaveFixture
+from tests.fixtures import BehaveFixture, GrizzlyFixture
 from tests.helpers import onerror
 
 
+def test_behave_no_pymqi_dependencies() -> None:
+    env = environ.copy()
+    try:
+        del env['LD_LIBRARY_PATH']
+    except KeyError:
+        pass
+
+    env['PYTHONPATH'] = '.'
+
+    process = subprocess.Popen(
+        [
+            sys.executable,
+            '-c',
+            (
+                'import grizzly.behave as gbehave;'
+                'print(f"{gbehave.pymqi.__name__=}");'
+            ),
+        ],
+        env=env,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+    )
+
+    out, _ = process.communicate()
+    output = out.decode()
+
+    assert process.returncode == 0
+    assert "gbehave.pymqi.__name__='grizzly_extras.dummy_pymqi'" in output
+
+
 def test_before_feature(behave_fixture: BehaveFixture, tmp_path_factory: TempPathFactory) -> None:
     context_root = tmp_path_factory.mktemp('test-context')
 
     behave = behave_fixture.context
     for key in ['GRIZZLY_CONTEXT_ROOT', 'GRIZZLY_FEATURE_FILE']:
         try:
             del environ[key]
@@ -54,14 +88,15 @@
         before_feature(context, feature)
 
         assert hasattr(context, 'grizzly')
         grizzly = cast(GrizzlyContext, context.grizzly)
         assert environ.get('GRIZZLY_CONTEXT_ROOT', None) == str(context_root)
         assert environ.get('GRIZZLY_FEATURE_FILE', None) == 'test.feature'
         assert grizzly.state.persistent == {}
+        assert context.last_task_count == {}
 
         context.grizzly = None
 
         (context_root / 'persistent').mkdir(exist_ok=True, parents=True)
         (context_root / 'persistent' / 'test.json').write_text(jsondumps({'foo': 'bar', 'hello': 'world'}, indent=2))
 
         before_feature(context, feature)
@@ -69,81 +104,126 @@
         assert hasattr(context, 'started')
         assert hasattr(context, 'grizzly')
         grizzly = cast(GrizzlyContext, context.grizzly)
         assert grizzly.state.persistent == {
             'foo': 'bar',
             'hello': 'world',
         }
+
+        GrizzlyContext.destroy()
+
+        before_feature(context, feature)
+
+        assert hasattr(context, 'started')
+        assert hasattr(context, 'grizzly')
+        grizzly = cast(GrizzlyContext, context.grizzly)
+        assert grizzly.state.persistent == {
+            'foo': 'bar',
+            'hello': 'world',
+        }
     finally:
         for key in ['GRIZZLY_CONTEXT_ROOT', 'GRIZZLY_FEATURE_FILE']:
             try:
                 del environ[key]
             except:
                 pass
 
         rmtree(context_root, onerror=onerror)
 
 
-def test_after_feature(behave_fixture: BehaveFixture, mocker: MockerFixture, capsys: CaptureFixture) -> None:
-    behave = behave_fixture.context
+def test_after_feature(grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, capsys: CaptureFixture) -> None:
+    behave = grizzly_fixture.behave
+    grizzly = grizzly_fixture.grizzly
     feature = Feature(None, None, '', '', scenarios=[behave.scenario])
-    behave.scenario.steps = [Step(None, None, '', '', '')]
+    behave.scenario.steps = [Step(None, None, '', '', ''), Step(None, None, '', '', '')]
     behave.started = datetime.now().astimezone()
 
-    class LocustRunning(Exception):
-        pass
-
-    mocker.patch(
+    locustrun_mock = mocker.patch(
         'grizzly.behave.locustrun',
-        side_effect=[LocustRunning]
+        return_value=0
     )
 
     # do not start locust if feature failed
     feature.set_status(Status.failed)
 
-    after_feature(behave, feature)
+    with pytest.raises(RuntimeError) as re:
+        after_feature(behave, feature)
+    assert str(re.value) == 'failed to prepare locust test'
+
+    locustrun_mock.assert_not_called()
 
     # start locust only if it's not a dry run and the feature passed
     feature.set_status(Status.passed)
 
-    with pytest.raises(LocustRunning):
-        after_feature(behave, feature)
-
-    mocker.patch(
-        'grizzly.behave.locustrun',
-        side_effect=[1, 123]
-    )
+    after_feature(behave, feature)
 
     assert feature.status == Status.passed
+    locustrun_mock.assert_called_once_with(behave)
+    locustrun_mock.reset_mock()
 
     capsys.readouterr()
 
-    after_feature(behave, feature)
+    # locustrun failed, and we actually had a grizzly scenario matching the behave scenario
+    locustrun_mock.return_value = 1
+    behave.scenario.name = 'test'
+    grizzly.scenarios.clear()
+    grizzly.scenarios.create(behave.scenario)
+    grizzly.scenario.description = behave.scenario.name
+
+    with pytest.raises(RuntimeError) as re:
+        after_feature(behave, feature)
+    assert str(re.value) == 'locust test failed'
+
+    locustrun_mock.assert_called_once_with(behave)
+    locustrun_mock.reset_mock()
 
     capture = capsys.readouterr()
 
     assert feature.status == Status.failed
     assert feature.duration == 0.0
     assert capture.err == ''
 
-    behave.start = perf_counter() - 1.0
+    # fail based on locust statistics having a feature/scenario that has failed
     feature.set_status(Status.passed)
+    locustrun_mock.return_value = 0
+    grizzly.state.locust.environment.stats.log_error(RequestType.SCENARIO(), '001 test', 'error error')
+    grizzly.state.locust.environment.stats.log_error(RequestType.SCENARIO(), '002 test', 'error error')
 
-    after_feature(behave, feature)
+    with pytest.raises(RuntimeError) as re:
+        after_feature(behave, feature)
+    assert str(re.value) == 'locust test failed'
 
-    capture = capsys.readouterr()
+    locustrun_mock.assert_called_once_with(behave)
+    locustrun_mock.reset_mock()
 
-    assert feature.duration > 0.0
-    assert capture.err == ''
+    # if the scenario had any errors, we should fail
+    grizzly.state.locust.environment.stats.clear_all()
+    grizzly.state.locust.environment.stats.log_request(RequestType.SCENARIO(), '001 test', 2, 3)
+    grizzly.state.locust.environment.stats.log_error(RequestType.UNTIL(), '001 until', 'error error')
+    grizzly.state.locust.environment.stats.log_error('GET', '001 get', 'foobared')
 
-    # feature is failed, will never start locust
-    after_feature(behave, feature)
+    with pytest.raises(RuntimeError) as re:
+        after_feature(behave, feature)
+    assert str(re.value) == 'locust test failed'
+
+    locustrun_mock.assert_called_once_with(behave)
+    locustrun_mock.reset_mock()
+
+    behave.start = perf_counter() - 1.0
+    feature.set_status(Status.passed)
+    locustrun_mock.return_value = 123
+
+    with pytest.raises(RuntimeError) as re:
+        after_feature(behave, feature)
+    assert str(re.value) == 'locust test failed'
 
     capture = capsys.readouterr()
 
+    assert feature.status == Status.failed
+    assert feature.duration > 0.0
     assert capture.err == ''
 
 
 def test_before_scenario(behave_fixture: BehaveFixture, mocker: MockerFixture) -> None:
     behave = behave_fixture.context
 
     class MatchedStep:
@@ -183,14 +263,15 @@
         background_background_step,
         both_step,
         local_step,
         None,
     ]
 
     behave.scenario.steps += [scenario_background_step, both_step, local_step, None]
+    behave.last_task_count = {}
 
     assert len(behave.scenario.steps) == 5
     assert len(behave.scenario.background.steps) == 5
 
     grizzly = cast(GrizzlyContext, behave.grizzly)
 
     assert len(grizzly.scenarios()) == 0
@@ -286,11 +367,29 @@
 
     setattr(step, 'location_status', 'incorrect')
 
     with pytest.raises(AssertionError):
         before_step(behave, step)
 
 
-def test_after_step(behave_fixture: BehaveFixture) -> None:
-    behave = behave_fixture.context
-    step = Step(filename=None, line=None, keyword='', step_type='step', name='')
+def test_after_step(grizzly_fixture: GrizzlyFixture) -> None:
+    behave = grizzly_fixture.behave
+    grizzly = grizzly_fixture.grizzly
+
+    behave.last_task_count = {}
+    step = Step(filename=None, line=None, keyword='And', step_type='step', name='this is a grizzly step')
+
+    after_step(behave, step)
+
+    assert grizzly.scenario.tasks.behave_steps == {}
+
+    # create grizzly scenario
+    behave.feature = Feature(None, None, '', '', scenarios=[behave.scenario])
+    behave.scenario.name = 'test'
+    behave.scenario.steps = [step]
+    grizzly.scenarios.create(behave.scenario)
+    grizzly.scenario.tasks.add(LogMessageTask('hello world'))
+    behave.last_task_count = {grizzly.scenario.identifier: 0}
+
     after_step(behave, step)
+
+    assert grizzly.scenario.tasks.behave_steps == {2: 'And this is a grizzly step'}
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_clients.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_context.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_locust.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_types.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,32 @@
         assert str(ae.value) == 'foobar does not exist'
 
     @pytest.mark.parametrize('input', [e for e in RequestType])
     def test___call___and___str__(self, input: RequestType) -> None:
         assert input() == input.value[0] == str(input)
 
     def test_weight(self) -> None:
-        assert RequestType.SCENARIO.weight == 0
+        assert RequestType.AUTH.weight == 0
+        assert RequestType.SCENARIO.weight == 1
         assert RequestType.TESTDATA.weight > RequestType.SCENARIO.weight
         assert RequestType.UNTIL.weight > RequestType.TESTDATA.weight
         assert RequestType.VARIABLE.weight == RequestType.UNTIL.weight
         assert RequestType.ASYNC_GROUP.weight == RequestType.VARIABLE.weight
         assert RequestType.CLIENT_TASK.weight == RequestType.ASYNC_GROUP.weight
         assert RequestType.HELLO.weight == RequestType.CLIENT_TASK.weight
         assert RequestType.RECEIVE.weight == RequestType.HELLO.weight
         assert RequestType.CONNECT.weight == RequestType.RECEIVE.weight
 
     def test_get_method_weight(self) -> None:
         assert RequestType.get_method_weight('ASDF') == RequestType.get_method_weight('GET')
         assert RequestType.get_method_weight('GET') == RequestType.get_method_weight('POST')
-        assert RequestType.get_method_weight('SCEN') == 0
-        assert RequestType.get_method_weight('TSTD') == 1
-        assert RequestType.get_method_weight('PACE') == 2
+        assert RequestType.get_method_weight('AUTH') == 0
+        assert RequestType.get_method_weight('SCEN') == 1
+        assert RequestType.get_method_weight('TSTD') == 2
+        assert RequestType.get_method_weight('PACE') == 3
 
         for request_type in RequestType:
             if request_type.weight < 10:
                 continue
 
             assert RequestType.get_method_weight(request_type.alias) == 10
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_utils.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,22 +194,22 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': None,
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': None,
     }
     user_type_1 = user_class_type_1(locust_fixture.env)
 
     assert user_type_1.headers == {
-        'Authorization': None,
         'Content-Type': 'application/json',
         'x-grizzly-user': f'grizzly.users.RestApiUser_{scenario.identifier}',
     }
     assert user_type_1.context() == {
         'log_all_requests': False,
         'variables': {},
         'verify_certificates': True,
@@ -221,14 +221,15 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': None,
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': None,
     }
     assert user_type_1._scenario is scenario
 
     scenario = GrizzlyContextScenario(1)
@@ -277,25 +278,25 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': 'grizzly-user',
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': {
             'Content-Type': 'application/xml',
             'Foo-Bar': 'hello world',
         },
     }
 
     user_type_2 = user_class_type_2(locust_fixture.env)
     assert user_type_2.headers == {
-        'Authorization': None,
         'Content-Type': 'application/xml',
         'x-grizzly-user': f'RestApiUser_{scenario.identifier}',
         'Foo-Bar': 'hello world',
     }
     assert user_type_2.context() == {
         'log_all_requests': True,
         'variables': {},
@@ -311,14 +312,15 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': 'grizzly-user',
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': {
             'Content-Type': 'application/xml',
             'Foo-Bar': 'hello world',
         },
     }
@@ -352,14 +354,15 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': None,
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': None,
     }
 
     assert user_class_type_1.host is not user_class_type_2.host
     assert user_class_type_2.host is not user_class_type_3.host
@@ -388,14 +391,15 @@
                 'secret': None,
                 'resource': None,
             },
             'user': {
                 'username': None,
                 'password': None,
                 'redirect_uri': None,
+                'initialize_uri': None,
             },
         },
         'metadata': None,
     }
 
     with pytest.raises(AttributeError):
         scenario = GrizzlyContextScenario(1)
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_ast.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_ast.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_communication.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_communication.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,16 +130,16 @@
                 assert 'AtomicIntegerIncrementer.messageID' in variables
                 assert 'AtomicDate.now' in variables
                 assert 'messageID' in variables
                 assert 'AtomicDate.utc' in variables
                 assert variables['AtomicIntegerIncrementer.messageID'] == 456
                 assert variables['messageID'] == 123
                 assert variables['AtomicDirectoryContents.test'] == f'adirectory{sep}file1.txt'
-                assert 'AtomicCsvReader.test.header1' not in variables
-                assert 'AtomicCsvReader.test.header2' not in variables
+                assert variables['AtomicCsvReader.test.header1'] == 'value1'
+                assert variables['AtomicCsvReader.test.header2'] == 'value2'
                 assert variables['AtomicIntegerIncrementer.value'] == 1
                 utc_date = variables['AtomicDate.utc']
                 assert 'T' in utc_date and utc_date.endswith('Z')
                 assert data['auth.user.username'] == 'value1'
                 assert data['auth.user.password'] == 'value2'
                 assert variables['tests.helpers.AtomicCustomVariable.foo'] == 'bar'
 
@@ -150,16 +150,16 @@
                 variables = data['variables']
                 assert 'AtomicIntegerIncrementer.messageID' in variables
                 assert 'AtomicDate.now' in variables
                 assert 'messageID' in variables
                 assert variables['AtomicIntegerIncrementer.messageID'] == 457
                 assert variables['messageID'] == 123
                 assert variables['AtomicDirectoryContents.test'] == f'adirectory{sep}file2.txt'
-                assert 'AtomicCsvReader.test.header1' not in variables
-                assert 'AtomicCsvReader.test.header2' not in variables
+                assert variables['AtomicCsvReader.test.header1'] == 'value3'
+                assert variables['AtomicCsvReader.test.header2'] == 'value4'
                 assert variables['AtomicIntegerIncrementer.value'] == 6
                 assert data['auth.user.username'] == 'value3'
                 assert data['auth.user.password'] == 'value4'
 
                 message = get_message_from_producer()
                 assert message['action'] == 'stop'
                 assert 'data' not in message
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_utils.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,36 @@
 
         grizzly.state.configuration['test.auth.refresh_time'] = 3000
         assert create_context_variable(grizzly, 'test.value', '$conf::test.auth.refresh_time$') == {
             'test': {
                 'value': 3000,
             }
         }
+
+        assert create_context_variable(grizzly, 'www.example.com/auth.user.username', 'bob') == {
+            'www.example.com': {
+                'auth': {
+                    'user': {
+                        'username': 'bob',
+                    },
+                },
+            },
+        }
+
+        grizzly.state.configuration.update({'test.host': 'www.example.net'})
+
+        assert create_context_variable(grizzly, '$conf::test.host$/auth.user.username', 'bob') == {
+            'www.example.net': {
+                'auth': {
+                    'user': {
+                        'username': 'bob',
+                    },
+                },
+            },
+        }
     finally:
         GrizzlyContext.destroy()
         try:
             del environ['HELLO_WORLD']
         except KeyError:
             pass
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_date.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_integer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_string.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/testdata/variables/test_random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_grizzly_user.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_grizzly_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_request_logger.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_request_logger.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_event.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_handler.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/base/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_blobstorage.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_dummy.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_iothub.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_messagequeue.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_servicebus.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_servicebus.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_sftp.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly/users/test_sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,53 +22,51 @@
     def test_create(self, locust_fixture: LocustFixture, tmp_path_factory: TempPathFactory) -> None:
         test_context = tmp_path_factory.mktemp('test_context') / 'requests'
         test_context.mkdir()
         test_context_root = path.dirname(str(test_context))
         environ['GRIZZLY_CONTEXT_ROOT'] = test_context_root
 
         try:
-            SftpUser.host = 'http://test.nu'
+            SftpUser.host = 'http://example.com'
 
             with pytest.raises(ValueError):
                 SftpUser(locust_fixture.env)
 
-            SftpUser.host = 'sftp://username:password@test.nu'
+            SftpUser.host = 'sftp://username:password@example.com'
 
             with pytest.raises(ValueError):
                 SftpUser(locust_fixture.env)
 
-            SftpUser.host = 'sftp://test.nu/pub/test'
+            SftpUser.host = 'sftp://example.com/pub/test'
 
             with pytest.raises(ValueError):
                 SftpUser(locust_fixture.env)
 
-            SftpUser.host = 'sftp://test.nu'
+            SftpUser.host = 'sftp://example.com'
 
             with pytest.raises(ValueError):
                 SftpUser(locust_fixture.env)
 
             SftpUser._context['auth']['username'] = 'syrsa'
 
             with pytest.raises(ValueError):
                 SftpUser(locust_fixture.env)
 
             SftpUser._context['auth']['password'] = 'hemligaarne'
 
             user = SftpUser(locust_fixture.env)
 
-            assert isinstance(user.sftp_client, SftpClientSession)
-            assert user.sftp_client.port == 22
-            assert user.sftp_client.host == 'test.nu'
+            assert user.port == 22
+            assert user.host == 'example.com'
 
-            SftpUser.host = 'sftp://test.nu:1337'
+            SftpUser.host = 'sftp://example.com:1337'
             user = SftpUser(locust_fixture.env)
 
-            assert isinstance(user.sftp_client, SftpClientSession)
-            assert user.sftp_client.port == 1337
-            assert user.sftp_client.host == 'test.nu'
+            assert user.port == 1337
+            assert user.host == 'example.com'
 
             SftpUser._context['auth']['key_file'] = '~/.ssh/id_rsa'
 
             with pytest.raises(NotImplementedError):
                 SftpUser(locust_fixture.env)
         finally:
             shutil.rmtree(test_context_root)
@@ -80,26 +78,24 @@
         SftpUser._context['auth'] = {
             'username': 'test',
             'password': 'hemligaarne',
             'key_file': None,
         }
         user = SftpUser(locust_fixture.env)
 
-        session_spy = mocker.patch.object(user.sftp_client, 'session', return_value=mocker.MagicMock())
+        sftp_client_mock = mocker.spy(SftpClientSession, '__init__')
+        session_spy = mocker.patch.object(SftpClientSession, 'session', return_value=mocker.MagicMock())
 
         assert not hasattr(user, 'session')
 
         user.on_start()
 
         assert hasattr(user, 'session')
-        assert session_spy.call_count == 1
-        args, kwargs = session_spy.call_args_list[-1]
-        assert len(args) == 0
-        assert kwargs == user._context['auth']
-
+        sftp_client_mock.assert_called_once_with(user.sftp_client, user.host, user.port)
+        session_spy.assert_called_once_with(**user._context['auth'])
         assert session_spy.return_value.__enter__.call_count == 1
 
     def test_on_stop(self, locust_fixture: LocustFixture, paramiko_fixture: ParamikoFixture, mocker: MockerFixture) -> None:
         paramiko_fixture()
         SftpUser.host = 'sftp://example.org'
         SftpUser._context['auth'] = {
             'username': 'test',
```

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test___init__.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_daemon.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_daemon.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_sb.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/async_message/test_sb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_arguments.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_arguments.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_transformer.py` & `grizzly-loadtester-2.6.4/tests/unit/test_grizzly_extras/test_transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.3/tests/webserver.py` & `grizzly-loadtester-2.6.4/tests/webserver.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 from flask import Flask, request, jsonify, Response as FlaskResponse, Request as FlaskRequest
 from werkzeug.datastructures import Headers as FlaskHeaders
 
 logger = logging.getLogger('webserver')
 
 
+auth_expected: Optional[Dict[str, Any]] = None
+
+
 app = Flask('webserver')
 
 # ugly hack to get correct path when webserver.py is injected for running distributed
 root_dir = (Path(__file__).parent / '..').resolve()
 
 if '/srv/grizzly' not in str(root_dir):
     root_dir = root_dir / 'example' / 'features'
@@ -73,24 +76,52 @@
     })
 
 
 def get_headers(request: FlaskRequest) -> FlaskHeaders:
     return FlaskHeaders({key: value for key, value in request.headers.items() if not key.lower() == 'content-length'})
 
 
-@app.route('/api/echo')
+@app.route('/api/statuscode/<statuscode>')
+def app_statuscode(statuscode: int) -> FlaskResponse:
+    response = jsonify({'message': 'a-okay!'})
+    response.status_code = statuscode
+
+    return response
+
+
+@app.route('/api/echo', methods=['POST', 'PUT', 'GET'])
 def app_echo() -> FlaskResponse:
     if request.method in ['POST', 'PUT']:
         payload = request.json
     elif request.method == 'GET':
         payload = {}
 
         for key, value in request.args.items():
             payload[key] = value
 
+    if auth_expected is not None:
+        try:
+            assert request.headers.get('Authorization', '') == f'Bearer {auth_expected["token"]}', 'not authenticated'
+
+            expected_headers = auth_expected.get('headers', None)
+            if expected_headers is not None:
+                for key, expected_value in expected_headers.items():
+                    actual_value = request.headers.get(key, '')
+                    assert actual_value == expected_value, f'header {key}: {actual_value} != {expected_value}'
+
+        except AssertionError as e:
+            response = jsonify({'message': str(e)})
+
+            if str(e) == 'not authenticated':
+                response.status_code = 401
+            else:
+                response.status_code = 403
+
+            return response
+
     headers = get_headers(request)
 
     response = jsonify(payload)
     response.headers = headers
     response.status_code = 200
 
     return response
@@ -152,14 +183,42 @@
 
     response = jsonify(json_result)
     response.status_code = status_code
 
     return response
 
 
+@app.route('/oauth2/authorize')
+def app_oauth2_authorize() -> FlaskResponse:
+    return jsonify({'message': 'not implemented'}, status=400)
+
+
+@app.route('/oauth2/token', methods=['POST'])
+def app_oauth2_token() -> FlaskResponse:
+    form = request.form
+
+    logger.debug(f'/oauth2/token called with {form=}')
+
+    if auth_expected is None:
+        response = jsonify({'error_description': 'not setup for authentication'})
+        response.status_code = 400
+        return response
+
+    try:
+        assert form['grant_type'] == 'client_credentials', f'grant_type {form["grant_type"]} != client_credentials'
+        assert form['client_secret'] == auth_expected['client']['secret'], f'client_secret {form["client_secret"]} != {auth_expected["client"]["secret"]}'
+        assert form['client_id'] == auth_expected['client']['id'], f'client_id {form["client_id"]} != {auth_expected["client"]["id"]}'
+    except AssertionError as e:
+        response = jsonify({'error_description': str(e)})
+        response.status_code = 400
+        return response
+
+    return jsonify({'access_token': auth_expected['token']})
+
+
 @app.errorhandler(404)
 def catch_all(_: Any) -> FlaskResponse:
     return jsonify({}, status=200)
 
 
 class Webserver:
     _web_server: WSGIServer
@@ -173,14 +232,27 @@
         )
         logger.debug(f'created webserver on port {port}')
 
     @property
     def port(self) -> int:
         return cast(int, self._web_server.server_port)
 
+    @property
+    def auth(self) -> Optional[Dict[str, Any]]:
+        return auth_expected
+
+    @auth.setter
+    def auth(self, value: Optional[Dict[str, Any]]) -> None:
+        global auth_expected
+        auth_expected = value
+
+    @property
+    def auth_provider_uri(self) -> str:
+        return '/oauth2'
+
     def start(self) -> None:
         self._greenlet = gevent.spawn(lambda: self._web_server.serve_forever())
         gevent.sleep(0.01)
         logger.debug(f'started webserver on port {self.port}')
 
     def __enter__(self) -> 'Webserver':
         self.start()
```

