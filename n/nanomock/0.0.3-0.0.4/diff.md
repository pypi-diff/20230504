# Comparing `tmp/nanomock-0.0.3.tar.gz` & `tmp/nanomock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomock-0.0.3.tar", last modified: Wed May  3 13:15:57 2023, max compression
+gzip compressed data, was "nanomock-0.0.4.tar", last modified: Thu May  4 20:56:09 2023, max compression
```

## Comparing `nanomock-0.0.3.tar` & `nanomock-0.0.4.tar`

### file list

```diff
@@ -1,72 +1,87 @@
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       44 2023-05-02 13:35:20.000000 nanomock-0.0.3/MANIFEST.in
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-03 13:15:57.513888 nanomock-0.0.3/PKG-INFO
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.3/README.md
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       22 2023-05-03 09:31:09.000000 nanomock-0.0.3/nanomock/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 11:22:58.000000 nanomock-0.0.3/nanomock/internal/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:05.000000 nanomock-0.0.3/nanomock/internal/data/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:25.000000 nanomock-0.0.3/nanomock/internal/data/services/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      432 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/custom_Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      297 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/default_config-node.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      298 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/default_config-node_voting-disabled.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      220 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/default_config-rpc.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1824 2023-05-03 07:50:15.000000 nanomock-0.0.3/nanomock/internal/data/services/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/nanolooker/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      960 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/nanolooker/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:55.000000 nanomock-0.0.3/nanomock/internal/data/services/nanolooker/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.3/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/nanomonitor/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:59.000000 nanomock-0.0.3/nanomock/internal/data/services/nanomonitor/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      659 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/nanomonitor/default_config.php
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      354 2023-05-03 09:06:45.000000 nanomock-0.0.3/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/nanoticker/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/nanoticker/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:02.000000 nanomock-0.0.3/nanomock/internal/data/services/nanoticker/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      466 2023-05-03 12:43:51.000000 nanomock-0.0.3/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      768 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:05.000000 nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      503 2023-05-03 12:43:54.000000 nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      325 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/promexporter/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      323 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:14.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1551 2023-05-03 12:44:47.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      420 2023-05-03 12:44:11.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.509888 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      132 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      515 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/promexporter/prometheus.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/internal/data/services/tcpdump/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      119 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/tcpdump/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:10.000000 nanomock-0.0.3/nanomock/internal/data/services/tcpdump/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      223 2023-05-03 09:06:45.000000 nanomock-0.0.3/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      685 2023-04-27 20:34:19.000000 nanomock-0.0.3/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.3/nanomock/internal/dependency_checker.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.3/nanomock/internal/nl_block_tools.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.3/nanomock/internal/nl_initialise.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     5215 2023-05-03 12:39:12.000000 nanomock-0.0.3/nanomock/internal/utils.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1539 2023-05-02 22:39:42.000000 nanomock-0.0.3/nanomock/main.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock/modules/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-04-27 15:36:50.000000 nanomock-0.0.3/nanomock/modules/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.3/nanomock/modules/nl_nanolib.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    43786 2023-05-03 12:58:29.000000 nanomock-0.0.3/nanomock/modules/nl_parse_config.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.3/nanomock/modules/nl_rpc.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    20055 2023-05-03 12:59:51.000000 nanomock-0.0.3/nanomock/nanomock_manager.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-03 13:15:57.513888 nanomock-0.0.3/nanomock.egg-info/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/PKG-INFO
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2599 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/SOURCES.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        1 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/dependency_links.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       48 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/entry_points.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       54 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/requires.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        9 2023-05-03 13:15:57.000000 nanomock-0.0.3/nanomock.egg-info/top_level.txt
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)       38 2023-05-03 13:15:57.513888 nanomock-0.0.3/setup.cfg
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      784 2023-05-03 12:52:55.000000 nanomock-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 20:56:09.832810 nanomock-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 20:43:16.000000 nanomock-0.0.4/nanomock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/docker/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.4/nanomock/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.4/nanomock/docker/autoheal.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.4/nanomock/docker/interface.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.4/nanomock/docker/linux.py
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.4/nanomock/docker/macos.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.4/nanomock/docker/mixin.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.4/nanomock/docker/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.4/nanomock/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.4/nanomock/internal/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.4/nanomock/internal/data/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/custom_Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-node.toml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-node_voting-disabled.toml
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-rpc.toml
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-05-03 07:50:15.000000 nanomock-0.0.4/nanomock/internal/data/services/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_config.php
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.4/nanomock/internal/dependency_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.4/nanomock/internal/feature_toggle.py
+-rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.4/nanomock/internal/nl_block_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.4/nanomock/internal/nl_initialise.py
+-rw-r--r--   0 root         (0) root         (0)     5550 2023-05-04 19:25:42.000000 nanomock-0.0.4/nanomock/internal/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-02 22:39:42.000000 nanomock-0.0.4/nanomock/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.4/nanomock/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.4/nanomock/modules/nl_nanolib.py
+-rw-rw-r--   0 root         (0) root         (0)    44005 2023-05-04 20:39:39.000000 nanomock-0.0.4/nanomock/modules/nl_parse_config.py
+-rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.4/nanomock/modules/nl_rpc.py
+-rw-rw-r--   0 root         (0) root         (0)    16991 2023-05-04 20:40:20.000000 nanomock-0.0.4/nanomock/nanomock_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/os_operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/interface.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/linux.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/macos.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-04 19:05:01.000000 nanomock-0.0.4/nanomock/os_operations/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 20:56:09.832810 nanomock-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-04 20:43:01.000000 nanomock-0.0.4/setup.py
```

### Comparing `nanomock-0.0.3/PKG-INFO` & `nanomock-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.3/README.md` & `nanomock-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/default_docker-compose.yml` & `nanomock-0.0.4/nanomock/internal/data/services/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/nanolooker/Dockerfile` & `nanomock-0.0.4/nanomock/internal/data/services/nanolooker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/nanolooker/default_docker-compose.yml` & `nanomock-0.0.4/nanomock/internal/data/services/nanolooker/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/nanomonitor/default_config.php` & `nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_config.php`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/nanoticker/Dockerfile` & `nanomock-0.0.4/nanomock/internal/data/services/nanoticker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/nanovotevisu/Dockerfile` & `nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/promexporter/default_docker-compose.yml` & `nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_docker-compose.yml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - 42091:9091
 
   nl_prometheus:
     image: prom/prometheus:latest
     container_name: nl_prometheus
     restart: unless-stopped
     volumes:
-      - services/promexporter/prometheus.yml:/etc/prometheus/prometheus.yml
+      - ./services/promexporter/prometheus.yml:/etc/prometheus/prometheus.yml
       - nl_prometheus_data:/prometheus
     # tmpfs: /prometheus:uid=99
     command:
       - '--web.enable-admin-api'
       - '--config.file=/etc/prometheus/prometheus.yml'
       - '--storage.tsdb.path=/prometheus'
       - '--web.console.libraries=/etc/prometheus/console_libraries'
@@ -48,15 +48,15 @@
     user: "472"
     depends_on:
       - nl_prometheus
     ports:
       - 42005:3000
     volumes:
       - nl_grafana_data:/var/lib/grafana
-      - services/promexporter/grafana/provisioning/:/etc/grafana/provisioning/
+      - ./services/promexporter/grafana/provisioning/:/etc/grafana/provisioning/
       # env_file:
       # - ./grafana/config.monitoring
     networks:
       - nano-local
 
 volumes:
   nl_grafana_data: { name: nl_grafana_data}
```

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json` & `nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml` & `nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/promexporter/prometheus.yml` & `nanomock-0.0.4/nanomock/internal/data/services/promexporter/prometheus.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json` & `nanomock-0.0.4/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/dependency_checker.py` & `nanomock-0.0.4/nanomock/internal/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/nl_block_tools.py` & `nanomock-0.0.4/nanomock/internal/nl_block_tools.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/nl_initialise.py` & `nanomock-0.0.4/nanomock/internal/nl_initialise.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/internal/utils.py` & `nanomock-0.0.4/nanomock/internal/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,17 +160,28 @@
     with resources.path("nanomock", "__init__.py") as src_dir:
         src_dir = src_dir.parent / "internal" / "data" / "services"
         dest_dir = destination_path / "services"
 
         if src_dir.exists():
             dest_dir.mkdir(parents=True, exist_ok=True)
             shutil.copytree(src_dir, dest_dir, dirs_exist_ok=True)
