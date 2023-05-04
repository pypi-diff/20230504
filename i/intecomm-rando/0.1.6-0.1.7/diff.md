# Comparing `tmp/intecomm-rando-0.1.6.tar.gz` & `tmp/intecomm-rando-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-rando-0.1.6.tar", last modified: Sat Apr 22 18:11:51 2023, max compression
+gzip compressed data, was "intecomm-rando-0.1.7.tar", last modified: Thu May  4 03:04:45 2023, max compression
```

## Comparing `intecomm-rando-0.1.6.tar` & `intecomm-rando-0.1.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311874 intecomm-rando-0.1.6/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.302187 intecomm-rando-0.1.6/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.305549 intecomm-rando-0.1.6/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.6/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-04-22 18:11:51.311957 intecomm-rando-0.1.6/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.307379 intecomm-rando-0.1.6/intecomm_rando/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.6/intecomm_rando/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/intecomm_rando/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.6/intecomm_rando/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/group_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/group_identifier.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.308785 intecomm-rando-0.1.6/intecomm_rando/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.309440 intecomm-rando-0.1.6/intecomm_rando/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-01-23 15:17:57.000000 intecomm-rando-0.1.6/intecomm_rando/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/randomization_list.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/registered_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2269 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4942 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/randomize_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1320 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.309829 intecomm-rando-0.1.6/intecomm_rando/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.6/intecomm_rando/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311505 intecomm-rando-0.1.6/intecomm_rando/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/intecomm_rando/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.6/intecomm_rando/tests/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.311751 intecomm-rando-0.1.6/intecomm_rando/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.6/intecomm_rando/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-04-22 18:11:43.000000 intecomm-rando-0.1.6/intecomm_rando/tests/tests/test_rando_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.6/intecomm_rando/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-22 18:11:51.308306 intecomm-rando-0.1.6/intecomm_rando.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-04-22 18:11:51.000000 intecomm-rando-0.1.6/intecomm_rando.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.6/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-04-22 18:11:51.312288 intecomm-rando-0.1.6/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838839 intecomm-rando-0.1.7/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.822990 intecomm-rando-0.1.7/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.828479 intecomm-rando-0.1.7/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.7/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-04 03:04:45.838947 intecomm-rando-0.1.7/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.830843 intecomm-rando-0.1.7/intecomm_rando/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.7/intecomm_rando/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/intecomm_rando/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.7/intecomm_rando/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/group_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/group_identifier.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.834064 intecomm-rando-0.1.7/intecomm_rando/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.834920 intecomm-rando-0.1.7/intecomm_rando/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-05-03 01:50:00.000000 intecomm-rando-0.1.7/intecomm_rando/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/models/randomization_list.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/models/registered_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3116 2023-05-04 03:04:38.000000 intecomm-rando-0.1.7/intecomm_rando/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4962 2023-05-04 03:04:38.000000 intecomm-rando-0.1.7/intecomm_rando/randomize_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1320 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.835475 intecomm-rando-0.1.7/intecomm_rando/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.7/intecomm_rando/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838213 intecomm-rando-0.1.7/intecomm_rando/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/tests/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838565 intecomm-rando-0.1.7/intecomm_rando/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.7/intecomm_rando/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-05-04 03:04:20.000000 intecomm-rando-0.1.7/intecomm_rando/tests/tests/test_rando_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/intecomm_rando/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.831966 intecomm-rando-0.1.7/intecomm_rando.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-05-04 03:04:45.839497 intecomm-rando-0.1.7/setup.cfg
```

### Comparing `intecomm-rando-0.1.6/.github/workflows/build.yml` & `intecomm-rando-0.1.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/.gitignore` & `intecomm-rando-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/.pre-commit-config.yaml` & `intecomm-rando-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/LICENSE` & `intecomm-rando-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/PKG-INFO` & `intecomm-rando-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.6
+Version: 0.1.7
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.6/README.rst` & `intecomm-rando-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/group_eligibility.py` & `intecomm-rando-0.1.7/intecomm_rando/group_eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/group_identifier.py` & `intecomm-rando-0.1.7/intecomm_rando/group_identifier.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/migrations/0001_initial.py` & `intecomm-rando-0.1.7/intecomm_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py` & `intecomm-rando-0.1.7/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/models/randomization_list.py` & `intecomm-rando-0.1.7/intecomm_rando/models/randomization_list.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/models/registered_group.py` & `intecomm-rando-0.1.7/intecomm_rando/models/registered_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/models/signals.py` & `intecomm-rando-0.1.7/intecomm_rando/models/signals.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,48 @@
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 from edc_constants.constants import COMPLETE, UUID_PATTERN, YES
 from edc_randomization.constants import RANDOMIZED
 from edc_randomization.randomizer import RandomizationError
 from edc_randomization.utils import get_object_for_subject
 from edc_registration.models import RegisteredSubject
+from edc_visit_schedule import site_visit_schedules
 
-from ..randomize_group import randomize_group
+from ..constants import CLINIC_CONTROL, COMM_INTERVENTION
+from ..randomize_group import RandomizeGroup
 
 
 @receiver(
     post_save,
     weak=False,
     dispatch_uid="randomize_group_on_post_save",
 )
 def randomize_patient_group_on_post_save(sender, instance, raw, **kwargs):
