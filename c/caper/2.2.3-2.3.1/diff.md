# Comparing `tmp/caper-2.2.3.tar.gz` & `tmp/caper-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caper-2.2.3.tar", last modified: Mon Oct 24 18:36:21 2022, max compression
+gzip compressed data, was "caper-2.3.1.tar", last modified: Thu May  4 21:26:21 2023, max compression
```

## Comparing `caper-2.2.3.tar` & `caper-2.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.939720 caper-2.2.3/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-06-10 20:40:20.000000 caper-2.2.3/LICENSE
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      493 2022-10-24 18:36:21.935721 caper-2.2.3/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7862 2022-10-24 18:36:07.000000 caper-2.2.3/README.md
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.887721 caper-2.2.3/bin/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      295 2022-06-10 20:40:20.000000 caper-2.2.3/bin/caper
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2285 2022-06-10 20:40:20.000000 caper-2.2.3/bin/run_mysql_server_docker.sh
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2563 2022-06-10 20:40:20.000000 caper-2.2.3/bin/run_mysql_server_singularity.sh
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.919721 caper-2.2.3/caper/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      180 2022-10-24 18:36:07.000000 caper-2.2.3/caper/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-06-10 20:40:20.000000 caper-2.2.3/caper/__main__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5321 2022-06-10 20:40:20.000000 caper-2.2.3/caper/arg_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      528 2022-06-10 20:40:20.000000 caper-2.2.3/caper/backward_compatibility.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    36845 2022-07-21 17:02:18.000000 caper-2.2.3/caper/caper_args.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15742 2022-07-25 22:46:52.000000 caper-2.2.3/caper/caper_backend_conf.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7789 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_base.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    14581 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_client.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5386 2022-10-24 18:36:07.000000 caper-2.2.3/caper/caper_init.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2180 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_labels.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    22964 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_runner.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2631 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_wdl_parser.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    11869 2022-06-10 20:40:20.000000 caper-2.2.3/caper/caper_workflow_opts.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25618 2022-07-21 17:02:18.000000 caper-2.2.3/caper/cli.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2721 2022-07-21 17:02:18.000000 caper-2.2.3/caper/cli_hpc.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17278 2022-07-25 22:46:52.000000 caper-2.2.3/caper/cromwell.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    41929 2022-07-25 22:46:52.000000 caper-2.2.3/caper/cromwell_backend.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17399 2022-06-10 20:40:20.000000 caper-2.2.3/caper/cromwell_metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18534 2022-06-10 20:40:20.000000 caper-2.2.3/caper/cromwell_rest_api.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    13900 2022-06-10 20:40:20.000000 caper-2.2.3/caper/cromwell_workflow_monitor.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8644 2022-06-10 20:40:20.000000 caper-2.2.3/caper/dict_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6710 2022-06-10 20:40:20.000000 caper-2.2.3/caper/hocon_string.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7295 2022-07-21 17:02:18.000000 caper-2.2.3/caper/hpc.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9329 2022-07-21 17:02:18.000000 caper-2.2.3/caper/nb_subproc_thread.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    12256 2022-06-10 20:40:20.000000 caper-2.2.3/caper/resource_analysis.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4407 2022-06-10 20:40:20.000000 caper-2.2.3/caper/server_heartbeat.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2755 2022-06-10 20:40:20.000000 caper-2.2.3/caper/singularity.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7464 2022-06-10 20:40:20.000000 caper-2.2.3/caper/wdl_parser.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.923721 caper-2.2.3/caper.egg-info/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      493 2022-10-24 18:36:20.000000 caper-2.2.3/caper.egg-info/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1469 2022-10-24 18:36:21.000000 caper-2.2.3/caper.egg-info/SOURCES.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2022-10-24 18:36:21.000000 caper-2.2.3/caper.egg-info/dependency_links.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      171 2022-10-24 18:36:21.000000 caper-2.2.3/caper.egg-info/requires.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       12 2022-10-24 18:36:21.000000 caper-2.2.3/caper.egg-info/top_level.txt
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.883721 caper-2.2.3/scripts/
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.923721 caper-2.2.3/scripts/gcp_caper_server/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)    11437 2022-07-21 17:02:18.000000 caper-2.2.3/scripts/gcp_caper_server/create_instance.sh
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2022-10-24 18:36:21.939720 caper-2.2.3/setup.cfg
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1877 2022-06-10 20:40:20.000000 caper-2.2.3/setup.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-10-24 18:36:21.935721 caper-2.2.3/tests/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-06-10 20:40:20.000000 caper-2.2.3/tests/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2191 2022-06-10 20:40:20.000000 caper-2.2.3/tests/conftest.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3885 2022-06-10 20:40:20.000000 caper-2.2.3/tests/example_wdl.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6057 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_arg_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1029 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_caper_labels.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1115 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_caper_wdl_parser.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9494 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_caper_workflow_opts.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7089 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cli_run.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4736 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cli_server_client_gcp.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6256 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cromwell.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1287 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cromwell_backend.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3183 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cromwell_metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6134 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_cromwell_rest_api.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3857 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_dict_tool.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5988 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_hocon_string.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_nb_subproc_thread.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3119 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_resource_analysis.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      886 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_server_heartbeat.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1755 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_singularity.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1973 2022-06-10 20:40:20.000000 caper-2.2.3/tests/test_wdl_parser.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.847903 caper-2.3.1/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-06-10 20:40:20.000000 caper-2.3.1/LICENSE
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-05-04 21:26:21.847903 caper-2.3.1/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9015 2023-05-04 21:24:00.000000 caper-2.3.1/README.md
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.795904 caper-2.3.1/bin/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      295 2022-06-10 20:40:20.000000 caper-2.3.1/bin/caper
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2285 2022-06-10 20:40:20.000000 caper-2.3.1/bin/run_mysql_server_docker.sh
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)     2563 2022-06-10 20:40:20.000000 caper-2.3.1/bin/run_mysql_server_singularity.sh
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.823903 caper-2.3.1/caper/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      180 2023-05-04 21:24:00.000000 caper-2.3.1/caper/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-06-10 20:40:20.000000 caper-2.3.1/caper/__main__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5322 2023-05-04 21:24:00.000000 caper-2.3.1/caper/arg_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      528 2022-06-10 20:40:20.000000 caper-2.3.1/caper/backward_compatibility.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    36785 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_args.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15742 2022-07-25 22:46:52.000000 caper-2.3.1/caper/caper_backend_conf.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7780 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_base.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    14581 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_client.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5199 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_init.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2180 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_labels.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    22800 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_runner.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2599 2023-05-04 21:24:00.000000 caper-2.3.1/caper/caper_wdl_parser.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    11869 2022-06-10 20:40:20.000000 caper-2.3.1/caper/caper_workflow_opts.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25758 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cli.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2660 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cli_hpc.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17327 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    41912 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_backend.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    17381 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18525 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_rest_api.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    13873 2023-05-04 21:24:00.000000 caper-2.3.1/caper/cromwell_workflow_monitor.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8639 2023-05-04 21:24:00.000000 caper-2.3.1/caper/dict_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6705 2023-05-04 21:24:00.000000 caper-2.3.1/caper/hocon_string.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7534 2023-05-04 21:24:00.000000 caper-2.3.1/caper/hpc.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9319 2023-05-04 21:24:00.000000 caper-2.3.1/caper/nb_subproc_thread.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    12256 2022-06-10 20:40:20.000000 caper-2.3.1/caper/resource_analysis.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4407 2022-06-10 20:40:20.000000 caper-2.3.1/caper/server_heartbeat.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2755 2022-06-10 20:40:20.000000 caper-2.3.1/caper/singularity.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7455 2023-05-04 21:24:00.000000 caper-2.3.1/caper/wdl_parser.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.827903 caper-2.3.1/caper.egg-info/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      457 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1469 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/SOURCES.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/dependency_links.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      171 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/requires.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       12 2023-05-04 21:26:21.000000 caper-2.3.1/caper.egg-info/top_level.txt
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.795904 caper-2.3.1/scripts/
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.831903 caper-2.3.1/scripts/gcp_caper_server/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)    11437 2022-07-21 17:02:18.000000 caper-2.3.1/scripts/gcp_caper_server/create_instance.sh
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2023-05-04 21:26:21.847903 caper-2.3.1/setup.cfg
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1877 2023-05-04 21:24:00.000000 caper-2.3.1/setup.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 21:26:21.847903 caper-2.3.1/tests/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-06-10 20:40:20.000000 caper-2.3.1/tests/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2186 2023-05-04 21:24:00.000000 caper-2.3.1/tests/conftest.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3885 2022-06-10 20:40:20.000000 caper-2.3.1/tests/example_wdl.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6057 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_arg_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1029 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_caper_labels.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1107 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_caper_wdl_parser.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     9479 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_caper_workflow_opts.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7079 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cli_run.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     4731 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cli_server_client_gcp.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6251 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1282 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell_backend.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3183 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_cromwell_metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6129 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_cromwell_rest_api.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3857 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_dict_tool.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5983 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_hocon_string.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2595 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_nb_subproc_thread.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3114 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_resource_analysis.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      886 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_server_heartbeat.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1755 2022-06-10 20:40:20.000000 caper-2.3.1/tests/test_singularity.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1957 2023-05-04 21:24:00.000000 caper-2.3.1/tests/test_wdl_parser.py
```

### Comparing `caper-2.2.3/LICENSE` & `caper-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/README.md` & `caper-2.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
 > **IMPORTANT**: Docker/singularity/conda defined in Caper's configuration file or in CLI (`--docker`, `--singularity` and `--conda`) will be overriden by those defined in WDL task's `runtime`. We provide these parameters to define default/base environment for a pipeline, not to override on WDL task's `runtime`.
 
 For Conda users, make sure that you have installed pipeline's Conda environments before running pipelines. Caper only knows Conda environment's name. You don't need to activate any Conda environment before running a pipeline since Caper will internally run `conda run -n ENV_NAME TASK_SHELL_SCRIPT` for each task.
 
 Take a look at the following examples:
 ```bash
-$ caper run test.wdl --docker # can be used as a flag too, Caper will find a docker image defined in WDL
-$ caper run test.wdl --singularity docker://ubuntu:latest
+$ caper run test.wdl --docker # can be used as a flag too, Caper will find a default docker image in WDL if defined
+$ caper run test.wdl --singularity docker://ubuntu:latest # define default singularity image in the command line
 $ caper hpc submit test.wdl --singularity --leader-job-name test1 # submit to job engine and use singularity defined in WDL
 $ caper submit test.wdl --conda your_conda_env_name # running caper server is required
 ```
 
 An environemnt defined here will be overriden by those defined in WDL task's `runtime`. Therefore, think of this as a base/default environment for your pipeline. You can define per-task docker, singularity images to override those defined in Caper's command line. For example:
 ```wdl
 task my_task {
@@ -94,15 +94,16 @@
 $ cd [OUTPUT_DIR]
 
 # Example with Singularity without using call-caching.
 $ caper hpc submit [WDL] -i [INPUT_JSON] --singularity --leader-job-name GOOD_NAME1
 
 # Example with Conda and using call-caching (restarting a workflow from where it left off)
 # Use the same --file-db PATH for next re-run then Caper will collect and softlink previous outputs.
-$ caper hpc submit [WDL] -i [INPUT_JSON] --conda --leader-job-name GOOD_NAME2 --db file --file-db [METADATA_DB_PATH] 
+# If you see any DB connection error then replace it with "--db in-memory" then call-cahing will be disabled
+$ caper hpc submit [WDL] -i [INPUT_JSON] --conda --leader-job-name GOOD_NAME2 --file-db [METADATA_DB_PATH]
 
 # List all leader jobs.
 $ caper hpc list
 
 # Check leader job's STDOUT file to monitor workflow's status.
 # Example for SLURM
 $ tail -f slurm-[JOB_ID].out
@@ -112,14 +113,32 @@
 $ ls -l cromwell.out*
 
 # Abort a leader job (this will cascade-kill all its child jobs)
 # If you directly use job engine's command like scancel or qdel then child jobs will still remain running.
 $ caper hpc abort [JOB_ID]
 ```
 
