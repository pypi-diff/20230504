# Comparing `tmp/sqlmesh-0.6.5.dev5.tar.gz` & `tmp/sqlmesh-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.6.5.dev5.tar", last modified: Wed May  3 23:40:07 2023, max compression
+gzip compressed data, was "sqlmesh-0.7.0.tar", last modified: Tue May  2 18:24:02 2023, max compression
```

## Comparing `sqlmesh-0.6.5.dev5.tar` & `sqlmesh-0.7.0.tar`

### file list

```diff
@@ -1,751 +1,753 @@
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.934162 sqlmesh-0.6.5.dev5/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.725837 sqlmesh-0.6.5.dev5/.circleci/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/.circleci/config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4414 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/.circleci/continue_config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/.dockerignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.6.5.dev5/.pre-commit-config.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.6.5.dev5/.readthedocs.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/Dockerfile.api
--rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/Dockerfile.app
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.6.5.dev5/LICENSE
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2166 2023-05-03 23:40:07.934276 sqlmesh-0.6.5.dev5/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1192 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1008 2023-04-27 17:19:12.000000 sqlmesh-0.6.5.dev5/docker-compose.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.728283 sqlmesh-0.6.5.dev5/docs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.708433 sqlmesh-0.6.5.dev5/docs/_readthedocs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.728503 sqlmesh-0.6.5.dev5/docs/_readthedocs/html/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.6.5.dev5/docs/_readthedocs/html/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/comparisons.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.730269 sqlmesh-0.6.5.dev5/docs/concepts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.730674 sqlmesh-0.6.5.dev5/docs/concepts/architecture/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/concepts/architecture/serialization.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.6.5.dev5/docs/concepts/audits.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/concepts/environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/concepts/glossary.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/concepts/hooks.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3027 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/concepts/macros.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.731696 sqlmesh-0.6.5.dev5/docs/concepts/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/docs/concepts/models/model_kinds.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8189 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/docs/concepts/models/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.6.5.dev5/docs/concepts/models/python_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.6.5.dev5/docs/concepts/models/seed_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.6.5.dev5/docs/concepts/models/sql_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/concepts/overview.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.731832 sqlmesh-0.6.5.dev5/docs/concepts/plans/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9954 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/docs/concepts/plans.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/docs/concepts/tests.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/docs/development.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.738047 sqlmesh-0.6.5.dev5/docs/guides/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1943 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/docs/guides/connections.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/guides/migrations.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.6.5.dev5/docs/guides/models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/guides/multi_repo.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.6.5.dev5/docs/guides/projects.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.739553 sqlmesh-0.6.5.dev5/docs/guides/scheduling/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5648 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/guides/scheduling.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/docs/guides/testing.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5459 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/docs/index.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/docs/installation.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.741371 sqlmesh-0.6.5.dev5/docs/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2905 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/docs/integrations/airflow.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/docs/integrations/dbt.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24057 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/docs/integrations/engines.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7737 2023-05-03 23:16:05.000000 sqlmesh-0.6.5.dev5/docs/integrations/github.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.743791 sqlmesh-0.6.5.dev5/docs/integrations/images/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   194172 2023-05-03 20:29:23.000000 sqlmesh-0.6.5.dev5/docs/integrations/images/github_deployed_plans.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   271175 2023-05-03 16:50:08.000000 sqlmesh-0.6.5.dev5/docs/integrations/images/github_env_summary.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   451584 2023-05-03 16:50:34.000000 sqlmesh-0.6.5.dev5/docs/integrations/images/github_prod_plan_preview.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   174084 2023-05-03 20:25:42.000000 sqlmesh-0.6.5.dev5/docs/integrations/images/github_reviewers.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   634144 2023-05-03 16:52:36.000000 sqlmesh-0.6.5.dev5/docs/integrations/images/github_test_summary.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/docs/integrations/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.6.5.dev5/docs/prerequisites.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12925 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/docs/quick_start.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.745323 sqlmesh-0.6.5.dev5/docs/reference/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/docs/reference/cli.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13607 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/docs/reference/configuration.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.6.5.dev5/docs/reference/notebook.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/reference/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/reference/python.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.6.5.dev5/docs/release_notes.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.6.5.dev5/docs/requirements.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/docs/sqlmesh.png
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.745596 sqlmesh-0.6.5.dev5/examples/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.746748 sqlmesh-0.6.5.dev5/examples/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.6.5.dev5/examples/airflow/Dockerfile.template
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/examples/airflow/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/airflow/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/airflow/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.746921 sqlmesh-0.6.5.dev5/examples/airflow/dags/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.6.5.dev5/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.6.5.dev5/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/airflow/requirements.txt
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.747469 sqlmesh-0.6.5.dev5/examples/airflow/spark_conf/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.712719 sqlmesh-0.6.5.dev5/examples/multi/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.747685 sqlmesh-0.6.5.dev5/examples/multi/repo_1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.747930 sqlmesh-0.6.5.dev5/examples/multi/repo_1/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.748290 sqlmesh-0.6.5.dev5/examples/multi/repo_1/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.748749 sqlmesh-0.6.5.dev5/examples/multi/repo_1/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.748945 sqlmesh-0.6.5.dev5/examples/multi/repo_1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.749036 sqlmesh-0.6.5.dev5/examples/multi/repo_2/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.749259 sqlmesh-0.6.5.dev5/examples/multi/repo_2/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.749465 sqlmesh-0.6.5.dev5/examples/multi/repo_2/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.749804 sqlmesh-0.6.5.dev5/examples/multi/repo_2/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.749954 sqlmesh-0.6.5.dev5/examples/multi/repo_2/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.750543 sqlmesh-0.6.5.dev5/examples/sushi/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.751155 sqlmesh-0.6.5.dev5/examples/sushi/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/audits/items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/audits/order_items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      829 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.751370 sqlmesh-0.6.5.dev5/examples/sushi/data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.6.5.dev5/examples/sushi/data/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/helper.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.751549 sqlmesh-0.6.5.dev5/examples/sushi/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.751840 sqlmesh-0.6.5.dev5/examples/sushi/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      702 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.761746 sqlmesh-0.6.5.dev5/examples/sushi/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      934 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      223 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1912 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/order_items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1643 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/orders.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.761983 sqlmesh-0.6.5.dev5/examples/sushi/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.762157 sqlmesh-0.6.5.dev5/examples/sushi/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.763020 sqlmesh-0.6.5.dev5/examples/sushi_dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/.user.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.763169 sqlmesh-0.6.5.dev5/examples/sushi_dbt/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.763386 sqlmesh-0.6.5.dev5/examples/sushi_dbt/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.764420 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.713747 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.764556 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.764681 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.764893 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765020 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765111 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765198 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765285 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1092 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765874 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.765992 sqlmesh-0.6.5.dev5/examples/sushi_dbt/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.766075 sqlmesh-0.6.5.dev5/examples/sushi_dbt/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.766250 sqlmesh-0.6.5.dev5/examples/wursthall/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.714462 sqlmesh-0.6.5.dev5/examples/wursthall/audits/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.766377 sqlmesh-0.6.5.dev5/examples/wursthall/audits/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.766584 sqlmesh-0.6.5.dev5/examples/wursthall/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      618 2023-04-06 22:49:28.000000 sqlmesh-0.6.5.dev5/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.766803 sqlmesh-0.6.5.dev5/examples/wursthall/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.767565 sqlmesh-0.6.5.dev5/examples/wursthall/models/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-27 17:28:43.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3158 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.768228 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1652 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.714779 sqlmesh-0.6.5.dev5/examples/wursthall/seeds/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.768377 sqlmesh-0.6.5.dev5/examples/wursthall/seeds/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.768630 sqlmesh-0.6.5.dev5/examples/wursthall/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-05-03 20:33:57.000000 sqlmesh-0.6.5.dev5/mkdocs.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.768750 sqlmesh-0.6.5.dev5/pdoc/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.6.5.dev5/pdoc/cli.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.768983 sqlmesh-0.6.5.dev5/pdoc/templates/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.769210 sqlmesh-0.6.5.dev5/posts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.775442 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18638 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/posts/virtual_data_environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/pytest.ini
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1393 2023-05-03 23:40:07.934766 sqlmesh-0.6.5.dev5/setup.cfg
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3270 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/setup.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.778118 sqlmesh-0.6.5.dev5/sqlmesh/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/.airflowignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh/_version.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.778920 sqlmesh-0.6.5.dev5/sqlmesh/cicd/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/cicd/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      572 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/cicd/bot.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.787536 sqlmesh-0.6.5.dev5/sqlmesh/cli/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/cli/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4742 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/cli/example_project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9930 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/cli/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/cli/options.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.791616 sqlmesh-0.6.5.dev5/sqlmesh/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      586 2023-03-15 16:48:19.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/_typing.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.792348 sqlmesh-0.6.5.dev5/sqlmesh/core/audit/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8136 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.794258 sqlmesh-0.6.5.dev5/sqlmesh/core/config/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      668 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/connection.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5611 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/root.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8407 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    38034 2023-05-03 23:18:58.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      826 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/constants.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    36734 2023-05-03 23:01:12.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8904 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/context_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17484 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/dialect.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.797044 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29549 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4191 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15681 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1971 2023-04-14 18:08:36.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2149 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6673 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4879 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1849 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/hooks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12673 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19726 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.798292 sqlmesh-0.6.5.dev5/sqlmesh/core/model/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    47510 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8168 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/kind.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13069 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/meta.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/model/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.799101 sqlmesh-0.6.5.dev5/sqlmesh/core/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      191 2022-12-27 18:08:03.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    23861 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/plan/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8565 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12623 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/renderer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.809445 sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-05-02 20:52:55.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    35436 2023-05-03 21:58:44.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19245 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.810332 sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13382 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14349 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20765 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10834 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/test.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      982 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/core/user.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.813401 sqlmesh-0.6.5.dev5/sqlmesh/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17485 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1762 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/column.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4978 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5087 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8044 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9851 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13257 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/package.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3701 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/profile.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4772 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      927 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/source.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13618 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/dbt/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.813688 sqlmesh-0.6.5.dev5/sqlmesh/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/commands.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.813995 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.814541 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.814703 sqlmesh-0.6.5.dev5/sqlmesh/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.815309 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.816248 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/cicd/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/cicd/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5128 2023-05-03 23:23:50.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/cicd/command.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24395 2023-05-03 23:23:50.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/cicd/controller.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      466 2023-05-03 23:16:05.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/cicd/options.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2210 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1726 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1829 2023-01-18 17:26:59.000000 sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13960 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/magics.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.817438 sqlmesh-0.6.5.dev5/sqlmesh/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/migrations/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      534 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/py.typed
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.817605 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.819516 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8128 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3888 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19132 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.820277 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.830352 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11104 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4660 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5213 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.836572 sqlmesh-0.6.5.dev5/sqlmesh/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4386 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/conversions.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7549 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1289 2023-05-02 02:48:02.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16133 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/rich.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1419 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.778737 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2166 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21918 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      178 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-05-03 23:40:07.000000 sqlmesh-0.6.5.dev5/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.6.5.dev5/sqlmesh.svg
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.837035 sqlmesh-0.6.5.dev5/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/common_fixtures.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4037 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.841699 sqlmesh-0.6.5.dev5/tests/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/core/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.848235 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    28133 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1270 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1253 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2613 2023-01-17 20:15:22.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8036 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7073 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/tests/core/test_audit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6611 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/core/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/core/test_connection_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10197 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/test_context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/core/test_dialect.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.6.5.dev5/tests/core/test_environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26773 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/tests/core/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6500 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_macros.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25378 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17081 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3890 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_plan_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4647 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/core/test_schema_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.6.5.dev5/tests/core/test_seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29629 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/tests/core/test_snapshot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10299 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24610 2023-05-03 21:54:44.000000 sqlmesh-0.6.5.dev5/tests/core/test_state_sync.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.849205 sqlmesh-0.6.5.dev5/tests/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.6.5.dev5/tests/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      739 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/dbt/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/dbt/test_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13195 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/dbt/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17095 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/dbt/test_transformation.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.849430 sqlmesh-0.6.5.dev5/tests/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/engines/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.849917 sqlmesh-0.6.5.dev5/tests/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/engines/spark/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.718521 sqlmesh-0.6.5.dev5/tests/fixtures/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.717385 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.851051 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.851269 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.717509 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.851377 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.851656 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.852318 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.717838 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.852458 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.852586 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.852829 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853249 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853407 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853511 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853606 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853843 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.853979 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.854341 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.854473 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.854779 sqlmesh-0.6.5.dev5/tests/fixtures/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/tests/fixtures/migrations/environments.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.855109 sqlmesh-0.6.5.dev5/tests/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.855274 sqlmesh-0.6.5.dev5/tests/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.855464 sqlmesh-0.6.5.dev5/tests/integrations/github/fixtures/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      816 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      477 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.855623 sqlmesh-0.6.5.dev5/tests/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.856659 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.857055 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4442 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4392 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9920 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6222 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6054 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.859276 sqlmesh-0.6.5.dev5/tests/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/tests/utils/test_cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/utils/test_date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/utils/test_filesystem.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.6.5.dev5/tests/utils/test_pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/tests/utils/test_transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/tests/utils/test_yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.859521 sqlmesh-0.6.5.dev5/tests/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/tests/web/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16232 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/tests/web/test_main.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.859657 sqlmesh-0.6.5.dev5/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/web/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.863371 sqlmesh-0.6.5.dev5/web/client/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/.eslintrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/.prettierignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/.prettierrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.6.5.dev5/web/client/index.html
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-27 17:30:24.000000 sqlmesh-0.6.5.dev5/web/client/openapi.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/orval.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/package-lock.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/package.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/web/client/playwright.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/postcss.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.719354 sqlmesh-0.6.5.dev5/web/client/public/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.863620 sqlmesh-0.6.5.dev5/web/client/public/favicons/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.864260 sqlmesh-0.6.5.dev5/web/client/src/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.864951 sqlmesh-0.6.5.dev5/web/client/src/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/api/channels.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/api/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.6.5.dev5/web/client/src/api/instance.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.719618 sqlmesh-0.6.5.dev5/web/client/src/assets/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.719737 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.867427 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.873182 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.886994 sqlmesh-0.6.5.dev5/web/client/src/context/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/context/context.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6470 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/context/editor.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/context/fileTree.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2187 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/context/lineage.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.6.5.dev5/web/client/src/context/plan.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/context/theme.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.887785 sqlmesh-0.6.5.dev5/web/client/src/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9555 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/index.css
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.719989 sqlmesh-0.6.5.dev5/web/client/src/library/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.721289 sqlmesh-0.6.5.dev5/web/client/src/library/components/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.888014 sqlmesh-0.6.5.dev5/web/client/src/library/components/banner/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.888255 sqlmesh-0.6.5.dev5/web/client/src/library/components/button/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.888513 sqlmesh-0.6.5.dev5/web/client/src/library/components/button/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.888702 sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.888933 sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.890719 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5764 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8518 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11905 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3527 2023-04-27 18:23:33.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.891129 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5820 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5744 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.893518 sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.894126 sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      159 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/Graph.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14454 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7679 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.894635 sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4933 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.895435 sqlmesh-0.6.5.dev5/web/client/src/library/components/input/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.895709 sqlmesh-0.6.5.dev5/web/client/src/library/components/loading/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.896385 sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.897041 sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.899421 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.899596 sqlmesh-0.6.5.dev5/web/client/src/library/components/progress/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.899797 sqlmesh-0.6.5.dev5/web/client/src/library/components/report/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.909193 sqlmesh-0.6.5.dev5/web/client/src/library/components/root/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.909570 sqlmesh-0.6.5.dev5/web/client/src/library/components/splitPane/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.909787 sqlmesh-0.6.5.dev5/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.910007 sqlmesh-0.6.5.dev5/web/client/src/library/components/toggle/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/main.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.928391 sqlmesh-0.6.5.dev5/web/client/src/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/models/artifact.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.6.5.dev5/web/client/src/models/directory.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/models/environment.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2190 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/models/file.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/models/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/models/initial.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/routes.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.928872 sqlmesh-0.6.5.dev5/web/client/src/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/web/client/src/tests/setup.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.929242 sqlmesh-0.6.5.dev5/web/client/src/types/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/types/enum.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.6.5.dev5/web/client/src/types/index.d.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.929701 sqlmesh-0.6.5.dev5/web/client/src/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.6.5.dev5/web/client/src/utils/index.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5413 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/client/src/utils/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.929944 sqlmesh-0.6.5.dev5/web/client/src/workers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/workers/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.930343 sqlmesh-0.6.5.dev5/web/client/src/workers/sqlglot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5879 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/client/tailwind.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.930520 sqlmesh-0.6.5.dev5/web/client/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/tests/initial.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/client/tsconfig.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.6.5.dev5/web/client/vite.config.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.932192 sqlmesh-0.6.5.dev5/web/server/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.5.dev5/web/server/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.932362 sqlmesh-0.6.5.dev5/web/server/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.5.dev5/web/server/api/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:40:07.933986 sqlmesh-0.6.5.dev5/web/server/api/endpoints/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/commands.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      819 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/directories.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/environments.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/events.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5383 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/files.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/lineage.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3635 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/server/api/endpoints/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.6.5.dev5/web/server/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/server/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-25 19:48:01.000000 sqlmesh-0.6.5.dev5/web/server/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.6.5.dev5/web/server/openapi.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-27 17:30:24.000000 sqlmesh-0.6.5.dev5/web/server/settings.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.6.5.dev5/web/server/sse.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.6.5.dev5/web/server/utils.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      790 2023-05-02 01:23:18.000000 sqlmesh-0.6.5.dev5/web/server/watcher.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.049085 sqlmesh-0.7.0/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.073086 sqlmesh-0.7.0/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3086 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8189 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9954 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.077086 sqlmesh-0.7.0/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1943 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24057 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/engines.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      867 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12925 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13607 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.081086 sqlmesh-0.7.0/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.049085 sqlmesh-0.7.0/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.085086 sqlmesh-0.7.0/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.089086 sqlmesh-0.7.0/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.093086 sqlmesh-0.7.0/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.053085 sqlmesh-0.7.0/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1092 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.097086 sqlmesh-0.7.0/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.053085 sqlmesh-0.7.0/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.057085 sqlmesh-0.7.0/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.101086 sqlmesh-0.7.0/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.105086 sqlmesh-0.7.0/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-05-02 18:24:02.217090 sqlmesh-0.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4742 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8136 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.117087 sqlmesh-0.7.0/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31743 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36329 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17484 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.121087 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29549 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15681 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1971 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2149 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6673 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4879 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19726 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47510 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8168 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13069 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23956 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8565 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12623 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34694 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19245 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.125087 sqlmesh-0.7.0/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14349 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20765 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10834 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.129087 sqlmesh-0.7.0/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9390 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17485 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11231 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4978 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5087 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8044 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9851 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13257 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3701 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4772 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13618 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.129087 sqlmesh-0.7.0/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2210 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/integrations/llm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.133087 sqlmesh-0.7.0/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.137087 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8128 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19132 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.137087 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.141088 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4660 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5213 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.145088 sqlmesh-0.7.0/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4386 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7606 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.109087 sqlmesh-0.7.0/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22014 2023-05-02 18:24:02.000000 sqlmesh-0.7.0/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-02 18:24:01.000000 sqlmesh-0.7.0/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.145088 sqlmesh-0.7.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.149088 sqlmesh-0.7.0/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.149088 sqlmesh-0.7.0/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28133 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1270 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8036 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7073 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6611 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26773 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6500 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25586 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17081 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3890 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29629 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24610 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13195 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17095 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.153088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.061085 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.157088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/integrations/github/fixtures/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      477 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.161088 sqlmesh-0.7.0/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.165088 sqlmesh-0.7.0/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.165088 sqlmesh-0.7.0/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9920 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5516 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16232 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.169088 sqlmesh-0.7.0/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.173088 sqlmesh-0.7.0/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.173088 sqlmesh-0.7.0/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24788 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Plan-683a0552.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43132 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/index-b61dbb6f.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2636063 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/index-f2c4b7c5.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-02 18:23:46.000000 sqlmesh-0.7.0/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-02 18:23:49.000000 sqlmesh-0.7.0/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37689 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.177089 sqlmesh-0.7.0/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.181089 sqlmesh-0.7.0/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.181089 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6470 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/lineage.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.065086 sqlmesh-0.7.0/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.189089 sqlmesh-0.7.0/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4517 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5764 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8518 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9819 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11905 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5820 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5744 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.193089 sqlmesh-0.7.0/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14454 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4933 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22356 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2087 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/loading/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.197089 sqlmesh-0.7.0/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10448 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15855 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/report/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11713 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.201089 sqlmesh-0.7.0/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1197 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5413 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.205089 sqlmesh-0.7.0/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 18:24:02.209089 sqlmesh-0.7.0/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      819 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2461 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      790 2023-05-02 18:23:56.000000 sqlmesh-0.7.0/web/server/watcher.py
```

### Comparing `sqlmesh-0.6.5.dev5/.circleci/config.yml` & `sqlmesh-0.7.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/.circleci/continue_config.yml` & `sqlmesh-0.7.0/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/.gitignore` & `sqlmesh-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/.pre-commit-config.yaml` & `sqlmesh-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/LICENSE` & `sqlmesh-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/Makefile` & `sqlmesh-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/PKG-INFO` & `sqlmesh-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.5.dev5
-Summary: UNKNOWN
+Version: 0.7.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: bigquery
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
-Provides-Extra: github
+Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.6.5.dev5/README.md` & `sqlmesh-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docker-compose.yml` & `sqlmesh-0.7.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/comparisons.md` & `sqlmesh-0.7.0/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/architecture/serialization.md` & `sqlmesh-0.7.0/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.7.0/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/audits.md` & `sqlmesh-0.7.0/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/environments.md` & `sqlmesh-0.7.0/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/glossary.md` & `sqlmesh-0.7.0/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/macros.md` & `sqlmesh-0.7.0/docs/concepts/macros.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 Variables:
 
 * date
     * @start_date
     * @end_date
     * @latest_date
 