-            print(
+            logger.info(
                 "nanomock data has been copied to your current working directory."
             )
         else:
-            print("Error: nanomock data not found.")
+            logger.error("Error: nanomock data not found.")
 
 
 def shutil_rmtree(path: Path):
     shutil.rmtree(path)
-    return f"Removed directory: {path}"
+    return f"Removed directory: {path}"
+
+
+def subprocess_run_capture_output(cmd, shell=True, cwd=None):
+
+    result = subprocess.run(cmd,
+                            shell=shell,
+                            check=True,
+                            capture_output=True,
+                            text=True,
+                            cwd=cwd)
+    return result
```

### Comparing `nanomock-0.0.3/nanomock/main.py` & `nanomock-0.0.4/nanomock/main.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/modules/nl_nanolib.py` & `nanomock-0.0.4/nanomock/modules/nl_nanolib.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/modules/nl_parse_config.py` & `nanomock-0.0.4/nanomock/modules/nl_parse_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import subprocess
 import tomli
 import tomli_w
 import oyaml as yaml
 import secrets
 import json
@@ -13,26 +12,28 @@
 from nanolib import Block
 from extradict import NestedData
 from pathlib import Path
 from importlib import resources
 
 from nanomock.modules.nl_nanolib import NanoLibTools, raw_high_precision_multiply
 from nanomock.modules.nl_rpc import NanoRpc
-from nanomock.internal.utils import read_from_package_if_needed, is_packaged_version, find_device_for_path, convert_to_bytes
+from nanomock.internal.utils import read_from_package_if_needed, is_packaged_version, find_device_for_path, convert_to_bytes, NanoLocalLogger
+from nanomock.internal.feature_toggle import toggle
+from nanomock.docker import get_docker_interface_class
 
 
 def str2bool(v):
     return str(v).lower() in ("yes", "true", "t", "1")
 
 
 class ConfigReadWrite:
 
     def __init__(self, config_path, logger=None):
         if logger is None:
-            self.logger = logging.getLogger(__name__)
+            self.logger = NanoLocalLogger.get_logger(__name__)
         if not os.path.exists(config_path):
             raise FileExistsError(config_path)
 
     @read_from_package_if_needed
     def read_json(self, path, is_packaged=False):
         with open(path, "r") as f:
             return json.load(f)
@@ -85,16 +86,15 @@
 
 
 class ConfigParser:
 
     preconfigured_peers = []
 
     def __init__(self, app_dir, config_file=None, logger=None):
-        if logger is None:
-            self.logger = logging.getLogger(__name__)
+        self.logger = logger or NanoLocalLogger.get_logger(__name__)
 
         self.enabled_services = []
         self._set_path_variables(app_dir, config_file)
         self.conf_rw = ConfigReadWrite(self.nl_config_path)
         self.nano_lib = NanoLibTools()
         self.config_dict = self.conf_rw.read_toml(self.nl_config_path)
         self.compose_dict = self.conf_rw.read_yaml(self.default_compose_path,
@@ -496,15 +496,19 @@
         if as_json:
             return json.loads(json_block)
 
         return json_block
 
     def get_node_rpc(self, node_name):
         node_conf = self.get_node_config(node_name)
-        return node_conf["rpc_url"]
+        if node_conf:
+            return node_conf["rpc_url"]
+        raise ValueError(
+            f"{node_name} undefined in {self.nl_config_path}\nValid names:{self.get_nodes_name()}"
+        )
 
     def get_nodes_rpc(self):
         api = []
         for node_name in self.get_nodes_name():
             node_conf = self.get_node_config(node_name)
             api.append(node_conf["rpc_url"])
         return api
@@ -743,32 +747,33 @@
             host_port_monitor = 46000 + host_port_inc
             self.enabled_services.append(
                 f'nano-node-monitor enabled at {self.get_config_value("remote_address")}:{host_port_monitor}'
             )
             host_port_inc = host_port_inc + 1
 
     def set_promexporter_compose(self):
+        DockerInterfaceClass = get_docker_interface_class()
+        host_ip = DockerInterfaceClass.get_docker_gateway_ip()
 
-        host_ip = self.get_config_value("remote_address")
-        if host_ip == '127.0.0.1':
-            raise ValueError(
-                "Please configure remote_address in nl_config.toml if you set promexporter_enable == True"
-            )
         #Create prometheus, prom-gateway and grafana IF we use default prom-gateway
         if self.get_config_value("prom_gateway") == "nl_pushgateway:9091":
             promexporter_compose = self.conf_rw.read_yaml(
                 f'{self.services_dir}/promexporter/default_docker-compose.yml',
                 is_packaged=True)
             for container in promexporter_compose["services"]:
                 self.compose_dict["services"][
                     container] = promexporter_compose["services"][container]
             for volume in promexporter_compose["volumes"]:
                 self.compose_dict["volumes"][volume] = promexporter_compose[
                     "volumes"][volume]
 
+            self.enabled_services.append(
+                f'promgateway enabled at {self.get_config_value("remote_address")}:42005'
+            )
+
         #Create 1 exporter per node
         for node in self.config_dict["representatives"]["nodes"]:
             node_config = self.get_node_config(node["name"])
             node_rpc_port = node_config["host_port_rpc"]
 
             prom_gateway = self.get_config_value("prom_gateway")
             prom_runid = self.get_config_value("prom_runid")
@@ -789,18 +794,14 @@
 
             self.compose_dict["services"][container_name][
                 "pid"] = f'service:{node["name"]}'
 
             self.enabled_services.append(
                 f'{container_name} added for node {node["name"]}')
 
-        self.enabled_services.append(
-            f'promexporter enabled at {self.get_config_value("remote_address")}:42005'
-        )
-
     def set_tcpdump_compose(self):
 
         tcp_analyzer_config_path = f'{self.tcp_analyzer_path}/config.json'
         if not os.path.exists(tcp_analyzer_config_path):
             conf_source_path = f'{self.services_dir}/tcpdump/tcp_analyzer_config.example.json'
             copy_conf = f'cp -p {conf_source_path} {tcp_analyzer_config_path}'
             os.system(copy_conf)
@@ -891,14 +892,15 @@
                 "device_read_iops": "100",
                 "device_write_iops": "100",
             },
         }
         return disk_defaults.get(disk_type.upper(), None)
 
     def add_container_blkio_config(self, container, node_name):