+## Restarting a pipeline on local machine (and HPCs)
+
+Caper uses Cromwell's call-caching to restart a pipeline from where it left off. Such database is automatically generated on `local_out_dir` defined in the configuration file `~/.caper/default.conf`. The DB file name is simply consist of WDL's basename and input JSON file's basename so you can simply run the same `caper run` command line on the same working directory to restart a workflow.
+
+```bash
+# for standalone/client
+$ caper run ... --db in-memory
+
+# for server
+$ caper server ... --db in-memory
+````
+
+
+## DB connection timeout
+
+If you see any DB connection timeout error, that means you have multiple caper/Cromwell processes trying to connect to the same file DB. Check any running Cromwell processes with `ps aux | grep cromwell` and close them with `kill         PID`. If that does not fix the problem, then use `caper run ... --db in-memory` to disable Cromwell's metadata DB. You will not be able to use call-caching.
+
+
 ## Customize resource parameters on HPCs
 
 If default settings of Caper does not work with your HPC, then see [this document](docs/resource_param.md) to manually customize resource command line (e.g. `sbatch ... [YOUR_CUSTOM_PARAMETER]`) for your chosen backend.
 
 # DETAILS
 
 See [details](DETAILS.md).
```

### Comparing `caper-2.2.3/bin/run_mysql_server_docker.sh` & `caper-2.3.1/bin/run_mysql_server_docker.sh`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/bin/run_mysql_server_singularity.sh` & `caper-2.3.1/bin/run_mysql_server_singularity.sh`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/arg_tool.py` & `caper-2.3.1/caper/arg_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from argparse import ArgumentParser
 from configparser import ConfigParser, MissingSectionHeaderError
+
 from distutils.util import strtobool
 
 
 def read_from_conf(
     conf_file, conf_section='defaults', conf_key_map=None, no_strip_quote=False
 ):
     """Read key/value from conf_section of conf_file.
```

### Comparing `caper-2.2.3/caper/backward_compatibility.py` & `caper-2.3.1/caper/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/caper_args.py` & `caper-2.3.1/caper/caper_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,22 +19,17 @@
     CromwellBackendCommon,
     CromwellBackendDatabase,
     CromwellBackendGcp,
     CromwellBackendLocal,
     CromwellBackendSlurm,
 )
 from .cromwell_rest_api import CromwellRestAPI
+from .hpc import LsfWrapper, PbsWrapper, SgeWrapper, SlurmWrapper
 from .resource_analysis import ResourceAnalysis
 from .server_heartbeat import ServerHeartbeat
-from .hpc import (
-    SlurmWrapper,
-    SgeWrapper,
-    PbsWrapper,
-    LsfWrapper,
-)
 
 DEFAULT_CAPER_CONF = '~/.caper/default.conf'
 DEFAULT_LIST_FORMAT = 'id,status,name,str_label,user,parent,submission'
 DEFAULT_OUT_DIR = '.'
 DEFAULT_CROMWELL_STDOUT = './cromwell.out'
 
 
@@ -159,15 +154,15 @@
         'incremented index. e.g. cromwell.out.1 ',
     )
     group_db = parent_runner.add_argument_group(
         title='General DB settings (for both file DB and MySQL DB)'
     )
     group_db.add_argument(
         '--db',
-        default=CromwellBackendDatabase.DEFAULT_DB,
+        default=CromwellBackendDatabase.DB_FILE,
         help='Cromwell metadata database type',
     )
     group_db.add_argument(
         '--db-timeout',
         type=int,
         default=CromwellBackendDatabase.DEFAULT_DB_TIMEOUT_MS,
         help='Milliseconds to wait for DB connection.',
@@ -530,39 +525,39 @@
     group_hpc_submit = parent_submit.add_argument_group(
         title='Parameters for "caper hpc submit" command only',
     )
     group_hpc_submit.add_argument(
         '--leader-job-name',
         help='Leader job name for a submitted workflow.'
         'This name will be appended to the prefix "CAPER_LEADER_" and then '
-        'submitted to HPC. Such prefix is used to identify Caper leader jobs.'
+        'submitted to HPC. Such prefix is used to identify Caper leader jobs.',
     )
     group_hpc_submit.add_argument(
         '--slurm-leader-job-resource-param',
         help='Resource parameters to submit a Caper leader job to SLURM. '
         'Make sure to quote if you use it in the command line arguments.',
-        default=' '.join(SlurmWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM)
+        default=' '.join(SlurmWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM),
     )
     group_hpc_submit.add_argument(
         '--sge-leader-job-resource-param',
         help='Resource parameters to submit a Caper leader job to SGE'
         'Make sure to quote if you use it in the command line arguments.',
-        default=' '.join(SgeWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM)
+        default=' '.join(SgeWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM),
     )
     group_hpc_submit.add_argument(
         '--pbs-leader-job-resource-param',
         help='Resource parameters to submit a Caper leader job to PBS'
         'Make sure to quote if you use it in the command line arguments.',
-        default=' '.join(PbsWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM)
+        default=' '.join(PbsWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM),
     )
     group_hpc_submit.add_argument(
         '--lsf-leader-job-resource-param',
         help='Resource parameters to submit a Caper leader job to LSF'
         'Make sure to quote if you use it in the command line arguments.',
-        default=' '.join(LsfWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM)
+        default=' '.join(LsfWrapper.DEFAULT_LEADER_JOB_RESOURCE_PARAM),
     )
 
     group_slurm = parent_submit.add_argument_group('SLURM arguments')
     group_slurm.add_argument('--slurm-partition', help='SLURM partition')
     group_slurm.add_argument('--slurm-account', help='SLURM account')
     group_slurm.add_argument(
         '--slurm-extra-param', help='SLURM extra parameters to be passed to sbatch. '
@@ -767,15 +762,15 @@
     )
 
     # hpc abort
     parent_hpc_abort = argparse.ArgumentParser(add_help=False)
     parent_hpc_abort.add_argument(
         'job_ids',
         nargs='+',
-        help='Job ID or list of job IDs to abort matching Caper leader jobs.'
+        help='Job ID or list of job IDs to abort matching Caper leader jobs.',
     )
 
     # all subcommands
     p_init = subparser.add_parser(
         'init',
         help='Initialize Caper\'s configuration file. THIS WILL OVERWRITE ON '
         'A SPECIFIED(-c)/DEFAULT CONF FILE. e.g. ~/.caper/default.conf.',
@@ -860,26 +855,26 @@
 
     p_hpc = subparser.add_parser(
         'hpc',
         help='Subcommand for HPCs',
         parents=[parent_all],
     )
     subparser_hpc = p_hpc.add_subparsers(dest='hpc_action')
-    p_hpc_submit = subparser_hpc.add_parser(
+    subparser_hpc.add_parser(
         'submit',
         help='Submit a single workflow to HPC.',
         parents=[parent_all, parent_submit, parent_run, parent_runner, parent_backend],
     )
 
-    p_hpc_list = subparser_hpc.add_parser(
+    subparser_hpc.add_parser(
         'list',
         help='List all workflows submitted to HPC.',
         parents=[parent_all, parent_backend],
     )
-    p_hpc_abort = subparser_hpc.add_parser(
+    subparser_hpc.add_parser(
         'abort',
         help='Abort a workflow submitted to HPC.',
         parents=[parent_all, parent_backend, parent_hpc_abort],
     )
 
     p_gcp_monitor = subparser.add_parser(
         'gcp_monitor',
```

### Comparing `caper-2.2.3/caper/caper_backend_conf.py` & `caper-2.3.1/caper/caper_backend_conf.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/caper_base.py` & `caper-2.3.1/caper/caper_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
         logger.info(
             'Creating a timestamped temporary directory. {d}'.format(d=work_dir)
         )
 
         return work_dir
 
     def get_loc_dir(self, backend):
-        """Get localization directory for a backend.
-        """
+        """Get localization directory for a backend."""
         if backend == BACKEND_GCP:
             return self._gcp_loc_dir
         elif backend == BACKEND_AWS:
             return self._aws_loc_dir
         else:
             return self._local_loc_dir
```

### Comparing `caper-2.2.3/caper/caper_client.py` & `caper-2.3.1/caper/caper_client.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/caper_init.py` & `caper-2.3.1/caper/caper_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,16 @@
     BACKEND_AWS,
     BACKEND_GCP,
     BACKEND_LOCAL,
     BACKEND_LSF,
     BACKEND_PBS,
     BACKEND_SGE,
     BACKEND_SLURM,
-    CromwellBackendLsf,
-    CromwellBackendPbs,
-    CromwellBackendSge,
-    CromwellBackendSlurm,
 )
 
-from .hpc import (
-    SlurmWrapper,
-    SgeWrapper,
-    PbsWrapper,
-    LsfWrapper,
-)
-
-
 CONF_CONTENTS_TMP_DIR = """
 # Local directory for localized files and Cromwell's intermediate files.
 # If not defined then Caper will make .caper_tmp/ on CWD or `local-out-dir`.
 # /tmp is not recommended since Caper store localized data files here.
 local-loc-dir=
 """
```

### Comparing `caper-2.2.3/caper/caper_labels.py` & `caper-2.3.1/caper/caper_labels.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/caper_runner.py` & `caper-2.3.1/caper/caper_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,55 +491,55 @@
         embed_subworkflow=False,
         java_heap_server=Cromwell.DEFAULT_JAVA_HEAP_CROMWELL_SERVER,
         auto_write_metadata=True,
         work_dir=None,
         dry_run=False,
     ):
         """Run a Cromwell server.