+* datetime
+    * @start_dt
+    * @end_dt
+    * @latest_dt
+
 * ds
     * @start_ds
     * @end_ds
     * @latest_ds
 
 * ts
     * @start_ts
```

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/models/model_kinds.md` & `sqlmesh-0.7.0/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/models/overview.md` & `sqlmesh-0.7.0/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/models/python_models.md` & `sqlmesh-0.7.0/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/models/seed_models.md` & `sqlmesh-0.7.0/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/models/sql_models.md` & `sqlmesh-0.7.0/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/overview.md` & `sqlmesh-0.7.0/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.7.0/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/plans.md` & `sqlmesh-0.7.0/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/concepts/tests.md` & `sqlmesh-0.7.0/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/development.md` & `sqlmesh-0.7.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/connections.md` & `sqlmesh-0.7.0/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/migrations.md` & `sqlmesh-0.7.0/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/models.md` & `sqlmesh-0.7.0/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/multi_repo.md` & `sqlmesh-0.7.0/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/projects.md` & `sqlmesh-0.7.0/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.7.0/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/scheduling.md` & `sqlmesh-0.7.0/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/guides/testing.md` & `sqlmesh-0.7.0/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/index.md` & `sqlmesh-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/integrations/airflow.md` & `sqlmesh-0.7.0/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/integrations/dbt.md` & `sqlmesh-0.7.0/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/integrations/engines.md` & `sqlmesh-0.7.0/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/prerequisites.md` & `sqlmesh-0.7.0/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/quick_start.md` & `sqlmesh-0.7.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/reference/cli.md` & `sqlmesh-0.7.0/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/reference/configuration.md` & `sqlmesh-0.7.0/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/reference/notebook.md` & `sqlmesh-0.7.0/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/reference/overview.md` & `sqlmesh-0.7.0/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/docs/sqlmesh.png` & `sqlmesh-0.7.0/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/airflow/Dockerfile.template` & `sqlmesh-0.7.0/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/airflow/Makefile` & `sqlmesh-0.7.0/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/airflow/README.md` & `sqlmesh-0.7.0/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.7.0/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.7.0/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/config.py` & `sqlmesh-0.7.0/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/helper.py` & `sqlmesh-0.7.0/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/macros/macros.py` & `sqlmesh-0.7.0/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/models/items.py` & `sqlmesh-0.7.0/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/models/order_items.py` & `sqlmesh-0.7.0/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/models/orders.py` & `sqlmesh-0.7.0/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.7.0/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.7.0/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.7.0/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.7.0/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/macros/macros.py` & `sqlmesh-0.7.0/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.7.0/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.7.0/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/models/src/shared.py` & `sqlmesh-0.7.0/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.7.0/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.7.0/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.7.0/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/mkdocs.yml` & `sqlmesh-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/pdoc/cli.py` & `sqlmesh-0.7.0/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.7.0/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/posts/virtual_data_environments.md` & `sqlmesh-0.7.0/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/pytest.ini` & `sqlmesh-0.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/setup.cfg` & `sqlmesh-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 [mypy-fsspec]
 ignore_missing_imports = True
 
 [mypy-psycopg2.*]
 ignore_missing_imports = True
 
+[mypy-langchain.*]
+ignore_missing_imports = True
+
 [autoflake]
 in-place = True
 expand-star-imports = True
 remove-all-unused-imports = True
 ignore-init-module-imports = True
 remove-duplicate-keys = True
 remove-unused-variables = True
```

