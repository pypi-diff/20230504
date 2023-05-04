# Comparing `tmp/celery-director-0.8.0.tar.gz` & `tmp/celery-director-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-director-0.8.0.tar", last modified: Wed Feb 22 10:11:28 2023, max compression
+gzip compressed data, was "celery-director-0.9.0.tar", last modified: Thu May  4 07:53:07 2023, max compression
```

## Comparing `celery-director-0.8.0.tar` & `celery-director-0.9.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.902953 celery-director-0.8.0/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      463 2022-03-10 17:20:52.000000 celery-director-0.8.0/AUTHORS
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2661 2022-03-10 17:20:52.000000 celery-director-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 ncrocfer   (501) staff       (20)      953 2022-05-04 14:56:56.000000 celery-director-0.8.0/CONTRIBUTORS
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1518 2022-03-10 17:20:52.000000 celery-director-0.8.0/LICENSE
--rw-r--r--   0 ncrocfer   (501) staff       (20)      193 2022-03-10 17:20:52.000000 celery-director-0.8.0/MANIFEST.in
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4365 2023-02-22 10:11:28.901788 celery-director-0.8.0/PKG-INFO
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3438 2022-07-25 08:37:45.000000 celery-director-0.8.0/README.md
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.707232 celery-director-0.8.0/celery_director.egg-info/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4365 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/PKG-INFO
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2028 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/SOURCES.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)        1 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/dependency_links.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       46 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/entry_points.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)      521 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/requires.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       15 2023-02-22 10:11:28.000000 celery-director-0.8.0/celery_director.egg-info/top_level.txt
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.747283 celery-director-0.8.0/director/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        6 2023-02-22 09:58:34.000000 celery-director-0.8.0/director/VERSION
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4818 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      120 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/_auto.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.751289 celery-director-0.8.0/director/api/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      425 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/api/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4454 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/api/workflows.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1034 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/auth.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4913 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/builder.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      652 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/cli.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.770314 celery-director-0.8.0/director/commands/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/commands/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3833 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/commands/assets.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1618 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/commands/celery.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      337 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/commands/db.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3380 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/commands/init.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1479 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/commands/user.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      769 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/commands/webserver.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5361 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/commands/workflows.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      278 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/context.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      223 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/exceptions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     7031 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/extensions.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.779640 celery-director-0.8.0/director/migrations/
--rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/migrations/README
--rw-r--r--   0 ncrocfer   (501) staff       (20)      770 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/migrations/alembic.ini
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2902 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/env.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      494 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/migrations/script.py.mako
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.800842 celery-director-0.8.0/director/migrations/versions/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      453 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/05cf96d6fcae_add_task_result.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      530 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/063ff371f2da_add_index_on_workflow_id_in_task_table.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2563 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/2ac615d6850b_force_varchar_255.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2512 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/30d6f6636351_initial_migration.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1085 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/3f8466b16023_add_users_table.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2070 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/46e4acde004e_add_cascade_in_task_model.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      456 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/9817ccf13cb5_add_is_hook_on_task.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      490 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/migrations/versions/9d563aaa548b_add_workflow_comment.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.836990 celery-director-0.8.0/director/models/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1137 2022-03-11 10:49:52.000000 celery-director-0.8.0/director/models/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1280 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/models/tasks.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      975 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/models/users.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      431 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/models/utils.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1188 2023-02-20 10:14:10.000000 celery-director-0.8.0/director/models/workflows.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3490 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/settings.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.844909 celery-director-0.8.0/director/static/
--rw-r--r--   0 ncrocfer   (501) staff       (20)    11779 2023-02-20 10:14:10.000000 celery-director-0.8.0/director/static/script.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1602 2022-11-29 15:31:29.000000 celery-director-0.8.0/director/static/style.css
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.872935 celery-director-0.8.0/director/tasks/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/tasks/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1780 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/tasks/base.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1797 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/tasks/periodic.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2407 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/tasks/workflows.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.876436 celery-director-0.8.0/director/templates/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      240 2022-03-10 17:20:52.000000 celery-director-0.8.0/director/templates/error.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)    30247 2023-02-20 10:14:10.000000 celery-director-0.8.0/director/templates/index.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2223 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/utils.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.878940 celery-director-0.8.0/director/views/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      600 2023-02-20 17:18:42.000000 celery-director-0.8.0/director/views/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      469 2023-02-20 17:07:10.000000 celery-director-0.8.0/requirements.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2023-02-22 10:11:28.903530 celery-director-0.8.0/setup.cfg
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1831 2023-02-21 09:29:46.000000 celery-director-0.8.0/setup.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-02-22 10:11:28.898736 celery-director-0.8.0/tests/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.8.0/tests/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2613 2023-01-27 16:12:49.000000 celery-director-0.8.0/tests/conftest.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)    13939 2023-02-20 10:14:10.000000 celery-director-0.8.0/tests/test_api.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      810 2022-03-10 17:20:52.000000 celery-director-0.8.0/tests/test_auth.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5793 2023-01-27 16:12:49.000000 celery-director-0.8.0/tests/test_builder.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      824 2022-03-10 17:20:52.000000 celery-director-0.8.0/tests/test_sentry.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      895 2022-03-10 17:20:52.000000 celery-director-0.8.0/tests/test_users.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      979 2022-04-19 15:49:31.000000 celery-director-0.8.0/tests/test_views.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)    18738 2023-02-21 09:29:46.000000 celery-director-0.8.0/tests/test_workflows.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.389770 celery-director-0.9.0/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      463 2022-03-10 17:20:52.000000 celery-director-0.9.0/AUTHORS
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2661 2022-03-10 17:20:52.000000 celery-director-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      953 2022-05-04 14:56:56.000000 celery-director-0.9.0/CONTRIBUTORS
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1518 2022-03-10 17:20:52.000000 celery-director-0.9.0/LICENSE
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      193 2022-03-10 17:20:52.000000 celery-director-0.9.0/MANIFEST.in
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4315 2023-05-04 07:53:07.388657 celery-director-0.9.0/PKG-INFO
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3438 2023-05-04 07:49:02.000000 celery-director-0.9.0/README.md
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.199479 celery-director-0.9.0/celery_director.egg-info/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4315 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/PKG-INFO
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2028 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/SOURCES.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        1 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/dependency_links.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       46 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/entry_points.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      538 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/requires.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       15 2023-05-04 07:53:07.000000 celery-director-0.9.0/celery_director.egg-info/top_level.txt
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.247043 celery-director-0.9.0/director/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        6 2023-05-04 07:49:02.000000 celery-director-0.9.0/director/VERSION
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4818 2023-05-02 10:20:22.000000 celery-director-0.9.0/director/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      120 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/_auto.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.250195 celery-director-0.9.0/director/api/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      425 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/api/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4454 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/api/workflows.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1034 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/auth.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4913 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/builder.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      652 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/cli.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.263960 celery-director-0.9.0/director/commands/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/commands/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3833 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/commands/assets.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1618 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/commands/celery.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      337 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/commands/db.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3380 2023-05-02 10:20:22.000000 celery-director-0.9.0/director/commands/init.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1479 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/commands/user.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      769 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/commands/webserver.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5361 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/commands/workflows.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      278 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/context.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      223 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/exceptions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     7031 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/extensions.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.281179 celery-director-0.9.0/director/migrations/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/migrations/README
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      770 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/migrations/alembic.ini
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2902 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/env.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      494 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/migrations/script.py.mako
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.298909 celery-director-0.9.0/director/migrations/versions/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      453 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/05cf96d6fcae_add_task_result.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      530 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/063ff371f2da_add_index_on_workflow_id_in_task_table.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2563 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/2ac615d6850b_force_varchar_255.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2512 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/30d6f6636351_initial_migration.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1085 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/3f8466b16023_add_users_table.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2070 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/46e4acde004e_add_cascade_in_task_model.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      456 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/9817ccf13cb5_add_is_hook_on_task.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      490 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/migrations/versions/9d563aaa548b_add_workflow_comment.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.319075 celery-director-0.9.0/director/models/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1137 2022-03-11 10:49:52.000000 celery-director-0.9.0/director/models/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1280 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/models/tasks.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      975 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/models/users.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      431 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/models/utils.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1188 2023-02-20 10:14:10.000000 celery-director-0.9.0/director/models/workflows.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3490 2023-05-02 10:20:22.000000 celery-director-0.9.0/director/settings.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.327292 celery-director-0.9.0/director/static/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    11779 2023-02-20 10:14:10.000000 celery-director-0.9.0/director/static/script.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1602 2022-11-29 15:31:29.000000 celery-director-0.9.0/director/static/style.css
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.356070 celery-director-0.9.0/director/tasks/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/tasks/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1780 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/tasks/base.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1797 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/tasks/periodic.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2407 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/tasks/workflows.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.360034 celery-director-0.9.0/director/templates/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      240 2022-03-10 17:20:52.000000 celery-director-0.9.0/director/templates/error.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    30247 2023-05-02 10:20:22.000000 celery-director-0.9.0/director/templates/index.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2223 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/utils.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.363102 celery-director-0.9.0/director/views/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      600 2023-02-20 17:18:42.000000 celery-director-0.9.0/director/views/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      486 2023-05-04 07:49:02.000000 celery-director-0.9.0/requirements.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2023-05-04 07:53:07.390022 celery-director-0.9.0/setup.cfg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1782 2023-05-04 07:49:02.000000 celery-director-0.9.0/setup.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-04 07:53:07.386306 celery-director-0.9.0/tests/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-03-10 17:20:52.000000 celery-director-0.9.0/tests/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2613 2023-01-27 16:12:49.000000 celery-director-0.9.0/tests/conftest.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    13939 2023-02-20 10:14:10.000000 celery-director-0.9.0/tests/test_api.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      810 2022-03-10 17:20:52.000000 celery-director-0.9.0/tests/test_auth.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5793 2023-01-27 16:12:49.000000 celery-director-0.9.0/tests/test_builder.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      824 2022-03-10 17:20:52.000000 celery-director-0.9.0/tests/test_sentry.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      895 2022-03-10 17:20:52.000000 celery-director-0.9.0/tests/test_users.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      979 2022-04-19 15:49:31.000000 celery-director-0.9.0/tests/test_views.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    18738 2023-02-21 09:29:46.000000 celery-director-0.9.0/tests/test_workflows.py
```

### Comparing `celery-director-0.8.0/CONTRIBUTING.md` & `celery-director-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/CONTRIBUTORS` & `celery-director-0.9.0/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/LICENSE` & `celery-director-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/PKG-INFO` & `celery-director-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: celery-director
-Version: 0.8.0
+Version: 0.9.0
 Summary: Celery Director
 Home-page: https://github.com/ovh/celery-director
 Author: OVHcloud
 Author-email: opensource@ovhcloud.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ci
 Provides-Extra: doc
 License-File: LICENSE
 License-File: AUTHORS
 
 <p align="center">
   <img alt="Celery Director logo" src="https://raw.githubusercontent.com/ovh/celery-director/master/logo.png">
 </p>
 <p align="center">
   <a href="https://github.com/ovh/celery-director/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/ovh/celery-director/workflows/Tests/badge.svg"></a>