+        if toggle.is_feature_disabled("config_blkio"): return
         blkio_config = {}
         config_tags = [
             "device_read_bps",
             "device_write_bps",
             "device_read_iops",
             "device_write_iops",
         ]
```

### Comparing `nanomock-0.0.3/nanomock/modules/nl_rpc.py` & `nanomock-0.0.4/nanomock/modules/nl_rpc.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.3/nanomock/nanomock_manager.py` & `nanomock-0.0.4/nanomock/nanomock_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import re
 import subprocess
 import logging
 from typing import List, Optional
 from .internal.dependency_checker import DependencyChecker
 from .modules.nl_parse_config import ConfigParser
 from .internal.nl_initialise import InitialBlocks
+from .docker import create_docker_interface
 from .modules.nl_rpc import NanoRpc
-from .internal.utils import log_on_success, NanoLocalLogger, shutil_rmtree, extract_packaged_services_to_disk
+from .internal.utils import log_on_success, NanoLocalLogger, shutil_rmtree, extract_packaged_services_to_disk, subprocess_run_capture_output
 from typing import List, Dict, Optional, Tuple, Union
 import concurrent.futures
 from math import floor
 import yaml
 import json
 import time
 import inspect
@@ -19,31 +20,34 @@
 logger = NanoLocalLogger.get_logger(__name__)
 
 
 class NanoLocalManager:
 
     def __init__(self, dir_path, project_name):
         self.command_mapping = self._initialize_command_mapping()