### Comparing `sqlmesh-0.6.5.dev5/setup.py` & `sqlmesh-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     author_email="engineering@tobikodata.com",
     license="Apache License 2.0",
     packages=find_packages(include=["sqlmesh", "sqlmesh.*", "web*"]),
     package_data={"web": ["client/dist/**"]},
     entry_points={
         "console_scripts": [
             "sqlmesh = sqlmesh.cli.main:cli",
-            "sqlmesh_cicd = sqlmesh.cicd.bot:bot",
         ],
         "airflow.plugins": [
             "sqlmesh_airflow = sqlmesh.schedulers.airflow.plugin:SqlmeshAirflowPlugin",
         ],
     },
     use_scm_version={
         "write_to": "sqlmesh/_version.py",
@@ -84,16 +83,17 @@
             "types-dateparser",
             "types-pytz",
             "types-requests==2.28.8",
         ],
         "dbt": [
             "dbt-core<1.5.0",
         ],
-        "github": [
-            "PyGithub",
+        "llm": [
+            "langchain",
+            "openai",
         ],
         "postgres": [
             "psycopg2",
         ],
         "redshift": [
             "redshift_connector",
         ],
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/__init__.py` & `sqlmesh-0.7.0/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/cli/__init__.py` & `sqlmesh-0.7.0/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/cli/example_project.py` & `sqlmesh-0.7.0/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/cli/main.py` & `sqlmesh-0.7.0/sqlmesh/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,9 +374,48 @@
 @click.pass_context
 @error_handler
 def migrate(ctx: click.Context) -> None:
     """Migrate SQLMesh to the current running version."""
     ctx.obj.migrate()
 
 
+@cli.command("prompt")
+@click.argument("prompt")
+@click.option(
+    "-e",
+    "--evaluate",
+    is_flag=True,
+    help="Evaluate the generated SQL query and display the results.",
+)
+@click.option(
+    "-t",
+    "--temperature",
+    type=float,
+    help="Sampling temperature. 0.0 - precise and predictable, 0.5 - balanced, 1.0 - creative. Default: 0.7",
+    default=0.7,
+)
+@opt.verbose
+@click.pass_context
+@error_handler
+def prompt(
+    ctx: click.Context, prompt: str, evaluate: bool, temperature: float, verbose: bool
+) -> None:
+    """Uses LLM to generate a SQL query from a prompt."""
+    from sqlmesh.integrations.llm import LLMIntegration
+
+    context = ctx.obj
+
+    llm_integration = LLMIntegration(
+        context.models.values(),
+        context.engine_adapter.dialect,
+        temperature=temperature,
+        verbose=verbose,
+    )
+    query = llm_integration.query(prompt)
+
+    context.console.log_status_update(query)
+    if evaluate:
+        context.console.log_success(context.fetchdf(query))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/cli/options.py` & `sqlmesh-0.7.0/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/_typing.py` & `sqlmesh-0.7.0/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.7.0/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/audit/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/base.py` & `sqlmesh-0.7.0/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.7.0/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/common.py` & `sqlmesh-0.7.0/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/connection.py` & `sqlmesh-0.7.0/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/loader.py` & `sqlmesh-0.7.0/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/model.py` & `sqlmesh-0.7.0/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/root.py` & `sqlmesh-0.7.0/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.7.0/sqlmesh/core/config/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,18 @@
     def create_plan_evaluator(self, context: Context) -> PlanEvaluator:
         return AirflowPlanEvaluator(
             airflow_client=self.get_client(context.console),
             dag_run_poll_interval_secs=self.dag_run_poll_interval_secs,
             dag_creation_poll_interval_secs=self.dag_creation_poll_interval_secs,
             dag_creation_max_retry_attempts=self.dag_creation_max_retry_attempts,
             console=context.console,
-            notification_targets=context.notification_targets,
+            notification_targets=context.config.notification_targets,
             backfill_concurrent_tasks=self.backfill_concurrent_tasks,
             ddl_concurrent_tasks=self.ddl_concurrent_tasks,
-            users=context.users,
+            users=context.config.users,
         )
 
 
 class AirflowSchedulerConfig(_BaseAirflowSchedulerConfig, BaseConfig):
     """The Airflow Scheduler configuration.
 
     Args:
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/console.py` & `sqlmesh-0.7.0/sqlmesh/core/console.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 
 SNAPSHOT_CHANGE_CATEGORY_STR = {
     None: "Unknown",
     SnapshotChangeCategory.BREAKING: "Breaking",
     SnapshotChangeCategory.NON_BREAKING: "Non-breaking",
     SnapshotChangeCategory.FORWARD_ONLY: "Forward-only",
-    SnapshotChangeCategory.INDIRECT_BREAKING: "Indirect Breaking",
-    SnapshotChangeCategory.INDIRECT_NON_BREAKING: "Indirect Non-breaking",
+    SnapshotChangeCategory.INDIRECT_BREAKING: "Indirect breaking",
+    SnapshotChangeCategory.INDIRECT_FORWARD_ONLY: "Indirect forward-only",
 }
 
 
 class Console(abc.ABC):
     """Abstract base class for defining classes used for displaying information to the user and also interact
     with them when their input is needed"""
 
@@ -753,176 +753,26 @@
             error_output = widgets.Textarea(output, layout={"height": "300px", "width": "100%"})
             test_info = widgets.HTML(
                 "<br>".join([header, message, footer, num_success, failures, footer])
             )
             self.display(widgets.VBox(children=[test_info, error_output], layout={"width": "100%"}))
 
 
-class CaptureTerminalConsole(TerminalConsole):
-    """
-    Captures the output of the terminal console so that it can be extracted out and displayed within other interfaces.
-    The captured output is cleared out after it is retrieved.
-
-    Note: `_prompt` and `_confirm` need to also be overriden to work with the custom interface if you want to use
-    this console interactively.
-    """
-
-    def __init__(self, console: t.Optional[RichConsole] = None, **kwargs: t.Any) -> None:
-        super().__init__(console=console, **kwargs)
-        self._captured_outputs: t.List[str] = []
-
-    @property
-    def captured_output(self) -> str:
-        return "".join(self._captured_outputs)
-
-    def consume_captured_output(self) -> str:
-        output = self.captured_output
-        self.clear_captured_outputs()
-        return output
-
-    def clear_captured_outputs(self) -> None:
-        self._captured_outputs = []
-
-    def _print(self, value: t.Any, **kwargs: t.Any) -> None:
-        with self.console.capture() as capture:
-            self.console.print(value, **kwargs)
-        self._captured_outputs.append(capture.get())
-
-
-class MarkdownConsole(CaptureTerminalConsole):
-    """
-    A console that outputs markdown. Currently this is only configured for non-interactive use so for use cases
-    where you want to display a plan or test results in markdown.
-    """
-
-    def show_model_difference_summary(
-        self, context_diff: ContextDiff, detailed: bool = False
-    ) -> None:
-        """Shows a summary of the differences.
-
-        Args:
-            context_diff: The context diff to use to print the summary
-            detailed: Show the actual SQL differences if True.
-        """
-        if context_diff.is_new_environment:
-            self._print(
-                f"**New environment `{context_diff.environment}` will be created from `{context_diff.create_from}`**\n\n"
-            )
-            if not context_diff.has_snapshot_changes:
-                return
-
-        if not context_diff.has_changes:
-            self._print(f"**No differences when compared to `{context_diff.environment}`**\n\n")
-            return
-
-        self._print(f"**Summary of differences against `{context_diff.environment}`:**\n\n")
-
-        if context_diff.added:
-            self._print(f"**Added Models:**\n")
-            for model in context_diff.added:
-                self._print(f"- {model}\n")
-            self._print("\n")
-
-        if context_diff.removed:
-            self._print(f"**Removed Models:**\n")
-            for model in context_diff.removed:
-                self._print(f"- {model}\n")
-            self._print("\n")
-
-        if context_diff.modified_snapshots:
-            directly_modified = []
-            indirectly_modified = []
-            metadata_modified = []
-            for model in context_diff.modified_snapshots:
-                if context_diff.directly_modified(model):
-                    directly_modified.append(model)
-                elif context_diff.indirectly_modified(model):
-                    indirectly_modified.append(model)
-                elif context_diff.metadata_updated(model):
-                    metadata_modified.append(model)
-            if directly_modified:
-                self._print(f"**Directly Modified:**\n")
-                for model in directly_modified:
-                    self._print(f"- `{model}`\n")
-                    if detailed:
-                        self._print(f"```diff\n{context_diff.text_diff(model)}\n```\n")
-                self._print("\n")
-            if indirectly_modified:
-                self._print(f"**Indirectly Modified:**\n")
-                for model in indirectly_modified:
-                    self._print(f"- `{model}`\n")
-                self._print("\n")
-            if metadata_modified:
-                self._print(f"**Metadata Updated:**\n")
-                for model in metadata_modified:
-                    self._print(f"- `{model}`\n")
-                self._print("\n")
-
-    def _show_missing_dates(self, plan: Plan) -> None:
-        """Displays the models with missing dates"""
-        if not plan.missing_intervals:
-            return
-        self._print("**Models needing backfill (missing dates):**\n\n")
-        for missing in plan.missing_intervals:
-            snapshot = plan.context_diff.snapshots[missing.snapshot_name]
-            view_name = snapshot.qualified_view_name.for_environment(plan.environment_name)
-            self._print(
-                f"* `{view_name}`: {missing.format_missing_range(snapshot.model.interval_unit())}\n"
-            )
-        self._print("\n")
-
-    def _show_categorized_snapshots(self, plan: Plan) -> None:
-        context_diff = plan.context_diff
-        for snapshot in plan.categorized:
-            if not context_diff.directly_modified(snapshot.name):
-                continue
-
-            category_str = SNAPSHOT_CHANGE_CATEGORY_STR[snapshot.change_category]
-            tree = Tree(f"[bold][direct]Directly Modified: {snapshot.name} ({category_str})")
-            indirect_tree = None
-            for child in plan.indirectly_modified[snapshot.name]:
-                if not indirect_tree:
-                    indirect_tree = Tree(f"[indirect]Indirectly Modified Children:")
-                    tree.add(indirect_tree)
-                indirect_tree.add(f"[indirect]{child}")
-            self._print(f"```diff\n{context_diff.text_diff(snapshot.name)}\n```\n")
-            self._print("```\n")
-            self._print(tree)
-            self._print("\n```")
-
-    def log_test_results(
-        self, result: unittest.result.TestResult, output: str, target_dialect: str
-    ) -> None:
-        # import ipywidgets as widgets
-        if result.wasSuccessful():
-            self._print(
-                f"**Successfully Ran `{str(result.testsRun)}` Tests Against `{target_dialect}`**\n\n"
-            )
-        else:
-            self._print(
-                f"**Num Successful Tests: {result.testsRun - len(result.failures) - len(result.errors)}**\n\n"
-            )
-            for test, _ in result.failures + result.errors:
-                if isinstance(test, ModelTest):
-                    self._print(f"* Failure Test: `{test.model_name}` - `{test.test_name}`\n\n")
-            self._print(f"```{output}```\n\n")
-
-
-class DatabricksMagicConsole(CaptureTerminalConsole):
+class DatabricksMagicConsole(TerminalConsole):
     """
     Note: Databricks Magic Console currently does not support progress bars while a plan is being applied. The
     NotebookMagicConsole does support progress bars, but they will time out after 5 minutes of execution
     and it makes it difficult to see the progress of the plan.
     """
 
     def _print(self, value: t.Any, **kwargs: t.Any) -> None:
-        super()._print(value, **kwargs)
-        for captured_output in self._captured_outputs:
-            print(captured_output)
-        self.clear_captured_outputs()
+        with self.console.capture() as capture:
+            self.console.print(value, **kwargs)
+        output = capture.get()
+        print(output)
 
     def _prompt(self, message: str, **kwargs: t.Any) -> t.Any:
         self._print(message)
         return super()._prompt("", **kwargs)
 
     def _confirm(self, message: str, **kwargs: t.Any) -> bool:
         message = f"{message} [y/n]"
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/constants.py` & `sqlmesh-0.7.0/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/context.py` & `sqlmesh-0.7.0/sqlmesh/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,19 +240,14 @@
 
         self._provided_state_sync: t.Optional[StateSync] = state_sync
         self._state_sync: t.Optional[StateSync] = None
         self._state_reader: t.Optional[StateReader] = None
 
         self._loader = (loader or self.config.loader or SqlMeshLoader)()
 
-        # Should we dedupe notification_targets? If so how?
-        self.notification_targets = (notification_targets or []) + self.config.notification_targets
-        self.users = (users or []) + self.config.users
-        self.users = list({user.username: user for user in self.users}.values())
-
         if load:
             self.load()
 
     @property
     def engine_adapter(self) -> EngineAdapter:
         """Returns an engine adapter."""
         return self._engine_adapter
@@ -862,25 +857,22 @@
                 self.test_connection or test_connection_name_in_config, self._test_engine_adapter
             )
 
     def close(self) -> None:
         """Releases all resources allocated by this context."""
         self.snapshot_evaluator.close()
 
-    def _run_tests(self) -> t.Tuple[unittest.result.TestResult, str]:
-        test_output_io = StringIO()
-        with contextlib.redirect_stderr(test_output_io):
-            result = self.test()
-        return result, test_output_io.getvalue()
-
     def _run_plan_tests(
         self, skip_tests: bool = False
     ) -> t.Tuple[t.Optional[unittest.result.TestResult], t.Optional[str]]:
         if self._test_engine_adapter and not skip_tests:
-            result, test_output = self._run_tests()
+            test_output_io = StringIO()
+            with contextlib.redirect_stderr(test_output_io):
+                result = self.test()
+            test_output = test_output_io.getvalue()
             self.console.log_test_results(result, test_output, self._test_engine_adapter.dialect)
             if not result.wasSuccessful():
                 raise PlanError(
                     "Cannot generate plan due to failing test(s). Fix test(s) and run again"
                 )
             return result, test_output
         return None, None
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/context_diff.py` & `sqlmesh-0.7.0/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/dialect.py` & `sqlmesh-0.7.0/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.7.0/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/environment.py` & `sqlmesh-0.7.0/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/hooks.py` & `sqlmesh-0.7.0/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/loader.py` & `sqlmesh-0.7.0/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/macros.py` & `sqlmesh-0.7.0/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/cache.py` & `sqlmesh-0.7.0/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/common.py` & `sqlmesh-0.7.0/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/decorator.py` & `sqlmesh-0.7.0/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/kind.py` & `sqlmesh-0.7.0/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/meta.py` & `sqlmesh-0.7.0/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/model/seed.py` & `sqlmesh-0.7.0/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/notification_target.py` & `sqlmesh-0.7.0/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/plan/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/plan/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     Intervals,
     Snapshot,
     SnapshotChangeCategory,
     SnapshotId,
     categorize_change,
     merge_intervals,
 )
-from sqlmesh.core.snapshot.definition import _format_date_time
 from sqlmesh.core.state_sync import StateReader
 from sqlmesh.utils import random_id
 from sqlmesh.utils.dag import DAG
 from sqlmesh.utils.date import (
     TimeLike,
     make_inclusive,
     make_inclusive_end,
     now,
     to_date,
     to_datetime,
+    to_ds,
     to_timestamp,
     validate_date_range,
     yesterday_ds,
 )
 from sqlmesh.utils.errors import PlanError, SQLMeshError
 from sqlmesh.utils.pydantic import PydanticModel
 
@@ -305,15 +305,15 @@
 
             if choice in (
                 SnapshotChangeCategory.BREAKING,
                 SnapshotChangeCategory.INDIRECT_BREAKING,
             ):
                 child_snapshot.categorize_as(SnapshotChangeCategory.INDIRECT_BREAKING)
             else:
-                child_snapshot.categorize_as(SnapshotChangeCategory.INDIRECT_NON_BREAKING)
+                child_snapshot.categorize_as(SnapshotChangeCategory.INDIRECT_FORWARD_ONLY)
             snapshot.indirect_versions[child] = child_snapshot.all_versions
 
             # If any other snapshot specified breaking this child, then that child
             # needs to be backfilled as a part of the plan.
             for upstream in self.directly_modified:
                 if child in upstream.indirect_versions:
                     data_version = upstream.indirect_versions[child][-1]
@@ -402,15 +402,15 @@
             if not downstream:
                 raise PlanError(
                     f"Cannot restate from '{table}'. Either such model doesn't exist or no other model references it."
                 )
             self._restatements.update(downstream)
 
     def _build_directly_and_indirectly_modified(self) -> t.Tuple[t.List[Snapshot], SnapshotMapping]:
-        """Builds collections of directly and indirectly modified snapshots.
+        """Builds collections of directly and inderectly modified snapshots.
 
         Returns:
             The tuple in which the first element contains a list of added and directly modified
             snapshots while the second element contains a mapping of indirectly modified snapshots.
         """
         directly_modified = []
         all_indirectly_modified = set()
@@ -439,23 +439,21 @@
         """Automatically categorizes snapshots that can be automatically categorized and
         returns a list of added and directly modified snapshots as well as the mapping of
         indirectly modified snapshots.
         """
         for model_name, snapshot in self.context_diff.snapshots.items():
             upstream_model_names = self._dag.upstream(model_name)
 
+            if not self.forward_only:
+                self._ensure_no_paused_forward_only_upstream(model_name, upstream_model_names)
+
             if model_name in self.context_diff.modified_snapshots:
                 is_directly_modified = self.context_diff.directly_modified(model_name)
 
                 if self.is_new_snapshot(snapshot):
-                    if not self.forward_only:
-                        self._ensure_no_paused_forward_only_upstream(
-                            model_name, upstream_model_names
-                        )
-
                     if self.forward_only:
                         # In case of the forward only plan any modifications result in reuse of the
                         # previous version for non-seed models.
                         # New snapshots of seed models are considered non-breaking ones.
                         if not snapshot.is_seed_kind:
                             snapshot.categorize_as(SnapshotChangeCategory.FORWARD_ONLY)
                         else:
@@ -575,7 +573,13 @@
 
     def format_missing_range(self, unit: t.Optional[IntervalUnit] = None) -> str:
         intervals = [make_inclusive(start, end) for start, end in self.merged_intervals]
         return ", ".join(
             f"({_format_date_time(start, unit)}, {_format_date_time(end, unit)})"
             for start, end in intervals
         )
+
+
+def _format_date_time(time_like: TimeLike, unit: t.Optional[IntervalUnit]) -> str:
+    if unit is None or unit == IntervalUnit.DAY:
+        return to_ds(time_like)
+    return to_datetime(time_like).isoformat()[:19]
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.7.0/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/renderer.py` & `sqlmesh-0.7.0/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/scheduler.py` & `sqlmesh-0.7.0/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/schema_diff.py` & `sqlmesh-0.7.0/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,22 @@
     Model,
     PythonModel,
     SeedModel,
     SqlModel,
     kind,
     parse_model_name,
 )