-            default_backend:
-                Default backend. If backend is not specified for a submitted workflow
-                then default backend will be used.
-                Choose among Caper's built-in backends.
-                (aws, gcp, Local, slurm, sge, pbs, lsf).
-                Or use a backend defined in your custom backend config file
-                (above "backend_conf" file).
-            server_heartbeat:
-                Server heartbeat to write hostname/port of a server.
-            server_port:
-                Server port to run Cromwell server.
-                Make sure to use different port for multiple Cromwell servers on the same
-                machine.
-            server_hostname:
-                Server hostname. If not defined then socket.gethostname() will be used.
-                If server_heartbeat is given, then this hostname will be written to
-                the server heartbeat file defined in server_heartbeat.
-            custom_backend_conf:
-                Backend config file (HOCON) to override Caper's auto-generated backend config.
-            fileobj_stdout:
-                File-like object to write Cromwell's STDOUT.
-            embed_subworkflow:
-                Caper stores/updates metadata.JSON file on
-                each workflow's root directory whenever there is status change
-                of workflow (or its tasks).
-                This flag ensures that any subworkflow's metadata JSON will be
-                embedded in main (this) workflow's metadata JSON.
-                This is to mimic behavior of Cromwell run mode's -m parameter.
-            java_heap_server:
-                Java heap (java -Xmx) for Cromwell server mode.
-            auto_write_metadata:
-                Automatic retrieval/writing of metadata.json upon workflow/task's status change.
-            work_dir:
-                Local temporary directory to store all temporary files.
-                Temporary files mean intermediate files used for running Cromwell.
-                For example, auto-generated backend config file and workflow options file.
-                If this is not defined, then cache directory self._local_loc_dir with a timestamp
-                will be used.
-                However, Cromwell Java process itself will run on CWD instead of this directory.
-            dry_run:
-                Stop before running Java command line for Cromwell.
+        default_backend:
+            Default backend. If backend is not specified for a submitted workflow
+            then default backend will be used.
+            Choose among Caper's built-in backends.
+            (aws, gcp, Local, slurm, sge, pbs, lsf).
+            Or use a backend defined in your custom backend config file
+            (above "backend_conf" file).
+        server_heartbeat:
+            Server heartbeat to write hostname/port of a server.
+        server_port:
+            Server port to run Cromwell server.
+            Make sure to use different port for multiple Cromwell servers on the same
+            machine.
+        server_hostname:
+            Server hostname. If not defined then socket.gethostname() will be used.
+            If server_heartbeat is given, then this hostname will be written to
+            the server heartbeat file defined in server_heartbeat.
+        custom_backend_conf:
+            Backend config file (HOCON) to override Caper's auto-generated backend config.
+        fileobj_stdout:
+            File-like object to write Cromwell's STDOUT.
+        embed_subworkflow:
+            Caper stores/updates metadata.JSON file on
+            each workflow's root directory whenever there is status change
+            of workflow (or its tasks).
+            This flag ensures that any subworkflow's metadata JSON will be
+            embedded in main (this) workflow's metadata JSON.
+            This is to mimic behavior of Cromwell run mode's -m parameter.
+        java_heap_server:
+            Java heap (java -Xmx) for Cromwell server mode.
+        auto_write_metadata:
+            Automatic retrieval/writing of metadata.json upon workflow/task's status change.
+        work_dir:
+            Local temporary directory to store all temporary files.
+            Temporary files mean intermediate files used for running Cromwell.
+            For example, auto-generated backend config file and workflow options file.
+            If this is not defined, then cache directory self._local_loc_dir with a timestamp
+            will be used.
+            However, Cromwell Java process itself will run on CWD instead of this directory.
+        dry_run:
+            Stop before running Java command line for Cromwell.
         """
         if work_dir is None:
             work_dir = self.create_timestamped_work_dir(
                 prefix=CaperRunner.SERVER_TMP_DIR_PREFIX
             )
 
         backend_conf = self._caper_backend_conf.create_file(
```

### Comparing `caper-2.2.3/caper/caper_wdl_parser.py` & `caper-2.3.1/caper/caper_wdl_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from .wdl_parser import WDLParser
 
 logger = logging.getLogger(__name__)
 
 
 class CaperWDLParser(WDLParser):
-    """WDL parser for Caper.
-    """
+    """WDL parser for Caper."""
 
     RE_WDL_COMMENT_DOCKER = r'^\s*\#\s*CAPER\s+docker\s(.+)'
     RE_WDL_COMMENT_SINGULARITY = r'^\s*\#\s*CAPER\s+singularity\s(.+)'
     WDL_WORKFLOW_META_DOCKER_KEYS = ('default_docker', 'caper_docker')
     WDL_WORKFLOW_META_SINGULARITY_KEYS = ('default_singularity', 'caper_singularity')
     WDL_WORKFLOW_META_CONDA_KEYS = (
         'default_conda',
@@ -21,16 +20,15 @@
     )
 
     def __init__(self, wdl):
         super().__init__(wdl)
 
     @property
     def caper_docker(self):
-        """Backward compatibility for property name. See property default_docker.
-        """
+        """Backward compatibility for property name. See property default_docker."""
         return self.default_docker
 
     @property
     def default_docker(self):
         """Find a default Docker image in WDL for Caper.
 
         Backward compatibililty:
@@ -44,16 +42,15 @@
 
         ret = self._find_val_of_matched_lines(CaperWDLParser.RE_WDL_COMMENT_DOCKER)
         if ret:
             return ret[0].strip('"\'')
 
     @property
     def caper_singularity(self):