-  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7%2B-blue.svg"></a>
+  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.8%2B-blue.svg"></a>
   <a href="https://github.com/ovh/depc/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg"></a>
   <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 <p align="center">
   <a href="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"><img alt="Celery Director" src="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"></a>
 </p>
```

### Comparing `celery-director-0.8.0/README.md` & `celery-director-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
   <img alt="Celery Director logo" src="https://raw.githubusercontent.com/ovh/celery-director/master/logo.png">
 </p>
 <p align="center">
   <a href="https://github.com/ovh/celery-director/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/ovh/celery-director/workflows/Tests/badge.svg"></a>
-  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7%2B-blue.svg"></a>
+  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.8%2B-blue.svg"></a>
   <a href="https://github.com/ovh/depc/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg"></a>
   <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 <p align="center">
   <a href="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"><img alt="Celery Director" src="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"></a>
 </p>
```

### Comparing `celery-director-0.8.0/celery_director.egg-info/PKG-INFO` & `celery-director-0.9.0/celery_director.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: celery-director
-Version: 0.8.0
+Version: 0.9.0
 Summary: Celery Director
 Home-page: https://github.com/ovh/celery-director
 Author: OVHcloud
 Author-email: opensource@ovhcloud.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ci
 Provides-Extra: doc
 License-File: LICENSE
 License-File: AUTHORS
 
 <p align="center">
   <img alt="Celery Director logo" src="https://raw.githubusercontent.com/ovh/celery-director/master/logo.png">
 </p>
 <p align="center">
   <a href="https://github.com/ovh/celery-director/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/ovh/celery-director/workflows/Tests/badge.svg"></a>