-from sqlmesh.core.model.meta import HookCall, IntervalUnit
+from sqlmesh.core.model.meta import HookCall
 from sqlmesh.utils.date import (
     TimeLike,
     is_date,
     make_inclusive_end,
     now,
     now_timestamp,
     to_datetime,
-    to_ds,
     to_timestamp,
 )
 from sqlmesh.utils.errors import SQLMeshError
 from sqlmesh.utils.pydantic import PydanticModel
 
 Interval = t.Tuple[int, int]
 Intervals = t.List[Interval]
@@ -41,42 +40,22 @@
     """
     Values are ordered by decreasing severity and that ordering is required.
 
     BREAKING: The change requires that snapshot modified and downstream dependencies be rebuilt
     NON_BREAKING: The change requires that only the snapshot modified be rebuilt
     FORWARD_ONLY: The change requires no rebuilding
     INDIRECT_BREAKING: The change was caused indirectly and is breaking.
-    INDIRECT_NON_BREAKING: The change was caused indirectly by a non-breaking change.
+    INDIRECT_FORWARD_ONLY: The change was caused indirectly and is forward-only.
     """
 
     BREAKING = 1
     NON_BREAKING = 2
     FORWARD_ONLY = 3
     INDIRECT_BREAKING = 4
-    INDIRECT_NON_BREAKING = 5
-
-    @property
-    def is_breaking(self) -> bool:
-        return self == self.BREAKING
-
-    @property
-    def is_non_breaking(self) -> bool:
-        return self == self.NON_BREAKING
-
-    @property
-    def is_forward_only(self) -> bool:
-        return self == self.FORWARD_ONLY
-
-    @property
-    def is_indirect_breaking(self) -> bool:
-        return self == self.INDIRECT_BREAKING
-
-    @property
-    def is_indirect_non_breaking(self) -> bool:
-        return self == self.INDIRECT_NON_BREAKING
+    INDIRECT_FORWARD_ONLY = 5
 
 
 class SnapshotFingerprint(PydanticModel, frozen=True):
     data_hash: str
     metadata_hash: str
     parent_data_hash: str = "0"
     parent_metadata_hash: str = "0"