-        self.dir_path = dir_path
+        self.conf_p = ConfigParser(dir_path, logger=logger)
         self.dependency_checker = DependencyChecker()
         self.dependency_checker.check_dependencies()
-        self.conf_p = ConfigParser(dir_path, logger=logger)
 
+        self.dir_path = dir_path
         self.nano_nodes_path = self.conf_p.nano_nodes_path
         self.compose_yml_path = self.conf_p.compose_out_path
         self.compose_env_path = os.path.join(self.nano_nodes_path,
                                              "dc_nano_local_env")
         self.project_name = project_name
         self.services_dir = self.conf_p.services_dir
         self.nodes_data_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest"
         self.config_node_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest/config-node.toml"
         self.config_rpc_path = f"{self.nano_nodes_path}/{{node_name}}/NanoTest/config-rpc.toml"
 
         os.makedirs(self.nano_nodes_path, exist_ok=True)
 
+        self.docker_interface = create_docker_interface(
+            self.compose_yml_path, self.project_name)
+
     def _initialize_command_mapping(self):
         #(command_method , validation_method)
         return {
             'create': (self.create_docker_compose_file, None),
             'start': (self.start_containers, None),
             'status': (self.network_status, None),
             'restart': (self.restart_containers, None),
@@ -52,46 +56,14 @@
             'stop': (self.stop_containers, None),
             'remove': (self.remove_containers, None),
             'down': (self.remove_containers, None),
             'destroy': (lambda: self.destroy(remove_files=True), None),
             'rpc': (self.run_rpc, self._rpc_validator)
         }
 
