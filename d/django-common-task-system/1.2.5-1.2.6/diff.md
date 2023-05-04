# Comparing `tmp/django-common-task-system-1.2.5.tar.gz` & `tmp/django-common-task-system-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-common-task-system-1.2.5.tar", last modified: Thu Apr 27 13:32:57 2023, max compression
+gzip compressed data, was "django-common-task-system-1.2.6.tar", last modified: Thu May  4 07:18:00 2023, max compression
```

## Comparing `django-common-task-system-1.2.5.tar` & `django-common-task-system-1.2.6.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/
--rw-r--r--   0 cone       (501) staff       (20)     1064 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/LICENSE
--rw-r--r--   0 cone       (501) staff       (20)      245 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/MANIFEST.in
--rw-r--r--   0 cone       (501) staff       (20)      289 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/PKG-INFO
--rw-r--r--   0 cone       (501) staff       (20)       24 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/README.md
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/
--rw-r--r--   0 cone       (501) staff       (20)     2923 2023-04-17 14:25:56.000000 django-common-task-system-1.2.5/django_common_task_system/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)    11056 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/admin.py
--rw-r--r--   0 cone       (501) staff       (20)      156 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/apps.py
--rw-r--r--   0 cone       (501) staff       (20)     1542 2023-04-17 14:25:56.000000 django-common-task-system-1.2.5/django_common_task_system/choices.py
--rw-r--r--   0 cone       (501) staff       (20)     1028 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/fields.py
--rw-r--r--   0 cone       (501) staff       (20)    15569 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/forms.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/
--rw-r--r--   0 cone       (501) staff       (20)     7699 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0001_initial.py
--rw-r--r--   0 cone       (501) staff       (20)      474 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-r--r--   0 cone       (501) staff       (20)      632 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-r--r--   0 cone       (501) staff       (20)     3225 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-r--r--   0 cone       (501) staff       (20)      477 2023-04-14 14:08:35.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-r--r--   0 cone       (501) staff       (20)     1527 2023-04-17 14:25:56.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0006_consumerpermission.py
--rw-r--r--   0 cone       (501) staff       (20)     1241 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/migrations/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)     2607 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/mixin.py
--rw-r--r--   0 cone       (501) staff       (20)    36031 2023-04-27 13:07:06.000000 django-common-task-system-1.2.5/django_common_task_system/models.py
--rw-r--r--   0 cone       (501) staff       (20)      973 2023-04-17 14:25:56.000000 django-common-task-system-1.2.5/django_common_task_system/permissions.py
--rw-r--r--   0 cone       (501) staff       (20)     2197 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/serializers.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/static/
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/css/
--rw-r--r--   0 cone       (501) staff       (20)     2162 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/css/calendar.css
--rw-r--r--   0 cone       (501) staff       (20)      262 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/js/
--rw-r--r--   0 cone       (501) staff       (20)    21674 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/js/calendar.js
--rw-r--r--   0 cone       (501) staff       (20)     2788 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-04-02 02:22:50.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)     5013 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/admin.py
--rw-r--r--   0 cone       (501) staff       (20)      243 2023-04-02 02:22:50.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/apps.py
--rw-r--r--   0 cone       (501) staff       (20)      619 2023-04-14 12:49:24.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/choices.py
--rw-r--r--   0 cone       (501) staff       (20)     4025 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/forms.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/
--rw-r--r--   0 cone       (501) staff       (20)    10451 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0001_initial.py
--rw-r--r--   0 cone       (501) staff       (20)      653 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-r--r--   0 cone       (501) staff       (20)     2166 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-r--r--   0 cone       (501) staff       (20)      978 2023-04-14 14:08:15.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-r--r--   0 cone       (501) staff       (20)      449 2023-04-14 14:08:35.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-r--r--   0 cone       (501) staff       (20)     1507 2023-04-17 14:25:56.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-r--r--   0 cone       (501) staff       (20)     1032 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-04-05 02:14:25.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)    14522 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/models.py
--rw-r--r--   0 cone       (501) staff       (20)     1092 2023-04-14 14:49:24.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/process.py
--rw-r--r--   0 cone       (501) staff       (20)     2156 2023-04-14 12:49:24.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/queue.py
--rw-r--r--   0 cone       (501) staff       (20)     1627 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/serializers.py
--rw-r--r--   0 cone       (501) staff       (20)       60 2023-04-02 02:22:50.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/tests.py
--rw-r--r--   0 cone       (501) staff       (20)      832 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/urls.py
--rw-r--r--   0 cone       (501) staff       (20)     5369 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task/views.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-04-05 02:14:25.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)     1632 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/main.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-04-05 02:14:25.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)     3005 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-r--r--   0 cone       (501) staff       (20)      421 2023-04-06 13:07:27.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)      850 2023-04-16 10:00:18.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-r--r--   0 cone       (501) staff       (20)     3621 2023-04-27 13:07:06.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-r--r--   0 cone       (501) staff       (20)      809 2023-04-16 10:18:51.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-r--r--   0 cone       (501) staff       (20)     1076 2023-04-14 12:49:24.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-r--r--   0 cone       (501) staff       (20)      363 2023-04-14 12:49:24.000000 django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/templates/
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/templates/admin/
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/templates/admin/system_schedule/
--rw-r--r--   0 cone       (501) staff       (20)     8242 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/
--rw-r--r--   0 cone       (501) staff       (20)      359 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-r--r--   0 cone       (501) staff       (20)      575 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-r--r--   0 cone       (501) staff       (20)     3155 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-r--r--   0 cone       (501) staff       (20)     1358 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-r--r--   0 cone       (501) staff       (20)      254 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/period.html
--rw-r--r--   0 cone       (501) staff       (20)      526 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-r--r--   0 cone       (501) staff       (20)       60 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/tests.py
--rw-r--r--   0 cone       (501) staff       (20)     1039 2023-04-23 14:06:59.000000 django-common-task-system-1.2.5/django_common_task_system/urls.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system/utils/
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/utils/__init__.py
--rw-r--r--   0 cone       (501) staff       (20)      871 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/utils/algorithm.py
--rw-r--r--   0 cone       (501) staff       (20)      233 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/utils/cron_utils.py
--rw-r--r--   0 cone       (501) staff       (20)      506 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/utils/foreign_key.py
--rw-r--r--   0 cone       (501) staff       (20)     1955 2023-03-13 14:05:58.000000 django-common-task-system-1.2.5/django_common_task_system/utils/schedule_time.py
--rw-r--r--   0 cone       (501) staff       (20)    11713 2023-04-27 13:26:57.000000 django-common-task-system-1.2.5/django_common_task_system/views.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/
--rw-r--r--   0 cone       (501) staff       (20)      289 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/PKG-INFO
--rw-r--r--   0 cone       (501) staff       (20)     4423 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/SOURCES.txt
--rw-r--r--   0 cone       (501) staff       (20)        1 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/dependency_links.txt
--rw-r--r--   0 cone       (501) staff       (20)      122 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/requires.txt
--rw-r--r--   0 cone       (501) staff       (20)       32 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/django_common_task_system.egg-info/top_level.txt
--rw-r--r--   0 cone       (501) staff       (20)       38 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/setup.cfg
--rw-r--r--   0 cone       (501) staff       (20)      591 2023-04-27 13:31:51.000000 django-common-task-system-1.2.5/setup.py
-drwxr-xr-x   0 cone       (501) staff       (20)        0 2023-04-27 13:32:57.000000 django-common-task-system-1.2.5/tests/
--rw-r--r--   0 cone       (501) staff       (20)        0 2023-04-02 02:22:50.000000 django-common-task-system-1.2.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.129160 django-common-task-system-1.2.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-05-04 07:18:00.129160 django-common-task-system-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.077477 django-common-task-system-1.2.6/django_common_task_system/
+-rw-rw-rw-   0        0        0     3015 2023-05-04 05:28:57.000000 django-common-task-system-1.2.6/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.6/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.6/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.6/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.6/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15985 2023-04-26 08:54:39.000000 django-common-task-system-1.2.6/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.095472 django-common-task-system-1.2.6/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.6/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    36866 2023-04-26 08:13:50.000000 django-common-task-system-1.2.6/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.6/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2425 2023-05-04 05:26:09.000000 django-common-task-system-1.2.6/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.063059 django-common-task-system-1.2.6/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.064067 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.096473 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.098482 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+-rw-rw-rw-   0        0        0     1145 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_type_admin.js
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.106482 django-common-task-system-1.2.6/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5503 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4728 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.113473 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.115148 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.117155 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.121157 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3708 2023-04-27 05:37:12.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.066058 django-common-task-system-1.2.6/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.065060 django-common-task-system-1.2.6/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.121157 django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.125164 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.6/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.128157 django-common-task-system-1.2.6/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.6/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.6/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.6/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.6/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.6/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    12089 2023-05-04 07:11:55.000000 django-common-task-system-1.2.6/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.089480 django-common-task-system-1.2.6/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4497 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:18:00.130159 django-common-task-system-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-05-04 07:17:46.000000 django-common-task-system-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.128157 django-common-task-system-1.2.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.6/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-common-task-system-1.2.5/LICENSE` & `django-common-task-system-1.2.6/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 cone387
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 cone387
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/__init__.py` & `django-common-task-system-1.2.6/django_common_task_system/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from django.apps import apps as django_apps
-from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
-from django.core.management.commands import runserver
-from django.utils.module_loading import import_string
-
-
-class Command(runserver.Command):
-
-    def run(self, **options):
-        import os
-        os.environ['DJANGO_SERVER_ADDRESS'] = "%(protocol)s://%(addr)s:%(port)s" % {
-            'protocol': self.protocol,
-            'addr': self.addr,
-            'port': self.port
-        }
-        super().run(**options)
-
-
-runserver.Command = Command
-
-
-if not hasattr(settings, 'TASK_MODEL'):
-    setattr(settings, 'TASK_MODEL', 'django_common_task_system.Task')
-
-if not hasattr(settings, 'TASK_SCHEDULE_MODEL'):
-    setattr(settings, 'TASK_SCHEDULE_MODEL', 'django_common_task_system.TaskSchedule')
-
-if not hasattr(settings, 'TASK_SCHEDULE_LOG_MODEL'):
-    setattr(settings, 'TASK_SCHEDULE_LOG_MODEL', 'django_common_task_system.TaskScheduleLog')
-
-if not hasattr(settings, 'TASK_SCHEDULE_SERIALIZER'):
-    setattr(settings, 'TASK_SCHEDULE_SERIALIZER', 'django_common_task_system.serializers.TaskScheduleSerializer')
-
-
-def get_task_model():
-    """
-    Return the User model that is active in this project.
-    """
-    try:
-        return django_apps.get_model(settings.TASK_MODEL, require_ready=False)
-    except ValueError:
-        raise ImproperlyConfigured(
-            "TASK_MODEL must be of the form 'app_label.model_name'"
-        )
-    except LookupError:
-        raise ImproperlyConfigured(
-            "TASK_MODEL refers to model '%s' that has not been installed"
-            % settings.TASK_MODEL
-        )
-
-
-def get_task_schedule_model():
-    """
-    Return the User model that is active in this project.
-    """
-    try:
-        return django_apps.get_model(settings.TASK_SCHEDULE_MODEL, require_ready=False)
-    except ValueError:
-        raise ImproperlyConfigured(
-            "TASK_SCHEDULE_MODEL must be of the form 'app_label.model_name'"
-        )
-    except LookupError:
-        raise ImproperlyConfigured(
-            "TASK_SCHEDULE_MODEL refers to model '%s' that has not been installed"
-            % settings.TASK_SCHEDULE_MODEL
-        )
-
-
-def get_schedule_log_model():
-    """
-    Return the User model that is active in this project.
-    """
-    try:
-        return django_apps.get_model(settings.TASK_SCHEDULE_LOG_MODEL, require_ready=False)
-    except ValueError:
-        raise ImproperlyConfigured(
-            "TASK_SCHEDULE_LOG_MODEL must be of the form 'app_label.model_name'"
-        )
-    except LookupError:
-        raise ImproperlyConfigured(
-            "TASK_SCHEDULE_LOG_MODEL refers to model '%s' that has not been installed"
-            % settings.SCHEDULE_LOG_MODEL
-        )
-
-
-def get_task_schedule_serializer():
-    """
-    Return the User model that is active in this project.
-    """
-    return import_string(settings.TASK_SCHEDULE_SERIALIZER)
+from django.apps import apps as django_apps
+from django.conf import settings
+from django.core.exceptions import ImproperlyConfigured
+from django.core.management.commands import runserver
+from django.utils.module_loading import import_string
+
+
+class Command(runserver.Command):
+
+    def run(self, **options):
+        import os
+        os.environ['DJANGO_SERVER_ADDRESS'] = "%(protocol)s://%(addr)s:%(port)s" % {
+            'protocol': self.protocol,
+            'addr': self.addr,
+            'port': self.port
+        }
+        super().run(**options)
+
+
+runserver.Command = Command
+
+
+if not hasattr(settings, 'TASK_MODEL'):
+    setattr(settings, 'TASK_MODEL', 'django_common_task_system.Task')
+
+if not hasattr(settings, 'TASK_SCHEDULE_MODEL'):
+    setattr(settings, 'TASK_SCHEDULE_MODEL', 'django_common_task_system.TaskSchedule')
+
+if not hasattr(settings, 'TASK_SCHEDULE_LOG_MODEL'):
+    setattr(settings, 'TASK_SCHEDULE_LOG_MODEL', 'django_common_task_system.TaskScheduleLog')
+
+if not hasattr(settings, 'TASK_SCHEDULE_SERIALIZER'):
+    setattr(settings, 'TASK_SCHEDULE_SERIALIZER', 'django_common_task_system.serializers.QueueScheduleSerializer')
+
+
+def get_task_model():
+    """
+    Return the User model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.TASK_MODEL, require_ready=False)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "TASK_MODEL must be of the form 'app_label.model_name'"
+        )
+    except LookupError:
+        raise ImproperlyConfigured(
+            "TASK_MODEL refers to model '%s' that has not been installed"
+            % settings.TASK_MODEL
+        )
+
+
+def get_task_schedule_model():
+    """
+    Return the User model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.TASK_SCHEDULE_MODEL, require_ready=False)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_MODEL must be of the form 'app_label.model_name'"
+        )
+    except LookupError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_MODEL refers to model '%s' that has not been installed"
+            % settings.TASK_SCHEDULE_MODEL
+        )
+
+
+def get_schedule_log_model():
+    """
+    Return the User model that is active in this project.
+    """
+    try:
+        return django_apps.get_model(settings.TASK_SCHEDULE_LOG_MODEL, require_ready=False)
+    except ValueError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_LOG_MODEL must be of the form 'app_label.model_name'"
+        )
+    except LookupError:
+        raise ImproperlyConfigured(
+            "TASK_SCHEDULE_LOG_MODEL refers to model '%s' that has not been installed"
+            % settings.SCHEDULE_LOG_MODEL
+        )
+
+
+def get_task_schedule_serializer():
+    """
+    Return the User model that is active in this project.
+    """
+    return import_string(settings.TASK_SCHEDULE_SERIALIZER)
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/choices.py` & `django-common-task-system-1.2.6/django_common_task_system/choices.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from django.db.models import TextChoices
-import queue
-
-
-class TaskStatus(TextChoices):
-    ENABLE = 'E', '启用'
-    DISABLE = 'D', '禁用'
-
-
-class TaskScheduleStatus(TextChoices):
-    OPENING = 'O', '开启'
-    CLOSED = 'C', '关闭'
-    DONE = 'D', '已完成'
-    TEST = 'T', '测试'
-    ERROR = 'E', '调度错误'
-
-
-class TaskScheduleType(TextChoices):
-    CRONTAB = 'C', 'Crontab'
-    ONCE = 'O', '一次性'
-    CONTINUOUS = 'S', '连续性'
-    TIMINGS = 'T', '指定时间'
-
-
-class ScheduleTimingType(TextChoices):
-    DAY = 'DAY', '按天'
-    WEEKDAY = 'WEEKDAY', '按周'
-    MONTHDAY = 'MONTHDAY', '按月'
-    YEAR = 'YEAR', "按年"
-    DATETIME = 'DATETIME', '自选日期'
-
-
-class TaskCallbackStatus(TextChoices):
-    ENABLE = 'E', '启用'
-    DISABLE = 'D', '禁用'
-
-
-class TaskCallbackEvent(TextChoices):
-    SUCCEED = 'S', '成功'
-    FAILED = 'F', '失败'
-    DONE = 'D', '完成'
-
-
-class ScheduleQueueModule(TextChoices):
-    QUEUE = "%s.%s" % (queue.Queue.__module__, queue.Queue.__name__), '普通队列'
-    STACK = "%s.%s" % (queue.LifoQueue.__module__, queue.LifoQueue.__name__), '后进先出队列'
-    PRIORITY_QUEUE = "%s.%s" % (queue.PriorityQueue.__module__, queue.PriorityQueue.__name__), '优先级队列'
-    SIMPLE_QUEUE = "%s.%s" % (queue.SimpleQueue.__module__, queue.SimpleQueue.__name__), '简单队列'
-    REDIS_LIST_QUEUE = "django_common_task_system.system_task.queue.RedisListQueue", 'Redis List队列'
-
-
-class ConsumerPermissionType(TextChoices):
-    IP_WHITE_LIST = 'I', 'IP白名单'
-
+from django.db.models import TextChoices
+import queue
+
+
+class TaskStatus(TextChoices):
+    ENABLE = 'E', '启用'
+    DISABLE = 'D', '禁用'
+
+
+class TaskScheduleStatus(TextChoices):
+    OPENING = 'O', '开启'
+    CLOSED = 'C', '关闭'
+    DONE = 'D', '已完成'
+    TEST = 'T', '测试'
+    ERROR = 'E', '调度错误'
+
+
+class TaskScheduleType(TextChoices):
+    CRONTAB = 'C', 'Crontab'
+    ONCE = 'O', '一次性'
+    CONTINUOUS = 'S', '连续性'
+    TIMINGS = 'T', '指定时间'
+
+
+class ScheduleTimingType(TextChoices):
+    DAY = 'DAY', '按天'
+    WEEKDAY = 'WEEKDAY', '按周'
+    MONTHDAY = 'MONTHDAY', '按月'
+    YEAR = 'YEAR', "按年"
+    DATETIME = 'DATETIME', '自选日期'
+
+
+class TaskCallbackStatus(TextChoices):
+    ENABLE = 'E', '启用'
+    DISABLE = 'D', '禁用'
+
+
+class TaskCallbackEvent(TextChoices):
+    SUCCEED = 'S', '成功'
+    FAILED = 'F', '失败'
+    DONE = 'D', '完成'
+
+
+class ScheduleQueueModule(TextChoices):
+    QUEUE = "%s.%s" % (queue.Queue.__module__, queue.Queue.__name__), '普通队列'
+    STACK = "%s.%s" % (queue.LifoQueue.__module__, queue.LifoQueue.__name__), '后进先出队列'
+    PRIORITY_QUEUE = "%s.%s" % (queue.PriorityQueue.__module__, queue.PriorityQueue.__name__), '优先级队列'
+    SIMPLE_QUEUE = "%s.%s" % (queue.SimpleQueue.__module__, queue.SimpleQueue.__name__), '简单队列'
+    REDIS_LIST_QUEUE = "django_common_task_system.system_task.queue.RedisListQueue", 'Redis List队列'
+
+
+class ConsumerPermissionType(TextChoices):
+    IP_WHITE_LIST = 'I', 'IP白名单'
+
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/forms.py` & `django-common-task-system-1.2.6/django_common_task_system/forms.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,416 +1,416 @@
-import inspect
-from django import forms
-from django.contrib.admin import widgets
-from django.utils.module_loading import import_string
-from .choices import TaskScheduleType, ScheduleTimingType, TaskScheduleStatus, TaskStatus
-from django_common_objects.widgets import JSONWidget
-from .utils import foreign_key
-from datetime import datetime, time as datetime_time
-from . import models
-
-
-class TaskForm(forms.ModelForm):
-
-    def __init__(self, *args, **kwargs):
-        super(TaskForm, self).__init__(*args, **kwargs)
-        task: models.Task = self.instance
-        if task.id:
-            self.fields['parent'].queryset = models.Task.objects.filter(
-                user=task.user
-            ).exclude(id__in=foreign_key.get_related_object_ids(task))
-
-
-class DateTimeRangeWidget(forms.widgets.MultiWidget):
-    template_name = 'task_schedule/datetime_range.html'
-
-    def __init__(self, attrs=None):
-        st = widgets.AdminSplitDateTime()
-        et = widgets.AdminSplitDateTime()
-        super().__init__([st, et], attrs=attrs)
-
-    def get_context(self, name, value, attrs):
-        context = super().get_context(name, value, attrs)
-        context["start_datetime"] = "开始时间:"
-        context["end_datetime"] = "结束时间:"
-        return context
-
-    def decompress(self, value):
-        if value:
-            return value
-        return [None, None]
-
-
-class PeriodWidget(widgets.AdminIntegerFieldWidget):
-    template_name = 'task_schedule/period.html'
-
-    def __init__(self, unit=ScheduleTimingType.DAY.value, attrs=None):
-        self.unit = unit
-        super().__init__(attrs=attrs)
-
-    def get_context(self, name, value, attrs):
-        context = super().get_context(name, value, attrs)
-        context["unit"] = self.unit
-        return context
-
-
-class NullableSplitDateTimeField(forms.SplitDateTimeField):
-
-    def clean(self, value):
-        if value[0] and not value[1]:
-            value[1] = '00:00:00'
-        elif not value[0] and value[1]:
-            value[0] = datetime.now().strftime('%Y-%m-%d')
-        return super(NullableSplitDateTimeField, self).clean(value)
-
-
-class MultiWeekdaySelectFiled(forms.MultipleChoiceField):
-    _choices = [
-        (1, "星期一"),
-        (2, "星期二"),
-        (3, "星期三"),
-        (4, "星期四"),
-        (5, "星期五"),
-        (6, "星期六"),
-        (7, "星期日"),
-    ]
-    widget = forms.CheckboxSelectMultiple
-
-    def __init__(self, *, choices=(), label="星期", widget=None, **kwargs):
-        super(MultiWeekdaySelectFiled, self).__init__(
-            choices=choices or self._choices,
-            label=label,
-            widget=widget or self.widget,
-            **kwargs)
-
-    def to_python(self, value):
-        if not value:
-            return value
-        elif not isinstance(value, (list, tuple)):
-            raise forms.ValidationError(
-                self.error_messages["invalid_list"], code="invalid_list"
-            )
-        return [int(val) for val in value]
-
-
-class PeriodScheduleWidget(forms.MultiWidget):
-    template_name = 'task_schedule/period_schedule.html'
-
-    def __init__(self, default_time=datetime.now, default_period=60, attrs=None):
-        ws = (
-            widgets.AdminSplitDateTime(),
-            widgets.AdminIntegerFieldWidget()
-        )
-        self.default_time = default_time() if callable(default_time) else default_time
-        self.default_period = default_period
-        super().__init__(ws)
-
-    def decompress(self, value):
-        if value:
-            return value
-        return [self.default_time, self.default_period]
-
-
-class PeriodScheduleFiled(forms.MultiValueField):
-    widget = PeriodScheduleWidget
-
-    def __init__(self, label="持续计划", **kwargs):
-        fs = (
-            forms.SplitDateTimeField(help_text="下次开始时间"),
-            forms.IntegerField(help_text="周期/每(秒)")
-        )
-        super(PeriodScheduleFiled, self).__init__(fs, label=label, **kwargs)
-
-    def to_python(self, value):
-        if not value:
-            return []
-        elif not isinstance(value, (list, tuple)):
-            raise forms.ValidationError(
-                self.error_messages["invalid_list"], code="invalid_list"
-            )
-        return [int(val) for val in value]
-
-    def compress(self, data_list):
-        return data_list
-
-
-class OnceScheduleField(forms.SplitDateTimeField):
-    widget = widgets.AdminSplitDateTime
-
-    def __init__(self, required=False, label="计划时间", **kwargs):
-        super(OnceScheduleField, self).__init__(
-            required=required,
-            label=label,
-            initial=datetime.now(), **kwargs)
-
-
-class MultiDaySelectWidget(forms.MultiWidget):
-    template_name = 'task_schedule/multi_day_select.html'
-
-    def __init__(self, attrs=None):
-        ws = (
-            forms.TextInput(attrs={'style': "width: 80%;"}),
-            widgets.AdminTimeWidget(attrs={'style': "margin-top: 5px;"})
-        )
-        super(MultiDaySelectWidget, self).__init__(ws, attrs=attrs)
-
-    def decompress(self, value):
-        if value:
-            return value
-        return [None, None]
-
-    def get_context(self, name, value, attrs):
-        context = super().get_context(name, value, attrs)
-        context['date_label'] = "日期："
-        context['time_label'] = "时间："
-        return context
-
-    class Media:
-        css = {
-            'all': ('common_task_system/css/calendar.css',)
-        }
-        js = ('common_task_system/js/calendar.js',)
-
-
-class MultiDaySelectField(forms.MultiValueField):
-    widget = MultiDaySelectWidget
-
-    def __init__(self, required=False, label="自选日期", **kwargs):
-        fs = (
-            forms.CharField(),
-            forms.TimeField()
-        )
-        super(MultiDaySelectField, self).__init__(fs, required=required, label=label, **kwargs)
-
-    def compress(self, data_list):
-        return data_list
-
-    def decompress(self, value):
-        if value:
-            return value
-        return [None, None]
-
-
-class MultiMonthdaySelectFiled(forms.MultipleChoiceField):
-    _choices = [
-        (0, "每月第一天"),
-        (32, "每月最后一天"),
-        (1, "1号"),
-        (2, "2号"),
-        (3, "3号"),
-        (4, "4号"),
-        (5, "5号"),
-        (6, "6号"),
-        (7, "7号"),
-        (8, "8号"),
-        (9, "9号"),
-        (10, "10号"),
-        (11, "11号"),
-        (12, "12号"),
-        (13, "13号"),
-        (14, "14号"),
-        (15, "15号"),
-        (16, "16号"),
-        (17, "17号"),
-        (18, "18号"),
-        (19, "19号"),
-        (20, "20号"),
-        (21, "21号"),
-        (22, "22号"),
-        (23, "23号"),
-        (24, "24号"),
-        (25, "25号"),
-        (26, "26号"),
-        (27, "27号"),
-        (28, "28号"),
-        (29, "29号"),
-        (30, "30号"),
-        (31, "31号"),
-    ]
-    widget = forms.CheckboxSelectMultiple()
-
-    template_name = 'task_schedule/multi_monthday_select.html'
-
-    def __init__(self, *, choices=(), label="日期", widget=None, **kwargs):
-        super(MultiMonthdaySelectFiled, self).__init__(
-            choices=choices or self._choices,
-            label=label,
-            widget=widget or self.widget,
-            **kwargs)
-
-    def to_python(self, value):
-        if not value:
-            return []
-        elif not isinstance(value, (list, tuple)):
-            raise forms.ValidationError(
-                self.error_messages["invalid_list"], code="invalid_list"
-            )
-        return [int(val) for val in value]
-
-
-class MultiYearDaySelectWidget(forms.TextInput):
-    template_name = 'task_schedule/multi_month_day_select.html'
-
-    class Media:
-        css = {
-            'all': ('common_task_system/css/calendar.css',)
-        }
-        js = ('common_task_system/js/calendar.js',)
-
-
-class NLPSentenceWidget(forms.TextInput):
-    template_name = 'task_schedule/nlp_input.html'
-
-
-class TaskScheduleForm(forms.ModelForm):
-    schedule_type = forms.ChoiceField(required=True, label="计划类型", choices=TaskScheduleType.choices)
-    base_on_now = forms.BooleanField(required=False, label="基于当前时间", initial=False)
-    next_schedule_time = forms.DateTimeField(required=False, label='下次计划时间',
-                                             widget=forms.TextInput(attrs={'readonly': 'readonly'}))
-    nlp_sentence = forms.CharField(required=False, label="NLP", help_text="自然语言，如：每天早上8点",
-                                   widget=NLPSentenceWidget(attrs={'style': "width: 60%;"}))
-    crontab = forms.CharField(required=False, label="Crontab表达式", help_text="crontab表达式，如：* * * * *")
-    period_schedule = PeriodScheduleFiled()
-    once_schedule = OnceScheduleField()
-    timing_type = forms.ChoiceField(required=False, label="指定时间", choices=ScheduleTimingType.choices)
-    timing_weekday = MultiWeekdaySelectFiled(required=False)
-    timing_monthday = MultiMonthdaySelectFiled(required=False)
-    timing_year = forms.CharField(required=False, label="选择日期",
-                                  widget=MultiYearDaySelectWidget(attrs={'style': "width: 60%;"}))
-    timing_datetime = MultiDaySelectField()
-    timing_period = forms.IntegerField(required=False, min_value=1, initial=1, label='频率', widget=PeriodWidget)
-    timing_time = forms.TimeField(required=False, initial=datetime_time(),
-                                  label="时间", widget=widgets.AdminTimeWidget)
-    config = forms.JSONField(required=False, initial={}, label="配置",
-                             widget=JSONWidget(attrs={'readonly': 'readonly'})
-                             )
-
-    def __init__(self, *args, **kwargs):
-        super(TaskScheduleForm, self).__init__(*args, **kwargs)
-        if self.instance.pk:
-            config = self.instance.config
-            schedule_type = config.get('schedule_type')
-            self.initial['schedule_type'] = schedule_type
-            type_config = config[schedule_type]
-            self.initial['nlp_sentence'] = config.get('nlp-sentence')
-            self.initial['base_on_now'] = config.get('base_on_now', False)
-            if schedule_type == TaskScheduleType.CONTINUOUS:
-                t = datetime.strptime(type_config['schedule_start_time'], '%Y-%m-%d %H:%M:%S')
-                self.initial['period_schedule'] = [t, type_config['period']]
-            elif schedule_type == TaskScheduleType.ONCE:
-                self.initial['once_schedule'] = datetime.strptime(type_config['schedule_start_time'],
-                                                                  '%Y-%m-%d %H:%M:%S')
-            elif schedule_type == TaskScheduleType.CRONTAB:
-                self.initial['crontab'] = type_config['crontab']
-            elif schedule_type == TaskScheduleType.TIMINGS:
-                timing_type = type_config.get('type')
-                timing_config = type_config.get(timing_type, {})
-                self.initial['timing_type'] = timing_type
-                self.initial['timing_time'] = type_config['time']
-                self.initial['timing_period'] = timing_config.get('period', 1)
-                if timing_type == ScheduleTimingType.WEEKDAY:
-                    self.initial['timing_weekday'] = timing_config.get('weekday')
-                elif timing_type == ScheduleTimingType.MONTHDAY:
-                    self.initial['timing_monthday'] = timing_config.get('monthday')
-                elif timing_type == ScheduleTimingType.YEAR:
-                    self.initial['timing_year'] = timing_config.get('year')
-                elif timing_type == ScheduleTimingType.DATETIME:
-                    self.initial['timing_datetime'] = timing_config.get('datetime')
-
-    def clean(self):
-        cleaned_data = super(TaskScheduleForm, self).clean()
-        cleaned_data.pop("config", None)
-        schedule = models.ScheduleConfig(**cleaned_data)
-        cleaned_data['config'] = schedule.config
-        cleaned_data['next_schedule_time'] = schedule.get_current_time(
-            start_time=cleaned_data.get('schedule_start_time', None)
-        )
-        return cleaned_data
-
-    class Meta:
-        model = models.TaskSchedule
-        fields = "__all__"
-
-
-class TaskScheduleQueueForm(forms.ModelForm):
-
-    def clean(self):
-        cleaned_data = super(TaskScheduleQueueForm, self).clean()
-        if not self.errors:
-            module = cleaned_data.get('module')
-            config = cleaned_data.get('config')
-            config.setdefault('name', 'SYSTEM_TASK_QUEUE:%s' % cleaned_data['code'])
-            queueCls = import_string(module)
-            validate_config = getattr(queueCls, 'validate_config', None)
-            if validate_config:
-                error = validate_config(config)
-                if error:
-                    self.add_error('config', error)
-            if not self.errors:
-                args = inspect.getfullargspec(getattr(queueCls, '__init__'))
-                kwargs = {k: v for k, v in config.items() if k in args.args}
-                if 'name' not in kwargs:
-                    config.pop('name')
-                queue = queueCls(**kwargs)
-                validate = getattr(queue, 'validate', None)
-                if validate:
-                    error = validate()
-                    if error:
-                        self.add_error('config', error)
-        return cleaned_data
-
-    class Meta:
-        model = models.TaskScheduleQueue
-        fields = '__all__'
-
-
-class TaskScheduleProducerForm(forms.ModelForm):
-    name = forms.CharField(max_length=100, label='名称', required=False)
-
-    def __init__(self, *args, **kwargs):
-        super(TaskScheduleProducerForm, self).__init__(*args, **kwargs)
-        if not self.instance.id:
-            self. initial['filters'] = {
-                'status': TaskScheduleStatus.OPENING.value,
-                'task__status': TaskStatus.ENABLE.value,
-            }
-
-    def clean(self):
-        cleaned_data = super(TaskScheduleProducerForm, self).clean()
-        if not self.errors:
-            filters = cleaned_data.get('filters')
-            if not filters:
-                self.add_error('filters', 'filters不能为空')
-            else:
-                try:
-                    models.TaskSchedule.objects.filter(**filters).first()
-                except Exception as e:
-                    self.add_error('filters', 'filters参数错误: %s' % e)
-                else:
-                    name = cleaned_data.get('name')
-                    if not name:
-                        cleaned_data['name'] = "队列(%s)生产者" % cleaned_data.get('queue').name
-        return cleaned_data
-
-    class Meta:
-        model = models.TaskScheduleProducer
-        fields = '__all__'
-
-
-class ConsumerPermissionForm(forms.ModelForm):
-    config = forms.JSONField(required=False, initial={}, label="配置",
-                             widget=forms.HiddenInput())
-    ip_whitelist = forms.CharField(required=False, label="IP白名单", widget=forms.Textarea(
-        attrs={'rows': 10, 'style': 'width: 60%'}))
-
-    def __init__(self, *args, **kwargs):
-        super(ConsumerPermissionForm, self).__init__(*args, **kwargs)
-        if self.instance.id:
-            self.initial['ip_whitelist'] = '\n'.join(self.instance.config.get('ip_whitelist', []) or [])
-
-    def clean(self):
-        cleaned_data = super(ConsumerPermissionForm, self).clean()
-        if not self.errors:
-            ip_whitelist = cleaned_data.pop('ip_whitelist', "")
-            cleaned_data['config'] = {'ip_whitelist': [x.strip() for x in ip_whitelist.split('\n')]}
-        return cleaned_data
-
+import inspect
+from django import forms
+from django.contrib.admin import widgets
+from django.utils.module_loading import import_string
+from .choices import TaskScheduleType, ScheduleTimingType, TaskScheduleStatus, TaskStatus
+from django_common_objects.widgets import JSONWidget
+from .utils import foreign_key
+from datetime import datetime, time as datetime_time
+from . import models
+
+
+class TaskForm(forms.ModelForm):
+
+    def __init__(self, *args, **kwargs):
+        super(TaskForm, self).__init__(*args, **kwargs)
+        task: models.Task = self.instance
+        if task.id:
+            self.fields['parent'].queryset = models.Task.objects.filter(
+                user=task.user
+            ).exclude(id__in=foreign_key.get_related_object_ids(task))
+
+
+class DateTimeRangeWidget(forms.widgets.MultiWidget):
+    template_name = 'task_schedule/datetime_range.html'
+
+    def __init__(self, attrs=None):
+        st = widgets.AdminSplitDateTime()
+        et = widgets.AdminSplitDateTime()
+        super().__init__([st, et], attrs=attrs)
+
+    def get_context(self, name, value, attrs):
+        context = super().get_context(name, value, attrs)
+        context["start_datetime"] = "开始时间:"
+        context["end_datetime"] = "结束时间:"
+        return context
+
+    def decompress(self, value):
+        if value:
+            return value
+        return [None, None]
+
+
+class PeriodWidget(widgets.AdminIntegerFieldWidget):
+    template_name = 'task_schedule/period.html'
+
+    def __init__(self, unit=ScheduleTimingType.DAY.value, attrs=None):
+        self.unit = unit
+        super().__init__(attrs=attrs)
+
+    def get_context(self, name, value, attrs):
+        context = super().get_context(name, value, attrs)
+        context["unit"] = self.unit
+        return context
+
+
+class NullableSplitDateTimeField(forms.SplitDateTimeField):
+
+    def clean(self, value):
+        if value[0] and not value[1]:
+            value[1] = '00:00:00'
+        elif not value[0] and value[1]:
+            value[0] = datetime.now().strftime('%Y-%m-%d')
+        return super(NullableSplitDateTimeField, self).clean(value)
+
+
+class MultiWeekdaySelectFiled(forms.MultipleChoiceField):
+    _choices = [
+        (1, "星期一"),
+        (2, "星期二"),
+        (3, "星期三"),
+        (4, "星期四"),
+        (5, "星期五"),
+        (6, "星期六"),
+        (7, "星期日"),
+    ]
+    widget = forms.CheckboxSelectMultiple
+
+    def __init__(self, *, choices=(), label="星期", widget=None, **kwargs):
+        super(MultiWeekdaySelectFiled, self).__init__(
+            choices=choices or self._choices,
+            label=label,
+            widget=widget or self.widget,
+            **kwargs)
+
+    def to_python(self, value):
+        if not value:
+            return value
+        elif not isinstance(value, (list, tuple)):
+            raise forms.ValidationError(
+                self.error_messages["invalid_list"], code="invalid_list"
+            )
+        return [int(val) for val in value]
+
+
+class PeriodScheduleWidget(forms.MultiWidget):
+    template_name = 'task_schedule/period_schedule.html'
+
+    def __init__(self, default_time=datetime.now, default_period=60, attrs=None):
+        ws = (
+            widgets.AdminSplitDateTime(),
+            widgets.AdminIntegerFieldWidget()
+        )
+        self.default_time = default_time() if callable(default_time) else default_time
+        self.default_period = default_period
+        super().__init__(ws)
+
+    def decompress(self, value):
+        if value:
+            return value
+        return [self.default_time, self.default_period]
+
+
+class PeriodScheduleFiled(forms.MultiValueField):
+    widget = PeriodScheduleWidget
+
+    def __init__(self, label="持续计划", **kwargs):
+        fs = (
+            forms.SplitDateTimeField(help_text="下次开始时间"),
+            forms.IntegerField(help_text="周期/每(秒)")
+        )
+        super(PeriodScheduleFiled, self).__init__(fs, label=label, **kwargs)
+
+    def to_python(self, value):
+        if not value:
+            return []
+        elif not isinstance(value, (list, tuple)):
+            raise forms.ValidationError(
+                self.error_messages["invalid_list"], code="invalid_list"
+            )
+        return [int(val) for val in value]
+
+    def compress(self, data_list):
+        return data_list
+
+
+class OnceScheduleField(forms.SplitDateTimeField):
+    widget = widgets.AdminSplitDateTime
+
+    def __init__(self, required=False, label="计划时间", **kwargs):
+        super(OnceScheduleField, self).__init__(
+            required=required,
+            label=label,
+            initial=datetime.now(), **kwargs)
+
+
+class MultiDaySelectWidget(forms.MultiWidget):
+    template_name = 'task_schedule/multi_day_select.html'
+
+    def __init__(self, attrs=None):
+        ws = (
+            forms.TextInput(attrs={'style': "width: 80%;"}),
+            widgets.AdminTimeWidget(attrs={'style': "margin-top: 5px;"})
+        )
+        super(MultiDaySelectWidget, self).__init__(ws, attrs=attrs)
+
+    def decompress(self, value):
+        if value:
+            return value
+        return [None, None]
+
+    def get_context(self, name, value, attrs):
+        context = super().get_context(name, value, attrs)
+        context['date_label'] = "日期："
+        context['time_label'] = "时间："
+        return context
+
+    class Media:
+        css = {
+            'all': ('common_task_system/css/calendar.css',)
+        }
+        js = ('common_task_system/js/calendar.js',)
+
+
+class MultiDaySelectField(forms.MultiValueField):
+    widget = MultiDaySelectWidget
+
+    def __init__(self, required=False, label="自选日期", **kwargs):
+        fs = (
+            forms.CharField(),
+            forms.TimeField()
+        )
+        super(MultiDaySelectField, self).__init__(fs, required=required, label=label, **kwargs)
+
+    def compress(self, data_list):
+        return data_list
+
+    def decompress(self, value):
+        if value:
+            return value
+        return [None, None]
+
+
+class MultiMonthdaySelectFiled(forms.MultipleChoiceField):
+    _choices = [
+        (0, "每月第一天"),
+        (32, "每月最后一天"),
+        (1, "1号"),
+        (2, "2号"),
+        (3, "3号"),
+        (4, "4号"),
+        (5, "5号"),
+        (6, "6号"),
+        (7, "7号"),
+        (8, "8号"),
+        (9, "9号"),
+        (10, "10号"),
+        (11, "11号"),
+        (12, "12号"),
+        (13, "13号"),
+        (14, "14号"),
+        (15, "15号"),
+        (16, "16号"),
+        (17, "17号"),
+        (18, "18号"),
+        (19, "19号"),
+        (20, "20号"),
+        (21, "21号"),
+        (22, "22号"),
+        (23, "23号"),
+        (24, "24号"),
+        (25, "25号"),
+        (26, "26号"),
+        (27, "27号"),
+        (28, "28号"),
+        (29, "29号"),
+        (30, "30号"),
+        (31, "31号"),
+    ]
+    widget = forms.CheckboxSelectMultiple()
+
+    template_name = 'task_schedule/multi_monthday_select.html'
+
+    def __init__(self, *, choices=(), label="日期", widget=None, **kwargs):
+        super(MultiMonthdaySelectFiled, self).__init__(
+            choices=choices or self._choices,
+            label=label,
+            widget=widget or self.widget,
+            **kwargs)
+
+    def to_python(self, value):
+        if not value:
+            return []
+        elif not isinstance(value, (list, tuple)):
+            raise forms.ValidationError(
+                self.error_messages["invalid_list"], code="invalid_list"
+            )
+        return [int(val) for val in value]
+
+
+class MultiYearDaySelectWidget(forms.TextInput):
+    template_name = 'task_schedule/multi_month_day_select.html'
+
+    class Media:
+        css = {
+            'all': ('common_task_system/css/calendar.css',)
+        }
+        js = ('common_task_system/js/calendar.js',)
+
+
+class NLPSentenceWidget(forms.TextInput):
+    template_name = 'task_schedule/nlp_input.html'
+
+
+class TaskScheduleForm(forms.ModelForm):
+    schedule_type = forms.ChoiceField(required=True, label="计划类型", choices=TaskScheduleType.choices)
+    base_on_now = forms.BooleanField(required=False, label="基于当前时间", initial=False)
+    next_schedule_time = forms.DateTimeField(required=False, label='下次计划时间',
+                                             widget=forms.TextInput(attrs={'readonly': 'readonly'}))
+    nlp_sentence = forms.CharField(required=False, label="NLP", help_text="自然语言，如：每天早上8点",
+                                   widget=NLPSentenceWidget(attrs={'style': "width: 60%;"}))
+    crontab = forms.CharField(required=False, label="Crontab表达式", help_text="crontab表达式，如：* * * * *")
+    period_schedule = PeriodScheduleFiled()
+    once_schedule = OnceScheduleField()
+    timing_type = forms.ChoiceField(required=False, label="指定时间", choices=ScheduleTimingType.choices)
+    timing_weekday = MultiWeekdaySelectFiled(required=False)
+    timing_monthday = MultiMonthdaySelectFiled(required=False)
+    timing_year = forms.CharField(required=False, label="选择日期",
+                                  widget=MultiYearDaySelectWidget(attrs={'style': "width: 60%;"}))
+    timing_datetime = MultiDaySelectField()
+    timing_period = forms.IntegerField(required=False, min_value=1, initial=1, label='频率', widget=PeriodWidget)
+    timing_time = forms.TimeField(required=False, initial=datetime_time(),
+                                  label="时间", widget=widgets.AdminTimeWidget)
+    config = forms.JSONField(required=False, initial={}, label="配置",
+                             widget=JSONWidget(attrs={'readonly': 'readonly'})
+                             )
+
+    def __init__(self, *args, **kwargs):
+        super(TaskScheduleForm, self).__init__(*args, **kwargs)
+        if self.instance.pk:
+            config = self.instance.config
+            schedule_type = config.get('schedule_type')
+            self.initial['schedule_type'] = schedule_type
+            type_config = config[schedule_type]
+            self.initial['nlp_sentence'] = config.get('nlp-sentence')
+            self.initial['base_on_now'] = config.get('base_on_now', False)
+            if schedule_type == TaskScheduleType.CONTINUOUS:
+                t = datetime.strptime(type_config['schedule_start_time'], '%Y-%m-%d %H:%M:%S')
+                self.initial['period_schedule'] = [t, type_config['period']]
+            elif schedule_type == TaskScheduleType.ONCE:
+                self.initial['once_schedule'] = datetime.strptime(type_config['schedule_start_time'],
+                                                                  '%Y-%m-%d %H:%M:%S')
+            elif schedule_type == TaskScheduleType.CRONTAB:
+                self.initial['crontab'] = type_config['crontab']
+            elif schedule_type == TaskScheduleType.TIMINGS:
+                timing_type = type_config.get('type')
+                timing_config = type_config.get(timing_type, {})
+                self.initial['timing_type'] = timing_type
+                self.initial['timing_time'] = type_config['time']
+                self.initial['timing_period'] = timing_config.get('period', 1)
+                if timing_type == ScheduleTimingType.WEEKDAY:
+                    self.initial['timing_weekday'] = timing_config.get('weekday')
+                elif timing_type == ScheduleTimingType.MONTHDAY:
+                    self.initial['timing_monthday'] = timing_config.get('monthday')
+                elif timing_type == ScheduleTimingType.YEAR:
+                    self.initial['timing_year'] = timing_config.get('year')
+                elif timing_type == ScheduleTimingType.DATETIME:
+                    self.initial['timing_datetime'] = timing_config.get('datetime')
+
+    def clean(self):
+        cleaned_data = super(TaskScheduleForm, self).clean()
+        cleaned_data.pop("config", None)
+        schedule = models.ScheduleConfig(**cleaned_data)
+        cleaned_data['config'] = schedule.config
+        cleaned_data['next_schedule_time'] = schedule.get_current_time(
+            start_time=cleaned_data.get('schedule_start_time', None)
+        )
+        return cleaned_data
+
+    class Meta:
+        model = models.TaskSchedule
+        fields = "__all__"
+
+
+class TaskScheduleQueueForm(forms.ModelForm):
+
+    def clean(self):
+        cleaned_data = super(TaskScheduleQueueForm, self).clean()
+        if not self.errors:
+            module = cleaned_data.get('module')
+            config = cleaned_data.get('config')
+            config.setdefault('name', 'SYSTEM_TASK_QUEUE:%s' % cleaned_data['code'])
+            queueCls = import_string(module)
+            validate_config = getattr(queueCls, 'validate_config', None)
+            if validate_config:
+                error = validate_config(config)
+                if error:
+                    self.add_error('config', error)
+            if not self.errors:
+                args = inspect.getfullargspec(getattr(queueCls, '__init__'))
+                kwargs = {k: v for k, v in config.items() if k in args.args}
+                if 'name' not in kwargs:
+                    config.pop('name')
+                queue = queueCls(**kwargs)
+                validate = getattr(queue, 'validate', None)
+                if validate:
+                    error = validate()
+                    if error:
+                        self.add_error('config', error)
+        return cleaned_data
+
+    class Meta:
+        model = models.TaskScheduleQueue
+        fields = '__all__'
+
+
+class TaskScheduleProducerForm(forms.ModelForm):
+    name = forms.CharField(max_length=100, label='名称', required=False)
+
+    def __init__(self, *args, **kwargs):
+        super(TaskScheduleProducerForm, self).__init__(*args, **kwargs)
+        if not self.instance.id:
+            self. initial['filters'] = {
+                'status': TaskScheduleStatus.OPENING.value,
+                'task__status': TaskStatus.ENABLE.value,
+            }
+
+    def clean(self):
+        cleaned_data = super(TaskScheduleProducerForm, self).clean()
+        if not self.errors:
+            filters = cleaned_data.get('filters')
+            if not filters:
+                self.add_error('filters', 'filters不能为空')
+            else:
+                try:
+                    models.TaskSchedule.objects.filter(**filters).first()
+                except Exception as e:
+                    self.add_error('filters', 'filters参数错误: %s' % e)
+                else:
+                    name = cleaned_data.get('name')
+                    if not name:
+                        cleaned_data['name'] = "队列(%s)生产者" % cleaned_data.get('queue').name
+        return cleaned_data
+
+    class Meta:
+        model = models.TaskScheduleProducer
+        fields = '__all__'
+
+
+class ConsumerPermissionForm(forms.ModelForm):
+    config = forms.JSONField(required=False, initial={}, label="配置",
+                             widget=forms.HiddenInput())
+    ip_whitelist = forms.CharField(required=False, label="IP白名单", widget=forms.Textarea(
+        attrs={'rows': 10, 'style': 'width: 60%'}))
+
+    def __init__(self, *args, **kwargs):
+        super(ConsumerPermissionForm, self).__init__(*args, **kwargs)
+        if self.instance.id:
+            self.initial['ip_whitelist'] = '\n'.join(self.instance.config.get('ip_whitelist', []) or [])
+
+    def clean(self):
+        cleaned_data = super(ConsumerPermissionForm, self).clean()
+        if not self.errors:
+            ip_whitelist = cleaned_data.pop('ip_whitelist', "")
+            cleaned_data['config'] = {'ip_whitelist': [x.strip() for x in ip_whitelist.split('\n')]}
+        return cleaned_data
+
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.6/django_common_task_system/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# Generated by Django 4.1.7 on 2023-03-30 03:30
-
-import datetime
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-import django.utils.timezone
-import django_common_objects.fields
-import django_common_objects.models
-import django_common_task_system.fields
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('django_common_objects', '0001_initial'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='Task',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=100, verbose_name='任务名')),
-                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('Task'), null=True, verbose_name='参数')),
-                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('category', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_objects.commoncategory', verbose_name='类别')),
-                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to=settings.TASK_MODEL, verbose_name='父任务')),
-                ('tags', models.ManyToManyField(blank=True, db_constraint=False, to='django_common_objects.commontag', verbose_name='标签')),
-                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
-            ],
-            options={
-                'verbose_name': '任务中心',
-                'verbose_name_plural': '任务中心',
-                'db_table': 'taskhub',
-                'abstract': False,
-                'swappable': 'TASK_MODEL',
-                'unique_together': {('name', 'user', 'parent')},
-            },
-        ),
-        migrations.CreateModel(
-            name='TaskSchedule',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('priority', models.IntegerField(default=0, verbose_name='优先级')),
-                ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
-                ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
-                ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
-                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
-                ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-            ],
-            options={
-                'verbose_name': '任务计划',
-                'verbose_name_plural': '任务计划',
-                'db_table': 'task_schedule',
-                'ordering': ('-priority', 'next_schedule_time'),
-                'abstract': False,
-                'swappable': 'TASK_SCHEDULE_MODEL',
-            },
-        ),
-        migrations.CreateModel(
-            name='TaskScheduleCallback',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=100, verbose_name='回调')),
-                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
-                ('trigger_event', django_common_objects.fields.CharField(choices=[('S', '成功'), ('F', '失败'), ('D', '完成')], default='D', max_length=1, verbose_name='触发事件')),
-                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('TaskCallback'), null=True, verbose_name='参数')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
-            ],
-            options={
-                'verbose_name': '任务回调',
-                'verbose_name_plural': '任务回调',
-                'db_table': 'task_schedule_callback',
-                'abstract': False,
-                'unique_together': {('name', 'user')},
-            },
-        ),
-        migrations.CreateModel(
-            name='TaskScheduleLog',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
-                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
-                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_SCHEDULE_MODEL, verbose_name='任务计划')),
-            ],
-            options={
-                'verbose_name': '任务日志',
-                'verbose_name_plural': '任务日志',
-                'db_table': 'task_schedule_log',
-                'abstract': False,
-                'swappable': 'TASK_SCHEDULE_LOG_MODEL',
-            },
-        ),
-        migrations.AddField(
-            model_name='taskschedule',
-            name='callback',
-            field=models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.taskschedulecallback', verbose_name='回调'),
-        ),
-        migrations.AddField(
-            model_name='taskschedule',
-            name='task',
-            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_MODEL, verbose_name='任务'),
-        ),
-        migrations.AddField(
-            model_name='taskschedule',
-            name='user',
-            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户'),
-        ),
-        migrations.AlterUniqueTogether(
-            name='taskschedule',
-            unique_together={('task', 'user')},
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-03-30 03:30
+
+import datetime
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+import django.utils.timezone
+import django_common_objects.fields
+import django_common_objects.models
+import django_common_task_system.fields
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('django_common_objects', '0001_initial'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='Task',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=100, verbose_name='任务名')),
+                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('Task'), null=True, verbose_name='参数')),
+                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('category', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_objects.commoncategory', verbose_name='类别')),
+                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to=settings.TASK_MODEL, verbose_name='父任务')),
+                ('tags', models.ManyToManyField(blank=True, db_constraint=False, to='django_common_objects.commontag', verbose_name='标签')),
+                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
+            ],
+            options={
+                'verbose_name': '任务中心',
+                'verbose_name_plural': '任务中心',
+                'db_table': 'taskhub',
+                'abstract': False,
+                'swappable': 'TASK_MODEL',
+                'unique_together': {('name', 'user', 'parent')},
+            },
+        ),
+        migrations.CreateModel(
+            name='TaskSchedule',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('priority', models.IntegerField(default=0, verbose_name='优先级')),
+                ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
+                ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
+                ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
+                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
+                ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+            ],
+            options={
+                'verbose_name': '任务计划',
+                'verbose_name_plural': '任务计划',
+                'db_table': 'task_schedule',
+                'ordering': ('-priority', 'next_schedule_time'),
+                'abstract': False,
+                'swappable': 'TASK_SCHEDULE_MODEL',
+            },
+        ),
+        migrations.CreateModel(
+            name='TaskScheduleCallback',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=100, verbose_name='回调')),
+                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
+                ('trigger_event', django_common_objects.fields.CharField(choices=[('S', '成功'), ('F', '失败'), ('D', '完成')], default='D', max_length=1, verbose_name='触发事件')),
+                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('TaskCallback'), null=True, verbose_name='参数')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
+            ],
+            options={
+                'verbose_name': '任务回调',
+                'verbose_name_plural': '任务回调',
+                'db_table': 'task_schedule_callback',
+                'abstract': False,
+                'unique_together': {('name', 'user')},
+            },
+        ),
+        migrations.CreateModel(
+            name='TaskScheduleLog',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
+                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
+                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_SCHEDULE_MODEL, verbose_name='任务计划')),
+            ],
+            options={
+                'verbose_name': '任务日志',
+                'verbose_name_plural': '任务日志',
+                'db_table': 'task_schedule_log',
+                'abstract': False,
+                'swappable': 'TASK_SCHEDULE_LOG_MODEL',
+            },
+        ),
+        migrations.AddField(
+            model_name='taskschedule',
+            name='callback',
+            field=models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.taskschedulecallback', verbose_name='回调'),
+        ),
+        migrations.AddField(
+            model_name='taskschedule',
+            name='task',
+            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.TASK_MODEL, verbose_name='任务'),
+        ),
+        migrations.AddField(
+            model_name='taskschedule',
+            name='user',
+            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户'),
+        ),
+        migrations.AlterUniqueTogether(
+            name='taskschedule',
+            unique_together={('task', 'user')},
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.6/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# Generated by Django 4.1.7 on 2023-04-13 16:54
-
-from django.db import migrations, models
-import django.db.models.deletion
-import django_common_task_system.models
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('django_common_task_system', '0003_alter_taskschedulelog_schedule'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='TaskScheduleQueue',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100, unique=True, verbose_name='队列名称')),
-                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.models.code_validator], verbose_name='队列编码')),
-                ('status', models.BooleanField(default=True, verbose_name='状态')),
-                ('module', models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列'), ('django_common_task_system.system_task.queue.RedisListQueue', 'Redis List队列')], default='queue.Queue', max_length=100, verbose_name='队列类型')),
-                ('config', models.JSONField(blank=True, default=dict, null=True, verbose_name='配置')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-            ],
-            options={
-                'verbose_name': '任务队列',
-                'verbose_name_plural': '任务队列',
-                'db_table': 'task_schedule_queue',
-                'abstract': False,
-            },
-        ),
-        migrations.AddField(
-            model_name='taskschedulelog',
-            name='queue',
-            field=models.CharField(default='opening', max_length=100, verbose_name='队列'),
-        ),
-        migrations.CreateModel(
-            name='TaskScheduleProducer',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100, verbose_name='生产者名称')),
-                ('filters', models.JSONField(verbose_name='过滤器')),
-                ('lte_now', models.BooleanField(default=True, verbose_name='小于等于当前时间')),
-                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='producers', to='django_common_task_system.taskschedulequeue', verbose_name='队列')),
-            ],
-            options={
-                'verbose_name': '计划生产',
-                'verbose_name_plural': '计划生产',
-                'db_table': 'task_schedule_producer',
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-13 16:54
+
+from django.db import migrations, models
+import django.db.models.deletion
+import django_common_task_system.models
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('django_common_task_system', '0003_alter_taskschedulelog_schedule'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='TaskScheduleQueue',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, unique=True, verbose_name='队列名称')),
+                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.models.code_validator], verbose_name='队列编码')),
+                ('status', models.BooleanField(default=True, verbose_name='状态')),
+                ('module', models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列'), ('django_common_task_system.system_task.queue.RedisListQueue', 'Redis List队列')], default='queue.Queue', max_length=100, verbose_name='队列类型')),
+                ('config', models.JSONField(blank=True, default=dict, null=True, verbose_name='配置')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+            ],
+            options={
+                'verbose_name': '任务队列',
+                'verbose_name_plural': '任务队列',
+                'db_table': 'task_schedule_queue',
+                'abstract': False,
+            },
+        ),
+        migrations.AddField(
+            model_name='taskschedulelog',
+            name='queue',
+            field=models.CharField(default='opening', max_length=100, verbose_name='队列'),
+        ),
+        migrations.CreateModel(
+            name='TaskScheduleProducer',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, verbose_name='生产者名称')),
+                ('filters', models.JSONField(verbose_name='过滤器')),
+                ('lte_now', models.BooleanField(default=True, verbose_name='小于等于当前时间')),
+                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='producers', to='django_common_task_system.taskschedulequeue', verbose_name='队列')),
+            ],
+            options={
+                'verbose_name': '计划生产',
+                'verbose_name_plural': '计划生产',
+                'db_table': 'task_schedule_producer',
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.2.6/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Generated by Django 4.1.7 on 2023-04-21 15:23
-
-from django.db import migrations, models
-import django.utils.timezone
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('django_common_task_system', '0006_consumerpermission'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='ExceptionReport',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('ip', models.CharField(max_length=100, verbose_name='IP')),
-                ('content', models.TextField(verbose_name='内容')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-            ],
-            options={
-                'verbose_name': '异常报告',
-                'verbose_name_plural': '异常报告',
-                'db_table': 'task_exception_report',
-                'ordering': ('-create_time',),
-                'abstract': False,
-            },
-        ),
-        migrations.AlterModelOptions(
-            name='taskschedulelog',
-            options={'ordering': ('-create_time',), 'verbose_name': '任务日志', 'verbose_name_plural': '任务日志'},
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-21 15:23
+
+from django.db import migrations, models
+import django.utils.timezone
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('django_common_task_system', '0006_consumerpermission'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='ExceptionReport',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('ip', models.CharField(max_length=100, verbose_name='IP')),
+                ('content', models.TextField(verbose_name='内容')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+            ],
+            options={
+                'verbose_name': '异常报告',
+                'verbose_name_plural': '异常报告',
+                'db_table': 'task_exception_report',
+                'ordering': ('-create_time',),
+                'abstract': False,
+            },
+        ),
+        migrations.AlterModelOptions(
+            name='taskschedulelog',
+            options={'ordering': ('-create_time',), 'verbose_name': '任务日志', 'verbose_name_plural': '任务日志'},
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/mixin.py` & `django-common-task-system-1.2.6/django_common_task_system/mixin.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from django.db import router, transaction
-from django.db.models.signals import post_save, pre_save
-
-
-class ProxyModelSignalMixin:
-
-    def save_base(
-            self,
-            raw=False,
-            force_insert=False,
-            force_update=False,
-            using=None,
-            update_fields=None,
-    ):
-        """
-                Handle the parts of saving which should be done only once per save,
-                yet need to be done in raw saves, too. This includes some sanity
-                checks and signal sending.
-
-                The 'raw' argument is telling save_base not to save any parent
-                models and not to do any changes to the values before save. This
-                is used by fixture loading.
-                """
-        using = using or router.db_for_write(self.__class__, instance=self)
-        assert not (force_insert and (force_update or update_fields))
-        assert update_fields is None or update_fields
-        # assume that the model is proxy model
-        cls = origin = self.__class__
-        # Skip proxies, but keep the origin as the proxy model.
-        if cls._meta.proxy:
-            cls = cls._meta.concrete_model
-        meta = cls._meta
-        if not meta.auto_created:
-            pre_save.send(
-                sender=cls,
-                instance=self,
-                raw=raw,
-                using=using,
-                update_fields=update_fields,
-            )
-        # A transaction isn't needed if one query is issued.
-        if meta.parents:
-            context_manager = transaction.atomic(using=using, savepoint=False)
-        else:
-            context_manager = transaction.mark_for_rollback_on_error(using=using)
-        with context_manager:
-            parent_inserted = False
-            if not raw:
-                parent_inserted = self._save_parents(cls, using, update_fields)
-            updated = self._save_table(
-                raw,
-                cls,
-                force_insert or parent_inserted,
-                force_update,
-                using,
-                update_fields,
-            )
-        # Store the database on which the object was saved
-        self._state.db = using
-        # Once saved, this is no longer a to-be-added instance.
-        self._state.adding = False
-
-        # Signal that the save is complete
-        if not meta.auto_created:
-            post_save.send(
-                sender=cls,
-                instance=self,
-                created=(not updated),
-                update_fields=update_fields,
-                raw=raw,
-                using=using,
-            )
+from django.db import router, transaction
+from django.db.models.signals import post_save, pre_save
+
+
+class ProxyModelSignalMixin:
+
+    def save_base(
+            self,
+            raw=False,
+            force_insert=False,
+            force_update=False,
+            using=None,
+            update_fields=None,
+    ):
+        """
+                Handle the parts of saving which should be done only once per save,
+                yet need to be done in raw saves, too. This includes some sanity
+                checks and signal sending.
+
+                The 'raw' argument is telling save_base not to save any parent
+                models and not to do any changes to the values before save. This
+                is used by fixture loading.
+                """
+        using = using or router.db_for_write(self.__class__, instance=self)
+        assert not (force_insert and (force_update or update_fields))
+        assert update_fields is None or update_fields
+        # assume that the model is proxy model
+        cls = origin = self.__class__
+        # Skip proxies, but keep the origin as the proxy model.
+        if cls._meta.proxy:
+            cls = cls._meta.concrete_model
+        meta = cls._meta
+        if not meta.auto_created:
+            pre_save.send(
+                sender=cls,
+                instance=self,
+                raw=raw,
+                using=using,
+                update_fields=update_fields,
+            )
+        # A transaction isn't needed if one query is issued.
+        if meta.parents:
+            context_manager = transaction.atomic(using=using, savepoint=False)
+        else:
+            context_manager = transaction.mark_for_rollback_on_error(using=using)
+        with context_manager:
+            parent_inserted = False
+            if not raw:
+                parent_inserted = self._save_parents(cls, using, update_fields)
+            updated = self._save_table(
+                raw,
+                cls,
+                force_insert or parent_inserted,
+                force_update,
+                using,
+                update_fields,
+            )
+        # Store the database on which the object was saved
+        self._state.db = using
+        # Once saved, this is no longer a to-be-added instance.
+        self._state.adding = False
+
+        # Signal that the save is complete
+        if not meta.auto_created:
+            post_save.send(
+                sender=cls,
+                instance=self,
+                created=(not updated),
+                update_fields=update_fields,
+                raw=raw,
+                using=using,
+            )
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/models.py` & `django-common-task-system-1.2.6/django_common_task_system/models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,835 +1,835 @@
-from django.utils import timezone
-from django.contrib.auth import get_user_model
-from django.db import models
-from django.utils.module_loading import import_string
-from .choices import TaskStatus, TaskScheduleStatus, TaskScheduleType, TaskCallbackStatus, \
-    TaskCallbackEvent, ScheduleTimingType, ScheduleQueueModule, ConsumerPermissionType
-from django_common_objects.models import CommonTag, CommonCategory, get_default_config
-from django_common_objects import fields as common_fields
-from .utils.cron_utils import get_next_cron_time
-from .utils import foreign_key
-from datetime import datetime, timedelta
-from . import fields
-from jionlp_time import parse_time
-from .utils.schedule_time import nlp_config_to_schedule_config
-from . import settings
-from . permissions import ConsumerPermissionValidator
-import re
-import os
-from django.core.validators import ValidationError
-from django.dispatch import Signal, receiver
-from threading import Event
-from collections import OrderedDict
-
-system_initialize_signal = Signal()
-system_schedule_event = Event()
-system_signal_sent = False
-
-mdays = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
-
-
-UserModel = get_user_model()
-
-is_task_initialized = 'django_common_task_system' in settings.INSTALLED_APPS
-is_system_task_initialized = 'django_common_system_task.system_task' in settings.INSTALLED_APPS
-
-
-@receiver(system_initialize_signal, sender='builtin_initialized')
-def on_builtin_initialized(sender, app=None, **kwargs):
-    global is_task_initialized, is_system_task_initialized, system_signal_sent
-    if app == 'django_common_task_system':
-        is_task_initialized = True
-    elif app == 'django_common_task_system.system_task':
-        is_system_task_initialized = True
-    # 加入system_signal_sent判断, 防止重复发送信号
-    if is_task_initialized and is_system_task_initialized and not system_signal_sent:
-        from threading import Timer
-
-        def send_signal():
-            system_initialize_signal.send(sender='system_initialized')
-        # 这里django_common_task_system和django_common_system_task都初始化完成了, 但是其他app还未
-        # 完成初始化, 所以这里延迟一段时间再发送信号
-        system_signal_sent = True
-        Timer(2, send_signal).start()
-
-
-def code_validator(value):
-    if re.match(r'[a-zA-Z_-]+', value) is None:
-        raise ValidationError('编码只能包含字母、数字、下划线和中划线')
-
-
-class AbstractTask(models.Model):
-    id = models.AutoField(primary_key=True)
-    parent = models.ForeignKey('self', db_constraint=False, on_delete=models.DO_NOTHING,
-                               null=True, blank=True, verbose_name='父任务')
-    name = models.CharField(max_length=100, verbose_name='任务名')
-    category = models.ForeignKey(CommonCategory, db_constraint=False, on_delete=models.DO_NOTHING, verbose_name='类别')
-    tags = models.ManyToManyField(CommonTag, blank=True, db_constraint=False, verbose_name='标签')
-    description = models.TextField(blank=True, null=True, verbose_name='描述')
-    config = common_fields.ConfigField(default=get_default_config('Task'),
-                                       blank=True, null=True, verbose_name='参数')
-    status = common_fields.CharField(max_length=1, default=TaskStatus.ENABLE.value, verbose_name='状态',
-                                     choices=TaskStatus.choices)
-    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
-    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    @property
-    def associated_tasks_ids(self):
-        return foreign_key.get_related_object_ids(self)
-
-    class Meta:
-        db_table = 'taskhub'
-        verbose_name = verbose_name_plural = '任务中心'
-        unique_together = ('name', 'user', 'parent')
-        abstract = True
-
-    def __str__(self):
-        return self.name
-
-    __repr__ = __str__
-
-
-class Task(AbstractTask):
-
-    class Meta(AbstractTask.Meta):
-        swappable = 'TASK_MODEL'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractScheduleCallback(models.Model):
-    id = models.AutoField(primary_key=True)
-    name = models.CharField(max_length=100, verbose_name='回调')
-    description = models.TextField(blank=True, null=True, verbose_name='描述')
-    trigger_event = common_fields.CharField(default=TaskCallbackEvent.DONE, choices=TaskCallbackEvent.choices,
-                                            verbose_name='触发事件')
-    status = common_fields.CharField(default=TaskCallbackStatus.ENABLE.value, verbose_name='状态',
-                                     choices=TaskCallbackStatus.choices)
-    config = common_fields.ConfigField(default=get_default_config('TaskCallback'), blank=True, null=True,
-                                       verbose_name='参数')
-    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
-    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    class Meta:
-        db_table = 'task_schedule_callback'
-        verbose_name = verbose_name_plural = '任务回调'
-        unique_together = ('name', 'user')
-        abstract = True
-
-    def __str__(self):
-        return self.name
-
-    __repr__ = __str__
-
-
-class TaskScheduleCallback(AbstractScheduleCallback):
-    class Meta(AbstractScheduleCallback.Meta):
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class ScheduleConfig:
-
-    def __init__(self,
-                 base_on_now=True,
-                 nlp_sentence=None,
-                 schedule_type=None,
-                 crontab=None,
-                 period_schedule=None,
-                 once_schedule=None,
-                 timing_type=None,
-                 timing_period=None,
-                 timing_time=None,
-                 timing_weekday=None,
-                 timing_monthday=None,
-                 timing_year=None,
-                 timing_datetime=None,
-                 config=None,
-                 **kwargs):
-        self.base_on_now = base_on_now
-        self.nlp_sentence = nlp_sentence
-        self.schedule_type = schedule_type
-        self.once_schedule = once_schedule
-        self.period_schedule = period_schedule
-        self.crontab = crontab
-        self.timing_type = timing_type
-        self.timing_period = timing_period
-        self.timing_time = timing_time
-        self.timing_weekday = timing_weekday
-        self.timing_monthday = timing_monthday
-        self.timing_year = timing_year
-        self.timing_datetime = timing_datetime
-        self.kwargs = kwargs
-        self.config = config or self.to_config()
-        if config:
-            self.parse_config(config)
-
-    def parse_config(self, config):
-        schedule_type = self.schedule_type = config['schedule_type']
-        self.base_on_now = config.get('base_on_now', False)
-        type_config = config[schedule_type]
-        if schedule_type == TaskScheduleType.ONCE:
-            self.once_schedule = type_config['schedule_start_time']
-        elif schedule_type == TaskScheduleType.CRONTAB:
-            self.crontab = type_config['crontab']
-        elif schedule_type == TaskScheduleType.CONTINUOUS:
-            self.period_schedule = [
-                type_config["schedule_start_time"],
-                type_config["period"]
-            ]
-        elif schedule_type == TaskScheduleType.TIMINGS:
-            timing_type = self.timing_type = type_config["type"]
-            self.timing_time = datetime.strptime(type_config["time"], '%H:%M:%S')
-            timing_config = type_config[timing_type]
-            self.timing_period = timing_config.get('period')
-            if timing_type == ScheduleTimingType.DAY:
-                pass
-            elif timing_type == ScheduleTimingType.WEEKDAY:
-                self.timing_monthday = timing_config['weekday']
-            elif timing_type == ScheduleTimingType.MONTHDAY:
-                self.timing_monthday = timing_config['monthday']
-            elif timing_type == ScheduleTimingType.YEAR:
-                self.timing_year = timing_config['year']
-
-    def to_config(self):
-        if self.nlp_sentence:
-            result = parse_time(self.nlp_sentence)
-            config = nlp_config_to_schedule_config(result, sentence=self.nlp_sentence)
-            self.schedule_type = config['schedule_type']
-            return config
-        config = {
-            'schedule_type': self.schedule_type,
-            'base_on_now': self.base_on_now,
-        }
-        schedule_type = self.schedule_type
-        type_config: dict = config.setdefault(self.schedule_type, {})
-        if schedule_type == TaskScheduleType.CRONTAB:
-            if not self.crontab:
-                raise ValidationError('crontab is required while type is crontab')
-            type_config['crontab'] = self.crontab
-        elif schedule_type == TaskScheduleType.CONTINUOUS:
-            if not self.period_schedule:
-                raise ValidationError("period_schedule is required while type is continuous")
-            schedule_time, period = self.period_schedule
-            if period == 0:
-                raise ValidationError("period can't be 0 while type is continuous")
-            type_config['period'] = period
-            type_config['schedule_start_time'] = schedule_time
-        elif schedule_type == TaskScheduleType.ONCE:
-            type_config['schedule_start_time'] = self.once_schedule
-        elif schedule_type == TaskScheduleType.TIMINGS:
-            timing_type = self.timing_type
-            type_config['time'] = self.timing_time.strftime('%H:%M:%S')
-            type_config['type'] = timing_type
-            timing_config = type_config.setdefault(timing_type, {})
-            if timing_type == ScheduleTimingType.DAY:
-                if self.timing_period == 0:
-                    raise ValidationError("period can't be 0 while type is timing")
-                timing_config['period'] = self.timing_period
-            elif timing_type == ScheduleTimingType.WEEKDAY:
-                if not self.timing_weekday:
-                    raise ValidationError("weekdays is required while type is timing")
-                timing_config['period'] = self.timing_period
-                timing_config['weekday'] = self.timing_weekday
-            elif timing_type == ScheduleTimingType.MONTHDAY:
-                timing_config['period'] = self.timing_period
-                timing_config['monthday'] = self.timing_monthday
-            elif timing_type == ScheduleTimingType.YEAR:
-                timing_config['period'] = self.timing_period
-                timing_config['year'] = self.timing_year
-            elif timing_type == ScheduleTimingType.DATETIME:
-                timing_config['datetime'] = self.timing_datetime
-            else:
-                raise ValidationError("timing_type is invalid")
-        else:
-            raise ValidationError("type<%s> is invalid" % schedule_type)
-        return config
-
-    def get_current_time(self, start_time=None):
-        if self.base_on_now:
-            now = datetime.now()
-        else:
-            if start_time and start_time != datetime.min:
-                now = datetime.fromtimestamp(start_time.timestamp())
-            else:
-                now = datetime.now()
-        now_seconds = now.hour * 3600 + now.minute * 60 + now.second
-        schedule_type = self.schedule_type
-        type_config = self.config[schedule_type]
-        schedule_time = None
-        if schedule_type == TaskScheduleType.CONTINUOUS.value:
-            schedule_time, period = self.period_schedule
-            while schedule_time < now:
-                schedule_time += timedelta(seconds=period)
-        elif schedule_type == TaskScheduleType.CRONTAB.value:
-            schedule_time = get_next_cron_time(type_config['crontab'], now)
-        elif schedule_type == TaskScheduleType.TIMINGS:
-            timing_type = type_config['type']
-            hour, minute, second = type_config['time'].split(':')
-            hour, minute, second = int(hour), int(minute), int(second)
-            timing_config = type_config[timing_type]
-            if timing_type == ScheduleTimingType.DAY:
-                schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
-                while schedule_time < now:
-                    schedule_time += timedelta(days=timing_config['period'])
-            elif timing_type == ScheduleTimingType.WEEKDAY:
-                weekdays = timing_config['weekday']
-                weekday = now.isoweekday()
-                schedule_again = weekday not in weekdays
-                if not schedule_again:
-                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
-                    if now > schedule_time:
-                        schedule_again = True
-                if schedule_again:
-                    for i in weekdays:
-                        if i > weekday:
-                            days = i - weekday
-                            delta = timedelta(days=days)
-                            break
-                    else:
-                        days = weekday - weekdays[0]
-                        delta = timedelta(days=timing_config['period'] * 7 - days)
-                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second) + delta
-            elif timing_type == ScheduleTimingType.MONTHDAY:
-                monthdays = timing_config['monthday']
-                if not monthdays:
-                    raise ValidationError("monthdays is required while type is timing-monthday")
-                schedule_again = now.day not in monthdays
-                if not schedule_again:
-                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
-                    if now > schedule_time:
-                        schedule_again = True
-                if schedule_again:
-                    def next_month(y, m):
-                        if m == 12:
-                            return y + 1, 1
-                        else:
-                            return y, m + 1
-                    for i in monthdays:
-                        if i == 0:
-                            i = 1
-                        elif i == 32:
-                            i = mdays[now.month]
-                        if i > now.day:
-                            schedule_time = datetime(now.year, now.month, i, hour, minute, second)
-                            break
-                    else:
-                        year, month = next_month(now.year, now.month)
-                        schedule_time = datetime(year, month, monthdays[0], hour, minute, second)
-            elif timing_type == ScheduleTimingType.YEAR:
-                month_days = timing_config['year']
-                if not month_days:
-                    raise ValidationError("year month day is required while type is timing-datetime")
-                month, day = 1, 1
-                for i in month_days.split(","):
-                    month, day = i.split('-')
-                    month, day = int(month), int(day)
-                    d = datetime(now.year, month, day, hour, minute, second)
-                    if d > now:
-                        schedule_time = d
-                        break
-                else:
-                    schedule_time = datetime(now.year + timing_config['period'], month, day, hour, minute, second)
-            elif timing_type == ScheduleTimingType.DATETIME:
-                dates, t = timing_config['datetime']
-                if not dates:
-                    raise ValidationError("datetime is required while type is timing-datetime")
-                if t:
-                    t: datetime.time
-                    seconds = t.hour * 3600 + t.minute * 60 + t.second
-                else:
-                    seconds = 0
-                for i in dates.split(','):
-                    d = datetime.strptime(i, '%Y-%m-%d')
-                    if d > now or (d == now and seconds >= now_seconds):
-                        break
-                else:
-                    raise ValidationError("cant find a datetime after now")
-                schedule_time = datetime(d.year, d.month, d.day, t.hour, t.minute, t.second)
-            else:
-                raise ValidationError('unsupported timing_type<%s>' % timing_type)
-        elif schedule_type == TaskScheduleType.ONCE:
-            schedule_time = type_config['schedule_start_time']
-        else:
-            raise ValidationError("type<%s> is invalid" % schedule_type)
-        if isinstance(schedule_time, str):
-            schedule_time = datetime.strptime(schedule_time, '%Y-%m-%d %H:%M:%S')
-        # if schedule_time < now:
-        #     raise ValidationError("cant create a schedule time before now, schedule_time<%s>" % schedule_time)
-        return schedule_time
-
-    def get_next_time(self, last_time: datetime):
-        schedule_type = self.schedule_type
-        type_config = self.config[schedule_type]
-        if self.base_on_now:
-            last_time = datetime.now()
-        next_time = last_time
-        if schedule_type == TaskScheduleType.CONTINUOUS.value:
-            while next_time <= last_time:
-                next_time += timedelta(seconds=self.period_schedule[1])
-        elif schedule_type == TaskScheduleType.CRONTAB.value:
-            next_time = get_next_cron_time(type_config['crontab'], last_time)
-        elif schedule_type == TaskScheduleType.TIMINGS:
-            timing_type = type_config['type']
-            hour, minute, second = type_config['time'].split(':')
-            hour, minute, second = int(hour), int(minute), int(second)
-            timing_config = type_config[timing_type]
-            timing_period = timing_config.get('period', 1)
-            next_time = datetime(next_time.year, next_time.month, next_time.day, hour, minute, second)
-            if timing_type == ScheduleTimingType.DAY:
-                while next_time <= last_time:
-                    next_time += timedelta(days=timing_period)
-            elif timing_type == ScheduleTimingType.WEEKDAY:
-                weekdays = timing_config['weekday']
-                weekday = last_time.isoweekday()
-                for i in weekdays:
-                    if i > weekday:
-                        days = i - weekday
-                        delta = timedelta(days=days)
-                        break
-                else:
-                    days = weekday - weekdays[0]
-                    delta = timedelta(days=timing_period * 7 - days)
-                next_time = next_time + delta
-            elif timing_type == ScheduleTimingType.MONTHDAY:
-                monthdays = timing_config['monthday']
-                day = 1
-                for day in monthdays:
-                    if day == 0:
-                        day = 1
-                    elif day == 32:
-                        day = mdays[last_time.month]
-                    next_time = datetime(last_time.year, last_time.month, day, hour, minute, second)
-                    if next_time > last_time:
-                        break
-                else:
-                    month = (last_time.month + timing_period) % 12
-                    if month == 0:
-                        month = 1
-                    year = last_time.year + (last_time.month + timing_period) // 12
-                    next_time = datetime(year, month, day, hour, minute, second)
-            elif timing_type == ScheduleTimingType.YEAR:
-                month_days = timing_config['year']
-                if not month_days:
-                    raise ValidationError("year month day is required while type is timing-datetime")
-                month, day = 1, 1
-                for i in month_days.split(","):
-                    month, day = i.split('-')
-                    month, day = int(month), int(day)
-                    next_time = datetime(last_time.year, month, day, hour, minute, second)
-                    if next_time > last_time:
-                        break
-                else:
-                    next_time = datetime(last_time.year + timing_period, month, day, hour, minute, second)
-            else:
-                raise ValidationError("unsupported timing type: %s" % schedule_type)
-        elif schedule_type == TaskScheduleType.ONCE:
-            next_time = datetime.max
-        else:
-            raise ValidationError("unsupported schedule type: %s" % schedule_type)
-        return next_time
-
-
-class AbstractTaskSchedule(models.Model):
-    id = models.AutoField(primary_key=True)
-    task = models.ForeignKey(settings.TASK_MODEL, on_delete=models.CASCADE, db_constraint=False, verbose_name='任务')
-    priority = models.IntegerField(default=0, verbose_name='优先级')
-    next_schedule_time = models.DateTimeField(default=timezone.now, verbose_name='下次运行时间', db_index=True)
-    schedule_start_time = models.DateTimeField(default=datetime.min, verbose_name='开始时间')
-    schedule_end_time = models.DateTimeField(default=datetime.max, verbose_name='结束时间')
-    config = fields.ScheduleConfigField(default=dict, verbose_name='参数')
-    status = common_fields.CharField(default=TaskScheduleStatus.OPENING.value, verbose_name='状态',
-                                     choices=TaskScheduleStatus.choices)
-    callback = models.ForeignKey(TaskScheduleCallback, on_delete=models.CASCADE,
-                                 null=True, blank=True, db_constraint=False, verbose_name='回调')
-    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
-    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    def generate_next_schedule(self):
-        try:
-            self.next_schedule_time = ScheduleConfig(config=self.config).get_next_time(self.next_schedule_time)
-        except Exception as e:
-            self.status = TaskScheduleStatus.ERROR.value
-            self.save(update_fields=('status',))
-            raise e
-        if self.next_schedule_time > self.schedule_end_time:
-            self.next_schedule_time = datetime.max
-            self.status = TaskScheduleStatus.DONE.value
-        self.save(update_fields=('next_schedule_time', 'status'))
-        return self
-
-    class Meta:
-        db_table = 'task_schedule'
-        verbose_name = verbose_name_plural = '任务计划'
-        ordering = ('-priority', 'next_schedule_time')
-        unique_together = ('task', 'status', 'user')
-        abstract = True
-
-    def __str__(self):
-        return self.task.name
-
-    __repr__ = __str__
-
-    def __lt__(self, other):
-        return self.priority < other.priority
-
-    def __gt__(self, other):
-        return self.priority > other.priority
-
-
-class TaskSchedule(AbstractTaskSchedule):
-    class Meta(AbstractTaskSchedule.Meta):
-        swappable = 'TASK_SCHEDULE_MODEL'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractTaskScheduleQueue(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    name = models.CharField(max_length=100, verbose_name='队列名称', unique=True)
-    code = models.CharField(max_length=100, verbose_name='队列编码', unique=True, validators=[code_validator])
-    status = models.BooleanField(default=True, verbose_name='状态')
-    module = models.CharField(max_length=100, verbose_name='队列类型',
-                              default=ScheduleQueueModule.QUEUE,
-                              choices=ScheduleQueueModule.choices)
-    config = models.JSONField(default=dict, verbose_name='配置', null=True, blank=True)
-    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    class Meta:
-        verbose_name = verbose_name_plural = '任务队列'
-        abstract = True
-
-    def __str__(self):
-        return "%s(%s)" % (self.name, self.code)
-
-
-class TaskScheduleQueue(AbstractTaskScheduleQueue):
-    class Meta(AbstractTaskScheduleQueue.Meta):
-        db_table = 'task_schedule_queue'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractTaskScheduleProducer(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    name = models.CharField(max_length=100, verbose_name='生产名称')
-    filters = models.JSONField(verbose_name='过滤器')
-    lte_now = models.BooleanField(default=True, verbose_name='小于等于当前时间')
-    queue = models.ForeignKey(TaskScheduleQueue, db_constraint=False, related_name='producers',
-                              on_delete=models.CASCADE, verbose_name='队列')
-    status = models.BooleanField(default=True, verbose_name='启用状态')
-    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    class Meta:
-        verbose_name = verbose_name_plural = '计划生产'
-        abstract = True
-
-    def __str__(self):
-        return self.name
-
-
-class TaskScheduleProducer(AbstractTaskScheduleProducer):
-    class Meta(AbstractTaskScheduleProducer.Meta):
-        db_table = 'task_schedule_producer'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractTaskScheduleLog(models.Model):
-    id = models.AutoField(primary_key=True)
-    schedule = models.ForeignKey(TaskSchedule, db_constraint=False, on_delete=models.CASCADE, verbose_name='任务计划')
-    status = common_fields.CharField(verbose_name='运行状态')
-    queue = models.CharField(max_length=100, verbose_name='队列', default='opening')
-    result = common_fields.ConfigField(blank=True, null=True, verbose_name='结果')
-    schedule_time = models.DateTimeField(verbose_name='计划时间')
-    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
-
-    class Meta:
-        db_table = 'task_schedule_log'
-        verbose_name = verbose_name_plural = '任务日志'
-        ordering = ('-create_time',)
-        abstract = True
-
-    def __str__(self):
-        return "schedule: %s, status: %s" % (self.schedule, self.status)
-
-    __repr__ = __str__
-
-
-class TaskScheduleLog(AbstractTaskScheduleLog):
-    schedule = models.ForeignKey(TaskSchedule, db_constraint=False, related_name='logs',
-                                 on_delete=models.CASCADE, verbose_name='任务计划')
-
-    class Meta(AbstractTaskScheduleLog.Meta):
-        swappable = 'TASK_SCHEDULE_LOG_MODEL'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractConsumerPermission(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    producer = models.ForeignKey(TaskScheduleProducer, db_constraint=False,
-                                 on_delete=models.CASCADE, verbose_name='生产者')
-    type = models.CharField(max_length=1, verbose_name='类型',
-                            default=ConsumerPermissionType.IP_WHITE_LIST,
-                            choices=ConsumerPermissionType.choices)
-    status = models.BooleanField(default=True, verbose_name='启用状态')
-    config = models.JSONField(default=dict, verbose_name='配置', null=True, blank=True)
-    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    class Meta:
-        verbose_name = verbose_name_plural = '消费权限'
-        unique_together = ('producer', 'status')
-        abstract = True
-
-    def __str__(self):
-        return self.producer.name
-
-    __repr__ = __str__
-
-
-class ConsumerPermission(AbstractConsumerPermission):
-    class Meta(AbstractConsumerPermission.Meta):
-        db_table = 'schedule_consumer_permission'
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class AbstractExceptionReport(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    ip = models.CharField(max_length=100, verbose_name='IP')
-    content = models.TextField(verbose_name='内容')
-    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
-
-    class Meta:
-        db_table = 'task_exception_report'
-        verbose_name = verbose_name_plural = '异常报告'
-        ordering = ('-create_time',)
-        abstract = True
-
-    def __str__(self):
-        return "Exception(%s, %s)" % (self.ip, self.content[:50])
-
-    __repr__ = __str__
-
-
-class ExceptionReport(AbstractExceptionReport):
-    class Meta(AbstractExceptionReport.Meta):
-        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
-
-
-class BuiltinModels(OrderedDict):
-    model: models.Model = None
-    model_unique_kwargs = []
-
-    def init_object(self, obj: models.Model):
-        kwargs = {
-            key: getattr(obj, key) for key in self.model_unique_kwargs
-        }
-        defaults = {
-            filed.name: getattr(obj, filed.name) for filed in obj._meta.fields if filed.name not in kwargs
-        }
-        current = self.model.objects.get_or_create(
-            defaults=defaults, **kwargs
-        )[0]
-        for field in obj._meta.fields:
-            setattr(obj, field.name, getattr(current, field.name))
-        return obj
-
-    def initialize(self):
-        for k, v in self.__dict__.items():
-            if isinstance(v, self.model):
-                obj = self.init_object(v)
-                self.add(obj, k)
-
-    def add(self, obj: models.Model, key=None):
-        if key:
-            self[key] = obj
-
-    def delete(self, obj, key):
-        if key:
-            self.pop(key, None)
-
-
-class BuiltinCallbacks(BuiltinModels):
-    model = TaskScheduleCallback
-    model_unique_kwargs = ['name']
-
-    def __init__(self, user):
-        self.http_log_upload = self.model(
-            name='Http日志上报',
-            trigger_event=TaskCallbackEvent.DONE,
-            status=TaskCallbackStatus.ENABLE.value,
-            user=user,
-        )
-        super(BuiltinCallbacks, self).__init__()
-
-    def init_object(self, obj: models.Model):
-        super(BuiltinCallbacks, self).init_object(obj)
-        
-    def initialize(self):
-        super(BuiltinCallbacks, self).initialize()
-
-
-class BaseBuiltinQueues(BuiltinModels):
-
-    status_params_mapping = {
-        TaskScheduleStatus.OPENING.value: 'opening',
-        TaskScheduleStatus.CLOSED.value: 'closed',
-        TaskScheduleStatus.TEST.value: 'test',
-        TaskScheduleStatus.DONE.value: 'done',
-        TaskScheduleStatus.ERROR.value: 'error',
-    }
-
-    model_unique_kwargs = ['code']
-
-    def __init__(self):
-        super(BaseBuiltinQueues, self).__init__()
-        for m in self.model.objects.filter(status=True):
-            self.add(m)
-
-    def add(self, instance: AbstractTaskScheduleQueue, key=None):
-        if instance.status:
-            old = self.get(instance.code)
-            if not old or old.module != instance.module or old.config != instance.config:
-                instance.queue = import_string(instance.module)(**instance.config)
-                self[instance.code] = instance
-        elif not instance.status:
-            self.pop(instance.code, None)
-
-    def delete(self, instance: AbstractTaskScheduleQueue, key=None):
-        self.pop(instance.code, None)
-
-
-class BuiltinQueues(BaseBuiltinQueues):
-    model = TaskScheduleQueue
-
-    def __init__(self):
-        self.opening = self.model(
-            code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
-            status=True,
-            module=ScheduleQueueModule.QUEUE.value,
-            name='已启用任务'
-        )
-        self.test = self.model(
-            code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
-            status=True,
-            module=ScheduleQueueModule.QUEUE.value,
-            name='测试任务'
-        )
-        super(BuiltinQueues, self).__init__()
-
-
-class BaseBuiltinProducers(BuiltinModels):
-    model_unique_kwargs = ['queue']
-
-    def __init__(self):
-        super(BaseBuiltinProducers, self).__init__()
-        for m in self.model.objects.filter(status=True):
-            self.add(m)
-
-    def add(self, instance: AbstractTaskScheduleProducer, key=None):
-        if instance.status:
-            old = self.get(instance.id)
-            if not old or old.queue != instance.queue:
-                self[instance.id] = instance
-        elif not instance.status:
-            self.pop(instance.id, None)
-
-    def delete(self, instance: AbstractTaskScheduleProducer, key=None):
-        self.pop(instance.id, None)
-
-
-class BuiltinProducers(BaseBuiltinProducers):
-    model = TaskScheduleProducer
-
-    def __init__(self, queues: BuiltinQueues):
-        self.opening = self.model(
-            queue=queues.opening,
-            lte_now=True,
-            filters={
-                'status': TaskScheduleStatus.OPENING.value,
-            },
-            status=True,
-            name='默认'
-        )
-        self.test = self.model(
-            queue=queues.test,
-            lte_now=True,
-            filters={
-                'status': TaskScheduleStatus.TEST.value,
-            },
-            status=True,
-            name='测试'
-        )
-        super(BuiltinProducers, self).__init__()
-
-
-class BaseConsumerPermissions(BuiltinModels):
-    model = ConsumerPermission
-    model_unique_kwargs = ['producer', 'type']
-
-    def __init__(self):
-        super(BaseConsumerPermissions, self).__init__()
-        for m in self.model.objects.filter(status=True):
-            self.add(m)
-
-    def add(self, instance: AbstractConsumerPermission, key=None):
-        if instance.status:
-            old = self.get(instance.producer_id)
-            if not old or old.type != instance.type or old.config != instance.config:
-                validator = ConsumerPermissionValidator.get(instance.type)
-                if validator:
-                    self[instance.producer.queue.code] = validator(instance.config)
-        elif not instance.status:
-            self.pop(instance.producer.queue.code, None)
-
-    def delete(self, instance: AbstractConsumerPermission, key=None):
-        self.pop(instance.producer.queue.code, None)
-
-
-class BuiltinConsumerPermissions(BaseConsumerPermissions):
-    model = ConsumerPermission
-
-
-class BaseBuiltins:
-
-    app = None
-
-    def __init__(self):
-        self._initialized = False
-        self.user = UserModel(username='系统', is_superuser=True)
-
-    def init_user(self):
-        user = UserModel.objects.filter(is_superuser=True).order_by('id').first()
-        if not user:
-            raise Exception('请先创建超级用户')
-        for field in user._meta.fields:
-            setattr(self.user, field.name, getattr(user, field.name))
-
-    def initialize(self):
-        if not self._initialized:
-            self._initialized = True
-            if os.environ.get('RUN_MAIN') == 'true' and os.environ.get('RUN_CLIENT') != 'true':
-                from django.conf import settings
-                if self.app in settings.INSTALLED_APPS:
-                    print('[%s]初始化内置任务' % self.app)
-                    self.init_user()
-                    for i in self.__dict__.values():
-                        if isinstance(i, BuiltinModels):
-                            i.initialize()
-                    system_initialize_signal.send(sender='builtin_initialized', app=self.app)
-
-
-class Builtins(BaseBuiltins):
-
-    app = 'django_common_task_system'
-
-    def __init__(self):
-        super(Builtins, self).__init__()
-        self.queues = BuiltinQueues()
-        self.callbacks = BuiltinCallbacks(self.user)
-        self.producers = BuiltinProducers(self.queues)
-        self.consumer_permissions = BuiltinConsumerPermissions()
-
-
-builtins = Builtins()
+from django.utils import timezone
+from django.contrib.auth import get_user_model
+from django.db import models
+from django.utils.module_loading import import_string
+from .choices import TaskStatus, TaskScheduleStatus, TaskScheduleType, TaskCallbackStatus, \
+    TaskCallbackEvent, ScheduleTimingType, ScheduleQueueModule, ConsumerPermissionType
+from django_common_objects.models import CommonTag, CommonCategory, get_default_config
+from django_common_objects import fields as common_fields
+from .utils.cron_utils import get_next_cron_time
+from .utils import foreign_key
+from datetime import datetime, timedelta
+from . import fields
+from jionlp_time import parse_time
+from .utils.schedule_time import nlp_config_to_schedule_config
+from . import settings
+from . permissions import ConsumerPermissionValidator
+import re
+import os
+from django.core.validators import ValidationError
+from django.dispatch import Signal, receiver
+from threading import Event
+from collections import OrderedDict
+
+system_initialize_signal = Signal()
+system_schedule_event = Event()
+system_signal_sent = False
+
+mdays = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+
+
+UserModel = get_user_model()
+
+is_task_initialized = 'django_common_task_system' in settings.INSTALLED_APPS
+is_system_task_initialized = 'django_common_system_task.system_task' in settings.INSTALLED_APPS
+
+
+@receiver(system_initialize_signal, sender='builtin_initialized')
+def on_builtin_initialized(sender, app=None, **kwargs):
+    global is_task_initialized, is_system_task_initialized, system_signal_sent
+    if app == 'django_common_task_system':
+        is_task_initialized = True
+    elif app == 'django_common_task_system.system_task':
+        is_system_task_initialized = True
+    # 加入system_signal_sent判断, 防止重复发送信号
+    if is_task_initialized and is_system_task_initialized and not system_signal_sent:
+        from threading import Timer
+
+        def send_signal():
+            system_initialize_signal.send(sender='system_initialized')
+        # 这里django_common_task_system和django_common_system_task都初始化完成了, 但是其他app还未
+        # 完成初始化, 所以这里延迟一段时间再发送信号
+        system_signal_sent = True
+        Timer(2, send_signal).start()
+
+
+def code_validator(value):
+    if re.match(r'[a-zA-Z_-]+', value) is None:
+        raise ValidationError('编码只能包含字母、数字、下划线和中划线')
+
+
+class AbstractTask(models.Model):
+    id = models.AutoField(primary_key=True)
+    parent = models.ForeignKey('self', db_constraint=False, on_delete=models.DO_NOTHING,
+                               null=True, blank=True, verbose_name='父任务')
+    name = models.CharField(max_length=100, verbose_name='任务名')
+    category = models.ForeignKey(CommonCategory, db_constraint=False, on_delete=models.DO_NOTHING, verbose_name='类别')
+    tags = models.ManyToManyField(CommonTag, blank=True, db_constraint=False, verbose_name='标签')
+    description = models.TextField(blank=True, null=True, verbose_name='描述')
+    config = common_fields.ConfigField(default=get_default_config('Task'),
+                                       blank=True, null=True, verbose_name='参数')
+    status = common_fields.CharField(max_length=1, default=TaskStatus.ENABLE.value, verbose_name='状态',
+                                     choices=TaskStatus.choices)
+    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    @property
+    def associated_tasks_ids(self):
+        return foreign_key.get_related_object_ids(self)
+
+    class Meta:
+        db_table = 'taskhub'
+        verbose_name = verbose_name_plural = '任务中心'
+        unique_together = ('name', 'user', 'parent')
+        abstract = True
+
+    def __str__(self):
+        return self.name
+
+    __repr__ = __str__
+
+
+class Task(AbstractTask):
+
+    class Meta(AbstractTask.Meta):
+        swappable = 'TASK_MODEL'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractScheduleCallback(models.Model):
+    id = models.AutoField(primary_key=True)
+    name = models.CharField(max_length=100, verbose_name='回调')
+    description = models.TextField(blank=True, null=True, verbose_name='描述')
+    trigger_event = common_fields.CharField(default=TaskCallbackEvent.DONE, choices=TaskCallbackEvent.choices,
+                                            verbose_name='触发事件')
+    status = common_fields.CharField(default=TaskCallbackStatus.ENABLE.value, verbose_name='状态',
+                                     choices=TaskCallbackStatus.choices)
+    config = common_fields.ConfigField(default=get_default_config('TaskCallback'), blank=True, null=True,
+                                       verbose_name='参数')
+    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    class Meta:
+        db_table = 'task_schedule_callback'
+        verbose_name = verbose_name_plural = '任务回调'
+        unique_together = ('name', 'user')
+        abstract = True
+
+    def __str__(self):
+        return self.name
+
+    __repr__ = __str__
+
+
+class TaskScheduleCallback(AbstractScheduleCallback):
+    class Meta(AbstractScheduleCallback.Meta):
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class ScheduleConfig:
+
+    def __init__(self,
+                 base_on_now=True,
+                 nlp_sentence=None,
+                 schedule_type=None,
+                 crontab=None,
+                 period_schedule=None,
+                 once_schedule=None,
+                 timing_type=None,
+                 timing_period=None,
+                 timing_time=None,
+                 timing_weekday=None,
+                 timing_monthday=None,
+                 timing_year=None,
+                 timing_datetime=None,
+                 config=None,
+                 **kwargs):
+        self.base_on_now = base_on_now
+        self.nlp_sentence = nlp_sentence
+        self.schedule_type = schedule_type
+        self.once_schedule = once_schedule
+        self.period_schedule = period_schedule
+        self.crontab = crontab
+        self.timing_type = timing_type
+        self.timing_period = timing_period
+        self.timing_time = timing_time
+        self.timing_weekday = timing_weekday
+        self.timing_monthday = timing_monthday
+        self.timing_year = timing_year
+        self.timing_datetime = timing_datetime
+        self.kwargs = kwargs
+        self.config = config or self.to_config()
+        if config:
+            self.parse_config(config)
+
+    def parse_config(self, config):
+        schedule_type = self.schedule_type = config['schedule_type']
+        self.base_on_now = config.get('base_on_now', False)
+        type_config = config[schedule_type]
+        if schedule_type == TaskScheduleType.ONCE:
+            self.once_schedule = type_config['schedule_start_time']
+        elif schedule_type == TaskScheduleType.CRONTAB:
+            self.crontab = type_config['crontab']
+        elif schedule_type == TaskScheduleType.CONTINUOUS:
+            self.period_schedule = [
+                type_config["schedule_start_time"],
+                type_config["period"]
+            ]
+        elif schedule_type == TaskScheduleType.TIMINGS:
+            timing_type = self.timing_type = type_config["type"]
+            self.timing_time = datetime.strptime(type_config["time"], '%H:%M:%S')
+            timing_config = type_config[timing_type]
+            self.timing_period = timing_config.get('period')
+            if timing_type == ScheduleTimingType.DAY:
+                pass
+            elif timing_type == ScheduleTimingType.WEEKDAY:
+                self.timing_monthday = timing_config['weekday']
+            elif timing_type == ScheduleTimingType.MONTHDAY:
+                self.timing_monthday = timing_config['monthday']
+            elif timing_type == ScheduleTimingType.YEAR:
+                self.timing_year = timing_config['year']
+
+    def to_config(self):
+        if self.nlp_sentence:
+            result = parse_time(self.nlp_sentence)
+            config = nlp_config_to_schedule_config(result, sentence=self.nlp_sentence)
+            self.schedule_type = config['schedule_type']
+            return config
+        config = {
+            'schedule_type': self.schedule_type,
+            'base_on_now': self.base_on_now,
+        }
+        schedule_type = self.schedule_type
+        type_config: dict = config.setdefault(self.schedule_type, {})
+        if schedule_type == TaskScheduleType.CRONTAB:
+            if not self.crontab:
+                raise ValidationError('crontab is required while type is crontab')
+            type_config['crontab'] = self.crontab
+        elif schedule_type == TaskScheduleType.CONTINUOUS:
+            if not self.period_schedule:
+                raise ValidationError("period_schedule is required while type is continuous")
+            schedule_time, period = self.period_schedule
+            if period == 0:
+                raise ValidationError("period can't be 0 while type is continuous")
+            type_config['period'] = period
+            type_config['schedule_start_time'] = schedule_time
+        elif schedule_type == TaskScheduleType.ONCE:
+            type_config['schedule_start_time'] = self.once_schedule
+        elif schedule_type == TaskScheduleType.TIMINGS:
+            timing_type = self.timing_type
+            type_config['time'] = self.timing_time.strftime('%H:%M:%S')
+            type_config['type'] = timing_type
+            timing_config = type_config.setdefault(timing_type, {})
+            if timing_type == ScheduleTimingType.DAY:
+                if self.timing_period == 0:
+                    raise ValidationError("period can't be 0 while type is timing")
+                timing_config['period'] = self.timing_period
+            elif timing_type == ScheduleTimingType.WEEKDAY:
+                if not self.timing_weekday:
+                    raise ValidationError("weekdays is required while type is timing")
+                timing_config['period'] = self.timing_period
+                timing_config['weekday'] = self.timing_weekday
+            elif timing_type == ScheduleTimingType.MONTHDAY:
+                timing_config['period'] = self.timing_period
+                timing_config['monthday'] = self.timing_monthday
+            elif timing_type == ScheduleTimingType.YEAR:
+                timing_config['period'] = self.timing_period
+                timing_config['year'] = self.timing_year
+            elif timing_type == ScheduleTimingType.DATETIME:
+                timing_config['datetime'] = self.timing_datetime
+            else:
+                raise ValidationError("timing_type is invalid")
+        else:
+            raise ValidationError("type<%s> is invalid" % schedule_type)
+        return config
+
+    def get_current_time(self, start_time=None):
+        if self.base_on_now:
+            now = datetime.now()
+        else:
+            if start_time and start_time != datetime.min:
+                now = datetime.fromtimestamp(start_time.timestamp())
+            else:
+                now = datetime.now()
+        now_seconds = now.hour * 3600 + now.minute * 60 + now.second
+        schedule_type = self.schedule_type
+        type_config = self.config[schedule_type]
+        schedule_time = None
+        if schedule_type == TaskScheduleType.CONTINUOUS.value:
+            schedule_time, period = self.period_schedule
+            while schedule_time < now:
+                schedule_time += timedelta(seconds=period)
+        elif schedule_type == TaskScheduleType.CRONTAB.value:
+            schedule_time = get_next_cron_time(type_config['crontab'], now)
+        elif schedule_type == TaskScheduleType.TIMINGS:
+            timing_type = type_config['type']
+            hour, minute, second = type_config['time'].split(':')
+            hour, minute, second = int(hour), int(minute), int(second)
+            timing_config = type_config[timing_type]
+            if timing_type == ScheduleTimingType.DAY:
+                schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
+                while schedule_time < now:
+                    schedule_time += timedelta(days=timing_config['period'])
+            elif timing_type == ScheduleTimingType.WEEKDAY:
+                weekdays = timing_config['weekday']
+                weekday = now.isoweekday()
+                schedule_again = weekday not in weekdays
+                if not schedule_again:
+                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
+                    if now > schedule_time:
+                        schedule_again = True
+                if schedule_again:
+                    for i in weekdays:
+                        if i > weekday:
+                            days = i - weekday
+                            delta = timedelta(days=days)
+                            break
+                    else:
+                        days = weekday - weekdays[0]
+                        delta = timedelta(days=timing_config['period'] * 7 - days)
+                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second) + delta
+            elif timing_type == ScheduleTimingType.MONTHDAY:
+                monthdays = timing_config['monthday']
+                if not monthdays:
+                    raise ValidationError("monthdays is required while type is timing-monthday")
+                schedule_again = now.day not in monthdays
+                if not schedule_again:
+                    schedule_time = datetime(now.year, now.month, now.day, hour, minute, second)
+                    if now > schedule_time:
+                        schedule_again = True
+                if schedule_again:
+                    def next_month(y, m):
+                        if m == 12:
+                            return y + 1, 1
+                        else:
+                            return y, m + 1
+                    for i in monthdays:
+                        if i == 0:
+                            i = 1
+                        elif i == 32:
+                            i = mdays[now.month]
+                        if i > now.day:
+                            schedule_time = datetime(now.year, now.month, i, hour, minute, second)
+                            break
+                    else:
+                        year, month = next_month(now.year, now.month)
+                        schedule_time = datetime(year, month, monthdays[0], hour, minute, second)
+            elif timing_type == ScheduleTimingType.YEAR:
+                month_days = timing_config['year']
+                if not month_days:
+                    raise ValidationError("year month day is required while type is timing-datetime")
+                month, day = 1, 1
+                for i in month_days.split(","):
+                    month, day = i.split('-')
+                    month, day = int(month), int(day)
+                    d = datetime(now.year, month, day, hour, minute, second)
+                    if d > now:
+                        schedule_time = d
+                        break
+                else:
+                    schedule_time = datetime(now.year + timing_config['period'], month, day, hour, minute, second)
+            elif timing_type == ScheduleTimingType.DATETIME:
+                dates, t = timing_config['datetime']
+                if not dates:
+                    raise ValidationError("datetime is required while type is timing-datetime")
+                if t:
+                    t: datetime.time
+                    seconds = t.hour * 3600 + t.minute * 60 + t.second
+                else:
+                    seconds = 0
+                for i in dates.split(','):
+                    d = datetime.strptime(i, '%Y-%m-%d')
+                    if d > now or (d == now and seconds >= now_seconds):
+                        break
+                else:
+                    raise ValidationError("cant find a datetime after now")
+                schedule_time = datetime(d.year, d.month, d.day, t.hour, t.minute, t.second)
+            else:
+                raise ValidationError('unsupported timing_type<%s>' % timing_type)
+        elif schedule_type == TaskScheduleType.ONCE:
+            schedule_time = type_config['schedule_start_time']
+        else:
+            raise ValidationError("type<%s> is invalid" % schedule_type)
+        if isinstance(schedule_time, str):
+            schedule_time = datetime.strptime(schedule_time, '%Y-%m-%d %H:%M:%S')
+        # if schedule_time < now:
+        #     raise ValidationError("cant create a schedule time before now, schedule_time<%s>" % schedule_time)
+        return schedule_time
+
+    def get_next_time(self, last_time: datetime):
+        schedule_type = self.schedule_type
+        type_config = self.config[schedule_type]
+        if self.base_on_now:
+            last_time = datetime.now()
+        next_time = last_time
+        if schedule_type == TaskScheduleType.CONTINUOUS.value:
+            while next_time <= last_time:
+                next_time += timedelta(seconds=self.period_schedule[1])
+        elif schedule_type == TaskScheduleType.CRONTAB.value:
+            next_time = get_next_cron_time(type_config['crontab'], last_time)
+        elif schedule_type == TaskScheduleType.TIMINGS:
+            timing_type = type_config['type']
+            hour, minute, second = type_config['time'].split(':')
+            hour, minute, second = int(hour), int(minute), int(second)
+            timing_config = type_config[timing_type]
+            timing_period = timing_config.get('period', 1)
+            next_time = datetime(next_time.year, next_time.month, next_time.day, hour, minute, second)
+            if timing_type == ScheduleTimingType.DAY:
+                while next_time <= last_time:
+                    next_time += timedelta(days=timing_period)
+            elif timing_type == ScheduleTimingType.WEEKDAY:
+                weekdays = timing_config['weekday']
+                weekday = last_time.isoweekday()
+                for i in weekdays:
+                    if i > weekday:
+                        days = i - weekday
+                        delta = timedelta(days=days)
+                        break
+                else:
+                    days = weekday - weekdays[0]
+                    delta = timedelta(days=timing_period * 7 - days)
+                next_time = next_time + delta
+            elif timing_type == ScheduleTimingType.MONTHDAY:
+                monthdays = timing_config['monthday']
+                day = 1
+                for day in monthdays:
+                    if day == 0:
+                        day = 1
+                    elif day == 32:
+                        day = mdays[last_time.month]
+                    next_time = datetime(last_time.year, last_time.month, day, hour, minute, second)
+                    if next_time > last_time:
+                        break
+                else:
+                    month = (last_time.month + timing_period) % 12
+                    if month == 0:
+                        month = 1
+                    year = last_time.year + (last_time.month + timing_period) // 12
+                    next_time = datetime(year, month, day, hour, minute, second)
+            elif timing_type == ScheduleTimingType.YEAR:
+                month_days = timing_config['year']
+                if not month_days:
+                    raise ValidationError("year month day is required while type is timing-datetime")
+                month, day = 1, 1
+                for i in month_days.split(","):
+                    month, day = i.split('-')
+                    month, day = int(month), int(day)
+                    next_time = datetime(last_time.year, month, day, hour, minute, second)
+                    if next_time > last_time:
+                        break
+                else:
+                    next_time = datetime(last_time.year + timing_period, month, day, hour, minute, second)
+            else:
+                raise ValidationError("unsupported timing type: %s" % schedule_type)
+        elif schedule_type == TaskScheduleType.ONCE:
+            next_time = datetime.max
+        else:
+            raise ValidationError("unsupported schedule type: %s" % schedule_type)
+        return next_time
+
+
+class AbstractTaskSchedule(models.Model):
+    id = models.AutoField(primary_key=True)
+    task = models.ForeignKey(settings.TASK_MODEL, on_delete=models.CASCADE, db_constraint=False, verbose_name='任务')
+    priority = models.IntegerField(default=0, verbose_name='优先级')
+    next_schedule_time = models.DateTimeField(default=timezone.now, verbose_name='下次运行时间', db_index=True)
+    schedule_start_time = models.DateTimeField(default=datetime.min, verbose_name='开始时间')
+    schedule_end_time = models.DateTimeField(default=datetime.max, verbose_name='结束时间')
+    config = fields.ScheduleConfigField(default=dict, verbose_name='参数')
+    status = common_fields.CharField(default=TaskScheduleStatus.OPENING.value, verbose_name='状态',
+                                     choices=TaskScheduleStatus.choices)
+    callback = models.ForeignKey(TaskScheduleCallback, on_delete=models.CASCADE,
+                                 null=True, blank=True, db_constraint=False, verbose_name='回调')
+    user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    def generate_next_schedule(self):
+        try:
+            self.next_schedule_time = ScheduleConfig(config=self.config).get_next_time(self.next_schedule_time)
+        except Exception as e:
+            self.status = TaskScheduleStatus.ERROR.value
+            self.save(update_fields=('status',))
+            raise e
+        if self.next_schedule_time > self.schedule_end_time:
+            self.next_schedule_time = datetime.max
+            self.status = TaskScheduleStatus.DONE.value
+        self.save(update_fields=('next_schedule_time', 'status'))
+        return self
+
+    class Meta:
+        db_table = 'task_schedule'
+        verbose_name = verbose_name_plural = '任务计划'
+        ordering = ('-priority', 'next_schedule_time')
+        unique_together = ('task', 'status', 'user')
+        abstract = True
+
+    def __str__(self):
+        return self.task.name
+
+    __repr__ = __str__
+
+    def __lt__(self, other):
+        return self.priority < other.priority
+
+    def __gt__(self, other):
+        return self.priority > other.priority
+
+
+class TaskSchedule(AbstractTaskSchedule):
+    class Meta(AbstractTaskSchedule.Meta):
+        swappable = 'TASK_SCHEDULE_MODEL'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractTaskScheduleQueue(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    name = models.CharField(max_length=100, verbose_name='队列名称', unique=True)
+    code = models.CharField(max_length=100, verbose_name='队列编码', unique=True, validators=[code_validator])
+    status = models.BooleanField(default=True, verbose_name='状态')
+    module = models.CharField(max_length=100, verbose_name='队列类型',
+                              default=ScheduleQueueModule.QUEUE,
+                              choices=ScheduleQueueModule.choices)
+    config = models.JSONField(default=dict, verbose_name='配置', null=True, blank=True)
+    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    class Meta:
+        verbose_name = verbose_name_plural = '任务队列'
+        abstract = True
+
+    def __str__(self):
+        return "%s(%s)" % (self.name, self.code)
+
+
+class TaskScheduleQueue(AbstractTaskScheduleQueue):
+    class Meta(AbstractTaskScheduleQueue.Meta):
+        db_table = 'task_schedule_queue'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractTaskScheduleProducer(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    name = models.CharField(max_length=100, verbose_name='生产名称')
+    filters = models.JSONField(verbose_name='过滤器')
+    lte_now = models.BooleanField(default=True, verbose_name='小于等于当前时间')
+    queue = models.ForeignKey(TaskScheduleQueue, db_constraint=False, related_name='producers',
+                              on_delete=models.CASCADE, verbose_name='队列')
+    status = models.BooleanField(default=True, verbose_name='启用状态')
+    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    class Meta:
+        verbose_name = verbose_name_plural = '计划生产'
+        abstract = True
+
+    def __str__(self):
+        return self.name
+
+
+class TaskScheduleProducer(AbstractTaskScheduleProducer):
+    class Meta(AbstractTaskScheduleProducer.Meta):
+        db_table = 'task_schedule_producer'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractTaskScheduleLog(models.Model):
+    id = models.AutoField(primary_key=True)
+    schedule = models.ForeignKey(TaskSchedule, db_constraint=False, on_delete=models.CASCADE, verbose_name='任务计划')
+    status = common_fields.CharField(verbose_name='运行状态')
+    queue = models.CharField(max_length=100, verbose_name='队列', default='opening')
+    result = common_fields.ConfigField(blank=True, null=True, verbose_name='结果')
+    schedule_time = models.DateTimeField(verbose_name='计划时间')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+
+    class Meta:
+        db_table = 'task_schedule_log'
+        verbose_name = verbose_name_plural = '任务日志'
+        ordering = ('-create_time',)
+        abstract = True
+
+    def __str__(self):
+        return "schedule: %s, status: %s" % (self.schedule, self.status)
+
+    __repr__ = __str__
+
+
+class TaskScheduleLog(AbstractTaskScheduleLog):
+    schedule = models.ForeignKey(TaskSchedule, db_constraint=False, related_name='logs',
+                                 on_delete=models.CASCADE, verbose_name='任务计划')
+
+    class Meta(AbstractTaskScheduleLog.Meta):
+        swappable = 'TASK_SCHEDULE_LOG_MODEL'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractConsumerPermission(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    producer = models.ForeignKey(TaskScheduleProducer, db_constraint=False,
+                                 on_delete=models.CASCADE, verbose_name='生产者')
+    type = models.CharField(max_length=1, verbose_name='类型',
+                            default=ConsumerPermissionType.IP_WHITE_LIST,
+                            choices=ConsumerPermissionType.choices)
+    status = models.BooleanField(default=True, verbose_name='启用状态')
+    config = models.JSONField(default=dict, verbose_name='配置', null=True, blank=True)
+    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    class Meta:
+        verbose_name = verbose_name_plural = '消费权限'
+        unique_together = ('producer', 'status')
+        abstract = True
+
+    def __str__(self):
+        return self.producer.name
+
+    __repr__ = __str__
+
+
+class ConsumerPermission(AbstractConsumerPermission):
+    class Meta(AbstractConsumerPermission.Meta):
+        db_table = 'schedule_consumer_permission'
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class AbstractExceptionReport(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    ip = models.CharField(max_length=100, verbose_name='IP')
+    content = models.TextField(verbose_name='内容')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+
+    class Meta:
+        db_table = 'task_exception_report'
+        verbose_name = verbose_name_plural = '异常报告'
+        ordering = ('-create_time',)
+        abstract = True
+
+    def __str__(self):
+        return "Exception(%s, %s)" % (self.ip, self.content[:50])
+
+    __repr__ = __str__
+
+
+class ExceptionReport(AbstractExceptionReport):
+    class Meta(AbstractExceptionReport.Meta):
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
+class BuiltinModels(OrderedDict):
+    model: models.Model = None
+    model_unique_kwargs = []
+
+    def init_object(self, obj: models.Model):
+        kwargs = {
+            key: getattr(obj, key) for key in self.model_unique_kwargs
+        }
+        defaults = {
+            filed.name: getattr(obj, filed.name) for filed in obj._meta.fields if filed.name not in kwargs
+        }
+        current = self.model.objects.get_or_create(
+            defaults=defaults, **kwargs
+        )[0]
+        for field in obj._meta.fields:
+            setattr(obj, field.name, getattr(current, field.name))
+        return obj
+
+    def initialize(self):
+        for k, v in self.__dict__.items():
+            if isinstance(v, self.model):
+                obj = self.init_object(v)
+                self.add(obj, k)
+
+    def add(self, obj: models.Model, key=None):
+        if key:
+            self[key] = obj
+
+    def delete(self, obj, key):
+        if key:
+            self.pop(key, None)
+
+
+class BuiltinCallbacks(BuiltinModels):
+    model = TaskScheduleCallback
+    model_unique_kwargs = ['name']
+
+    def __init__(self, user):
+        self.http_log_upload = self.model(
+            name='Http日志上报',
+            trigger_event=TaskCallbackEvent.DONE,
+            status=TaskCallbackStatus.ENABLE.value,
+            user=user,
+        )
+        super(BuiltinCallbacks, self).__init__()
+
+    def init_object(self, obj: models.Model):
+        super(BuiltinCallbacks, self).init_object(obj)
+        
+    def initialize(self):
+        super(BuiltinCallbacks, self).initialize()
+
+
+class BaseBuiltinQueues(BuiltinModels):
+
+    status_params_mapping = {
+        TaskScheduleStatus.OPENING.value: 'opening',
+        TaskScheduleStatus.CLOSED.value: 'closed',
+        TaskScheduleStatus.TEST.value: 'test',
+        TaskScheduleStatus.DONE.value: 'done',
+        TaskScheduleStatus.ERROR.value: 'error',
+    }
+
+    model_unique_kwargs = ['code']
+
+    def __init__(self):
+        super(BaseBuiltinQueues, self).__init__()
+        for m in self.model.objects.filter(status=True):
+            self.add(m)
+
+    def add(self, instance: AbstractTaskScheduleQueue, key=None):
+        if instance.status:
+            old = self.get(instance.code)
+            if not old or old.module != instance.module or old.config != instance.config:
+                instance.queue = import_string(instance.module)(**instance.config)
+                self[instance.code] = instance
+        elif not instance.status:
+            self.pop(instance.code, None)
+
+    def delete(self, instance: AbstractTaskScheduleQueue, key=None):
+        self.pop(instance.code, None)
+
+
+class BuiltinQueues(BaseBuiltinQueues):
+    model = TaskScheduleQueue
+
+    def __init__(self):
+        self.opening = self.model(
+            code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='已启用任务'
+        )
+        self.test = self.model(
+            code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='测试任务'
+        )
+        super(BuiltinQueues, self).__init__()
+
+
+class BaseBuiltinProducers(BuiltinModels):
+    model_unique_kwargs = ['queue']
+
+    def __init__(self):
+        super(BaseBuiltinProducers, self).__init__()
+        for m in self.model.objects.filter(status=True):
+            self.add(m)
+
+    def add(self, instance: AbstractTaskScheduleProducer, key=None):
+        if instance.status:
+            old = self.get(instance.id)
+            if not old or old.queue != instance.queue:
+                self[instance.id] = instance
+        elif not instance.status:
+            self.pop(instance.id, None)
+
+    def delete(self, instance: AbstractTaskScheduleProducer, key=None):
+        self.pop(instance.id, None)
+
+
+class BuiltinProducers(BaseBuiltinProducers):
+    model = TaskScheduleProducer
+
+    def __init__(self, queues: BuiltinQueues):
+        self.opening = self.model(
+            queue=queues.opening,
+            lte_now=True,
+            filters={
+                'status': TaskScheduleStatus.OPENING.value,
+            },
+            status=True,
+            name='默认'
+        )
+        self.test = self.model(
+            queue=queues.test,
+            lte_now=True,
+            filters={
+                'status': TaskScheduleStatus.TEST.value,
+            },
+            status=True,
+            name='测试'
+        )
+        super(BuiltinProducers, self).__init__()
+
+
+class BaseConsumerPermissions(BuiltinModels):
+    model = ConsumerPermission
+    model_unique_kwargs = ['producer', 'type']
+
+    def __init__(self):
+        super(BaseConsumerPermissions, self).__init__()
+        for m in self.model.objects.filter(status=True):
+            self.add(m)
+
+    def add(self, instance: AbstractConsumerPermission, key=None):
+        if instance.status:
+            old = self.get(instance.producer_id)
+            if not old or old.type != instance.type or old.config != instance.config:
+                validator = ConsumerPermissionValidator.get(instance.type)
+                if validator:
+                    self[instance.producer.queue.code] = validator(instance.config)
+        elif not instance.status:
+            self.pop(instance.producer.queue.code, None)
+
+    def delete(self, instance: AbstractConsumerPermission, key=None):
+        self.pop(instance.producer.queue.code, None)
+
+
+class BuiltinConsumerPermissions(BaseConsumerPermissions):
+    model = ConsumerPermission
+
+
+class BaseBuiltins:
+
+    app = None
+
+    def __init__(self):
+        self._initialized = False
+        self.user = UserModel(username='系统', is_superuser=True)
+
+    def init_user(self):
+        user = UserModel.objects.filter(is_superuser=True).order_by('id').first()
+        if not user:
+            raise Exception('请先创建超级用户')
+        for field in user._meta.fields:
+            setattr(self.user, field.name, getattr(user, field.name))
+
+    def initialize(self):
+        if not self._initialized:
+            self._initialized = True
+            if os.environ.get('RUN_MAIN') == 'true' and os.environ.get('RUN_CLIENT') != 'true':
+                from django.conf import settings
+                if self.app in settings.INSTALLED_APPS:
+                    print('[%s]初始化内置任务' % self.app)
+                    self.init_user()
+                    for i in self.__dict__.values():
+                        if isinstance(i, BuiltinModels):
+                            i.initialize()
+                    system_initialize_signal.send(sender='builtin_initialized', app=self.app)
+
+
+class Builtins(BaseBuiltins):
+
+    app = 'django_common_task_system'
+
+    def __init__(self):
+        super(Builtins, self).__init__()
+        self.queues = BuiltinQueues()
+        self.callbacks = BuiltinCallbacks(self.user)
+        self.producers = BuiltinProducers(self.queues)
+        self.consumer_permissions = BuiltinConsumerPermissions()
+
+
+builtins = Builtins()
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/serializers.py` & `django-common-task-system-1.2.6/django_common_task_system/serializers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-from . import models
-from django_common_objects.serializers import CommonCategorySerializer, CommonTagSerializer
-from rest_framework import serializers
-from . import get_task_model, get_schedule_log_model
-
-
-TaskModel = get_task_model()
-TaskScheduleLogModel = get_schedule_log_model()
-
-
-class TaskSerializer(serializers.ModelSerializer):
-    category = CommonCategorySerializer()
-    tags = CommonTagSerializer(many=True)
-    parent = serializers.SerializerMethodField()
-
-    def get_parent(self, obj):
-        if obj.parent:
-            return self.__class__(obj.parent).data
-
-    class Meta:
-        model = TaskModel
-        exclude = ('update_time', )
-
-
-class QueueTaskSerializer(TaskSerializer):
-    tags = None
-
-    class Meta:
-        model = TaskModel
-        # fields = ('id', 'name', 'config', 'category', 'status', 'parent', )
-        exclude = ('user', 'update_time', 'description', 'create_time')
-
-
-class TaskCallbackSerializer(serializers.ModelSerializer):
-
-    class Meta:
-        model = models.TaskScheduleCallback
-        exclude = ('update_time', )
-
-
-class TaskScheduleSerializer(serializers.ModelSerializer):
-    task = TaskSerializer()
-    callback = TaskCallbackSerializer()
-
-    class Meta:
-        model = models.TaskSchedule
-        exclude = ('update_time', )
-
-
-class QueueScheduleSerializer(TaskScheduleSerializer):
-    task = QueueTaskSerializer()
-    callback = TaskCallbackSerializer()
-    schedule_time = serializers.DateTimeField(source="next_schedule_time")
-
-    class Meta:
-        model = models.TaskSchedule
-        # fields = ('id', 'task', 'schedule_time', 'update_time', 'callback', 'user')
-        exclude = ('priority', 'create_time', 'next_schedule_time', 'schedule_start_time',
-                   'schedule_end_time', 'status', 'config')
-
-
-class TaskScheduleLogSerializer(serializers.ModelSerializer):
-    schedule = serializers.PrimaryKeyRelatedField(queryset=models.TaskSchedule.objects.all())
-
-    class Meta:
-        model = TaskScheduleLogModel
-        fields = '__all__'
-
-
-class ExceptionSerializer(serializers.ModelSerializer):
-    ip = serializers.ReadOnlyField()
-
-    class Meta:
-        model = models.ExceptionReport
-        fields = '__all__'
+from . import models
+from django_common_objects.serializers import CommonCategorySerializer, CommonTagSerializer
+from rest_framework import serializers
+from . import get_task_model, get_schedule_log_model
+
+
+TaskModel = get_task_model()
+TaskScheduleLogModel = get_schedule_log_model()
+
+
+class TaskSerializer(serializers.ModelSerializer):
+    category = CommonCategorySerializer()
+    tags = CommonTagSerializer(many=True)
+    parent = serializers.SerializerMethodField()
+
+    def get_parent(self, obj):
+        if obj.parent:
+            return self.__class__(obj.parent).data
+
+    class Meta:
+        model = TaskModel
+        exclude = ('update_time', )
+
+
+class QueueTaskSerializer(TaskSerializer):
+    tags = None
+
+    class Meta:
+        model = TaskModel
+        # fields = ('id', 'name', 'config', 'category', 'status', 'parent', )
+        exclude = ('user', 'update_time', 'description', 'create_time')
+
+
+class TaskCallbackSerializer(serializers.ModelSerializer):
+
+    class Meta:
+        model = models.TaskScheduleCallback
+        exclude = ('update_time', )
+
+
+class TaskScheduleSerializer(serializers.ModelSerializer):
+    task = TaskSerializer()
+    callback = TaskCallbackSerializer()
+
+    class Meta:
+        model = models.TaskSchedule
+        exclude = ('update_time', )
+
+
+class QueueScheduleSerializer(TaskScheduleSerializer):
+    task = QueueTaskSerializer()
+    callback = TaskCallbackSerializer()
+    schedule_time = serializers.DateTimeField(source="next_schedule_time")
+    generator = serializers.SerializerMethodField()
+
+    @staticmethod
+    def get_generator(obj):
+        return getattr(obj, 'generator', 'auto')
+
+    class Meta:
+        model = models.TaskSchedule
+        # fields = ('id', 'task', 'schedule_time', 'update_time', 'callback', 'user')
+        exclude = ('priority', 'create_time', 'next_schedule_time', 'schedule_start_time',
+                   'schedule_end_time', 'status', 'config')
+
+
+class TaskScheduleLogSerializer(serializers.ModelSerializer):
+    schedule = serializers.PrimaryKeyRelatedField(queryset=models.TaskSchedule.objects.all())
+
+    class Meta:
+        model = TaskScheduleLogModel
+        fields = '__all__'
+
+
+class ExceptionSerializer(serializers.ModelSerializer):
+    ip = serializers.ReadOnlyField()
+
+    class Meta:
+        model = models.ExceptionReport
+        fields = '__all__'
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-.ui-calendar { border: 1px solid #ccc; background-color: #f9f9f9; position: absolute; color: #666; font-family: arial, 'Hiragino Sans GB', sans-serif; position: absolute; }
-.ui-calendar ul { list-style: none; overflow: hidden; margin: 0; padding: 0; background-color: #fff; width: 210px; }
-.ui-calendar li { list-style: none; float: left; width: 30px; height: 26px; line-height: 26px; text-align: center; cursor: pointer; }
-.ui-calendar li:hover, .ui-calendar-pannel span:hover ,.ui-calendar-toolbar a:hover{ background-color: #f2f2f2; }
-.ui-calendar-pannel span { cursor: pointer; display: block; float: left; width: 30px; text-align: center; height: 30px; line-height: 30px; }
-.ui-calendar-pannel .month, .ui-calendar-pannel .year { width: 40px; }
-.ui-calendar-pannel .month { width: 50px; }
-.ui-calendar-toolbar { border-top:1px solid #ccc;}
-.ui-month-list,.ui-year-list{display: none; position:absolute;top:30px;left: -1px;height:176px;width: 100%;background-color: #fff;border:1px solid #ccc;}
-.ui-month-list .current,.ui-year-list .current{background-color: #f2f2f2;}
-.ui-month-list div,.ui-year-list div{cursor: pointer;float: left;width:25%;height:33.33%;line-height:3;overflow:hidden;box-sizing:border-box;text-align: center;display: table-cell;vertical-align: middle;border:none;}
-.ui-month-list div:hover,.ui-year-list div:hover{background-color: #f2f2f2;}
-.ui-calendar-toolbar a {cursor: pointer; display: inline-block; height: 30px; line-height: 30px; width:51px; text-align: center; border-right: 1px solid #ccc; }
-.ui-calendar-toolbar a.ui-calendar-close { border-right-width: 0; }
-.ui-calendar-time{margin: 0 auto;text-align: center;padding:3px;}
-.ui-calendar-time a{display: inline-block;padding:2px 3px;cursor: pointer;}
-.preday, .nextday,.prevtenyear,.nexttenyear { color: #999; }
-.calendar-header { }
-.calendar-header b { width: 30px; float: left; display: block; text-align: center; }
-.ui-calendar li.focus { background-color: #288df0; color: #FFF; }
-.ui-calendar li.disabled { background-color: #ccc; }
-.clearfix:after { display: block; height: 0; clear: both; visibility: hidden; content: '.'; zoom:1;}
+.ui-calendar { border: 1px solid #ccc; background-color: #f9f9f9; position: absolute; color: #666; font-family: arial, 'Hiragino Sans GB', sans-serif; position: absolute; }
+.ui-calendar ul { list-style: none; overflow: hidden; margin: 0; padding: 0; background-color: #fff; width: 210px; }
+.ui-calendar li { list-style: none; float: left; width: 30px; height: 26px; line-height: 26px; text-align: center; cursor: pointer; }
+.ui-calendar li:hover, .ui-calendar-pannel span:hover ,.ui-calendar-toolbar a:hover{ background-color: #f2f2f2; }
+.ui-calendar-pannel span { cursor: pointer; display: block; float: left; width: 30px; text-align: center; height: 30px; line-height: 30px; }
+.ui-calendar-pannel .month, .ui-calendar-pannel .year { width: 40px; }
+.ui-calendar-pannel .month { width: 50px; }
+.ui-calendar-toolbar { border-top:1px solid #ccc;}
+.ui-month-list,.ui-year-list{display: none; position:absolute;top:30px;left: -1px;height:176px;width: 100%;background-color: #fff;border:1px solid #ccc;}
+.ui-month-list .current,.ui-year-list .current{background-color: #f2f2f2;}
+.ui-month-list div,.ui-year-list div{cursor: pointer;float: left;width:25%;height:33.33%;line-height:3;overflow:hidden;box-sizing:border-box;text-align: center;display: table-cell;vertical-align: middle;border:none;}
+.ui-month-list div:hover,.ui-year-list div:hover{background-color: #f2f2f2;}
+.ui-calendar-toolbar a {cursor: pointer; display: inline-block; height: 30px; line-height: 30px; width:51px; text-align: center; border-right: 1px solid #ccc; }
+.ui-calendar-toolbar a.ui-calendar-close { border-right-width: 0; }
+.ui-calendar-time{margin: 0 auto;text-align: center;padding:3px;}
+.ui-calendar-time a{display: inline-block;padding:2px 3px;cursor: pointer;}
+.preday, .nextday,.prevtenyear,.nexttenyear { color: #999; }
+.calendar-header { }
+.calendar-header b { width: 30px; float: left; display: block; text-align: center; }
+.ui-calendar li.focus { background-color: #288df0; color: #FFF; }
+.ui-calendar li.disabled { background-color: #ccc; }
+.clearfix:after { display: block; height: 0; clear: both; visibility: hidden; content: '.'; zoom:1;}
 .clearfix { display: block;zoom:1; }
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,592 +1,592 @@
-/*
- * Created with vs code.
- * github: https://github.com/tianxiangbing/calendar   记得加星星
- * demo地址: http://www.lovewebgames.com/jsmodule/index.html
- * User: 田想兵
- * Date: 2015-03-09
- * Time: 17:02:02
- * Contact: 55342775@qq.com
- * Desc: 确保代码最新及时修复bug，请去github上下载最新源码 https://github.com/tianxiangbing/calendar
- */
-;
-(function(root, factory) {
-    //amd
-    if (typeof define === 'function' && define.amd) {
-        define(['$'], factory);
-    } else if (typeof exports === 'object') { //umd
-        module.exports = factory();
-    } else {
-        root.CustomCalendar = factory(window.Zepto || window.jQuery || $);
-    }
-})(this, function($) {
-    $.fn.CustomCalendar = function(settings) {
-        var list = [];
-        $(this).each(function() {
-            var calendar = new CustomCalendar();
-            var options = $.extend({
-                target: $(this)
-            }, settings);
-            calendar.init(options);
-            list.push(calendar);
-        });
-        return list;
-    };
-    var CustomCalendar = function() {
-        this.monthArr = ["一月", "二月", "三月", "四月", "五月", "六月", "七月", "八月", "九月", "十月", "十一月", "十二月"];
-        this.dayArr = ['日', '一', '二', '三', '四', '五', '六'];
-        var rnd = Math.random().toString().replace('.', '');
-        this.id = 'calendar_' + rnd;
-        this.calendarContainer;
-        this.settings = {
-            goCallback: function() {}
-        };
-        this.isShow = false;
-        this.autohide = true;
-        this.toolbarTpl = '<div class="ui-calendar-toolbar clearfix"><a class="js-calendar-submit">确定</a><a class="js-clear">清空</a><a class="ui-calendar-today">现在</a><a class="ui-calendar-close">关闭</a></div>';
-        this.timeTpl = '<div class="ui-calendar-time clearfix"><select class="js-calendar-hours">时</select>:<select class="js-calendar-minutes">分</select><s>:</s><select class="js-calendar-second">秒</select></div>';
-        this.dateArr = [];
-        this.maxDays = 9999;
-    };
-    CustomCalendar.prototype = {
-        separator: '-',
-        defaultDate: new Date(),
-        setRange: function(range) {
-            this.range = $.extend([null, null], range);
-        },
-        getDefaultDate: function() {
-            var _this = this;
-            if (this.settings.target && $(this.settings.target).length) {
-                if ($(this.settings.target)[0].nodeType === 1) {
-                    this.settings.focusDate = $(this.settings.target).val() || this.settings.focusDate || '';
-                } else {
-                    this.settings.focusDate = $(this.settings.target).prev().val() || this.settings.focusDate || '';
-                }
-                if (this.settings.onlyYM && $(this.settings.target).val()) {
-                    this.settings.focusDate = $(this.settings.target).val() + this.separator + "01";
-                }
-            }
-            if (this.settings.focusDate && !this.settings.multiple) {
-                var focusDateArr = this.settings.focusDate.split(' ')[0].split(this.separator);
-                var t = this.settings.focusDate.split(' ')[1] || "00:00:00";
-                this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
-            }
-            if (this.settings.focusDate && this.settings.multiple) {
-                var arr = this.settings.focusDate.split(',');
-                this.dateArr = [];
-                for (var i = arr.length - 1; i >= 0; i--) {
-                    var item = arr[i];
-                    var focusDateArr = item.split(this.separator);
-                    this.dateArr.push(new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]));
-                };
-                this.defaultDate = this.dateArr[0];
-                if (!_this._dateInArr(_this.defaultDate, _this.dateArr)) {
-                    _this.dateArr.push(_this.date);
-                }
-            }
-        },
-        init: function(settings) {
-            $('body').append('<div class="ui-calendar clearfix" id="' + this.id + '"><div class="ui-calendar-pannel clearfix" data-role="pannel"><span class="ui-calendar-control" data-role="prev-year">&lt;&lt;</span><span class="ui-calendar-control" data-role="prev-month">&lt;</span><span class="ui-calendar-control month" data-role="current-month"></span><span class="ui-calendar-control year" data-role="current-year"></span><span class="ui-calendar-control" data-role="next-month">&gt;</span><span class="ui-calendar-control" data-role="next-year">&gt;&gt;</span></div><div class="calendar-header clearfix"></div><div class="c_days clearfix"></div></div>');
-            this.calendarContainer = $('#' + this.id);
-            var _this = this;
-            this.settings = $.extend({}, this.settings, settings);
-            this.maxDays = this.settings.maxdays || this.maxDays;
-            this.mutilSeparator = this.settings.mutilSeparator || ",";
-            $(this.settings.target).attr('readonly', 'readonly');
-            this.getDefaultDate();
-            if (this.settings.multiple) {
-                this.settings.toolbar = true;
-            }
-            var zIndex = this.settings.zIndex || 1;
-            this.calendarContainer.css('zIndex', zIndex);
-            this.date = this.defaultDate;
-            this.setRange(this.settings.range);
-            if (this.settings.time) {
-                this.settings.toolbar = true;
-                this.autohide = false;
-                this.showTime();
-                this.showToolbar();
-            }
-            if (this.settings.toolbar) {
-                this.autohide = false;
-                this.showToolbar();
-            }
-            // this.formatDate();
-            // this.renderHeader();
-            this.bindEvent();
-            if (this.settings.target) {
-                this.hide();
-            } else {
-                this.autohide = false;
-                this.show();
-            }
-        },
-        showToolbar: function() {
-            if (this.settings.toolbar && $('.ui-calendar-toolbar', this.calendarContainer).length == 0) {
-                this.calendarContainer.append(this.toolbarTpl);
-            }
-        },
-        showTime: function() {
-            if (this.calendarContainer.find('.ui-calendar-time').length == 0) {
-                this.calendarContainer.append(this.timeTpl);
-            }
-            var _this = this;
-            $('.js-calendar-minutes', this.calendarContainer).html('');
-            $('.js-calendar-second', this.calendarContainer).html('');
-            for (var i = 0, l = 60; i < l; i++) {
-                if (i < 24) {
-                    $('.js-calendar-hours', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
-                }
-                $('.js-calendar-minutes', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
-                $('.js-calendar-second', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
-            }
-            var value = this.date;
-            var t = _this._getTowNum(value.getHours()) + ":" + _this._getTowNum(value.getMinutes()) + ":" + _this._getTowNum(value.getSeconds());
-            $('.js-calendar-hours', this.calendarContainer).val(_this._getTowNum(value.getHours()));
-            $('.js-calendar-minutes', this.calendarContainer).val(_this._getTowNum(value.getMinutes()));
-            $('.js-calendar-second', this.calendarContainer).val(_this._getTowNum(value.getSeconds()));
-            if (_this.settings.onlyHm) {
-                $('.js-calendar-second', this.calendarContainer).hide().val('00').prev().hide();
-            }
-        },
-        show: function() {
-            this.getDefaultDate();
-            this.calendarContainer.show();
-            this.date = this.defaultDate;
-            this.formatDate();
-            this.renderHeader();
-            this.isShow = true;
-            this.setPosition();
-            this.settings.show && this.settings.show(this.calendarContainer);
-            var _this = this;
-            this.timer = setInterval(function() {
-                _this.setPosition.call(_this);
-            }, 500);
-            if (this.settings.time) {
-                this.settings.toolbar = true;
-                this.autohide = false;
-                this.showTime();
-            }
-            if (this.settings.onlyYM) {
-                this.settings.toolbar = false;
-                $('[data-role="current-month"]', this.calendarContainer).trigger('click');
-                $('.ui-month-list', this.calendarContainer).show();
-                $('.c_days', this.calendarContainer).hide();
-            }
-        },
-        hide: function() {
-            this.calendarContainer.hide();
-            this.isShow = false;
-            this.settings.hide && this.settings.hide(this.calendarContainer);
-            clearInterval(this.timer);
-        },
-        setPosition: function() {
-            var x = 0,
-                y = 0;
-            if (this.settings.target && $(this.settings.target).length) {
-                if ($(this.settings.target)[0].nodeType === 1) {
-                    y = $(this.settings.target).offset().top + $(this.settings.target).outerHeight();
-                    x = $(this.settings.target).offset().left;
-                } else {
-                    y = $(this.settings.target).prev().offset().top + $(this.settings.target).prev().outerHeight();
-                    x = $(this.settings.target).prev().offset().left;
-                }
-                var st = $(window).scrollTop();
-                var winY = $(window).height();
-                if (y + this.calendarContainer.outerHeight() > st + winY) {
-                    var tmp = y - this.calendarContainer.outerHeight() - $(this.settings.target).outerHeight();
-                    if (tmp > 0) {
-                        y = tmp;
-                    }
-                }
-                this.calendarContainer.css({
-                    top: y,
-                    left: x
-                });
-            }
-        },
-        setDate: function(value) {
-            var _this = this,
-                v;
-            if (typeof value === "object") {
-                _this.defaultDate = value;
-                v = value.getFullYear() + _this.separator + _this._getTowNum((value.getMonth() + 1)) + _this.separator + _this._getTowNum(value.getDate());
-                if (_this.settings.time) {
-                    v += " " + _this._getTowNum(value.getHours()) + ":" + _this._getTowNum(value.getMinutes()) + ":" + _this._getTowNum(value.getSeconds());
-                }
-            } else {
-                var a = value.split(' ');
-                var d = a[0];
-                var t = a[1] || "00:00:00";
-                var focusDateArr = d.split(_this.separator);
-                _this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
-                v = value;
-            }
-            _this.date = _this.defaultDate;
-            return v;
-        },
-        bindEvent: function() {
-            var _this = this;
-            $('.ui-calendar-control[data-role]', _this.calendarContainer).click(function() {
-                _this.go[$(this).data('role')].call(_this);
-                return false;
-            })
-            $(_this.calendarContainer).click(function() {
-                return false;
-            });
-            $('.c_days', _this.calendarContainer).delegate('li', 'click', function() {
-                _this.settings.beforeSelect && _this.settings.beforeSelect(_this.date, _this.calendarContainer);
-                if ($(this).hasClass('disabled')) {
-                    return false;
-                };
-                var value = $(this).data('value');
-                _this.setDate(value);
-                if (_this.settings.multiple) {
-                    if (!$(this).hasClass('focus')) {
-                        if (_this.maxDays <= _this.dateArr.length) {
-                            //alert('添加已达上限 ' + _this.maxDays + ' 天');
-                            _this.settings.overdays && _this.settings.overdays(_this.maxDays, _this.dateArr, _this.calendarContainer);
-                            return false;
-                        }
-                        _this.dateArr.push(_this.defaultDate);
-                    } else {
-                        _this._removeDate(_this.defaultDate, _this.dateArr);
-                    }
-                } else {
-                    _this.dateArr = [_this.date];
-                }
-                _this.formatDate();
-                _this.renderHeader();
-                _this.settings.selected && _this.settings.selected.call(_this, _this.date, _this.calendarContainer);
-                if (_this.settings.target && $(_this.settings.target).length && $(_this.settings.target)[0].nodeType === 1 && _this.autohide) {
-                    $(_this.settings.target).val(value);
-                    _this.hide();
-                    _this.settings.afterSelected && _this.settings.afterSelected.call(_this, $(_this.settings.target), _this.date, _this.calendarContainer);
-                }
-                return false;
-            });
-            $('.ui-calendar-toolbar', _this.calendarContainer).delegate('a', 'click', function() {
-                if ($(this).hasClass('js-calendar-submit')) { //点确定
-                    _this.settings.selected && _this.settings.selected.call(_this, _this.dateArr, _this.calendarContainer);
-                    if (_this.dateArr.length === 0) {
-                        _this.dateArr.push($('.focus', _this.calendarContainer).data('value'));
-                    }
-                    var arr = _this._toString(_this.dateArr);
-                    value = arr.join(_this.mutilSeparator);
-                    if (_this.settings.time) {
-                        value += " " + $('.js-calendar-hours', _this.calendarContainer).val() + ":" + $('.js-calendar-minutes', _this.calendarContainer).val() + ":" + $('.js-calendar-second', _this.calendarContainer).val()
-                    }
-                    $(_this.settings.target).val(value);
-                    _this.hide();
-                }
-                if ($(this).hasClass('ui-calendar-close')) {
-                    _this.hide();
-                }
-                if ($(this).hasClass('ui-calendar-today')) { //点现在
-                    var now = new Date();
-                    var value = _this.setDate(now);
-                    _this.date = now;
-                    _this.hide();
-                    $(_this.settings.target).val(value);
-                }
-                if ($(this).hasClass('js-clear')) {
-                    _this.dateArr = [];
-                    _this.settings.focusDate = '';
-                    _this.date = null;
-                    $(_this.settings.target).val('');
-                    _this.formatDate();
-                }
-                var value = $(_this.settings.target).val();
-                var currentValue = new Date(value)
-                if (_this.settings.time && currentValue) {
-                    //时间时，判断
-                    var start = _this.range[0],
-                        startDate,
-                        end = _this.range[1],
-                        endDate;
-                    if (start) {
-                        start = +new Date(Date.parse(start));
-                    };
-                    if (end) {
-                        end = +new Date(Date.parse(end));
-                    }
-                    if ((currentValue < start && start) || (currentValue > end && end)) {
-                        _this.date = null;
-                        $(_this.settings.target).val('');
-                        alert('所选日期超出限定范围内');
-                    }
-                }
-                _this.settings.afterSelected && _this.settings.afterSelected.call(_this, $(_this.settings.target), _this.date, _this.calendarContainer);
-            });
-            if (_this.settings.target) {
-                $(_this.settings.target).bind('click', function() {
-                    if ($(this).hasClass('disabled') || $(this).filter('[disabled="true"]').length > 0) {
-                        return;
-                    }
-                    $(document).trigger('click');
-                    _this.show();
-                    return false;
-                });
-                $(document).click(function() {
-                    _this.isShow && _this.hide()
-                })
-            }
-            $(document).keydown(function(e) {
-                if (e.keyCode === 27) {
-                    _this.hide();
-                }
-            });
-        },
-        actionFlow: function(obj, action) {
-            if (obj.siblings('.ui-calendar-flow').length) {
-                obj.siblings('.ui-calendar-flow').hide(300, function() {
-                    obj[action](300);
-                });
-            } else {
-                obj[action](300);
-            }
-        },
-        go: {
-            'next-month': function() {
-                this.month += 1;
-                this.day = 1;
-                this._getDate();
-                this.formatDate();
-                this.renderHeader();
-                this.settings.goCallback.call(this, 'next-month', this.date);
-            },
-            'prev-month': function() {
-                this.month -= 1;
-                this.day = 1;
-                this.changeDate();
-                this.settings.goCallback.call(this, 'prev-month', this.date);
-            },
-            'next-year': function() {
-                this.day = 1;
-                this.year += 1;
-                this.changeDate();
-                this.settings.goCallback.call(this, 'next-year', this.date);
-            },
-            'prev-year': function() {
-                this.day = 1;
-                this.year -= 1;
-                this.changeDate();
-                this.settings.goCallback.call(this, 'prev-year', this.date);
-            },
-            'current-year': function(show) {
-                var _this = this;
-                if (!this.yearContainer) {
-                    this.yearContainer = $('<div class="ui-year-list ui-calendar-flow"/>');
-                    this.calendarContainer.append(this.yearContainer);
-                    _this.actionFlow(_this.yearContainer, 'show');
-                    this.yearContainer.on('click', 'div', function() {
-                        var index = $(this).data('value');
-                        _this.year = index;
-                        _this.changeDate();
-                        if (!$(this).hasClass('cross')) {
-                            _this.actionFlow(_this.yearContainer, 'hide');
-                            if (_this.settings.onlyYM) {
-                                _this.actionFlow(_this.monthContainer, 'show');
-                            }
-                        } else {
-                            _this.go['current-year'].call(_this, true);
-                        }
-                    });
-                } else {
-                    if (!show) {
-                        _this.actionFlow(_this.yearContainer, 'toggle');
-                    }
-                }
-                var yearTen = Math.floor(_this.year / 10);
-                this.yearContainer.html('');
-                this.yearContainer.append('<div class="cross prevtenyear" data-value="' + ((yearTen - 1).toString() + 9) + '">...</div>');
-                for (var i = 0, l = 10; i < l; i++) {
-                    var y = yearTen.toString() + i;
-                    var cls = '';
-                    if (_this.year == y) {
-                        cls = ' class="current" ';
-                    }
-                    this.yearContainer.append('<div ' + cls + ' data-value="' + y + '">' + y + '</div>');
-                };
-                this.yearContainer.append('<div class="cross nexttenyear" data-value="' + ((yearTen + 1).toString() + 0) + '">...</div>');
-                this.settings.goCallback.call(this, 'current-year', this.date);
-            },
-            'current-month': function() {
-                var _this = this;
-                if (!this.monthContainer) {
-                    this.monthContainer = $('<div class="ui-month-list ui-calendar-flow"/>');
-                    this.calendarContainer.append(this.monthContainer);
-                    if (!_this.settings.onlyYM) {
-                        _this.actionFlow(_this.monthContainer, 'show');
-                    }
-                    this.monthContainer.on('click', 'div', function() {
-                        var index = $(this).data('value');
-                        _this.month = index;
-                        _this.day = 1;
-                        _this.changeDate();
-                        if (!_this.settings.onlyYM) {
-                            _this.monthContainer.hide(300);
-                        } else {
-                            $(_this.settings.target).val(_this.year.toString() + _this.separator + (_this.month + 1));
-                            _this.hide();
-                            _this.settings.selected && _this.settings.selected.call(_this, _this.date, _this.calendarContainer);
-                        }
-                    });
-                } else if (!this.settings.onlyYM) {
-                    _this.actionFlow(_this.monthContainer, 'toggle');
-                } else {
-                    _this.actionFlow(_this.monthContainer, 'show');
-                }
-                this.monthContainer.html('');
-                for (var i = 0, l = this.monthArr.length; i < l; i++) {
-                    var m = this.monthArr[i];
-                    var cls = '';
-                    if (_this.month == i) {
-                        cls = ' class="current" ';
-                    }
-                    this.monthContainer.append('<div ' + cls + ' data-value="' + i + '">' + m + '</div>');
-                };
-                this.settings.goCallback && this.settings.goCallback.call(this, 'current-month', this.date);
-            }
-        },
-        changeDate: function() {
-            this._getDate();
-            this.formatDate();
-            this.renderHeader();
-        },
-        renderHeader: function() {
-            $('[data-role="current-month"]', this.calendarContainer).html(this.monthArr[this.month])
-            $('[data-role="current-year"]', this.calendarContainer).html(this.year);
-            var daylist = '';
-            for (var i = 0, l = this.dayArr.length; i < l; i++) {
-                daylist += '<b>' + this.dayArr[i] + '</b>';
-            };
-            if (!this.settings.onlyYM) {
-                $('.calendar-header', this.calendarContainer).html(daylist);
-            }
-        },
-        _getDate: function() {
-            this.date = new Date(this.year, this.month, this.day);
-        },
-        formatDate: function() {
-            var date = this.date || this.defaultDate;
-            this.year = date.getFullYear();
-            this.month = date.getMonth();
-            this.day = date.getDate();
-            var ndate = new Date(this.year, this.month + 1, 0);
-            var dayNum = ndate.getDate();
-            var list = '<ul>';
-            var firstDay = (new Date(this.year, this.month, 1)).getDay();
-            var preDate = new Date(this.year, this.month, 0);
-            var preDateNum = preDate.getDate();
-            var nextDate = new Date(this.year, this.month + 2, 0);
-            if (firstDay > 0) {
-                list += this._getDay(preDateNum - firstDay + 1, preDateNum, "preday", preDate);
-            }
-            list += this._getDay(1, dayNum, '', date);
-            var lastDay = (new Date(this.year, this.month, dayNum)).getDay();
-            list += this._getDay(1, 6 - lastDay, "nextday", nextDate);
-            list += '</ul>';
-            $('#' + this.id).find(".c_days").html(list);
-        },
-        _toString: function(dateArr) {
-            var arr = [];
-            var len = dateArr.length;
-            for (var i = 0; i < len; i++) {
-                var item = dateArr[i];
-                if (typeof item === "string") {
-                    dateArr[i] = new Date(item);
-                };
-                for (var j = 0; j < i; j++) {
-                    if (item.getTime() < dateArr[j]) {
-                        var tmp = dateArr[i];
-                        dateArr[i] = dateArr[j];
-                        dateArr[j] = tmp;
-                    }
-                }
-            };
-            for (var i = 0, l = dateArr.length; i < l; i++) {
-                var d = dateArr[i];
-                var year = d.getFullYear();
-                var month = this._getTowNum(d.getMonth() + 1);
-                var day = this._getTowNum(d.getDate());
-                arr.push(year + this.separator + month + this.separator + day);
-            }
-            return arr;
-        },
-        _getDay: function(startNum, dayNum, cls, date) {
-            var list = '';
-            var start = this.range[0],
-                startDate,
-                end = this.range[1],
-                endDate;
-            if (start) {
-                start = new Date(Date.parse(start));
-                startDate = +new Date(start.getFullYear(), start.getMonth(), start.getDate());
-            };
-            if (end) {
-                end = new Date(Date.parse(end));
-                endDate = +new Date(end.getFullYear(), end.getMonth(), end.getDate());
-            }
-            for (var i = startNum; i <= dayNum; i++) {
-                var className = cls || "";
-                var datavalue = date.getFullYear() + this.separator + this._getTowNum(date.getMonth() + 1) + this.separator;
-                datavalue += this._getTowNum(i);
-                var d = new Date(date.getFullYear(), date.getMonth(), i);
-                var time = d.getTime();
-                //多选
-                //console.log(this.dateArr)
-                if (this.settings.multiple) {
-                    if (this._dateInArr(d, this.dateArr)) {
-                        className += ' focus';
-                    }
-                } else
-                if (time == +new Date(this.defaultDate.getFullYear(), this.defaultDate.getMonth(), this.defaultDate.getDate())) {
-                    className += ' focus';
-                }
-                if ((startDate && time < startDate) || (endDate && time > endDate)) {
-                    className += " disabled";
-                }
-                if (this.settings.filter && !this.settings.filter(time)) {
-                    className += " disabled";
-                }
-                list += '<li class="' + className + '" data-value="' + datavalue + '">' + i + '</li>';
-            };
-            return list;
-        },
-        _dateInArr: function(date, arr) {
-            for (var i = arr.length - 1; i >= 0; i--) {
-                var item = arr[i];
-                var idate = item;
-                if (typeof item === "string") {
-                    var focusDateArr = item.split(this.separator);
-                    idate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]);
-                }
-                if (date.getTime() == idate.getTime()) {
-                    return true;
-                    break;
-                }
-            };
-        },
-        _removeDate: function(date, arr) {
-            var newArr = [];
-            for (var i = arr.length - 1; i >= 0; i--) {
-                var item = arr[i];
-                var idate = item;
-                if (typeof item === "string") {
-                    var focusDateArr = item.split(this.separator);
-                    idate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]);
-                }
-                if (date.getTime() == idate.getTime()) {
-                    continue;
-                }
-                newArr.push(idate);
-            };
-            this.dateArr = newArr;
-        },
-        _getTowNum: function(n) {
-            var num = '0' + n.toString();
-            return num.length == 2 ? num : num.substr(1, 2);
-        }
-    };
-    return CustomCalendar;
+/*
+ * Created with vs code.
+ * github: https://github.com/tianxiangbing/calendar   记得加星星
+ * demo地址: http://www.lovewebgames.com/jsmodule/index.html
+ * User: 田想兵
+ * Date: 2015-03-09
+ * Time: 17:02:02
+ * Contact: 55342775@qq.com
+ * Desc: 确保代码最新及时修复bug，请去github上下载最新源码 https://github.com/tianxiangbing/calendar
+ */
+;
+(function(root, factory) {
+    //amd
+    if (typeof define === 'function' && define.amd) {
+        define(['$'], factory);
+    } else if (typeof exports === 'object') { //umd
+        module.exports = factory();
+    } else {
+        root.CustomCalendar = factory(window.Zepto || window.jQuery || $);
+    }
+})(this, function($) {
+    $.fn.CustomCalendar = function(settings) {
+        var list = [];
+        $(this).each(function() {
+            var calendar = new CustomCalendar();
+            var options = $.extend({
+                target: $(this)
+            }, settings);
+            calendar.init(options);
+            list.push(calendar);
+        });
+        return list;
+    };
+    var CustomCalendar = function() {
+        this.monthArr = ["一月", "二月", "三月", "四月", "五月", "六月", "七月", "八月", "九月", "十月", "十一月", "十二月"];
+        this.dayArr = ['日', '一', '二', '三', '四', '五', '六'];
+        var rnd = Math.random().toString().replace('.', '');
+        this.id = 'calendar_' + rnd;
+        this.calendarContainer;
+        this.settings = {
+            goCallback: function() {}
+        };
+        this.isShow = false;
+        this.autohide = true;
+        this.toolbarTpl = '<div class="ui-calendar-toolbar clearfix"><a class="js-calendar-submit">确定</a><a class="js-clear">清空</a><a class="ui-calendar-today">现在</a><a class="ui-calendar-close">关闭</a></div>';
+        this.timeTpl = '<div class="ui-calendar-time clearfix"><select class="js-calendar-hours">时</select>:<select class="js-calendar-minutes">分</select><s>:</s><select class="js-calendar-second">秒</select></div>';
+        this.dateArr = [];
+        this.maxDays = 9999;
+    };
+    CustomCalendar.prototype = {
+        separator: '-',
+        defaultDate: new Date(),
+        setRange: function(range) {
+            this.range = $.extend([null, null], range);
+        },
+        getDefaultDate: function() {
+            var _this = this;
+            if (this.settings.target && $(this.settings.target).length) {
+                if ($(this.settings.target)[0].nodeType === 1) {
+                    this.settings.focusDate = $(this.settings.target).val() || this.settings.focusDate || '';
+                } else {
+                    this.settings.focusDate = $(this.settings.target).prev().val() || this.settings.focusDate || '';
+                }
+                if (this.settings.onlyYM && $(this.settings.target).val()) {
+                    this.settings.focusDate = $(this.settings.target).val() + this.separator + "01";
+                }
+            }
+            if (this.settings.focusDate && !this.settings.multiple) {
+                var focusDateArr = this.settings.focusDate.split(' ')[0].split(this.separator);
+                var t = this.settings.focusDate.split(' ')[1] || "00:00:00";
+                this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
+            }
+            if (this.settings.focusDate && this.settings.multiple) {
+                var arr = this.settings.focusDate.split(',');
+                this.dateArr = [];
+                for (var i = arr.length - 1; i >= 0; i--) {
+                    var item = arr[i];
+                    var focusDateArr = item.split(this.separator);
+                    this.dateArr.push(new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]));
+                };
+                this.defaultDate = this.dateArr[0];
+                if (!_this._dateInArr(_this.defaultDate, _this.dateArr)) {
+                    _this.dateArr.push(_this.date);
+                }
+            }
+        },
+        init: function(settings) {
+            $('body').append('<div class="ui-calendar clearfix" id="' + this.id + '"><div class="ui-calendar-pannel clearfix" data-role="pannel"><span class="ui-calendar-control" data-role="prev-year">&lt;&lt;</span><span class="ui-calendar-control" data-role="prev-month">&lt;</span><span class="ui-calendar-control month" data-role="current-month"></span><span class="ui-calendar-control year" data-role="current-year"></span><span class="ui-calendar-control" data-role="next-month">&gt;</span><span class="ui-calendar-control" data-role="next-year">&gt;&gt;</span></div><div class="calendar-header clearfix"></div><div class="c_days clearfix"></div></div>');
+            this.calendarContainer = $('#' + this.id);
+            var _this = this;
+            this.settings = $.extend({}, this.settings, settings);
+            this.maxDays = this.settings.maxdays || this.maxDays;
+            this.mutilSeparator = this.settings.mutilSeparator || ",";
+            $(this.settings.target).attr('readonly', 'readonly');
+            this.getDefaultDate();
+            if (this.settings.multiple) {
+                this.settings.toolbar = true;
+            }
+            var zIndex = this.settings.zIndex || 1;
+            this.calendarContainer.css('zIndex', zIndex);
+            this.date = this.defaultDate;
+            this.setRange(this.settings.range);
+            if (this.settings.time) {
+                this.settings.toolbar = true;
+                this.autohide = false;
+                this.showTime();
+                this.showToolbar();
+            }
+            if (this.settings.toolbar) {
+                this.autohide = false;
+                this.showToolbar();
+            }
+            // this.formatDate();
+            // this.renderHeader();
+            this.bindEvent();
+            if (this.settings.target) {
+                this.hide();
+            } else {
+                this.autohide = false;
+                this.show();
+            }
+        },
+        showToolbar: function() {
+            if (this.settings.toolbar && $('.ui-calendar-toolbar', this.calendarContainer).length == 0) {
+                this.calendarContainer.append(this.toolbarTpl);
+            }
+        },
+        showTime: function() {
+            if (this.calendarContainer.find('.ui-calendar-time').length == 0) {
+                this.calendarContainer.append(this.timeTpl);
+            }
+            var _this = this;
+            $('.js-calendar-minutes', this.calendarContainer).html('');
+            $('.js-calendar-second', this.calendarContainer).html('');
+            for (var i = 0, l = 60; i < l; i++) {
+                if (i < 24) {
+                    $('.js-calendar-hours', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
+                }
+                $('.js-calendar-minutes', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
+                $('.js-calendar-second', this.calendarContainer).append('<option>' + _this._getTowNum(i) + '</option>');
+            }
+            var value = this.date;
+            var t = _this._getTowNum(value.getHours()) + ":" + _this._getTowNum(value.getMinutes()) + ":" + _this._getTowNum(value.getSeconds());
+            $('.js-calendar-hours', this.calendarContainer).val(_this._getTowNum(value.getHours()));
+            $('.js-calendar-minutes', this.calendarContainer).val(_this._getTowNum(value.getMinutes()));
+            $('.js-calendar-second', this.calendarContainer).val(_this._getTowNum(value.getSeconds()));
+            if (_this.settings.onlyHm) {
+                $('.js-calendar-second', this.calendarContainer).hide().val('00').prev().hide();
+            }
+        },
+        show: function() {
+            this.getDefaultDate();
+            this.calendarContainer.show();
+            this.date = this.defaultDate;
+            this.formatDate();
+            this.renderHeader();
+            this.isShow = true;
+            this.setPosition();
+            this.settings.show && this.settings.show(this.calendarContainer);
+            var _this = this;
+            this.timer = setInterval(function() {
+                _this.setPosition.call(_this);
+            }, 500);
+            if (this.settings.time) {
+                this.settings.toolbar = true;
+                this.autohide = false;
+                this.showTime();
+            }
+            if (this.settings.onlyYM) {
+                this.settings.toolbar = false;
+                $('[data-role="current-month"]', this.calendarContainer).trigger('click');
+                $('.ui-month-list', this.calendarContainer).show();
+                $('.c_days', this.calendarContainer).hide();
+            }
+        },
+        hide: function() {
+            this.calendarContainer.hide();
+            this.isShow = false;
+            this.settings.hide && this.settings.hide(this.calendarContainer);
+            clearInterval(this.timer);
+        },
+        setPosition: function() {
+            var x = 0,
+                y = 0;
+            if (this.settings.target && $(this.settings.target).length) {
+                if ($(this.settings.target)[0].nodeType === 1) {
+                    y = $(this.settings.target).offset().top + $(this.settings.target).outerHeight();
+                    x = $(this.settings.target).offset().left;
+                } else {
+                    y = $(this.settings.target).prev().offset().top + $(this.settings.target).prev().outerHeight();
+                    x = $(this.settings.target).prev().offset().left;
+                }
+                var st = $(window).scrollTop();
+                var winY = $(window).height();
+                if (y + this.calendarContainer.outerHeight() > st + winY) {
+                    var tmp = y - this.calendarContainer.outerHeight() - $(this.settings.target).outerHeight();
+                    if (tmp > 0) {
+                        y = tmp;
+                    }
+                }
+                this.calendarContainer.css({
+                    top: y,
+                    left: x
+                });
+            }
+        },
+        setDate: function(value) {
+            var _this = this,
+                v;
+            if (typeof value === "object") {
+                _this.defaultDate = value;
+                v = value.getFullYear() + _this.separator + _this._getTowNum((value.getMonth() + 1)) + _this.separator + _this._getTowNum(value.getDate());
+                if (_this.settings.time) {
+                    v += " " + _this._getTowNum(value.getHours()) + ":" + _this._getTowNum(value.getMinutes()) + ":" + _this._getTowNum(value.getSeconds());
+                }
+            } else {
+                var a = value.split(' ');
+                var d = a[0];
+                var t = a[1] || "00:00:00";
+                var focusDateArr = d.split(_this.separator);
+                _this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
+                v = value;
+            }
+            _this.date = _this.defaultDate;
+            return v;
+        },
+        bindEvent: function() {
+            var _this = this;
+            $('.ui-calendar-control[data-role]', _this.calendarContainer).click(function() {
+                _this.go[$(this).data('role')].call(_this);
+                return false;
+            })
+            $(_this.calendarContainer).click(function() {
+                return false;
+            });
+            $('.c_days', _this.calendarContainer).delegate('li', 'click', function() {
+                _this.settings.beforeSelect && _this.settings.beforeSelect(_this.date, _this.calendarContainer);
+                if ($(this).hasClass('disabled')) {
+                    return false;
+                };
+                var value = $(this).data('value');
+                _this.setDate(value);
+                if (_this.settings.multiple) {
+                    if (!$(this).hasClass('focus')) {
+                        if (_this.maxDays <= _this.dateArr.length) {
+                            //alert('添加已达上限 ' + _this.maxDays + ' 天');
+                            _this.settings.overdays && _this.settings.overdays(_this.maxDays, _this.dateArr, _this.calendarContainer);
+                            return false;
+                        }
+                        _this.dateArr.push(_this.defaultDate);
+                    } else {
+                        _this._removeDate(_this.defaultDate, _this.dateArr);
+                    }
+                } else {
+                    _this.dateArr = [_this.date];
+                }
+                _this.formatDate();
+                _this.renderHeader();
+                _this.settings.selected && _this.settings.selected.call(_this, _this.date, _this.calendarContainer);
+                if (_this.settings.target && $(_this.settings.target).length && $(_this.settings.target)[0].nodeType === 1 && _this.autohide) {
+                    $(_this.settings.target).val(value);
+                    _this.hide();
+                    _this.settings.afterSelected && _this.settings.afterSelected.call(_this, $(_this.settings.target), _this.date, _this.calendarContainer);
+                }
+                return false;
+            });
+            $('.ui-calendar-toolbar', _this.calendarContainer).delegate('a', 'click', function() {
+                if ($(this).hasClass('js-calendar-submit')) { //点确定
+                    _this.settings.selected && _this.settings.selected.call(_this, _this.dateArr, _this.calendarContainer);
+                    if (_this.dateArr.length === 0) {
+                        _this.dateArr.push($('.focus', _this.calendarContainer).data('value'));
+                    }
+                    var arr = _this._toString(_this.dateArr);
+                    value = arr.join(_this.mutilSeparator);
+                    if (_this.settings.time) {
+                        value += " " + $('.js-calendar-hours', _this.calendarContainer).val() + ":" + $('.js-calendar-minutes', _this.calendarContainer).val() + ":" + $('.js-calendar-second', _this.calendarContainer).val()
+                    }
+                    $(_this.settings.target).val(value);
+                    _this.hide();
+                }
+                if ($(this).hasClass('ui-calendar-close')) {
+                    _this.hide();
+                }
+                if ($(this).hasClass('ui-calendar-today')) { //点现在
+                    var now = new Date();
+                    var value = _this.setDate(now);
+                    _this.date = now;
+                    _this.hide();
+                    $(_this.settings.target).val(value);
+                }
+                if ($(this).hasClass('js-clear')) {
+                    _this.dateArr = [];
+                    _this.settings.focusDate = '';
+                    _this.date = null;
+                    $(_this.settings.target).val('');
+                    _this.formatDate();
+                }
+                var value = $(_this.settings.target).val();
+                var currentValue = new Date(value)
+                if (_this.settings.time && currentValue) {
+                    //时间时，判断
+                    var start = _this.range[0],
+                        startDate,
+                        end = _this.range[1],
+                        endDate;
+                    if (start) {
+                        start = +new Date(Date.parse(start));
+                    };
+                    if (end) {
+                        end = +new Date(Date.parse(end));
+                    }
+                    if ((currentValue < start && start) || (currentValue > end && end)) {
+                        _this.date = null;
+                        $(_this.settings.target).val('');
+                        alert('所选日期超出限定范围内');
+                    }
+                }
+                _this.settings.afterSelected && _this.settings.afterSelected.call(_this, $(_this.settings.target), _this.date, _this.calendarContainer);
+            });
+            if (_this.settings.target) {
+                $(_this.settings.target).bind('click', function() {
+                    if ($(this).hasClass('disabled') || $(this).filter('[disabled="true"]').length > 0) {
+                        return;
+                    }
+                    $(document).trigger('click');
+                    _this.show();
+                    return false;
+                });
+                $(document).click(function() {
+                    _this.isShow && _this.hide()
+                })
+            }
+            $(document).keydown(function(e) {
+                if (e.keyCode === 27) {
+                    _this.hide();
+                }
+            });
+        },
+        actionFlow: function(obj, action) {
+            if (obj.siblings('.ui-calendar-flow').length) {
+                obj.siblings('.ui-calendar-flow').hide(300, function() {
+                    obj[action](300);
+                });
+            } else {
+                obj[action](300);
+            }
+        },
+        go: {
+            'next-month': function() {
+                this.month += 1;
+                this.day = 1;
+                this._getDate();
+                this.formatDate();
+                this.renderHeader();
+                this.settings.goCallback.call(this, 'next-month', this.date);
+            },
+            'prev-month': function() {
+                this.month -= 1;
+                this.day = 1;
+                this.changeDate();
+                this.settings.goCallback.call(this, 'prev-month', this.date);
+            },
+            'next-year': function() {
+                this.day = 1;
+                this.year += 1;
+                this.changeDate();
+                this.settings.goCallback.call(this, 'next-year', this.date);
+            },
+            'prev-year': function() {
+                this.day = 1;
+                this.year -= 1;
+                this.changeDate();
+                this.settings.goCallback.call(this, 'prev-year', this.date);
+            },
+            'current-year': function(show) {
+                var _this = this;
+                if (!this.yearContainer) {
+                    this.yearContainer = $('<div class="ui-year-list ui-calendar-flow"/>');
+                    this.calendarContainer.append(this.yearContainer);
+                    _this.actionFlow(_this.yearContainer, 'show');
+                    this.yearContainer.on('click', 'div', function() {
+                        var index = $(this).data('value');
+                        _this.year = index;
+                        _this.changeDate();
+                        if (!$(this).hasClass('cross')) {
+                            _this.actionFlow(_this.yearContainer, 'hide');
+                            if (_this.settings.onlyYM) {
+                                _this.actionFlow(_this.monthContainer, 'show');
+                            }
+                        } else {
+                            _this.go['current-year'].call(_this, true);
+                        }
+                    });
+                } else {
+                    if (!show) {
+                        _this.actionFlow(_this.yearContainer, 'toggle');
+                    }
+                }
+                var yearTen = Math.floor(_this.year / 10);
+                this.yearContainer.html('');
+                this.yearContainer.append('<div class="cross prevtenyear" data-value="' + ((yearTen - 1).toString() + 9) + '">...</div>');
+                for (var i = 0, l = 10; i < l; i++) {
+                    var y = yearTen.toString() + i;
+                    var cls = '';
+                    if (_this.year == y) {
+                        cls = ' class="current" ';
+                    }
+                    this.yearContainer.append('<div ' + cls + ' data-value="' + y + '">' + y + '</div>');
+                };
+                this.yearContainer.append('<div class="cross nexttenyear" data-value="' + ((yearTen + 1).toString() + 0) + '">...</div>');
+                this.settings.goCallback.call(this, 'current-year', this.date);
+            },
+            'current-month': function() {
+                var _this = this;
+                if (!this.monthContainer) {
+                    this.monthContainer = $('<div class="ui-month-list ui-calendar-flow"/>');
+                    this.calendarContainer.append(this.monthContainer);
+                    if (!_this.settings.onlyYM) {
+                        _this.actionFlow(_this.monthContainer, 'show');
+                    }
+                    this.monthContainer.on('click', 'div', function() {
+                        var index = $(this).data('value');
+                        _this.month = index;
+                        _this.day = 1;
+                        _this.changeDate();
+                        if (!_this.settings.onlyYM) {
+                            _this.monthContainer.hide(300);
+                        } else {
+                            $(_this.settings.target).val(_this.year.toString() + _this.separator + (_this.month + 1));
+                            _this.hide();
+                            _this.settings.selected && _this.settings.selected.call(_this, _this.date, _this.calendarContainer);
+                        }
+                    });
+                } else if (!this.settings.onlyYM) {
+                    _this.actionFlow(_this.monthContainer, 'toggle');
+                } else {
+                    _this.actionFlow(_this.monthContainer, 'show');
+                }
+                this.monthContainer.html('');
+                for (var i = 0, l = this.monthArr.length; i < l; i++) {
+                    var m = this.monthArr[i];
+                    var cls = '';
+                    if (_this.month == i) {
+                        cls = ' class="current" ';
+                    }
+                    this.monthContainer.append('<div ' + cls + ' data-value="' + i + '">' + m + '</div>');
+                };
+                this.settings.goCallback && this.settings.goCallback.call(this, 'current-month', this.date);
+            }
+        },
+        changeDate: function() {
+            this._getDate();
+            this.formatDate();
+            this.renderHeader();
+        },
+        renderHeader: function() {
+            $('[data-role="current-month"]', this.calendarContainer).html(this.monthArr[this.month])
+            $('[data-role="current-year"]', this.calendarContainer).html(this.year);
+            var daylist = '';
+            for (var i = 0, l = this.dayArr.length; i < l; i++) {
+                daylist += '<b>' + this.dayArr[i] + '</b>';
+            };
+            if (!this.settings.onlyYM) {
+                $('.calendar-header', this.calendarContainer).html(daylist);
+            }
+        },
+        _getDate: function() {
+            this.date = new Date(this.year, this.month, this.day);
+        },
+        formatDate: function() {
+            var date = this.date || this.defaultDate;
+            this.year = date.getFullYear();
+            this.month = date.getMonth();
+            this.day = date.getDate();
+            var ndate = new Date(this.year, this.month + 1, 0);
+            var dayNum = ndate.getDate();
+            var list = '<ul>';
+            var firstDay = (new Date(this.year, this.month, 1)).getDay();
+            var preDate = new Date(this.year, this.month, 0);
+            var preDateNum = preDate.getDate();
+            var nextDate = new Date(this.year, this.month + 2, 0);
+            if (firstDay > 0) {
+                list += this._getDay(preDateNum - firstDay + 1, preDateNum, "preday", preDate);
+            }
+            list += this._getDay(1, dayNum, '', date);
+            var lastDay = (new Date(this.year, this.month, dayNum)).getDay();
+            list += this._getDay(1, 6 - lastDay, "nextday", nextDate);
+            list += '</ul>';
+            $('#' + this.id).find(".c_days").html(list);
+        },
+        _toString: function(dateArr) {
+            var arr = [];
+            var len = dateArr.length;
+            for (var i = 0; i < len; i++) {
+                var item = dateArr[i];
+                if (typeof item === "string") {
+                    dateArr[i] = new Date(item);
+                };
+                for (var j = 0; j < i; j++) {
+                    if (item.getTime() < dateArr[j]) {
+                        var tmp = dateArr[i];
+                        dateArr[i] = dateArr[j];
+                        dateArr[j] = tmp;
+                    }
+                }
+            };
+            for (var i = 0, l = dateArr.length; i < l; i++) {
+                var d = dateArr[i];
+                var year = d.getFullYear();
+                var month = this._getTowNum(d.getMonth() + 1);
+                var day = this._getTowNum(d.getDate());
+                arr.push(year + this.separator + month + this.separator + day);
+            }
+            return arr;
+        },
+        _getDay: function(startNum, dayNum, cls, date) {
+            var list = '';
+            var start = this.range[0],
+                startDate,
+                end = this.range[1],
+                endDate;
+            if (start) {
+                start = new Date(Date.parse(start));
+                startDate = +new Date(start.getFullYear(), start.getMonth(), start.getDate());
+            };
+            if (end) {
+                end = new Date(Date.parse(end));
+                endDate = +new Date(end.getFullYear(), end.getMonth(), end.getDate());
+            }
+            for (var i = startNum; i <= dayNum; i++) {
+                var className = cls || "";
+                var datavalue = date.getFullYear() + this.separator + this._getTowNum(date.getMonth() + 1) + this.separator;
+                datavalue += this._getTowNum(i);
+                var d = new Date(date.getFullYear(), date.getMonth(), i);
+                var time = d.getTime();
+                //多选
+                //console.log(this.dateArr)
+                if (this.settings.multiple) {
+                    if (this._dateInArr(d, this.dateArr)) {
+                        className += ' focus';
+                    }
+                } else
+                if (time == +new Date(this.defaultDate.getFullYear(), this.defaultDate.getMonth(), this.defaultDate.getDate())) {
+                    className += ' focus';
+                }
+                if ((startDate && time < startDate) || (endDate && time > endDate)) {
+                    className += " disabled";
+                }
+                if (this.settings.filter && !this.settings.filter(time)) {
+                    className += " disabled";
+                }
+                list += '<li class="' + className + '" data-value="' + datavalue + '">' + i + '</li>';
+            };
+            return list;
+        },
+        _dateInArr: function(date, arr) {
+            for (var i = arr.length - 1; i >= 0; i--) {
+                var item = arr[i];
+                var idate = item;
+                if (typeof item === "string") {
+                    var focusDateArr = item.split(this.separator);
+                    idate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]);
+                }
+                if (date.getTime() == idate.getTime()) {
+                    return true;
+                    break;
+                }
+            };
+        },
+        _removeDate: function(date, arr) {
+            var newArr = [];
+            for (var i = arr.length - 1; i >= 0; i--) {
+                var item = arr[i];
+                var idate = item;
+                if (typeof item === "string") {
+                    var focusDateArr = item.split(this.separator);
+                    idate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2]);
+                }
+                if (date.getTime() == idate.getTime()) {
+                    continue;
+                }
+                newArr.push(idate);
+            };
+            this.dateArr = newArr;
+        },
+        _getTowNum: function(n) {
+            var num = '0' + n.toString();
+            return num.length == 2 ? num : num.substr(1, 2);
+        }
+    };
+    return CustomCalendar;
 });
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,92 +1,92 @@
-$(document).ready(function() {
-    const $scheduleType = $('#id_schedule_type');
-    const $crontab = $('.form-row.field-crontab');
-    const $onceSchedule = $('.form-row.field-once_schedule')
-    const $periodSchedule = $('.form-row.field-period_schedule');
-
-    const $timingDiv = $("div[class*='timing']");
-    const $timingType = $('#id_timing_type');
-    const $timingDay = $('.form-row.field-timing_time,.fieldBox.field-timing_period');
-    const $timingWeekday = $('.form-row.field-timing_weekday');
-    const $timingMonthday = $('.form-row.field-timing_monthday');
-    const $timingYear = $('.form-row.field-timing_year');
-    const $timingDatetime = $('.form-row.field-timing_datetime');
-
-
-    function show_hide_timing_fields() {
-        const timingType = $timingType.val();
-        console.log("timingType is ", timingType);
-        if (timingType === "DATETIME") {
-            $timingWeekday.hide();
-            $timingDay.hide();
-            $timingMonthday.hide();
-            $timingYear.hide();
-            $timingDatetime.show();
-            return;
-        }
-        $timingDatetime.hide();
-        $timingDay.show();
-        const $timingPeriodUnit = $('#id_period_unit');
-        if (timingType === 'DAY') {
-            $timingWeekday.hide();
-            $timingMonthday.hide();
-            $timingYear.hide();
-            $timingPeriodUnit.text('天');
-        }
-        if (timingType === 'WEEKDAY') {
-            $timingWeekday.show();
-            $timingMonthday.hide();
-            $timingYear.hide();
-            $timingPeriodUnit.text('周');
-        } else if (timingType === "MONTHDAY") {
-            $timingWeekday.hide();
-            $timingMonthday.show();
-            $timingYear.hide();
-            $timingPeriodUnit.text('月');
-        } else if (timingType === "YEAR") {
-            $timingWeekday.hide();
-            $timingMonthday.hide();
-            $timingYear.show();
-            $timingPeriodUnit.text('年');
-        }
-    }
-
-    function show_hide_timing(show) {
-        if (show) {
-            $timingDiv.show();
-            show_hide_timing_fields();
-        } else {
-            $timingDiv.hide();
-        }
-    }
-
-    function show_hide_fields() {
-        console.log($scheduleType.val());
-        const scheduleType = $scheduleType.val();
-        if (scheduleType === 'C') {
-            $crontab.show();
-            $onceSchedule.hide();
-            $periodSchedule.hide();
-        } else if (scheduleType === 'S') {
-            $crontab.hide();
-            $onceSchedule.hide();
-            $periodSchedule.show();
-        } else if (scheduleType === 'O') {
-            $crontab.hide();
-            $onceSchedule.show();
-            $periodSchedule.hide();
-        } else if (scheduleType === 'T') {
-            $crontab.hide();
-            $onceSchedule.hide();
-            $periodSchedule.hide();
-        } else if (scheduleType === 'N') {
-            $crontab.hide();
-            $onceSchedule.hide();
-            $periodSchedule.hide();
-        }
-        show_hide_timing(scheduleType === 'T');
-    }
-    show_hide_fields();
-    $scheduleType.on('change', show_hide_fields);
-    $timingType.on('change', show_hide_timing_fields);
+$(document).ready(function() {
+    const $scheduleType = $('#id_schedule_type');
+    const $crontab = $('.form-row.field-crontab');
+    const $onceSchedule = $('.form-row.field-once_schedule')
+    const $periodSchedule = $('.form-row.field-period_schedule');
+
+    const $timingDiv = $("div[class*='timing']");
+    const $timingType = $('#id_timing_type');
+    const $timingDay = $('.form-row.field-timing_time,.fieldBox.field-timing_period');
+    const $timingWeekday = $('.form-row.field-timing_weekday');
+    const $timingMonthday = $('.form-row.field-timing_monthday');
+    const $timingYear = $('.form-row.field-timing_year');
+    const $timingDatetime = $('.form-row.field-timing_datetime');
+
+
+    function show_hide_timing_fields() {
+        const timingType = $timingType.val();
+        console.log("timingType is ", timingType);
+        if (timingType === "DATETIME") {
+            $timingWeekday.hide();
+            $timingDay.hide();
+            $timingMonthday.hide();
+            $timingYear.hide();
+            $timingDatetime.show();
+            return;
+        }
+        $timingDatetime.hide();
+        $timingDay.show();
+        const $timingPeriodUnit = $('#id_period_unit');
+        if (timingType === 'DAY') {
+            $timingWeekday.hide();
+            $timingMonthday.hide();
+            $timingYear.hide();
+            $timingPeriodUnit.text('天');
+        }
+        if (timingType === 'WEEKDAY') {
+            $timingWeekday.show();
+            $timingMonthday.hide();
+            $timingYear.hide();
+            $timingPeriodUnit.text('周');
+        } else if (timingType === "MONTHDAY") {
+            $timingWeekday.hide();
+            $timingMonthday.show();
+            $timingYear.hide();
+            $timingPeriodUnit.text('月');
+        } else if (timingType === "YEAR") {
+            $timingWeekday.hide();
+            $timingMonthday.hide();
+            $timingYear.show();
+            $timingPeriodUnit.text('年');
+        }
+    }
+
+    function show_hide_timing(show) {
+        if (show) {
+            $timingDiv.show();
+            show_hide_timing_fields();
+        } else {
+            $timingDiv.hide();
+        }
+    }
+
+    function show_hide_fields() {
+        console.log($scheduleType.val());
+        const scheduleType = $scheduleType.val();
+        if (scheduleType === 'C') {
+            $crontab.show();
+            $onceSchedule.hide();
+            $periodSchedule.hide();
+        } else if (scheduleType === 'S') {
+            $crontab.hide();
+            $onceSchedule.hide();
+            $periodSchedule.show();
+        } else if (scheduleType === 'O') {
+            $crontab.hide();
+            $onceSchedule.show();
+            $periodSchedule.hide();
+        } else if (scheduleType === 'T') {
+            $crontab.hide();
+            $onceSchedule.hide();
+            $periodSchedule.hide();
+        } else if (scheduleType === 'N') {
+            $crontab.hide();
+            $onceSchedule.hide();
+            $periodSchedule.hide();
+        }
+        show_hide_timing(scheduleType === 'T');
+    }
+    show_hide_fields();
+    $scheduleType.on('change', show_hide_fields);
+    $timingType.on('change', show_hide_timing_fields);
 });
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/admin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,314 +1,344 @@
 00000000: 6672 6f6d 2064 6a61 6e67 6f2e 636f 6e74  from django.cont
 00000010: 7269 6220 696d 706f 7274 2061 646d 696e  rib import admin
-00000020: 0a66 726f 6d20 646a 616e 676f 2e64 6973  .from django.dis
-00000030: 7061 7463 6820 696d 706f 7274 2072 6563  patch import rec
-00000040: 6569 7665 720a 6672 6f6d 2064 6a61 6e67  eiver.from djang
-00000050: 6f2e 7368 6f72 7463 7574 7320 696d 706f  o.shortcuts impo
-00000060: 7274 2072 6576 6572 7365 0a66 726f 6d20  rt reverse.from 
-00000070: 646a 616e 676f 2e75 7469 6c73 2e68 746d  django.utils.htm
-00000080: 6c20 696d 706f 7274 2066 6f72 6d61 745f  l import format_
-00000090: 6874 6d6c 0a66 726f 6d20 646a 616e 676f  html.from django
-000000a0: 2e64 622e 6d6f 6465 6c73 2e73 6967 6e61  .db.models.signa
-000000b0: 6c73 2069 6d70 6f72 7420 706f 7374 5f64  ls import post_d
-000000c0: 656c 6574 650a 6672 6f6d 202e 2069 6d70  elete.from . imp
-000000d0: 6f72 7420 6d6f 6465 6c73 0a66 726f 6d20  ort models.from 
-000000e0: 2e20 696d 706f 7274 2066 6f72 6d73 0a66  . import forms.f
-000000f0: 726f 6d20 2e2e 2069 6d70 6f72 7420 6164  rom .. import ad
-00000100: 6d69 6e20 6173 2062 6173 655f 6164 6d69  min as base_admi
-00000110: 6e0a 6672 6f6d 202e 7072 6f63 6573 7320  n.from .process 
-00000120: 696d 706f 7274 2050 726f 6365 7373 4d61  import ProcessMa
-00000130: 6e61 6765 720a 6672 6f6d 202e 2e73 7973  nager.from ..sys
-00000140: 7465 6d5f 7461 736b 5f65 7865 6375 7469  tem_task_executi
-00000150: 6f6e 2e6d 6169 6e20 696d 706f 7274 2073  on.main import s
-00000160: 7461 7274 5f73 7973 7465 6d5f 636c 6965  tart_system_clie
-00000170: 6e74 0a69 6d70 6f72 7420 6f73 0a0a 0a64  nt.import os...d
-00000180: 6566 2069 6e69 745f 7379 7374 656d 5f70  ef init_system_p
-00000190: 726f 6365 7373 2829 3a0a 2020 2020 6c6f  rocess():.    lo
-000001a0: 6773 5f70 6174 6820 3d20 6f73 2e70 6174  gs_path = os.pat
-000001b0: 682e 6a6f 696e 286f 732e 6765 7463 7764  h.join(os.getcwd
-000001c0: 2829 2c20 276c 6f67 7327 290a 2020 2020  (), 'logs').    
-000001d0: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
-000001e0: 7869 7374 7328 6c6f 6773 5f70 6174 6829  xists(logs_path)
-000001f0: 3a0a 2020 2020 2020 2020 6f73 2e6d 6b64  :.        os.mkd
-00000200: 6972 286c 6f67 735f 7061 7468 290a 2020  ir(logs_path).  
-00000210: 2020 6d6f 6465 6c73 2e53 7973 7465 6d50    models.SystemP
-00000220: 726f 6365 7373 2e6f 626a 6563 7473 2e61  rocess.objects.a
-00000230: 6c6c 2829 2e64 656c 6574 6528 290a 2020  ll().delete().  
-00000240: 2020 6e61 6d65 203d 2027 7379 7374 656d    name = 'system
-00000250: 2d70 726f 6365 7373 2d64 6566 6175 6c74  -process-default
-00000260: 270a 2020 2020 6c6f 675f 6669 6c65 203d  '.    log_file =
-00000270: 206f 732e 7061 7468 2e6a 6f69 6e28 6c6f   os.path.join(lo
-00000280: 6773 5f70 6174 682c 2066 277b 6e61 6d65  gs_path, f'{name
-00000290: 7d2e 6c6f 6727 290a 2020 2020 696e 7374  }.log').    inst
-000002a0: 616e 6365 203d 206d 6f64 656c 732e 5379  ance = models.Sy
-000002b0: 7374 656d 5072 6f63 6573 7328 0a20 2020  stemProcess(.   
-000002c0: 2020 2020 2070 726f 6365 7373 5f6e 616d       process_nam
-000002d0: 653d 6e61 6d65 2c0a 2020 2020 2020 2020  e=name,.        
-000002e0: 6c6f 675f 6669 6c65 3d6c 6f67 5f66 696c  log_file=log_fil
-000002f0: 650a 2020 2020 290a 2020 2020 7072 6f63  e.    ).    proc
-00000300: 6573 7320 3d20 5072 6f63 6573 734d 616e  ess = ProcessMan
-00000310: 6167 6572 2e63 7265 6174 6528 7374 6172  ager.create(star
-00000320: 745f 7379 7374 656d 5f63 6c69 656e 742c  t_system_client,
-00000330: 2069 6e73 7461 6e63 652e 6c6f 675f 6669   instance.log_fi
-00000340: 6c65 290a 2020 2020 696e 7374 616e 6365  le).    instance
-00000350: 2e70 726f 6365 7373 5f69 6420 3d20 7072  .process_id = pr
-00000360: 6f63 6573 732e 7069 640a 2020 2020 696e  ocess.pid.    in
-00000370: 7374 616e 6365 2e73 6176 6528 290a 0a0a  stance.save()...
-00000380: 6465 6620 696e 6974 5f73 7973 7465 6d5f  def init_system_
-00000390: 6461 7461 2829 3a0a 2020 2020 6672 6f6d  data():.    from
-000003a0: 202e 6d6f 6465 6c73 2069 6d70 6f72 7420   .models import 
-000003b0: 6275 696c 7469 6e73 0a20 2020 2062 7569  builtins.    bui
-000003c0: 6c74 696e 732e 696e 6974 6961 6c69 7a65  ltins.initialize
-000003d0: 2829 0a0a 0a69 6620 6f73 2e65 6e76 6972  ()...if os.envir
-000003e0: 6f6e 2e67 6574 2827 5255 4e5f 4d41 494e  on.get('RUN_MAIN
-000003f0: 2729 203d 3d20 2774 7275 6527 2061 6e64  ') == 'true' and
-00000400: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
-00000410: 2752 554e 5f43 4c49 454e 5427 2920 213d  'RUN_CLIENT') !=
-00000420: 2027 7472 7565 273a 0a20 2020 2069 6e69   'true':.    ini
-00000430: 745f 7379 7374 656d 5f70 726f 6365 7373  t_system_process
-00000440: 2829 0a20 2020 2069 6e69 745f 7379 7374  ().    init_syst
-00000450: 656d 5f64 6174 6128 290a 0a0a 4072 6563  em_data()...@rec
-00000460: 6569 7665 7228 706f 7374 5f64 656c 6574  eiver(post_delet
-00000470: 652c 2073 656e 6465 723d 6d6f 6465 6c73  e, sender=models
-00000480: 2e53 7973 7465 6d50 726f 6365 7373 290a  .SystemProcess).
-00000490: 6465 6620 6465 6c65 7465 5f70 726f 6365  def delete_proce
-000004a0: 7373 2873 656e 6465 722c 2069 6e73 7461  ss(sender, insta
-000004b0: 6e63 653a 206d 6f64 656c 732e 5379 7374  nce: models.Syst
-000004c0: 656d 5072 6f63 6573 732c 202a 2a6b 7761  emProcess, **kwa
-000004d0: 7267 7329 3a0a 2020 2020 5072 6f63 6573  rgs):.    Proces
-000004e0: 734d 616e 6167 6572 2e6b 696c 6c28 696e  sManager.kill(in
-000004f0: 7374 616e 6365 2e70 726f 6365 7373 5f69  stance.process_i
-00000500: 6429 0a20 2020 2069 6620 6f73 2e70 6174  d).    if os.pat
-00000510: 682e 6973 6669 6c65 2869 6e73 7461 6e63  h.isfile(instanc
-00000520: 652e 6c6f 675f 6669 6c65 2920 616e 6420  e.log_file) and 
-00000530: 6e6f 7420 696e 7374 616e 6365 2e6c 6f67  not instance.log
-00000540: 5f66 696c 652e 656e 6473 7769 7468 2827  _file.endswith('
-00000550: 7379 7374 656d 2d70 726f 6365 7373 2d64  system-process-d
-00000560: 6566 6175 6c74 2e6c 6f67 2729 3a0a 2020  efault.log'):.  
-00000570: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-00000580: 696e 7374 616e 6365 2e6c 6f67 5f66 696c  instance.log_fil
-00000590: 6529 0a0a 0a63 6c61 7373 2053 7973 7465  e)...class Syste
-000005a0: 6d54 6173 6b41 646d 696e 2862 6173 655f  mTaskAdmin(base_
-000005b0: 6164 6d69 6e2e 5461 736b 4164 6d69 6e29  admin.TaskAdmin)
-000005c0: 3a0a 2020 2020 666f 726d 203d 2066 6f72  :.    form = for
-000005d0: 6d73 2e53 7973 7465 6d54 6173 6b46 6f72  ms.SystemTaskFor
-000005e0: 6d0a 2020 2020 7363 6865 6475 6c65 5f6d  m.    schedule_m
-000005f0: 6f64 656c 203d 206d 6f64 656c 732e 5379  odel = models.Sy
-00000600: 7374 656d 5363 6865 6475 6c65 0a20 2020  stemSchedule.   
-00000610: 206c 6973 745f 6469 7370 6c61 7920 3d20   list_display = 
-00000620: 2827 6964 272c 2027 6164 6d69 6e5f 7061  ('id', 'admin_pa
-00000630: 7265 6e74 272c 2027 6e61 6d65 272c 2027  rent', 'name', '
-00000640: 6361 7465 676f 7279 272c 2027 6164 6d69  category', 'admi
-00000650: 6e5f 7374 6174 7573 272c 2027 7363 6865  n_status', 'sche
-00000660: 6475 6c65 7327 2c20 2775 7064 6174 655f  dules', 'update_
-00000670: 7469 6d65 2729 0a0a 2020 2020 6669 656c  time')..    fiel
-00000680: 6473 203d 2028 0a20 2020 2020 2020 2028  ds = (.        (
-00000690: 2270 6172 656e 7422 2c20 2763 6174 6567  "parent", 'categ
-000006a0: 6f72 7927 2c29 2c0a 2020 2020 2020 2020  ory',),.        
-000006b0: 2827 7175 6575 6527 2c29 2c0a 2020 2020  ('queue',),.    
-000006c0: 2020 2020 2822 6e61 6d65 222c 2022 7374      ("name", "st
-000006d0: 6174 7573 222c 292c 0a20 2020 2020 2020  atus",),.       
-000006e0: 2022 636f 6e66 6967 222c 0a20 2020 2020   "config",.     
-000006f0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
-00000700: 2c0a 2020 2020 290a 2020 2020 6669 6c74  ,.    ).    filt
-00000710: 6572 5f68 6f72 697a 6f6e 7461 6c20 3d20  er_horizontal = 
-00000720: 5b5d 0a20 2020 206c 6973 745f 6669 6c74  [].    list_filt
-00000730: 6572 203d 2028 2763 6174 6567 6f72 7927  er = ('category'
-00000740: 2c20 2770 6172 656e 7427 290a 0a20 2020  , 'parent')..   
-00000750: 2064 6566 2068 6173 5f64 656c 6574 655f   def has_delete_
-00000760: 7065 726d 6973 7369 6f6e 2873 656c 662c  permission(self,
-00000770: 2072 6571 7565 7374 2c20 6f62 6a3d 4e6f   request, obj=No
-00000780: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-00000790: 6f62 6a3a 0a20 2020 2020 2020 2020 2020  obj:.           
-000007a0: 2072 6574 7572 6e20 6f62 6a2e 6361 7465   return obj.cate
-000007b0: 676f 7279 2021 3d20 6d6f 6465 6c73 2e62  gory != models.b
-000007c0: 7569 6c74 696e 732e 6361 7465 676f 7269  uiltins.categori
-000007d0: 6573 2e73 7973 7465 6d5f 6465 6661 756c  es.system_defaul
-000007e0: 745f 6361 7465 676f 7279 0a20 2020 2020  t_category.     
-000007f0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00000800: 0a63 6c61 7373 2053 7973 7465 6d53 6368  .class SystemSch
-00000810: 6564 756c 6543 616c 6c62 6163 6b41 646d  eduleCallbackAdm
-00000820: 696e 2862 6173 655f 6164 6d69 6e2e 5461  in(base_admin.Ta
-00000830: 736b 5363 6865 6475 6c65 4361 6c6c 6261  skScheduleCallba
-00000840: 636b 4164 6d69 6e29 3a0a 2020 2020 7061  ckAdmin):.    pa
-00000850: 7373 0a0a 0a63 6c61 7373 2053 7973 7465  ss...class Syste
-00000860: 6d53 6368 6564 756c 6541 646d 696e 2862  mScheduleAdmin(b
-00000870: 6173 655f 6164 6d69 6e2e 5461 736b 5363  ase_admin.TaskSc
-00000880: 6865 6475 6c65 4164 6d69 6e29 3a0a 0a20  heduleAdmin):.. 
-00000890: 2020 2074 6173 6b5f 6d6f 6465 6c20 3d20     task_model = 
-000008a0: 6d6f 6465 6c73 2e53 7973 7465 6d54 6173  models.SystemTas
-000008b0: 6b0a 2020 2020 7363 6865 6475 6c65 5f6c  k.    schedule_l
-000008c0: 6f67 5f6d 6f64 656c 203d 206d 6f64 656c  og_model = model
-000008d0: 732e 5379 7374 656d 5363 6865 6475 6c65  s.SystemSchedule
-000008e0: 4c6f 670a 2020 2020 7175 6575 6573 203d  Log.    queues =
-000008f0: 206d 6f64 656c 732e 6275 696c 7469 6e73   models.builtins
-00000900: 2e71 7565 7565 730a 2020 2020 7363 6865  .queues.    sche
-00000910: 6475 6c65 5f70 7574 5f6e 616d 6520 3d20  dule_put_name = 
-00000920: 2773 7973 7465 6d5f 7363 6865 6475 6c65  'system_schedule
-00000930: 5f70 7574 270a 2020 2020 6c69 7374 5f64  _put'.    list_d
-00000940: 6973 706c 6179 203d 2028 2769 6427 2c20  isplay = ('id', 
-00000950: 2761 646d 696e 5f74 6173 6b27 2c20 2773  'admin_task', 's
-00000960: 6368 6564 756c 655f 7479 7065 272c 2027  chedule_type', '
-00000970: 7363 6865 6475 6c65 5f73 7562 5f74 7970  schedule_sub_typ
-00000980: 6527 2c20 276e 6578 745f 7363 6865 6475  e', 'next_schedu
-00000990: 6c65 5f74 696d 6527 2c0a 2020 2020 2020  le_time',.      
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-000009b0: 7461 7475 7327 2c20 2770 7574 272c 2027  tatus', 'put', '
-000009c0: 6c6f 6773 272c 2027 7570 6461 7465 5f74  logs', 'update_t
-000009d0: 696d 6527 290a 2020 2020 6c69 7374 5f66  ime').    list_f
-000009e0: 696c 7465 7220 3d20 2827 7461 736b 5f5f  ilter = ('task__
-000009f0: 6361 7465 676f 7279 272c 2029 0a0a 2020  category', )..  
-00000a00: 2020 6465 6620 6861 735f 6465 6c65 7465    def has_delete
-00000a10: 5f70 6572 6d69 7373 696f 6e28 7365 6c66  _permission(self
-00000a20: 2c20 7265 7175 6573 742c 206f 626a 3d4e  , request, obj=N
-00000a30: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00000a40: 206f 626a 3a0a 2020 2020 2020 2020 2020   obj:.          
-00000a50: 2020 7265 7475 726e 206f 626a 2e74 6173    return obj.tas
-00000a60: 6b2e 6361 7465 676f 7279 2021 3d20 6d6f  k.category != mo
-00000a70: 6465 6c73 2e62 7569 6c74 696e 732e 6361  dels.builtins.ca
-00000a80: 7465 676f 7269 6573 2e73 7973 7465 6d5f  tegories.system_
-00000a90: 6465 6661 756c 745f 6361 7465 676f 7279  default_category
-00000aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000ab0: 5472 7565 0a0a 0a63 6c61 7373 2053 7973  True...class Sys
-00000ac0: 7465 6d53 6368 6564 756c 654c 6f67 4164  temScheduleLogAd
-00000ad0: 6d69 6e28 6261 7365 5f61 646d 696e 2e54  min(base_admin.T
-00000ae0: 6173 6b53 6368 6564 756c 654c 6f67 4164  askScheduleLogAd
-00000af0: 6d69 6e29 3a0a 2020 2020 7363 6865 6475  min):.    schedu
-00000b00: 6c65 5f72 6574 7279 5f6e 616d 6520 3d20  le_retry_name = 
-00000b10: 2773 7973 7465 6d5f 7363 6865 6475 6c65  'system_schedule
-00000b20: 5f72 6574 7279 270a 0a0a 636c 6173 7320  _retry'...class 
-00000b30: 5379 7374 656d 5072 6f63 6573 7341 646d  SystemProcessAdm
-00000b40: 696e 2861 646d 696e 2e4d 6f64 656c 4164  in(admin.ModelAd
-00000b50: 6d69 6e29 3a0a 2020 2020 6c69 7374 5f64  min):.    list_d
-00000b60: 6973 706c 6179 203d 2028 2770 726f 6365  isplay = ('proce
-00000b70: 7373 5f69 6427 2c20 2770 726f 6365 7373  ss_id', 'process
-00000b80: 5f6e 616d 6527 2c20 276c 6f67 5f66 696c  _name', 'log_fil
-00000b90: 6527 2c20 2773 7461 7475 7327 2c20 2773  e', 'status', 's
-00000ba0: 746f 705f 7072 6f63 6573 7327 2c20 2773  top_process', 's
-00000bb0: 686f 775f 6c6f 6727 2c20 2775 7064 6174  how_log', 'updat
-00000bc0: 655f 7469 6d65 2729 0a20 2020 2066 6f72  e_time').    for
-00000bd0: 6d20 3d20 666f 726d 732e 5379 7374 656d  m = forms.System
-00000be0: 5072 6f63 6573 7346 6f72 6d0a 2020 2020  ProcessForm.    
-00000bf0: 6669 656c 6473 203d 2028 0a20 2020 2020  fields = (.     
-00000c00: 2020 2027 7379 7374 656d 5f70 6174 6827     'system_path'
-00000c10: 2c0a 2020 2020 2020 2020 2770 726f 6365  ,.        'proce
-00000c20: 7373 5f6e 616d 6527 2c0a 2020 2020 2020  ss_name',.      
-00000c30: 2020 2765 6e76 272c 0a20 2020 2020 2020    'env',.       
-00000c40: 2027 6c6f 675f 6669 6c65 272c 0a20 2020   'log_file',.   
-00000c50: 2020 2020 2027 7072 6f63 6573 735f 6964       'process_id
-00000c60: 272c 0a20 2020 2020 2020 2027 6372 6561  ',.        'crea
-00000c70: 7465 5f74 696d 6527 2c0a 2020 2020 290a  te_time',.    ).
-00000c80: 0a20 2020 2072 6561 646f 6e6c 795f 6669  .    readonly_fi
-00000c90: 656c 6473 203d 2028 2763 7265 6174 655f  elds = ('create_
-00000ca0: 7469 6d65 272c 2027 7570 6461 7465 5f74  time', 'update_t
-00000cb0: 696d 6527 290a 0a20 2020 2064 6566 2073  ime')..    def s
-00000cc0: 746f 705f 7072 6f63 6573 7328 7365 6c66  top_process(self
-00000cd0: 2c20 6f62 6a29 3a0a 2020 2020 2020 2020  , obj):.        
-00000ce0: 7572 6c20 3d20 7265 7665 7273 6528 2773  url = reverse('s
-00000cf0: 7973 7465 6d5f 7072 6f63 6573 735f 7374  ystem_process_st
-00000d00: 6f70 272c 2061 7267 733d 286f 626a 2e70  op', args=(obj.p
-00000d10: 726f 6365 7373 5f69 642c 2929 0a20 2020  rocess_id,)).   
-00000d20: 2020 2020 2072 6574 7572 6e20 666f 726d       return form
-00000d30: 6174 5f68 746d 6c28 0a20 2020 2020 2020  at_html(.       
-00000d40: 2020 2020 2027 3c61 2068 7265 663d 2225       '<a href="%
-00000d50: 7322 2074 6172 6765 743d 225f 626c 616e  s" target="_blan
-00000d60: 6b22 3ee5 819c e6ad a23c 2f61 3e27 2025  k">......</a>' %
-00000d70: 2075 726c 0a20 2020 2020 2020 2029 0a20   url.        ). 
-00000d80: 2020 2073 746f 705f 7072 6f63 6573 732e     stop_process.
-00000d90: 7368 6f72 745f 6465 7363 7269 7074 696f  short_descriptio
-00000da0: 6e20 3d20 27e5 819c e6ad a2e8 bf90 e8a1  n = '...........
-00000db0: 8c27 0a0a 2020 2020 6465 6620 7368 6f77  .'..    def show
-00000dc0: 5f6c 6f67 2873 656c 662c 206f 626a 293a  _log(self, obj):
-00000dd0: 0a20 2020 2020 2020 2075 726c 203d 2072  .        url = r
-00000de0: 6576 6572 7365 2827 7379 7374 656d 5f70  everse('system_p
-00000df0: 726f 6365 7373 5f6c 6f67 272c 2061 7267  rocess_log', arg
-00000e00: 733d 286f 626a 2e70 726f 6365 7373 5f69  s=(obj.process_i
-00000e10: 642c 2929 0a20 2020 2020 2020 2072 6574  d,)).        ret
-00000e20: 7572 6e20 666f 726d 6174 5f68 746d 6c28  urn format_html(
-00000e30: 0a20 2020 2020 2020 2020 2020 2027 3c61  .            '<a
-00000e40: 2068 7265 663d 2225 7322 2074 6172 6765   href="%s" targe
-00000e50: 743d 225f 626c 616e 6b22 3ee6 9fa5 e79c  t="_blank">.....
-00000e60: 8be6 97a5 e5bf 973c 2f61 3e27 2025 2075  .......</a>' % u
-00000e70: 726c 0a20 2020 2020 2020 2029 0a20 2020  rl.        ).   
-00000e80: 2073 686f 775f 6c6f 672e 7368 6f72 745f   show_log.short_
-00000e90: 6465 7363 7269 7074 696f 6e20 3d20 27e6  description = '.
-00000ea0: 97a5 e5bf 9727 0a0a 2020 2020 6465 6620  .....'..    def 
-00000eb0: 6861 735f 6465 6c65 7465 5f70 6572 6d69  has_delete_permi
-00000ec0: 7373 696f 6e28 7365 6c66 2c20 7265 7175  ssion(self, requ
-00000ed0: 6573 742c 206f 626a 3d4e 6f6e 6529 3a0a  est, obj=None):.
-00000ee0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000ef0: 616c 7365 0a0a 0a63 6c61 7373 2053 7973  alse...class Sys
-00000f00: 7465 6d53 6368 6564 756c 6551 7565 7565  temScheduleQueue
-00000f10: 4164 6d69 6e28 6261 7365 5f61 646d 696e  Admin(base_admin
-00000f20: 2e54 6173 6b53 6368 6564 756c 6551 7565  .TaskScheduleQue
-00000f30: 7565 4164 6d69 6e29 3a0a 2020 2020 666f  ueAdmin):.    fo
-00000f40: 726d 203d 2066 6f72 6d73 2e53 7973 7465  rm = forms.Syste
-00000f50: 6d53 6368 6564 756c 6551 7565 7565 466f  mScheduleQueueFo
-00000f60: 726d 0a20 2020 2062 7569 6c74 696e 7320  rm.    builtins 
-00000f70: 3d20 6d6f 6465 6c73 2e62 7569 6c74 696e  = models.builtin
-00000f80: 730a 2020 2020 7363 6865 6475 6c65 5f67  s.    schedule_g
-00000f90: 6574 5f6e 616d 6520 3d20 2773 7973 7465  et_name = 'syste
-00000fa0: 6d5f 7363 6865 6475 6c65 5f67 6574 270a  m_schedule_get'.
-00000fb0: 0a0a 636c 6173 7320 5379 7374 656d 5363  ..class SystemSc
-00000fc0: 6865 6475 6c65 5072 6f64 7563 6572 4164  heduleProducerAd
-00000fd0: 6d69 6e28 6261 7365 5f61 646d 696e 2e54  min(base_admin.T
-00000fe0: 6173 6b53 6368 6564 756c 6550 726f 6475  askScheduleProdu
-00000ff0: 6365 7241 646d 696e 293a 0a20 2020 2066  cerAdmin):.    f
-00001000: 6f72 6d20 3d20 666f 726d 732e 5379 7374  orm = forms.Syst
-00001010: 656d 5363 6865 6475 6c65 5072 6f64 7563  emScheduleProduc
-00001020: 6572 466f 726d 0a20 2020 2073 6368 6564  erForm.    sched
-00001030: 756c 655f 6765 745f 6e61 6d65 203d 2027  ule_get_name = '
-00001040: 7379 7374 656d 5f73 6368 6564 756c 655f  system_schedule_
-00001050: 6765 7427 0a20 2020 2062 7569 6c74 696e  get'.    builtin
-00001060: 7320 3d20 6d6f 6465 6c73 2e62 7569 6c74  s = models.built
-00001070: 696e 730a 0a0a 636c 6173 7320 5379 7374  ins...class Syst
-00001080: 656d 436f 6e73 756d 6572 5065 726d 6973  emConsumerPermis
-00001090: 7369 6f6e 4164 6d69 6e28 6261 7365 5f61  sionAdmin(base_a
-000010a0: 646d 696e 2e43 6f6e 7375 6d65 7250 6572  dmin.ConsumerPer
-000010b0: 6d69 7373 696f 6e41 646d 696e 293a 0a20  missionAdmin):. 
-000010c0: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
-000010d0: 5379 7374 656d 4578 6365 7074 696f 6e41  SystemExceptionA
-000010e0: 646d 696e 2862 6173 655f 6164 6d69 6e2e  dmin(base_admin.
-000010f0: 4578 6365 7074 696f 6e52 6570 6f72 7441  ExceptionReportA
-00001100: 646d 696e 293a 0a20 2020 2070 6173 730a  dmin):.    pass.
-00001110: 0a0a 6164 6d69 6e2e 7369 7465 2e72 6567  ..admin.site.reg
-00001120: 6973 7465 7228 6d6f 6465 6c73 2e53 7973  ister(models.Sys
-00001130: 7465 6d54 6173 6b2c 2053 7973 7465 6d54  temTask, SystemT
-00001140: 6173 6b41 646d 696e 290a 6164 6d69 6e2e  askAdmin).admin.
-00001150: 7369 7465 2e72 6567 6973 7465 7228 6d6f  site.register(mo
-00001160: 6465 6c73 2e53 7973 7465 6d53 6368 6564  dels.SystemSched
-00001170: 756c 6543 616c 6c62 6163 6b2c 2053 7973  uleCallback, Sys
-00001180: 7465 6d53 6368 6564 756c 6543 616c 6c62  temScheduleCallb
-00001190: 6163 6b41 646d 696e 290a 6164 6d69 6e2e  ackAdmin).admin.
-000011a0: 7369 7465 2e72 6567 6973 7465 7228 6d6f  site.register(mo
-000011b0: 6465 6c73 2e53 7973 7465 6d53 6368 6564  dels.SystemSched
-000011c0: 756c 652c 2053 7973 7465 6d53 6368 6564  ule, SystemSched
-000011d0: 756c 6541 646d 696e 290a 6164 6d69 6e2e  uleAdmin).admin.
-000011e0: 7369 7465 2e72 6567 6973 7465 7228 6d6f  site.register(mo
-000011f0: 6465 6c73 2e53 7973 7465 6d53 6368 6564  dels.SystemSched
-00001200: 756c 654c 6f67 2c20 5379 7374 656d 5363  uleLog, SystemSc
-00001210: 6865 6475 6c65 4c6f 6741 646d 696e 290a  heduleLogAdmin).
-00001220: 6164 6d69 6e2e 7369 7465 2e72 6567 6973  admin.site.regis
-00001230: 7465 7228 6d6f 6465 6c73 2e53 7973 7465  ter(models.Syste
-00001240: 6d53 6368 6564 756c 6551 7565 7565 2c20  mScheduleQueue, 
-00001250: 5379 7374 656d 5363 6865 6475 6c65 5175  SystemScheduleQu
-00001260: 6575 6541 646d 696e 290a 6164 6d69 6e2e  eueAdmin).admin.
-00001270: 7369 7465 2e72 6567 6973 7465 7228 6d6f  site.register(mo
-00001280: 6465 6c73 2e53 7973 7465 6d53 6368 6564  dels.SystemSched
-00001290: 756c 6550 726f 6475 6365 722c 2053 7973  uleProducer, Sys
-000012a0: 7465 6d53 6368 6564 756c 6550 726f 6475  temScheduleProdu
-000012b0: 6365 7241 646d 696e 290a 6164 6d69 6e2e  cerAdmin).admin.
-000012c0: 7369 7465 2e72 6567 6973 7465 7228 6d6f  site.register(mo
-000012d0: 6465 6c73 2e53 7973 7465 6d50 726f 6365  dels.SystemProce
-000012e0: 7373 2c20 5379 7374 656d 5072 6f63 6573  ss, SystemProces
-000012f0: 7341 646d 696e 290a 6164 6d69 6e2e 7369  sAdmin).admin.si
-00001300: 7465 2e72 6567 6973 7465 7228 6d6f 6465  te.register(mode
-00001310: 6c73 2e53 7973 7465 6d43 6f6e 7375 6d65  ls.SystemConsume
-00001320: 7250 6572 6d69 7373 696f 6e2c 2053 7973  rPermission, Sys
-00001330: 7465 6d43 6f6e 7375 6d65 7250 6572 6d69  temConsumerPermi
-00001340: 7373 696f 6e41 646d 696e 290a 6164 6d69  ssionAdmin).admi
-00001350: 6e2e 7369 7465 2e72 6567 6973 7465 7228  n.site.register(
-00001360: 6d6f 6465 6c73 2e53 7973 7465 6d45 7863  models.SystemExc
-00001370: 6570 7469 6f6e 5265 706f 7274 2c20 5379  eptionReport, Sy
-00001380: 7374 656d 4578 6365 7074 696f 6e41 646d  stemExceptionAdm
-00001390: 696e 290a 0a                             in)..
+00000020: 0d0a 6672 6f6d 2064 6a61 6e67 6f2e 6469  ..from django.di
+00000030: 7370 6174 6368 2069 6d70 6f72 7420 7265  spatch import re
+00000040: 6365 6976 6572 0d0a 6672 6f6d 2064 6a61  ceiver..from dja
+00000050: 6e67 6f2e 7368 6f72 7463 7574 7320 696d  ngo.shortcuts im
+00000060: 706f 7274 2072 6576 6572 7365 0d0a 6672  port reverse..fr
+00000070: 6f6d 2064 6a61 6e67 6f2e 7574 696c 732e  om django.utils.
+00000080: 6874 6d6c 2069 6d70 6f72 7420 666f 726d  html import form
+00000090: 6174 5f68 746d 6c0d 0a66 726f 6d20 646a  at_html..from dj
+000000a0: 616e 676f 2e64 622e 6d6f 6465 6c73 2e73  ango.db.models.s
+000000b0: 6967 6e61 6c73 2069 6d70 6f72 7420 706f  ignals import po
+000000c0: 7374 5f64 656c 6574 650d 0a66 726f 6d20  st_delete..from 
+000000d0: 2e20 696d 706f 7274 206d 6f64 656c 730d  . import models.
+000000e0: 0a66 726f 6d20 2e20 696d 706f 7274 2066  .from . import f
+000000f0: 6f72 6d73 0d0a 6672 6f6d 202e 2e20 696d  orms..from .. im
+00000100: 706f 7274 2061 646d 696e 2061 7320 6261  port admin as ba
+00000110: 7365 5f61 646d 696e 0d0a 6672 6f6d 202e  se_admin..from .
+00000120: 7072 6f63 6573 7320 696d 706f 7274 2050  process import P
+00000130: 726f 6365 7373 4d61 6e61 6765 720d 0a66  rocessManager..f
+00000140: 726f 6d20 2e2e 7379 7374 656d 5f74 6173  rom ..system_tas
+00000150: 6b5f 6578 6563 7574 696f 6e2e 6d61 696e  k_execution.main
+00000160: 2069 6d70 6f72 7420 7374 6172 745f 7379   import start_sy
+00000170: 7374 656d 5f63 6c69 656e 740d 0a69 6d70  stem_client..imp
+00000180: 6f72 7420 6f73 0d0a 0d0a 0d0a 6465 6620  ort os......def 
+00000190: 696e 6974 5f73 7973 7465 6d5f 7072 6f63  init_system_proc
+000001a0: 6573 7328 293a 0d0a 2020 2020 6c6f 6773  ess():..    logs
+000001b0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+000001c0: 6a6f 696e 286f 732e 6765 7463 7764 2829  join(os.getcwd()
+000001d0: 2c20 276c 6f67 7327 290d 0a20 2020 2069  , 'logs')..    i
+000001e0: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
+000001f0: 6973 7473 286c 6f67 735f 7061 7468 293a  ists(logs_path):
+00000200: 0d0a 2020 2020 2020 2020 6f73 2e6d 6b64  ..        os.mkd
+00000210: 6972 286c 6f67 735f 7061 7468 290d 0a20  ir(logs_path).. 
+00000220: 2020 206d 6f64 656c 732e 5379 7374 656d     models.System
+00000230: 5072 6f63 6573 732e 6f62 6a65 6374 732e  Process.objects.
+00000240: 616c 6c28 292e 6465 6c65 7465 2829 0d0a  all().delete()..
+00000250: 2020 2020 6e61 6d65 203d 2027 7379 7374      name = 'syst
+00000260: 656d 2d70 726f 6365 7373 2d64 6566 6175  em-process-defau
+00000270: 6c74 270d 0a20 2020 206c 6f67 5f66 696c  lt'..    log_fil
+00000280: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
+00000290: 286c 6f67 735f 7061 7468 2c20 6627 7b6e  (logs_path, f'{n
+000002a0: 616d 657d 2e6c 6f67 2729 0d0a 2020 2020  ame}.log')..    
+000002b0: 696e 7374 616e 6365 203d 206d 6f64 656c  instance = model
+000002c0: 732e 5379 7374 656d 5072 6f63 6573 7328  s.SystemProcess(
+000002d0: 0d0a 2020 2020 2020 2020 7072 6f63 6573  ..        proces
+000002e0: 735f 6e61 6d65 3d6e 616d 652c 0d0a 2020  s_name=name,..  
+000002f0: 2020 2020 2020 6c6f 675f 6669 6c65 3d6c        log_file=l
+00000300: 6f67 5f66 696c 650d 0a20 2020 2029 0d0a  og_file..    )..
+00000310: 2020 2020 7072 6f63 6573 7320 3d20 5072      process = Pr
+00000320: 6f63 6573 734d 616e 6167 6572 2e63 7265  ocessManager.cre
+00000330: 6174 6528 7374 6172 745f 7379 7374 656d  ate(start_system
+00000340: 5f63 6c69 656e 742c 2069 6e73 7461 6e63  _client, instanc
+00000350: 652e 6c6f 675f 6669 6c65 290d 0a20 2020  e.log_file)..   
+00000360: 2069 6e73 7461 6e63 652e 7072 6f63 6573   instance.proces
+00000370: 735f 6964 203d 2070 726f 6365 7373 2e70  s_id = process.p
+00000380: 6964 0d0a 2020 2020 696e 7374 616e 6365  id..    instance
+00000390: 2e73 6176 6528 290d 0a0d 0a0d 0a64 6566  .save()......def
+000003a0: 2069 6e69 745f 7379 7374 656d 5f64 6174   init_system_dat
+000003b0: 6128 293a 0d0a 2020 2020 6672 6f6d 202e  a():..    from .
+000003c0: 6d6f 6465 6c73 2069 6d70 6f72 7420 6275  models import bu
+000003d0: 696c 7469 6e73 0d0a 2020 2020 6275 696c  iltins..    buil
+000003e0: 7469 6e73 2e69 6e69 7469 616c 697a 6528  tins.initialize(
+000003f0: 290d 0a0d 0a0d 0a69 6620 6f73 2e65 6e76  )......if os.env
+00000400: 6972 6f6e 2e67 6574 2827 5255 4e5f 4d41  iron.get('RUN_MA
+00000410: 494e 2729 203d 3d20 2774 7275 6527 2061  IN') == 'true' a
+00000420: 6e64 206f 732e 656e 7669 726f 6e2e 6765  nd os.environ.ge
+00000430: 7428 2752 554e 5f43 4c49 454e 5427 2920  t('RUN_CLIENT') 
+00000440: 213d 2027 7472 7565 273a 0d0a 2020 2020  != 'true':..    
+00000450: 696e 6974 5f73 7973 7465 6d5f 7072 6f63  init_system_proc
+00000460: 6573 7328 290d 0a20 2020 2069 6e69 745f  ess()..    init_
+00000470: 7379 7374 656d 5f64 6174 6128 290d 0a0d  system_data()...
+00000480: 0a0d 0a40 7265 6365 6976 6572 2870 6f73  ...@receiver(pos
+00000490: 745f 6465 6c65 7465 2c20 7365 6e64 6572  t_delete, sender
+000004a0: 3d6d 6f64 656c 732e 5379 7374 656d 5072  =models.SystemPr
+000004b0: 6f63 6573 7329 0d0a 6465 6620 6465 6c65  ocess)..def dele
+000004c0: 7465 5f70 726f 6365 7373 2873 656e 6465  te_process(sende
+000004d0: 722c 2069 6e73 7461 6e63 653a 206d 6f64  r, instance: mod
+000004e0: 656c 732e 5379 7374 656d 5072 6f63 6573  els.SystemProces
+000004f0: 732c 202a 2a6b 7761 7267 7329 3a0d 0a20  s, **kwargs):.. 
+00000500: 2020 2050 726f 6365 7373 4d61 6e61 6765     ProcessManage
+00000510: 722e 6b69 6c6c 2869 6e73 7461 6e63 652e  r.kill(instance.
+00000520: 7072 6f63 6573 735f 6964 290d 0a20 2020  process_id)..   
+00000530: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+00000540: 6c65 2869 6e73 7461 6e63 652e 6c6f 675f  le(instance.log_
+00000550: 6669 6c65 2920 616e 6420 6e6f 7420 696e  file) and not in
+00000560: 7374 616e 6365 2e6c 6f67 5f66 696c 652e  stance.log_file.
+00000570: 656e 6473 7769 7468 2827 7379 7374 656d  endswith('system
+00000580: 2d70 726f 6365 7373 2d64 6566 6175 6c74  -process-default
+00000590: 2e6c 6f67 2729 3a0d 0a20 2020 2020 2020  .log'):..       
+000005a0: 206f 732e 7265 6d6f 7665 2869 6e73 7461   os.remove(insta
+000005b0: 6e63 652e 6c6f 675f 6669 6c65 290d 0a0d  nce.log_file)...
+000005c0: 0a0d 0a63 6c61 7373 2053 7973 7465 6d54  ...class SystemT
+000005d0: 6173 6b41 646d 696e 2862 6173 655f 6164  askAdmin(base_ad
+000005e0: 6d69 6e2e 5461 736b 4164 6d69 6e29 3a0d  min.TaskAdmin):.
+000005f0: 0a20 2020 2066 6f72 6d20 3d20 666f 726d  .    form = form
+00000600: 732e 5379 7374 656d 5461 736b 466f 726d  s.SystemTaskForm
+00000610: 0d0a 2020 2020 7363 6865 6475 6c65 5f6d  ..    schedule_m
+00000620: 6f64 656c 203d 206d 6f64 656c 732e 5379  odel = models.Sy
+00000630: 7374 656d 5363 6865 6475 6c65 0d0a 2020  stemSchedule..  
+00000640: 2020 6c69 7374 5f64 6973 706c 6179 203d    list_display =
+00000650: 2028 2769 6427 2c20 2761 646d 696e 5f70   ('id', 'admin_p
+00000660: 6172 656e 7427 2c20 276e 616d 6527 2c20  arent', 'name', 
+00000670: 2763 6174 6567 6f72 7927 2c20 2761 646d  'category', 'adm
+00000680: 696e 5f73 7461 7475 7327 2c20 2773 6368  in_status', 'sch
+00000690: 6564 756c 6573 272c 2027 7570 6461 7465  edules', 'update
+000006a0: 5f74 696d 6527 290d 0a0d 0a20 2020 2066  _time')....    f
+000006b0: 6965 6c64 7320 3d20 280d 0a20 2020 2020  ields = (..     
+000006c0: 2020 2027 6361 7465 676f 7279 272c 0d0a     'category',..
+000006d0: 2020 2020 2020 2020 2822 6e61 6d65 222c          ("name",
+000006e0: 2022 7374 6174 7573 222c 292c 0d0a 2020   "status",),..  
+000006f0: 2020 2020 2020 2822 7061 7265 6e74 222c        ("parent",
+00000700: 2027 7175 6575 6527 292c 0d0a 2020 2020   'queue'),..    
+00000710: 2020 2020 2273 6372 6970 7422 2c0d 0a20      "script",.. 
+00000720: 2020 2020 2020 2022 636f 6e66 6967 222c         "config",
+00000730: 0d0a 2020 2020 2020 2020 2764 6573 6372  ..        'descr
+00000740: 6970 7469 6f6e 272c 0d0a 2020 2020 290d  iption',..    ).
+00000750: 0a20 2020 2066 696c 7465 725f 686f 7269  .    filter_hori
+00000760: 7a6f 6e74 616c 203d 205b 5d0d 0a20 2020  zontal = []..   
+00000770: 206c 6973 745f 6669 6c74 6572 203d 2028   list_filter = (
+00000780: 2763 6174 6567 6f72 7927 2c20 2770 6172  'category', 'par
+00000790: 656e 7427 290d 0a0d 0a20 2020 2064 6566  ent')....    def
+000007a0: 2068 6173 5f64 656c 6574 655f 7065 726d   has_delete_perm
+000007b0: 6973 7369 6f6e 2873 656c 662c 2072 6571  ission(self, req
+000007c0: 7565 7374 2c20 6f62 6a3d 4e6f 6e65 293a  uest, obj=None):
+000007d0: 0d0a 2020 2020 2020 2020 6966 206f 626a  ..        if obj
+000007e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000007f0: 6574 7572 6e20 6f62 6a2e 6361 7465 676f  eturn obj.catego
+00000800: 7279 2021 3d20 6d6f 6465 6c73 2e62 7569  ry != models.bui
+00000810: 6c74 696e 732e 6361 7465 676f 7269 6573  ltins.categories
+00000820: 2e73 7973 7465 6d5f 6465 6661 756c 745f  .system_default_
+00000830: 6361 7465 676f 7279 0d0a 2020 2020 2020  category..      
+00000840: 2020 7265 7475 726e 2054 7275 650d 0a0d    return True...
+00000850: 0a20 2020 2063 6c61 7373 204d 6564 6961  .    class Media
+00000860: 3a0d 0a20 2020 2020 2020 206a 7320 3d20  :..        js = 
+00000870: 280d 0a20 2020 2020 2020 2020 2020 2027  (..            '
+00000880: 6874 7470 733a 2f2f 6364 6e2e 626f 6f74  https://cdn.boot
+00000890: 6373 732e 636f 6d2f 6a71 7565 7279 2f33  css.com/jquery/3
+000008a0: 2e33 2e31 2f6a 7175 6572 792e 6d69 6e2e  .3.1/jquery.min.
+000008b0: 6a73 272c 0d0a 2020 2020 2020 2020 2020  js',..          
+000008c0: 2020 2768 7474 7073 3a2f 2f63 646e 2e62    'https://cdn.b
+000008d0: 6f6f 7463 7373 2e63 6f6d 2f70 6f70 7065  ootcss.com/poppe
+000008e0: 722e 6a73 2f31 2e31 342e 332f 756d 642f  r.js/1.14.3/umd/
+000008f0: 706f 7070 6572 2e6d 696e 2e6a 7327 2c0d  popper.min.js',.
+00000900: 0a20 2020 2020 2020 2020 2020 2027 6874  .            'ht
+00000910: 7470 733a 2f2f 6364 6e2e 626f 6f74 6373  tps://cdn.bootcs
+00000920: 732e 636f 6d2f 626f 6f74 7374 7261 702f  s.com/bootstrap/
+00000930: 342e 312e 332f 6a73 2f62 6f6f 7473 7472  4.1.3/js/bootstr
+00000940: 6170 2e6d 696e 2e6a 7327 2c0d 0a20 2020  ap.min.js',..   
+00000950: 2020 2020 2020 2020 2027 636f 6d6d 6f6e           'common
+00000960: 5f74 6173 6b5f 7379 7374 656d 2f6a 732f  _task_system/js/
+00000970: 7461 736b 5f74 7970 655f 6164 6d69 6e2e  task_type_admin.
+00000980: 6a73 272c 0d0a 2020 2020 2020 2020 290d  js',..        ).
+00000990: 0a0d 0a0d 0a63 6c61 7373 2053 7973 7465  .....class Syste
+000009a0: 6d53 6368 6564 756c 6543 616c 6c62 6163  mScheduleCallbac
+000009b0: 6b41 646d 696e 2862 6173 655f 6164 6d69  kAdmin(base_admi
+000009c0: 6e2e 5461 736b 5363 6865 6475 6c65 4361  n.TaskScheduleCa
+000009d0: 6c6c 6261 636b 4164 6d69 6e29 3a0d 0a20  llbackAdmin):.. 
+000009e0: 2020 2070 6173 730d 0a0d 0a0d 0a63 6c61     pass......cla
+000009f0: 7373 2053 7973 7465 6d53 6368 6564 756c  ss SystemSchedul
+00000a00: 6541 646d 696e 2862 6173 655f 6164 6d69  eAdmin(base_admi
+00000a10: 6e2e 5461 736b 5363 6865 6475 6c65 4164  n.TaskScheduleAd
+00000a20: 6d69 6e29 3a0d 0a0d 0a20 2020 2074 6173  min):....    tas
+00000a30: 6b5f 6d6f 6465 6c20 3d20 6d6f 6465 6c73  k_model = models
+00000a40: 2e53 7973 7465 6d54 6173 6b0d 0a20 2020  .SystemTask..   
+00000a50: 2073 6368 6564 756c 655f 6c6f 675f 6d6f   schedule_log_mo
+00000a60: 6465 6c20 3d20 6d6f 6465 6c73 2e53 7973  del = models.Sys
+00000a70: 7465 6d53 6368 6564 756c 654c 6f67 0d0a  temScheduleLog..
+00000a80: 2020 2020 7175 6575 6573 203d 206d 6f64      queues = mod
+00000a90: 656c 732e 6275 696c 7469 6e73 2e71 7565  els.builtins.que
+00000aa0: 7565 730d 0a20 2020 2073 6368 6564 756c  ues..    schedul
+00000ab0: 655f 7075 745f 6e61 6d65 203d 2027 7379  e_put_name = 'sy
+00000ac0: 7374 656d 5f73 6368 6564 756c 655f 7075  stem_schedule_pu
+00000ad0: 7427 0d0a 2020 2020 6c69 7374 5f64 6973  t'..    list_dis
+00000ae0: 706c 6179 203d 2028 2769 6427 2c20 2761  play = ('id', 'a
+00000af0: 646d 696e 5f74 6173 6b27 2c20 2773 6368  dmin_task', 'sch
+00000b00: 6564 756c 655f 7479 7065 272c 2027 7363  edule_type', 'sc
+00000b10: 6865 6475 6c65 5f73 7562 5f74 7970 6527  hedule_sub_type'
+00000b20: 2c20 276e 6578 745f 7363 6865 6475 6c65  , 'next_schedule
+00000b30: 5f74 696d 6527 2c0d 0a20 2020 2020 2020  _time',..       
+00000b40: 2020 2020 2020 2020 2020 2020 2027 7374               'st
+00000b50: 6174 7573 272c 2027 7075 7427 2c20 276c  atus', 'put', 'l
+00000b60: 6f67 7327 2c20 2775 7064 6174 655f 7469  ogs', 'update_ti
+00000b70: 6d65 2729 0d0a 2020 2020 6c69 7374 5f66  me')..    list_f
+00000b80: 696c 7465 7220 3d20 2827 7461 736b 5f5f  ilter = ('task__
+00000b90: 6361 7465 676f 7279 272c 2029 0d0a 0d0a  category', )....
+00000ba0: 2020 2020 6465 6620 6861 735f 6465 6c65      def has_dele
+00000bb0: 7465 5f70 6572 6d69 7373 696f 6e28 7365  te_permission(se
+00000bc0: 6c66 2c20 7265 7175 6573 742c 206f 626a  lf, request, obj
+00000bd0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+00000be0: 2069 6620 6f62 6a3a 0d0a 2020 2020 2020   if obj:..      
+00000bf0: 2020 2020 2020 7265 7475 726e 206f 626a        return obj
+00000c00: 2e74 6173 6b2e 6361 7465 676f 7279 2021  .task.category !
+00000c10: 3d20 6d6f 6465 6c73 2e62 7569 6c74 696e  = models.builtin
+00000c20: 732e 6361 7465 676f 7269 6573 2e73 7973  s.categories.sys
+00000c30: 7465 6d5f 6465 6661 756c 745f 6361 7465  tem_default_cate
+00000c40: 676f 7279 0d0a 2020 2020 2020 2020 7265  gory..        re
+00000c50: 7475 726e 2054 7275 650d 0a0d 0a0d 0a63  turn True......c
+00000c60: 6c61 7373 2053 7973 7465 6d53 6368 6564  lass SystemSched
+00000c70: 756c 654c 6f67 4164 6d69 6e28 6261 7365  uleLogAdmin(base
+00000c80: 5f61 646d 696e 2e54 6173 6b53 6368 6564  _admin.TaskSched
+00000c90: 756c 654c 6f67 4164 6d69 6e29 3a0d 0a20  uleLogAdmin):.. 
+00000ca0: 2020 2073 6368 6564 756c 655f 7265 7472     schedule_retr
+00000cb0: 795f 6e61 6d65 203d 2027 7379 7374 656d  y_name = 'system
+00000cc0: 5f73 6368 6564 756c 655f 7265 7472 7927  _schedule_retry'
+00000cd0: 0d0a 0d0a 0d0a 636c 6173 7320 5379 7374  ......class Syst
+00000ce0: 656d 5072 6f63 6573 7341 646d 696e 2861  emProcessAdmin(a
+00000cf0: 646d 696e 2e4d 6f64 656c 4164 6d69 6e29  dmin.ModelAdmin)
+00000d00: 3a0d 0a20 2020 206c 6973 745f 6469 7370  :..    list_disp
+00000d10: 6c61 7920 3d20 2827 7072 6f63 6573 735f  lay = ('process_
+00000d20: 6964 272c 2027 7072 6f63 6573 735f 6e61  id', 'process_na
+00000d30: 6d65 272c 2027 6c6f 675f 6669 6c65 272c  me', 'log_file',
+00000d40: 2027 7374 6174 7573 272c 2027 7374 6f70   'status', 'stop
+00000d50: 5f70 726f 6365 7373 272c 2027 7368 6f77  _process', 'show
+00000d60: 5f6c 6f67 272c 2027 7570 6461 7465 5f74  _log', 'update_t
+00000d70: 696d 6527 290d 0a20 2020 2066 6f72 6d20  ime')..    form 
+00000d80: 3d20 666f 726d 732e 5379 7374 656d 5072  = forms.SystemPr
+00000d90: 6f63 6573 7346 6f72 6d0d 0a20 2020 2066  ocessForm..    f
+00000da0: 6965 6c64 7320 3d20 280d 0a20 2020 2020  ields = (..     
+00000db0: 2020 2027 7379 7374 656d 5f70 6174 6827     'system_path'
+00000dc0: 2c0d 0a20 2020 2020 2020 2027 7072 6f63  ,..        'proc
+00000dd0: 6573 735f 6e61 6d65 272c 0d0a 2020 2020  ess_name',..    
+00000de0: 2020 2020 2765 6e76 272c 0d0a 2020 2020      'env',..    
+00000df0: 2020 2020 276c 6f67 5f66 696c 6527 2c0d      'log_file',.
+00000e00: 0a20 2020 2020 2020 2027 7072 6f63 6573  .        'proces
+00000e10: 735f 6964 272c 0d0a 2020 2020 2020 2020  s_id',..        
+00000e20: 2763 7265 6174 655f 7469 6d65 272c 0d0a  'create_time',..
+00000e30: 2020 2020 290d 0a0d 0a20 2020 2072 6561      )....    rea
+00000e40: 646f 6e6c 795f 6669 656c 6473 203d 2028  donly_fields = (
+00000e50: 2763 7265 6174 655f 7469 6d65 272c 2027  'create_time', '
+00000e60: 7570 6461 7465 5f74 696d 6527 290d 0a0d  update_time')...
+00000e70: 0a20 2020 2064 6566 2073 746f 705f 7072  .    def stop_pr
+00000e80: 6f63 6573 7328 7365 6c66 2c20 6f62 6a29  ocess(self, obj)
+00000e90: 3a0d 0a20 2020 2020 2020 2075 726c 203d  :..        url =
+00000ea0: 2072 6576 6572 7365 2827 7379 7374 656d   reverse('system
+00000eb0: 5f70 726f 6365 7373 5f73 746f 7027 2c20  _process_stop', 
+00000ec0: 6172 6773 3d28 6f62 6a2e 7072 6f63 6573  args=(obj.proces
+00000ed0: 735f 6964 2c29 290d 0a20 2020 2020 2020  s_id,))..       
+00000ee0: 2072 6574 7572 6e20 666f 726d 6174 5f68   return format_h
+00000ef0: 746d 6c28 0d0a 2020 2020 2020 2020 2020  tml(..          
+00000f00: 2020 273c 6120 6872 6566 3d22 2573 2220    '<a href="%s" 
+00000f10: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000f20: e581 9ce6 ada2 3c2f 613e 2720 2520 7572  ......</a>' % ur
+00000f30: 6c0d 0a20 2020 2020 2020 2029 0d0a 2020  l..        )..  
+00000f40: 2020 7374 6f70 5f70 726f 6365 7373 2e73    stop_process.s
+00000f50: 686f 7274 5f64 6573 6372 6970 7469 6f6e  hort_description
+00000f60: 203d 2027 e581 9ce6 ada2 e8bf 90e8 a18c   = '............
+00000f70: 270d 0a0d 0a20 2020 2064 6566 2073 686f  '....    def sho
+00000f80: 775f 6c6f 6728 7365 6c66 2c20 6f62 6a29  w_log(self, obj)
+00000f90: 3a0d 0a20 2020 2020 2020 2075 726c 203d  :..        url =
+00000fa0: 2072 6576 6572 7365 2827 7379 7374 656d   reverse('system
+00000fb0: 5f70 726f 6365 7373 5f6c 6f67 272c 2061  _process_log', a
+00000fc0: 7267 733d 286f 626a 2e70 726f 6365 7373  rgs=(obj.process
+00000fd0: 5f69 642c 2929 0d0a 2020 2020 2020 2020  _id,))..        
+00000fe0: 7265 7475 726e 2066 6f72 6d61 745f 6874  return format_ht
+00000ff0: 6d6c 280d 0a20 2020 2020 2020 2020 2020  ml(..           
+00001000: 2027 3c61 2068 7265 663d 2225 7322 2074   '<a href="%s" t
+00001010: 6172 6765 743d 225f 626c 616e 6b22 3ee6  arget="_blank">.
+00001020: 9fa5 e79c 8be6 97a5 e5bf 973c 2f61 3e27  ...........</a>'
+00001030: 2025 2075 726c 0d0a 2020 2020 2020 2020   % url..        
+00001040: 290d 0a20 2020 2073 686f 775f 6c6f 672e  )..    show_log.
+00001050: 7368 6f72 745f 6465 7363 7269 7074 696f  short_descriptio
+00001060: 6e20 3d20 27e6 97a5 e5bf 9727 0d0a 0d0a  n = '......'....
+00001070: 2020 2020 6465 6620 6861 735f 6465 6c65      def has_dele
+00001080: 7465 5f70 6572 6d69 7373 696f 6e28 7365  te_permission(se
+00001090: 6c66 2c20 7265 7175 6573 742c 206f 626a  lf, request, obj
+000010a0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+000010b0: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
+000010c0: 0a0d 0a63 6c61 7373 2053 7973 7465 6d53  ...class SystemS
+000010d0: 6368 6564 756c 6551 7565 7565 4164 6d69  cheduleQueueAdmi
+000010e0: 6e28 6261 7365 5f61 646d 696e 2e54 6173  n(base_admin.Tas
+000010f0: 6b53 6368 6564 756c 6551 7565 7565 4164  kScheduleQueueAd
+00001100: 6d69 6e29 3a0d 0a20 2020 2066 6f72 6d20  min):..    form 
+00001110: 3d20 666f 726d 732e 5379 7374 656d 5363  = forms.SystemSc
+00001120: 6865 6475 6c65 5175 6575 6546 6f72 6d0d  heduleQueueForm.
+00001130: 0a20 2020 2062 7569 6c74 696e 7320 3d20  .    builtins = 
+00001140: 6d6f 6465 6c73 2e62 7569 6c74 696e 730d  models.builtins.
+00001150: 0a20 2020 2073 6368 6564 756c 655f 6765  .    schedule_ge
+00001160: 745f 6e61 6d65 203d 2027 7379 7374 656d  t_name = 'system
+00001170: 5f73 6368 6564 756c 655f 6765 7427 0d0a  _schedule_get'..
+00001180: 0d0a 0d0a 636c 6173 7320 5379 7374 656d  ....class System
+00001190: 5363 6865 6475 6c65 5072 6f64 7563 6572  ScheduleProducer
+000011a0: 4164 6d69 6e28 6261 7365 5f61 646d 696e  Admin(base_admin
+000011b0: 2e54 6173 6b53 6368 6564 756c 6550 726f  .TaskSchedulePro
+000011c0: 6475 6365 7241 646d 696e 293a 0d0a 2020  ducerAdmin):..  
+000011d0: 2020 666f 726d 203d 2066 6f72 6d73 2e53    form = forms.S
+000011e0: 7973 7465 6d53 6368 6564 756c 6550 726f  ystemSchedulePro
+000011f0: 6475 6365 7246 6f72 6d0d 0a20 2020 2073  ducerForm..    s
+00001200: 6368 6564 756c 655f 6765 745f 6e61 6d65  chedule_get_name
+00001210: 203d 2027 7379 7374 656d 5f73 6368 6564   = 'system_sched
+00001220: 756c 655f 6765 7427 0d0a 2020 2020 6275  ule_get'..    bu
+00001230: 696c 7469 6e73 203d 206d 6f64 656c 732e  iltins = models.
+00001240: 6275 696c 7469 6e73 0d0a 0d0a 0d0a 636c  builtins......cl
+00001250: 6173 7320 5379 7374 656d 436f 6e73 756d  ass SystemConsum
+00001260: 6572 5065 726d 6973 7369 6f6e 4164 6d69  erPermissionAdmi
+00001270: 6e28 6261 7365 5f61 646d 696e 2e43 6f6e  n(base_admin.Con
+00001280: 7375 6d65 7250 6572 6d69 7373 696f 6e41  sumerPermissionA
+00001290: 646d 696e 293a 0d0a 2020 2020 7061 7373  dmin):..    pass
+000012a0: 0d0a 0d0a 0d0a 636c 6173 7320 5379 7374  ......class Syst
+000012b0: 656d 4578 6365 7074 696f 6e41 646d 696e  emExceptionAdmin
+000012c0: 2862 6173 655f 6164 6d69 6e2e 4578 6365  (base_admin.Exce
+000012d0: 7074 696f 6e52 6570 6f72 7441 646d 696e  ptionReportAdmin
+000012e0: 293a 0d0a 2020 2020 7061 7373 0d0a 0d0a  ):..    pass....
+000012f0: 0d0a 6164 6d69 6e2e 7369 7465 2e72 6567  ..admin.site.reg
+00001300: 6973 7465 7228 6d6f 6465 6c73 2e53 7973  ister(models.Sys
+00001310: 7465 6d54 6173 6b2c 2053 7973 7465 6d54  temTask, SystemT
+00001320: 6173 6b41 646d 696e 290d 0a61 646d 696e  askAdmin)..admin
+00001330: 2e73 6974 652e 7265 6769 7374 6572 286d  .site.register(m
+00001340: 6f64 656c 732e 5379 7374 656d 5363 6865  odels.SystemSche
+00001350: 6475 6c65 4361 6c6c 6261 636b 2c20 5379  duleCallback, Sy
+00001360: 7374 656d 5363 6865 6475 6c65 4361 6c6c  stemScheduleCall
+00001370: 6261 636b 4164 6d69 6e29 0d0a 6164 6d69  backAdmin)..admi
+00001380: 6e2e 7369 7465 2e72 6567 6973 7465 7228  n.site.register(
+00001390: 6d6f 6465 6c73 2e53 7973 7465 6d53 6368  models.SystemSch
+000013a0: 6564 756c 652c 2053 7973 7465 6d53 6368  edule, SystemSch
+000013b0: 6564 756c 6541 646d 696e 290d 0a61 646d  eduleAdmin)..adm
+000013c0: 696e 2e73 6974 652e 7265 6769 7374 6572  in.site.register
+000013d0: 286d 6f64 656c 732e 5379 7374 656d 5363  (models.SystemSc
+000013e0: 6865 6475 6c65 4c6f 672c 2053 7973 7465  heduleLog, Syste
+000013f0: 6d53 6368 6564 756c 654c 6f67 4164 6d69  mScheduleLogAdmi
+00001400: 6e29 0d0a 6164 6d69 6e2e 7369 7465 2e72  n)..admin.site.r
+00001410: 6567 6973 7465 7228 6d6f 6465 6c73 2e53  egister(models.S
+00001420: 7973 7465 6d53 6368 6564 756c 6551 7565  ystemScheduleQue
+00001430: 7565 2c20 5379 7374 656d 5363 6865 6475  ue, SystemSchedu
+00001440: 6c65 5175 6575 6541 646d 696e 290d 0a61  leQueueAdmin)..a
+00001450: 646d 696e 2e73 6974 652e 7265 6769 7374  dmin.site.regist
+00001460: 6572 286d 6f64 656c 732e 5379 7374 656d  er(models.System
+00001470: 5363 6865 6475 6c65 5072 6f64 7563 6572  ScheduleProducer
+00001480: 2c20 5379 7374 656d 5363 6865 6475 6c65  , SystemSchedule
+00001490: 5072 6f64 7563 6572 4164 6d69 6e29 0d0a  ProducerAdmin)..
+000014a0: 6164 6d69 6e2e 7369 7465 2e72 6567 6973  admin.site.regis
+000014b0: 7465 7228 6d6f 6465 6c73 2e53 7973 7465  ter(models.Syste
+000014c0: 6d50 726f 6365 7373 2c20 5379 7374 656d  mProcess, System
+000014d0: 5072 6f63 6573 7341 646d 696e 290d 0a61  ProcessAdmin)..a
+000014e0: 646d 696e 2e73 6974 652e 7265 6769 7374  dmin.site.regist
+000014f0: 6572 286d 6f64 656c 732e 5379 7374 656d  er(models.System
+00001500: 436f 6e73 756d 6572 5065 726d 6973 7369  ConsumerPermissi
+00001510: 6f6e 2c20 5379 7374 656d 436f 6e73 756d  on, SystemConsum
+00001520: 6572 5065 726d 6973 7369 6f6e 4164 6d69  erPermissionAdmi
+00001530: 6e29 0d0a 6164 6d69 6e2e 7369 7465 2e72  n)..admin.site.r
+00001540: 6567 6973 7465 7228 6d6f 6465 6c73 2e53  egister(models.S
+00001550: 7973 7465 6d45 7863 6570 7469 6f6e 5265  ystemExceptionRe
+00001560: 706f 7274 2c20 5379 7374 656d 4578 6365  port, SystemExce
+00001570: 7074 696f 6e41 646d 696e 290d 0a0d 0a    ptionAdmin)....
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/choices.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# import queue
-# from django.db.models import TextChoices
-#
-#
-# class ScheduleQueueModule(TextChoices):
-#     QUEUE = "%s.%s" % (queue.Queue.__module__, queue.Queue.__name__), '普通队列'
-#     STACK = "%s.%s" % (queue.LifoQueue.__module__, queue.LifoQueue.__name__), '后进先出队列'
-#     PRIORITY_QUEUE = "%s.%s" % (queue.PriorityQueue.__module__, queue.PriorityQueue.__name__), '优先级队列'
-#     SIMPLE_QUEUE = "%s.%s" % (queue.SimpleQueue.__module__, queue.SimpleQueue.__name__), '简单队列'
-#     REDIS_LIST_QUEUE = "django_common_task_system.system_task.queue.RedisListQueue", 'Redis List队列'
+# import queue
+# from django.db.models import TextChoices
+#
+#
+# class ScheduleQueueModule(TextChoices):
+#     QUEUE = "%s.%s" % (queue.Queue.__module__, queue.Queue.__name__), '普通队列'
+#     STACK = "%s.%s" % (queue.LifoQueue.__module__, queue.LifoQueue.__name__), '后进先出队列'
+#     PRIORITY_QUEUE = "%s.%s" % (queue.PriorityQueue.__module__, queue.PriorityQueue.__name__), '优先级队列'
+#     SIMPLE_QUEUE = "%s.%s" % (queue.SimpleQueue.__module__, queue.SimpleQueue.__name__), '简单队列'
+#     REDIS_LIST_QUEUE = "django_common_task_system.system_task.queue.RedisListQueue", 'Redis List队列'
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# Generated by Django 4.1.7 on 2023-04-07 16:41
-
-import datetime
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-import django.utils.timezone
-import django_common_objects.fields
-import django_common_objects.models
-import django_common_task_system.fields
-import django_common_task_system.system_task.models
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('django_common_objects', '0002_alter_commoncategory_model_and_more'),
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='SystemProcess',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('process_id', models.PositiveIntegerField(unique=True, verbose_name='进程ID')),
-                ('process_name', models.CharField(max_length=100, verbose_name='进程名称')),
-                ('env', models.CharField(blank=True, max_length=500, null=True, verbose_name='环境变量')),
-                ('status', models.BooleanField(default=True, verbose_name='状态')),
-                ('log_file', models.CharField(max_length=200, verbose_name='日志文件')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-            ],
-            options={
-                'verbose_name': '系统进程',
-                'verbose_name_plural': '系统进程',
-                'db_table': 'system_process',
-            },
-        ),
-        migrations.CreateModel(
-            name='SystemSchedule',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('priority', models.IntegerField(default=0, verbose_name='优先级')),
-                ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
-                ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
-                ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
-                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
-                ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-            ],
-            options={
-                'verbose_name': '系统计划',
-                'verbose_name_plural': '系统计划',
-                'db_table': 'system_schedule',
-                'ordering': ('-update_time',),
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='SystemScheduleQueue',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100, unique=True, verbose_name='队列名称')),
-                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.models.code_validator], verbose_name='队列编码')),
-                ('status', models.BooleanField(default=True, verbose_name='状态')),
-                ('module', models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列')], default='queue.Queue', max_length=100, verbose_name='队列类型')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-            ],
-            options={
-                'verbose_name': '系统队列',
-                'verbose_name_plural': '系统队列',
-                'db_table': 'system_schedule_queue',
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='SystemTask',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=100, verbose_name='任务名')),
-                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('Task'), null=True, verbose_name='参数')),
-                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('task_type', models.CharField(choices=[('SQL_TASK_EXECUTION', 'SQL任务执行'), ('SQL_TASK_PRODUCE', 'SQL任务生产'), ('SHELL_EXECUTION', 'SHELL任务执行'), ('CUSTOM', '自定义任务')], default='SQL_TASK_PRODUCE', max_length=32, verbose_name='任务类型')),
-                ('category', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_objects.commoncategory', verbose_name='类别')),
-                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to='system_task.systemtask', verbose_name='父任务')),
-                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
-            ],
-            options={
-                'verbose_name': '系统任务',
-                'verbose_name_plural': '系统任务',
-                'db_table': 'system_task',
-                'abstract': False,
-                'unique_together': {('name', 'user', 'parent')},
-            },
-        ),
-        migrations.CreateModel(
-            name='SystemScheduleLog',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
-                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
-                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='logs', to='system_task.systemschedule', verbose_name='任务计划')),
-            ],
-            options={
-                'verbose_name': '系统日志',
-                'verbose_name_plural': '系统日志',
-                'db_table': 'system_schedule_log',
-                'ordering': ('-schedule_time',),
-                'abstract': False,
-            },
-        ),
-        migrations.CreateModel(
-            name='SystemScheduleCallback',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False)),
-                ('name', models.CharField(max_length=100, verbose_name='回调')),
-                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
-                ('trigger_event', django_common_objects.fields.CharField(choices=[('S', '成功'), ('F', '失败'), ('D', '完成')], default='D', max_length=1, verbose_name='触发事件')),
-                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('TaskCallback'), null=True, verbose_name='参数')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='callbacks', to='system_task.systemschedulequeue', verbose_name='队列')),
-                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
-            ],
-            options={
-                'verbose_name': '系统回调',
-                'verbose_name_plural': '系统回调',
-                'db_table': 'system_schedule_callback',
-                'abstract': False,
-                'unique_together': {('name', 'user')},
-            },
-        ),
-        migrations.AddField(
-            model_name='systemschedule',
-            name='callback',
-            field=models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, to='system_task.systemschedulecallback', verbose_name='回调'),
-        ),
-        migrations.AddField(
-            model_name='systemschedule',
-            name='task',
-            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='schedules', to='system_task.systemtask', verbose_name='任务'),
-        ),
-        migrations.AddField(
-            model_name='systemschedule',
-            name='user',
-            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户'),
-        ),
-        migrations.AlterUniqueTogether(
-            name='systemschedule',
-            unique_together={('task', 'status', 'user')},
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-07 16:41
+
+import datetime
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+import django.utils.timezone
+import django_common_objects.fields
+import django_common_objects.models
+import django_common_task_system.fields
+import django_common_task_system.system_task.models
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('django_common_objects', '0002_alter_commoncategory_model_and_more'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='SystemProcess',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('process_id', models.PositiveIntegerField(unique=True, verbose_name='进程ID')),
+                ('process_name', models.CharField(max_length=100, verbose_name='进程名称')),
+                ('env', models.CharField(blank=True, max_length=500, null=True, verbose_name='环境变量')),
+                ('status', models.BooleanField(default=True, verbose_name='状态')),
+                ('log_file', models.CharField(max_length=200, verbose_name='日志文件')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+            ],
+            options={
+                'verbose_name': '系统进程',
+                'verbose_name_plural': '系统进程',
+                'db_table': 'system_process',
+            },
+        ),
+        migrations.CreateModel(
+            name='SystemSchedule',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('priority', models.IntegerField(default=0, verbose_name='优先级')),
+                ('next_schedule_time', models.DateTimeField(db_index=True, default=django.utils.timezone.now, verbose_name='下次运行时间')),
+                ('schedule_start_time', models.DateTimeField(default=datetime.datetime(1, 1, 1, 0, 0), verbose_name='开始时间')),
+                ('schedule_end_time', models.DateTimeField(default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), verbose_name='结束时间')),
+                ('config', django_common_task_system.fields.ScheduleConfigField(default=dict, verbose_name='参数')),
+                ('status', django_common_objects.fields.CharField(choices=[('O', '开启'), ('C', '关闭'), ('D', '已完成'), ('T', '测试'), ('E', '调度错误')], default='O', max_length=1, verbose_name='状态')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+            ],
+            options={
+                'verbose_name': '系统计划',
+                'verbose_name_plural': '系统计划',
+                'db_table': 'system_schedule',
+                'ordering': ('-update_time',),
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='SystemScheduleQueue',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, unique=True, verbose_name='队列名称')),
+                ('code', models.CharField(max_length=100, unique=True, validators=[django_common_task_system.models.code_validator], verbose_name='队列编码')),
+                ('status', models.BooleanField(default=True, verbose_name='状态')),
+                ('module', models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列')], default='queue.Queue', max_length=100, verbose_name='队列类型')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+            ],
+            options={
+                'verbose_name': '系统队列',
+                'verbose_name_plural': '系统队列',
+                'db_table': 'system_schedule_queue',
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='SystemTask',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=100, verbose_name='任务名')),
+                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('Task'), null=True, verbose_name='参数')),
+                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('task_type', models.CharField(choices=[('SQL_TASK_EXECUTION', 'SQL任务执行'), ('SQL_TASK_PRODUCE', 'SQL任务生产'), ('SHELL_EXECUTION', 'SHELL任务执行'), ('CUSTOM', '自定义任务')], default='SQL_TASK_PRODUCE', max_length=32, verbose_name='任务类型')),
+                ('category', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.DO_NOTHING, to='django_common_objects.commoncategory', verbose_name='类别')),
+                ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to='system_task.systemtask', verbose_name='父任务')),
+                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
+            ],
+            options={
+                'verbose_name': '系统任务',
+                'verbose_name_plural': '系统任务',
+                'db_table': 'system_task',
+                'abstract': False,
+                'unique_together': {('name', 'user', 'parent')},
+            },
+        ),
+        migrations.CreateModel(
+            name='SystemScheduleLog',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('status', django_common_objects.fields.CharField(max_length=1, verbose_name='运行状态')),
+                ('result', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='结果')),
+                ('schedule_time', models.DateTimeField(verbose_name='计划时间')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('schedule', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='logs', to='system_task.systemschedule', verbose_name='任务计划')),
+            ],
+            options={
+                'verbose_name': '系统日志',
+                'verbose_name_plural': '系统日志',
+                'db_table': 'system_schedule_log',
+                'ordering': ('-schedule_time',),
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='SystemScheduleCallback',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False)),
+                ('name', models.CharField(max_length=100, verbose_name='回调')),
+                ('description', models.TextField(blank=True, null=True, verbose_name='描述')),
+                ('trigger_event', django_common_objects.fields.CharField(choices=[('S', '成功'), ('F', '失败'), ('D', '完成')], default='D', max_length=1, verbose_name='触发事件')),
+                ('status', django_common_objects.fields.CharField(choices=[('E', '启用'), ('D', '禁用')], default='E', max_length=1, verbose_name='状态')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('TaskCallback'), null=True, verbose_name='参数')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='callbacks', to='system_task.systemschedulequeue', verbose_name='队列')),
+                ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
+            ],
+            options={
+                'verbose_name': '系统回调',
+                'verbose_name_plural': '系统回调',
+                'db_table': 'system_schedule_callback',
+                'abstract': False,
+                'unique_together': {('name', 'user')},
+            },
+        ),
+        migrations.AddField(
+            model_name='systemschedule',
+            name='callback',
+            field=models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, to='system_task.systemschedulecallback', verbose_name='回调'),
+        ),
+        migrations.AddField(
+            model_name='systemschedule',
+            name='task',
+            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='schedules', to='system_task.systemtask', verbose_name='任务'),
+        ),
+        migrations.AddField(
+            model_name='systemschedule',
+            name='user',
+            field=models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户'),
+        ),
+        migrations.AlterUniqueTogether(
+            name='systemschedule',
+            unique_together={('task', 'status', 'user')},
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Generated by Django 4.1.7 on 2023-04-13 13:28
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('system_task', '0002_remove_systemtask_task_type_systemtask_tags'),
-    ]
-
-    operations = [
-        migrations.AddField(
-            model_name='systemschedulequeue',
-            name='config',
-            field=models.JSONField(default=dict, verbose_name='配置'),
-        ),
-        migrations.AlterField(
-            model_name='systemschedulequeue',
-            name='module',
-            field=models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列'), ('django_common_task_system.system_task.queue.RedisListQueue', 'Redis List队列')], default='queue.Queue', max_length=100, verbose_name='队列类型'),
-        ),
-        migrations.CreateModel(
-            name='SystemScheduleProducer',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100, verbose_name='生产者名称')),
-                ('filters', models.JSONField(verbose_name='过滤器')),
-                ('lte_now', models.BooleanField(default=True, verbose_name='小于等于当前时间')),
-                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='producers', to='system_task.systemschedulequeue', verbose_name='队列')),
-            ],
-            options={
-                'verbose_name': '计划生产',
-                'verbose_name_plural': '计划生产',
-                'db_table': 'system_schedule_producer',
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-13 13:28
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('system_task', '0002_remove_systemtask_task_type_systemtask_tags'),
+    ]
+
+    operations = [
+        migrations.AddField(
+            model_name='systemschedulequeue',
+            name='config',
+            field=models.JSONField(default=dict, verbose_name='配置'),
+        ),
+        migrations.AlterField(
+            model_name='systemschedulequeue',
+            name='module',
+            field=models.CharField(choices=[('queue.Queue', '普通队列'), ('queue.LifoQueue', '后进先出队列'), ('queue.PriorityQueue', '优先级队列'), ('_queue.SimpleQueue', '简单队列'), ('django_common_task_system.system_task.queue.RedisListQueue', 'Redis List队列')], default='queue.Queue', max_length=100, verbose_name='队列类型'),
+        ),
+        migrations.CreateModel(
+            name='SystemScheduleProducer',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, verbose_name='生产者名称')),
+                ('filters', models.JSONField(verbose_name='过滤器')),
+                ('lte_now', models.BooleanField(default=True, verbose_name='小于等于当前时间')),
+                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('queue', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, related_name='producers', to='system_task.systemschedulequeue', verbose_name='队列')),
+            ],
+            options={
+                'verbose_name': '计划生产',
+                'verbose_name_plural': '计划生产',
+                'db_table': 'system_schedule_producer',
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.6/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Generated by Django 4.1.7 on 2023-04-17 16:33
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('system_task', '0005_alter_systemscheduleproducer_name'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='SystemConsumerPermission',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('type', models.CharField(choices=[('I', 'IP白名单')], default='I', max_length=1, verbose_name='类型')),
-                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
-                ('config', models.JSONField(blank=True, default=dict, null=True, verbose_name='配置')),
-                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
-                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
-                ('producer', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to='system_task.systemscheduleproducer', verbose_name='生产者')),
-            ],
-            options={
-                'verbose_name': '消费权限',
-                'verbose_name_plural': '消费权限',
-                'db_table': 'system_consumer_permission',
-                'abstract': False,
-                'unique_together': {('producer', 'status')},
-            },
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-17 16:33
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('django_common_task_system', '0005_alter_taskscheduleproducer_name'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='ConsumerPermission',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('type', models.CharField(choices=[('I', 'IP白名单')], default='I', max_length=1, verbose_name='类型')),
+                ('status', models.BooleanField(default=True, verbose_name='启用状态')),
+                ('config', models.JSONField(blank=True, default=dict, null=True, verbose_name='配置')),
+                ('create_time', models.DateTimeField(auto_now_add=True, verbose_name='创建时间')),
+                ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
+                ('producer', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to='django_common_task_system.taskscheduleproducer', verbose_name='生产者')),
+            ],
+            options={
+                'verbose_name': '消费权限',
+                'verbose_name_plural': '消费权限',
+                'db_table': 'schedule_consumer_permission',
+                'abstract': False,
+                'unique_together': {('producer', 'status')},
+            },
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Generated by Django 4.1.7 on 2023-04-21 15:23
-
-from django.db import migrations, models
-import django.utils.timezone
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('system_task', '0006_systemconsumerpermission'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='SystemExceptionReport',
-            fields=[
-                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
-                ('ip', models.CharField(max_length=100, verbose_name='IP')),
-                ('content', models.TextField(verbose_name='内容')),
-                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
-            ],
-            options={
-                'verbose_name': '异常报告',
-                'verbose_name_plural': '异常报告',
-                'db_table': 'system_exception_report',
-                'ordering': ('-create_time',),
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 4.1.7 on 2023-04-21 15:23
+
+from django.db import migrations, models
+import django.utils.timezone
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('system_task', '0006_systemconsumerpermission'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='SystemExceptionReport',
+            fields=[
+                ('id', models.AutoField(primary_key=True, serialize=False, verbose_name='ID')),
+                ('ip', models.CharField(max_length=100, verbose_name='IP')),
+                ('content', models.TextField(verbose_name='内容')),
+                ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
+            ],
+            options={
+                'verbose_name': '异常报告',
+                'verbose_name_plural': '异常报告',
+                'db_table': 'system_exception_report',
+                'ordering': ('-create_time',),
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,423 +1,423 @@
-from django.db import models
-from django.conf import settings
-from django_common_task_system.choices import ScheduleQueueModule, TaskScheduleStatus, ConsumerPermissionType
-from django_common_task_system.models import (
-    AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, TaskScheduleLog, AbstractScheduleCallback, 
-    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, AbstractExceptionReport,
-    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins,
-    BuiltinModels
-)
-from django_common_objects.models import CommonCategory
-from django.contrib.auth import get_user_model
-
-User = get_user_model()
-
-
-class SystemTask(AbstractTask):
-
-    class Meta(AbstractTask.Meta):
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-        db_table = 'system_task'
-        verbose_name = verbose_name_plural = '系统任务'
-
-    def save(
-        self, force_insert=False, force_update=False, using=None, update_fields=None
-    ):
-        if self.category_id is None:
-            self.category = builtins.categories.system_default_category
-        super().save(force_insert, force_update, using, update_fields)
-
-
-class SystemScheduleQueue(AbstractTaskScheduleQueue):
-
-    class Meta(AbstractTaskScheduleQueue.Meta):
-        db_table = 'system_schedule_queue'
-        verbose_name = verbose_name_plural = '系统队列'
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemScheduleCallback(AbstractScheduleCallback):
-    queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='callbacks',
-                              on_delete=models.CASCADE, verbose_name='队列')
-
-    class Meta(AbstractScheduleCallback.Meta):
-        db_table = 'system_schedule_callback'
-        verbose_name = verbose_name_plural = '系统回调'
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemSchedule(AbstractTaskSchedule):
-    task = models.ForeignKey(SystemTask, db_constraint=False, related_name='schedules',
-                             on_delete=models.CASCADE, verbose_name='任务')
-    callback = models.ForeignKey(SystemScheduleCallback, on_delete=models.CASCADE,
-                                 null=True, blank=True, db_constraint=False, verbose_name='回调')
-
-    class Meta(AbstractTaskSchedule.Meta):
-        db_table = 'system_schedule'
-        verbose_name = verbose_name_plural = '系统计划'
-        ordering = ('-update_time',)
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemScheduleProducer(AbstractTaskScheduleProducer):
-    queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='producers',
-                              on_delete=models.CASCADE, verbose_name='队列')
-
-    class Meta(AbstractTaskScheduleProducer.Meta):
-        db_table = 'system_schedule_producer'
-        verbose_name = verbose_name_plural = '计划生产'
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemScheduleLog(AbstractTaskScheduleLog):
-    schedule = models.ForeignKey(SystemSchedule, db_constraint=False, related_name='logs',
-                                 on_delete=models.CASCADE, verbose_name='任务计划')
-
-    class Meta(AbstractTaskScheduleLog.Meta):
-        db_table = 'system_schedule_log'
-        verbose_name = verbose_name_plural = '系统日志'
-        ordering = ('-schedule_time',)
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemConsumerPermission(AbstractConsumerPermission):
-    producer = models.ForeignKey(SystemScheduleProducer, db_constraint=False,
-                                 on_delete=models.CASCADE, verbose_name='生产者')
-
-    class Meta(AbstractConsumerPermission.Meta):
-        db_table = 'system_consumer_permission'
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemExceptionReport(AbstractExceptionReport):
-
-    class Meta(AbstractExceptionReport.Meta):
-        db_table = 'system_exception_report'
-        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
-
-
-class SystemProcess(models.Model):
-    id = models.AutoField(primary_key=True, verbose_name='ID')
-    process_id = models.PositiveIntegerField(verbose_name='进程ID', unique=True)
-    process_name = models.CharField(max_length=100, verbose_name='进程名称')
-    env = models.CharField(max_length=500, verbose_name='环境变量', blank=True, null=True)
-    status = models.BooleanField(default=True, verbose_name='状态')
-    log_file = models.CharField(max_length=200, verbose_name='日志文件')
-    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
-    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
-
-    class Meta:
-        db_table = 'system_process'
-        verbose_name = verbose_name_plural = '系统进程'
-
-    def __str__(self):
-        return "%s(%s)" % (self.process_name, self.process_id)
-
-
-class BuiltinCategories(BuiltinModels):
-    model = CommonCategory
-    model_unique_kwargs = ('name',)
-
-    def __init__(self, user):
-        model = SystemTask._meta.label
-        self.system_default_category = self.model(
-            name='系统任务',
-            model=model,
-            user=user,
-        )
-
-        self.system_base_category = self.model(
-            name='系统基础',
-            model=model,
-            user=user,
-        )
-
-        self.system_test_category = self.model(
-            name='系统测试',
-            model=model,
-            user=user,
-        )
-        super(BuiltinCategories, self).__init__()
-
-
-class BuiltinQueues(BaseBuiltinQueues):
-    model = SystemScheduleQueue
-
-    def __init__(self):
-        self.opening = self.model(
-            code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
-            status=True,
-            module=ScheduleQueueModule.QUEUE.value,
-            name='系统任务队列'
-        )
-
-        self.test = self.model(
-            code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
-            status=True,
-            module=ScheduleQueueModule.QUEUE.value,
-            name='测试任务队列'
-        )
-        super(BuiltinQueues, self).__init__()
-
-
-class BuiltinProducers(BaseBuiltinProducers):
-    model = SystemScheduleProducer
-
-    def __init__(self, queues: BuiltinQueues):
-        self.opening = self.model(
-            queue=queues.opening,
-            lte_now=True,
-            filters={
-                'status': TaskScheduleStatus.OPENING.value,
-            },
-            status=True,
-            name='默认'
-        )
-        self.test = self.model(
-            queue=queues.test,
-            lte_now=True,
-            filters={
-                'status': TaskScheduleStatus.TEST.value,
-            },
-            status=True,
-            name='测试'
-        )
-        super(BuiltinProducers, self).__init__()
-
-
-class BuiltinTasks(BuiltinModels):
-    model = SystemTask
-    model_unique_kwargs = ['name', 'user', 'parent', 'category']
-
-    def __init__(self, categories: BuiltinCategories, queues: BuiltinQueues):
-        user = categories.system_default_category.user
-
-        self.shell_execution_parent_task = self.model(
-            name='Shell执行',
-            user=user,
-            category=categories.system_base_category,
-            config={
-                'required_fields': ['shell'],
-            }
-        )
-        self.sql_execution_parent_task = self.model(
-            name='SQL执行',
-            user=user,
-            category=categories.system_base_category,
-            config={
-                'required_fields': ['sql'],
-            }
-        )
-
-        self.sql_produce_parent_task = self.model(
-            name='SQL生产',
-            user=user,
-            category=categories.system_base_category,
-            config={
-                'required_fields': ['sql', 'queue'],
-            }
-        )
-
-        interval = 1
-        unit = 'month'
-        self.system_log_cleaning = self.model(
-            name='系统日志清理',
-            parent=self.sql_execution_parent_task,
-            category=categories.system_default_category,
-            user=user,
-            config={
-                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
-                       (SystemScheduleLog._meta.db_table, interval, unit)
-            },
-        )
-
-        max_retry_times = 5
-        self.system_exception_handling = self.model(
-            name='系统异常处理',
-            user=user,
-            category=categories.system_default_category,
-            config={
-                'max_retry_times': max_retry_times,
-            },
-        )
-
-        interval = 1
-        unit = 'month'
-        self.task_log_cleaning = self.model(
-            name='任务日志清理',
-            user=user,
-            category=categories.system_default_category,
-            parent=self.sql_execution_parent_task,
-            config={
-                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
-                       (TaskScheduleLog._meta.db_table, interval, unit)
-            },
-        )
-
-        max_retry_times = 5
-        self.task_exception_handling = self.model(
-            name='任务异常处理',
-            user=user,
-            category=categories.system_default_category,
-            config={
-                'max_retry_times': max_retry_times,
-            },
-        )
-
-        self.test_sql_execution = self.model(
-            name='测试SQL执行任务',
-            parent=self.sql_execution_parent_task,
-            category=categories.system_test_category,
-            config={
-                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table
-            },
-            user=user
-        )
-
-        self.test_sql_produce = self.model(
-            name='测试SQL生产任务',
-            parent=self.sql_produce_parent_task,
-            category=categories.system_test_category,
-            config={
-                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
-                'queue': queues.test.code
-            },
-            user=user
-        )
-        self.test_shell_execution = self.model(
-            name='测试Shell执行任务',
-            parent=self.shell_execution_parent_task,
-            category=categories.system_test_category,
-            config={
-                'shell': 'echo "hello world"'
-            },
-            user=user
-        )
-        super(BuiltinTasks, self).__init__()
-
-
-class BuiltinSchedules(BuiltinModels):
-    model_unique_kwargs = ['task', 'user']
-    model = SystemSchedule
-
-    def __init__(self, user, tasks: BuiltinTasks):
-        self.system_log_cleaning = self.model(
-            task=tasks.system_log_cleaning,
-            user=user,
-            config={
-                "T": {
-                    "DAY": {
-                        "period": 1
-                    },
-                    "time": "01:00:00",
-                    "type": "DAY"
-                },
-                "base_on_now": True,
-                "schedule_type": "T"
-            }
-        )
-
-        self.system_exception_handling = self.model(
-            task=tasks.system_exception_handling,
-            user=user,
-            config={
-                "S": {
-                    "period": 60,
-                    "schedule_start_time": "2023-04-04 15:31:00"
-                },
-                "base_on_now": True,
-                "schedule_type": "S"
-            }
-        )
-
-        self.task_log_cleaning = self.model(
-            task=tasks.task_log_cleaning,
-            user=user,
-            config={
-                "T": {
-                    "DAY": {
-                        "period": 1
-                    },
-                    "time": "01:00:00",
-                    "type": "DAY"
-                },
-                "base_on_now": True,
-                "schedule_type": "T"
-            }
-        )
-
-        self.task_exception_handling = self.model(
-            task=tasks.task_exception_handling,
-            user=user,
-            config={
-                "S": {
-                    "period": 60,
-                    "schedule_start_time": "2023-04-04 15:31:00"
-                },
-                "base_on_now": True,
-                "schedule_type": "S"
-            }
-        )
-
-        config = {
-            'config': {
-                "S": {
-                    "period": 60,
-                    "schedule_start_time": "2023-04-04 15:31:00"
-                },
-                "base_on_now": True,
-                "schedule_type": "S"
-            }
-        }
-
-        self.test_sql_execution = self.model(
-            task=tasks.test_sql_execution,
-            user=user,
-            status=TaskScheduleStatus.TEST.value,
-            config=config
-        )
-        self.test_sql_produce = self.model(
-            task=tasks.test_sql_produce,
-            user=user,
-            status=TaskScheduleStatus.TEST.value,
-            config=config
-        )
-        self.test_shell_execution = self.model(
-            task=tasks.test_shell_execution,
-            user=user,
-            status=TaskScheduleStatus.TEST.value,
-            config=config
-        )
-
-        super(BuiltinSchedules, self).__init__()
-
-
-class BuiltinConsumerPermissions(BaseConsumerPermissions):
-    model = SystemConsumerPermission
-
-    def __init__(self, producers: BuiltinProducers):
-        self.system_consumer_permission = self.model(
-            producer=producers.opening,
-            type=ConsumerPermissionType.IP_WHITE_LIST.value,
-            status=True,
-            config={
-                'ip_whitelist': ['127.0.0.1']
-            }
-        )
-        super(BuiltinConsumerPermissions, self).__init__()
-
-
-class Builtins(BaseBuiltins):
-    app = 'django_common_task_system.system_task'
-
-    def __init__(self):
-        super(Builtins, self).__init__()
-        self.queues = BuiltinQueues()
-        self.categories = BuiltinCategories(self.user)
-        self.tasks = BuiltinTasks(self.categories, self.queues)
-        self.schedules = BuiltinSchedules(self.user, self.tasks)
-        self.producers = BuiltinProducers(self.queues)
-        self.consumer_permissions = BuiltinConsumerPermissions(self.producers)
-
-
-builtins = Builtins()
+from django.db import models
+from django.conf import settings
+from django_common_task_system.choices import ScheduleQueueModule, TaskScheduleStatus, ConsumerPermissionType
+from django_common_task_system.models import (
+    AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, TaskScheduleLog, AbstractScheduleCallback, 
+    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, AbstractExceptionReport,
+    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins,
+    BuiltinModels
+)
+from django_common_objects.models import CommonCategory
+from django.contrib.auth import get_user_model
+
+User = get_user_model()
+
+
+class SystemTask(AbstractTask):
+
+    class Meta(AbstractTask.Meta):
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+        db_table = 'system_task'
+        verbose_name = verbose_name_plural = '系统任务'
+
+    def save(
+        self, force_insert=False, force_update=False, using=None, update_fields=None
+    ):
+        if self.category_id is None:
+            self.category = builtins.categories.system_default_category
+        super().save(force_insert, force_update, using, update_fields)
+
+
+class SystemScheduleQueue(AbstractTaskScheduleQueue):
+
+    class Meta(AbstractTaskScheduleQueue.Meta):
+        db_table = 'system_schedule_queue'
+        verbose_name = verbose_name_plural = '系统队列'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemScheduleCallback(AbstractScheduleCallback):
+    queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='callbacks',
+                              on_delete=models.CASCADE, verbose_name='队列')
+
+    class Meta(AbstractScheduleCallback.Meta):
+        db_table = 'system_schedule_callback'
+        verbose_name = verbose_name_plural = '系统回调'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemSchedule(AbstractTaskSchedule):
+    task = models.ForeignKey(SystemTask, db_constraint=False, related_name='schedules',
+                             on_delete=models.CASCADE, verbose_name='任务')
+    callback = models.ForeignKey(SystemScheduleCallback, on_delete=models.CASCADE,
+                                 null=True, blank=True, db_constraint=False, verbose_name='回调')
+
+    class Meta(AbstractTaskSchedule.Meta):
+        db_table = 'system_schedule'
+        verbose_name = verbose_name_plural = '系统计划'
+        ordering = ('-update_time',)
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemScheduleProducer(AbstractTaskScheduleProducer):
+    queue = models.ForeignKey(SystemScheduleQueue, db_constraint=False, related_name='producers',
+                              on_delete=models.CASCADE, verbose_name='队列')
+
+    class Meta(AbstractTaskScheduleProducer.Meta):
+        db_table = 'system_schedule_producer'
+        verbose_name = verbose_name_plural = '计划生产'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemScheduleLog(AbstractTaskScheduleLog):
+    schedule = models.ForeignKey(SystemSchedule, db_constraint=False, related_name='logs',
+                                 on_delete=models.CASCADE, verbose_name='任务计划')
+
+    class Meta(AbstractTaskScheduleLog.Meta):
+        db_table = 'system_schedule_log'
+        verbose_name = verbose_name_plural = '系统日志'
+        ordering = ('-schedule_time',)
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemConsumerPermission(AbstractConsumerPermission):
+    producer = models.ForeignKey(SystemScheduleProducer, db_constraint=False,
+                                 on_delete=models.CASCADE, verbose_name='生产者')
+
+    class Meta(AbstractConsumerPermission.Meta):
+        db_table = 'system_consumer_permission'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemExceptionReport(AbstractExceptionReport):
+
+    class Meta(AbstractExceptionReport.Meta):
+        db_table = 'system_exception_report'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
+class SystemProcess(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    process_id = models.PositiveIntegerField(verbose_name='进程ID', unique=True)
+    process_name = models.CharField(max_length=100, verbose_name='进程名称')
+    env = models.CharField(max_length=500, verbose_name='环境变量', blank=True, null=True)
+    status = models.BooleanField(default=True, verbose_name='状态')
+    log_file = models.CharField(max_length=200, verbose_name='日志文件')
+    create_time = models.DateTimeField(auto_now_add=True, verbose_name='创建时间')
+    update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
+
+    class Meta:
+        db_table = 'system_process'
+        verbose_name = verbose_name_plural = '系统进程'
+
+    def __str__(self):
+        return "%s(%s)" % (self.process_name, self.process_id)
+
+
+class BuiltinCategories(BuiltinModels):
+    model = CommonCategory
+    model_unique_kwargs = ('name',)
+
+    def __init__(self, user):
+        model = SystemTask._meta.label
+        self.system_default_category = self.model(
+            name='系统任务',
+            model=model,
+            user=user,
+        )
+
+        self.system_base_category = self.model(
+            name='系统基础',
+            model=model,
+            user=user,
+        )
+
+        self.system_test_category = self.model(
+            name='系统测试',
+            model=model,
+            user=user,
+        )
+        super(BuiltinCategories, self).__init__()
+
+
+class BuiltinQueues(BaseBuiltinQueues):
+    model = SystemScheduleQueue
+
+    def __init__(self):
+        self.opening = self.model(
+            code=self.status_params_mapping[TaskScheduleStatus.OPENING.value],
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='系统任务队列'
+        )
+
+        self.test = self.model(
+            code=self.status_params_mapping[TaskScheduleStatus.TEST.value],
+            status=True,
+            module=ScheduleQueueModule.QUEUE.value,
+            name='测试任务队列'
+        )
+        super(BuiltinQueues, self).__init__()
+
+
+class BuiltinProducers(BaseBuiltinProducers):
+    model = SystemScheduleProducer
+
+    def __init__(self, queues: BuiltinQueues):
+        self.opening = self.model(
+            queue=queues.opening,
+            lte_now=True,
+            filters={
+                'status': TaskScheduleStatus.OPENING.value,
+            },
+            status=True,
+            name='默认'
+        )
+        self.test = self.model(
+            queue=queues.test,
+            lte_now=True,
+            filters={
+                'status': TaskScheduleStatus.TEST.value,
+            },
+            status=True,
+            name='测试'
+        )
+        super(BuiltinProducers, self).__init__()
+
+
+class BuiltinTasks(BuiltinModels):
+    model = SystemTask
+    model_unique_kwargs = ['name', 'user', 'parent', 'category']
+
+    def __init__(self, categories: BuiltinCategories, queues: BuiltinQueues):
+        user = categories.system_default_category.user
+
+        self.shell_execution_parent_task = self.model(
+            name='Shell执行',
+            user=user,
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['shell'],
+            }
+        )
+        self.sql_execution_parent_task = self.model(
+            name='SQL执行',
+            user=user,
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['sql'],
+            }
+        )
+
+        self.sql_produce_parent_task = self.model(
+            name='SQL生产',
+            user=user,
+            category=categories.system_base_category,
+            config={
+                'required_fields': ['sql', 'queue'],
+            }
+        )
+
+        interval = 1
+        unit = 'month'
+        self.system_log_cleaning = self.model(
+            name='系统日志清理',
+            parent=self.sql_execution_parent_task,
+            category=categories.system_default_category,
+            user=user,
+            config={
+                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                       (SystemScheduleLog._meta.db_table, interval, unit)
+            },
+        )
+
+        max_retry_times = 5
+        self.system_exception_handling = self.model(
+            name='系统异常处理',
+            user=user,
+            category=categories.system_default_category,
+            config={
+                'max_retry_times': max_retry_times,
+            },
+        )
+
+        interval = 1
+        unit = 'month'
+        self.task_log_cleaning = self.model(
+            name='任务日志清理',
+            user=user,
+            category=categories.system_default_category,
+            parent=self.sql_execution_parent_task,
+            config={
+                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                       (TaskScheduleLog._meta.db_table, interval, unit)
+            },
+        )
+
+        max_retry_times = 5
+        self.task_exception_handling = self.model(
+            name='任务异常处理',
+            user=user,
+            category=categories.system_default_category,
+            config={
+                'max_retry_times': max_retry_times,
+            },
+        )
+
+        self.test_sql_execution = self.model(
+            name='测试SQL执行任务',
+            parent=self.sql_execution_parent_task,
+            category=categories.system_test_category,
+            config={
+                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table
+            },
+            user=user
+        )
+
+        self.test_sql_produce = self.model(
+            name='测试SQL生产任务',
+            parent=self.sql_produce_parent_task,
+            category=categories.system_test_category,
+            config={
+                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
+                'queue': queues.test.code
+            },
+            user=user
+        )
+        self.test_shell_execution = self.model(
+            name='测试Shell执行任务',
+            parent=self.shell_execution_parent_task,
+            category=categories.system_test_category,
+            config={
+                'shell': 'echo "hello world"'
+            },
+            user=user
+        )
+        super(BuiltinTasks, self).__init__()
+
+
+class BuiltinSchedules(BuiltinModels):
+    model_unique_kwargs = ['task', 'user']
+    model = SystemSchedule
+
+    def __init__(self, user, tasks: BuiltinTasks):
+        self.system_log_cleaning = self.model(
+            task=tasks.system_log_cleaning,
+            user=user,
+            config={
+                "T": {
+                    "DAY": {
+                        "period": 1
+                    },
+                    "time": "01:00:00",
+                    "type": "DAY"
+                },
+                "base_on_now": True,
+                "schedule_type": "T"
+            }
+        )
+
+        self.system_exception_handling = self.model(
+            task=tasks.system_exception_handling,
+            user=user,
+            config={
+                "S": {
+                    "period": 60,
+                    "schedule_start_time": "2023-04-04 15:31:00"
+                },
+                "base_on_now": True,
+                "schedule_type": "S"
+            }
+        )
+
+        self.task_log_cleaning = self.model(
+            task=tasks.task_log_cleaning,
+            user=user,
+            config={
+                "T": {
+                    "DAY": {
+                        "period": 1
+                    },
+                    "time": "01:00:00",
+                    "type": "DAY"
+                },
+                "base_on_now": True,
+                "schedule_type": "T"
+            }
+        )
+
+        self.task_exception_handling = self.model(
+            task=tasks.task_exception_handling,
+            user=user,
+            config={
+                "S": {
+                    "period": 60,
+                    "schedule_start_time": "2023-04-04 15:31:00"
+                },
+                "base_on_now": True,
+                "schedule_type": "S"
+            }
+        )
+
+        config = {
+            'config': {
+                "S": {
+                    "period": 60,
+                    "schedule_start_time": "2023-04-04 15:31:00"
+                },
+                "base_on_now": True,
+                "schedule_type": "S"
+            }
+        }
+
+        self.test_sql_execution = self.model(
+            task=tasks.test_sql_execution,
+            user=user,
+            status=TaskScheduleStatus.TEST.value,
+            config=config
+        )
+        self.test_sql_produce = self.model(
+            task=tasks.test_sql_produce,
+            user=user,
+            status=TaskScheduleStatus.TEST.value,
+            config=config
+        )
+        self.test_shell_execution = self.model(
+            task=tasks.test_shell_execution,
+            user=user,
+            status=TaskScheduleStatus.TEST.value,
+            config=config
+        )
+
+        super(BuiltinSchedules, self).__init__()
+
+
+class BuiltinConsumerPermissions(BaseConsumerPermissions):
+    model = SystemConsumerPermission
+
+    def __init__(self, producers: BuiltinProducers):
+        self.system_consumer_permission = self.model(
+            producer=producers.opening,
+            type=ConsumerPermissionType.IP_WHITE_LIST.value,
+            status=True,
+            config={
+                'ip_whitelist': ['127.0.0.1']
+            }
+        )
+        super(BuiltinConsumerPermissions, self).__init__()
+
+
+class Builtins(BaseBuiltins):
+    app = 'django_common_task_system.system_task'
+
+    def __init__(self):
+        super(Builtins, self).__init__()
+        self.queues = BuiltinQueues()
+        self.categories = BuiltinCategories(self.user)
+        self.tasks = BuiltinTasks(self.categories, self.queues)
+        self.schedules = BuiltinSchedules(self.user, self.tasks)
+        self.producers = BuiltinProducers(self.queues)
+        self.consumer_permissions = BuiltinConsumerPermissions(self.producers)
+
+
+builtins = Builtins()
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/process.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from multiprocessing import Process, set_start_method
-
-
-class _ProcessManager:
-
-    def __init__(self):
-        self._processes = {}
-
-    @property
-    def all(self):
-        return [x for x in self._processes.values() if x.is_alive()]
-
-    @property
-    def all_process_ids(self):
-        return [k for k, v in self._processes.items() if v.is_alive()]
-
-    def create(self, target, *args, **kwargs) -> Process:
-        set_start_method('spawn', True)
-        process = Process(target=target, args=args, kwargs=kwargs, daemon=True)
-        process.start()
-        self._processes[process.pid] = process
-        return process
-
-    def kill(self, pid):
-        if pid in self._processes:
-            self._processes[pid].kill()
-            self._processes.pop(pid)
-
-    def terminate(self, pid):
-        if pid in self._processes:
-            self._processes[pid].terminate()
-        else:
-            raise ValueError('pid %s not found' % pid)
-
-    def terminate_all(self):
-        for process in self._processes.values():
-            process.terminate()
-
-
-ProcessManager = _ProcessManager()
+from multiprocessing import Process, set_start_method
+
+
+class _ProcessManager:
+
+    def __init__(self):
+        self._processes = {}
+
+    @property
+    def all(self):
+        return [x for x in self._processes.values() if x.is_alive()]
+
+    @property
+    def all_process_ids(self):
+        return [k for k, v in self._processes.items() if v.is_alive()]
+
+    def create(self, target, *args, **kwargs) -> Process:
+        set_start_method('spawn', True)
+        process = Process(target=target, args=args, kwargs=kwargs, daemon=True)
+        process.start()
+        self._processes[process.pid] = process
+        return process
+
+    def kill(self, pid):
+        if pid in self._processes:
+            self._processes[pid].kill()
+            self._processes.pop(pid)
+
+    def terminate(self, pid):
+        if pid in self._processes:
+            self._processes[pid].terminate()
+        else:
+            raise ValueError('pid %s not found' % pid)
+
+    def terminate_all(self):
+        for process in self._processes.values():
+            process.terminate()
+
+
+ProcessManager = _ProcessManager()
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/urls.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.urls import path
-from . import views
-
-
-urlpatterns = [
-    path('schedule/produce/<int:pk>/', views.ScheduleProduceView.as_view(), name='system_schedule_produce'),
-    path('schedule/queue/<slug:code>/get/', views.SystemScheduleQueueAPI.get, name='system_schedule_get'),
-    path('schedule/put/', views.SystemScheduleQueueAPI.put, name='system_schedule_put'),
-    path('schedule/retry/', views.SystemScheduleQueueAPI.retry, name='system_schedule_retry'),
-    path('schedule/queue/status/', views.SystemScheduleQueueAPI.status),
-    path('process/logs/<int:process_id>/', views.SystemProcessView.show_logs, name='system_process_log'),
-    path('process/stop/<int:process_id>/', views.SystemProcessView.stop_process, name='system_process_stop'),
-    path('exception/report/', views.SystemExceptionReportView.as_view()),
-]
+from django.urls import path
+from . import views
+
+
+urlpatterns = [
+    path('schedule/produce/<int:pk>/', views.ScheduleProduceView.as_view(), name='system_schedule_produce'),
+    path('schedule/queue/<slug:code>/get/', views.SystemScheduleQueueAPI.get, name='system_schedule_get'),
+    path('schedule/put/', views.SystemScheduleQueueAPI.put, name='system_schedule_put'),
+    path('schedule/retry/', views.SystemScheduleQueueAPI.retry, name='system_schedule_retry'),
+    path('schedule/queue/status/', views.SystemScheduleQueueAPI.status),
+    path('process/logs/<int:process_id>/', views.SystemProcessView.show_logs, name='system_process_log'),
+    path('process/stop/<int:process_id>/', views.SystemProcessView.stop_process, name='system_process_stop'),
+    path('exception/report/', views.SystemExceptionReportView.as_view()),
+]
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task/views.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from django.dispatch import receiver
-from rest_framework.response import Response
-from rest_framework.views import APIView
-from rest_framework.request import Request
-from rest_framework import status
-from django.db.models.signals import post_save, post_delete
-from django.db import connection
-from django.http.response import HttpResponse
-from django_common_task_system.models import system_initialize_signal
-from .models import SystemScheduleQueue, SystemSchedule, \
-    SystemProcess, SystemScheduleProducer, SystemScheduleLog, SystemConsumerPermission, SystemExceptionReport
-from django_common_task_system.views import TaskScheduleQueueAPI, TaskScheduleThread, ExceptionReportView
-from .models import builtins
-from .serializers import QueueScheduleSerializer, ExceptionSerializer
-import os
-
-
-builtins.initialize()
-
-
-class SystemScheduleThread(TaskScheduleThread):
-    schedule_model = SystemSchedule
-    queues = builtins.queues
-    producers = builtins.producers
-    serializer = QueueScheduleSerializer
-
-
-@receiver(system_initialize_signal, sender='system_initialized')
-def on_system_initialized(sender, **kwargs):
-    thread = SystemScheduleThread()
-    thread.start()
-
-
-@receiver(post_delete, sender=SystemScheduleQueue)
-def delete_queue(sender, instance: SystemScheduleQueue, **kwargs):
-    builtins.queues.delete(instance)
-
-
-@receiver(post_save, sender=SystemScheduleQueue)
-def add_queue(sender, instance: SystemScheduleQueue, created, **kwargs):
-    builtins.queues.add(instance)
-
-
-@receiver(post_delete, sender=SystemScheduleProducer)
-def delete_producer(sender, instance: SystemScheduleProducer, **kwargs):
-    builtins.producers.delete(instance)
-
-
-@receiver(post_save, sender=SystemScheduleProducer)
-def add_producer(sender, instance: SystemScheduleProducer, created, **kwargs):
-    builtins.producers.add(instance)
-
-
-@receiver(post_save, sender=SystemConsumerPermission)
-def add_consumer_permission(sender, instance: SystemConsumerPermission, created, **kwargs):
-    builtins.consumer_permissions.add(instance)
-
-
-@receiver(post_delete, sender=SystemConsumerPermission)
-def delete_consumer_permission(sender, instance: SystemConsumerPermission, **kwargs):
-    builtins.consumer_permissions.delete(instance)
-
-
-class ScheduleProduceView(APIView):
-
-    def post(self, request: Request, pk: int):
-        try:
-            schedule = SystemSchedule.objects.get(id=pk)
-        except SystemSchedule.DoesNotExist:
-            return Response({'message': 'schedule_id(%s)不存在' % pk}, status=status.HTTP_404_NOT_FOUND)
-        sql: str = schedule.task.config.get('sql', '').strip()
-        if not sql:
-            return Response({'message': 'sql语句不能为空'}, status=status.HTTP_400_BAD_REQUEST)
-        if not sql.startswith('select'):
-            return Response({'message': 'sql语句必须以select开头'}, status=status.HTTP_400_BAD_REQUEST)
-        try:
-            queue = builtins.queues[schedule.task.config['queue']].queue
-            max_size = schedule.task.config.get('max_size', 10000)
-            if queue.qsize() > max_size:
-                return Response({'message': '队列(%s)已满(%s)' % (schedule.task.config['queue'], max_size)},
-                                status=status.HTTP_400_BAD_REQUEST)
-            with connection.cursor() as cursor:
-                cursor.execute(sql)
-                rows = cursor.fetchall()
-                col_names = [desc[0] for desc in cursor.description]
-                nums = len(rows)
-                for row in rows:
-                    obj = {}
-                    for index, value in enumerate(row):
-                        obj[col_names[index]] = value
-                    queue.put(obj)
-        except Exception as e:
-            return Response({'message': 'sql语句执行失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-        return Response({'message': '成功产生%s条数据' % nums})
-
-
-class SystemScheduleQueueAPI(TaskScheduleQueueAPI):
-
-    queues = builtins.queues
-    consumer_permissions = builtins.consumer_permissions
-    schedule_model = SystemSchedule
-    log_model = SystemScheduleLog
-    serializer = QueueScheduleSerializer
-
-
-class SystemProcessView:
-
-    @staticmethod
-    def show_logs(request: Request, process_id: int):
-        # 此处pk为进程id
-        try:
-            process = SystemProcess.objects.get(process_id=process_id)
-        except SystemProcess.DoesNotExist:
-            return HttpResponse('SystemProcess(%s)不存在' % process_id)
-        if not os.path.isfile(process.log_file):
-            return HttpResponse('log文件不存在')
-        offset = int(request.GET.get('offset', 0))
-        with open(process.log_file, 'r', encoding='utf-8') as f:
-            f.seek(offset)
-            logs = f.read(offset + 1024 * 1024 * 8)
-        return HttpResponse(logs, content_type='text/plain; charset=utf-8')
-
-    @staticmethod
-    def stop_process(request: Request, process_id: int):
-        try:
-            process = SystemProcess.objects.get(process_id=process_id)
-        except SystemProcess.DoesNotExist:
-            return HttpResponse('SystemProcess(%s)不存在' % process_id)
-        process.delete()
-        return HttpResponse('SystemProcess(%s)已停止' % process_id)
-
-
-class SystemExceptionReportView(ExceptionReportView):
-
-    queryset = SystemExceptionReport.objects.all()
-    serializer_class = ExceptionSerializer
+from django.dispatch import receiver
+from rest_framework.response import Response
+from rest_framework.views import APIView
+from rest_framework.request import Request
+from rest_framework import status
+from django.db.models.signals import post_save, post_delete
+from django.db import connection
+from django.http.response import HttpResponse
+from django_common_task_system.models import system_initialize_signal
+from .models import SystemScheduleQueue, SystemSchedule, \
+    SystemProcess, SystemScheduleProducer, SystemScheduleLog, SystemConsumerPermission, SystemExceptionReport
+from django_common_task_system.views import TaskScheduleQueueAPI, TaskScheduleThread, ExceptionReportView
+from .models import builtins
+from .serializers import QueueScheduleSerializer, ExceptionSerializer
+import os
+
+
+builtins.initialize()
+
+
+class SystemScheduleThread(TaskScheduleThread):
+    schedule_model = SystemSchedule
+    queues = builtins.queues
+    producers = builtins.producers
+    serializer = QueueScheduleSerializer
+
+
+@receiver(system_initialize_signal, sender='system_initialized')
+def on_system_initialized(sender, **kwargs):
+    thread = SystemScheduleThread()
+    thread.start()
+
+
+@receiver(post_delete, sender=SystemScheduleQueue)
+def delete_queue(sender, instance: SystemScheduleQueue, **kwargs):
+    builtins.queues.delete(instance)
+
+
+@receiver(post_save, sender=SystemScheduleQueue)
+def add_queue(sender, instance: SystemScheduleQueue, created, **kwargs):
+    builtins.queues.add(instance)
+
+
+@receiver(post_delete, sender=SystemScheduleProducer)
+def delete_producer(sender, instance: SystemScheduleProducer, **kwargs):
+    builtins.producers.delete(instance)
+
+
+@receiver(post_save, sender=SystemScheduleProducer)
+def add_producer(sender, instance: SystemScheduleProducer, created, **kwargs):
+    builtins.producers.add(instance)
+
+
+@receiver(post_save, sender=SystemConsumerPermission)
+def add_consumer_permission(sender, instance: SystemConsumerPermission, created, **kwargs):
+    builtins.consumer_permissions.add(instance)
+
+
+@receiver(post_delete, sender=SystemConsumerPermission)
+def delete_consumer_permission(sender, instance: SystemConsumerPermission, **kwargs):
+    builtins.consumer_permissions.delete(instance)
+
+
+class ScheduleProduceView(APIView):
+
+    def post(self, request: Request, pk: int):
+        try:
+            schedule = SystemSchedule.objects.get(id=pk)
+        except SystemSchedule.DoesNotExist:
+            return Response({'message': 'schedule_id(%s)不存在' % pk}, status=status.HTTP_404_NOT_FOUND)
+        sql: str = schedule.task.config.get('sql', '').strip()
+        if not sql:
+            return Response({'message': 'sql语句不能为空'}, status=status.HTTP_400_BAD_REQUEST)
+        if not sql.startswith('select'):
+            return Response({'message': 'sql语句必须以select开头'}, status=status.HTTP_400_BAD_REQUEST)
+        try:
+            queue = builtins.queues[schedule.task.config['queue']].queue
+            max_size = schedule.task.config.get('max_size', 10000)
+            if queue.qsize() > max_size:
+                return Response({'message': '队列(%s)已满(%s)' % (schedule.task.config['queue'], max_size)},
+                                status=status.HTTP_400_BAD_REQUEST)
+            with connection.cursor() as cursor:
+                cursor.execute(sql)
+                rows = cursor.fetchall()
+                col_names = [desc[0] for desc in cursor.description]
+                nums = len(rows)
+                for row in rows:
+                    obj = {}
+                    for index, value in enumerate(row):
+                        obj[col_names[index]] = value
+                    queue.put(obj)
+        except Exception as e:
+            return Response({'message': 'sql语句执行失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+        return Response({'message': '成功产生%s条数据' % nums})
+
+
+class SystemScheduleQueueAPI(TaskScheduleQueueAPI):
+
+    queues = builtins.queues
+    consumer_permissions = builtins.consumer_permissions
+    schedule_model = SystemSchedule
+    log_model = SystemScheduleLog
+    serializer = QueueScheduleSerializer
+
+
+class SystemProcessView:
+
+    @staticmethod
+    def show_logs(request: Request, process_id: int):
+        # 此处pk为进程id
+        try:
+            process = SystemProcess.objects.get(process_id=process_id)
+        except SystemProcess.DoesNotExist:
+            return HttpResponse('SystemProcess(%s)不存在' % process_id)
+        if not os.path.isfile(process.log_file):
+            return HttpResponse('log文件不存在')
+        offset = int(request.GET.get('offset', 0))
+        with open(process.log_file, 'r', encoding='utf-8') as f:
+            f.seek(offset)
+            logs = f.read(offset + 1024 * 1024 * 8)
+        return HttpResponse(logs, content_type='text/plain; charset=utf-8')
+
+    @staticmethod
+    def stop_process(request: Request, process_id: int):
+        try:
+            process = SystemProcess.objects.get(process_id=process_id)
+        except SystemProcess.DoesNotExist:
+            return HttpResponse('SystemProcess(%s)不存在' % process_id)
+        process.delete()
+        return HttpResponse('SystemProcess(%s)已停止' % process_id)
+
+
+class SystemExceptionReportView(ExceptionReportView):
+
+    queryset = SystemExceptionReport.objects.all()
+    serializer_class = ExceptionSerializer
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/main.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-import argparse
-import sys
-import logging
-from logging.handlers import RotatingFileHandler
-
-
-def start_system_client(log_file=None, **kwargs):
-    os.environ['RUN_CLIENT'] = 'true'
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--system-path', type=str, required=False)
-    parser.add_argument('--system-setting', type=str, required=False)
-    shell_args = parser.parse_known_args()[0]
-    if shell_args.system_path:
-        assert os.path.exists(shell_args.system_path), 'system path not found'
-        sys.path.append(shell_args.system_path)
-    env = shell_args.system_setting or os.environ.get('DJANGO_SETTINGS_MODULE')
-    assert env, 'django settings module not found'
-    os.environ.setdefault('DJANGO_SETTINGS_MODULE', env)
-    import django
-    django.setup()
-
-    if log_file:
-        from .system_task_execution import settings
-        logger = settings.logger
-        logger.handlers.clear()
-        if not os.path.exists(os.path.dirname(log_file)):
-            os.makedirs(os.path.dirname(log_file))
-        if os.path.isfile(log_file):
-            os.remove(log_file)
-        handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
-        formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
-        logger.setLevel(logging.INFO)
-
-    from django_common_task_system.system_task_execution.system_task_execution.executor import start_client
-    start_client(**kwargs)
-
-
-if __name__ == '__main__':
-    start_system_client()
+import os
+import argparse
+import sys
+import logging
+from logging.handlers import RotatingFileHandler
+
+
+def start_system_client(log_file=None, **kwargs):
+    os.environ['RUN_CLIENT'] = 'true'
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--system-path', type=str, required=False)
+    parser.add_argument('--system-setting', type=str, required=False)
+    shell_args = parser.parse_known_args()[0]
+    if shell_args.system_path:
+        assert os.path.exists(shell_args.system_path), 'system path not found'
+        sys.path.append(shell_args.system_path)
+    env = shell_args.system_setting or os.environ.get('DJANGO_SETTINGS_MODULE')
+    assert env, 'django settings module not found'
+    os.environ.setdefault('DJANGO_SETTINGS_MODULE', env)
+    import django
+    django.setup()
+
+    if log_file:
+        from .system_task_execution import settings
+        logger = settings.logger
+        logger.handlers.clear()
+        if not os.path.exists(os.path.dirname(log_file)):
+            os.makedirs(os.path.dirname(log_file))
+        if os.path.isfile(log_file):
+            os.remove(log_file)
+        handler = RotatingFileHandler(log_file, maxBytes=1024 * 1024 * 10, encoding='utf-8', backupCount=5)
+        formatter = logging.Formatter('[%(asctime)s][%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+        logger.setLevel(logging.INFO)
+
+    from django_common_task_system.system_task_execution.system_task_execution.executor import start_client
+    start_client(**kwargs)
+
+
+if __name__ == '__main__':
+    start_system_client()
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule
-
-
-class BaseExecutor(object):
-    name = None
-
-    def __init__(self, schedule):
-        self.schedule: SystemSchedule = schedule
-
-    def execute(self):
-        raise NotImplementedError
-
-    def start(self):
-        log = SystemScheduleLog(schedule=self.schedule, result={},
-                                status='S', queue=self.schedule.queue,
-                                schedule_time=self.schedule.next_schedule_time)
-        err = None
-        try:
-            log.result['result'] = self.execute()
-        except Exception as e:
-            log.result['error'] = str(e)
-            log.status = 'F'    # F: failed
-            err = err
-        try:
-            log.save()
-        except Exception as e:
-            err = e
-        return log, err
+from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule
+
+
+class BaseExecutor(object):
+    name = None
+
+    def __init__(self, schedule):
+        self.schedule: SystemSchedule = schedule
+
+    def execute(self):
+        raise NotImplementedError
+
+    def start(self):
+        log = SystemScheduleLog(schedule=self.schedule, result={},
+                                status='S', queue=self.schedule.queue,
+                                schedule_time=self.schedule.next_schedule_time)
+        err = None
+        try:
+            log.result['result'] = self.execute()
+        except Exception as e:
+            log.result['error'] = str(e)
+            log.status = 'F'    # F: failed
+            err = err
+        try:
+            log.save()
+        except Exception as e:
+            err = e
+        return log, err
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from django.urls import reverse
-import requests
-from .base import BaseExecutor
-from django.db import connection
-from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule, builtins
-from django_common_task_system import get_task_schedule_model, get_schedule_log_model
-from django_common_task_system.models import ScheduleConfig
-from .. import settings
-
-_columns = None
-
-TaskScheduleLog = get_schedule_log_model()
-TaskSchedule = get_task_schedule_model()
-
-
-def get_schedule_table_columns(table):
-    global _columns
-    if not _columns:
-        cmd = '''select GROUP_CONCAT(column_name SEPARATOR ',') from information_schema.`COLUMNS` 
-        where column_name <> 'next_schedule_time' 
-        and table_name = '%s' GROUP BY table_name''' % table
-        with connection.cursor() as cursor:
-            cursor.execute(cmd)
-            _columns = cursor.fetchone()[0].split(',')
-    return _columns
-
-
-class SystemExceptionExecutor(BaseExecutor):
-    name = builtins.tasks.system_exception_handling.name
-    schedule_id = builtins.schedules.system_exception_handling.id
-    schedule_model = SystemSchedule
-    schedule_log_model = SystemScheduleLog
-    handle_url = 'system_schedule_put'
-
-    def execute(self):
-        max_retry_times = self.schedule.task.config.get('max_retry_times', 5)
-        max_fetch_num = self.schedule.task.config.get('max_fetch_num', 1000)
-        # columns = get_schedule_table_columns(table=self.schedule_model._meta.db_table)
-        next_schedule_time = ScheduleConfig(config=self.schedule.config).get_next_time(
-            self.schedule.next_schedule_time)
-        last_schedule_time = self.schedule.next_schedule_time - (next_schedule_time - self.schedule.next_schedule_time)
-        command = '''
-            select * from (
-            select queue, schedule_id, schedule_time, count(*) as times, max(create_time) as lastest_time 
-            from %s where create_time > CURDATE() and status != 'S' 
-            GROUP BY queue, schedule_id, schedule_time order by queue, schedule_id, schedule_time
-            ) a where a.times < %s and a.lastest_time > '%s' limit %s
-        ''' % (self.schedule_log_model._meta.db_table, max_retry_times, last_schedule_time, max_fetch_num,)
-        with connection.cursor() as cursor:
-            cursor.execute(command)
-            rows = list(cursor.fetchall())
-        batch_num = 1000
-        i = 0
-        batch = rows[:batch_num]
-        result = {}
-        error = None
-        while batch:
-            path = reverse(self.handle_url)
-            ids, queues, times = [], [], []
-            for q, i, t, *_ in batch:
-                if i == self.schedule_id:
-                    continue
-                ids.append(str(i))
-                queues.append(q)
-                times.append(t.strftime('%Y-%m-%d %H:%M:%S'))
-            url = settings.HOST + path
-            batch_result = requests.get(url, params={
-                'i': ','.join(ids),
-                'q': ','.join(queues),
-                't': ','.join(times)
-            }).json()
-            result[i] = batch_result
-            if 'error' in batch_result:
-                error = batch_result['error']
-            i += 1
-            batch = rows[i * batch_num: (i + 1) * batch_num]
-        if error:
-            raise Exception(error)
-        return result
-
-
-class ScheduleExceptionExecutor(SystemExceptionExecutor):
-    name = builtins.tasks.task_exception_handling.name
-    schedule_model = TaskSchedule
-    schedule_id = builtins.schedules.task_exception_handling.id
-    schedule_log_model = TaskScheduleLog
-    handle_url = 'task_schedule_put'
+from django.urls import reverse
+import requests
+from .base import BaseExecutor
+from django.db import connection
+from django_common_task_system.system_task.models import SystemScheduleLog, SystemSchedule, builtins
+from django_common_task_system import get_task_schedule_model, get_schedule_log_model
+from django_common_task_system.models import ScheduleConfig
+from .. import settings
+
+_columns = None
+
+TaskScheduleLog = get_schedule_log_model()
+TaskSchedule = get_task_schedule_model()
+
+
+def get_schedule_table_columns(table):
+    global _columns
+    if not _columns:
+        cmd = '''select GROUP_CONCAT(column_name SEPARATOR ',') from information_schema.`COLUMNS` 
+        where column_name <> 'next_schedule_time' 
+        and table_name = '%s' GROUP BY table_name''' % table
+        with connection.cursor() as cursor:
+            cursor.execute(cmd)
+            _columns = cursor.fetchone()[0].split(',')
+    return _columns
+
+
+class SystemExceptionExecutor(BaseExecutor):
+    name = builtins.tasks.system_exception_handling.name
+    schedule_id = builtins.schedules.system_exception_handling.id
+    schedule_model = SystemSchedule
+    schedule_log_model = SystemScheduleLog
+    handle_url = 'system_schedule_put'
+
+    def execute(self):
+        max_retry_times = self.schedule.task.config.get('max_retry_times', 5)
+        max_fetch_num = self.schedule.task.config.get('max_fetch_num', 1000)
+        # columns = get_schedule_table_columns(table=self.schedule_model._meta.db_table)
+        next_schedule_time = ScheduleConfig(config=self.schedule.config).get_next_time(
+            self.schedule.next_schedule_time)
+        last_schedule_time = self.schedule.next_schedule_time - (next_schedule_time - self.schedule.next_schedule_time)
+        command = '''
+            select * from (
+            select queue, schedule_id, schedule_time, count(*) as times, max(create_time) as lastest_time 
+            from %s where create_time > CURDATE() and status != 'S' 
+            GROUP BY queue, schedule_id, schedule_time order by queue, schedule_id, schedule_time
+            ) a where a.times < %s and a.lastest_time > '%s' limit %s
+        ''' % (self.schedule_log_model._meta.db_table, max_retry_times, last_schedule_time, max_fetch_num,)
+        with connection.cursor() as cursor:
+            cursor.execute(command)
+            rows = list(cursor.fetchall())
+        batch_num = 1000
+        i = 0
+        batch = rows[:batch_num]
+        result = {}
+        error = None
+        while batch:
+            path = reverse(self.handle_url)
+            ids, queues, times = [], [], []
+            for q, i, t, *_ in batch:
+                if i == self.schedule_id:
+                    continue
+                ids.append(str(i))
+                queues.append(q)
+                times.append(t.strftime('%Y-%m-%d %H:%M:%S'))
+            url = settings.HOST + path
+            batch_result = requests.get(url, params={
+                'i': ','.join(ids),
+                'q': ','.join(queues),
+                't': ','.join(times)
+            }).json()
+            result[i] = batch_result
+            if 'error' in batch_result:
+                error = batch_result['error']
+            i += 1
+            batch = rows[i * batch_num: (i + 1) * batch_num]
+        if error:
+            raise Exception(error)
+        return result
+
+
+class ScheduleExceptionExecutor(SystemExceptionExecutor):
+    name = builtins.tasks.task_exception_handling.name
+    schedule_model = TaskSchedule
+    schedule_id = builtins.schedules.task_exception_handling.id
+    schedule_log_model = TaskScheduleLog
+    handle_url = 'task_schedule_put'
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .base import BaseExecutor
-from django_common_task_system.system_task.models import builtins
-import sys
-import subprocess
-
-
-class ShellExecutor(BaseExecutor):
-    name = builtins.tasks.shell_execution_parent_task.name
-
-    def execute(self):
-        if sys.platform == 'win32':
-            raise RuntimeError('Windows系统不支持shell命令执行')
-
-        commands = self.schedule.task.config.get('shell', '').split(';')
-        filename = '/tmp/shell_executor.sh'
-        with open(filename, 'w') as f:
-            f.write('#!/bin/bash -e \n')
-            f.write('; \n'.join(commands))
-        p = subprocess.Popen(f'/bin/bash {filename}', shell=True, stdout=subprocess.PIPE)
-        out, err = p.communicate()
-        if err:
-            raise RuntimeError(err)
-        return out.decode('utf-8')
+from .base import BaseExecutor
+from django_common_task_system.system_task.models import builtins
+import sys
+import subprocess
+
+
+class ShellExecutor(BaseExecutor):
+    name = builtins.tasks.shell_execution_parent_task.name
+
+    def execute(self):
+        if sys.platform == 'win32':
+            raise RuntimeError('Windows系统不支持shell命令执行')
+
+        commands = self.schedule.task.config.get('shell', '').split(';')
+        filename = '/tmp/shell_executor.sh'
+        with open(filename, 'w') as f:
+            f.write('#!/bin/bash -e \n')
+            f.write('; \n'.join(commands))
+        p = subprocess.Popen(f'/bin/bash {filename}', shell=True, stdout=subprocess.PIPE)
+        out, err = p.communicate()
+        if err:
+            raise RuntimeError(err)
+        return out.decode('utf-8')
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from .base import BaseExecutor
-from django.db import connection
-from django.shortcuts import reverse
-from .. import settings
-from urllib.parse import urljoin
-from django_common_task_system.system_task.models import builtins
-import requests
-
-
-class SqlExecutor(BaseExecutor):
-    name = builtins.tasks.sql_execution_parent_task.name
-
-    def execute(self):
-        result = []
-        commands = self.schedule.task.config.get('sql', '').split(';')
-        with connection.cursor() as cursor:
-            for sql in commands:
-                sql = sql.strip()
-                if sql:
-                    cmd_result = {
-                        'sql': sql,
-                        'result': cursor.execute(sql)
-                    }
-                    result.append(cmd_result)
-        return result
-
-
-class SqlProduceExecutor(BaseExecutor):
-    name = builtins.tasks.sql_produce_parent_task.name
-
-    def execute(self):
-        url = reverse('system_schedule_produce', args=(self.schedule.id,))
-        res = requests.post(urljoin(settings.HOST, url))
-        return res.json()
+from .base import BaseExecutor
+from django.db import connection
+from django.shortcuts import reverse
+from .. import settings
+from urllib.parse import urljoin
+from django_common_task_system.system_task.models import builtins
+import requests
+
+
+class SqlExecutor(BaseExecutor):
+    name = builtins.tasks.sql_execution_parent_task.name
+
+    def execute(self):
+        result = []
+        commands = self.schedule.task.config.get('sql', '').split(';')
+        with connection.cursor() as cursor:
+            for sql in commands:
+                sql = sql.strip()
+                if sql:
+                    cmd_result = {
+                        'sql': sql,
+                        'result': cursor.execute(sql)
+                    }
+                    result.append(cmd_result)
+        return result
+
+
+class SqlProduceExecutor(BaseExecutor):
+    name = builtins.tasks.sql_produce_parent_task.name
+
+    def execute(self):
+        url = reverse('system_schedule_produce', args=(self.schedule.id,))
+        res = requests.post(urljoin(settings.HOST, url))
+        return res.json()
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-<input type="{{ widget.type }}" name="{{ widget.name }}"{% if widget.value != None %} value="{{ widget.value|stringformat:'s' }}"{% endif %}{% include "django/forms/widgets/attrs.html" %}>
-
-<script>
-    const monthCalendar = new CustomCalendar();
-    function toString(dateArr) {
-        let arr = [];
-        let len = dateArr.length;
-        for (let i = 0; i < len; i++) {
-            let item = dateArr[i];
-            if (typeof item === "string") {
-                dateArr[i] = new Date(item);
-            };
-            for (let j = 0; j < i; j++) {
-                if (item.getTime() < dateArr[j]) {
-                    let tmp = dateArr[i];
-                    dateArr[i] = dateArr[j];
-                    dateArr[j] = tmp;
-                }
-            }
-        };
-        for (let i = 0, l = dateArr.length; i < l; i++) {
-            let d = dateArr[i];
-            let month = this._getTowNum(d.getMonth() + 1);
-            let day = this._getTowNum(d.getDate());
-            arr.push(month + this.separator + day);
-        }
-        return arr;
-    }
-    function getDefaultDate() {
-        var _this = this;
-        if (this.settings.target && $(this.settings.target).length) {
-            if ($(this.settings.target)[0].nodeType === 1) {
-                this.settings.focusDate = $(this.settings.target).val() || this.settings.focusDate || '';
-            } else {
-                this.settings.focusDate = $(this.settings.target).prev().val() || this.settings.focusDate || '';
-            }
-            if (this.settings.onlyYM && $(this.settings.target).val()) {
-                this.settings.focusDate = $(this.settings.target).val() + this.separator + "01";
-            }
-        }
-        if (this.settings.focusDate && !this.settings.multiple) {
-            var focusDateArr = this.settings.focusDate.split(' ')[0].split(this.separator);
-            var t = this.settings.focusDate.split(' ')[1] || "00:00:00";
-            this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
-        }
-        if (this.settings.focusDate && this.settings.multiple) {
-            var arr = this.settings.focusDate.split(',');
-            this.dateArr = [];
-            for (var i = arr.length - 1; i >= 0; i--) {
-                var item = arr[i];
-                var focusDateArr = item.split(this.separator);
-                let date = new Date()
-                this.dateArr.push(new Date(date.getFullYear(), Number(focusDateArr[0]) - 1, focusDateArr[1]));
-            };
-            this.defaultDate = this.dateArr[0];
-            if (!_this._dateInArr(_this.defaultDate, _this.dateArr)) {
-                _this.dateArr.push(_this.date);
-            }
-        }
-    }
-    monthCalendar._toString = toString;
-    monthCalendar.getDefaultDate = getDefaultDate
-    monthCalendar.init({
-        target: $('#id_timing_year'),
-        {#range: ['2015-3-5', '2015-3-25'],#}
-        multiple: true,
-        {#maxdays: 5,#}
-        overdays: function(a) {
-            alert('添加已达上限 ' + a + ' 天');
-        },
-        toolbar: false,
-    });
-
-</script>
+<input type="{{ widget.type }}" name="{{ widget.name }}"{% if widget.value != None %} value="{{ widget.value|stringformat:'s' }}"{% endif %}{% include "django/forms/widgets/attrs.html" %}>
+
+<script>
+    const monthCalendar = new CustomCalendar();
+    function toString(dateArr) {
+        let arr = [];
+        let len = dateArr.length;
+        for (let i = 0; i < len; i++) {
+            let item = dateArr[i];
+            if (typeof item === "string") {
+                dateArr[i] = new Date(item);
+            };
+            for (let j = 0; j < i; j++) {
+                if (item.getTime() < dateArr[j]) {
+                    let tmp = dateArr[i];
+                    dateArr[i] = dateArr[j];
+                    dateArr[j] = tmp;
+                }
+            }
+        };
+        for (let i = 0, l = dateArr.length; i < l; i++) {
+            let d = dateArr[i];
+            let month = this._getTowNum(d.getMonth() + 1);
+            let day = this._getTowNum(d.getDate());
+            arr.push(month + this.separator + day);
+        }
+        return arr;
+    }
+    function getDefaultDate() {
+        var _this = this;
+        if (this.settings.target && $(this.settings.target).length) {
+            if ($(this.settings.target)[0].nodeType === 1) {
+                this.settings.focusDate = $(this.settings.target).val() || this.settings.focusDate || '';
+            } else {
+                this.settings.focusDate = $(this.settings.target).prev().val() || this.settings.focusDate || '';
+            }
+            if (this.settings.onlyYM && $(this.settings.target).val()) {
+                this.settings.focusDate = $(this.settings.target).val() + this.separator + "01";
+            }
+        }
+        if (this.settings.focusDate && !this.settings.multiple) {
+            var focusDateArr = this.settings.focusDate.split(' ')[0].split(this.separator);
+            var t = this.settings.focusDate.split(' ')[1] || "00:00:00";
+            this.defaultDate = new Date(focusDateArr[0], Number(focusDateArr[1]) - 1, focusDateArr[2], t.split(':')[0], t.split(':')[1], t.split(':')[2]);
+        }
+        if (this.settings.focusDate && this.settings.multiple) {
+            var arr = this.settings.focusDate.split(',');
+            this.dateArr = [];
+            for (var i = arr.length - 1; i >= 0; i--) {
+                var item = arr[i];
+                var focusDateArr = item.split(this.separator);
+                let date = new Date()
+                this.dateArr.push(new Date(date.getFullYear(), Number(focusDateArr[0]) - 1, focusDateArr[1]));
+            };
+            this.defaultDate = this.dateArr[0];
+            if (!_this._dateInArr(_this.defaultDate, _this.dateArr)) {
+                _this.dateArr.push(_this.date);
+            }
+        }
+    }
+    monthCalendar._toString = toString;
+    monthCalendar.getDefaultDate = getDefaultDate
+    monthCalendar.init({
+        target: $('#id_timing_year'),
+        {#range: ['2015-3-5', '2015-3-25'],#}
+        multiple: true,
+        {#maxdays: 5,#}
+        overdays: function(a) {
+            alert('添加已达上限 ' + a + ' 天');
+        },
+        toolbar: false,
+    });
+
+</script>
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-
-<div id="period-schedule">
-    <span class="required" style="float: left">计划时间:&nbsp;&nbsp;</span>
-    <div style="display: inline-block; float: left">
-        {% with widget=widget.subwidgets.0 %}{% include widget.template_name %}{% endwith %}<br>
-    </div>
-    <span style="float: left; margin-left: 100px">计划周期:&nbsp;&nbsp;</span>
-    <div style="display: inline-block; float: left;">
-        每 {% with widget=widget.subwidgets.1 %}{% include widget.template_name %}{% endwith %} 秒
-    </div>
-
-</div>
+
+<div id="period-schedule">
+    <span class="required" style="float: left">计划时间:&nbsp;&nbsp;</span>
+    <div style="display: inline-block; float: left">
+        {% with widget=widget.subwidgets.0 %}{% include widget.template_name %}{% endwith %}<br>
+    </div>
+    <span style="float: left; margin-left: 100px">计划周期:&nbsp;&nbsp;</span>
+    <div style="display: inline-block; float: left;">
+        每 {% with widget=widget.subwidgets.1 %}{% include widget.template_name %}{% endwith %} 秒
+    </div>
+
+</div>
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/urls.py` & `django-common-task-system-1.2.6/django_common_task_system/urls.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django.urls import path
-from . import views
-from rest_framework import routers
-
-router = routers.DefaultRouter()
-router.register(r'schedule-log', views.ScheduleLogViewSet)
-
-
-urlpatterns = [
-    path('task/', views.TaskListView.as_view()),
-    path('task/<int:pk>/', views.TaskDetailView.as_view()),
-    path('schedule/list/', views.TaskScheduleListView.as_view()),
-    path('schedule/retry/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
-    path('schedule/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
-    path('schedule/detail/<int:pk>/', views.TaskScheduleDetailView.as_view()),
-    path('schedule/queue/<slug:code>/get/', views.TaskScheduleQueueAPI.get, name='task_schedule_get'),
-    path('schedule/queue/detail/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
-    path('schedule/queue/status/', views.TaskScheduleQueueAPI.status),
-    path('schedule/time-parse/', views.ScheduleTimeParseView.as_view()),
-    path('exception/report/', views.ExceptionReportView.as_view()),
-] + router.urls
+from django.urls import path
+from . import views
+from rest_framework import routers
+
+router = routers.DefaultRouter()
+router.register(r'schedule-log', views.ScheduleLogViewSet)
+
+
+urlpatterns = [
+    path('task/', views.TaskListView.as_view()),
+    path('task/<int:pk>/', views.TaskDetailView.as_view()),
+    path('schedule/list/', views.TaskScheduleListView.as_view()),
+    path('schedule/retry/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
+    path('schedule/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
+    path('schedule/detail/<int:pk>/', views.TaskScheduleDetailView.as_view()),
+    path('schedule/queue/<slug:code>/get/', views.TaskScheduleQueueAPI.get, name='task_schedule_get'),
+    path('schedule/queue/detail/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
+    path('schedule/queue/status/', views.TaskScheduleQueueAPI.status),
+    path('schedule/time-parse/', views.ScheduleTimeParseView.as_view()),
+    path('exception/report/', views.ExceptionReportView.as_view()),
+] + router.urls
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.6/django_common_task_system/utils/algorithm.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-
-
-def list_to_tree(source, parent, cache=None):
-    cache = cache or []
-    tree = []
-    for item in source:
-        if item["id"] in cache:
-            continue
-        if item["parent"] == parent:
-            cache.append(item["id"])
-            item["children"] = list_to_tree(source, item["id"], cache)
-            tree.append(item)
-    return tree
-
-
-def tree_to_list(tree, result=None):
-    result = result or []
-    for item in tree:
-        result.append(item)
-        if item.get("children", None):
-            tree_to_list(item["children"], result)
-    return result
-
-
-def get_tree_by_id(tree, target_id):
-    for item in tree:
-        if item["id"] == target_id:
-            return item
-        if item.get("children", None):
-            result = get_tree_by_id(item["children"], target_id)
-            if result:
-                return result
-    return None
+
+
+def list_to_tree(source, parent, cache=None):
+    cache = cache or []
+    tree = []
+    for item in source:
+        if item["id"] in cache:
+            continue
+        if item["parent"] == parent:
+            cache.append(item["id"])
+            item["children"] = list_to_tree(source, item["id"], cache)
+            tree.append(item)
+    return tree
+
+
+def tree_to_list(tree, result=None):
+    result = result or []
+    for item in tree:
+        result.append(item)
+        if item.get("children", None):
+            tree_to_list(item["children"], result)
+    return result
+
+
+def get_tree_by_id(tree, target_id):
+    for item in tree:
+        if item["id"] == target_id:
+            return item
+        if item.get("children", None):
+            result = get_tree_by_id(item["children"], target_id)
+            if result:
+                return result
+    return None
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.6/django_common_task_system/utils/schedule_time.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# -*- coding:utf-8 -*-
-
-# author: Cone
-# datetime: 2023/3/5 15:33
-# software: PyCharm
-from typing import Dict
-
-
-def nlp_config_to_schedule_config(nlp_syntax: Dict, sentence=None):
-    nlp_type = nlp_syntax['type']
-    definition = nlp_syntax['definition']
-    config = {
-        "nlp-sentence": sentence,
-    }
-    nlp_time = nlp_syntax['time']
-    if nlp_type == 'time_point':
-        config['schedule_type'] = "O"
-        config['O'] = {
-            "schedule_start_time": nlp_syntax['time'][0],
-        }
-    elif nlp_type == 'time_period':
-        delta = nlp_syntax['time']['delta']
-        years = delta.get('year', 0)
-        months = delta.get('month', 0)
-        days = delta.get('day', 0)
-        hours = delta.get('hour', 0)
-        minutes = delta.get('minute', 0)
-        seconds = delta.get('second', 0)
-        seconds = seconds + minutes * 60 + hours * 3600
-        if seconds:
-            config['schedule_type'] = 'S'
-            config['S'] = {
-                "period": seconds,
-                "schedule_start_time": nlp_time['point']['time'][0],
-            }
-        else:
-            config['schedule_type'] = "T"
-            date, time = nlp_time['point']['time'][0].split()
-            year, month, day = date.split('-')
-            timing_config = config['T'] = {
-                "time": time,
-            }
-            if days:
-                timing_config["DAY"] = {
-                    "period": days,
-                }
-                timing_config["type"] = "DAY"
-            elif months:
-                timing_config["MONTHDAY"] = {
-                    "period": months,
-                    "monthday": [int(day)]
-                }
-                timing_config["type"] = "MONTHDAY"
-            elif years:
-                timing_config["YEAR"] = {
-                    "period": years,
-                    "year": "%s-%s" % (month, day)
-                }
-                timing_config["type"] = "YEAR"
-    return config
+# -*- coding:utf-8 -*-
+
+# author: Cone
+# datetime: 2023/3/5 15:33
+# software: PyCharm
+from typing import Dict
+
+
+def nlp_config_to_schedule_config(nlp_syntax: Dict, sentence=None):
+    nlp_type = nlp_syntax['type']
+    definition = nlp_syntax['definition']
+    config = {
+        "nlp-sentence": sentence,
+    }
+    nlp_time = nlp_syntax['time']
+    if nlp_type == 'time_point':
+        config['schedule_type'] = "O"
+        config['O'] = {
+            "schedule_start_time": nlp_syntax['time'][0],
+        }
+    elif nlp_type == 'time_period':
+        delta = nlp_syntax['time']['delta']
+        years = delta.get('year', 0)
+        months = delta.get('month', 0)
+        days = delta.get('day', 0)
+        hours = delta.get('hour', 0)
+        minutes = delta.get('minute', 0)
+        seconds = delta.get('second', 0)
+        seconds = seconds + minutes * 60 + hours * 3600
+        if seconds:
+            config['schedule_type'] = 'S'
+            config['S'] = {
+                "period": seconds,
+                "schedule_start_time": nlp_time['point']['time'][0],
+            }
+        else:
+            config['schedule_type'] = "T"
+            date, time = nlp_time['point']['time'][0].split()
+            year, month, day = date.split('-')
+            timing_config = config['T'] = {
+                "time": time,
+            }
+            if days:
+                timing_config["DAY"] = {
+                    "period": days,
+                }
+                timing_config["type"] = "DAY"
+            elif months:
+                timing_config["MONTHDAY"] = {
+                    "period": months,
+                    "monthday": [int(day)]
+                }
+                timing_config["type"] = "MONTHDAY"
+            elif years:
+                timing_config["YEAR"] = {
+                    "period": years,
+                    "year": "%s-%s" % (month, day)
+                }
+                timing_config["type"] = "YEAR"
+    return config
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system/views.py` & `django-common-task-system-1.2.6/django_common_task_system/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,282 +1,284 @@
-from django.db.models.signals import post_delete, post_save
-from django.dispatch import receiver
-from rest_framework import status
-from rest_framework.decorators import api_view
-from rest_framework.generics import CreateAPIView
-from rest_framework.request import Request
-from rest_framework.response import Response
-from rest_framework.views import APIView
-from rest_framework.viewsets import ModelViewSet
-from django.http.response import JsonResponse
-from django.conf import settings
-from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
-from .choices import TaskScheduleStatus
-from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, \
-    ConsumerPermission, ExceptionReport, builtins, ScheduleConfig
-from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
-from queue import Empty
-from datetime import datetime
-from jionlp_time import parse_time
-from .utils.schedule_time import nlp_config_to_schedule_config
-from .models import system_initialize_signal, system_schedule_event
-from threading import Thread
-import time
-import traceback
-
-
-TaskModel = get_task_model()
-ScheduleLogModel = get_schedule_log_model()
-ScheduleModel = get_task_schedule_model()
-ScheduleSerializer = get_task_schedule_serializer()
-
-builtins.initialize()
-
-
-class TaskScheduleThread(Thread):
-    schedule_model = ScheduleModel
-    producers = builtins.producers
-    queues = builtins.queues
-    serializer = ScheduleSerializer
-
-    def __init__(self):
-        super().__init__(daemon=True)
-
-    def produce(self):
-        now = datetime.now()
-        qsize = getattr(settings, 'SCHEDULE_QUEUE_MAX_SIZE', 1000)
-        max_queue_size = qsize * 2
-        for producer in self.producers.values():
-            queue_instance = self.queues[producer.queue.code]
-            queue = queue_instance.queue
-            # 队列长度大于1000时不再生产, 防止内存溢出
-            if queue.qsize() >= qsize:
-                continue
-            queryset = self.schedule_model.objects.filter(**producer.filters)
-            if producer.lte_now:
-                queryset = queryset.filter(next_schedule_time__lte=now)
-            for schedule in queryset:
-                try:
-                    # 限制队列长度, 防止内存溢出
-                    while queue.qsize() < max_queue_size and schedule.next_schedule_time <= now:
-                        data = self.serializer(schedule).data
-                        data['queue'] = queue_instance.code
-                        queue.put(data)
-                        schedule.next_schedule_time = ScheduleConfig(config=schedule.config
-                                                                     ).get_next_time(schedule.next_schedule_time)
-                    schedule.save(update_fields=('next_schedule_time', ))
-                except Exception as e:
-                    schedule.status = TaskScheduleStatus.ERROR.value
-                    schedule.save(update_fields=('status',))
-                    traceback.print_exc()
-
-    def run(self) -> None:
-        # 等待系统初始化完成, 5秒后自动开始
-        system_schedule_event.wait(timeout=5)
-        SCHEDULE_INTERVAL = getattr(settings, 'SCHEDULE_INTERVAL', 1)
-        while True:
-            try:
-                self.produce()
-            except Exception as err:
-                traceback.print_exc()
-            time.sleep(SCHEDULE_INTERVAL)
-
-
-@receiver(system_initialize_signal, sender='system_initialized')
-def on_system_initialized(sender, **kwargs):
-    thread = TaskScheduleThread()
-    thread.start()
-
-
-@receiver(post_delete, sender=TaskScheduleQueue)
-def delete_queue(sender, instance: TaskScheduleQueue, **kwargs):
-    builtins.queues.delete(instance)
-
-
-@receiver(post_save, sender=TaskScheduleQueue)
-def add_queue(sender, instance: TaskScheduleQueue, created, **kwargs):
-    builtins.queues.add(instance)
-
-
-@receiver(post_save, sender=TaskScheduleProducer)
-def add_producer(sender, instance: TaskScheduleProducer, created, **kwargs):
-    builtins.producers.add(instance)
-
-
-@receiver(post_delete, sender=TaskScheduleProducer)
-def delete_producer(sender, instance: TaskScheduleProducer, **kwargs):
-    builtins.producers.delete(instance)
-
-
-@receiver(post_save, sender=ConsumerPermission)
-def add_consumer_permission(sender, instance: ConsumerPermission, created, **kwargs):
-    builtins.consumer_permissions.add(instance)
-
-
-@receiver(post_delete, sender=ConsumerPermission)
-def delete_consumer_permission(sender, instance: ConsumerPermission, **kwargs):
-    builtins.consumer_permissions.delete(instance)
-
-
-class TaskListView(UserListAPIView):
-    queryset = TaskModel.objects.all()
-    serializer_class = serializers.TaskSerializer
-
-
-class TaskDetailView(UserRetrieveAPIView):
-    queryset = TaskModel.objects.all()
-    serializer_class = serializers.TaskSerializer
-
-
-class TaskScheduleListView(UserListAPIView):
-    queryset = TaskSchedule.objects.all()
-    serializer_class = serializers.TaskScheduleSerializer
-
-
-class TaskScheduleDetailView(UserRetrieveAPIView):
-    queryset = TaskSchedule.objects.all()
-    serializer_class = serializers.TaskScheduleSerializer
-
-
-class ScheduleLogViewSet(ModelViewSet):
-    queryset = ScheduleLogModel.objects.all()
-    serializer_class = serializers.TaskScheduleLogSerializer
-
-
-class TaskScheduleQueueAPI(object):
-    queues = builtins.queues
-    consumer_permissions = builtins.consumer_permissions
-    schedule_model = TaskSchedule
-    log_model = ScheduleLogModel
-    serializer = ScheduleSerializer
-    permission_validator = None
-
-    @classmethod
-    def get(cls, request: Request, code: str):
-        instance = cls.queues.get(code, None)
-        if instance is None:
-            return JsonResponse({'error': '队列(%s)不存在' % code}, status=status.HTTP_404_NOT_FOUND)
-        permission_validator = cls.permission_validator or cls.consumer_permissions.get(code, None)
-        if permission_validator is not None:
-            error = permission_validator.validate(request)
-            if error:
-                return JsonResponse({'error': error}, status=status.HTTP_403_FORBIDDEN)
-        try:
-            task = instance.queue.get_nowait()
-        except Empty:
-            return JsonResponse({'message': 'no schedule for %s' % code}, status=status.HTTP_202_ACCEPTED)
-        except Exception as e:
-            return JsonResponse({'error': 'get schedule error: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-        return JsonResponse(task)
-
-    @classmethod
-    def get_by_id(cls, request, pk):
-        try:
-            schedule = cls.schedule_model.objects.get(id=pk)
-            return Response(cls.serializer(schedule).data)
-        except TaskSchedule.DoesNotExist:
-            return Response({'error': 'schedule not found'}, status=status.HTTP_404_NOT_FOUND)
-
-    @classmethod
-    def retry(cls, request):
-        log_ids = request.GET.get('log-ids', None)
-        if not log_ids:
-            return JsonResponse({'error': 'log-ids不能为空'}, status=status.HTTP_400_BAD_REQUEST)
-        try:
-            log_ids = [int(i) for i in log_ids.split(',')]
-            assert len(log_ids) < 1000, 'log-ids不能超过1000个'
-        except Exception as e:
-            return JsonResponse({'error': 'logs_ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-        try:
-            result = {x: 'no such log' for x in log_ids}
-            logs = cls.log_model.objects.filter(id__in=log_ids)
-            for log in logs:
-                queue = cls.queues[log.queue].queue
-                log.schedule.next_schedule_time = log.schedule_time
-                data = cls.serializer(log.schedule).data
-                data['queue'] = log.queue
-                queue.put(data)
-                result[log.id] = log.queue
-            return JsonResponse(result)
-        except Exception as e:
-            return JsonResponse({'error': '重试失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-
-    @classmethod
-    def put(cls, request: Request):
-        schedule_ids = request.GET.get('i', None)
-        queues = request.GET.get('q', None)
-        schedule_times = request.GET.get('t', None)
-        if not schedule_ids or not queues or not schedule_times:
-            return JsonResponse({'error': 'schedule_ids(i)、queues(q)、schedule_times(t)不能为空'},
-                                status=status.HTTP_400_BAD_REQUEST)
-        try:
-            schedule_ids = [int(i) for i in schedule_ids.split(',')]
-            queues = [i.strip() for i in queues.split(',')]
-            schedule_times = [datetime.strptime(i, '%Y-%m-%d %H:%M:%S') for i in schedule_times.split(',')]
-            assert len(schedule_ids) <= 1000, '不能超过1000个'
-            if len(queues) == 1:
-                q = queues[0]
-                queues = [q for _ in schedule_ids]
-            elif len(queues) != len(schedule_ids):
-                raise Exception('ids和queues长度不一致')
-            if len(schedule_times) == 1:
-                t = schedule_times[0]
-                schedule_times = [t for _ in schedule_ids]
-            elif len(schedule_times) != len(schedule_ids):
-                raise Exception('ids和schedule_times长度不一致')
-        except Exception as e:
-            return JsonResponse({'error': 'ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-        try:
-            schedules = cls.schedule_model.objects.filter(id__in=set(schedule_ids))
-            schedule_mapping = {x.id: x for x in schedules}
-            result = {}
-            for i, q, t in zip(schedule_ids, queues, schedule_times):
-                queue_instance = cls.queues.get(q, None)
-                if queue_instance is None:
-                    result[q] = 'no such queue: %s' % q
-                    continue
-                queue_result = result.setdefault(q, {})
-                schedule = schedule_mapping.get(i, None)
-                if schedule is None:
-                    queue_result[i] = 'no such schedule: %s' % i
-                    continue
-                schedule_result = queue_result.setdefault(i, [])
-                schedule.next_schedule_time = t
-                data = cls.serializer(schedule).data
-                data['queue'] = q
-                queue_instance.queue.put(data)
-                schedule_result.append(t.strftime('%Y-%m-%d %H:%M:%S'))
-            return JsonResponse(result)
-        except Exception as e:
-            return JsonResponse({'error': '添加到队列失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
-
-    @staticmethod
-    @api_view(['GET'])
-    def status(request):
-        return Response({x: y.queue.qsize() for x, y in builtins.queues.items()})
-
-
-class ScheduleTimeParseView(APIView):
-
-    def get(self, request, *args, **kwargs):
-        sentence = request.query_params.get('sentence')
-        if not sentence:
-            return Response({'error': 'sentence is required'}, status=status.HTTP_400_BAD_REQUEST)
-        try:
-            result = parse_time(sentence)
-            schedule = nlp_config_to_schedule_config(result, sentence=sentence)
-            return Response({
-                "jio_result": result,
-                "schedule": schedule
-            })
-        except Exception as e:
-            return Response({'error': str(e)}, status=status.HTTP_500_INTERNAL_SERVER_ERROR)
-
-
-class ExceptionReportView(CreateAPIView):
-    queryset = ExceptionReport.objects.all()
-    serializer_class = serializers.ExceptionSerializer
-
-    def perform_create(self, serializer):
-        meta = self.request.META
-        ip = meta.get('HTTP_X_FORWARDED_FOR') if meta.get('HTTP_X_FORWARDED_FOR') else meta.get('REMOTE_ADDR')
-        serializer.save(ip=ip)
+from django.db.models.signals import post_delete, post_save
+from django.dispatch import receiver
+from rest_framework import status
+from rest_framework.decorators import api_view
+from rest_framework.generics import CreateAPIView
+from rest_framework.request import Request
+from rest_framework.response import Response
+from rest_framework.views import APIView
+from rest_framework.viewsets import ModelViewSet
+from django.http.response import JsonResponse
+from django.conf import settings
+from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
+from .choices import TaskScheduleStatus
+from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, \
+    ConsumerPermission, ExceptionReport, builtins, ScheduleConfig
+from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
+from queue import Empty
+from datetime import datetime
+from jionlp_time import parse_time
+from .utils.schedule_time import nlp_config_to_schedule_config
+from .models import system_initialize_signal, system_schedule_event
+from threading import Thread
+import time
+import traceback
+
+
+TaskModel = get_task_model()
+ScheduleLogModel = get_schedule_log_model()
+ScheduleModel = get_task_schedule_model()
+ScheduleSerializer = get_task_schedule_serializer()
+
+builtins.initialize()
+
+
+class TaskScheduleThread(Thread):
+    schedule_model = ScheduleModel
+    producers = builtins.producers
+    queues = builtins.queues
+    serializer = ScheduleSerializer
+
+    def __init__(self):
+        super().__init__(daemon=True)
+
+    def produce(self):
+        now = datetime.now()
+        qsize = getattr(settings, 'SCHEDULE_QUEUE_MAX_SIZE', 1000)
+        max_queue_size = qsize * 2
+        for producer in self.producers.values():
+            queue_instance = self.queues[producer.queue.code]
+            queue = queue_instance.queue
+            # 队列长度大于1000时不再生产, 防止内存溢出
+            if queue.qsize() >= qsize:
+                continue
+            queryset = self.schedule_model.objects.filter(**producer.filters)
+            if producer.lte_now:
+                queryset = queryset.filter(next_schedule_time__lte=now)
+            for schedule in queryset:
+                try:
+                    # 限制队列长度, 防止内存溢出
+                    while queue.qsize() < max_queue_size and schedule.next_schedule_time <= now:
+                        data = self.serializer(schedule).data
+                        data['queue'] = queue_instance.code
+                        queue.put(data)
+                        schedule.next_schedule_time = ScheduleConfig(config=schedule.config
+                                                                     ).get_next_time(schedule.next_schedule_time)
+                    schedule.save(update_fields=('next_schedule_time', ))
+                except Exception as e:
+                    schedule.status = TaskScheduleStatus.ERROR.value
+                    schedule.save(update_fields=('status',))
+                    traceback.print_exc()
+
+    def run(self) -> None:
+        # 等待系统初始化完成, 5秒后自动开始
+        system_schedule_event.wait(timeout=5)
+        SCHEDULE_INTERVAL = getattr(settings, 'SCHEDULE_INTERVAL', 1)
+        while True:
+            try:
+                self.produce()
+            except Exception as err:
+                traceback.print_exc()
+            time.sleep(SCHEDULE_INTERVAL)
+
+
+@receiver(system_initialize_signal, sender='system_initialized')
+def on_system_initialized(sender, **kwargs):
+    thread = TaskScheduleThread()
+    thread.start()
+
+
+@receiver(post_delete, sender=TaskScheduleQueue)
+def delete_queue(sender, instance: TaskScheduleQueue, **kwargs):
+    builtins.queues.delete(instance)
+
+
+@receiver(post_save, sender=TaskScheduleQueue)
+def add_queue(sender, instance: TaskScheduleQueue, created, **kwargs):
+    builtins.queues.add(instance)
+
+
+@receiver(post_save, sender=TaskScheduleProducer)
+def add_producer(sender, instance: TaskScheduleProducer, created, **kwargs):
+    builtins.producers.add(instance)
+
+
+@receiver(post_delete, sender=TaskScheduleProducer)
+def delete_producer(sender, instance: TaskScheduleProducer, **kwargs):
+    builtins.producers.delete(instance)
+
+
+@receiver(post_save, sender=ConsumerPermission)
+def add_consumer_permission(sender, instance: ConsumerPermission, created, **kwargs):
+    builtins.consumer_permissions.add(instance)
+
+
+@receiver(post_delete, sender=ConsumerPermission)
+def delete_consumer_permission(sender, instance: ConsumerPermission, **kwargs):
+    builtins.consumer_permissions.delete(instance)
+
+
+class TaskListView(UserListAPIView):
+    queryset = TaskModel.objects.all()
+    serializer_class = serializers.TaskSerializer
+
+
+class TaskDetailView(UserRetrieveAPIView):
+    queryset = TaskModel.objects.all()
+    serializer_class = serializers.TaskSerializer
+
+
+class TaskScheduleListView(UserListAPIView):
+    queryset = TaskSchedule.objects.all()
+    serializer_class = serializers.TaskScheduleSerializer
+
+
+class TaskScheduleDetailView(UserRetrieveAPIView):
+    queryset = TaskSchedule.objects.all()
+    serializer_class = serializers.TaskScheduleSerializer
+
+
+class ScheduleLogViewSet(ModelViewSet):
+    queryset = ScheduleLogModel.objects.all()
+    serializer_class = serializers.TaskScheduleLogSerializer
+
+
+class TaskScheduleQueueAPI(object):
+    queues = builtins.queues
+    consumer_permissions = builtins.consumer_permissions
+    schedule_model = TaskSchedule
+    log_model = ScheduleLogModel
+    serializer = ScheduleSerializer
+    permission_validator = None
+
+    @classmethod
+    def get(cls, request: Request, code: str):
+        instance = cls.queues.get(code, None)
+        if instance is None:
+            return JsonResponse({'error': '队列(%s)不存在' % code}, status=status.HTTP_404_NOT_FOUND)
+        permission_validator = cls.permission_validator or cls.consumer_permissions.get(code, None)
+        if permission_validator is not None:
+            error = permission_validator.validate(request)
+            if error:
+                return JsonResponse({'error': error}, status=status.HTTP_403_FORBIDDEN)
+        try:
+            task = instance.queue.get_nowait()
+        except Empty:
+            return JsonResponse({'message': 'no schedule for %s' % code}, status=status.HTTP_202_ACCEPTED)
+        except Exception as e:
+            return JsonResponse({'error': 'get schedule error: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+        return JsonResponse(task)
+
+    @classmethod
+    def get_by_id(cls, request, pk):
+        try:
+            schedule = cls.schedule_model.objects.get(id=pk)
+            return Response(cls.serializer(schedule).data)
+        except TaskSchedule.DoesNotExist:
+            return Response({'error': 'schedule not found'}, status=status.HTTP_404_NOT_FOUND)
+
+    @classmethod
+    def retry(cls, request):
+        log_ids = request.GET.get('log-ids', None)
+        if not log_ids:
+            return JsonResponse({'error': 'log-ids不能为空'}, status=status.HTTP_400_BAD_REQUEST)
+        try:
+            log_ids = [int(i) for i in log_ids.split(',')]
+            assert len(log_ids) < 1000, 'log-ids不能超过1000个'
+        except Exception as e:
+            return JsonResponse({'error': 'logs_ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+        try:
+            result = {x: 'no such log' for x in log_ids}
+            logs = cls.log_model.objects.filter(id__in=log_ids)
+            for log in logs:
+                queue = cls.queues[log.queue].queue
+                log.schedule.next_schedule_time = log.schedule_time
+                log.schedule.generator = 'retry'
+                data = cls.serializer(log.schedule).data
+                data['queue'] = log.queue
+                queue.put(data)
+                result[log.id] = log.queue
+            return JsonResponse(result)
+        except Exception as e:
+            return JsonResponse({'error': '重试失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+
+    @classmethod
+    def put(cls, request: Request):
+        schedule_ids = request.GET.get('i', None)
+        queues = request.GET.get('q', None)
+        schedule_times = request.GET.get('t', None)
+        if not schedule_ids or not queues or not schedule_times:
+            return JsonResponse({'error': 'schedule_ids(i)、queues(q)、schedule_times(t)不能为空'},
+                                status=status.HTTP_400_BAD_REQUEST)
+        try:
+            schedule_ids = [int(i) for i in schedule_ids.split(',')]
+            queues = [i.strip() for i in queues.split(',')]
+            schedule_times = [datetime.strptime(i, '%Y-%m-%d %H:%M:%S') for i in schedule_times.split(',')]
+            assert len(schedule_ids) <= 1000, '不能超过1000个'
+            if len(queues) == 1:
+                q = queues[0]
+                queues = [q for _ in schedule_ids]
+            elif len(queues) != len(schedule_ids):
+                raise Exception('ids和queues长度不一致')
+            if len(schedule_times) == 1:
+                t = schedule_times[0]
+                schedule_times = [t for _ in schedule_ids]
+            elif len(schedule_times) != len(schedule_ids):
+                raise Exception('ids和schedule_times长度不一致')
+        except Exception as e:
+            return JsonResponse({'error': 'ids参数错误: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+        try:
+            schedules = cls.schedule_model.objects.filter(id__in=set(schedule_ids))
+            schedule_mapping = {x.id: x for x in schedules}
+            result = {}
+            for i, q, t in zip(schedule_ids, queues, schedule_times):
+                queue_instance = cls.queues.get(q, None)
+                if queue_instance is None:
+                    result[q] = 'no such queue: %s' % q
+                    continue
+                queue_result = result.setdefault(q, {})
+                schedule = schedule_mapping.get(i, None)
+                if schedule is None:
+                    queue_result[i] = 'no such schedule: %s' % i
+                    continue
+                schedule_result = queue_result.setdefault(i, [])
+                schedule.next_schedule_time = t
+                schedule.generator = 'put'
+                data = cls.serializer(schedule).data
+                data['queue'] = q
+                queue_instance.queue.put(data)
+                schedule_result.append(t.strftime('%Y-%m-%d %H:%M:%S'))
+            return JsonResponse(result)
+        except Exception as e:
+            return JsonResponse({'error': '添加到队列失败: %s' % e}, status=status.HTTP_400_BAD_REQUEST)
+
+    @staticmethod
+    @api_view(['GET'])
+    def status(request):
+        return Response({x: y.queue.qsize() for x, y in builtins.queues.items()})
+
+
+class ScheduleTimeParseView(APIView):
+
+    def get(self, request, *args, **kwargs):
+        sentence = request.query_params.get('sentence')
+        if not sentence:
+            return Response({'error': 'sentence is required'}, status=status.HTTP_400_BAD_REQUEST)
+        try:
+            result = parse_time(sentence)
+            schedule = nlp_config_to_schedule_config(result, sentence=sentence)
+            return Response({
+                "jio_result": result,
+                "schedule": schedule
+            })
+        except Exception as e:
+            return Response({'error': str(e)}, status=status.HTTP_500_INTERNAL_SERVER_ERROR)
+
+
+class ExceptionReportView(CreateAPIView):
+    queryset = ExceptionReport.objects.all()
+    serializer_class = serializers.ExceptionSerializer
+
+    def perform_create(self, serializer):
+        meta = self.request.META
+        ip = meta.get('HTTP_X_FORWARDED_FOR') if meta.get('HTTP_X_FORWARDED_FOR') else meta.get('REMOTE_ADDR')
+        serializer.save(ip=ip)
```

### Comparing `django-common-task-system-1.2.5/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.6/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 django_common_task_system/migrations/0006_consumerpermission.py
 django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
 django_common_task_system/migrations/__init__.py
 django_common_task_system/static/common_task_system/css/calendar.css
 django_common_task_system/static/common_task_system/css/task_schedule_admin.css
 django_common_task_system/static/common_task_system/js/calendar.js
 django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+django_common_task_system/static/common_task_system/js/task_type_admin.js
 django_common_task_system/system_task/__init__.py
 django_common_task_system/system_task/admin.py
 django_common_task_system/system_task/apps.py
 django_common_task_system/system_task/choices.py
 django_common_task_system/system_task/forms.py
 django_common_task_system/system_task/models.py
 django_common_task_system/system_task/process.py
```

### Comparing `django-common-task-system-1.2.5/setup.py` & `django-common-task-system-1.2.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='django-common-task-system',
-    packages=find_packages(exclude=['local_tests']),
-    version='1.2.5',
-    install_requires=[
-        "django-common-objects>=1.0.5",
-        "django>=3.2.18",
-        "croniter>=1.3.8",
-        "djangorestframework>=3.14.0",
-        "PyMySQL>=1.0.2",
-        "jionlp-time>=1.0.0",
-    ],
-    include_package_data=True,
-    author='cone387',
-    maintainer_email='1183008540@qq.com',
-    license='MIT',
-    url='https://github.com/cone387/CommonTaskSystemServer',
-    python_requires='>=3.7, <4',
+from setuptools import setup, find_packages
+
+setup(
+    name='django-common-task-system',
+    packages=find_packages(exclude=['local_tests']),
+    version='1.2.6',
+    install_requires=[
+        "django-common-objects>=1.0.5",
+        "django>=3.2.18",
+        "croniter>=1.3.8",
+        "djangorestframework>=3.14.0",
+        "PyMySQL>=1.0.2",
+        "jionlp-time>=1.0.0",
+    ],
+    include_package_data=True,
+    author='cone387',
+    maintainer_email='1183008540@qq.com',
+    license='MIT',
+    url='https://github.com/cone387/CommonTaskSystemServer',
+    python_requires='>=3.7, <4',
 )
```