-  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7%2B-blue.svg"></a>
+  <a href="https://www.python.org/"><img alt="Python versions" src="https://img.shields.io/badge/python-3.8%2B-blue.svg"></a>
   <a href="https://github.com/ovh/depc/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg"></a>
   <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 <p align="center">
   <a href="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"><img alt="Celery Director" src="https://raw.githubusercontent.com/ovh/celery-director/master/director.gif"></a>
 </p>
```

### Comparing `celery-director-0.8.0/celery_director.egg-info/SOURCES.txt` & `celery-director-0.9.0/celery_director.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/__init__.py` & `celery-director-0.9.0/director/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/api/workflows.py` & `celery-director-0.9.0/director/api/workflows.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/auth.py` & `celery-director-0.9.0/director/auth.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/builder.py` & `celery-director-0.9.0/director/builder.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/cli.py` & `celery-director-0.9.0/director/cli.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/assets.py` & `celery-director-0.9.0/director/commands/assets.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/celery.py` & `celery-director-0.9.0/director/commands/celery.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/init.py` & `celery-director-0.9.0/director/commands/init.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/user.py` & `celery-director-0.9.0/director/commands/user.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/webserver.py` & `celery-director-0.9.0/director/commands/webserver.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/commands/workflows.py` & `celery-director-0.9.0/director/commands/workflows.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/extensions.py` & `celery-director-0.9.0/director/extensions.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/alembic.ini` & `celery-director-0.9.0/director/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/env.py` & `celery-director-0.9.0/director/migrations/env.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/versions/063ff371f2da_add_index_on_workflow_id_in_task_table.py` & `celery-director-0.9.0/director/migrations/versions/063ff371f2da_add_index_on_workflow_id_in_task_table.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/versions/2ac615d6850b_force_varchar_255.py` & `celery-director-0.9.0/director/migrations/versions/2ac615d6850b_force_varchar_255.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/versions/30d6f6636351_initial_migration.py` & `celery-director-0.9.0/director/migrations/versions/30d6f6636351_initial_migration.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/versions/3f8466b16023_add_users_table.py` & `celery-director-0.9.0/director/migrations/versions/3f8466b16023_add_users_table.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/migrations/versions/46e4acde004e_add_cascade_in_task_model.py` & `celery-director-0.9.0/director/migrations/versions/46e4acde004e_add_cascade_in_task_model.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/models/__init__.py` & `celery-director-0.9.0/director/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/models/tasks.py` & `celery-director-0.9.0/director/models/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/models/users.py` & `celery-director-0.9.0/director/models/users.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/models/workflows.py` & `celery-director-0.9.0/director/models/workflows.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/settings.py` & `celery-director-0.9.0/director/settings.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/static/script.js` & `celery-director-0.9.0/director/static/script.js`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/static/style.css` & `celery-director-0.9.0/director/static/style.css`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/tasks/base.py` & `celery-director-0.9.0/director/tasks/base.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/tasks/periodic.py` & `celery-director-0.9.0/director/tasks/periodic.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/tasks/workflows.py` & `celery-director-0.9.0/director/tasks/workflows.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/templates/index.html` & `celery-director-0.9.0/director/templates/index.html`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/utils.py` & `celery-director-0.9.0/director/utils.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/director/views/__init__.py` & `celery-director-0.9.0/director/views/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/setup.py` & `celery-director-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: System :: Monitoring",
     ],
-    python_requires="~=3.7",
+    python_requires="~=3.8",
 )
```

### Comparing `celery-director-0.8.0/tests/conftest.py` & `celery-director-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_api.py` & `celery-director-0.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_auth.py` & `celery-director-0.9.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_builder.py` & `celery-director-0.9.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_sentry.py` & `celery-director-0.9.0/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_users.py` & `celery-director-0.9.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_views.py` & `celery-director-0.9.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `celery-director-0.8.0/tests/test_workflows.py` & `celery-director-0.9.0/tests/test_workflows.py`

 * *Files identical despite different names*

