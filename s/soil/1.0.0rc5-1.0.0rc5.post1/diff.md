# Comparing `tmp/soil-1.0.0rc5.tar.gz` & `tmp/soil-1.0.0rc5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil-1.0.0rc5.tar", last modified: Thu May  4 10:01:04 2023, max compression
+gzip compressed data, was "soil-1.0.0rc5.post1.tar", last modified: Thu May  4 11:13:21 2023, max compression
```

## Comparing `soil-1.0.0rc5.tar` & `soil-1.0.0rc5.post1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.640427 soil-1.0.0rc5/
--rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc5/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc5/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)     5739 2023-05-04 10:01:04.640427 soil-1.0.0rc5/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc5/README.md
--rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-24 16:44:33.000000 soil-1.0.0rc5/requirements.txt
--rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-04 10:01:04.640427 soil-1.0.0rc5/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc5/setup.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.632428 soil-1.0.0rc5/soil/
--rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc5/soil/.VERSION.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc5/soil/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc5/soil/.analysis.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc5/soil/.datacollection.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    37698 2023-04-29 12:20:51.000000 soil-1.0.0rc5/soil/.environment.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc5/soil/.events.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc5/soil/.exporters.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc5/soil/.serialization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc5/soil/.simulation.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc5/soil/.stats.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)   185860 2023-04-27 15:33:19.000000 soil-1.0.0rc5/soil/.time.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc5/soil/.utils.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc5/soil/.visualization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)        9 2023-05-04 10:00:56.000000 soil-1.0.0rc5/soil/VERSION
--rw-rw-r--   0 j         (1000) j         (1000)     7899 2023-05-04 09:48:46.000000 soil-1.0.0rc5/soil/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/__main__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/agents/
--rw-rw-r--   0 j         (1000) j         (1000)    82293 2023-04-27 07:13:41.000000 soil-1.0.0rc5/soil/agents/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc5/soil/agents/.evented.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    61000 2023-04-27 07:10:51.000000 soil-1.0.0rc5/soil/agents/.fsm.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc5/soil/agents/.network_agents.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/agents/BassModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/agents/CounterModel.py
--rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/agents/IndependentCascadeModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/agents/SISaModel.py
--rw-rw-r--   0 j         (1000) j         (1000)    20411 2023-05-02 22:04:24.000000 soil-1.0.0rc5/soil/agents/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1814 2023-05-02 17:48:59.000000 soil-1.0.0rc5/soil/agents/evented.py
--rw-rw-r--   0 j         (1000) j         (1000)     4891 2023-05-02 22:14:42.000000 soil-1.0.0rc5/soil/agents/fsm.py
--rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc5/soil/agents/geo.py
--rw-rw-r--   0 j         (1000) j         (1000)     3420 2023-04-25 03:00:06.000000 soil-1.0.0rc5/soil/agents/network_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2434 2023-05-02 17:39:42.000000 soil-1.0.0rc5/soil/analysis.py
--rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/config.py
--rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc5/soil/datacollection.py
--rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/debugging.py
--rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/decorators.py
--rw-rw-r--   0 j         (1000) j         (1000)    15501 2023-05-04 09:46:28.000000 soil-1.0.0rc5/soil/environment.py
--rw-rw-r--   0 j         (1000) j         (1000)      541 2023-04-25 22:09:53.000000 soil-1.0.0rc5/soil/events.py
--rw-rw-r--   0 j         (1000) j         (1000)     9048 2023-05-02 17:55:40.000000 soil-1.0.0rc5/soil/exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/network.py
--rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/parameters.py
--rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc5/soil/serialization.py
--rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc5/soil/settings.py
--rw-rw-r--   0 j         (1000) j         (1000)    13043 2023-05-02 20:14:49.000000 soil-1.0.0rc5/soil/simulation.py
--rw-rw-r--   0 j         (1000) j         (1000)     5101 2023-05-04 10:00:23.000000 soil-1.0.0rc5/soil/time.py
--rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/utils.py
--rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/version.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/
--rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc5/soil/web/.gitignore
--rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc5/soil/web/README.md
--rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/web/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/web/__main__.py
--rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/web/config.yml
--rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc5/soil/web/run.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.628428 soil-1.0.0rc5/soil/web/static/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/static/css/
--rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc5/soil/web/static/css/main.css
--rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc5/soil/web/static/css/timeline.css
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/static/img/
--rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/logo_gsi.svg
--rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/logo_soil.png
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/static/img/svg/
--rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/svg/home.svg
--rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/svg/person.svg
--rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/svg/plus.svg
--rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/svg/target.svg
--rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/img/svg/time.svg
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/static/js/
--rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/js/socket.js
--rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/js/template.js
--rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/js/timeline.js
--rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/static/js/visualization.js
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.636427 soil-1.0.0rc5/soil/web/templates/
--rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc5/soil/web/templates/index.html
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.632428 soil-1.0.0rc5/soil.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     5739 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2123 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) j         (1000)      292 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-04 10:01:04.000000 soil-1.0.0rc5/soil.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc5/test-requirements.txt
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 10:01:04.640427 soil-1.0.0rc5/tests/
--rw-rw-r--   0 j         (1000) j         (1000)    11851 2023-05-02 19:21:49.000000 soil-1.0.0rc5/tests/test_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc5/tests/test_config.py
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc5/tests/test_examples.py
--rw-rw-r--   0 j         (1000) j         (1000)     3761 2023-04-27 16:08:44.000000 soil-1.0.0rc5/tests/test_exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc5/tests/test_ipython.py
--rw-rw-r--   0 j         (1000) j         (1000)     7561 2023-05-02 15:39:46.000000 soil-1.0.0rc5/tests/test_main.py
--rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc5/tests/test_mesa.py
--rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc5/tests/test_network.py
--rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc5/tests/test_time.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/
+-rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc5.post1/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc5.post1/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)     5751 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4655 2023-04-24 16:43:50.000000 soil-1.0.0rc5.post1/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-24 16:44:33.000000 soil-1.0.0rc5.post1/requirements.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      191 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     2211 2023-04-24 16:05:52.000000 soil-1.0.0rc5.post1/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.264182 soil-1.0.0rc5.post1/soil/
+-rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc5.post1/soil/.VERSION.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc5.post1/soil/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc5.post1/soil/.analysis.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     3720 2023-04-26 07:50:45.000000 soil-1.0.0rc5.post1/soil/.datacollection.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    37698 2023-04-29 12:20:51.000000 soil-1.0.0rc5.post1/soil/.environment.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13143 2023-04-25 22:09:53.000000 soil-1.0.0rc5.post1/soil/.events.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc5.post1/soil/.exporters.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc5.post1/soil/.serialization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc5.post1/soil/.simulation.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc5.post1/soil/.stats.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)   185860 2023-04-27 15:33:19.000000 soil-1.0.0rc5.post1/soil/.time.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    32688 2023-04-21 14:21:10.000000 soil-1.0.0rc5.post1/soil/.utils.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc5.post1/soil/.visualization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)       15 2023-05-04 11:13:12.000000 soil-1.0.0rc5.post1/soil/VERSION
+-rw-rw-r--   0 j         (1000) j         (1000)     7899 2023-05-04 09:48:46.000000 soil-1.0.0rc5.post1/soil/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/__main__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/agents/
+-rw-rw-r--   0 j         (1000) j         (1000)    82293 2023-04-27 07:13:41.000000 soil-1.0.0rc5.post1/soil/agents/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    59903 2023-04-25 23:21:25.000000 soil-1.0.0rc5.post1/soil/agents/.evented.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    61000 2023-04-27 07:10:51.000000 soil-1.0.0rc5.post1/soil/agents/.fsm.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5801 2023-04-25 03:00:06.000000 soil-1.0.0rc5.post1/soil/agents/.network_agents.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/BassModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/CounterModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/IndependentCascadeModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/agents/SISaModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)    20467 2023-05-04 10:45:09.000000 soil-1.0.0rc5.post1/soil/agents/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1814 2023-05-02 17:48:59.000000 soil-1.0.0rc5.post1/soil/agents/evented.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5408 2023-05-04 11:04:55.000000 soil-1.0.0rc5.post1/soil/agents/fsm.py
+-rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-29 09:53:33.000000 soil-1.0.0rc5.post1/soil/agents/geo.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3420 2023-04-25 03:00:06.000000 soil-1.0.0rc5.post1/soil/agents/network_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2434 2023-05-02 17:39:42.000000 soil-1.0.0rc5.post1/soil/analysis.py
+-rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/config.py
+-rw-rw-r--   0 j         (1000) j         (1000)      853 2023-04-26 07:50:45.000000 soil-1.0.0rc5.post1/soil/datacollection.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/debugging.py
+-rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/decorators.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15695 2023-05-04 10:22:08.000000 soil-1.0.0rc5.post1/soil/environment.py
+-rw-rw-r--   0 j         (1000) j         (1000)      541 2023-04-25 22:09:53.000000 soil-1.0.0rc5.post1/soil/events.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9048 2023-05-02 17:55:40.000000 soil-1.0.0rc5.post1/soil/exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/network.py
+-rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/parameters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8070 2023-04-29 09:32:04.000000 soil-1.0.0rc5.post1/soil/serialization.py
+-rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc5.post1/soil/settings.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13043 2023-05-02 20:14:49.000000 soil-1.0.0rc5.post1/soil/simulation.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5247 2023-05-04 11:12:52.000000 soil-1.0.0rc5.post1/soil/time.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/utils.py
+-rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/version.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/
+-rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/.gitignore
+-rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/__main__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/config.yml
+-rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/soil/web/run.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.260182 soil-1.0.0rc5.post1/soil/web/static/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/css/
+-rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/static/css/main.css
+-rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc5.post1/soil/web/static/css/timeline.css
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/img/
+-rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/logo_gsi.svg
+-rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/logo_soil.png
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/img/svg/
+-rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/home.svg
+-rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/person.svg
+-rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/plus.svg
+-rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/target.svg
+-rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/img/svg/time.svg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/static/js/
+-rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/socket.js
+-rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/template.js
+-rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/timeline.js
+-rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/static/js/visualization.js
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.268182 soil-1.0.0rc5.post1/soil/web/templates/
+-rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc5.post1/soil/web/templates/index.html
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.264182 soil-1.0.0rc5.post1/soil.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     5751 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     2123 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       78 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/entry_points.txt
+-rw-r--r--   0 j         (1000) j         (1000)      292 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2023-05-04 11:13:21.000000 soil-1.0.0rc5.post1/soil.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       90 2023-04-24 17:04:44.000000 soil-1.0.0rc5.post1/test-requirements.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-05-04 11:13:21.272182 soil-1.0.0rc5.post1/tests/
+-rw-rw-r--   0 j         (1000) j         (1000)    11851 2023-05-02 19:21:49.000000 soil-1.0.0rc5.post1/tests/test_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2231 2023-04-25 13:22:59.000000 soil-1.0.0rc5.post1/tests/test_config.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_examples.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3761 2023-04-27 16:08:44.000000 soil-1.0.0rc5.post1/tests/test_exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)      636 2023-04-24 16:55:59.000000 soil-1.0.0rc5.post1/tests/test_ipython.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8511 2023-05-04 11:04:12.000000 soil-1.0.0rc5.post1/tests/test_main.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_mesa.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 12:27:50.000000 soil-1.0.0rc5.post1/tests/test_network.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1549 2023-05-02 15:39:46.000000 soil-1.0.0rc5.post1/tests/test_time.py
```

### Comparing `soil-1.0.0rc5/LICENSE` & `soil-1.0.0rc5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/PKG-INFO` & `soil-1.0.0rc5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc5
+Version: 1.0.0rc5.post1
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.post1.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc5/README.md` & `soil-1.0.0rc5.post1/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/setup.py` & `soil-1.0.0rc5.post1/setup.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.analysis.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.analysis.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.datacollection.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.datacollection.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.environment.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.environment.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.events.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.events.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.exporters.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.exporters.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.serialization.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.serialization.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.simulation.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.simulation.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.stats.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.stats.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.time.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.time.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/.utils.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/.utils.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/__init__.py` & `soil-1.0.0rc5.post1/soil/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/.__init__.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/agents/.__init__.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/.evented.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/agents/.evented.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/.fsm.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/agents/.fsm.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/.network_agents.py.~undo-tree~` & `soil-1.0.0rc5.post1/soil/agents/.network_agents.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/BassModel.py` & `soil-1.0.0rc5.post1/soil/agents/BassModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/CounterModel.py` & `soil-1.0.0rc5.post1/soil/agents/CounterModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/IndependentCascadeModel.py` & `soil-1.0.0rc5.post1/soil/agents/IndependentCascadeModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/SISaModel.py` & `soil-1.0.0rc5.post1/soil/agents/SISaModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/__init__.py` & `soil-1.0.0rc5.post1/soil/agents/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,18 +678,23 @@
 
 from .network_agents import *
 from .fsm import *
 from .evented import *
 from typing import Optional
 
 
