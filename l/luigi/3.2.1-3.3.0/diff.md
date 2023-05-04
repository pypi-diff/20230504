# Comparing `tmp/luigi-3.2.1.tar.gz` & `tmp/luigi-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luigi-3.2.1.tar", last modified: Tue Mar 14 09:46:32 2023, max compression
+gzip compressed data, was "luigi-3.3.0.tar", last modified: Thu May  4 09:32:34 2023, max compression
```

## Comparing `luigi-3.2.1.tar` & `luigi-3.3.0.tar`

### file list

```diff
@@ -1,316 +1,316 @@
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.257763 luigi-3.2.1/
--rw-r--r--   0 honnix     (501) staff       (20)    11345 2022-06-09 13:02:03.000000 luigi-3.2.1/LICENSE
--rw-r--r--   0 honnix     (501) staff       (20)      140 2018-03-13 15:21:03.000000 luigi-3.2.1/MANIFEST.in
--rw-r--r--   0 honnix     (501) staff       (20)    13833 2023-03-14 09:46:32.257415 luigi-3.2.1/PKG-INFO
--rw-r--r--   0 honnix     (501) staff       (20)    12747 2023-01-16 12:13:44.000000 luigi-3.2.1/README.rst
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.362716 luigi-3.2.1/examples/
--rw-r--r--   0 honnix     (501) staff       (20)      603 2018-03-13 15:21:03.000000 luigi-3.2.1/examples/__init__.py
--rw-r--r--   0 honnix     (501) staff       (20)     3746 2023-01-16 12:13:44.000000 luigi-3.2.1/examples/dynamic_requirements.py
--rw-r--r--   0 honnix     (501) staff       (20)     3410 2018-03-13 15:21:03.000000 luigi-3.2.1/examples/elasticsearch_index.py
--rw-r--r--   0 honnix     (501) staff       (20)     3319 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/execution_summary_example.py
--rw-r--r--   0 honnix     (501) staff       (20)     1462 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/foo.py
--rw-r--r--   0 honnix     (501) staff       (20)     1876 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/foo_complex.py
--rw-r--r--   0 honnix     (501) staff       (20)     3239 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/ftp_experiment_outputs.py
--rw-r--r--   0 honnix     (501) staff       (20)      500 2020-05-20 08:28:52.000000 luigi-3.2.1/examples/hello_world.py
--rw-r--r--   0 honnix     (501) staff       (20)     1986 2020-06-01 12:15:59.000000 luigi-3.2.1/examples/kubernetes.py
--rw-r--r--   0 honnix     (501) staff       (20)     5264 2018-08-22 11:25:34.000000 luigi-3.2.1/examples/per_task_retry_policy.py
--rw-r--r--   0 honnix     (501) staff       (20)     3388 2019-12-16 11:25:16.000000 luigi-3.2.1/examples/pyspark_wc.py
--rw-r--r--   0 honnix     (501) staff       (20)     4363 2019-12-16 11:25:16.000000 luigi-3.2.1/examples/spark_als.py
--rw-r--r--   0 honnix     (501) staff       (20)     2823 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/ssh_remote_execution.py
--rw-r--r--   0 honnix     (501) staff       (20)     3400 2018-03-13 15:21:03.000000 luigi-3.2.1/examples/terasort.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     9069 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/top_artists.py
--rwxr-xr-x   0 honnix     (501) staff       (20)      645 2019-05-06 14:47:19.000000 luigi-3.2.1/examples/top_artists_spark.py
--rw-r--r--   0 honnix     (501) staff       (20)     2904 2020-06-01 20:15:53.000000 luigi-3.2.1/examples/wordcount.py
--rw-r--r--   0 honnix     (501) staff       (20)     2729 2019-12-16 11:25:16.000000 luigi-3.2.1/examples/wordcount_hadoop.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.442974 luigi-3.2.1/luigi/
--rw-r--r--   0 honnix     (501) staff       (20)     3723 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/__init__.py
--rw-r--r--   0 honnix     (501) staff       (20)      683 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/__main__.py
--rw-r--r--   0 honnix     (501) staff       (20)      249 2023-03-14 09:46:21.000000 luigi-3.2.1/luigi/__meta__.py
--rw-r--r--   0 honnix     (501) staff       (20)     8863 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/batch_notifier.py
--rw-r--r--   0 honnix     (501) staff       (20)     1426 2018-12-19 13:45:13.000000 luigi-3.2.1/luigi/cmdline.py
--rw-r--r--   0 honnix     (501) staff       (20)     5458 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/cmdline_parser.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.539602 luigi-3.2.1/luigi/configuration/
--rw-r--r--   0 honnix     (501) staff       (20)      837 2019-12-16 11:25:16.000000 luigi-3.2.1/luigi/configuration/__init__.py
--rw-r--r--   0 honnix     (501) staff       (20)     1307 2018-08-22 11:25:34.000000 luigi-3.2.1/luigi/configuration/base_parser.py
--rw-r--r--   0 honnix     (501) staff       (20)     8402 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/configuration/cfg_parser.py
--rw-r--r--   0 honnix     (501) staff       (20)     2760 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/configuration/core.py
--rw-r--r--   0 honnix     (501) staff       (20)     2831 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/configuration/toml_parser.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.746751 luigi-3.2.1/luigi/contrib/
--rw-r--r--   0 honnix     (501) staff       (20)      661 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/contrib/__init__.py
--rw-r--r--   0 honnix     (501) staff       (20)    13302 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/azureblob.py
--rw-r--r--   0 honnix     (501) staff       (20)     7990 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/batch.py
--rw-r--r--   0 honnix     (501) staff       (20)    16573 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/beam_dataflow.py
--rw-r--r--   0 honnix     (501) staff       (20)    30816 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/bigquery.py
--rw-r--r--   0 honnix     (501) staff       (20)     4347 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/bigquery_avro.py
--rw-r--r--   0 honnix     (501) staff       (20)     5730 2018-12-19 13:45:13.000000 luigi-3.2.1/luigi/contrib/datadog_metric.py
--rw-r--r--   0 honnix     (501) staff       (20)    10231 2019-12-16 11:25:16.000000 luigi-3.2.1/luigi/contrib/dataproc.py
--rw-r--r--   0 honnix     (501) staff       (20)     8771 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/docker_runner.py
--rw-r--r--   0 honnix     (501) staff       (20)    11283 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/dropbox.py
--rw-r--r--   0 honnix     (501) staff       (20)     9599 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/ecs.py
--rw-r--r--   0 honnix     (501) staff       (20)    14188 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/esindex.py
--rw-r--r--   0 honnix     (501) staff       (20)     2330 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/external_daily_snapshot.py
--rw-r--r--   0 honnix     (501) staff       (20)    11285 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/external_program.py
--rw-r--r--   0 honnix     (501) staff       (20)    13354 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/ftp.py
--rw-r--r--   0 honnix     (501) staff       (20)     1498 2019-12-16 11:25:17.000000 luigi-3.2.1/luigi/contrib/gcp.py
--rw-r--r--   0 honnix     (501) staff       (20)    18537 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/gcs.py
--rw-r--r--   0 honnix     (501) staff       (20)    37546 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/hadoop.py
--rw-r--r--   0 honnix     (501) staff       (20)     5524 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/hadoop_jar.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.768375 luigi-3.2.1/luigi/contrib/hdfs/
--rw-r--r--   0 honnix     (501) staff       (20)     2901 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/__init__.py
--rw-r--r--   0 honnix     (501) staff       (20)     2839 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/abstract_client.py
--rw-r--r--   0 honnix     (501) staff       (20)     1922 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/clients.py
--rw-r--r--   0 honnix     (501) staff       (20)     4138 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/hdfs/config.py
--rw-r--r--   0 honnix     (501) staff       (20)     1120 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/error.py
--rw-r--r--   0 honnix     (501) staff       (20)     6019 2019-12-16 11:25:17.000000 luigi-3.2.1/luigi/contrib/hdfs/format.py
--rw-r--r--   0 honnix     (501) staff       (20)     9572 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/hadoopcli_clients.py
--rw-r--r--   0 honnix     (501) staff       (20)     7327 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/hdfs/target.py
--rw-r--r--   0 honnix     (501) staff       (20)     6721 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hdfs/webhdfs_client.py
--rw-r--r--   0 honnix     (501) staff       (20)    19494 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/hive.py
--rw-r--r--   0 honnix     (501) staff       (20)    14284 2020-12-16 13:26:58.000000 luigi-3.2.1/luigi/contrib/kubernetes.py
--rwxr-xr-x   0 honnix     (501) staff       (20)    12181 2019-12-27 14:24:38.000000 luigi-3.2.1/luigi/contrib/lsf.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     2297 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/lsf_runner.py
--rw-r--r--   0 honnix     (501) staff       (20)     6603 2019-12-27 14:24:38.000000 luigi-3.2.1/luigi/contrib/mongodb.py
--rw-r--r--   0 honnix     (501) staff       (20)     2806 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/mrrunner.py
--rw-r--r--   0 honnix     (501) staff       (20)     5475 2019-05-06 14:47:19.000000 luigi-3.2.1/luigi/contrib/mssqldb.py
--rw-r--r--   0 honnix     (501) staff       (20)     8613 2019-12-16 11:25:17.000000 luigi-3.2.1/luigi/contrib/mysqldb.py
--rw-r--r--   0 honnix     (501) staff       (20)     7286 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/opener.py
--rw-r--r--   0 honnix     (501) staff       (20)    11126 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/pai.py
--rw-r--r--   0 honnix     (501) staff       (20)     6517 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/pig.py
--rw-r--r--   0 honnix     (501) staff       (20)    16353 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/postgres.py
--rw-r--r--   0 honnix     (501) staff       (20)     7771 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/presto.py
--rw-r--r--   0 honnix     (501) staff       (20)     2430 2019-12-16 11:25:17.000000 luigi-3.2.1/luigi/contrib/prometheus_metric.py
--rw-r--r--   0 honnix     (501) staff       (20)     3897 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/pyspark_runner.py
--rw-r--r--   0 honnix     (501) staff       (20)    11181 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/rdbms.py
--rw-r--r--   0 honnix     (501) staff       (20)     3028 2019-12-16 11:25:17.000000 luigi-3.2.1/luigi/contrib/redis_store.py
--rw-r--r--   0 honnix     (501) staff       (20)    25778 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/redshift.py
--rw-r--r--   0 honnix     (501) staff       (20)    27902 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/s3.py
--rw-r--r--   0 honnix     (501) staff       (20)    27695 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/salesforce.py
--rw-r--r--   0 honnix     (501) staff       (20)    10682 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/scalding.py
--rwxr-xr-x   0 honnix     (501) staff       (20)    13563 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/sge.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     2830 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/sge_runner.py
--rw-r--r--   0 honnix     (501) staff       (20)     3354 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/simulate.py
--rw-r--r--   0 honnix     (501) staff       (20)    12313 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/spark.py
--rw-r--r--   0 honnix     (501) staff       (20)     1970 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/sparkey.py
--rw-r--r--   0 honnix     (501) staff       (20)    16375 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/contrib/sqla.py
--rw-r--r--   0 honnix     (501) staff       (20)    12356 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/contrib/ssh.py
--rw-r--r--   0 honnix     (501) staff       (20)     2811 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/target.py
--rw-r--r--   0 honnix     (501) staff       (20)     2974 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/contrib/webhdfs.py
--rw-r--r--   0 honnix     (501) staff       (20)     8620 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/date_interval.py
--rw-r--r--   0 honnix     (501) staff       (20)    11268 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/db_task_history.py
--rw-r--r--   0 honnix     (501) staff       (20)     1758 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/event.py
--rw-r--r--   0 honnix     (501) staff       (20)    20264 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/execution_summary.py
--rw-r--r--   0 honnix     (501) staff       (20)    14691 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/format.py
--rw-r--r--   0 honnix     (501) staff       (20)     2122 2023-01-17 11:14:47.000000 luigi-3.2.1/luigi/freezing.py
--rw-r--r--   0 honnix     (501) staff       (20)     8881 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/interface.py
--rw-r--r--   0 honnix     (501) staff       (20)     6182 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/local_target.py
--rw-r--r--   0 honnix     (501) staff       (20)     5410 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/lock.py
--rw-r--r--   0 honnix     (501) staff       (20)     2516 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/metrics.py
--rw-r--r--   0 honnix     (501) staff       (20)     5663 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/mock.py
--rw-r--r--   0 honnix     (501) staff       (20)    14535 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/notifications.py
--rw-r--r--   0 honnix     (501) staff       (20)    53828 2023-03-13 12:10:47.000000 luigi-3.2.1/luigi/parameter.py
--rw-r--r--   0 honnix     (501) staff       (20)     3489 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/process.py
--rw-r--r--   0 honnix     (501) staff       (20)     4658 2020-01-28 21:51:00.000000 luigi-3.2.1/luigi/retcodes.py
--rw-r--r--   0 honnix     (501) staff       (20)     6907 2023-03-13 12:10:47.000000 luigi-3.2.1/luigi/rpc.py
--rw-r--r--   0 honnix     (501) staff       (20)    65995 2023-01-16 12:34:07.000000 luigi-3.2.1/luigi/scheduler.py
--rw-r--r--   0 honnix     (501) staff       (20)    14294 2023-03-13 12:10:43.000000 luigi-3.2.1/luigi/server.py
--rw-r--r--   0 honnix     (501) staff       (20)     5819 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/setup_logging.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.286430 luigi-3.2.1/luigi/static/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.782871 luigi-3.2.1/luigi/static/visualiser/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.788862 luigi-3.2.1/luigi/static/visualiser/css/
--rw-r--r--   0 honnix     (501) staff       (20)    23739 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/css/font-awesome.min.css
--rw-r--r--   0 honnix     (501) staff       (20)     3413 2020-06-01 12:15:59.000000 luigi-3.2.1/luigi/static/visualiser/css/luigi.css
--rw-r--r--   0 honnix     (501) staff       (20)     2162 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/css/tipsy.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.814316 luigi-3.2.1/luigi/static/visualiser/fonts/
--rw-r--r--   0 honnix     (501) staff       (20)    93888 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/FontAwesome.otf
--rwxr-xr-x   0 honnix     (501) staff       (20)    60767 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.eot
--rw-r--r--   0 honnix     (501) staff       (20)   313398 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.svg
--rwxr-xr-x   0 honnix     (501) staff       (20)   122092 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.ttf
--rwxr-xr-x   0 honnix     (501) staff       (20)    71508 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff
--rw-r--r--   0 honnix     (501) staff       (20)    56780 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 honnix     (501) staff       (20)    20335 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 honnix     (501) staff       (20)    62927 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 honnix     (501) staff       (20)    41280 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 honnix     (501) staff       (20)    23320 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 honnix     (501) staff       (20)    33256 2023-03-14 09:02:28.000000 luigi-3.2.1/luigi/static/visualiser/index.html
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.832363 luigi-3.2.1/luigi/static/visualiser/js/
--rw-r--r--   0 honnix     (501) staff       (20)    12091 2023-03-14 09:02:28.000000 luigi-3.2.1/luigi/static/visualiser/js/graph.js
--rw-r--r--   0 honnix     (501) staff       (20)     8076 2019-08-26 08:30:29.000000 luigi-3.2.1/luigi/static/visualiser/js/luigi.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.834657 luigi-3.2.1/luigi/static/visualiser/js/test/
--rw-r--r--   0 honnix     (501) staff       (20)     3619 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/static/visualiser/js/test/graph_test.js
--rw-r--r--   0 honnix     (501) staff       (20)    11097 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/js/tipsy.js
--rw-r--r--   0 honnix     (501) staff       (20)      189 2023-03-14 09:02:28.000000 luigi-3.2.1/luigi/static/visualiser/js/util.js
--rw-r--r--   0 honnix     (501) staff       (20)    58572 2023-03-14 09:02:28.000000 luigi-3.2.1/luigi/static/visualiser/js/visualiserApp.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.862678 luigi-3.2.1/luigi/static/visualiser/lib/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.289061 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.870920 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/
--rw-r--r--   0 honnix     (501) staff       (20)    75652 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css
--rw-r--r--   0 honnix     (501) staff       (20)     3800 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css
--rw-r--r--   0 honnix     (501) staff       (20)     3033 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.876197 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/js/
--rw-r--r--   0 honnix     (501) staff       (20)     9420 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/js/app.min.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.289615 luigi-3.2.1/luigi/static/visualiser/lib/URI/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.883417 luigi-3.2.1/luigi/static/visualiser/lib/URI/1.18.2/
--rw-r--r--   0 honnix     (501) staff       (20)    62788 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/URI/1.18.2/URI.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.290763 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.886311 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/css/
--rwxr-xr-x   0 honnix     (501) staff       (20)     1590 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.891013 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/js/
--rwxr-xr-x   0 honnix     (501) staff       (20)     4129 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.291678 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.896174 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/css/
--rw-r--r--   0 honnix     (501) staff       (20)    19970 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css
--rw-r--r--   0 honnix     (501) staff       (20)   117308 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.905484 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/js/
--rw-r--r--   0 honnix     (501) staff       (20)    35951 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.948747 luigi-3.2.1/luigi/static/visualiser/lib/d3/
--rw-r--r--   0 honnix     (501) staff       (20)   151143 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/d3/d3.min.js
--rw-r--r--   0 honnix     (501) staff       (20)   113027 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/d3/dagre-d3.min.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.293419 luigi-3.2.1/luigi/static/visualiser/lib/datatables/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.952095 luigi-3.2.1/luigi/static/visualiser/lib/datatables/css/
--rw-r--r--   0 honnix     (501) staff       (20)    15353 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.961394 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/
--rw-r--r--   0 honnix     (501) staff       (20)    27490 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd
--rw-r--r--   0 honnix     (501) staff       (20)      894 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/favicon.ico
--rw-r--r--   0 honnix     (501) staff       (20)      160 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/sort_asc.png
--rw-r--r--   0 honnix     (501) staff       (20)      148 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 honnix     (501) staff       (20)      201 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/sort_both.png
--rw-r--r--   0 honnix     (501) staff       (20)      158 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/sort_desc.png
--rw-r--r--   0 honnix     (501) staff       (20)      146 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/sort_desc_disabled.png
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.983185 luigi-3.2.1/luigi/static/visualiser/lib/datatables/js/
--rw-r--r--   0 honnix     (501) staff       (20)    79457 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js
--rw-r--r--   0 honnix     (501) staff       (20)    93026 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-1.10.0.min.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.294932 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.985891 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.001108 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/
--rwxr-xr-x   0 honnix     (501) staff       (20)     1738 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif
--rwxr-xr-x   0 honnix     (501) staff       (20)      212 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      208 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_75_ffffff_40x100.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      335 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_55_fbf9ee_1x400.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      207 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_65_ffffff_1x400.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      262 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_dadada_1x400.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      262 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_e6e6e6_1x400.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      332 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_95_fef1ec_1x400.png
--rwxr-xr-x   0 honnix     (501) staff       (20)      280 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rwxr-xr-x   0 honnix     (501) staff       (20)     4970 2018-10-31 12:14:57.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png
--rwxr-xr-x   0 honnix     (501) staff       (20)     4510 2018-10-31 12:14:57.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png
--rwxr-xr-x   0 honnix     (501) staff       (20)     4974 2018-10-31 12:14:57.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png
--rwxr-xr-x   0 honnix     (501) staff       (20)     4979 2018-10-31 12:14:57.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png
--rwxr-xr-x   0 honnix     (501) staff       (20)     4510 2018-10-31 12:14:57.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png
--rwxr-xr-x   0 honnix     (501) staff       (20)    17063 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.012429 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/js/
--rwxr-xr-x   0 honnix     (501) staff       (20)    38439 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js
--rw-r--r--   0 honnix     (501) staff       (20)     4650 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/jquery.slimscroll.min.js
--rw-r--r--   0 honnix     (501) staff       (20)    14853 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/lib/mustache.js
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.016494 luigi-3.2.1/luigi/static/visualiser/mockdata/
--rw-r--r--   0 honnix     (501) staff       (20)     1097 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/mockdata/dep_graph
--rw-r--r--   0 honnix     (501) staff       (20)      400 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/mockdata/fetch_error
--rw-r--r--   0 honnix     (501) staff       (20)     1097 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/mockdata/task_list
--rw-r--r--   0 honnix     (501) staff       (20)      510 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/static/visualiser/test.html
--rw-r--r--   0 honnix     (501) staff       (20)    12207 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/target.py
--rw-r--r--   0 honnix     (501) staff       (20)    36073 2023-03-13 12:10:47.000000 luigi-3.2.1/luigi/task.py
--rw-r--r--   0 honnix     (501) staff       (20)     1991 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/task_history.py
--rw-r--r--   0 honnix     (501) staff       (20)     7999 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/task_register.py
--rw-r--r--   0 honnix     (501) staff       (20)      892 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/task_status.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.027561 luigi-3.2.1/luigi/templates/
--rwxr-xr-x   0 honnix     (501) staff       (20)     4270 2019-06-14 12:14:36.000000 luigi-3.2.1/luigi/templates/history.html
--rwxr-xr-x   0 honnix     (501) staff       (20)     3033 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/templates/layout.html
--rwxr-xr-x   0 honnix     (501) staff       (20)      553 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/templates/menu.html
--rw-r--r--   0 honnix     (501) staff       (20)      730 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/templates/recent.html
--rw-r--r--   0 honnix     (501) staff       (20)     1282 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/templates/show.html
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.038457 luigi-3.2.1/luigi/tools/
--rw-r--r--   0 honnix     (501) staff       (20)      751 2018-03-13 15:21:03.000000 luigi-3.2.1/luigi/tools/__init__.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     4753 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/tools/deps.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     2566 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/tools/deps_tree.py
--rwxr-xr-x   0 honnix     (501) staff       (20)     2808 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/tools/luigi_grep.py
--rwxr-xr-x   0 honnix     (501) staff       (20)    33931 2020-06-01 20:15:53.000000 luigi-3.2.1/luigi/tools/range.py
--rw-r--r--   0 honnix     (501) staff       (20)    16503 2022-06-09 13:02:03.000000 luigi-3.2.1/luigi/util.py
--rw-r--r--   0 honnix     (501) staff       (20)    52738 2023-01-16 12:13:44.000000 luigi-3.2.1/luigi/worker.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:31.446071 luigi-3.2.1/luigi.egg-info/
--rw-r--r--   0 honnix     (501) staff       (20)    13833 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/PKG-INFO
--rw-r--r--   0 honnix     (501) staff       (20)     9111 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/SOURCES.txt
--rw-r--r--   0 honnix     (501) staff       (20)        1 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/dependency_links.txt
--rw-r--r--   0 honnix     (501) staff       (20)      201 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/entry_points.txt
--rw-r--r--   0 honnix     (501) staff       (20)      158 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/requires.txt
--rw-r--r--   0 honnix     (501) staff       (20)        6 2023-03-14 09:46:31.000000 luigi-3.2.1/luigi.egg-info/top_level.txt
--rw-r--r--   0 honnix     (501) staff       (20)       38 2023-03-14 09:46:32.257830 luigi-3.2.1/setup.cfg
--rw-r--r--   0 honnix     (501) staff       (20)     4198 2023-01-17 11:14:47.000000 luigi-3.2.1/setup.py
-drwxr-xr-x   0 honnix     (501) staff       (20)        0 2023-03-14 09:46:32.256925 luigi-3.2.1/test/
--rw-r--r--   0 honnix     (501) staff       (20)     1732 2019-12-16 11:25:17.000000 luigi-3.2.1/test/_mysqldb_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7317 2020-06-01 20:15:53.000000 luigi-3.2.1/test/_test_ftp.py
--rw-r--r--   0 honnix     (501) staff       (20)    21729 2020-06-01 20:15:53.000000 luigi-3.2.1/test/batch_notifier_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2250 2019-12-16 11:25:17.000000 luigi-3.2.1/test/choice_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2286 2019-12-16 11:25:17.000000 luigi-3.2.1/test/clone_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    14333 2020-06-01 20:15:53.000000 luigi-3.2.1/test/cmdline_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3496 2022-06-09 13:02:03.000000 luigi-3.2.1/test/config_env_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3012 2019-12-16 11:25:17.000000 luigi-3.2.1/test/config_toml_test.py
--rw-r--r--   0 honnix     (501) staff       (20)        0 2022-06-09 13:02:03.000000 luigi-3.2.1/test/conftest.py
--rw-r--r--   0 honnix     (501) staff       (20)     3996 2022-06-09 13:02:03.000000 luigi-3.2.1/test/customized_run_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5623 2019-12-16 11:25:17.000000 luigi-3.2.1/test/date_interval_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7052 2020-06-01 20:15:53.000000 luigi-3.2.1/test/date_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     6002 2022-06-09 13:02:03.000000 luigi-3.2.1/test/db_task_history_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    10659 2022-06-09 13:02:03.000000 luigi-3.2.1/test/decorator_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5510 2023-03-13 12:10:47.000000 luigi-3.2.1/test/dict_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1179 2019-12-16 11:25:17.000000 luigi-3.2.1/test/dynamic_import_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     9651 2022-06-09 13:02:03.000000 luigi-3.2.1/test/event_callbacks_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    38687 2019-12-27 14:24:38.000000 luigi-3.2.1/test/execution_summary_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1449 2019-12-16 11:25:17.000000 luigi-3.2.1/test/factorial_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2262 2019-12-16 11:25:17.000000 luigi-3.2.1/test/fib_test.py
--rw-r--r--   0 honnix     (501) staff       (20)      858 2018-03-13 15:21:03.000000 luigi-3.2.1/test/hdfs_client_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7619 2022-06-09 13:02:03.000000 luigi-3.2.1/test/helpers.py
--rw-r--r--   0 honnix     (501) staff       (20)     1686 2018-03-13 15:21:03.000000 luigi-3.2.1/test/helpers_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2249 2018-03-13 15:21:03.000000 luigi-3.2.1/test/import_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2677 2022-06-09 13:02:03.000000 luigi-3.2.1/test/instance_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3012 2019-12-16 11:25:17.000000 luigi-3.2.1/test/instance_wrap_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     8909 2019-12-27 14:24:38.000000 luigi-3.2.1/test/interface_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4547 2023-03-13 12:10:47.000000 luigi-3.2.1/test/list_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    11446 2022-06-09 13:02:03.000000 luigi-3.2.1/test/local_target_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5704 2023-01-16 12:13:44.000000 luigi-3.2.1/test/lock_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1323 2019-12-27 14:24:38.000000 luigi-3.2.1/test/metrics_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3312 2020-06-01 20:15:53.000000 luigi-3.2.1/test/mock_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1082 2019-12-16 11:25:17.000000 luigi-3.2.1/test/most_common_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    15673 2022-06-09 13:02:03.000000 luigi-3.2.1/test/notifications_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4528 2019-12-16 11:25:17.000000 luigi-3.2.1/test/numerical_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7194 2022-06-09 13:02:03.000000 luigi-3.2.1/test/optional_parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)      836 2018-03-13 15:21:03.000000 luigi-3.2.1/test/other_module.py
--rw-r--r--   0 honnix     (501) staff       (20)    50865 2023-01-17 11:14:47.000000 luigi-3.2.1/test/parameter_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1592 2019-12-16 11:25:17.000000 luigi-3.2.1/test/priority_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    65249 2023-03-13 12:10:47.000000 luigi-3.2.1/test/range_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1547 2020-06-01 20:15:53.000000 luigi-3.2.1/test/recursion_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1430 2018-03-13 15:21:03.000000 luigi-3.2.1/test/remote_scheduler_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     6722 2020-06-01 20:15:53.000000 luigi-3.2.1/test/retcodes_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7810 2023-03-13 12:10:47.000000 luigi-3.2.1/test/rpc_test.py
--rw-r--r--   0 honnix     (501) staff       (20)      946 2022-06-09 13:02:03.000000 luigi-3.2.1/test/runtests.py
--rw-r--r--   0 honnix     (501) staff       (20)   108568 2022-06-09 13:02:03.000000 luigi-3.2.1/test/scheduler_api_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3833 2019-12-16 11:25:17.000000 luigi-3.2.1/test/scheduler_message_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5046 2019-12-16 11:25:17.000000 luigi-3.2.1/test/scheduler_parameter_visibilities_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    15901 2022-06-09 13:02:03.000000 luigi-3.2.1/test/scheduler_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    19929 2020-06-01 20:15:53.000000 luigi-3.2.1/test/scheduler_visualisation_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    19988 2022-06-09 13:02:03.000000 luigi-3.2.1/test/server_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1218 2019-12-16 11:25:17.000000 luigi-3.2.1/test/set_task_name_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5184 2019-12-16 11:25:17.000000 luigi-3.2.1/test/setup_logging_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2971 2019-12-27 14:24:38.000000 luigi-3.2.1/test/simulate_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1450 2020-06-01 20:15:53.000000 luigi-3.2.1/test/subtask_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    11128 2022-06-09 13:02:03.000000 luigi-3.2.1/test/target_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2361 2019-12-27 14:24:38.000000 luigi-3.2.1/test/task_bulk_complete_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3033 2023-01-16 12:13:44.000000 luigi-3.2.1/test/task_forwarded_attributes_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1687 2019-12-16 11:25:17.000000 luigi-3.2.1/test/task_history_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1166 2019-12-16 11:25:17.000000 luigi-3.2.1/test/task_progress_percentage_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1847 2019-12-16 11:25:17.000000 luigi-3.2.1/test/task_register_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4482 2022-06-09 13:02:03.000000 luigi-3.2.1/test/task_running_resources_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4092 2022-06-09 13:02:03.000000 luigi-3.2.1/test/task_serialize_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     1223 2019-12-16 11:25:17.000000 luigi-3.2.1/test/task_status_message_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    18409 2023-03-13 12:10:47.000000 luigi-3.2.1/test/task_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2848 2019-12-16 11:25:17.000000 luigi-3.2.1/test/test_sigpipe.py
--rw-r--r--   0 honnix     (501) staff       (20)     1796 2019-12-16 11:25:17.000000 luigi-3.2.1/test/test_ssh.py
--rw-r--r--   0 honnix     (501) staff       (20)     6500 2019-12-16 11:25:17.000000 luigi-3.2.1/test/util_previous_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     7333 2022-06-09 13:02:03.000000 luigi-3.2.1/test/util_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     3499 2019-12-16 11:25:17.000000 luigi-3.2.1/test/visible_parameters_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     6664 2020-09-23 11:52:17.000000 luigi-3.2.1/test/worker_external_task_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4240 2020-06-01 20:15:53.000000 luigi-3.2.1/test/worker_keep_alive_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     4005 2019-12-16 11:25:17.000000 luigi-3.2.1/test/worker_multiprocess_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     6351 2019-12-16 11:25:17.000000 luigi-3.2.1/test/worker_parallel_scheduling_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     6895 2020-06-01 20:15:53.000000 luigi-3.2.1/test/worker_scheduler_com_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2797 2020-06-01 20:15:53.000000 luigi-3.2.1/test/worker_task_process_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     5127 2020-08-10 12:05:46.000000 luigi-3.2.1/test/worker_task_test.py
--rw-r--r--   0 honnix     (501) staff       (20)    76915 2023-01-16 12:13:44.000000 luigi-3.2.1/test/worker_test.py
--rw-r--r--   0 honnix     (501) staff       (20)     2878 2022-06-09 13:02:03.000000 luigi-3.2.1/test/wrap_test.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.905421 luigi-3.3.0/
+-rw-r--r--   0 sonjae     (501) staff       (20)    11345 2022-10-02 14:57:54.000000 luigi-3.3.0/LICENSE
+-rw-r--r--   0 sonjae     (501) staff       (20)      140 2022-10-02 14:57:54.000000 luigi-3.3.0/MANIFEST.in
+-rw-r--r--   0 sonjae     (501) staff       (20)    13833 2023-05-04 09:32:34.903183 luigi-3.3.0/PKG-INFO
+-rw-r--r--   0 sonjae     (501) staff       (20)    12747 2023-01-18 15:50:13.000000 luigi-3.3.0/README.rst
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.773275 luigi-3.3.0/examples/
+-rw-r--r--   0 sonjae     (501) staff       (20)      603 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/__init__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3746 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/dynamic_requirements.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3410 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/elasticsearch_index.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3319 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/execution_summary_example.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1462 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/foo.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1876 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/foo_complex.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3239 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/ftp_experiment_outputs.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      500 2023-01-18 15:50:07.000000 luigi-3.3.0/examples/hello_world.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1986 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/kubernetes.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5264 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/per_task_retry_policy.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3388 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/pyspark_wc.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4363 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/spark_als.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2823 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/ssh_remote_execution.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3400 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/terasort.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     9069 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/top_artists.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      645 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/top_artists_spark.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2904 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/wordcount.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2729 2022-10-02 14:57:54.000000 luigi-3.3.0/examples/wordcount_hadoop.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.902811 luigi-3.3.0/luigi/
+-rw-r--r--   0 sonjae     (501) staff       (20)     3723 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/__init__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      683 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/__main__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      249 2023-05-04 09:31:56.000000 luigi-3.3.0/luigi/__meta__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8863 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/batch_notifier.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1426 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/cmdline.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5458 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/cmdline_parser.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.928547 luigi-3.3.0/luigi/configuration/
+-rw-r--r--   0 sonjae     (501) staff       (20)      837 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/configuration/__init__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1307 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/configuration/base_parser.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8402 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/configuration/cfg_parser.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2760 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/configuration/core.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2831 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/configuration/toml_parser.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.156844 luigi-3.3.0/luigi/contrib/
+-rw-r--r--   0 sonjae     (501) staff       (20)      661 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/__init__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    13302 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/azureblob.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7990 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/batch.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    16573 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/beam_dataflow.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    30813 2023-05-04 09:31:56.000000 luigi-3.3.0/luigi/contrib/bigquery.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4347 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/bigquery_avro.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5730 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/datadog_metric.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    10231 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/dataproc.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     9524 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/contrib/docker_runner.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11283 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/dropbox.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     9599 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/ecs.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14188 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/esindex.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2330 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/external_daily_snapshot.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11285 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/external_program.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    13354 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/ftp.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1498 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/gcp.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    18537 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/gcs.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    37546 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/contrib/hadoop.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5524 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hadoop_jar.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.195409 luigi-3.3.0/luigi/contrib/hdfs/
+-rw-r--r--   0 sonjae     (501) staff       (20)     2901 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/__init__.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2839 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/abstract_client.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1922 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/clients.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4138 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/config.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1120 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/error.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6019 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/format.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     9572 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/hadoopcli_clients.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7327 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/target.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6721 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hdfs/webhdfs_client.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    19494 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/hive.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14284 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/kubernetes.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    12181 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/lsf.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     2297 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/lsf_runner.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6603 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/mongodb.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2806 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/mrrunner.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5475 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/mssqldb.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8613 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/mysqldb.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7286 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/opener.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11126 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/pai.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6517 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/pig.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    16353 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/postgres.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7771 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/presto.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2430 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/prometheus_metric.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3897 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/pyspark_runner.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11181 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/rdbms.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3028 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/redis_store.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    25778 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/redshift.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    27902 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/contrib/s3.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    27695 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/salesforce.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    10682 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/scalding.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    13563 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/sge.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     2830 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/sge_runner.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3354 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/contrib/simulate.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    12313 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/spark.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1970 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/sparkey.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    16375 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/sqla.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    12356 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/ssh.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2811 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/target.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2974 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/contrib/webhdfs.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8620 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/date_interval.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11268 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/db_task_history.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1758 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/event.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    20264 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/execution_summary.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14691 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/format.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2122 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/freezing.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8881 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/interface.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6182 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/local_target.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5410 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/lock.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2516 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/metrics.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5663 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/mock.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14535 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/notifications.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    53828 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/parameter.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3489 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/process.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4658 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/retcodes.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6907 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/rpc.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    65995 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/scheduler.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14294 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/server.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5889 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/setup_logging.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.673295 luigi-3.3.0/luigi/static/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.215889 luigi-3.3.0/luigi/static/visualiser/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.226056 luigi-3.3.0/luigi/static/visualiser/css/
+-rw-r--r--   0 sonjae     (501) staff       (20)    23739 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/css/font-awesome.min.css
+-rw-r--r--   0 sonjae     (501) staff       (20)     3413 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/css/luigi.css
+-rw-r--r--   0 sonjae     (501) staff       (20)     2162 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/css/tipsy.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.255568 luigi-3.3.0/luigi/static/visualiser/fonts/
+-rw-r--r--   0 sonjae     (501) staff       (20)    93888 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/FontAwesome.otf
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    60767 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 sonjae     (501) staff       (20)   313398 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.svg
+-rwxr-xr-x   0 sonjae     (501) staff       (20)   122092 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.ttf
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    71508 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 sonjae     (501) staff       (20)    56780 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 sonjae     (501) staff       (20)    20335 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 sonjae     (501) staff       (20)    62927 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 sonjae     (501) staff       (20)    41280 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 sonjae     (501) staff       (20)    23320 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 sonjae     (501) staff       (20)    33256 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/static/visualiser/index.html
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.283683 luigi-3.3.0/luigi/static/visualiser/js/
+-rw-r--r--   0 sonjae     (501) staff       (20)    12091 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/static/visualiser/js/graph.js
+-rw-r--r--   0 sonjae     (501) staff       (20)     8076 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/js/luigi.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.291198 luigi-3.3.0/luigi/static/visualiser/js/test/
+-rw-r--r--   0 sonjae     (501) staff       (20)     3619 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/js/test/graph_test.js
+-rw-r--r--   0 sonjae     (501) staff       (20)    11097 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/js/tipsy.js
+-rw-r--r--   0 sonjae     (501) staff       (20)      189 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/static/visualiser/js/util.js
+-rw-r--r--   0 sonjae     (501) staff       (20)    58572 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/static/visualiser/js/visualiserApp.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.326063 luigi-3.3.0/luigi/static/visualiser/lib/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.676344 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.340504 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/
+-rw-r--r--   0 sonjae     (501) staff       (20)    75652 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css
+-rw-r--r--   0 sonjae     (501) staff       (20)     3800 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css
+-rw-r--r--   0 sonjae     (501) staff       (20)     3033 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.347063 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/js/
+-rw-r--r--   0 sonjae     (501) staff       (20)     9420 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/js/app.min.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.677604 luigi-3.3.0/luigi/static/visualiser/lib/URI/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.356950 luigi-3.3.0/luigi/static/visualiser/lib/URI/1.18.2/
+-rw-r--r--   0 sonjae     (501) staff       (20)    62788 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/URI/1.18.2/URI.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.678990 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.360014 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/css/
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     1590 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.365013 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/js/
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4129 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.680101 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.373063 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/css/
+-rw-r--r--   0 sonjae     (501) staff       (20)    19970 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css
+-rw-r--r--   0 sonjae     (501) staff       (20)   117308 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.382846 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/js/
+-rw-r--r--   0 sonjae     (501) staff       (20)    35951 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.431853 luigi-3.3.0/luigi/static/visualiser/lib/d3/
+-rw-r--r--   0 sonjae     (501) staff       (20)   151143 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/d3/d3.min.js
+-rw-r--r--   0 sonjae     (501) staff       (20)   113027 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/d3/dagre-d3.min.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.681597 luigi-3.3.0/luigi/static/visualiser/lib/datatables/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.436695 luigi-3.3.0/luigi/static/visualiser/lib/datatables/css/
+-rw-r--r--   0 sonjae     (501) staff       (20)    15353 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.448496 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/
+-rw-r--r--   0 sonjae     (501) staff       (20)    27490 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd
+-rw-r--r--   0 sonjae     (501) staff       (20)      894 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/favicon.ico
+-rw-r--r--   0 sonjae     (501) staff       (20)      160 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/sort_asc.png
+-rw-r--r--   0 sonjae     (501) staff       (20)      148 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 sonjae     (501) staff       (20)      201 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/sort_both.png
+-rw-r--r--   0 sonjae     (501) staff       (20)      158 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/sort_desc.png
+-rw-r--r--   0 sonjae     (501) staff       (20)      146 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/sort_desc_disabled.png
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.473243 luigi-3.3.0/luigi/static/visualiser/lib/datatables/js/
+-rw-r--r--   0 sonjae     (501) staff       (20)    79457 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js
+-rw-r--r--   0 sonjae     (501) staff       (20)    93026 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-1.10.0.min.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.682844 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.479540 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.496536 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     1738 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      212 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      208 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      335 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      207 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      262 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_dadada_1x400.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      262 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      332 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_95_fef1ec_1x400.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      280 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4970 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4510 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4974 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4979 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4510 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    17063 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.507277 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/js/
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    38439 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js
+-rw-r--r--   0 sonjae     (501) staff       (20)     4650 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/jquery.slimscroll.min.js
+-rw-r--r--   0 sonjae     (501) staff       (20)    14853 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/lib/mustache.js
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.514042 luigi-3.3.0/luigi/static/visualiser/mockdata/
+-rw-r--r--   0 sonjae     (501) staff       (20)     1097 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/mockdata/dep_graph
+-rw-r--r--   0 sonjae     (501) staff       (20)      400 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/mockdata/fetch_error
+-rw-r--r--   0 sonjae     (501) staff       (20)     1097 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/mockdata/task_list
+-rw-r--r--   0 sonjae     (501) staff       (20)      510 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/static/visualiser/test.html
+-rw-r--r--   0 sonjae     (501) staff       (20)    12207 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/target.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    36073 2023-05-03 09:14:45.000000 luigi-3.3.0/luigi/task.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1991 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/task_history.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7999 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/task_register.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      892 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/task_status.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.529826 luigi-3.3.0/luigi/templates/
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4270 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/templates/history.html
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     3033 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/templates/layout.html
+-rwxr-xr-x   0 sonjae     (501) staff       (20)      553 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/templates/menu.html
+-rw-r--r--   0 sonjae     (501) staff       (20)      730 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/templates/recent.html
+-rw-r--r--   0 sonjae     (501) staff       (20)     1282 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/templates/show.html
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.548043 luigi-3.3.0/luigi/tools/
+-rw-r--r--   0 sonjae     (501) staff       (20)      751 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/tools/__init__.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     4753 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/tools/deps.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     2566 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/tools/deps_tree.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)     2808 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/tools/luigi_grep.py
+-rwxr-xr-x   0 sonjae     (501) staff       (20)    33931 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/tools/range.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    16503 2022-10-02 14:57:54.000000 luigi-3.3.0/luigi/util.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    52738 2023-01-18 15:50:13.000000 luigi-3.3.0/luigi/worker.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:33.907737 luigi-3.3.0/luigi.egg-info/
+-rw-r--r--   0 sonjae     (501) staff       (20)    13833 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/PKG-INFO
+-rw-r--r--   0 sonjae     (501) staff       (20)     9111 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/SOURCES.txt
+-rw-r--r--   0 sonjae     (501) staff       (20)        1 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/dependency_links.txt
+-rw-r--r--   0 sonjae     (501) staff       (20)      201 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/entry_points.txt
+-rw-r--r--   0 sonjae     (501) staff       (20)      158 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/requires.txt
+-rw-r--r--   0 sonjae     (501) staff       (20)        6 2023-05-04 09:32:33.000000 luigi-3.3.0/luigi.egg-info/top_level.txt
+-rw-r--r--   0 sonjae     (501) staff       (20)       38 2023-05-04 09:32:34.906257 luigi-3.3.0/setup.cfg
+-rw-r--r--   0 sonjae     (501) staff       (20)     4198 2023-01-18 15:50:13.000000 luigi-3.3.0/setup.py
+drwxr-xr-x   0 sonjae     (501) staff       (20)        0 2023-05-04 09:32:34.902294 luigi-3.3.0/test/
+-rw-r--r--   0 sonjae     (501) staff       (20)     1732 2023-05-03 12:50:04.000000 luigi-3.3.0/test/_mysqldb_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7317 2023-05-03 12:50:04.000000 luigi-3.3.0/test/_test_ftp.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    21729 2023-05-03 12:50:04.000000 luigi-3.3.0/test/batch_notifier_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2250 2023-05-03 12:50:04.000000 luigi-3.3.0/test/choice_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2286 2023-05-03 12:50:04.000000 luigi-3.3.0/test/clone_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    14333 2023-05-03 12:50:04.000000 luigi-3.3.0/test/cmdline_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3496 2023-05-03 12:50:04.000000 luigi-3.3.0/test/config_env_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3012 2023-05-03 12:50:04.000000 luigi-3.3.0/test/config_toml_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)        0 2023-05-03 12:50:04.000000 luigi-3.3.0/test/conftest.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3996 2023-05-03 12:50:04.000000 luigi-3.3.0/test/customized_run_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5623 2023-05-03 12:50:04.000000 luigi-3.3.0/test/date_interval_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7052 2023-05-03 12:50:04.000000 luigi-3.3.0/test/date_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6002 2023-05-03 12:50:04.000000 luigi-3.3.0/test/db_task_history_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    10659 2023-05-03 12:50:04.000000 luigi-3.3.0/test/decorator_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5510 2023-05-03 12:50:04.000000 luigi-3.3.0/test/dict_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1179 2023-05-03 12:50:04.000000 luigi-3.3.0/test/dynamic_import_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     9651 2023-05-03 12:50:04.000000 luigi-3.3.0/test/event_callbacks_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    38687 2023-05-03 12:50:04.000000 luigi-3.3.0/test/execution_summary_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1449 2023-05-03 12:50:04.000000 luigi-3.3.0/test/factorial_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2262 2023-05-03 12:50:04.000000 luigi-3.3.0/test/fib_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      858 2023-05-03 12:50:04.000000 luigi-3.3.0/test/hdfs_client_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7619 2023-05-03 12:50:04.000000 luigi-3.3.0/test/helpers.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1686 2023-05-03 12:50:04.000000 luigi-3.3.0/test/helpers_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2249 2023-05-03 12:50:04.000000 luigi-3.3.0/test/import_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2677 2023-05-03 12:50:04.000000 luigi-3.3.0/test/instance_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3012 2023-05-03 12:50:04.000000 luigi-3.3.0/test/instance_wrap_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     8909 2023-05-03 12:50:04.000000 luigi-3.3.0/test/interface_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4547 2023-05-03 12:50:04.000000 luigi-3.3.0/test/list_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11446 2023-05-03 12:50:04.000000 luigi-3.3.0/test/local_target_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5704 2023-05-03 12:50:04.000000 luigi-3.3.0/test/lock_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1323 2023-05-03 12:50:04.000000 luigi-3.3.0/test/metrics_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3312 2023-05-03 12:50:04.000000 luigi-3.3.0/test/mock_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1082 2023-05-03 12:50:04.000000 luigi-3.3.0/test/most_common_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    15673 2023-05-03 12:50:04.000000 luigi-3.3.0/test/notifications_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4528 2023-05-03 12:50:04.000000 luigi-3.3.0/test/numerical_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7194 2023-05-03 12:50:04.000000 luigi-3.3.0/test/optional_parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      836 2023-05-03 12:50:04.000000 luigi-3.3.0/test/other_module.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    50865 2023-05-03 12:50:04.000000 luigi-3.3.0/test/parameter_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1592 2023-05-03 12:50:04.000000 luigi-3.3.0/test/priority_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    65249 2023-05-03 12:50:04.000000 luigi-3.3.0/test/range_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1547 2023-05-03 12:50:04.000000 luigi-3.3.0/test/recursion_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1430 2023-05-03 12:50:04.000000 luigi-3.3.0/test/remote_scheduler_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6722 2023-05-03 12:50:04.000000 luigi-3.3.0/test/retcodes_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7810 2023-05-03 12:50:04.000000 luigi-3.3.0/test/rpc_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)      946 2023-05-03 12:46:33.000000 luigi-3.3.0/test/runtests.py
+-rw-r--r--   0 sonjae     (501) staff       (20)   108568 2023-05-03 12:50:04.000000 luigi-3.3.0/test/scheduler_api_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3833 2023-05-03 12:50:04.000000 luigi-3.3.0/test/scheduler_message_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5046 2023-05-03 12:50:04.000000 luigi-3.3.0/test/scheduler_parameter_visibilities_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    15901 2023-05-03 12:50:04.000000 luigi-3.3.0/test/scheduler_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    19929 2023-05-03 12:50:04.000000 luigi-3.3.0/test/scheduler_visualisation_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    19988 2023-05-03 12:50:04.000000 luigi-3.3.0/test/server_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1218 2023-05-03 12:50:04.000000 luigi-3.3.0/test/set_task_name_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6226 2023-05-03 12:50:04.000000 luigi-3.3.0/test/setup_logging_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2971 2023-05-03 12:50:04.000000 luigi-3.3.0/test/simulate_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1450 2023-05-03 12:50:04.000000 luigi-3.3.0/test/subtask_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    11128 2023-05-03 12:50:04.000000 luigi-3.3.0/test/target_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2361 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_bulk_complete_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3033 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_forwarded_attributes_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1687 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_history_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1166 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_progress_percentage_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1847 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_register_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4482 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_running_resources_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4092 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_serialize_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1223 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_status_message_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    18409 2023-05-03 12:50:04.000000 luigi-3.3.0/test/task_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2848 2023-05-03 12:50:04.000000 luigi-3.3.0/test/test_sigpipe.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     1796 2023-05-03 12:50:04.000000 luigi-3.3.0/test/test_ssh.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6500 2023-05-03 12:50:04.000000 luigi-3.3.0/test/util_previous_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     7333 2023-05-03 12:50:04.000000 luigi-3.3.0/test/util_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     3499 2023-05-03 12:50:04.000000 luigi-3.3.0/test/visible_parameters_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6664 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_external_task_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4240 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_keep_alive_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     4005 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_multiprocess_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6351 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_parallel_scheduling_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     6895 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_scheduler_com_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2797 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_task_process_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     5127 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_task_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)    76915 2023-05-03 12:50:04.000000 luigi-3.3.0/test/worker_test.py
+-rw-r--r--   0 sonjae     (501) staff       (20)     2878 2023-05-03 12:50:04.000000 luigi-3.3.0/test/wrap_test.py
```

### Comparing `luigi-3.2.1/LICENSE` & `luigi-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/PKG-INFO` & `luigi-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi
-Version: 3.2.1
+Version: 3.3.0
 Summary: Workflow mgmgt + task scheduling + dependency resolution.
 Home-page: https://github.com/spotify/luigi
 Author: The Luigi Authors
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `luigi-3.2.1/README.rst` & `luigi-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/__init__.py` & `luigi-3.3.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/dynamic_requirements.py` & `luigi-3.3.0/examples/dynamic_requirements.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/elasticsearch_index.py` & `luigi-3.3.0/examples/elasticsearch_index.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/execution_summary_example.py` & `luigi-3.3.0/examples/execution_summary_example.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/foo.py` & `luigi-3.3.0/examples/foo.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/foo_complex.py` & `luigi-3.3.0/examples/foo_complex.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/ftp_experiment_outputs.py` & `luigi-3.3.0/examples/ftp_experiment_outputs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/kubernetes.py` & `luigi-3.3.0/examples/kubernetes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/per_task_retry_policy.py` & `luigi-3.3.0/examples/per_task_retry_policy.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/pyspark_wc.py` & `luigi-3.3.0/examples/pyspark_wc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/spark_als.py` & `luigi-3.3.0/examples/spark_als.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/ssh_remote_execution.py` & `luigi-3.3.0/examples/ssh_remote_execution.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/terasort.py` & `luigi-3.3.0/examples/terasort.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/top_artists.py` & `luigi-3.3.0/examples/top_artists.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/top_artists_spark.py` & `luigi-3.3.0/examples/top_artists_spark.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/wordcount.py` & `luigi-3.3.0/examples/wordcount.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/examples/wordcount_hadoop.py` & `luigi-3.3.0/examples/wordcount_hadoop.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/__init__.py` & `luigi-3.3.0/luigi/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/__main__.py` & `luigi-3.3.0/luigi/__main__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/batch_notifier.py` & `luigi-3.3.0/luigi/batch_notifier.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/cmdline.py` & `luigi-3.3.0/luigi/cmdline.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/cmdline_parser.py` & `luigi-3.3.0/luigi/cmdline_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/configuration/__init__.py` & `luigi-3.3.0/luigi/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/configuration/base_parser.py` & `luigi-3.3.0/luigi/configuration/base_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/configuration/cfg_parser.py` & `luigi-3.3.0/luigi/configuration/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/configuration/core.py` & `luigi-3.3.0/luigi/configuration/core.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/configuration/toml_parser.py` & `luigi-3.3.0/luigi/configuration/toml_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/__init__.py` & `luigi-3.3.0/luigi/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/azureblob.py` & `luigi-3.3.0/luigi/contrib/azureblob.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/batch.py` & `luigi-3.3.0/luigi/contrib/batch.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/beam_dataflow.py` & `luigi-3.3.0/luigi/contrib/beam_dataflow.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/bigquery.py` & `luigi-3.3.0/luigi/contrib/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     return isinstance(err, errors.HttpError) and err.resp.status >= 500
 
 
 bq_retry = retry(retry=(retry_if_exception(is_error_5xx) | retry_if_exception_type(RETRYABLE_ERRORS)),
                  wait=wait_exponential(multiplier=1, min=1, max=10),
                  stop=stop_after_attempt(3),
                  reraise=True,
-                 after=lambda x: x.args[0].__initialise_client()
+                 after=lambda x: x.args[0]._initialise_client()
                  )
 
 
 class CreateDisposition:
     CREATE_IF_NEEDED = 'CREATE_IF_NEEDED'
     CREATE_NEVER = 'CREATE_NEVER'
 
@@ -148,17 +148,17 @@
     def __init__(self, oauth_credentials=None, descriptor='', http_=None):
         # Save initialisation arguments in case we need to re-create client
         # due to connection timeout
         self.oauth_credentials = oauth_credentials
         self.descriptor = descriptor
         self.http_ = http_
 
-        self.__initialise_client()
+        self._initialise_client()
 
-    def __initialise_client(self):
+    def _initialise_client(self):
         authenticate_kwargs = gcp.get_authenticate_kwargs(self.oauth_credentials, self.http_)
 
         if self.descriptor:
             self.client = discovery.build_from_document(self.descriptor, **authenticate_kwargs)
         else:
             self.client = discovery.build('bigquery', 'v2', cache_discovery=False, **authenticate_kwargs)
```