@@ -160,15 +139,15 @@
     physical_schema: str
     previous_versions: t.Tuple[SnapshotDataVersion, ...] = ()
 
     def is_temporary_table(self, is_dev: bool) -> bool:
         """Provided whether the snapshot is used in a development mode or not, returns True
         if the snapshot targets a temporary table or a clone and False otherwise.
         """
-        return is_dev and (self.is_forward_only or self.is_indirect_non_breaking)
+        return is_dev and (self.is_forward_only or self.is_indirect_forward_only)
 
     @property
     def identifier(self) -> str:
         return self.fingerprint.to_identifier()
 
     @property
     def snapshot_id(self) -> SnapshotId:
@@ -195,16 +174,16 @@
         raise NotImplementedError
 
     @property
     def is_forward_only(self) -> bool:
         return self.change_category == SnapshotChangeCategory.FORWARD_ONLY
 
     @property
-    def is_indirect_non_breaking(self) -> bool:
-        return self.change_category == SnapshotChangeCategory.INDIRECT_NON_BREAKING
+    def is_indirect_forward_only(self) -> bool:
+        return self.change_category == SnapshotChangeCategory.INDIRECT_FORWARD_ONLY
 
     @property
     def all_versions(self) -> t.Tuple[SnapshotDataVersion, ...]:
         """Returns previous versions with the current version trimmed to DATA_VERSION_LIMIT."""
         return (*self.previous_versions, self.data_version)[-c.DATA_VERSION_LIMIT :]
 
     def data_hash_matches(self, other: t.Optional[SnapshotInfoMixin | SnapshotDataVersion]) -> bool:
@@ -221,15 +200,15 @@
         if is_dev and for_read:
             # If this snapshot is used for **reading**, return a temporary table
             # only if this snapshot captures a direct forward-only change applied to its model.
             is_temp = self.is_forward_only
         elif is_dev:
             # Use a temporary table in the dev environment when **writing** a forward-only snapshot
             # which was modified either directly or indirectly.
-            is_temp = self.is_forward_only or self.is_indirect_non_breaking
+            is_temp = self.is_forward_only or self.is_indirect_forward_only
         else:
             is_temp = False
 
         if is_temp:
             version = self.temp_version or self.fingerprint.to_version()
 
         return table_name(
@@ -608,15 +587,15 @@
         """Assigns the given category to this snapshot.
 
         Args:
             category: The change category to assign to this snapshot.
         """
         is_forward_only = category in (
             SnapshotChangeCategory.FORWARD_ONLY,
-            SnapshotChangeCategory.INDIRECT_NON_BREAKING,
+            SnapshotChangeCategory.INDIRECT_FORWARD_ONLY,
         )
         if is_forward_only and self.previous_version:
             self.version = self.previous_version.data_version.version
         else:
             self.version = self.fingerprint.to_version()
 
         self.change_category = category
@@ -948,20 +927,14 @@
             merged[-1] = (current[0], max(current[1], interval[1]))
         else:
             merged.append(interval)
 
     return merged
 
 
-def _format_date_time(time_like: TimeLike, unit: t.Optional[IntervalUnit]) -> str:
-    if unit is None or unit == IntervalUnit.DAY:
-        return to_ds(time_like)
-    return to_datetime(time_like).isoformat()[:19]
-
-
 def remove_interval(intervals: Intervals, remove_start: int, remove_end: int) -> Intervals:
     """Remove an interval from a list of intervals.
 
     Args:
         intervals: A list of exclusive intervals.
         remove_start: The inclusive start to remove.
         remove_end: The exclusive end to remove.
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.7.0/sqlmesh/core/snapshot/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         if snapshot.is_embedded_kind:
             return
 
         self.adapter.create_schema(snapshot.physical_schema)
 
         # If a snapshot reuses an existing version we assume that the table for that version
         # has already been created, so we only need to create a temporary table or a clone.
-        is_dev = snapshot.is_forward_only or snapshot.is_indirect_non_breaking
+        is_dev = snapshot.is_forward_only or snapshot.is_indirect_forward_only
         table_name = snapshot.table_name(is_dev=is_dev)
 
         parent_snapshots_by_name = {
             snapshots[p_sid].name: snapshots[p_sid] for p_sid in snapshot.parents
         }
 
         if snapshot.is_view_kind:
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.7.0/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
 
             # Infer the missing change category to account for SQLMesh versions in which
             # we didn't assign a change category to indirectly modified snapshots.
             if not new_snapshot.change_category:
                 new_snapshot.change_category = (
                     SnapshotChangeCategory.INDIRECT_BREAKING
                     if snapshot.fingerprint.to_version() == snapshot.version
-                    else SnapshotChangeCategory.INDIRECT_NON_BREAKING
+                    else SnapshotChangeCategory.INDIRECT_FORWARD_ONLY
                 )
 
             if not new_snapshot.temp_version:
                 new_snapshot.temp_version = snapshot.fingerprint.to_version()
 
             if new_snapshot == snapshot:
                 logger.debug(f"{new_snapshot.snapshot_id} is unchanged.")
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/test.py` & `sqlmesh-0.7.0/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/core/user.py` & `sqlmesh-0.7.0/sqlmesh/core/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 
 from sqlmesh.utils.pydantic import PydanticModel
 
 
 class UserRole(str, Enum):
     """A role to associate the user with"""
 
-    REQUIRED_APPROVER = "required_approver"
+    GATEKEEPER = "gatekeeper"
+    BOT = "bot"
 
     @property
-    def is_required_approver(self) -> bool:
-        return self == UserRole.REQUIRED_APPROVER
+    def is_gatekeeper(self) -> bool:
+        return self == UserRole.GATEKEEPER
+
+    @property
+    def is_bot(self) -> bool:
+        return self == UserRole.BOT
 
 
 class User(PydanticModel):
     """SQLMesh user information that can be used for notifications"""
 
     username: str
     """The name to refer to the user"""
@@ -25,10 +30,18 @@
     """The slack username"""
     email: t.Optional[str] = None
     """The email for the user (full address)"""
     roles: t.List[UserRole] = []
     """List of roles to associate with the user"""
 
     @property
-    def is_required_approver(self) -> bool:
-        """Indicates if this is a required approver for PR approvals."""
-        return UserRole.REQUIRED_APPROVER in self.roles
+    def is_gatekeeper(self) -> bool:
+        """Indicates if this is a gatekeeper for PR approvals.
+        TODO: Users should be able to define this on a "per-project" level but that requires adding the concept of
+        "projects" to SQLMesh so making this a global config for now
+        """
+        return UserRole.GATEKEEPER in self.roles
+
+    @property
+    def is_bot(self) -> bool:
+        """Indicates if this is a CI/CD bot account. There should only be one of these per project"""
+        return UserRole.BOT in self.roles
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/adapter.py` & `sqlmesh-0.7.0/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.7.0/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/builtin.py` & `sqlmesh-0.7.0/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/column.py` & `sqlmesh-0.7.0/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/common.py` & `sqlmesh-0.7.0/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/context.py` & `sqlmesh-0.7.0/sqlmesh/dbt/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/loader.py` & `sqlmesh-0.7.0/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/model.py` & `sqlmesh-0.7.0/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/package.py` & `sqlmesh-0.7.0/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/profile.py` & `sqlmesh-0.7.0/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/project.py` & `sqlmesh-0.7.0/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/seed.py` & `sqlmesh-0.7.0/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/source.py` & `sqlmesh-0.7.0/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/dbt/target.py` & `sqlmesh-0.7.0/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/engines/commands.py` & `sqlmesh-0.7.0/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/app.py` & `sqlmesh-0.7.0/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.7.0/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.7.0/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/magics.py` & `sqlmesh-0.7.0/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py` & `sqlmesh-0.7.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.7.0/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/__init__.py` & `sqlmesh-0.7.0/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/cache.py` & `sqlmesh-0.7.0/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/concurrency.py` & `sqlmesh-0.7.0/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.7.0/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/dag.py` & `sqlmesh-0.7.0/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/date.py` & `sqlmesh-0.7.0/sqlmesh/utils/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,40 +154,41 @@
         A date object with tz utc.
     """
     return to_datetime(value, relative_base).date()
 
 
 def date_dict(
     start: TimeLike, end: TimeLike, latest: TimeLike, only_latest: bool = False
-) -> t.Dict[str, t.Union[str, datetime, float, int]]:
+) -> t.Dict[str, t.Union[str, datetime, date, float, int]]:
     """Creates a kwarg dictionary of datetime variables for use in SQL Contexts.
 
     Keys are like start_date, start_ds, end_date, end_ds...
 
     Args:
         start: Start time.
         end: End time.
         latest: Latest time.
         only_latest: Only the latest timestamps will be returned.
 
     Returns:
         A dictionary with various keys pointing to datetime formats.
     """