-    def _subprocess_capture_raise(self,
-                                  cmd,
-                                  shell=True,
-                                  cwd=None,
-                                  increment=0):
-        #Capture output to stdout or raise CalledProcessError if the command returns a non-zero exit code
-        try:
-            result = subprocess.run(cmd,
-                                    shell=shell,
-                                    check=True,
-                                    capture_output=True,
-                                    text=True,
-                                    cwd=cwd)
-
-            #print(str.join(" ", [str(e) for e in cmd]))
-            return result
-        except subprocess.CalledProcessError as e:
-            response = self.auto_heal(e, shell, cwd, increment)
-            return response
-
-    def _run_docker_compose_command(self,
-                                    command,
-                                    nodes: Optional[List[str]] = None):
-        base_command = [
-            "docker-compose", "-f", self.compose_yml_path, "-p",
-            self.project_name
-        ]
-        base_command.extend(command)
-        if nodes: base_command.extend(nodes)
-
-        return self._subprocess_capture_raise(base_command, shell=False)
-
     def _get_default(self, config_name):
         """ Load config with default values"""
         #minimal node config if no file is provided in the nl_config.toml
         if config_name == "config_node":
             default_config_path = os.path.join(self.services_dir,
                                                "default_config-node.toml")
             return self.conf_p.conf_rw.read_toml(default_config_path,
@@ -165,15 +137,15 @@
         self._generate_config_rpc_file(node_name)
         self._generate_nanomonitor_config_file(node_name)
 
     def _online_containers(self, node_names: List[str]) -> List[str]:
         online_containers = []
         for container in node_names:
             cmd = f"docker ps |grep {container}$ | wc -l"
-            res = self._subprocess_capture_raise(cmd)
+            res = subprocess_run_capture_output(cmd)
             online = int(res.stdout.strip())
 
             if online == 1:
                 online_containers.append(container)
 
         return online_containers
 
@@ -189,14 +161,16 @@
         nodes_rpc = ([
             NanoRpc(self.conf_p.get_node_rpc(node)) for node in nodes_name
         ] if nodes_name is not None else self._get_all_rpc())
 
         for nano_rpc in nodes_rpc:
             block_count = nano_rpc.block_count()
             version_rpc_call = nano_rpc.version()
+            if not (block_count or version_rpc_call):
+                continue
             node_name = self.conf_p.get_node_name_from_rpc_url(nano_rpc)
             count = int(block_count["count"])
             nodes_block_count.append({
                 "node_name": node_name,
                 "count": count,
                 "cemented": block_count["cemented"],
                 "version": version_rpc_call
@@ -378,110 +352,57 @@
     @log_on_success
     def reset_nodes_data(self, nodes: Optional[List[str]] = None):
         self.stop_containers(nodes)
         nodes_to_process = nodes or ['.']
         for node in nodes_to_process:
             node_path = f'{self.nano_nodes_path}/{node}' if nodes else self.nano_nodes_path
             cmd = 'rm -f $(find . -name "*.ldb")'
-            self._subprocess_capture_raise(cmd, node_path)
+            subprocess_run_capture_output(cmd, node_path)
 
     def init_containers(self):
         self.create_docker_compose_file()
         self.build_containers()
 
     @log_on_success
     def restart_containers(self, nodes: Optional[List[str]] = None):
-        self._run_docker_compose_command(["restart"], nodes)
+        return self.docker_interface.compose_restart(nodes)
 
     @log_on_success
     def build_containers(self):
-        self._run_docker_compose_command(["build"])
+        return self.docker_interface.compose_build()
 
     @log_on_success
     def start_containers(self, nodes: Optional[List[str]] = None):
-        self._run_docker_compose_command(["up", "-d"], nodes)
+        self.docker_interface.compose_start(nodes)
         self._wait_for_rpc_availability(nodes)
 
     @log_on_success
     def stop_containers(self, nodes: Optional[List[str]] = None):
-        self._run_docker_compose_command(["stop"], nodes)
+        self.docker_interface.compose_stop(nodes)
 
     @log_on_success
     def remove_containers(self):
-        self._run_docker_compose_command(["down"])
+        self.docker_interface.compose_down()
 
     @log_on_success
     def destroy(self, remove_files=False):
         # Stop and remove containers
         self.remove_containers()
 
         # Remove the created files and folders if remove_files is True
         if remove_files:
             return shutil_rmtree(self.nano_nodes_path)
 
     @log_on_success
     def update(self):
-        self._run_docker_compose_command(["pull"])
+        self.docker_interface.compose_pull()
         # Remove containers and networks
         self.remove_containers()
         self.build_containers()
 
-    def auto_heal(self,
-                  error: subprocess.CalledProcessError,
-                  cmd_shell,
-                  cmd_cwd,
-                  increment=0):
-        if increment >= 10:
-            raise (error)
-
-        stderr = error.stderr
-        healable_errors = {
-            "address_in_use": ("programming external connectivity on endpoint",
-                               self._heal_address_in_use),
-            "docker_in_use":
-            ("Error response from daemon: Conflict. The container name",
-             self._heal_docker_in_use),
-        }
-
-        for error_key, (error_msg, heal_func) in healable_errors.items():
-            if error_msg not in stderr:
-                continue
-
-            logger.warning(
-                f"Retry attempt {increment}... {error_key}: \n {stderr}")
-
-            if heal_func(error_msg, stderr):
-                increment += 1
-                return self._subprocess_capture_raise(error.cmd,
-                                                      cmd_shell,
-                                                      cmd_cwd,
-                                                      increment=increment)
-
-        raise ValueError(error.stderr)
-        raise (error)
-
-    def _heal_address_in_use(self, error_msg, stderr):
-        container_name = re.search(r"{} (\w+)".format(error_msg),
-                                   stderr).group(1)
-        self._subprocess_capture_raise(
-            f"docker stop -t 0 {container_name} && sleep 5 && docker start {container_name}",
-            shell=True)
-        return True
-
-    def _heal_docker_in_use(self, error_msg, stderr):
-        pattern = r'{} "/([^"]+)"'.format(error_msg)
-        match = re.search(pattern, stderr)
-        if match:
-            container_name = match.group(1)
-            self._subprocess_capture_raise(
-                f"docker stop -t 0 {container_name} && docker rm {container_name} && sleep 5",
-                shell=True)
-            return True
-        return False
-
     def _filter_args(self, func, **kwargs):
         sig = inspect.signature(func)
         filtered_args = {
             k: v
             for k, v in kwargs.items() if k in sig.parameters
         }
         return filtered_args
```

### Comparing `nanomock-0.0.3/nanomock.egg-info/PKG-INFO` & `nanomock-0.0.4/nanomock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.3/nanomock.egg-info/SOURCES.txt` & `nanomock-0.0.4/nanomock.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 nanomock/nanomock_manager.py
 nanomock.egg-info/PKG-INFO
 nanomock.egg-info/SOURCES.txt
 nanomock.egg-info/dependency_links.txt
 nanomock.egg-info/entry_points.txt
 nanomock.egg-info/requires.txt
 nanomock.egg-info/top_level.txt
+nanomock/docker/__init__.py
+nanomock/docker/autoheal.py
+nanomock/docker/interface.py
+nanomock/docker/linux.py
+nanomock/docker/macos.py
+nanomock/docker/mixin.py
+nanomock/docker/windows.py
 nanomock/internal/__init__.py
 nanomock/internal/dependency_checker.py
+nanomock/internal/feature_toggle.py
 nanomock/internal/nl_block_tools.py
 nanomock/internal/nl_initialise.py
 nanomock/internal/utils.py
 nanomock/internal/data/__init__.py
 nanomock/internal/data/services/__init__.py
 nanomock/internal/data/services/custom_Dockerfile
 nanomock/internal/data/services/default_config-node.toml
@@ -46,8 +54,13 @@
 nanomock/internal/data/services/tcpdump/Dockerfile
 nanomock/internal/data/services/tcpdump/__init__.py
 nanomock/internal/data/services/tcpdump/default_docker-compose.yml
 nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
 nanomock/modules/__init__.py
 nanomock/modules/nl_nanolib.py
 nanomock/modules/nl_parse_config.py
-nanomock/modules/nl_rpc.py
+nanomock/modules/nl_rpc.py
+nanomock/os_operations/__init__.py
+nanomock/os_operations/interface.py
+nanomock/os_operations/linux.py
+nanomock/os_operations/macos.py
+nanomock/os_operations/mixin.py
```

### Comparing `nanomock-0.0.3/setup.py` & `nanomock-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanomock",
-      version="0.0.3",
+      version="0.0.4",
       author="gr0vity",
       description="Create local dockerized nano-currency networks",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanomock",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