-    """Randomize a patient group if ready and not already randomized."""
+    """Randomize a patient group if ready and not already randomized.
+
+    Note: may be called by the model or its proxy.
+    """
     if not raw and instance and instance._meta.label_lower.split(".")[1] == "patientgroup":
         if (
             not instance.randomized
             and instance.randomize_now == YES
             and instance.confirm_randomize_now == "RANDOMIZE"
             and instance.status == COMPLETE
         ):
             if not re.match(UUID_PATTERN, str(instance.group_identifier)):
                 raise RandomizationError(
                     "Failed to randomize group. Group identifier is not a uuid. "
                     f"Has this group already been randomized? Got {instance.group_identifier}."
                 )
-            randomize_group(instance)
+
+            rando = RandomizeGroup(instance)
+            _, _, _, group_identifier = rando.randomize_group()
+
             rando_obj = get_object_for_subject(
-                instance.group_identifier, "default", identifier_fld="group_identifier"
+                group_identifier, "default", identifier_fld="group_identifier"
             )
             randomization_datetime = rando_obj.allocated_datetime
             for patient in instance.patients.all():
                 rs_obj = RegisteredSubject.objects.get(
                     subject_identifier=patient.subject_identifier
                 )
                 rs_obj.randomization_datetime = randomization_datetime
@@ -47,7 +55,18 @@
                     update_fields=[
                         "randomization_datetime",
                         "sid",
                         "registration_status",
                         "randomization_list_model",
                     ]
                 )
+                if rando_obj.assignment in [COMM_INTERVENTION, CLINIC_CONTROL]:
+                    model_name = (
+                        "intecomm_prn.onschedulecomm"
+                        if rando_obj.assignment == COMM_INTERVENTION
+                        else "intecomm_prn.onscheduleinte"
+                    )
+                    _, schedule = site_visit_schedules.get_by_onschedule_model(model_name)
+                    schedule.put_on_schedule(
+                        subject_identifier=patient.subject_identifier,
+                        onschedule_datetime=randomization_datetime,
+                    )
```

### Comparing `intecomm-rando-0.1.6/intecomm_rando/randomize_group.py` & `intecomm-rando-0.1.7/intecomm_rando/randomize_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from datetime import datetime
+from typing import TYPE_CHECKING, Tuple
 
 from django.apps import apps as django_apps
 from edc_constants.constants import COMPLETE, YES
 from edc_randomization.constants import RANDOMIZED
 from edc_randomization.site_randomizers import site_randomizers
 from edc_randomization.utils import get_object_for_subject
 from edc_registration.models import RegisteredSubject
@@ -18,27 +19,22 @@
 if TYPE_CHECKING:
     from .models import RandomizationList
 
 if TYPE_CHECKING:
     from intecomm_screening.models import PatientGroup, PatientLog
 
 
-def randomize_group(instance: PatientGroup) -> None:
-    rando = RandomizeGroup(instance)
-    rando.randomize_group()
-
-
 class RandomizeGroup:
     min_group_size = 14
     subject_consent_model = "intecomm_consent.subjectconsent"
 
     def __init__(self, instance: PatientGroup):
         self.instance = instance
 
-    def randomize_group(self):
+    def randomize_group(self) -> Tuple[bool, datetime, str, str]:
         if self.instance.randomized:
             raise GroupAlreadyRandomized(f"Group is already randomized. Got {self.instance}.")
         if (
             self.instance.randomize_now != YES
             or self.instance.confirm_randomize_now != "RANDOMIZE"
         ):
             raise GroupRandomizationError(
@@ -100,22 +96,22 @@
         for patient in self.instance.patients.all():
             self.update_patient_log(patient)
             self.update_subject_consent(patient)
             self.update_registered_subject(patient)
 
     def update_patient_log(self, patient_log: PatientLog):
         patient_log.group_identifier = self.instance.group_identifier
-        patient_log.save()
+        patient_log.save(update_fields=["group_identifier"])
 
     def update_subject_consent(self, patient_log: PatientLog):
         subject_consent = self.subject_consent_model_cls.objects.get(
             subject_identifier=patient_log.subject_identifier
         )
         subject_consent.group_identifier = self.instance.group_identifier
-        subject_consent.save()
+        subject_consent.save(update_fields=["group_identifier"])
 
     def update_registered_subject(self, patient_log: PatientLog):
         randomization_datetime = self.randomization_list_obj.allocated_datetime
         rs_obj = RegisteredSubject.objects.get(
             subject_identifier=patient_log.subject_identifier
         )
         rs_obj.randomization_datetime = randomization_datetime
```

### Comparing `intecomm-rando-0.1.6/intecomm_rando/randomizers.py` & `intecomm-rando-0.1.7/intecomm_rando/randomizers.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-local-private.pem` & `intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/tests/etc/user-rsa-restricted-private.pem` & `intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando/tests/tests/test_rando_group.py` & `intecomm-rando-0.1.7/intecomm_rando/tests/tests/test_rando_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/intecomm_rando.egg-info/PKG-INFO` & `intecomm-rando-0.1.7/intecomm_rando.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.6
+Version: 0.1.7
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.6/intecomm_rando.egg-info/SOURCES.txt` & `intecomm-rando-0.1.7/intecomm_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/pyproject.toml` & `intecomm-rando-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/runtests.py` & `intecomm-rando-0.1.7/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.6/setup.cfg` & `intecomm-rando-0.1.7/setup.cfg`

 * *Files identical despite different names*