-    kwargs: t.Dict[str, t.Union[str, datetime, float, int]] = {}
+    kwargs: t.Dict[str, t.Union[str, datetime, date, float, int]] = {}
 
     prefixes = [("latest", to_datetime(latest))]
 
     if not only_latest:
         prefixes.append(("start", to_datetime(start)))
         prefixes.append(("end", to_datetime(end)))
 
     for prefix, time_like in prefixes:
         dt = to_datetime(time_like)
         millis = to_timestamp(time_like)
-        kwargs[f"{prefix}_date"] = dt
+        kwargs[f"{prefix}_dt"] = dt
+        kwargs[f"{prefix}_date"] = to_date(dt)
         kwargs[f"{prefix}_ds"] = to_ds(time_like)
         kwargs[f"{prefix}_ts"] = dt.isoformat()
         kwargs[f"{prefix}_epoch"] = millis / 1000
         kwargs[f"{prefix}_millis"] = millis
     return kwargs
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/errors.py` & `sqlmesh-0.7.0/sqlmesh/utils/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,18 +69,14 @@
     pass
 
 
 class NotFoundError(ApiClientError):
     pass
 
 
-class CICDBotError(SQLMeshError):
-    pass
-
-
 def raise_config_error(
     msg: str,
     location: t.Optional[str | Path] = None,
     error_type: t.Type[ConfigError] = ConfigError,
 ) -> None:
     if location:
         raise error_type(f"{msg} at '{location}'")
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/jinja.py` & `sqlmesh-0.7.0/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.7.0/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/pandas.py` & `sqlmesh-0.7.0/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/pydantic.py` & `sqlmesh-0.7.0/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/rich.py` & `sqlmesh-0.7.0/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.7.0/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh/utils/yaml.py` & `sqlmesh-0.7.0/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.7.0/sqlmesh.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.5.dev5
-Summary: UNKNOWN
+Version: 0.7.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: bigquery
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
-Provides-Extra: github
+Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.7.0/sqlmesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,14 @@
 docs/guides/scheduling/airflow_successful_plan_apply.png
 docs/guides/scheduling/airflow_successful_setup.png
 docs/integrations/airflow.md
 docs/integrations/dbt.md
 docs/integrations/engines.md
 docs/integrations/github.md
 docs/integrations/overview.md
-docs/integrations/images/github_deployed_plans.png
-docs/integrations/images/github_env_summary.png
-docs/integrations/images/github_prod_plan_preview.png
-docs/integrations/images/github_reviewers.png
-docs/integrations/images/github_test_summary.png
 docs/reference/cli.md
 docs/reference/configuration.md
 docs/reference/notebook.md
 docs/reference/overview.md
 docs/reference/python.md
 examples/__init__.py
 examples/airflow/Dockerfile.template
@@ -178,16 +173,14 @@
 sqlmesh/py.typed
 sqlmesh.egg-info/PKG-INFO
 sqlmesh.egg-info/SOURCES.txt
 sqlmesh.egg-info/dependency_links.txt
 sqlmesh.egg-info/entry_points.txt
 sqlmesh.egg-info/requires.txt
 sqlmesh.egg-info/top_level.txt
-sqlmesh/cicd/__init__.py
-sqlmesh/cicd/bot.py
 sqlmesh/cli/__init__.py
 sqlmesh/cli/example_project.py
 sqlmesh/cli/main.py
 sqlmesh/cli/options.py
 sqlmesh/core/__init__.py
 sqlmesh/core/_typing.py
 sqlmesh/core/console.py
@@ -270,22 +263,19 @@
 sqlmesh/engines/commands.py
 sqlmesh/engines/spark/__init__.py
 sqlmesh/engines/spark/app.py
 sqlmesh/engines/spark/db_api/__init__.py
 sqlmesh/engines/spark/db_api/errors.py
 sqlmesh/engines/spark/db_api/spark_session.py
 sqlmesh/integrations/__init__.py
+sqlmesh/integrations/llm.py
 sqlmesh/integrations/github/__init__.py
 sqlmesh/integrations/github/notification_operator_provider.py
 sqlmesh/integrations/github/notification_target.py
 sqlmesh/integrations/github/shared.py
-sqlmesh/integrations/github/cicd/__init__.py
-sqlmesh/integrations/github/cicd/command.py
-sqlmesh/integrations/github/cicd/controller.py
-sqlmesh/integrations/github/cicd/options.py
 sqlmesh/migrations/__init__.py
 sqlmesh/migrations/v0001_init.py
 sqlmesh/migrations/v0002_remove_identify.py
 sqlmesh/migrations/v0003_move_batch_size.py
 sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
 sqlmesh/schedulers/__init__.py
 sqlmesh/schedulers/airflow/__init__.py
@@ -441,14 +431,26 @@
 web/client/package-lock.json
 web/client/package.json
 web/client/playwright.config.ts
 web/client/postcss.config.js
 web/client/tailwind.config.js
 web/client/tsconfig.json
 web/client/vite.config.ts
+web/client/dist/index.html
+web/client/dist/assets/CircularStd-Black-52659624.otf
+web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+web/client/dist/assets/Plan-683a0552.js
+web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+web/client/dist/assets/Publico-Bold-c79acd56.otf
+web/client/dist/assets/Publico-Medium-01b4a891.otf
+web/client/dist/assets/index-b61dbb6f.css
+web/client/dist/assets/index-f2c4b7c5.js
+web/client/dist/assets/worker-e891d118.js
+web/client/dist/favicons/favicon.ico
 web/client/public/favicons/favicon.ico
 web/client/src/index.css
 web/client/src/main.tsx
 web/client/src/routes.tsx
 web/client/src/api/channels.ts
 web/client/src/api/index.ts
 web/client/src/api/instance.ts
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.7.0/sqlmesh.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -49,16 +49,17 @@
 sqlalchemy-stubs
 tenacity==8.1.0
 types-croniter
 types-dateparser
 types-pytz
 types-requests==2.28.8
 
-[github]
-PyGithub
+[llm]
+langchain
+openai
 
 [postgres]
 psycopg2
 
 [redshift]
 redshift_connector
```

### Comparing `sqlmesh-0.6.5.dev5/sqlmesh.svg` & `sqlmesh-0.7.0/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/conftest.py` & `sqlmesh-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.7.0/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_audit.py` & `sqlmesh-0.7.0/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_config.py` & `sqlmesh-0.7.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_connection_config.py` & `sqlmesh-0.7.0/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_context.py` & `sqlmesh-0.7.0/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_dialect.py` & `sqlmesh-0.7.0/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_integration.py` & `sqlmesh-0.7.0/tests/core/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
 
     model = t.cast(SqlModel, sushi_context.models["sushi.waiters"])
     sushi_context.upsert_model("sushi.waiters", query=model.query.select("'foo' AS foo"))  # type: ignore
     apply_to_environment(sushi_context, environment)
 
     assert (
         sushi_context.snapshots["sushi.waiter_as_customer_by_day"].change_category
-        == SnapshotChangeCategory.INDIRECT_NON_BREAKING
+        == SnapshotChangeCategory.INDIRECT_FORWARD_ONLY
     )
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].fingerprint != fingerprint
     assert sushi_context.snapshots["sushi.waiter_as_customer_by_day"].version == version
 
 
 @pytest.mark.integration
 @pytest.mark.core_integration