-        """Backward compatibility for property name. See property default_singularity.
-        """
+        """Backward compatibility for property name. See property default_singularity."""
         return self.default_singularity
 
     @property
     def default_singularity(self):
         """Find a default Singularity image in WDL for Caper.
 
         Backward compatibililty:
@@ -67,13 +64,12 @@
 
         ret = self._find_val_of_matched_lines(CaperWDLParser.RE_WDL_COMMENT_SINGULARITY)
         if ret:
             return ret[0].strip('"\'')
 
     @property
     def default_conda(self):
-        """Find a default Conda environment name in WDL for Caper.
-        """
+        """Find a default Conda environment name in WDL for Caper."""
         if self.workflow_meta:
             for conda_key in CaperWDLParser.WDL_WORKFLOW_META_CONDA_KEYS:
                 if conda_key in self.workflow_meta:
                     return self.workflow_meta[conda_key]
```

### Comparing `caper-2.2.3/caper/caper_workflow_opts.py` & `caper-2.3.1/caper/caper_workflow_opts.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/cli.py` & `caper-2.3.1/caper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 #!/usr/bin/env python3
 import copy
 import csv
 import json
 import logging
 import os
 import re
-import subprocess
 import sys
 
 from autouri import GCSURI, AutoURI
 
 from . import __version__ as version
 from .caper_args import ResourceAnalysisReductionMethod, get_parser_and_defaults
 from .caper_client import CaperClient, CaperClientSubmit
 from .caper_init import init_caper_conf
 from .caper_labels import CaperLabels
 from .caper_runner import CaperRunner
+from .cli_hpc import subcmd_hpc
 from .cromwell_backend import (
     BACKEND_ALIAS_LOCAL,
     BACKEND_LOCAL,
     CromwellBackendDatabase,
 )
 from .cromwell_metadata import CromwellMetadata
 from .dict_tool import flatten_dict
 from .resource_analysis import LinearResourceAnalysis
 from .server_heartbeat import ServerHeartbeat
-from .cli_hpc import subcmd_hpc
-
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_DB_FILE_PREFIX = 'caper_file_db'
+DEFAULT_DB_FILE_PREFIX = 'caper-db'
 DEFAULT_SERVER_HEARTBEAT_FILE = '~/.caper/default_server_heartbeat'
 USER_INTERRUPT_WARNING = (
     '\n\n'
     '*** DO NOT CTRL+C MULTIPLE TIMES! ***\n'
     '*** OR CAPER WILL NOT BE ABLE TO STOP CROMWELL AND RUNNING WORKFLOWS/TASKS ***'
     '\n\n'
 )
@@ -168,19 +166,21 @@
 
 
 def check_db_path(args):
     if hasattr(args, 'db') and args.db == CromwellBackendDatabase.DB_FILE:
         args.file_db = get_abspath(args.file_db)
 
         if not args.file_db:
-            prefix = DEFAULT_DB_FILE_PREFIX
+            db_filename_list = [DEFAULT_DB_FILE_PREFIX]
+            if hasattr(args, 'wdl') and args.wdl:
+                db_filename_list.append(os.path.basename(args.wdl))
             if hasattr(args, 'inputs') and args.inputs:
-                prefix += '_' + os.path.splitext(os.path.basename(args.inputs))[0]
-
-            args.file_db = os.path.join(args.local_out_dir, prefix)
+                db_filename_list.append(os.path.basename(args.inputs))
+            db_filename = '_'.join(db_filename_list)
+            args.file_db = os.path.join(args.local_out_dir, db_filename)
 
 
 def check_backend(args):
     """Check if local backend is in lower cases.
     "Local" should be capitalized. i.e. local -> Local.
     BACKEND_LOCAL is Local.
     BACKEND_ALIAS_LOCAL is local.
@@ -322,15 +322,14 @@
             subcmd_gcp_res_analysis(c, args)
         elif args.action == 'cleanup':
             subcmd_cleanup(c, args)
         else:
             raise ValueError('Unsupported client action {act}'.format(act=args.action))
 
 
-
 def subcmd_server(caper_runner, args, nonblocking=False):
     """
     Args:
         nonblocking:
             Make this function return a Thread object
             instead of blocking (Thread.join()).
             Also writes Cromwell's STDOUT to sys.stdout
@@ -537,16 +536,15 @@
             raise ValueError('Found no workflow matching with search query.')
         metadata = metadata_objs[0]
 
     return CromwellMetadata(metadata)
 
 
 def split_list_into_file_and_non_file(lst):
-    """Returns tuple of (list of existing files, list of non-file strings)
-    """
+    """Returns tuple of (list of existing files, list of non-file strings)"""
     files = []
     non_files = []
 
     for maybe_file in lst:
         if AutoURI(get_abspath(maybe_file)).exists:
             files.append(maybe_file)
         else:
@@ -662,16 +660,15 @@
         target_resources=args.target_resources,
         plot_pdf=get_abspath(args.plot_pdf),
     )
     print(json.dumps(result, indent=4))
 
 
 def subcmd_cleanup(caper_client, args):
-    """Cleanup outputs of a workflow.
-    """
+    """Cleanup outputs of a workflow."""
     cm = get_single_cromwell_metadata_obj(caper_client, args, 'cleanup')
     cm.cleanup(dry_run=not args.delete, num_threads=args.num_threads, no_lock=True)
     if not args.delete:
         logger.warning(
             'Use --delete to DELETE ALL OUTPUTS of this workflow. '
             'This action is NOT REVERSIBLE. Use this at your own risk.'
         )
```

### Comparing `caper-2.2.3/caper/cli_hpc.py` & `caper-2.3.1/caper/cli_hpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sys
 
-from .hpc import (SlurmWrapper, SgeWrapper, PbsWrapper, LsfWrapper)
+from .hpc import LsfWrapper, PbsWrapper, SgeWrapper, SlurmWrapper
 
 logger = logging.getLogger(__name__)
 
 
 def make_caper_run_command_for_hpc_submit():
     """Makes `caper run ...` command from `caper hpc submit` command by simply
     replacing `caper hpc submit` with `caper run`.
@@ -30,33 +30,30 @@
             )
         caper_run_command = make_caper_run_command_for_hpc_submit()
 
         if args.backend == 'slurm':
             stdout = SlurmWrapper(
                 args.slurm_leader_job_resource_param.split(),
                 args.slurm_partition,
-                args.slurm_account
+                args.slurm_account,
             ).submit(args.leader_job_name, caper_run_command)
 
         elif args.backend == 'sge':
             stdout = SgeWrapper(
-                args.sge_leader_job_resource_param.split(),
-                args.sge_queue
+                args.sge_leader_job_resource_param.split(), args.sge_queue
             ).submit(args.leader_job_name, caper_run_command)
-            
+
         elif args.backend == 'pbs':
             stdout = PbsWrapper(
-                args.pbs_leader_job_resource_param.split(),
-                args.pbs_queue
+                args.pbs_leader_job_resource_param.split(), args.pbs_queue
             ).submit(args.leader_job_name, caper_run_command)
 
         elif args.backend == 'lsf':
             stdout = LsfWrapper(
-                args.lsf_leader_job_resource_param.split(),
-                args.lsf_queue
+                args.lsf_leader_job_resource_param.split(), args.lsf_queue
             ).submit(args.leader_job_name, caper_run_command)
 
         else:
             raise ValueError('Unsupported backend {b} for hpc'.format(b=args.backend))
     else:
         if args.backend == 'slurm':
             hpc_wrapper = SlurmWrapper()
```

### Comparing `caper-2.2.3/caper/cromwell.py` & `caper-2.3.1/caper/cromwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         return AbsPath(f).uri
     logger.info('Installing {label}... {f}'.format(label=label, f=f))
     path = os.path.join(os.path.expanduser(install_dir), AutoURI(f).basename)
     return AutoURI(f).cp(path)
 
 
 class Cromwell:
-    """Wraps Cromwell/Womtool.
-    """
+    """Wraps Cromwell/Womtool."""
 
     DEFAULT_CROMWELL = 'https://github.com/broadinstitute/cromwell/releases/download/82/cromwell-82.jar'
     DEFAULT_WOMTOOL = (
         'https://github.com/broadinstitute/cromwell/releases/download/82/womtool-82.jar'
     )
     DEFAULT_CROMWELL_INSTALL_DIR = '~/.caper/cromwell_jar'
     DEFAULT_WOMTOOL_INSTALL_DIR = '~/.caper/womtool_jar'