### Comparing `luigi-3.2.1/luigi/contrib/bigquery_avro.py` & `luigi-3.3.0/luigi/contrib/bigquery_avro.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/datadog_metric.py` & `luigi-3.3.0/luigi/contrib/datadog_metric.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/dataproc.py` & `luigi-3.3.0/luigi/contrib/dataproc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/docker_runner.py` & `luigi-3.3.0/luigi/contrib/docker_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,31 @@
         return "echo hello world"
 
     @property
     def name(self):
         return None
 
     @property
+    def host_config_options(self):
+        '''
+        Override this to specify host_config options like gpu requests or shm
+        size e.g. `{"device_requests": [docker.types.DeviceRequest(count=1, capabilities=[["gpu"]])]}`
+
+        See https://docker-py.readthedocs.io/en/stable/api.html#docker.api.container.ContainerApiMixin.create_host_config
+        '''
+        return {}
+
+    @property
     def container_options(self):
+        '''
+        Override this to specify container options like user or ports e.g.
+        `{"user": f"{os.getuid()}:{os.getgid()}"}`
+
+        See https://docker-py.readthedocs.io/en/stable/api.html#docker.api.container.ContainerApiMixin.create_container
+        '''
         return {}
 
     @property
     def environment(self):
         return {}
 
     @property