```

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_macros.py` & `sqlmesh-0.7.0/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_model.py` & `sqlmesh-0.7.0/tests/core/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,29 +546,33 @@
         model.render_query(start="2020-10-28", end="2020-10-28"),
         """
         SELECT
           x.y AS y
         FROM x AS x
         WHERE
           x.y <= '2020-10-28'
+          AND x.y <= DATE_STR_TO_DATE('2020-10-28')
           AND x.y <= TIME_STR_TO_TIME('2020-10-28T23:59:59.999000+00:00')
           AND x.y >= '2020-10-28'
+          AND x.y >= DATE_STR_TO_DATE('2020-10-28')
           AND x.y >= TIME_STR_TO_TIME('2020-10-28T00:00:00+00:00')
         """,
     )
     assert_exp_eq(
         model.render_query(start="2020-10-28", end=to_datetime("2020-10-29")),
         """
         SELECT
           x.y AS y
         FROM x AS x
         WHERE
           x.y <= '2020-10-28'
+          AND x.y <= DATE_STR_TO_DATE('2020-10-28')
           AND x.y <= TIME_STR_TO_TIME('2020-10-28T23:59:59.999000+00:00')
           AND x.y >= '2020-10-28'
+          AND x.y >= DATE_STR_TO_DATE('2020-10-28')
           AND x.y >= TIME_STR_TO_TIME('2020-10-28T00:00:00+00:00')
         """,
     )
 
 
 def test_time_column():
     expressions = parse(
```

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_plan.py` & `sqlmesh-0.7.0/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_plan_evaluator.py` & `sqlmesh-0.7.0/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_scheduler.py` & `sqlmesh-0.7.0/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_schema_diff.py` & `sqlmesh-0.7.0/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_seed.py` & `sqlmesh-0.7.0/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_snapshot.py` & `sqlmesh-0.7.0/tests/core/test_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
 
     # Mimic an indirect forward-only change.
     previous_data_version = snapshot.data_version
     snapshot.fingerprint = SnapshotFingerprint(
         data_hash="1", metadata_hash="1", parent_data_hash="2"
     )
     snapshot.previous_versions = (previous_data_version,)
-    snapshot.categorize_as(SnapshotChangeCategory.INDIRECT_NON_BREAKING)
+    snapshot.categorize_as(SnapshotChangeCategory.INDIRECT_FORWARD_ONLY)
     assert snapshot.table_name(is_dev=False, for_read=False) == "sqlmesh.name__3078928823"
     assert snapshot.table_name(is_dev=True, for_read=False) == "sqlmesh.name__781051917__temp"
     assert snapshot.table_name(is_dev=False, for_read=True) == "sqlmesh.name__3078928823"
     assert snapshot.table_name(is_dev=True, for_read=True) == "sqlmesh.name__3078928823"
     assert snapshot.table_name_for_mapping(is_dev=False) == "sqlmesh.name__3078928823"
     assert snapshot.table_name_for_mapping(is_dev=True) == "sqlmesh.name__3078928823"
```

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.7.0/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/core/test_state_sync.py` & `sqlmesh-0.7.0/tests/core/test_state_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
     snapshot = make_snapshot(model, version="a")
     snapshot.change_category = SnapshotChangeCategory.BREAKING
     snapshot.add_interval("2022-01-01", "2022-01-02")
     state_sync.push_snapshots([snapshot])
     promote_snapshots(state_sync, [snapshot], "prod", no_gaps=True)
 
     new_snapshot_same_version = make_snapshot(model, version="a")
-    new_snapshot_same_version.change_category = SnapshotChangeCategory.INDIRECT_NON_BREAKING
+    new_snapshot_same_version.change_category = SnapshotChangeCategory.INDIRECT_FORWARD_ONLY
     new_snapshot_same_version.fingerprint = snapshot.fingerprint.copy(
         update={"data_hash": "new_snapshot_same_version"}
     )
     new_snapshot_same_version.add_interval("2022-01-03", "2022-01-03")
     state_sync.push_snapshots([new_snapshot_same_version])
     promote_snapshots(state_sync, [new_snapshot_same_version], "prod", no_gaps=True)
```

### Comparing `sqlmesh-0.6.5.dev5/tests/dbt/conftest.py` & `sqlmesh-0.7.0/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/dbt/test_adapter.py` & `sqlmesh-0.7.0/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/dbt/test_config.py` & `sqlmesh-0.7.0/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/dbt/test_transformation.py` & `sqlmesh-0.7.0/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/engines/spark/test_db_api.py` & `sqlmesh-0.7.0/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.7.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/migrations/environments.json` & `sqlmesh-0.7.0/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.7.0/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.7.0/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.7.0/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_cache.py` & `sqlmesh-0.7.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_concurrency.py` & `sqlmesh-0.7.0/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_connection_pool.py` & `sqlmesh-0.7.0/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_dag.py` & `sqlmesh-0.7.0/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_date.py` & `sqlmesh-0.7.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_filesystem.py` & `sqlmesh-0.7.0/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_jinja.py` & `sqlmesh-0.7.0/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_metaprogramming.py` & `sqlmesh-0.7.0/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_pandas.py` & `sqlmesh-0.7.0/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_pydantic.py` & `sqlmesh-0.7.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_transactional_file.py` & `sqlmesh-0.7.0/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/utils/test_yaml.py` & `sqlmesh-0.7.0/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/tests/web/test_main.py` & `sqlmesh-0.7.0/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/.eslintrc.js` & `sqlmesh-0.7.0/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/index.html` & `sqlmesh-0.7.0/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/openapi.json` & `sqlmesh-0.7.0/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/package-lock.json` & `sqlmesh-0.7.0/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/package.json` & `sqlmesh-0.7.0/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/playwright.config.ts` & `sqlmesh-0.7.0/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/public/favicons/favicon.ico` & `sqlmesh-0.7.0/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/api/channels.ts` & `sqlmesh-0.7.0/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/api/index.ts` & `sqlmesh-0.7.0/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/api/instance.ts` & `sqlmesh-0.7.0/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.7.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.7.0/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.7.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/context.ts` & `sqlmesh-0.7.0/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/editor.ts` & `sqlmesh-0.7.0/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/fileTree.ts` & `sqlmesh-0.7.0/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/lineage.tsx` & `sqlmesh-0.7.0/web/client/src/context/lineage.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/plan.ts` & `sqlmesh-0.7.0/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/context/theme.tsx` & `sqlmesh-0.7.0/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.7.0/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/index.css` & `sqlmesh-0.7.0/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.7.0/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.7.0/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/main.tsx` & `sqlmesh-0.7.0/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/models/artifact.ts` & `sqlmesh-0.7.0/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/models/directory.ts` & `sqlmesh-0.7.0/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/models/environment.ts` & `sqlmesh-0.7.0/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/models/file.ts` & `sqlmesh-0.7.0/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/models/initial.ts` & `sqlmesh-0.7.0/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/tests/utils.tsx` & `sqlmesh-0.7.0/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/utils/index.spec.ts` & `sqlmesh-0.7.0/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/utils/index.ts` & `sqlmesh-0.7.0/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.7.0/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.7.0/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/tailwind.config.js` & `sqlmesh-0.7.0/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/tsconfig.json` & `sqlmesh-0.7.0/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/client/vite.config.ts` & `sqlmesh-0.7.0/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/__init__.py` & `sqlmesh-0.7.0/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/commands.py` & `sqlmesh-0.7.0/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/context.py` & `sqlmesh-0.7.0/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/directories.py` & `sqlmesh-0.7.0/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/environments.py` & `sqlmesh-0.7.0/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/events.py` & `sqlmesh-0.7.0/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/files.py` & `sqlmesh-0.7.0/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/lineage.py` & `sqlmesh-0.7.0/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/models.py` & `sqlmesh-0.7.0/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/api/endpoints/plan.py` & `sqlmesh-0.7.0/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/console.py` & `sqlmesh-0.7.0/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/main.py` & `sqlmesh-0.7.0/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/models.py` & `sqlmesh-0.7.0/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/settings.py` & `sqlmesh-0.7.0/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/sse.py` & `sqlmesh-0.7.0/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/utils.py` & `sqlmesh-0.7.0/web/server/utils.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.5.dev5/web/server/watcher.py` & `sqlmesh-0.7.0/web/server/watcher.py`

 * *Files identical despite different names*