@@ -154,15 +153,17 @@
                 if th.returncode == 127:
                     raise FileNotFoundError(
                         'Java executable not found on your system? '
                         'Please install Java and try again.'
                     )
                 else:
                     raise WomtoolValidationFailed(
-                        'RC={rc}\nSTDERR={stderr}'.format(rc=th.returncode, stderr=stderr)
+                        'RC={rc}\nSTDERR={stderr}'.format(
+                            rc=th.returncode, stderr=stderr
+                        )
                     )
 
             logger.info('Passed Womtool validation.')
 
     def run(
         self,
         wdl,
```

### Comparing `caper-2.2.3/caper/cromwell_backend.py` & `caper-2.3.1/caper/cromwell_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 CALL_CACHING_DUP_STRAT_HARDLINK = 'hard-link'
 CALL_CACHING_DUP_STRAT_REFERENCE = 'reference'
 CALL_CACHING_DUP_STRAT_SOFTLINK = 'soft-link'
 
 LOCAL_HASH_STRAT_FILE = 'file'
 LOCAL_HASH_STRAT_PATH = 'path'
 LOCAL_HASH_STRAT_PATH_MTIME = 'path+modtime'
+LOCAL_HASH_START_XXH64 = 'xxh64'
 SOFT_GLOB_OUTPUT_CMD = 'ln -sL GLOB_PATTERN GLOB_DIRECTORY 2> /dev/null'
 
 
 def get_s3_bucket_name(s3_uri):
     return s3_uri.replace('s3://', '', 1).split('/')[0]
 
 
 class CromwellBackendCommon(UserDict):
-    """Basic stanzas for Cromwell backend conf.
-    """
+    """Basic stanzas for Cromwell backend conf."""
 
     TEMPLATE = {
         'backend': {},
         'webservice': {},
         'services': {
             'LoadController': {
                 'class': 'cromwell.services.loadcontroller.impl'
@@ -101,30 +101,28 @@
         # if memory_retry_error_keys:
         #     if isinstance(memory_retry_error_keys, tuple):
         #         memory_retry_error_keys = list(memory_retry_error_keys)
         #     self['system']['memory-retry-error-keys'] = memory_retry_error_keys
 
 
 class CromwellBackendServer(UserDict):
-    """Stanzas for Cromwell server.
-    """
+    """Stanzas for Cromwell server."""
 
     TEMPLATE = {'webservice': {}}
 
     DEFAULT_SERVER_PORT = 8000
 
     def __init__(self, server_port=DEFAULT_SERVER_PORT):
         super().__init__(deepcopy(CromwellBackendServer.TEMPLATE))
 
         self['webservice']['port'] = server_port
 
 
 class CromwellBackendDatabase(UserDict):
-    """Common stanzas for Cromwell's metadata database.
-    """
+    """Common stanzas for Cromwell's metadata database."""
 
     TEMPLATE = {'database': {'db': {'connectionTimeout': 5000, 'numThreads': 1}}}
 
     DB_IN_MEMORY = 'in-memory'
     DB_FILE = 'file'
     DB_MYSQL = 'mysql'
     DB_POSTGRESQL = 'postgresql'
@@ -215,16 +213,15 @@
             db_obj['password'] = postgresql_db_password
 
         else:
             raise ValueError('Unsupported DB type {db}'.format(db=db))
 
 
 class CromwellBackendBase(UserDict):
-    """Base skeleton backend for all backends
-    """
+    """Base skeleton backend for all backends"""
 
     TEMPLATE = {'backend': {'providers': {}}}
     TEMPLATE_BACKEND = {'config': {'default-runtime-attributes': {}, 'filesystems': {}}}
     DEFAULT_CALL_CACHING_DUP_STRAT = (
         CALL_CACHING_DUP_STRAT_SOFTLINK,
         CALL_CACHING_DUP_STRAT_HARDLINK,
         CALL_CACHING_DUP_STRAT_COPY,
@@ -282,24 +279,21 @@
 
     @property
     def backend_config(self):
         return self.backend['config']
 
     @property
     def default_runtime_attributes(self):
-        """Backend's default runtime attributes in self.backend_config.
-        """
+        """Backend's default runtime attributes in self.backend_config."""
         return self.backend_config['default-runtime-attributes']
 
 
 class CromwellBackendGcp(CromwellBackendBase):
     TEMPLATE = {
-        'google': {
-            'application-name': 'cromwell'
-        },
+        'google': {'application-name': 'cromwell'},
         'engine': {'filesystems': {FILESYSTEM_GCS: {'auth': 'default'}}},
     }
     TEMPLATE_BACKEND = {
         'config': {
             'default-runtime-attributes': {},
             'genomics-api-queries-per-100-seconds': 1000,
             'maximum-polling-interval': 600,
@@ -386,15 +380,17 @@
             self['engine']['filesystems'][FILESYSTEM_GCS]['auth'] = 'service-account'
         else:
             genomics['auth'] = 'application-default'
             filesystems[FILESYSTEM_GCS]['auth'] = 'application-default'
             self['google']['auths'] = [
                 {'name': 'application-default', 'scheme': 'application_default'}
             ]
-            self['engine']['filesystems'][FILESYSTEM_GCS]['auth'] = 'application-default'
+            self['engine']['filesystems'][FILESYSTEM_GCS][
+                'auth'
+            ] = 'application-default'
 
         if use_google_cloud_life_sciences:
             self.backend['actor-factory'] = CromwellBackendGcp.ACTOR_FACTORY_V2BETA
             genomics['endpoint-url'] = CromwellBackendGcp.GENOMICS_ENDPOINT_V2BETA
             genomics['location'] = gcp_region
         else:
             self.backend['actor-factory'] = CromwellBackendGcp.ACTOR_FACTORY_V2ALPHA
@@ -486,34 +482,34 @@
         )
         self.default_runtime_attributes['queueArn'] = aws_batch_arn
 
 
 class CromwellBackendLocal(CromwellBackendBase):
     """Class constants:
 
-        SUBMIT_DOCKER:
-            Cromwell falls back to 'submit_docker' instead of 'submit' if WDL task has
-            'docker' in runtime and runtime-attributes are declared in backend's config.
-
-            Docker and Singularity can map paths between inside and outside of the container.
-            So this is not an issue for those container environments.
-
-            For Conda, any container paths (docker_cwd, e.g. /cromwell-executions/**)
-            in the script is simply replaced with CWD.
-
-            This also replaces filenames written in write_*.tsv files (globbed by WDL functions).
-            e.g. write_lines(), write_tsv(), ...
-
-            See the following document for such WDL functions:
-            https://github.com/openwdl/wdl/blob/main/versions/development/SPEC.md#file-write_linesarraystring
-
-            Possible issue:
-            - 'sed' is used here with a delimiter as hash mark (#)
-              so hash marks in output path can result in error.
-            - Files globbed by WDL functions other than write_*() will still have paths inside a container.
+    SUBMIT_DOCKER:
+        Cromwell falls back to 'submit_docker' instead of 'submit' if WDL task has
+        'docker' in runtime and runtime-attributes are declared in backend's config.
+
+        Docker and Singularity can map paths between inside and outside of the container.
+        So this is not an issue for those container environments.
+
+        For Conda, any container paths (docker_cwd, e.g. /cromwell-executions/**)
+        in the script is simply replaced with CWD.
+
+        This also replaces filenames written in write_*.tsv files (globbed by WDL functions).
+        e.g. write_lines(), write_tsv(), ...
+
+        See the following document for such WDL functions:
+        https://github.com/openwdl/wdl/blob/main/versions/development/SPEC.md#file-write_linesarraystring
+
+        Possible issue:
+        - 'sed' is used here with a delimiter as hash mark (#)
+          so hash marks in output path can result in error.
+        - Files globbed by WDL functions other than write_*() will still have paths inside a container.
     """
 
     RUNTIME_ATTRIBUTES = dedent(
         """
         ## Caper custom attributes
         # Environment choices = (docker, conda, singularity)
         # If environment is not specified then prioritize docker > singularity > conda
@@ -635,15 +631,15 @@
             },
             'runtime-attributes': RUNTIME_ATTRIBUTES + RUNTIME_ATTRIBUTES_DOCKER,
             'submit': SUBMIT,
             'submit-docker': SUBMIT_DOCKER,
             'kill-docker': KILL_DOCKER,
         },
     }
-    DEFAULT_LOCAL_HASH_STRAT = LOCAL_HASH_STRAT_PATH_MTIME
+    DEFAULT_LOCAL_HASH_STRAT = LOCAL_HASH_START_XXH64
 
     def __init__(
         self,
         local_out_dir,
         backend_name=BACKEND_LOCAL,
         soft_glob_output=False,
         local_hash_strat=DEFAULT_LOCAL_HASH_STRAT,
@@ -667,14 +663,15 @@
         filesystem_local = config['filesystems'][FILESYSTEM_LOCAL]
         caching = filesystem_local['caching']
 
         if local_hash_strat not in (
             LOCAL_HASH_STRAT_FILE,
             LOCAL_HASH_STRAT_PATH,
             LOCAL_HASH_STRAT_PATH_MTIME,
+            LOCAL_HASH_START_XXH64,
         ):
             raise ValueError(
                 'Wrong local_hash_strat: {strat}'.format(strat=local_hash_strat)
             )
         caching['hashing-strategy'] = local_hash_strat
 
         if soft_glob_output:
```

### Comparing `caper-2.2.3/caper/cromwell_metadata.py` & `caper-2.3.1/caper/cromwell_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,44 +23,40 @@
 
 def get_workflow_id_from_workflow_root(workflow_root):
     if workflow_root:
         return workflow_root.split('/')[-1]
 
 
 def parse_cromwell_disks(s):
-    """Parses Cromwell's disks in runtime attribute.
-    """
+    """Parses Cromwell's disks in runtime attribute."""
     if s:
         m = re.findall(r'(\d+)', s)
         if m:
             return int(m[0]) * 1024 * 1024 * 1024
 
 
 def parse_cromwell_memory(s):
-    """Parses Cromwell's memory runtime attribute.
-    """
+    """Parses Cromwell's memory runtime attribute."""
     if s:
         return humanfriendly.parse_size(s)
 
 
 def convert_type_np_to_py(o):
-    """Convert numpy type to Python type.
-    """
+    """Convert numpy type to Python type."""
     if isinstance(o, np.generic):
         return o.item()
     raise TypeError
 
 
 class CromwellMetadata:
     DEFAULT_METADATA_BASENAME = 'metadata.json'
     DEFAULT_GCP_MONITOR_STAT_METHODS = ('mean', 'std', 'max', 'min', 'last')
 
     def __init__(self, metadata):
-        """Parses metadata JSON (dict) object or file.
-        """
+        """Parses metadata JSON (dict) object or file."""
         if isinstance(metadata, dict):
             self._metadata = metadata
         elif isinstance(metadata, CromwellMetadata):
             self._metadata = metadata._metadata
         else:
             s = AutoURI(metadata).read()
             self._metadata = json.loads(s)
@@ -155,16 +151,15 @@
                     yield from subworkflow_metadata.recurse_calls(
                         fn_call, parent_call_names=parent_call_names + (call_name,)
                     )
                 else:
                     yield fn_call(call_name, call, parent_call_names)
 
     def write_on_workflow_root(self, basename=DEFAULT_METADATA_BASENAME):
-        """Update metadata JSON file on metadata's output root directory.
-        """
+        """Update metadata JSON file on metadata's output root directory."""
         root = self.workflow_root
 
         if root:
             metadata_file = os.path.join(root, basename)
 
             AutoURI(metadata_file).write(json.dumps(self._metadata, indent=4) + '\n')
             logger.info('Wrote metadata file. {f}'.format(f=metadata_file))
@@ -180,30 +175,31 @@
                 Show STDERR/STDOUT of completed tasks.
             show_stdout:
                 Show failed task's STDOUT along with STDERR.
         Return:
             result:
                 Troubleshooting report as a plain string.
         """
-        result = '* Started troubleshooting workflow: id={id}, status={status}\n'.format(
-            id=self.workflow_id, status=self.workflow_status
+        result = (
+            '* Started troubleshooting workflow: id={id}, status={status}\n'.format(
+                id=self.workflow_id, status=self.workflow_status
+            )
         )
 
         if self.workflow_status == 'Succeeded':
             result += '* Workflow ran Successfully.\n'
 
         else:
             if self.failures:
                 result += '* Found failures JSON object.\n{s}\n'.format(
                     s=json.dumps(self.failures, indent=4)
                 )
 
             def troubleshoot_call(call_name, call, parent_call_names):
-                """Returns troubleshooting help message.
-                """
+                """Returns troubleshooting help message."""
                 nonlocal show_completed_task
                 nonlocal show_stdout
                 status = call.get('executionStatus')
                 shard_index = call.get('shardIndex')
                 rc = call.get('returnCode')
                 job_id = call.get('jobId')
                 stdout = call.get('stdout')
```

### Comparing `caper-2.2.3/caper/cromwell_rest_api.py` & `caper-2.3.1/caper/cromwell_rest_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,16 +489,15 @@
                 if workflow['id'] not in workflow_ids_found_by_labels
             ]
         )
 
         return result
 
     def __init_auth(self):
-        """Init auth object
-        """
+        """Init auth object"""
         if self._user is not None and self._password is not None:
             self._auth = (self._user, self._password)
         else:
             self._auth = None
 
     @requests_error_handler
     def __request_get(self, endpoint, params=None):
```

### Comparing `caper-2.2.3/caper/cromwell_workflow_monitor.py` & `caper-2.3.1/caper/cromwell_workflow_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,16 +220,15 @@
                     self._is_server_started = True
                     if self._on_server_start:
                         self._on_server_start()
                     logger.info('Cromwell server started. Ready to take submissions.')
                     break
 
     def _update_workflows(self, stderr):
-        """Updates workflow status by parsing Cromwell's stderr lines.
-        """
+        """Updates workflow status by parsing Cromwell's stderr lines."""
         updated_workflows = set()
         workflows_to_write_metadata = set()
         for line in stderr.split('\n'):
             for st_transitions in CromwellWorkflowMonitor.ALL_STATUS_TRANSITIONS:
                 workflow_id, status, auto_write_metadata = st_transitions.parse(
                     line, self._workflow_status_map
                 )
@@ -247,16 +246,15 @@
             if r_sub:
                 subworkflow_id = r_sub[0]
                 if subworkflow_id not in self._subworkflows:
                     logger.info('Subworkflow found: {id}'.format(id=subworkflow_id))
                 self._subworkflows.add(subworkflow_id)
 
     def _update_tasks(self, stderr):
-        """Check if workflow's task status changed by parsing Cromwell's stderr lines.
-        """
+        """Check if workflow's task status changed by parsing Cromwell's stderr lines."""
         for line in stderr.split('\n'):
             r_common = None
             r_start = re.findall(CromwellWorkflowMonitor.RE_TASK_START, line)
             if r_start:
                 r_common = r_start[0]
                 status = 'Started'
                 job_id = r_common[4]
@@ -299,16 +297,15 @@
 
     def _find_workflow_id_from_short_id(self, short_id):
         for w in self._subworkflows.union(set(self._workflow_status_map.keys())):
             if w.startswith(short_id):
                 return w
 
     def _write_metadata(self, workflow_id):
-        """Update metadata on Cromwell'e exec root.
-        """
+        """Update metadata on Cromwell'e exec root."""
         if not self._is_server or not self._auto_write_metadata:
             return
         if workflow_id in self._subworkflows and self._embed_subworkflow:
             logger.debug(
                 'Skipped writing metadata JSON file of subworkflow {wf_id}'.format(
                     wf_id=workflow_id
                 )
```

### Comparing `caper-2.2.3/caper/dict_tool.py` & `caper-2.3.1/caper/dict_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         for v in d:
             recurse_dict_value(v, fnc)
     else:
         fnc(d)
 
 
 def unflatten_dict(d_flat):
-    """Unflattens single-level-tuple-keyed dict into dict
-    """
+    """Unflattens single-level-tuple-keyed dict into dict"""
     result = type(d_flat)()
     for k_tuple, v in d_flat.items():
         d_curr = result
         for i, k in enumerate(k_tuple):
             if i == len(k_tuple) - 1:
                 d_curr[k] = v
             elif k not in d_curr:
```

### Comparing `caper-2.2.3/caper/hocon_string.py` & `caper-2.3.1/caper/hocon_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,15 @@
             is_valid_format = True
             break
 
     return is_valid_format
 
 
 def get_include_key(include_str):
-    """Use md5sum hash of the whole include statement string for a key.
-    """
+    """Use md5sum hash of the whole include statement string for a key."""
     return hashlib.md5(include_str.encode()).hexdigest()
 
 
 def wrap_includes(hocon_str):
     """Convert `include` statement string into key = val format.
     Returns '{key} = "{double_quote_escaped_val}"'.
     """
```

### Comparing `caper-2.2.3/caper/hpc.py` & `caper-2.3.1/caper/hpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 """Caper's HPC Wrapper based on job engine's CLI (shell command).
 e.g. sbatch, squeue, qsub, qstat
 """
 import logging
 import os
 import subprocess
 from abc import ABC, abstractmethod
-from collections import namedtuple
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 logger = logging.getLogger(__name__)
 
 CAPER_LEADER_JOB_NAME_PREFIX = 'CAPER_'
 ILLEGAL_CHARS_IN_JOB_NAME = [',', ' ', '\t']
 
 
 def get_user_from_os_environ():
     return os.environ['USER']
 
+
 def make_bash_script_contents(contents):
     return f'#!/bin/bash\n{contents}\n'
 
+
 def make_caper_leader_job_name(job_name):
     """Check if job name contains Comma, TAB or whitespace.
     They are not allowed since they can be used as separators.
     """
-    if any(illegal_char in job_name for illegal_char in ILLEGAL_CHARS_IN_JOB_NAME):
-        raise ValueError('Illegal character {chr} in job name {job}'.format(
-            chr=illegal_chr, job=job_name
-        ))
+    for illegal_char in ILLEGAL_CHARS_IN_JOB_NAME:
+        if illegal_char in job_name:
+            raise ValueError(
+                'Illegal character {chr} in job name {job}'.format(
+                    chr=illegal_char, job=job_name
+                )
+            )
     return CAPER_LEADER_JOB_NAME_PREFIX + job_name
 
 
 class HpcWrapper(ABC):
     def __init__(
         self,
         leader_job_resource_param=[],
     ):
-        """Base class for HPC job engine wrapper.
-        """
+        """Base class for HPC job engine wrapper."""
         self._leader_job_resource_param = leader_job_resource_param
 
     def submit(self, job_name, caper_run_command):
         """Submits a caper leader job to HPC (e.g. sbatch, qsub).
         Such leader job will be prefixed with CAPER_LEADER_JOB_NAME_PREFIX.
 
         Returns output STDOUT from submission command.
@@ -70,40 +73,41 @@
         for line in lines[1:]:
             if CAPER_LEADER_JOB_NAME_PREFIX in line:
                 result.append(line)
 
         return '\n'.join(result)
 
     def abort(self, job_ids):
-        """Returns output STDOUT from job engine's abort command (e.g. scancel, qdel).
-        """
+        """Returns output STDOUT from job engine's abort command (e.g. scancel, qdel)."""
         return self._abort(job_ids)
 
     @abstractmethod
-    def _submit(self, job_name, shell_script):        
+    def _submit(self, job_name, shell_script):
         pass
 
     def _list(self):
         pass
 
     @abstractmethod
     def _abort(self, job_ids):
-        """Sends SIGINT (or SIGTERM) to Caper for a graceful shutdown.
-        """
+        """Sends SIGINT (or SIGTERM) to Caper for a graceful shutdown."""
         pass
 
     def _run_command(self, command):
-        """Runs a shell command line and returns STDOUT.
-        """
+        """Runs a shell command line and returns STDOUT."""
         logger.info(f'Running shell command: {" ".join(command)}')
-        return subprocess.run(
-            command,
-            stdout=subprocess.PIPE,
-            env=os.environ,
-        ).stdout.decode().strip()
+        return (
+            subprocess.run(
+                command,
+                stdout=subprocess.PIPE,
+                env=os.environ,
+            )
+            .stdout.decode()
+            .strip()
+        )
 
 
 class SlurmWrapper(HpcWrapper):
     DEFAULT_LEADER_JOB_RESOURCE_PARAM = ['-t', '48:00:00', '--mem', '4G']
 
     def __init__(
         self,
@@ -115,24 +119,36 @@
             leader_job_resource_param=leader_job_resource_param,
         )
         slurm_partition_param = ['-p', slurm_partition] if slurm_partition else []
         slurm_account_param = ['-A', slurm_account] if slurm_account else []
         self._slurm_extra_param = slurm_partition_param + slurm_account_param
 
     def _submit(self, job_name, shell_script):
-        command = ['sbatch'] + self._leader_job_resource_param + self._slurm_extra_param + [
-            '--export=ALL', '-J', make_caper_leader_job_name(job_name),
-            shell_script,
-        ]
+        command = (
+            ['sbatch']
+            + self._leader_job_resource_param
+            + self._slurm_extra_param
+            + [
+                '--export=ALL',
+                '-J',
+                make_caper_leader_job_name(job_name),
+                shell_script,
+            ]
+        )
         return self._run_command(command)
 
     def _list(self):
-        return self._run_command([
-            'squeue', '-u', get_user_from_os_environ(), '--Format=JobID,Name,State,SubmitTime'
-        ])
+        return self._run_command(
+            [
+                'squeue',
+                '-u',
+                get_user_from_os_environ(),
+                '--Format=JobID,Name,State,SubmitTime',
+            ]
+        )
 
     def _abort(self, job_ids):
         """Notes: --full is necessary to correctly send SIGINT to the leader job (Cromwell process).
         Sending SIGTERM may result in an immediate shutdown of the leaderjob on some clusters.
         SIGINT is much better to trigger a graceful shutdown.
         """
         return self._run_command(['scancel', '--full', '--signal=SIGINT'] + job_ids)
@@ -148,24 +164,24 @@
     ):
         super().__init__(
             leader_job_resource_param=leader_job_resource_param,
         )
         self._sge_queue_param = ['-q', sge_queue] if sge_queue else []
 
     def _submit(self, job_name, shell_script):
-        command = ['qsub'] + self._leader_job_resource_param + self._sge_queue_param + [
-            '-V', '-terse', '-N', make_caper_leader_job_name(job_name),
-            shell_script
-        ]
+        command = (
+            ['qsub']
+            + self._leader_job_resource_param
+            + self._sge_queue_param
+            + ['-V', '-terse', '-N', make_caper_leader_job_name(job_name), shell_script]
+        )
         return self._run_command(command)
 
     def _list(self):
-        return self._run_command([
-            'qstat', '-u', get_user_from_os_environ()
-        ])
+        return self._run_command(['qstat', '-u', get_user_from_os_environ()])
 
     def _abort(self, job_ids):
         return self._run_command(['qdel'] + job_ids)
 
 
 class PbsWrapper(HpcWrapper):
     DEFAULT_LEADER_JOB_RESOURCE_PARAM = ['-l', 'walltime=48:00:00,mem=4gb']
@@ -177,24 +193,24 @@
     ):
         super().__init__(
             leader_job_resource_param=leader_job_resource_param,
         )
         self._pbs_queue_param = ['-q', pbs_queue] if pbs_queue else []
 
     def _submit(self, job_name, shell_script):
-        command = ['qsub'] + self._leader_job_resource_param + self._pbs_queue_param + [
-            '-V', '-N', make_caper_leader_job_name(job_name),
-            shell_script
-        ]
+        command = (
+            ['qsub']
+            + self._leader_job_resource_param
+            + self._pbs_queue_param
+            + ['-V', '-N', make_caper_leader_job_name(job_name), shell_script]
+        )
         return self._run_command(command)
 
     def _list(self):
-        return self._run_command([
-            'qstat', '-u', get_user_from_os_environ()
-        ])
+        return self._run_command(['qstat', '-u', get_user_from_os_environ()])
 
     def _abort(self, job_ids):
         return self._run_command(['qdel', '-W', '30'] + job_ids)
 
 
 class LsfWrapper(HpcWrapper):
     DEFAULT_LEADER_JOB_RESOURCE_PARAM = ['-W', '2880', '-M', '4g']
@@ -206,20 +222,20 @@
     ):
         super().__init__(
             leader_job_resource_param=leader_job_resource_param,
         )
         self._lsf_queue_param = ['-q', lsf_queue] if lsf_queue else []
 
     def _submit(self, job_name, shell_script):
-        command = ['bsub'] + self._leader_job_resource_param + self._lsf_queue_param + [
-            '-env', 'all', '-J', make_caper_leader_job_name(job_name),
-            shell_script
-        ]
+        command = (
+            ['bsub']
+            + self._leader_job_resource_param
+            + self._lsf_queue_param
+            + ['-env', 'all', '-J', make_caper_leader_job_name(job_name), shell_script]
+        )
         return self._run_command(command)
 
     def _list(self):
-        return self._run_command([
-            'bjobs', '-u', get_user_from_os_environ()
-        ])
+        return self._run_command(['bjobs', '-u', get_user_from_os_environ()])
 
     def _abort(self, job_ids):
         return self._run_command(['bkill'] + job_ids)
```

### Comparing `caper-2.2.3/caper/nb_subproc_thread.py` & `caper-2.3.1/caper/nb_subproc_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
-import time
 import signal
+import time
 from subprocess import PIPE, Popen
 from threading import Thread
 
-
 logger = logging.getLogger(__name__)
 interrupted = False
 terminated = False
 
 
 def sigterm_handler(signo, frame):
     global terminated
@@ -177,16 +176,15 @@
         cwd=None,
         stdin=None,
         on_poll=None,
         on_stdout=None,
         on_stderr=None,
         on_finish=None,
     ):
-        """Wrapper for subprocess.Popen().
-        """
+        """Wrapper for subprocess.Popen()."""
         global terminated
         global interrupted
 
         def read_stdout(stdout_bytes):
             text = stdout_bytes.decode()
             if text:
                 self._stdout_list.append(text)
```

### Comparing `caper-2.2.3/caper/resource_analysis.py` & `caper-2.3.1/caper/resource_analysis.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/server_heartbeat.py` & `caper-2.3.1/caper/server_heartbeat.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/singularity.py` & `caper-2.3.1/caper/singularity.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/caper/wdl_parser.py` & `caper-2.3.1/caper/wdl_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 class WDLParser:
     RE_WDL_IMPORT = r'^\s*import\s+[\"\'](.+)[\"\']\s*'
     RECURSION_DEPTH_LIMIT = 20
     BASENAME_IMPORTS = 'imports.zip'
 
     def __init__(self, wdl):
-        """Wraps miniwdl's parse_document().
-        """
+        """Wraps miniwdl's parse_document()."""
         u = AutoURI(wdl)
         if not u.exists:
             raise FileNotFoundError('WDL does not exist: wdl={wdl}'.format(wdl=wdl))
         self._wdl = wdl
         self._wdl_contents = AutoURI(wdl).read()
         try:
             self._wdl_doc = parse_document(self._wdl_contents)
```

### Comparing `caper-2.2.3/caper.egg-info/SOURCES.txt` & `caper-2.3.1/caper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/scripts/gcp_caper_server/create_instance.sh` & `caper-2.3.1/scripts/gcp_caper_server/create_instance.sh`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/setup.py` & `caper-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
     ],
     install_requires=[
         'pyhocon>=0.3.53',
         'requests>=2.20',
         'pyopenssl',
-        'autouri>=0.2.4',
+        'autouri>=0.4.4',
         'miniwdl>=0.7.0',
         'humanfriendly',
         'numpy>=1.8.2',
         'pandas>=1.0',
         'scikit-learn>=0.19.2',
         'matplotlib>=1.5',
         'six>=1.13.0',
```

### Comparing `caper-2.2.3/tests/conftest.py` & `caper-2.3.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 @pytest.fixture(scope='session')
 def ci_prefix(request):
     return request.config.getoption('--ci-prefix').rstrip('/')
 
 
 @pytest.fixture(scope='session')
 def gcs_root(request):
-    """GCS root to generate test GCS URIs on.
-    """
+    """GCS root to generate test GCS URIs on."""
     return request.config.getoption('--gcs-root').rstrip('/')
 
 
 @pytest.fixture(scope='session')
 def cromwell(request):
     return request.config.getoption('--cromwell')
```

### Comparing `caper-2.2.3/tests/example_wdl.py` & `caper-2.3.1/tests/example_wdl.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_arg_tool.py` & `caper-2.3.1/tests/test_arg_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_caper_labels.py` & `caper-2.3.1/tests/test_caper_labels.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_caper_wdl_parser.py` & `caper-2.3.1/tests/test_caper_wdl_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     }
 """
 )
 
 
 def test_properties(tmp_path):
     """Test the following properties.
-        - caper_docker
-        - caper_singularity
+    - caper_docker
+    - caper_singularity
     """
     main_wdl = tmp_path / 'main.wdl'
     main_wdl.write_text(WDL_CONTENTS)
 
     old_wdl = tmp_path / 'old_main.wdl'
     old_wdl.write_text(OLD_WDL_CONTENTS)
```

### Comparing `caper-2.2.3/tests/test_caper_workflow_opts.py` & `caper-2.3.1/tests/test_caper_workflow_opts.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import pytest
 
 from caper.caper_workflow_opts import CaperWorkflowOpts
 from caper.cromwell_backend import BACKEND_AWS, BACKEND_GCP
 
 
 def test_create_file(tmp_path):
-    """Test without docker/singularity.
-    """
+    """Test without docker/singularity."""
     use_google_cloud_life_sciences = False
     gcp_zones = ['us-west-1', 'us-west-2']
     slurm_partition = 'my_partition'
     slurm_account = 'my_account'
     slurm_extra_param = 'my_extra_param'
     sge_pe = 'my_pe'
     sge_queue = 'my_queue'
@@ -131,16 +130,15 @@
         d = json.loads(fp.read())
 
     dra = d[CaperWorkflowOpts.DEFAULT_RUNTIME_ATTRIBUTES]
     assert 'zones' not in dra
 
 
 def test_create_file_docker(tmp_path):
-    """Test with docker and docker defined in WDL.
-    """
+    """Test with docker and docker defined in WDL."""
     wdl_contents = dedent(
         """\
         version 1.0
         workflow test_docker {
             meta {
                 caper_docker: "ubuntu:latest"
             }
@@ -201,16 +199,15 @@
     with open(f_local2) as fp:
         d_local2 = json.loads(fp.read())
         dra_local2 = d_local2[CaperWorkflowOpts.DEFAULT_RUNTIME_ATTRIBUTES]
     assert dra_local2['docker'] == 'ubuntu:16'
 
 
 def test_create_file_singularity(tmp_path):
-    """Test with singularity and singularity defined in WDL.
-    """
+    """Test with singularity and singularity defined in WDL."""
     wdl_contents = dedent(
         """\
         version 1.0
         workflow test_singularity {
             meta {
                 default_docker: "ubuntu:latest"
                 default_singularity: "docker://ubuntu:latest"
```

### Comparing `caper-2.2.3/tests/test_cli_run.py` & `caper-2.3.1/tests/test_cli_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     cmd = ['run', str(tmp_path / 'main.wdl')] + cmd
     with pytest.raises(ValueError):
         cli_main(cmd)
 
 
 @pytest.mark.integration
 def test_run(tmp_path, cromwell, womtool, debug_caper):
-    """Will test most local parameters (run only) here.
-    """
+    """Will test most local parameters (run only) here."""
     make_directory_with_wdls(str(tmp_path))
     wdl = tmp_path / 'main.wdl'
     inputs = tmp_path / 'inputs.json'
     p = WDLParser(str(wdl))
     imports = p.zip_subworkflows(str(tmp_path / 'imports.zip'))
 
     cmd = ['run']
@@ -112,16 +111,15 @@
     ci_prefix,
     cromwell,
     womtool,
     gcp_prj,
     gcp_service_account_key_json,
     debug_caper,
 ):
-    """Test run with Google Cloud Life Sciences API
-    """
+    """Test run with Google Cloud Life Sciences API"""
     out_gcs_bucket = os.path.join(gcs_root, 'caper_out', ci_prefix)
     tmp_gcs_bucket = os.path.join(gcs_root, 'caper_tmp')
 
     # prepare WDLs and input JSON, imports to be submitted
     make_directory_with_wdls(str(tmp_path))
     wdl = tmp_path / 'main.wdl'
     inputs = tmp_path / 'inputs.json'
```

### Comparing `caper-2.2.3/tests/test_cli_server_client_gcp.py` & `caper-2.3.1/tests/test_cli_server_client_gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     ci_prefix,
     cromwell,
     womtool,
     gcp_prj,
     gcp_service_account_key_json,
     debug_caper,
 ):
-    """Test server, client stuffs
-    """
+    """Test server, client stuffs"""
     # server command line
     server_port = 8015
 
     out_gcs_bucket = os.path.join(gcs_root, 'caper_out', ci_prefix)
     tmp_gcs_bucket = os.path.join(gcs_root, 'caper_tmp')
 
     cmd = ['server']
```

### Comparing `caper-2.2.3/tests/test_cromwell.py` & `caper-2.3.1/tests/test_cromwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,15 @@
         )
     finally:
         th.join()
     assert th.returncode == 0
 
 
 def test_server(tmp_path, cromwell, womtool):
-    """Test Cromwell.server() method, which returns a Thread object.
-    """
+    """Test Cromwell.server() method, which returns a Thread object."""
     server_port = 8005
     fileobj_stdout = sys.stdout
 
     c = Cromwell(cromwell=cromwell, womtool=womtool)
 
     o_dir = tmp_path / 'output'
     o_dir.mkdir()
```

### Comparing `caper-2.2.3/tests/test_cromwell_backend.py` & `caper-2.3.1/tests/test_cromwell_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     - CromwellBackendBase
 
 """
 from caper.cromwell_backend import CromwellBackendBase
 
 
 def test_cromwell_backend_base_backend():
-    """Test a property backend's getter, setter
-    """
+    """Test a property backend's getter, setter"""
     bb1 = CromwellBackendBase('test1')
     backend_dict = {'a': 1, 'b': '2'}
 
     bb1.backend = backend_dict
     assert bb1.backend == backend_dict
```

### Comparing `caper-2.2.3/tests/test_cromwell_metadata.py` & `caper-2.3.1/tests/test_cromwell_metadata.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_cromwell_rest_api.py` & `caper-2.3.1/tests/test_cromwell_rest_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     ],
 )
 def test_has_wildcard(test_input, expected):
     assert has_wildcard(test_input) == expected
 
 
 def test_all(tmp_path, cromwell, womtool):
-    """Test Cromwell.server() method, which returns a Thread object.
-    """
+    """Test Cromwell.server() method, which returns a Thread object."""
     server_port = 8010
     fileobj_stdout = sys.stdout
     test_label = 'test_label'
 
     c = Cromwell(cromwell=cromwell, womtool=womtool)
 
     o_dir = tmp_path / 'output'
```

### Comparing `caper-2.2.3/tests/test_dict_tool.py` & `caper-2.3.1/tests/test_dict_tool.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_hocon_string.py` & `caper-2.3.1/tests/test_hocon_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,15 @@
             'HOCONSTRING_INCLUDE_ad5c3c187d5107c099f66681f1896c70'
         ] = 'include required(classpath("application"))'
 
     return base_dict
 
 
 def get_test_dict2():
-    """Without "include" lines.
-    """
+    """Without "include" lines."""
     return {'backend': {'providers': {'gcp': {'actor-factory': 'GOOGLE'}}}}
 
 
 def get_test_multiple_includes(with_include=False):
     if with_include:
         return {
             "HOCONSTRING_INCLUDE_ad5c3c187d5107c099f66681f1896c70": "include required(classpath(\"application\"))",
```

### Comparing `caper-2.2.3/tests/test_nb_subproc_thread.py` & `caper-2.3.1/tests/test_nb_subproc_thread.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_resource_analysis.py` & `caper-2.3.1/tests/test_resource_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,15 @@
             3749246230,
             3749246230,
         ]
     }
 
 
 def test_resource_analysis_analyze(gcp_res_analysis_metadata):
-    """Test method analyze() which analyze all tasks defined in in_file_vars.
-    """
+    """Test method analyze() which analyze all tasks defined in in_file_vars."""
     analysis = LinearResourceAnalysis()
     analysis.collect_resource_data([gcp_res_analysis_metadata])
 
     result = analysis.analyze(
         in_file_vars={
             'atac.align*': ['fastqs_R1', 'fastqs_R2'],
             'atac.filter*': ['bam'],
```

### Comparing `caper-2.2.3/tests/test_server_heartbeat.py` & `caper-2.3.1/tests/test_server_heartbeat.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_singularity.py` & `caper-2.3.1/tests/test_singularity.py`

 * *Files identical despite different names*

### Comparing `caper-2.2.3/tests/test_wdl_parser.py` & `caper-2.3.1/tests/test_wdl_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     MAIN_WDL_PARAMETER_META_DICT,
     make_directory_with_wdls,
 )
 
 
 def test_properties(tmp_path):
     """Test the following properties.
-        - contents
-        - workflow_meta
-        - workflow_parameter_meta
-        - imports
+    - contents
+    - workflow_meta
+    - workflow_parameter_meta
+    - imports
     """
     wdl = tmp_path / 'main.wdl'
     wdl.write_text(MAIN_WDL)
 
     wp = WDLParser(str(wdl))
     assert wp.contents == MAIN_WDL
     assert wp.workflow_meta == MAIN_WDL_META_DICT
```

