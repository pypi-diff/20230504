# Comparing `tmp/openmldb-exporter-0.6.0.tar.gz` & `tmp/openmldb_exporter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmldb-exporter-0.6.0.tar", max compression
+gzip compressed data, was "openmldb_exporter-0.7.0.tar", max compression
```

## Comparing `openmldb-exporter-0.6.0.tar` & `openmldb_exporter-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     4674 2022-05-25 06:38:38.125134 openmldb-exporter-0.6.0/README.md
--rw-r--r--   0        0        0      107 2022-05-25 06:38:38.125860 openmldb-exporter-0.6.0/openmldb_exporter/__init__.py
--rw-r--r--   0        0        0      969 2022-05-25 06:38:38.126689 openmldb-exporter-0.6.0/openmldb_exporter/collector/__init__.py
--rw-r--r--   0        0        0     6315 2022-08-25 07:37:35.268347 openmldb-exporter-0.6.0/openmldb_exporter/collector/collectors.py
--rw-r--r--   0        0        0     2857 2022-05-25 06:38:38.127331 openmldb-exporter-0.6.0/openmldb_exporter/collector/configstore.py
--rw-r--r--   0        0        0     2911 2022-05-25 06:38:38.127784 openmldb-exporter-0.6.0/openmldb_exporter/collector/metrics.py
--rw-r--r--   0        0        0     2306 2022-08-25 07:37:35.268678 openmldb-exporter-0.6.0/openmldb_exporter/exporter.py
--rw-r--r--   0        0        0     1036 2022-08-25 07:37:35.270740 openmldb-exporter-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5664 2022-08-25 07:38:20.036656 openmldb-exporter-0.6.0/setup.py
--rw-r--r--   0        0        0     5603 2022-08-25 07:38:20.037541 openmldb-exporter-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5598 2023-05-04 17:02:50.645029 openmldb_exporter-0.7.0/README.md
+-rw-r--r--   0        0        0      107 2023-05-04 05:10:31.217764 openmldb_exporter-0.7.0/openmldb_exporter/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-04 05:10:31.218447 openmldb_exporter-0.7.0/openmldb_exporter/collector/__init__.py
+-rw-r--r--   0        0        0      903 2023-05-04 05:10:31.218696 openmldb_exporter-0.7.0/openmldb_exporter/collector/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5464 2023-05-04 05:10:31.218894 openmldb_exporter-0.7.0/openmldb_exporter/collector/__pycache__/collectors.cpython-310.pyc
+-rw-r--r--   0        0        0     2449 2023-05-04 05:10:31.219070 openmldb_exporter-0.7.0/openmldb_exporter/collector/__pycache__/configstore.cpython-310.pyc
+-rw-r--r--   0        0        0     1902 2023-05-04 05:10:31.219234 openmldb_exporter-0.7.0/openmldb_exporter/collector/__pycache__/metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     6320 2023-05-04 05:10:31.219431 openmldb_exporter-0.7.0/openmldb_exporter/collector/collectors.py
+-rw-r--r--   0        0        0     2857 2023-05-04 05:10:31.219588 openmldb_exporter-0.7.0/openmldb_exporter/collector/configstore.py
+-rw-r--r--   0        0        0     2911 2023-05-04 05:10:31.219779 openmldb_exporter-0.7.0/openmldb_exporter/collector/metrics.py
+-rw-r--r--   0        0        0     2306 2023-05-04 05:10:31.219987 openmldb_exporter-0.7.0/openmldb_exporter/exporter.py
+-rw-r--r--   0        0        0     1113 2023-05-04 16:54:49.791949 openmldb_exporter-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6628 1970-01-01 00:00:00.000000 openmldb_exporter-0.7.0/PKG-INFO
```

### Comparing `openmldb-exporter-0.6.0/README.md` & `openmldb_exporter-0.7.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,62 +6,90 @@
 ## Intro
 
 This directory contains
 
 1. OpenMLDB Exporter exposing prometheus metrics
 2. OpenMLDB mixin provides well-configured examples for prometheus server and grafana dashboard
 
