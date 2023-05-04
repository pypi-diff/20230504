# Comparing `tmp/irails-1.1.2.tar.gz` & `tmp/irails-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.2.tar", last modified: Wed May  3 14:54:30 2023, max compression
+gzip compressed data, was "irails-1.1.3.tar", last modified: Thu May  4 04:33:18 2023, max compression
```

## Comparing `irails-1.1.2.tar` & `irails-1.1.3.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.545630 irails-1.1.2/
--rw-rw-rw-   0        0        0       39 2023-04-30 09:03:04.000000 irails-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6937 2023-05-03 14:54:30.543624 irails-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6156 2023-05-03 14:54:30.000000 irails-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.461842 irails-1.1.2/irails/
--rw-rw-rw-   0        0        0      318 2023-05-03 14:19:47.000000 irails-1.1.2/irails/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-05-02 08:43:36.000000 irails-1.1.2/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.2/irails/_utils.py
--rw-rw-rw-   0        0        0    11616 2023-05-02 08:29:17.000000 irails-1.1.2/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.2/irails/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.2/irails/cbv.py
--rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.2/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.2/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.2/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14411 2023-05-03 14:49:52.000000 irails-1.1.2/irails/core.py
--rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.2/irails/database.py
--rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.2/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.2/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.2/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.483783 irails-1.1.2/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.2/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.2/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7133 2023-05-03 07:16:46.000000 irails-1.1.2/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.2/irails/scripts/_project.py
--rw-rw-rw-   0        0        0      591 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1702 2023-05-03 14:31:14.000000 irails-1.1.2/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.418322 irails-1.1.2/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.497745 irails-1.1.2/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.2/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.2/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.2/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.2/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.2/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.2/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.2/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.500739 irails-1.1.2/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.2/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.503730 irails-1.1.2/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.2/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.517693 irails-1.1.2/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.2/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.2/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.2/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.2/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.2/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.2/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.2/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.522679 irails-1.1.2/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.2/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.2/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.525671 irails-1.1.2/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.425304 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.531655 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.537639 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.427299 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.540631 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.2/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.473811 irails-1.1.2/irails.egg-info/
--rw-rw-rw-   0        0        0     6937 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      767 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 14:54:30.546615 irails-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.847989 irails-1.1.3/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6937 2023-05-04 04:33:18.846994 irails-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6156 2023-05-04 04:33:18.000000 irails-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.798123 irails-1.1.3/irails/
+-rw-rw-rw-   0        0        0      318 2023-05-04 04:32:01.000000 irails-1.1.3/irails/__init__.py
+-rw-rw-rw-   0        0        0     1682 2023-05-02 08:43:36.000000 irails-1.1.3/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.3/irails/_utils.py
+-rw-rw-rw-   0        0        0    11616 2023-05-02 08:29:17.000000 irails-1.1.3/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.3/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.807101 irails-1.1.3/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.808103 irails-1.1.3/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.3/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.3/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.3/irails/cbv.py
+-rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.3/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.3/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.3/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14305 2023-05-04 04:15:21.000000 irails-1.1.3/irails/core.py
+-rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.3/irails/database.py
+-rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.3/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.3/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.3/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.813083 irails-1.1.3/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.3/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.3/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7133 2023-05-03 07:16:46.000000 irails-1.1.3/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.3/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.3/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1702 2023-05-03 14:31:14.000000 irails-1.1.3/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.774300 irails-1.1.3/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.821063 irails-1.1.3/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.3/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.3/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.3/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.3/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.3/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.3/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.3/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.3/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.824054 irails-1.1.3/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.3/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.825051 irails-1.1.3/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.3/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.831036 irails-1.1.3/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.3/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.3/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.3/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.3/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.3/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.3/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.3/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.3/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.833034 irails-1.1.3/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.3/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.3/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.835026 irails-1.1.3/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.778288 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.840021 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.844019 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.779285 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.844999 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.3/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.804108 irails-1.1.3/irails.egg-info/
+-rw-rw-rw-   0        0        0     6937 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 04:33:18.847989 irails-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.3/setup.py
```

### Comparing `irails-1.1.2/PKG-INFO` & `irails-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.2/README.md` & `irails-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/_loader.py` & `irails-1.1.3/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/_utils.py` & `irails-1.1.3/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/auth.py` & `irails-1.1.3/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/base_controller.py` & `irails-1.1.3/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/cbv.py` & `irails-1.1.3/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/config.py` & `irails-1.1.3/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/controller.py` & `irails-1.1.3/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/controller_utils.py` & `irails-1.1.3/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/core.py` & `irails-1.1.3/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,13 @@
         _log.info("init casbin auth system...")
         application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
     _log.info("init mvc app end.")
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
-    global __is_debug
-    host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
-    port = "port" in kwargs  and kwargs["port"] or 8000  
+    global __is_debug 
     if  "debug" in kwargs:
-        __is_debug = kwargs["debug"]  
+        __is_debug = kwargs["debug"] 
+        del kwargs['debug'] 
      
-    uvicorn.run(app, host=host, port=port)
+    uvicorn.run(app, **kwargs)
```

### Comparing `irails-1.1.2/irails/database.py` & `irails-1.1.3/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/midware.py` & `irails-1.1.3/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/midware_casbin.py` & `irails-1.1.3/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/midware_session.py` & `irails-1.1.3/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/_app.py` & `irails-1.1.3/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/_controller.py` & `irails-1.1.3/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/_project.py` & `irails-1.1.3/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/main.py` & `irails-1.1.3/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/app/controller.tpl` & `irails-1.1.3/irails/scripts/tpls/app/controller.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.3/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/app/home.tpl` & `irails-1.1.3/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.3/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.3/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.3/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.3/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.3/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails/view.py` & `irails-1.1.3/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.2/irails.egg-info/PKG-INFO` & `irails-1.1.3/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.2/irails.egg-info/SOURCES.txt` & `irails-1.1.3/irails.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 irails.egg-info/PKG-INFO
 irails.egg-info/SOURCES.txt
 irails.egg-info/dependency_links.txt
 irails.egg-info/entry_points.txt
 irails.egg-info/requires.txt
 irails.egg-info/top_level.txt
 irails/scripts/main.py
+irails/casbin_adapters/sqlalchemy_adapter.py
+irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
 irails/scripts/__init__.py
 irails/scripts/_app.py
 irails/scripts/_controller.py
 irails/scripts/_project.py
 irails/scripts/_run.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
```

### Comparing `irails-1.1.2/irails.egg-info/requires.txt` & `irails-1.1.3/irails.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -39,8 +39,7 @@
 ujson==5.5.0
 urllib3==1.26.15
 uvicorn==0.21.1
 watchfiles==0.19.0
 websockets==11.0.2
 yarg==0.1.9
 chardet==5.1.0
-pusher==3.3.2
```

### Comparing `irails-1.1.2/setup.py` & `irails-1.1.3/setup.py`

 * *Files identical despite different names*