@@ -188,15 +204,16 @@
 
         # run the container
         try:
             logger.debug('Creating image: %s command: %s volumes: %s'
                          % (self._image, self.command, self._binds))
 
             host_config = self._client.create_host_config(binds=self._binds,
-                                                          network_mode=self.network_mode)
+                                                          network_mode=self.network_mode,
+                                                          **self.host_config_options)
 
             container = self._client.create_container(self._image,
                                                       command=self.command,
                                                       name=self.name,
                                                       environment=self.environment,
                                                       volumes=self._volumes,
                                                       host_config=host_config,
```

### Comparing `luigi-3.2.1/luigi/contrib/dropbox.py` & `luigi-3.3.0/luigi/contrib/dropbox.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/ecs.py` & `luigi-3.3.0/luigi/contrib/ecs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/esindex.py` & `luigi-3.3.0/luigi/contrib/esindex.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/external_daily_snapshot.py` & `luigi-3.3.0/luigi/contrib/external_daily_snapshot.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/external_program.py` & `luigi-3.3.0/luigi/contrib/external_program.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/ftp.py` & `luigi-3.3.0/luigi/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/gcp.py` & `luigi-3.3.0/luigi/contrib/gcp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/gcs.py` & `luigi-3.3.0/luigi/contrib/gcs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hadoop.py` & `luigi-3.3.0/luigi/contrib/hadoop.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hadoop_jar.py` & `luigi-3.3.0/luigi/contrib/hadoop_jar.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/__init__.py` & `luigi-3.3.0/luigi/contrib/hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/abstract_client.py` & `luigi-3.3.0/luigi/contrib/hdfs/abstract_client.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/clients.py` & `luigi-3.3.0/luigi/contrib/hdfs/clients.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/config.py` & `luigi-3.3.0/luigi/contrib/hdfs/config.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/error.py` & `luigi-3.3.0/luigi/contrib/hdfs/error.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/format.py` & `luigi-3.3.0/luigi/contrib/hdfs/format.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/hadoopcli_clients.py` & `luigi-3.3.0/luigi/contrib/hdfs/hadoopcli_clients.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/target.py` & `luigi-3.3.0/luigi/contrib/hdfs/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hdfs/webhdfs_client.py` & `luigi-3.3.0/luigi/contrib/hdfs/webhdfs_client.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/hive.py` & `luigi-3.3.0/luigi/contrib/hive.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/kubernetes.py` & `luigi-3.3.0/luigi/contrib/kubernetes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/lsf.py` & `luigi-3.3.0/luigi/contrib/lsf.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/lsf_runner.py` & `luigi-3.3.0/luigi/contrib/lsf_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/mongodb.py` & `luigi-3.3.0/luigi/contrib/mongodb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/mrrunner.py` & `luigi-3.3.0/luigi/contrib/mrrunner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/mssqldb.py` & `luigi-3.3.0/luigi/contrib/mssqldb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/mysqldb.py` & `luigi-3.3.0/luigi/contrib/mysqldb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/opener.py` & `luigi-3.3.0/luigi/contrib/opener.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/pai.py` & `luigi-3.3.0/luigi/contrib/pai.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/pig.py` & `luigi-3.3.0/luigi/contrib/pig.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/postgres.py` & `luigi-3.3.0/luigi/contrib/postgres.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/presto.py` & `luigi-3.3.0/luigi/contrib/presto.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/prometheus_metric.py` & `luigi-3.3.0/luigi/contrib/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/pyspark_runner.py` & `luigi-3.3.0/luigi/contrib/pyspark_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/rdbms.py` & `luigi-3.3.0/luigi/contrib/rdbms.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/redis_store.py` & `luigi-3.3.0/luigi/contrib/redis_store.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/redshift.py` & `luigi-3.3.0/luigi/contrib/redshift.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/s3.py` & `luigi-3.3.0/luigi/contrib/s3.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/salesforce.py` & `luigi-3.3.0/luigi/contrib/salesforce.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/scalding.py` & `luigi-3.3.0/luigi/contrib/scalding.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/sge.py` & `luigi-3.3.0/luigi/contrib/sge.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/sge_runner.py` & `luigi-3.3.0/luigi/contrib/sge_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/simulate.py` & `luigi-3.3.0/luigi/contrib/simulate.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/spark.py` & `luigi-3.3.0/luigi/contrib/spark.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/sparkey.py` & `luigi-3.3.0/luigi/contrib/sparkey.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/sqla.py` & `luigi-3.3.0/luigi/contrib/sqla.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/ssh.py` & `luigi-3.3.0/luigi/contrib/ssh.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/target.py` & `luigi-3.3.0/luigi/contrib/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/contrib/webhdfs.py` & `luigi-3.3.0/luigi/contrib/webhdfs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/date_interval.py` & `luigi-3.3.0/luigi/date_interval.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/db_task_history.py` & `luigi-3.3.0/luigi/db_task_history.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/event.py` & `luigi-3.3.0/luigi/event.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/execution_summary.py` & `luigi-3.3.0/luigi/execution_summary.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/format.py` & `luigi-3.3.0/luigi/format.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/freezing.py` & `luigi-3.3.0/luigi/freezing.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/interface.py` & `luigi-3.3.0/luigi/interface.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/local_target.py` & `luigi-3.3.0/luigi/local_target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/lock.py` & `luigi-3.3.0/luigi/lock.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/metrics.py` & `luigi-3.3.0/luigi/metrics.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/mock.py` & `luigi-3.3.0/luigi/mock.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/notifications.py` & `luigi-3.3.0/luigi/notifications.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/parameter.py` & `luigi-3.3.0/luigi/parameter.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/process.py` & `luigi-3.3.0/luigi/process.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/retcodes.py` & `luigi-3.3.0/luigi/retcodes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/rpc.py` & `luigi-3.3.0/luigi/rpc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/scheduler.py` & `luigi-3.3.0/luigi/scheduler.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/server.py` & `luigi-3.3.0/luigi/server.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/setup_logging.py` & `luigi-3.3.0/luigi/setup_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 
 import logging
 import logging.config
 import os.path
 
 from luigi.configuration import get_config, LuigiConfigParser
+from luigi.freezing import recursively_unfreeze
 
 from configparser import NoSectionError
 
 
 class BaseLogging:
     config = get_config()
 
@@ -36,15 +37,15 @@
         """Get logging settings from config file section "logging"."""
         if isinstance(cls.config, LuigiConfigParser):
             return False
         try:
             logging_config = cls.config['logging']
         except (TypeError, KeyError, NoSectionError):
             return False
-        logging.config.dictConfig(logging_config)
+        logging.config.dictConfig(recursively_unfreeze(logging_config))
         return True
 
     @classmethod
     def setup(cls,
               opts=type('opts', (), {
                   'background': None,
                   'logdir': None,
```

### Comparing `luigi-3.2.1/luigi/static/visualiser/css/font-awesome.min.css` & `luigi-3.3.0/luigi/static/visualiser/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/css/luigi.css` & `luigi-3.3.0/luigi/static/visualiser/css/luigi.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/css/tipsy.css` & `luigi-3.3.0/luigi/static/visualiser/css/tipsy.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/FontAwesome.otf` & `luigi-3.3.0/luigi/static/visualiser/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.eot` & `luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.svg` & `luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.ttf` & `luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff` & `luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff2` & `luigi-3.3.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot` & `luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg` & `luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf` & `luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff` & `luigi-3.3.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/index.html` & `luigi-3.3.0/luigi/static/visualiser/index.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/js/graph.js` & `luigi-3.3.0/luigi/static/visualiser/js/graph.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/js/luigi.js` & `luigi-3.3.0/luigi/static/visualiser/js/luigi.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/js/test/graph_test.js` & `luigi-3.3.0/luigi/static/visualiser/js/test/graph_test.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/js/tipsy.js` & `luigi-3.3.0/luigi/static/visualiser/js/tipsy.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/js/visualiserApp.js` & `luigi-3.3.0/luigi/static/visualiser/js/visualiserApp.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/AdminLTE/js/app.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/AdminLTE/js/app.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/URI/1.18.2/URI.js` & `luigi-3.3.0/luigi/static/visualiser/lib/URI/1.18.2/URI.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/d3/d3.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/d3/dagre-d3.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd` & `luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/datatables/images/favicon.ico` & `luigi-3.3.0/luigi/static/visualiser/lib/datatables/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-1.10.0.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-1.10.0.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/jquery.slimscroll.min.js` & `luigi-3.3.0/luigi/static/visualiser/lib/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/lib/mustache.js` & `luigi-3.3.0/luigi/static/visualiser/lib/mustache.js`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/mockdata/dep_graph` & `luigi-3.3.0/luigi/static/visualiser/mockdata/dep_graph`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/static/visualiser/mockdata/task_list` & `luigi-3.3.0/luigi/static/visualiser/mockdata/task_list`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/target.py` & `luigi-3.3.0/luigi/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/task.py` & `luigi-3.3.0/luigi/task.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/task_history.py` & `luigi-3.3.0/luigi/task_history.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/task_register.py` & `luigi-3.3.0/luigi/task_register.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/task_status.py` & `luigi-3.3.0/luigi/task_status.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/templates/history.html` & `luigi-3.3.0/luigi/templates/history.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/templates/layout.html` & `luigi-3.3.0/luigi/templates/layout.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/templates/menu.html` & `luigi-3.3.0/luigi/templates/menu.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/templates/recent.html` & `luigi-3.3.0/luigi/templates/recent.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/templates/show.html` & `luigi-3.3.0/luigi/templates/show.html`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/tools/__init__.py` & `luigi-3.3.0/luigi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/tools/deps.py` & `luigi-3.3.0/luigi/tools/deps.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/tools/deps_tree.py` & `luigi-3.3.0/luigi/tools/deps_tree.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/tools/luigi_grep.py` & `luigi-3.3.0/luigi/tools/luigi_grep.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/tools/range.py` & `luigi-3.3.0/luigi/tools/range.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/util.py` & `luigi-3.3.0/luigi/util.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi/worker.py` & `luigi-3.3.0/luigi/worker.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/luigi.egg-info/PKG-INFO` & `luigi-3.3.0/luigi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi
-Version: 3.2.1
+Version: 3.3.0
 Summary: Workflow mgmgt + task scheduling + dependency resolution.
 Home-page: https://github.com/spotify/luigi
 Author: The Luigi Authors
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `luigi-3.2.1/luigi.egg-info/SOURCES.txt` & `luigi-3.3.0/luigi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/setup.py` & `luigi-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/_mysqldb_test.py` & `luigi-3.3.0/test/_mysqldb_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/_test_ftp.py` & `luigi-3.3.0/test/_test_ftp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/batch_notifier_test.py` & `luigi-3.3.0/test/batch_notifier_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/choice_parameter_test.py` & `luigi-3.3.0/test/choice_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/clone_test.py` & `luigi-3.3.0/test/clone_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/cmdline_test.py` & `luigi-3.3.0/test/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/config_env_test.py` & `luigi-3.3.0/test/config_env_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/config_toml_test.py` & `luigi-3.3.0/test/config_toml_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/customized_run_test.py` & `luigi-3.3.0/test/customized_run_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/date_interval_test.py` & `luigi-3.3.0/test/date_interval_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/date_parameter_test.py` & `luigi-3.3.0/test/date_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/db_task_history_test.py` & `luigi-3.3.0/test/db_task_history_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/decorator_test.py` & `luigi-3.3.0/test/decorator_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/dict_parameter_test.py` & `luigi-3.3.0/test/dict_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/dynamic_import_test.py` & `luigi-3.3.0/test/dynamic_import_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/event_callbacks_test.py` & `luigi-3.3.0/test/event_callbacks_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/execution_summary_test.py` & `luigi-3.3.0/test/execution_summary_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/factorial_test.py` & `luigi-3.3.0/test/factorial_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/fib_test.py` & `luigi-3.3.0/test/fib_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/hdfs_client_test.py` & `luigi-3.3.0/test/hdfs_client_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/helpers.py` & `luigi-3.3.0/test/helpers.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/helpers_test.py` & `luigi-3.3.0/test/helpers_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/import_test.py` & `luigi-3.3.0/test/import_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/instance_test.py` & `luigi-3.3.0/test/instance_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/instance_wrap_test.py` & `luigi-3.3.0/test/instance_wrap_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/interface_test.py` & `luigi-3.3.0/test/interface_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/list_parameter_test.py` & `luigi-3.3.0/test/list_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/local_target_test.py` & `luigi-3.3.0/test/local_target_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/lock_test.py` & `luigi-3.3.0/test/lock_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/metrics_test.py` & `luigi-3.3.0/test/metrics_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/mock_test.py` & `luigi-3.3.0/test/mock_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/most_common_test.py` & `luigi-3.3.0/test/most_common_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/notifications_test.py` & `luigi-3.3.0/test/notifications_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/numerical_parameter_test.py` & `luigi-3.3.0/test/numerical_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/optional_parameter_test.py` & `luigi-3.3.0/test/optional_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/other_module.py` & `luigi-3.3.0/test/other_module.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/parameter_test.py` & `luigi-3.3.0/test/parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/priority_test.py` & `luigi-3.3.0/test/priority_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/range_test.py` & `luigi-3.3.0/test/range_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/recursion_test.py` & `luigi-3.3.0/test/recursion_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/remote_scheduler_test.py` & `luigi-3.3.0/test/remote_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/retcodes_test.py` & `luigi-3.3.0/test/retcodes_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/rpc_test.py` & `luigi-3.3.0/test/rpc_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/runtests.py` & `luigi-3.3.0/test/runtests.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/scheduler_api_test.py` & `luigi-3.3.0/test/scheduler_api_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/scheduler_message_test.py` & `luigi-3.3.0/test/scheduler_message_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/scheduler_parameter_visibilities_test.py` & `luigi-3.3.0/test/scheduler_parameter_visibilities_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/scheduler_test.py` & `luigi-3.3.0/test/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/scheduler_visualisation_test.py` & `luigi-3.3.0/test/scheduler_visualisation_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/server_test.py` & `luigi-3.3.0/test/server_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/set_task_name_test.py` & `luigi-3.3.0/test/set_task_name_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/setup_logging_test.py` & `luigi-3.3.0/test/setup_logging_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,18 +27,47 @@
 
         opts.background = False
         opts.logdir = False
         result = self.cls._cli(opts)
         self.assertFalse(result)
 
     def test_section(self):
-        self.cls.config = {'logging': {
-            'version': 1,
-            'disable_existing_loggers': False,
-        }}
+        self.cls.config = {
+            'logging': {
+                'version': 1,
+                'disable_existing_loggers': False,
+                'formatters': {
+                    'mockformatter': {
+                        'format': '{levelname}: {message}',
+                        'style': '{',
+                        'datefmt': '%Y-%m-%d %H:%M:%S',
+                    },
+                },
+                'handlers': {
+                    'mockhandler': {
+                        'class': 'logging.StreamHandler',
+                        'level': 'INFO',
+                        'formatter': 'mockformatter',
+                    },
+                },
+                'loggers': {
+                    'mocklogger': {
+                        'handlers': ('mockhandler',),
+                        'level': 'INFO',
+                        'disabled': False,
+                        'propagate': False,
+                    },
+                },
+            },
+        }
+        result = self.cls._section(None)
+        self.assertTrue(result)
+
+        self.cls.config = LuigiTomlParser()
+        self.cls.config.read(['./test/testconfig/luigi_logging.toml'])
         result = self.cls._section(None)
         self.assertTrue(result)
 
         self.cls.config = {}
         result = self.cls._section(None)
         self.assertFalse(result)
```

### Comparing `luigi-3.2.1/test/simulate_test.py` & `luigi-3.3.0/test/simulate_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/subtask_test.py` & `luigi-3.3.0/test/subtask_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/target_test.py` & `luigi-3.3.0/test/target_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_bulk_complete_test.py` & `luigi-3.3.0/test/task_bulk_complete_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_forwarded_attributes_test.py` & `luigi-3.3.0/test/task_forwarded_attributes_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_history_test.py` & `luigi-3.3.0/test/task_history_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_progress_percentage_test.py` & `luigi-3.3.0/test/task_progress_percentage_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_register_test.py` & `luigi-3.3.0/test/task_register_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_running_resources_test.py` & `luigi-3.3.0/test/task_running_resources_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_serialize_test.py` & `luigi-3.3.0/test/task_serialize_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_status_message_test.py` & `luigi-3.3.0/test/task_status_message_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/task_test.py` & `luigi-3.3.0/test/task_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/test_sigpipe.py` & `luigi-3.3.0/test/test_sigpipe.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/test_ssh.py` & `luigi-3.3.0/test/test_ssh.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/util_previous_test.py` & `luigi-3.3.0/test/util_previous_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/util_test.py` & `luigi-3.3.0/test/util_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/visible_parameters_test.py` & `luigi-3.3.0/test/visible_parameters_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_external_task_test.py` & `luigi-3.3.0/test/worker_external_task_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_keep_alive_test.py` & `luigi-3.3.0/test/worker_keep_alive_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_multiprocess_test.py` & `luigi-3.3.0/test/worker_multiprocess_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_parallel_scheduling_test.py` & `luigi-3.3.0/test/worker_parallel_scheduling_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_scheduler_com_test.py` & `luigi-3.3.0/test/worker_scheduler_com_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_task_process_test.py` & `luigi-3.3.0/test/worker_task_process_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_task_test.py` & `luigi-3.3.0/test/worker_task_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/worker_test.py` & `luigi-3.3.0/test/worker_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.2.1/test/wrap_test.py` & `luigi-3.3.0/test/wrap_test.py`

 * *Files identical despite different names*