-class Agent(NetworkAgent, FSM, EventedAgent):
+class Agent(FSM, EventedAgent, NetworkAgent):
     """Default agent class, has both network and event capabilities"""
 
 
+class Noop(Agent):
+    def step(self):
+        return
+
+
 from ..environment import NetworkEnvironment
 
 
 from .BassModel import *
 from .IndependentCascadeModel import *
 from .SISaModel import *
 from .CounterModel import *
```

### Comparing `soil-1.0.0rc5/soil/agents/evented.py` & `soil-1.0.0rc5.post1/soil/agents/evented.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/fsm.py` & `soil-1.0.0rc5.post1/soil/agents/fsm.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,18 @@
                 f"No default state specified for {type(self)}({self.unique_id})"
             )
         for (k, v) in self._states.items():
             setattr(self, k, v.bind(self))
 
         if init:
             self.init()
+        if not self._state and (self.step == FSM.step):
+            raise ValueError(
+                f"No default state specified for {type(self)}({self.unique_id})"
+            )
 
     @classmethod
     def states(cls):
         return list(cls._states.keys())
 
     @property
     def state_id(self):
@@ -136,14 +140,20 @@
     
     def set_state(self, value):
         if self.now > 0:
             raise ValueError("Cannot change state after init")
         self._set_state(value)
 
     def step(self):