-Supported versions:
+## Requirements
+
+- A runnable OpenMLDB instance that is accessible from your network
+- OpenMLDB version >= 0.5.0
+- Python >= 3.8
+
+
+## Setup
+
+For those want to try, simply install from pip, it will install the latest release:
+
+```bash
+pip install openmldb-exporter
+```
+
+Then type
+
+```sh
+openmldb-exporter -h
+```
+
+To see which flags should provided.
+
+Developers may refer [Development](#development) for how to setup openmldb exporter from source code.
 
-+ OpenMLDB >= 0.5.0
 
 ## Development
 
-### Requirements
+### Extra Requirements
 
-- Python >= 3.8 
+- Same in [Requirements](#requirements)
 - [poetry](https://github.com/python-poetry/poetry) as build tool
 - cmake (optional if want to test latest commit)
-- a runnable OpenMLDB instance that is accessible from your network
 
-### Build
+### Build python SDK (Optional)
 
-The exporter is a python project, the only thing need to built was the native library required by python sdk. To build, `cd` to root directory of OpenMLDB, and run:
+openmldb exporter depends on [openmldb python SDK](https://pypi.org/project/openmldb/). For those introducing changes in python SDK or native code as well, this steps is required in order to take the latest Python SDK locally instead of the published one.
+
+#### 1. Build native code
+
+`cd` to root directory of OpenMLDB, and run:
 
 ```bash
 make SQL_PYSDK_ENABLE=ON
 ```
 
-Note: build is only required when tesing over latest commit is needed, otherwise, it can installed directly from pip (when 0.5.0 released):
+This will generate compiled shared library in `python` source directory.
 
-```bash
-pip install openmldb-exporter==0.5.0
+#### 2. Fix dependency list
+
+Back to openmldb exporter directory, modify `pyproject.toml` and make content like below:
+
+```toml
+[tool.poetry.dependencies]
+# ...
+# openmldb = "^0.6.0"
+# uncomment below to use openmldb sdk built from source
+# set develop = true so changes in python will take effect immediately
+openmldb = { path = "../python/", develop = true }
 ```
 
 ### Run
 
-1. setup python dependencies:
+1. Setup python dependencies:
 
    ```bash
    poetry install
    ```
 
-2. enter virtual environment
-
-   ```bash
-   poetry shell
-   ```
-
-3. start openmldb exporter
+2. Start openmldb exporter
 
    ```bash
    poetry run openmldb-exporter
    ```
 
-   you need pass necessary flags after `openmldb-exporter`. run `poetry run openmldb-exporter --help` to get the help info
+   You need pass necessary flags after `openmldb-exporter`. Run `poetry run openmldb-exporter --help` to get the help info
 
    ```bash
    usage: openmldb-exporter [-h] [--log.level LOG.LEVEL] [--web.listen-address WEB.LISTEN_ADDRESS]
                             [--web.telemetry-path WEB.TELEMETRY_PATH] [--config.zk_root CONFIG.ZK_ROOT]
                             [--config.zk_path CONFIG.ZK_PATH] [--config.interval CONFIG.INTERVAL]
    
    OpenMLDB exporter
@@ -78,21 +106,21 @@
                            endpoint to zookeeper, default 127.0.0.1:6181
      --config.zk_path CONFIG.ZK_PATH
                            root path in zookeeper for OpenMLDB, default /
      --config.interval CONFIG.INTERVAL
                            interval in seconds to pull metrics periodically, default 30.0
    ```
 
-4. view the available metrics, you can pull through `curl`
+3. View the available metrics, you can pull through `curl`
 
    ```bash
    curl http://127.0.0.1:8000/metrics
    ```
 
-   a example output:
+   A example output:
 
    ```bash
    # HELP openmldb_connected_seconds_total duration for a component conncted time in seconds                              
    # TYPE openmldb_connected_seconds_total counter                                                                        
    openmldb_connected_seconds_total{endpoint="172.17.0.15:9520",role="tablet"} 208834.70900011063                         
    openmldb_connected_seconds_total{endpoint="172.17.0.15:9521",role="tablet"} 208834.70700001717                         
    openmldb_connected_seconds_total{endpoint="172.17.0.15:9522",role="tablet"} 208834.71399998665                         
@@ -104,7 +132,15 @@
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9520",role="tablet"} 1.6501813860467942e+09                   
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9521",role="tablet"} 1.6501813860495396e+09                   
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9522",role="tablet"} 1.650181386050323e+09                    
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9622",role="nameserver"} 1.6501813860512116e+09               
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9623",role="nameserver"} 1.650181386051238e+09                
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9624",role="nameserver"} 1.6501813860512598e+09               
    ```
+
+## Release History
+
+- 0.7.0
+    * Features
+        - Depends OpenMLDB SDK v0.7.x
+    * Bug fixes
+        - Integral metric overflow: https://github.com/4paradigm/OpenMLDB/pull/3003
```

### Comparing `openmldb-exporter-0.6.0/openmldb_exporter/collector/__init__.py` & `openmldb_exporter-0.7.0/openmldb_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `openmldb-exporter-0.6.0/openmldb_exporter/collector/collectors.py` & `openmldb_exporter-0.7.0/openmldb_exporter/collector/collectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
         for row in rows:
             logging.debug(row)
 
             # TODO: use storage_type
             tid, tb_name, db_name, storage_type, rows, mem, disk, partition, partition_unalive, replica, *_ = row
             tb_path = f"{db_name}_{tb_name}"
             tid = int(tid)
-            table_rows.labels(tb_path, tid, storage_type).set(int(rows))
+            table_rows.labels(tb_path, tid, storage_type).set(long(rows))
             table_partitions.labels(tb_path, tid, storage_type).set(int(partition))
             table_partitions_unalive.labels(tb_path, tid, storage_type).set(int(partition_unalive))
             table_replica.labels(tb_path, tid, storage_type).set(int(replica))
-            table_memory.labels(tb_path, tid, storage_type).set(int(mem))
+            table_memory.labels(tb_path, tid, storage_type).set(long(mem))
             table_disk.labels(tb_path, tid, storage_type).set(int(disk))
 
 
 class DeployQueryStatCollector(Collector, SDKConnectable):
     '''
     deploy query statistics collector
     '''
@@ -93,15 +93,15 @@
             dp_name, time_second, count, total = row
             time_second = float(time_second)
 
             # update bucket count
             for i, bound in enumerate(deploy_response_time._upper_bounds):
                 if time_second <= bound:
                     # FIXME: handle Histogram reset correctly
-                    deploy_response_time.labels(dp_name)._buckets[i].set(int(count))
+                    deploy_response_time.labels(dp_name)._buckets[i].set(long(count))
                     break
             # update sum for each deploy
             if dp_name in acc_map:
                 acc_map[dp_name] += float(total)
             else:
                 acc_map[dp_name] = float(total)
             row = rs.fetchone()
@@ -157,20 +157,20 @@
         memory_acutal_used = 0
         # http request with 1s timeout
         with request.urlopen(url, timeout=1) as resp:
             for i in resp:
                 line = i.decode().strip()
                 if line.rfind("use by application") > 0:
                     try:
-                        memory_by_application = int(line.split()[1])
+                        memory_by_application = long(line.split()[1])
                     except ValueError as e:
                         memory_by_application = 0
                         logging.error(e)
                 elif line.rfind("Actual memory used") > 0:
                     try:
-                        memory_acutal_used = int(line.split()[2])
+                        memory_acutal_used = long(line.split()[2])
                     except ValueError as e:
                         memory_acutal_used = 0
                         logging.error(e)
                 else:
                     continue
         return memory_by_application, memory_acutal_used
```

### Comparing `openmldb-exporter-0.6.0/openmldb_exporter/collector/configstore.py` & `openmldb_exporter-0.7.0/openmldb_exporter/collector/configstore.py`

 * *Files identical despite different names*

### Comparing `openmldb-exporter-0.6.0/openmldb_exporter/collector/metrics.py` & `openmldb_exporter-0.7.0/openmldb_exporter/collector/metrics.py`

 * *Files identical despite different names*

### Comparing `openmldb-exporter-0.6.0/openmldb_exporter/exporter.py` & `openmldb_exporter-0.7.0/openmldb_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `openmldb-exporter-0.6.0/pyproject.toml` & `openmldb_exporter-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmldb-exporter"
-version = "0.6.0"
+version = "0.7.0"
 description = "prometheus exporter for OpenMLDB"
 authors = ["aceforeverd <teapot@aceforeverd.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://openmldb.ai"
 repository = "https://github.com/4paradigm/OpenMLDB"
 documentation = "https://openmldb.ai/docs/zh/main/maintain/monitoring.html"
@@ -16,20 +16,24 @@
 ]
 
 [tool.poetry.scripts]
 openmldb-exporter = "openmldb_exporter.exporter:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-prometheus-client = "^0.14.1"
-openmldb = "^0.6.0"
+prometheus-client = "^0.16.0"
+openmldb = "^0.7.0"
 # uncomment below to use openmldb sdk built from source
 # set develop = true so changes in python will take effect immediately
 # openmldb = { path = "../python/", develop = true }
 Twisted = "^22.2.0"
 
 [tool.poetry.dev-dependencies]
-pylint = "^2.13.4"
+pylint = "^2.17.3"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+requests = "^2.29.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openmldb-exporter-0.6.0/setup.py` & `openmldb_exporter-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,173 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openmldb-exporter
+Version: 0.7.0
+Summary: prometheus exporter for OpenMLDB
+Home-page: https://openmldb.ai
+License: Apache-2.0
+Keywords: openmldb,prometheus
+Author: aceforeverd
+Author-email: teapot@aceforeverd.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Database
+Classifier: Topic :: System :: Monitoring
+Requires-Dist: Twisted (>=22.2.0,<23.0.0)
+Requires-Dist: openmldb (>=0.7.0,<0.8.0)
+Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
+Project-URL: Documentation, https://openmldb.ai/docs/zh/main/maintain/monitoring.html
+Project-URL: Repository, https://github.com/4paradigm/OpenMLDB
+Description-Content-Type: text/markdown
+
+# OpenMLDB Prometheus Exporter
+
+[![PyPI](https://img.shields.io/pypi/v/openmldb-exporter?label=openmldb-exporter)](https://pypi.org/project/openmldb-exporter/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmldb-exporter)
+
+## Intro
+
+This directory contains
+
+1. OpenMLDB Exporter exposing prometheus metrics
+2. OpenMLDB mixin provides well-configured examples for prometheus server and grafana dashboard
+
+## Requirements
+
+- A runnable OpenMLDB instance that is accessible from your network
+- OpenMLDB version >= 0.5.0
+- Python >= 3.8
+
+
+## Setup
+
+For those want to try, simply install from pip, it will install the latest release:
+
+```bash
+pip install openmldb-exporter
+```
+
+Then type
+
+```sh
+openmldb-exporter -h
+```
+
+To see which flags should provided.
+
+Developers may refer [Development](#development) for how to setup openmldb exporter from source code.
+
+
+## Development
+
+### Extra Requirements
+
+- Same in [Requirements](#requirements)
+- [poetry](https://github.com/python-poetry/poetry) as build tool
+- cmake (optional if want to test latest commit)
+
+### Build python SDK (Optional)
+
+openmldb exporter depends on [openmldb python SDK](https://pypi.org/project/openmldb/). For those introducing changes in python SDK or native code as well, this steps is required in order to take the latest Python SDK locally instead of the published one.
+
+#### 1. Build native code
+
+`cd` to root directory of OpenMLDB, and run:
+
+```bash
+make SQL_PYSDK_ENABLE=ON
+```
+
+This will generate compiled shared library in `python` source directory.
+
+#### 2. Fix dependency list
+
+Back to openmldb exporter directory, modify `pyproject.toml` and make content like below:
+
+```toml
+[tool.poetry.dependencies]
+# ...
+# openmldb = "^0.6.0"
+# uncomment below to use openmldb sdk built from source
+# set develop = true so changes in python will take effect immediately
+openmldb = { path = "../python/", develop = true }
+```
+
+### Run
+
+1. Setup python dependencies:
+
+   ```bash
+   poetry install
+   ```
+
+2. Start openmldb exporter
+
+   ```bash
+   poetry run openmldb-exporter
+   ```
+
+   You need pass necessary flags after `openmldb-exporter`. Run `poetry run openmldb-exporter --help` to get the help info
+
+   ```bash
+   usage: openmldb-exporter [-h] [--log.level LOG.LEVEL] [--web.listen-address WEB.LISTEN_ADDRESS]
+                            [--web.telemetry-path WEB.TELEMETRY_PATH] [--config.zk_root CONFIG.ZK_ROOT]
+                            [--config.zk_path CONFIG.ZK_PATH] [--config.interval CONFIG.INTERVAL]
+   
+   OpenMLDB exporter
+   
+   optional arguments:
+     -h, --help            show this help message and exit
+     --log.level LOG.LEVEL
+                           config log level, default WARN
+     --web.listen-address WEB.LISTEN_ADDRESS
+                           process listen port, default 8000
+     --web.telemetry-path WEB.TELEMETRY_PATH
+                           Path under which to expose metrics, default metrics
+     --config.zk_root CONFIG.ZK_ROOT
+                           endpoint to zookeeper, default 127.0.0.1:6181
+     --config.zk_path CONFIG.ZK_PATH
+                           root path in zookeeper for OpenMLDB, default /
+     --config.interval CONFIG.INTERVAL
+                           interval in seconds to pull metrics periodically, default 30.0
+   ```
+
+3. View the available metrics, you can pull through `curl`
+
+   ```bash
+   curl http://127.0.0.1:8000/metrics
+   ```
+
+   A example output:
+
+   ```bash
+   # HELP openmldb_connected_seconds_total duration for a component conncted time in seconds                              
+   # TYPE openmldb_connected_seconds_total counter                                                                        
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9520",role="tablet"} 208834.70900011063                         
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9521",role="tablet"} 208834.70700001717                         
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9522",role="tablet"} 208834.71399998665                         
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9622",role="nameserver"} 208833.70000004768                     
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9623",role="nameserver"} 208831.70900011063                     
+   openmldb_connected_seconds_total{endpoint="172.17.0.15:9624",role="nameserver"} 208829.7230000496                      
+   # HELP openmldb_connected_seconds_created duration for a component conncted time in seconds                            
+   # TYPE openmldb_connected_seconds_created gauge                                                                        
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9520",role="tablet"} 1.6501813860467942e+09                   
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9521",role="tablet"} 1.6501813860495396e+09                   
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9522",role="tablet"} 1.650181386050323e+09                    
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9622",role="nameserver"} 1.6501813860512116e+09               
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9623",role="nameserver"} 1.650181386051238e+09                
+   openmldb_connected_seconds_created{endpoint="172.17.0.15:9624",role="nameserver"} 1.6501813860512598e+09               
+   ```
+
+## Release History
+
+- 0.7.0
+    * Features
+        - Depends OpenMLDB SDK v0.7.x
+    * Bug fixes
+        - Integral metric overflow: https://github.com/4paradigm/OpenMLDB/pull/3003
 
-packages = \
-['openmldb_exporter', 'openmldb_exporter.collector']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Twisted>=22.2.0,<23.0.0',
- 'openmldb>=0.6.0,<0.7.0',
- 'prometheus-client>=0.14.1,<0.15.0']
-
-entry_points = \
-{'console_scripts': ['openmldb-exporter = openmldb_exporter.exporter:main']}
-
-setup_kwargs = {
-    'name': 'openmldb-exporter',
-    'version': '0.6.0',
-    'description': 'prometheus exporter for OpenMLDB',
-    'long_description': '# OpenMLDB Prometheus Exporter\n\n[![PyPI](https://img.shields.io/pypi/v/openmldb-exporter?label=openmldb-exporter)](https://pypi.org/project/openmldb-exporter/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmldb-exporter)\n\n## Intro\n\nThis directory contains\n\n1. OpenMLDB Exporter exposing prometheus metrics\n2. OpenMLDB mixin provides well-configured examples for prometheus server and grafana dashboard\n\nSupported versions:\n\n+ OpenMLDB >= 0.5.0\n\n## Development\n\n### Requirements\n\n- Python >= 3.8 \n- [poetry](https://github.com/python-poetry/poetry) as build tool\n- cmake (optional if want to test latest commit)\n- a runnable OpenMLDB instance that is accessible from your network\n\n### Build\n\nThe exporter is a python project, the only thing need to built was the native library required by python sdk. To build, `cd` to root directory of OpenMLDB, and run:\n\n```bash\nmake SQL_PYSDK_ENABLE=ON\n```\n\nNote: build is only required when tesing over latest commit is needed, otherwise, it can installed directly from pip (when 0.5.0 released):\n\n```bash\npip install openmldb-exporter==0.5.0\n```\n\n### Run\n\n1. setup python dependencies:\n\n   ```bash\n   poetry install\n   ```\n\n2. enter virtual environment\n\n   ```bash\n   poetry shell\n   ```\n\n3. start openmldb exporter\n\n   ```bash\n   poetry run openmldb-exporter\n   ```\n\n   you need pass necessary flags after `openmldb-exporter`. run `poetry run openmldb-exporter --help` to get the help info\n\n   ```bash\n   usage: openmldb-exporter [-h] [--log.level LOG.LEVEL] [--web.listen-address WEB.LISTEN_ADDRESS]\n                            [--web.telemetry-path WEB.TELEMETRY_PATH] [--config.zk_root CONFIG.ZK_ROOT]\n                            [--config.zk_path CONFIG.ZK_PATH] [--config.interval CONFIG.INTERVAL]\n   \n   OpenMLDB exporter\n   \n   optional arguments:\n     -h, --help            show this help message and exit\n     --log.level LOG.LEVEL\n                           config log level, default WARN\n     --web.listen-address WEB.LISTEN_ADDRESS\n                           process listen port, default 8000\n     --web.telemetry-path WEB.TELEMETRY_PATH\n                           Path under which to expose metrics, default metrics\n     --config.zk_root CONFIG.ZK_ROOT\n                           endpoint to zookeeper, default 127.0.0.1:6181\n     --config.zk_path CONFIG.ZK_PATH\n                           root path in zookeeper for OpenMLDB, default /\n     --config.interval CONFIG.INTERVAL\n                           interval in seconds to pull metrics periodically, default 30.0\n   ```\n\n4. view the available metrics, you can pull through `curl`\n\n   ```bash\n   curl http://127.0.0.1:8000/metrics\n   ```\n\n   a example output:\n\n   ```bash\n   # HELP openmldb_connected_seconds_total duration for a component conncted time in seconds                              \n   # TYPE openmldb_connected_seconds_total counter                                                                        \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9520",role="tablet"} 208834.70900011063                         \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9521",role="tablet"} 208834.70700001717                         \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9522",role="tablet"} 208834.71399998665                         \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9622",role="nameserver"} 208833.70000004768                     \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9623",role="nameserver"} 208831.70900011063                     \n   openmldb_connected_seconds_total{endpoint="172.17.0.15:9624",role="nameserver"} 208829.7230000496                      \n   # HELP openmldb_connected_seconds_created duration for a component conncted time in seconds                            \n   # TYPE openmldb_connected_seconds_created gauge                                                                        \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9520",role="tablet"} 1.6501813860467942e+09                   \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9521",role="tablet"} 1.6501813860495396e+09                   \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9522",role="tablet"} 1.650181386050323e+09                    \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9622",role="nameserver"} 1.6501813860512116e+09               \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9623",role="nameserver"} 1.650181386051238e+09                \n   openmldb_connected_seconds_created{endpoint="172.17.0.15:9624",role="nameserver"} 1.6501813860512598e+09               \n   ```\n',
-    'author': 'aceforeverd',
-    'author_email': 'teapot@aceforeverd.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://openmldb.ai',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