+        if self._state is None:
+            if len(self._states) == 1:
+                raise Exception("Agent class has no valid states: {}. Make sure to define states or define a custom step function".format(self.__class__.__name__))
+            else:
+                raise Exception("Invalid state (None) for agent {}".format(self))
+
         self._check_alive()
         next_state = yield from self._state.step(self)
 
         try:
             next_state, when = next_state
         except (TypeError, ValueError) as ex:
             try:
```

### Comparing `soil-1.0.0rc5/soil/agents/geo.py` & `soil-1.0.0rc5.post1/soil/agents/geo.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/agents/network_agents.py` & `soil-1.0.0rc5.post1/soil/agents/network_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/analysis.py` & `soil-1.0.0rc5.post1/soil/analysis.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/datacollection.py` & `soil-1.0.0rc5.post1/soil/datacollection.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/debugging.py` & `soil-1.0.0rc5.post1/soil/debugging.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/environment.py` & `soil-1.0.0rc5.post1/soil/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
 import sqlite3
 import math
+import sys
 import logging
 import inspect
 
 from typing import Any, Callable, Dict, Optional, Union, List, Type
 from collections import namedtuple
 from time import time as current_time
 from copy import deepcopy
@@ -201,23 +202,26 @@
             self.logger.debug(f"--- Steps: {self.schedule.steps:^5} - Time: {self.now:^5} --- " + msg)
 
     def add_model_reporter(self, name, func=None):
         if not func:
             func = name
         self.datacollector._new_model_reporter(name, func)
 
-    def add_agent_reporter(self, name, reporter=None, agent_type=None):
-        if not reporter and not agent_type:
-            reporter = name
+    def add_agent_reporter(self, name, reporter=None, agent_class=None, *, agent_type=None):
         if agent_type:
+            print("agent_type is deprecated, use agent_class instead", file=sys.stderr)
+        agent_class = agent_type or agent_class
+        if not reporter and not agent_class:
+            reporter = name
+        if agent_class:
             if reporter:
                 _orig = reporter
             else:
                 _orig = lambda a: getattr(a, name)
-            reporter = lambda a: (_orig(a) if isinstance(a, agent_type) else None)
+            reporter = lambda a: (_orig(a) if isinstance(a, agent_class) else None)
         self.datacollector._new_agent_reporter(name, reporter)
 
     @classmethod
     def run(cls, *,
             name=None,
             iterations=1,
             num_processes=1, **kwargs):
```

### Comparing `soil-1.0.0rc5/soil/events.py` & `soil-1.0.0rc5.post1/soil/events.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/exporters.py` & `soil-1.0.0rc5.post1/soil/exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/network.py` & `soil-1.0.0rc5.post1/soil/network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/parameters.py` & `soil-1.0.0rc5.post1/soil/parameters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/serialization.py` & `soil-1.0.0rc5.post1/soil/serialization.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/simulation.py` & `soil-1.0.0rc5.post1/soil/simulation.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/time.py` & `soil-1.0.0rc5.post1/soil/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,18 @@
         return self.delta
     
     def __await__(self):
         return (yield self.delta)
 
 class When:
     def __init__(self, when):
-        raise Exception("The use of When is deprecated. Use Delay instead, or the `at` and `delay` methods of an agent")
+        raise Exception("The use of When is deprecated. Use the `Agent.at` and `Agent.delay` methods instead")
+class Delta:
+    def __init__(self, delta):
+        raise Exception("The use of Delay is deprecated. Use the `Agent.at` and `Agent.delay` methods instead")
 
 class DeadAgent(Exception):
     pass
 
 
 class PQueueActivation(BaseScheduler):
     """
```

### Comparing `soil-1.0.0rc5/soil/utils.py` & `soil-1.0.0rc5.post1/soil/utils.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/README.md` & `soil-1.0.0rc5.post1/soil/web/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/__init__.py` & `soil-1.0.0rc5.post1/soil/web/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/config.yml` & `soil-1.0.0rc5.post1/soil/web/config.yml`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/run.py` & `soil-1.0.0rc5.post1/soil/web/run.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/css/main.css` & `soil-1.0.0rc5.post1/soil/web/static/css/main.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/css/timeline.css` & `soil-1.0.0rc5.post1/soil/web/static/css/timeline.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/logo_gsi.svg` & `soil-1.0.0rc5.post1/soil/web/static/img/logo_gsi.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/logo_soil.png` & `soil-1.0.0rc5.post1/soil/web/static/img/logo_soil.png`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/svg/person.svg` & `soil-1.0.0rc5.post1/soil/web/static/img/svg/person.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/svg/plus.svg` & `soil-1.0.0rc5.post1/soil/web/static/img/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/svg/target.svg` & `soil-1.0.0rc5.post1/soil/web/static/img/svg/target.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/img/svg/time.svg` & `soil-1.0.0rc5.post1/soil/web/static/img/svg/time.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/js/socket.js` & `soil-1.0.0rc5.post1/soil/web/static/js/socket.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/js/template.js` & `soil-1.0.0rc5.post1/soil/web/static/js/template.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/js/timeline.js` & `soil-1.0.0rc5.post1/soil/web/static/js/timeline.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/static/js/visualization.js` & `soil-1.0.0rc5.post1/soil/web/static/js/visualization.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil/web/templates/index.html` & `soil-1.0.0rc5.post1/soil/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/soil.egg-info/PKG-INFO` & `soil-1.0.0rc5.post1/soil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc5
+Version: 1.0.0rc5.post1
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc5.post1.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `soil-1.0.0rc5/soil.egg-info/SOURCES.txt` & `soil-1.0.0rc5.post1/soil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_agents.py` & `soil-1.0.0rc5.post1/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_config.py` & `soil-1.0.0rc5.post1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_examples.py` & `soil-1.0.0rc5.post1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_exporters.py` & `soil-1.0.0rc5.post1/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_ipython.py` & `soil-1.0.0rc5.post1/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_main.py` & `soil-1.0.0rc5.post1/tests/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -223,7 +223,33 @@
         b = [3, 4]
         sim = simulation.Simulation(matrix=dict(a=a, b=b))
         configs = sim._collect_params()
         assert len(configs) == len(a) * len(b)
         for i in a:
             for j in b:
                 assert {"a": i, "b": j} in configs
+    
+    def test_agent_reporters(self):
+        """An environment should be able to set its own reporters"""
+        class Noop2(agents.Noop):
+            pass
+
+        e = Environment()
+        e.add_agent(agents.Noop)
+        e.add_agent(Noop2)
+        e.add_agent_reporter("now")
+        e.add_agent_reporter("base", lambda a: "base", agent_class=agents.Noop)
+        e.add_agent_reporter("subclass", lambda a:"subclass", agent_class=Noop2)
+        e.step()
+
+        # Step 0 is not present because we added the reporters
+        # after initialization.
+        df = e.agent_df()
+        assert "now" in df.columns
+        assert "base" in df.columns
+        assert "subclass" in df.columns
+        assert df["now"][(0,0)] == 1
+        assert df["now"][(0,1)] == 1
+        assert df["base"][(0,0)] == "base"
+        assert df["base"][(0,1)] == "base"
+        assert df["subclass"][(0,0)] is None
+        assert df["subclass"][(0,1)] == "subclass"
```

### Comparing `soil-1.0.0rc5/tests/test_mesa.py` & `soil-1.0.0rc5.post1/tests/test_mesa.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_network.py` & `soil-1.0.0rc5.post1/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc5/tests/test_time.py` & `soil-1.0.0rc5.post1/tests/test_time.py`

 * *Files identical despite different names*

